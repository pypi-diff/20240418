# Comparing `tmp/pykdtree-1.3.7.post0.tar.gz` & `tmp/pykdtree-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykdtree-1.3.7.post0.tar", last modified: Mon Mar 20 16:52:11 2023, max compression
+gzip compressed data, was "pykdtree-1.3.9.tar", last modified: Fri Sep 22 06:52:39 2023, max compression
```

## Comparing `pykdtree-1.3.7.post0.tar` & `pykdtree-1.3.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:52:11.733753 pykdtree-1.3.7.post0/
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-03-20 16:52:11.733753 pykdtree-1.3.7.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/README
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:52:11.733753 pykdtree-1.3.7.post0/pykdtree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/pykdtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/pykdtree/_kdtree_core.c
--rw-r--r--   0 runner    (1001) docker     (123)   420964 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/pykdtree/kdtree.c
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/pykdtree/kdtree.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/pykdtree/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:52:11.733753 pykdtree-1.3.7.post0/pykdtree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 16:52:11.000000 pykdtree-1.3.7.post0/pykdtree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-20 16:52:11.733753 pykdtree-1.3.7.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-20 16:52:00.000000 pykdtree-1.3.7.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:52:39.885298 pykdtree-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2023-09-22 06:52:27.000000 pykdtree-1.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-22 06:52:27.000000 pykdtree-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2023-09-22 06:52:39.885298 pykdtree-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2023-09-22 06:52:27.000000 pykdtree-1.3.9/README
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2023-09-22 06:52:27.000000 pykdtree-1.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:52:39.885298 pykdtree-1.3.9/pykdtree/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 06:52:27.000000 pykdtree-1.3.9/pykdtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46750 2023-09-22 06:52:27.000000 pykdtree-1.3.9/pykdtree/_kdtree_core.c
+-rw-r--r--   0 runner    (1001) docker     (127)   613086 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree/kdtree.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2023-09-22 06:52:27.000000 pykdtree-1.3.9/pykdtree/kdtree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2023-09-22 06:52:27.000000 pykdtree-1.3.9/pykdtree/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:52:39.885298 pykdtree-1.3.9/pykdtree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-22 06:52:39.000000 pykdtree-1.3.9/pykdtree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-09-22 06:52:27.000000 pykdtree-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-22 06:52:39.885298 pykdtree-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2023-09-22 06:52:27.000000 pykdtree-1.3.9/setup.py
```

### Comparing `pykdtree-1.3.7.post0/LICENSE.txt` & `pykdtree-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pykdtree-1.3.7.post0/PKG-INFO` & `pykdtree-1.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pykdtree
-Version: 1.3.7.post0
+Version: 1.3.9
 Summary: Fast kd-tree implementation with OpenMP-enabled queries
 Home-page: https://github.com/storpipfugl/pykdtree
 Author: Esben S. Nielsen
 Author-email: storpipfugl@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE.txt
+Requires-Dist: numpy
 
 .. image:: https://github.com/storpipfugl/pykdtree/actions/workflows/deploy-wheels.yml/badge.svg?branch=master
     :target: https://github.com/storpipfugl/pykdtree/actions/workflows/deploy-wheels.yml
 
 ========
 pykdtree
 ========
@@ -195,41 +196,7 @@
 turned off by adding the following to `appveyor.yml` in the
 `environment` section:
 
     environment:
       global:
         # Don't build with openmp because it isn't supported in appveyor's compilers
         USE_OMP: "0"
-
-Changelog
----------
-v1.3.6 : Fix Python 3.11 compatibility and build Python 3.11 wheels
-
-v1.3.5 : Build Python 3.10 wheels and other CI updates
-
-v1.3.4 : Fix Python 3.9 wheels not being built for linux
-
-v1.3.3 : Add compatibility to python 3.9
-
-v1.3.2 : Change OSX installation to not use OpenMP without conda interpreter
-
-v1.3.1 : Fix masking in the "query" method introduced in 1.3.0
-
-v1.3.0 : Keyword argument "mask" added to "query" method. OpenMP compilation now works for MS Visual Studio compiler
-
-v1.2.2 : Build process fixes
-
-v1.2.1 : Fixed OpenMP thread safety issue introduced in v1.2.0
-
-v1.2.0 : 64 and 32 bit MSVC Windows support added
-
-v1.1.1 : Same as v1.1 release due to incorrect pypi release
-
-v1.1 : Build process improvements. Add data attribute to kdtree class for scipy interface compatibility
-
-v1.0 : Switched license from GPLv3 to LGPLv3
-
-v0.3 : Avoid zipping of installed egg
-
-v0.2 : Reduced memory footprint. Can now handle single precision data internally avoiding copy conversion to double precision. Default leafsize changed from 10 to 16 as this reduces the memory footprint and makes it a cache line multiplum (negligible if any query performance observed in benchmarks). Reduced memory allocation for leaf nodes. Applied patch for building on OS X.
-
-v0.1 : Initial version.
```

### Comparing `pykdtree-1.3.7.post0/README` & `pykdtree-1.3.9/pykdtree.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pykdtree
+Version: 1.3.9
+Summary: Fast kd-tree implementation with OpenMP-enabled queries
+Home-page: https://github.com/storpipfugl/pykdtree
+Author: Esben S. Nielsen
+Author-email: storpipfugl@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+License-File: LICENSE.txt
+Requires-Dist: numpy
+
 .. image:: https://github.com/storpipfugl/pykdtree/actions/workflows/deploy-wheels.yml/badge.svg?branch=master
     :target: https://github.com/storpipfugl/pykdtree/actions/workflows/deploy-wheels.yml
 
 ========
 pykdtree
 ========
 
@@ -179,41 +196,7 @@
 turned off by adding the following to `appveyor.yml` in the
 `environment` section:
 
     environment:
       global:
         # Don't build with openmp because it isn't supported in appveyor's compilers
         USE_OMP: "0"
-
-Changelog
----------
-v1.3.6 : Fix Python 3.11 compatibility and build Python 3.11 wheels
-
-v1.3.5 : Build Python 3.10 wheels and other CI updates
-
-v1.3.4 : Fix Python 3.9 wheels not being built for linux
-
-v1.3.3 : Add compatibility to python 3.9
-
-v1.3.2 : Change OSX installation to not use OpenMP without conda interpreter
-
-v1.3.1 : Fix masking in the "query" method introduced in 1.3.0
-
-v1.3.0 : Keyword argument "mask" added to "query" method. OpenMP compilation now works for MS Visual Studio compiler
-
-v1.2.2 : Build process fixes
-
-v1.2.1 : Fixed OpenMP thread safety issue introduced in v1.2.0
-
-v1.2.0 : 64 and 32 bit MSVC Windows support added
-
-v1.1.1 : Same as v1.1 release due to incorrect pypi release
-
-v1.1 : Build process improvements. Add data attribute to kdtree class for scipy interface compatibility
-
-v1.0 : Switched license from GPLv3 to LGPLv3
-
-v0.3 : Avoid zipping of installed egg
-
-v0.2 : Reduced memory footprint. Can now handle single precision data internally avoiding copy conversion to double precision. Default leafsize changed from 10 to 16 as this reduces the memory footprint and makes it a cache line multiplum (negligible if any query performance observed in benchmarks). Reduced memory allocation for leaf nodes. Applied patch for building on OS X.
-
-v0.1 : Initial version.
```

### Comparing `pykdtree-1.3.7.post0/README.rst` & `pykdtree-1.3.9/README`

 * *Files 16% similar despite different names*

```diff
@@ -179,41 +179,7 @@
 turned off by adding the following to `appveyor.yml` in the
 `environment` section:
 
     environment:
       global:
         # Don't build with openmp because it isn't supported in appveyor's compilers
         USE_OMP: "0"
-
-Changelog
----------
-v1.3.6 : Fix Python 3.11 compatibility and build Python 3.11 wheels
-
-v1.3.5 : Build Python 3.10 wheels and other CI updates
-
-v1.3.4 : Fix Python 3.9 wheels not being built for linux
-
-v1.3.3 : Add compatibility to python 3.9
-
-v1.3.2 : Change OSX installation to not use OpenMP without conda interpreter
-
-v1.3.1 : Fix masking in the "query" method introduced in 1.3.0
-
-v1.3.0 : Keyword argument "mask" added to "query" method. OpenMP compilation now works for MS Visual Studio compiler
-
-v1.2.2 : Build process fixes
-
-v1.2.1 : Fixed OpenMP thread safety issue introduced in v1.2.0
-
-v1.2.0 : 64 and 32 bit MSVC Windows support added
-
-v1.1.1 : Same as v1.1 release due to incorrect pypi release
-
-v1.1 : Build process improvements. Add data attribute to kdtree class for scipy interface compatibility
-
-v1.0 : Switched license from GPLv3 to LGPLv3
-
-v0.3 : Avoid zipping of installed egg
-
-v0.2 : Reduced memory footprint. Can now handle single precision data internally avoiding copy conversion to double precision. Default leafsize changed from 10 to 16 as this reduces the memory footprint and makes it a cache line multiplum (negligible if any query performance observed in benchmarks). Reduced memory allocation for leaf nodes. Applied patch for building on OS X.
-
-v0.1 : Initial version.
```

### Comparing `pykdtree-1.3.7.post0/pykdtree/_kdtree_core.c` & `pykdtree-1.3.9/pykdtree/_kdtree_core.c`

 * *Files identical despite different names*

### Comparing `pykdtree-1.3.7.post0/pykdtree/kdtree.c` & `pykdtree-1.3.9/pykdtree/kdtree.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,66 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 3.0.2 */
+
+/* BEGIN: Cython Metadata
+{
+    "distutils": {
+        "depends": [
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+        ],
+        "include_dirs": [
+            "/tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/core/include"
+        ],
+        "name": "pykdtree.kdtree",
+        "sources": [
+            "pykdtree/kdtree.pyx",
+            "pykdtree/_kdtree_core.c"
+        ]
+    },
+    "module_name": "pykdtree.kdtree"
+}
+END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#if CYTHON_LIMITED_API
+#define __PYX_EXTRA_ABI_MODULE_NAME "limited"
+#else
+#define __PYX_EXTRA_ABI_MODULE_NAME ""
+#endif
+#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030002F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -31,31 +71,35 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#define __PYX_LIMITED_VERSION_HEX PY_VERSION_HEX
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -72,76 +116,163 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PYSTON_VERSION)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
+  #ifdef Py_LIMITED_API
+    #undef __PYX_LIMITED_VERSION_HEX
+    #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
   #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
   #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
@@ -177,36 +308,34 @@
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
@@ -222,45 +351,67 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
+  #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -282,78 +433,136 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
+#ifndef CYTHON_USE_CPP_STD_MOVE
+  #if defined(__cplusplus) && (\
+    __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600))
+    #define CYTHON_USE_CPP_STD_MOVE 1
+  #else
+    #define CYTHON_USE_CPP_STD_MOVE 0
+  #endif
+#endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -361,152 +570,255 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+#if CYTHON_COMPILING_IN_LIMITED_API
+    static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyObject *exception_table = NULL;
+        PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        PyObject *version_info; // borrowed
+        PyObject *py_minor_version = NULL;
+        long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
+        #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
+        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        #else
+        if (!(version_info = PySys_GetObject("version_info"))) goto end;
+        if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
+        minor_version = PyLong_AsLong(py_minor_version);
+        if (minor_version == -1 && PyErr_Occurred()) goto end;
+        #endif
+        if (!(types_module = PyImport_ImportModule("types"))) goto end;
+        if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
+        if (minor_version <= 7) {
+            (void)p;
+            result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else if (minor_version <= 10) {
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else {
+            if (!(exception_table = PyBytes_FromStringAndSize(NULL, 0))) goto end;
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
+        }
+    end:
+        Py_XDECREF(code_type);
+        Py_XDECREF(exception_table);
+        Py_XDECREF(types_module);
+        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
+    #ifndef CO_OPTIMIZED
+    #define CO_OPTIMIZED 0x0001
+    #endif
+    #ifndef CO_NEWLOCALS
+    #define CO_NEWLOCALS 0x0002
+    #endif
+    #ifndef CO_VARARGS
+    #define CO_VARARGS 0x0004
+    #endif
+    #ifndef CO_VARKEYWORDS
+    #define CO_VARKEYWORDS 0x0008
+    #endif
+    #ifndef CO_ASYNC_GENERATOR
+    #define CO_ASYNC_GENERATOR 0x0200
+    #endif
+    #ifndef CO_GENERATOR
+    #define CO_GENERATOR 0x0020
+    #endif
+    #ifndef CO_COROUTINE
+    #define CO_COROUTINE 0x0080
+    #endif
+#elif PY_VERSION_HEX >= 0x030B0000
+  static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+    PyCodeObject *result;
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    if (!empty_bytes) return NULL;
+    result =
+      #if PY_VERSION_HEX >= 0x030C0000
+        PyUnstable_Code_NewWithPosOnlyArgs
+      #else
+        PyCode_NewWithPosOnlyArgs
+      #endif
+        (a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, name, fline, lnos, empty_bytes);
+    Py_DECREF(empty_bytes);
+    return result;
+  }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if __PYX_LIMITED_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -529,86 +841,171 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
   #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+  #define CYTHON_PEP393_ENABLED 1
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -629,45 +1026,72 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_ITEM(o, i)
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) (PyTuple_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyList_SET_ITEM(o, i, v) (PyList_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_GET_SIZE(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_GET_SIZE(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_GET_SIZE(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_GET_SIZE(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_GET_SIZE(o)
 #else
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_GetItem(o, i)
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) PyTuple_SetItem(o, i, v)
+  #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -677,19 +1101,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -726,35 +1145,44 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__pykdtree__kdtree
 #define __PYX_HAVE_API__pykdtree__kdtree
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
+
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
+    
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
-
-    /* NumPy API declarations from "numpy/__init__.pxd" */
-    
 #include <stdint.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -816,29 +1244,40 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -856,15 +1295,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -878,15 +1362,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -943,31 +1427,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -977,23 +1457,24 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "pykdtree/kdtree.pyx",
-  "stringsource",
-  "__init__.pxd",
+  "__init__.cython-30.pxd",
+  "<stringsource>",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -1032,259 +1513,244 @@
 #define __Pyx_FastGilFuncInit()
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":718
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8pykdtree_6kdtree_KDTree;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1373,138 +1839,132 @@
   float *_data_pts_data_float;
   double *_data_pts_data_double;
   uint32_t n;
   int8_t ndim;
   uint32_t leafsize;
 };
 
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
-/* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
-
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
-
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
-
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1512,17 +1972,142 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_VARARGS(args, i) PySequence_GetItem(args, i)
+#elif CYTHON_ASSUME_SAFE_MACROS
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#else
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
+#else
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+#endif
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg) __Pyx_Arg_XDECREF_VARARGS(arg)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
+    const char* function_name);
+
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1543,85 +2128,76 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
+#endif
+#endif
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
@@ -1642,104 +2218,248 @@
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
 /* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
+#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_2 {
+   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+#else
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
+#endif
+
+/* PyMethodNew.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    typesModule = PyImport_ImportModule("types");
+    if (!typesModule) return NULL;
+    methodType = PyObject_GetAttrString(typesModule, "MethodType");
+    Py_DECREF(typesModule);
+    if (!methodType) return NULL;
+    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
+    Py_DECREF(methodType);
+    return result;
+}
+#elif PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject_HEAD
+    PyObject *func;
+#elif PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1761,15 +2481,15 @@
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
@@ -1788,15 +2508,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1826,15 +2546,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1875,247 +2595,2205 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int8_t(int8_t value);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cpython.buffer' */
-
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
+/* Module declarations from "libc.stdint" */
 
-/* Module declarations from 'libc.stdint' */
+/* Module declarations from "cython" */
 
-/* Module declarations from 'cython' */
-
-/* Module declarations from 'pykdtree.kdtree' */
-static PyTypeObject *__pyx_ptype_8pykdtree_6kdtree_KDTree = 0;
+/* Module declarations from "pykdtree.kdtree" */
 __PYX_EXTERN_C DL_IMPORT(struct __pyx_t_8pykdtree_6kdtree_tree_float) *construct_tree_float(float *, int8_t, uint32_t, uint32_t); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) search_tree_float(struct __pyx_t_8pykdtree_6kdtree_tree_float *, float *, float *, uint32_t, uint32_t, float, float, uint8_t *, uint32_t *, float *); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) delete_tree_float(struct __pyx_t_8pykdtree_6kdtree_tree_float *); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(struct __pyx_t_8pykdtree_6kdtree_tree_double) *construct_tree_double(double *, int8_t, uint32_t, uint32_t); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) search_tree_double(struct __pyx_t_8pykdtree_6kdtree_tree_double *, double *, double *, uint32_t, uint32_t, double, double, uint8_t *, uint32_t *, double *); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) delete_tree_double(struct __pyx_t_8pykdtree_6kdtree_tree_double *); /*proto*/
+/* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_float = { "float", NULL, sizeof(float), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint32_t = { "uint32_t", NULL, sizeof(uint32_t), { 0 }, 0, IS_UNSIGNED(uint32_t) ? 'U' : 'I', IS_UNSIGNED(uint32_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t = { "uint8_t", NULL, sizeof(__pyx_t_5numpy_uint8_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_uint8_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_uint8_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint32_t = { "uint32_t", NULL, sizeof(uint32_t), { 0 }, 0, __PYX_IS_UNSIGNED(uint32_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(uint32_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t = { "uint8_t", NULL, sizeof(__pyx_t_5numpy_uint8_t), { 0 }, 0, __PYX_IS_UNSIGNED(__pyx_t_5numpy_uint8_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(__pyx_t_5numpy_uint8_t), 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "pykdtree.kdtree"
 extern int __pyx_module_is_main_pykdtree__kdtree;
 int __pyx_module_is_main_pykdtree__kdtree = 0;
 
-/* Implementation of 'pykdtree.kdtree' */
+/* Implementation of "pykdtree.kdtree" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_k[] = "k";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k_Inf[] = "Inf";
+static const char __pyx_k__11[] = "*";
+static const char __pyx_k__19[] = "?";
 static const char __pyx_k_eps[] = "eps";
+static const char __pyx_k_inf[] = "inf";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mask[] = "mask";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_self[] = "self";
 static const char __pyx_k_size[] = "size";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_sqrt[] = "sqrt";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_finfo[] = "finfo";
+static const char __pyx_k_num_n[] = "num_n";
 static const char __pyx_k_numpy[] = "numpy";
+static const char __pyx_k_query[] = "query";
 static const char __pyx_k_ravel[] = "ravel";
 static const char __pyx_k_uint8[] = "uint8";
 static const char __pyx_k_KDTree[] = "KDTree";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_q_ndim[] = "q_ndim";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_uint32[] = "uint32";
+static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float32[] = "float32";
 static const char __pyx_k_float64[] = "float64";
+static const char __pyx_k_idx_out[] = "idx_out";
 static const char __pyx_k_reshape[] = "reshape";
 static const char __pyx_k_data_pts[] = "data_pts";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_leafsize[] = "leafsize";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
+static const char __pyx_k_dub_float[] = "dub_float";
+static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_query_pts[] = "query_pts";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_sqr_dists[] = "sqr_dists";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_dub_double[] = "dub_double";
+static const char __pyx_k_query_mask[] = "query_mask";
 static const char __pyx_k_ImportError[] = "ImportError";
+static const char __pyx_k_num_qpoints[] = "num_qpoints";
+static const char __pyx_k_KDTree_query[] = "KDTree.query";
+static const char __pyx_k_closest_idxs[] = "closest_idxs";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_stringsource[] = "<stringsource>";
+static const char __pyx_k_closest_dists[] = "closest_dists";
+static const char __pyx_k_epsilon_float[] = "epsilon_float";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_epsilon_double[] = "epsilon_double";
+static const char __pyx_k_pykdtree_kdtree[] = "pykdtree.kdtree";
+static const char __pyx_k_query_mask_data[] = "query_mask_data";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_closest_idxs_res[] = "closest_idxs_res";
 static const char __pyx_k_ascontiguousarray[] = "ascontiguousarray";
+static const char __pyx_k_closest_dists_res[] = "closest_dists_res";
+static const char __pyx_k_closest_idxs_data[] = "closest_idxs_data";
+static const char __pyx_k_query_array_float[] = "query_array_float";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_query_array_double[] = "query_array_double";
+static const char __pyx_k_closest_dists_float[] = "closest_dists_float";
+static const char __pyx_k_pykdtree_kdtree_pyx[] = "pykdtree/kdtree.pyx";
+static const char __pyx_k_closest_dists_double[] = "closest_dists_double";
 static const char __pyx_k_distance_upper_bound[] = "distance_upper_bound";
+static const char __pyx_k_KDTree___reduce_cython[] = "KDTree.__reduce_cython__";
+static const char __pyx_k_query_array_data_float[] = "query_array_data_float";
+static const char __pyx_k_query_array_data_double[] = "query_array_data_double";
+static const char __pyx_k_KDTree___setstate_cython[] = "KDTree.__setstate_cython__";
+static const char __pyx_k_closest_dists_data_float[] = "closest_dists_data_float";
 static const char __pyx_k_eps_must_be_non_negative[] = "eps must be non-negative";
+static const char __pyx_k_closest_dists_data_double[] = "closest_dists_data_double";
 static const char __pyx_k_Max_127_dimensions_allowed[] = "Max 127 dimensions allowed";
 static const char __pyx_k_Data_and_query_points_must_have[] = "Data and query points must have same dimensions";
 static const char __pyx_k_Mask_must_have_the_same_size_as[] = "Mask must have the same size as data points";
 static const char __pyx_k_Type_mismatch_query_points_must[] = "Type mismatch. query points must be of type float32 when data points are of type float32";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Number_of_neighbours_must_be_gre[] = "Number of neighbours must be greater than zero";
 static const char __pyx_k_distance_upper_bound_must_be_non[] = "distance_upper_bound must be non negative";
 static const char __pyx_k_leafsize_must_be_greater_than_ze[] = "leafsize must be greater than zero";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static PyObject *__pyx_kp_u_Data_and_query_points_must_have;
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_Inf;
-static PyObject *__pyx_n_s_KDTree;
-static PyObject *__pyx_kp_u_Mask_must_have_the_same_size_as;
-static PyObject *__pyx_kp_u_Max_127_dimensions_allowed;
-static PyObject *__pyx_kp_u_Number_of_neighbours_must_be_gre;
-static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_kp_u_Type_mismatch_query_points_must;
-static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_n_s_ascontiguousarray;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_data_pts;
-static PyObject *__pyx_n_s_distance_upper_bound;
-static PyObject *__pyx_kp_u_distance_upper_bound_must_be_non;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_empty;
-static PyObject *__pyx_n_s_eps;
-static PyObject *__pyx_kp_u_eps_must_be_non_negative;
-static PyObject *__pyx_n_s_finfo;
-static PyObject *__pyx_n_s_float32;
-static PyObject *__pyx_n_s_float64;
-static PyObject *__pyx_n_s_getstate;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_k;
-static PyObject *__pyx_n_s_leafsize;
-static PyObject *__pyx_kp_u_leafsize_must_be_greater_than_ze;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_mask;
-static PyObject *__pyx_n_s_max;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_query_pts;
-static PyObject *__pyx_n_s_ravel;
-static PyObject *__pyx_n_s_reduce;
-static PyObject *__pyx_n_s_reduce_cython;
-static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_reshape;
-static PyObject *__pyx_n_s_setstate;
-static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_size;
-static PyObject *__pyx_n_s_sqr_dists;
-static PyObject *__pyx_n_s_sqrt;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_uint32;
-static PyObject *__pyx_n_s_uint8;
+/* #### Code section: decls ### */
 static int __pyx_pf_8pykdtree_6kdtree_6KDTree___cinit__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static int __pyx_pf_8pykdtree_6kdtree_6KDTree_2__init__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, PyArrayObject *__pyx_v_data_pts, int __pyx_v_leafsize); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_4query(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, PyArrayObject *__pyx_v_query_pts, PyObject *__pyx_v_k, PyObject *__pyx_v_eps, PyObject *__pyx_v_distance_upper_bound, PyObject *__pyx_v_sqr_dists, PyObject *__pyx_v_mask); /* proto */
 static void __pyx_pf_8pykdtree_6kdtree_6KDTree_6__dealloc__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_8data_pts___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_4data___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_1n___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_4ndim___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_8leafsize___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8pykdtree_6kdtree_KDTree(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_1;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__12;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_8pykdtree_6kdtree_KDTree;
+  #endif
+  PyTypeObject *__pyx_ptype_8pykdtree_6kdtree_KDTree;
+  PyObject *__pyx_kp_s_Data_and_query_points_must_have;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s_KDTree;
+  PyObject *__pyx_n_s_KDTree___reduce_cython;
+  PyObject *__pyx_n_s_KDTree___setstate_cython;
+  PyObject *__pyx_n_s_KDTree_query;
+  PyObject *__pyx_kp_s_Mask_must_have_the_same_size_as;
+  PyObject *__pyx_kp_s_Max_127_dimensions_allowed;
+  PyObject *__pyx_kp_s_Number_of_neighbours_must_be_gre;
+  PyObject *__pyx_n_s_TypeError;
+  PyObject *__pyx_kp_s_Type_mismatch_query_points_must;
+  PyObject *__pyx_n_s_ValueError;
+  PyObject *__pyx_n_s__11;
+  PyObject *__pyx_n_s__19;
+  PyObject *__pyx_n_s_ascontiguousarray;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_closest_dists;
+  PyObject *__pyx_n_s_closest_dists_data_double;
+  PyObject *__pyx_n_s_closest_dists_data_float;
+  PyObject *__pyx_n_s_closest_dists_double;
+  PyObject *__pyx_n_s_closest_dists_float;
+  PyObject *__pyx_n_s_closest_dists_res;
+  PyObject *__pyx_n_s_closest_idxs;
+  PyObject *__pyx_n_s_closest_idxs_data;
+  PyObject *__pyx_n_s_closest_idxs_res;
+  PyObject *__pyx_n_s_data_pts;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_distance_upper_bound;
+  PyObject *__pyx_kp_s_distance_upper_bound_must_be_non;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_dub_double;
+  PyObject *__pyx_n_s_dub_float;
+  PyObject *__pyx_n_s_empty;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_eps;
+  PyObject *__pyx_kp_s_eps_must_be_non_negative;
+  PyObject *__pyx_n_s_epsilon_double;
+  PyObject *__pyx_n_s_epsilon_float;
+  PyObject *__pyx_n_s_finfo;
+  PyObject *__pyx_n_s_float32;
+  PyObject *__pyx_n_s_float64;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_n_s_idx_out;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_inf;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_k;
+  PyObject *__pyx_n_s_leafsize;
+  PyObject *__pyx_kp_s_leafsize_must_be_greater_than_ze;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_mask;
+  PyObject *__pyx_n_s_max;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_num_n;
+  PyObject *__pyx_n_s_num_qpoints;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_pykdtree_kdtree;
+  PyObject *__pyx_kp_s_pykdtree_kdtree_pyx;
+  PyObject *__pyx_n_s_pyx_state;
+  PyObject *__pyx_n_s_q_ndim;
+  PyObject *__pyx_n_s_query;
+  PyObject *__pyx_n_s_query_array_data_double;
+  PyObject *__pyx_n_s_query_array_data_float;
+  PyObject *__pyx_n_s_query_array_double;
+  PyObject *__pyx_n_s_query_array_float;
+  PyObject *__pyx_n_s_query_mask;
+  PyObject *__pyx_n_s_query_mask_data;
+  PyObject *__pyx_n_s_query_pts;
+  PyObject *__pyx_n_s_ravel;
+  PyObject *__pyx_n_s_reduce;
+  PyObject *__pyx_n_s_reduce_cython;
+  PyObject *__pyx_n_s_reduce_ex;
+  PyObject *__pyx_n_s_reshape;
+  PyObject *__pyx_n_s_self;
+  PyObject *__pyx_n_s_setstate;
+  PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_size;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_sqr_dists;
+  PyObject *__pyx_n_s_sqrt;
+  PyObject *__pyx_kp_s_stringsource;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_uint32;
+  PyObject *__pyx_n_s_uint8;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_int_1;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_tuple__12;
+  PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__15;
+  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__18;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_ptype_8pykdtree_6kdtree_KDTree);
+  Py_CLEAR(clear_module_state->__pyx_type_8pykdtree_6kdtree_KDTree);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Data_and_query_points_must_have);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_KDTree);
+  Py_CLEAR(clear_module_state->__pyx_n_s_KDTree___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_KDTree___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_KDTree_query);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Mask_must_have_the_same_size_as);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Max_127_dimensions_allowed);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Number_of_neighbours_must_be_gre);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Type_mismatch_query_points_must);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__11);
+  Py_CLEAR(clear_module_state->__pyx_n_s__19);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ascontiguousarray);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists_data_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists_data_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_dists_res);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_idxs);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_idxs_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_closest_idxs_res);
+  Py_CLEAR(clear_module_state->__pyx_n_s_data_pts);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_distance_upper_bound);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_distance_upper_bound_must_be_non);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dub_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dub_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_empty);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_eps);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_eps_must_be_non_negative);
+  Py_CLEAR(clear_module_state->__pyx_n_s_epsilon_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_epsilon_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_finfo);
+  Py_CLEAR(clear_module_state->__pyx_n_s_float32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_float64);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_idx_out);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_inf);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_k);
+  Py_CLEAR(clear_module_state->__pyx_n_s_leafsize);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_leafsize_must_be_greater_than_ze);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_mask);
+  Py_CLEAR(clear_module_state->__pyx_n_s_max);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_num_n);
+  Py_CLEAR(clear_module_state->__pyx_n_s_num_qpoints);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pykdtree_kdtree);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_pykdtree_kdtree_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_q_ndim);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_array_data_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_array_data_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_array_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_array_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_mask);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_mask_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_pts);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ravel);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reshape);
+  Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_size);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sqr_dists);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sqrt);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_uint32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_uint8);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__12);
+  Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__15);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__18);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_ptype_8pykdtree_6kdtree_KDTree);
+  Py_VISIT(traverse_module_state->__pyx_type_8pykdtree_6kdtree_KDTree);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Data_and_query_points_must_have);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_KDTree);
+  Py_VISIT(traverse_module_state->__pyx_n_s_KDTree___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_KDTree___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_KDTree_query);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Mask_must_have_the_same_size_as);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Max_127_dimensions_allowed);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Number_of_neighbours_must_be_gre);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Type_mismatch_query_points_must);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__11);
+  Py_VISIT(traverse_module_state->__pyx_n_s__19);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ascontiguousarray);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists_data_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists_data_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_dists_res);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_idxs);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_idxs_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_closest_idxs_res);
+  Py_VISIT(traverse_module_state->__pyx_n_s_data_pts);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_distance_upper_bound);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_distance_upper_bound_must_be_non);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dub_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dub_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_empty);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_eps);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_eps_must_be_non_negative);
+  Py_VISIT(traverse_module_state->__pyx_n_s_epsilon_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_epsilon_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_finfo);
+  Py_VISIT(traverse_module_state->__pyx_n_s_float32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_float64);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_idx_out);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_inf);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_k);
+  Py_VISIT(traverse_module_state->__pyx_n_s_leafsize);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_leafsize_must_be_greater_than_ze);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_mask);
+  Py_VISIT(traverse_module_state->__pyx_n_s_max);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_num_n);
+  Py_VISIT(traverse_module_state->__pyx_n_s_num_qpoints);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pykdtree_kdtree);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_pykdtree_kdtree_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_q_ndim);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_array_data_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_array_data_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_array_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_array_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_mask);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_mask_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_pts);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ravel);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reshape);
+  Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_size);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sqr_dists);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sqrt);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_uint32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_uint8);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__12);
+  Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__15);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__18);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_8pykdtree_6kdtree_KDTree __pyx_mstate_global->__pyx_type_8pykdtree_6kdtree_KDTree
+#endif
+#define __pyx_ptype_8pykdtree_6kdtree_KDTree __pyx_mstate_global->__pyx_ptype_8pykdtree_6kdtree_KDTree
+#define __pyx_kp_s_Data_and_query_points_must_have __pyx_mstate_global->__pyx_kp_s_Data_and_query_points_must_have
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s_KDTree __pyx_mstate_global->__pyx_n_s_KDTree
+#define __pyx_n_s_KDTree___reduce_cython __pyx_mstate_global->__pyx_n_s_KDTree___reduce_cython
+#define __pyx_n_s_KDTree___setstate_cython __pyx_mstate_global->__pyx_n_s_KDTree___setstate_cython
+#define __pyx_n_s_KDTree_query __pyx_mstate_global->__pyx_n_s_KDTree_query
+#define __pyx_kp_s_Mask_must_have_the_same_size_as __pyx_mstate_global->__pyx_kp_s_Mask_must_have_the_same_size_as
+#define __pyx_kp_s_Max_127_dimensions_allowed __pyx_mstate_global->__pyx_kp_s_Max_127_dimensions_allowed
+#define __pyx_kp_s_Number_of_neighbours_must_be_gre __pyx_mstate_global->__pyx_kp_s_Number_of_neighbours_must_be_gre
+#define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
+#define __pyx_kp_s_Type_mismatch_query_points_must __pyx_mstate_global->__pyx_kp_s_Type_mismatch_query_points_must
+#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
+#define __pyx_n_s__11 __pyx_mstate_global->__pyx_n_s__11
+#define __pyx_n_s__19 __pyx_mstate_global->__pyx_n_s__19
+#define __pyx_n_s_ascontiguousarray __pyx_mstate_global->__pyx_n_s_ascontiguousarray
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_closest_dists __pyx_mstate_global->__pyx_n_s_closest_dists
+#define __pyx_n_s_closest_dists_data_double __pyx_mstate_global->__pyx_n_s_closest_dists_data_double
+#define __pyx_n_s_closest_dists_data_float __pyx_mstate_global->__pyx_n_s_closest_dists_data_float
+#define __pyx_n_s_closest_dists_double __pyx_mstate_global->__pyx_n_s_closest_dists_double
+#define __pyx_n_s_closest_dists_float __pyx_mstate_global->__pyx_n_s_closest_dists_float
+#define __pyx_n_s_closest_dists_res __pyx_mstate_global->__pyx_n_s_closest_dists_res
+#define __pyx_n_s_closest_idxs __pyx_mstate_global->__pyx_n_s_closest_idxs
+#define __pyx_n_s_closest_idxs_data __pyx_mstate_global->__pyx_n_s_closest_idxs_data
+#define __pyx_n_s_closest_idxs_res __pyx_mstate_global->__pyx_n_s_closest_idxs_res
+#define __pyx_n_s_data_pts __pyx_mstate_global->__pyx_n_s_data_pts
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_distance_upper_bound __pyx_mstate_global->__pyx_n_s_distance_upper_bound
+#define __pyx_kp_s_distance_upper_bound_must_be_non __pyx_mstate_global->__pyx_kp_s_distance_upper_bound_must_be_non
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_dub_double __pyx_mstate_global->__pyx_n_s_dub_double
+#define __pyx_n_s_dub_float __pyx_mstate_global->__pyx_n_s_dub_float
+#define __pyx_n_s_empty __pyx_mstate_global->__pyx_n_s_empty
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_eps __pyx_mstate_global->__pyx_n_s_eps
+#define __pyx_kp_s_eps_must_be_non_negative __pyx_mstate_global->__pyx_kp_s_eps_must_be_non_negative
+#define __pyx_n_s_epsilon_double __pyx_mstate_global->__pyx_n_s_epsilon_double
+#define __pyx_n_s_epsilon_float __pyx_mstate_global->__pyx_n_s_epsilon_float
+#define __pyx_n_s_finfo __pyx_mstate_global->__pyx_n_s_finfo
+#define __pyx_n_s_float32 __pyx_mstate_global->__pyx_n_s_float32
+#define __pyx_n_s_float64 __pyx_mstate_global->__pyx_n_s_float64
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_n_s_idx_out __pyx_mstate_global->__pyx_n_s_idx_out
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_inf __pyx_mstate_global->__pyx_n_s_inf
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
+#define __pyx_n_s_leafsize __pyx_mstate_global->__pyx_n_s_leafsize
+#define __pyx_kp_s_leafsize_must_be_greater_than_ze __pyx_mstate_global->__pyx_kp_s_leafsize_must_be_greater_than_ze
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_mask __pyx_mstate_global->__pyx_n_s_mask
+#define __pyx_n_s_max __pyx_mstate_global->__pyx_n_s_max
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_num_n __pyx_mstate_global->__pyx_n_s_num_n
+#define __pyx_n_s_num_qpoints __pyx_mstate_global->__pyx_n_s_num_qpoints
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_s_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_s_numpy_core_multiarray_failed_to
+#define __pyx_kp_s_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_s_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_pykdtree_kdtree __pyx_mstate_global->__pyx_n_s_pykdtree_kdtree
+#define __pyx_kp_s_pykdtree_kdtree_pyx __pyx_mstate_global->__pyx_kp_s_pykdtree_kdtree_pyx
+#define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
+#define __pyx_n_s_q_ndim __pyx_mstate_global->__pyx_n_s_q_ndim
+#define __pyx_n_s_query __pyx_mstate_global->__pyx_n_s_query
+#define __pyx_n_s_query_array_data_double __pyx_mstate_global->__pyx_n_s_query_array_data_double
+#define __pyx_n_s_query_array_data_float __pyx_mstate_global->__pyx_n_s_query_array_data_float
+#define __pyx_n_s_query_array_double __pyx_mstate_global->__pyx_n_s_query_array_double
+#define __pyx_n_s_query_array_float __pyx_mstate_global->__pyx_n_s_query_array_float
+#define __pyx_n_s_query_mask __pyx_mstate_global->__pyx_n_s_query_mask
+#define __pyx_n_s_query_mask_data __pyx_mstate_global->__pyx_n_s_query_mask_data
+#define __pyx_n_s_query_pts __pyx_mstate_global->__pyx_n_s_query_pts
+#define __pyx_n_s_ravel __pyx_mstate_global->__pyx_n_s_ravel
+#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
+#define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
+#define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
+#define __pyx_n_s_reshape __pyx_mstate_global->__pyx_n_s_reshape
+#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
+#define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_sqr_dists __pyx_mstate_global->__pyx_n_s_sqr_dists
+#define __pyx_n_s_sqrt __pyx_mstate_global->__pyx_n_s_sqrt
+#define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_uint32 __pyx_mstate_global->__pyx_n_s_uint32
+#define __pyx_n_s_uint8 __pyx_mstate_global->__pyx_n_s_uint8
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
+#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
+/* #### Code section: module_code ### */
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
+ * 
+ *     ctypedef unsigned char      npy_bool
+ */
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):
+ *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_array_base", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ */
+  Py_INCREF(__pyx_v_base);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ */
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 969, __pyx_L1_error)
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("get_array_base", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
+ *         return None
+ */
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = (__pyx_v_base == NULL);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ *         return None             # <<<<<<<<<<<<<<
+ *     return <object>base
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+ *     if base is NULL:
+ *         return None
+ *     return <object>base             # <<<<<<<<<<<<<<
+ * 
+ * # Versions of the import_* functions which are more suitable for
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_array", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+ * cdef inline int import_array() except -1:
+ *     try:
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ */
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 981, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+ *     try:
+ *         __pyx_import_array()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 982, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 983, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_umath", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+ * cdef inline int import_umath() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 987, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 989, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_ufunc", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+ * cdef inline int import_ufunc() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 993, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 995, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
 /* "pykdtree/kdtree.pyx":87
  *     cdef readonly uint32_t leafsize
  * 
  *     def __cinit__(KDTree self):             # <<<<<<<<<<<<<<
  *         self._kdtree_float = NULL
  *         self._kdtree_double = NULL
  */
 
 /* Python wrapper */
 static int __pyx_pw_8pykdtree_6kdtree_6KDTree_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8pykdtree_6kdtree_6KDTree_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
-  if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
-  if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 87, __pyx_L3_error)
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return -1;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree___cinit__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2165,81 +4843,108 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_8pykdtree_6kdtree_6KDTree_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8pykdtree_6kdtree_6KDTree_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_data_pts = 0;
   int __pyx_v_leafsize;
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[2] = {0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 91, __pyx_L3_error)
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data_pts,&__pyx_n_s_leafsize,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data_pts,&__pyx_n_s_leafsize,0};
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_pts)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data_pts)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_leafsize);
-          if (value) { values[1] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_leafsize);
+          if (value) { values[1] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_data_pts = ((PyArrayObject *)values[0]);
     if (values[1]) {
       __pyx_v_leafsize = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_leafsize == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
     } else {
       __pyx_v_leafsize = ((int)16);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 91, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 91, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data_pts), __pyx_ptype_5numpy_ndarray, 0, "data_pts", 0))) __PYX_ERR(0, 91, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_2__init__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self), __pyx_v_data_pts, __pyx_v_leafsize);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_8pykdtree_6kdtree_6KDTree_2__init__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, PyArrayObject *__pyx_v_data_pts, int __pyx_v_leafsize) {
   PyArrayObject *__pyx_v_data_array_float = 0;
   PyArrayObject *__pyx_v_data_array_double = 0;
@@ -2250,21 +4955,23 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyArrayObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  PyArrayObject *__pyx_t_12 = NULL;
+  char *__pyx_t_12;
+  PyArrayObject *__pyx_t_13 = NULL;
+  npy_intp *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __pyx_pybuffer_data_array_float.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_float.refcount = 0;
   __pyx_pybuffernd_data_array_float.data = NULL;
@@ -2277,25 +4984,25 @@
   /* "pykdtree/kdtree.pyx":94
  * 
  *         # Check arguments
  *         if leafsize < 1:             # <<<<<<<<<<<<<<
  *             raise ValueError('leafsize must be greater than zero')
  * 
  */
-  __pyx_t_1 = ((__pyx_v_leafsize < 1) != 0);
+  __pyx_t_1 = (__pyx_v_leafsize < 1);
   if (unlikely(__pyx_t_1)) {
 
     /* "pykdtree/kdtree.pyx":95
  *         # Check arguments
  *         if leafsize < 1:
  *             raise ValueError('leafsize must be greater than zero')             # <<<<<<<<<<<<<<
  * 
  *         # Get data content
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 95, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":94
  * 
@@ -2319,15 +5026,15 @@
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_1) {
 
     /* "pykdtree/kdtree.pyx":102
  * 
  *         if data_pts.dtype == np.float32:
  *             data_array_float = np.ascontiguousarray(data_pts.ravel(), dtype=np.float32)             # <<<<<<<<<<<<<<
@@ -2338,90 +5045,98 @@
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_6 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    #endif
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
     __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 102, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 102, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 102, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 102, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 102, __pyx_L1_error)
-    __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
+    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 102, __pyx_L1_error)
+    __pyx_t_8 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float.rcbuffer->pybuffer);
-      __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_8 < 0)) {
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_data_array_float, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_9, __pyx_t_10, __pyx_t_11);
         }
         __pyx_t_9 = __pyx_t_10 = __pyx_t_11 = 0;
       }
       __pyx_pybuffernd_data_array_float.diminfo[0].strides = __pyx_pybuffernd_data_array_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_float.diminfo[0].shape = __pyx_pybuffernd_data_array_float.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+      if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 102, __pyx_L1_error)
     }
+    __pyx_t_8 = 0;
+    __pyx_v_data_array_float = ((PyArrayObject *)__pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_v_data_array_float = ((PyArrayObject *)__pyx_t_6);
-    __pyx_t_6 = 0;
 
     /* "pykdtree/kdtree.pyx":103
  *         if data_pts.dtype == np.float32:
  *             data_array_float = np.ascontiguousarray(data_pts.ravel(), dtype=np.float32)
  *             self._data_pts_data_float = <float *>data_array_float.data             # <<<<<<<<<<<<<<
  *             self.data_pts = data_array_float
  *         else:
  */
-    __pyx_v_self->_data_pts_data_float = ((float *)__pyx_v_data_array_float->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_data_array_float)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_v_self->_data_pts_data_float = ((float *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":104
  *             data_array_float = np.ascontiguousarray(data_pts.ravel(), dtype=np.float32)
  *             self._data_pts_data_float = <float *>data_array_float.data
  *             self.data_pts = data_array_float             # <<<<<<<<<<<<<<
  *         else:
  *             data_array_double = np.ascontiguousarray(data_pts.ravel(), dtype=np.float64)
  */
-    __Pyx_INCREF(((PyObject *)__pyx_v_data_array_float));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_data_array_float));
-    __Pyx_GOTREF(__pyx_v_self->data_pts);
-    __Pyx_DECREF(((PyObject *)__pyx_v_self->data_pts));
+    __Pyx_INCREF((PyObject *)__pyx_v_data_array_float);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_data_array_float);
+    __Pyx_GOTREF((PyObject *)__pyx_v_self->data_pts);
+    __Pyx_DECREF((PyObject *)__pyx_v_self->data_pts);
     __pyx_v_self->data_pts = ((PyArrayObject *)__pyx_v_data_array_float);
 
     /* "pykdtree/kdtree.pyx":101
  *         cdef np.ndarray[double, ndim=1] data_array_double
  * 
  *         if data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *             data_array_float = np.ascontiguousarray(data_pts.ravel(), dtype=np.float32)
@@ -2434,125 +5149,134 @@
  *             self.data_pts = data_array_float
  *         else:
  *             data_array_double = np.ascontiguousarray(data_pts.ravel(), dtype=np.float64)             # <<<<<<<<<<<<<<
  *             self._data_pts_data_double = <double *>data_array_double.data
  *             self.data_pts = data_array_double
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_6 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    #endif
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_4, };
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
     __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error);
+    __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 106, __pyx_L1_error)
-    __pyx_t_12 = ((PyArrayObject *)__pyx_t_5);
+    __pyx_t_13 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_double.rcbuffer->pybuffer);
-      __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_12, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_8 < 0)) {
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_11, &__pyx_t_10, &__pyx_t_9);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_v_data_array_double, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_9);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_11, __pyx_t_10, __pyx_t_9);
         }
         __pyx_t_11 = __pyx_t_10 = __pyx_t_9 = 0;
       }
       __pyx_pybuffernd_data_array_double.diminfo[0].strides = __pyx_pybuffernd_data_array_double.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_double.diminfo[0].shape = __pyx_pybuffernd_data_array_double.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 106, __pyx_L1_error)
+      if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 106, __pyx_L1_error)
     }
-    __pyx_t_12 = 0;
+    __pyx_t_13 = 0;
     __pyx_v_data_array_double = ((PyArrayObject *)__pyx_t_5);
     __pyx_t_5 = 0;
 
     /* "pykdtree/kdtree.pyx":107
  *         else:
  *             data_array_double = np.ascontiguousarray(data_pts.ravel(), dtype=np.float64)
  *             self._data_pts_data_double = <double *>data_array_double.data             # <<<<<<<<<<<<<<
  *             self.data_pts = data_array_double
  * 
  */
-    __pyx_v_self->_data_pts_data_double = ((double *)__pyx_v_data_array_double->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_data_array_double)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_v_self->_data_pts_data_double = ((double *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":108
  *             data_array_double = np.ascontiguousarray(data_pts.ravel(), dtype=np.float64)
  *             self._data_pts_data_double = <double *>data_array_double.data
  *             self.data_pts = data_array_double             # <<<<<<<<<<<<<<
  * 
  *         # scipy interface compatibility
  */
-    __Pyx_INCREF(((PyObject *)__pyx_v_data_array_double));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_data_array_double));
-    __Pyx_GOTREF(__pyx_v_self->data_pts);
-    __Pyx_DECREF(((PyObject *)__pyx_v_self->data_pts));
+    __Pyx_INCREF((PyObject *)__pyx_v_data_array_double);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_data_array_double);
+    __Pyx_GOTREF((PyObject *)__pyx_v_self->data_pts);
+    __Pyx_DECREF((PyObject *)__pyx_v_self->data_pts);
     __pyx_v_self->data_pts = ((PyArrayObject *)__pyx_v_data_array_double);
   }
   __pyx_L4:;
 
   /* "pykdtree/kdtree.pyx":111
  * 
  *         # scipy interface compatibility
  *         self.data = self.data_pts             # <<<<<<<<<<<<<<
  * 
  *         # Get tree info
  */
   __pyx_t_5 = ((PyObject *)__pyx_v_self->data_pts);
   __Pyx_INCREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
-  __Pyx_GOTREF(__pyx_v_self->data);
-  __Pyx_DECREF(((PyObject *)__pyx_v_self->data));
+  __Pyx_GOTREF((PyObject *)__pyx_v_self->data);
+  __Pyx_DECREF((PyObject *)__pyx_v_self->data);
   __pyx_v_self->data = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "pykdtree/kdtree.pyx":114
  * 
  *         # Get tree info
  *         self.n = <uint32_t>data_pts.shape[0]             # <<<<<<<<<<<<<<
  *         self.leafsize = <uint32_t>leafsize
  *         if data_pts.ndim == 1:
  */
-  __pyx_v_self->n = ((uint32_t)(__pyx_v_data_pts->dimensions[0]));
+  __pyx_t_14 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_data_pts); if (unlikely(__pyx_t_14 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_v_self->n = ((uint32_t)(__pyx_t_14[0]));
 
   /* "pykdtree/kdtree.pyx":115
  *         # Get tree info
  *         self.n = <uint32_t>data_pts.shape[0]
  *         self.leafsize = <uint32_t>leafsize             # <<<<<<<<<<<<<<
  *         if data_pts.ndim == 1:
  *             self.ndim = 1
@@ -2562,15 +5286,16 @@
   /* "pykdtree/kdtree.pyx":116
  *         self.n = <uint32_t>data_pts.shape[0]
  *         self.leafsize = <uint32_t>leafsize
  *         if data_pts.ndim == 1:             # <<<<<<<<<<<<<<
  *             self.ndim = 1
  *         elif data_pts.shape[1] > 127:
  */
-  __pyx_t_1 = ((__pyx_v_data_pts->nd == 1) != 0);
+  __pyx_t_6 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_data_pts); if (unlikely(__pyx_t_6 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_1 = (__pyx_t_6 == 1);
   if (__pyx_t_1) {
 
     /* "pykdtree/kdtree.pyx":117
  *         self.leafsize = <uint32_t>leafsize
  *         if data_pts.ndim == 1:
  *             self.ndim = 1             # <<<<<<<<<<<<<<
  *         elif data_pts.shape[1] > 127:
@@ -2591,25 +5316,26 @@
   /* "pykdtree/kdtree.pyx":118
  *         if data_pts.ndim == 1:
  *             self.ndim = 1
  *         elif data_pts.shape[1] > 127:             # <<<<<<<<<<<<<<
  *             raise ValueError('Max 127 dimensions allowed')
  *         else:
  */
-  __pyx_t_1 = (((__pyx_v_data_pts->dimensions[1]) > 0x7F) != 0);
+  __pyx_t_14 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_data_pts); if (unlikely(__pyx_t_14 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = ((__pyx_t_14[1]) > 0x7F);
   if (unlikely(__pyx_t_1)) {
 
     /* "pykdtree/kdtree.pyx":119
  *             self.ndim = 1
  *         elif data_pts.shape[1] > 127:
  *             raise ValueError('Max 127 dimensions allowed')             # <<<<<<<<<<<<<<
  *         else:
  *             self.ndim = <int8_t>data_pts.shape[1]
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __PYX_ERR(0, 119, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":118
  *         if data_pts.ndim == 1:
@@ -2624,49 +5350,51 @@
  *             raise ValueError('Max 127 dimensions allowed')
  *         else:
  *             self.ndim = <int8_t>data_pts.shape[1]             # <<<<<<<<<<<<<<
  * 
  *         # Release GIL and construct tree
  */
   /*else*/ {
-    __pyx_v_self->ndim = ((int8_t)(__pyx_v_data_pts->dimensions[1]));
+    __pyx_t_14 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_data_pts); if (unlikely(__pyx_t_14 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_v_self->ndim = ((int8_t)(__pyx_t_14[1]));
   }
   __pyx_L5:;
 
   /* "pykdtree/kdtree.pyx":124
  * 
  *         # Release GIL and construct tree
  *         if data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 self._kdtree_float = construct_tree_float(self._data_pts_data_float, self.ndim,
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyObject_RichCompare(__pyx_t_5, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_5, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_1) {
 
     /* "pykdtree/kdtree.pyx":125
  *         # Release GIL and construct tree
  *         if data_pts.dtype == np.float32:
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 self._kdtree_float = construct_tree_float(self._data_pts_data_float, self.ndim,
  *                                                           self.n, self.leafsize)
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
+        _save = NULL;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
           /* "pykdtree/kdtree.pyx":126
  *         if data_pts.dtype == np.float32:
@@ -2714,14 +5442,15 @@
  *                 self._kdtree_double = construct_tree_double(self._data_pts_data_double, self.ndim,
  *                                                             self.n, self.leafsize)
  */
   /*else*/ {
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
+        _save = NULL;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
           /* "pykdtree/kdtree.pyx":130
  *         else:
@@ -2766,15 +5495,15 @@
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_double.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
@@ -2796,131 +5525,173 @@
  * 
  *     def query(KDTree self, np.ndarray query_pts not None, k=1, eps=0,             # <<<<<<<<<<<<<<
  *               distance_upper_bound=None, sqr_dists=False, mask=None):
  *         """Query the kd-tree for nearest neighbors
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_5query(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8pykdtree_6kdtree_6KDTree_4query[] = "Query the kd-tree for nearest neighbors\n\n        :Parameters:\n        query_pts : numpy array\n            Query points with shape (m, dims)\n        k : int\n            The number of nearest neighbours to return\n        eps : non-negative float\n            Return approximate nearest neighbours; the k-th returned value\n            is guaranteed to be no further than (1 + eps) times the distance\n            to the real k-th nearest neighbour\n        distance_upper_bound : non-negative float\n            Return only neighbors within this distance.\n            This is used to prune tree searches.\n        sqr_dists : bool, optional\n            Internally pykdtree works with squared distances.\n            Determines if the squared or Euclidean distances are returned.\n        mask : numpy array, optional\n            Array of booleans where neighbors are considered invalid and\n            should not be returned. A mask value of True represents an\n            invalid pixel. Mask should have shape (n,) to match data points.\n            By default all points are considered valid.\n\n        ";
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_5query(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_5query(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8pykdtree_6kdtree_6KDTree_4query, "Query the kd-tree for nearest neighbors\n\n        :Parameters:\n        query_pts : numpy array\n            Query points with shape (m, dims)\n        k : int\n            The number of nearest neighbours to return\n        eps : non-negative float\n            Return approximate nearest neighbours; the k-th returned value\n            is guaranteed to be no further than (1 + eps) times the distance\n            to the real k-th nearest neighbour\n        distance_upper_bound : non-negative float\n            Return only neighbors within this distance.\n            This is used to prune tree searches.\n        sqr_dists : bool, optional\n            Internally pykdtree works with squared distances.\n            Determines if the squared or Euclidean distances are returned.\n        mask : numpy array, optional\n            Array of booleans where neighbors are considered invalid and\n            should not be returned. A mask value of True represents an\n            invalid pixel. Mask should have shape (n,) to match data points.\n            By default all points are considered valid.\n\n        ");
+static PyMethodDef __pyx_mdef_8pykdtree_6kdtree_6KDTree_5query = {"query", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_5query, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8pykdtree_6kdtree_6KDTree_4query};
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_5query(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_query_pts = 0;
   PyObject *__pyx_v_k = 0;
   PyObject *__pyx_v_eps = 0;
   PyObject *__pyx_v_distance_upper_bound = 0;
   PyObject *__pyx_v_sqr_dists = 0;
   PyObject *__pyx_v_mask = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[6] = {0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("query (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 134, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_query_pts,&__pyx_n_s_k,&__pyx_n_s_eps,&__pyx_n_s_distance_upper_bound,&__pyx_n_s_sqr_dists,&__pyx_n_s_mask,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
-    values[1] = ((PyObject *)__pyx_int_1);
-    values[2] = ((PyObject *)__pyx_int_0);
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_query_pts,&__pyx_n_s_k,&__pyx_n_s_eps,&__pyx_n_s_distance_upper_bound,&__pyx_n_s_sqr_dists,&__pyx_n_s_mask,0};
+    values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_1));
+    values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_0));
 
     /* "pykdtree/kdtree.pyx":135
  * 
  *     def query(KDTree self, np.ndarray query_pts not None, k=1, eps=0,
  *               distance_upper_bound=None, sqr_dists=False, mask=None):             # <<<<<<<<<<<<<<
  *         """Query the kd-tree for nearest neighbors
  * 
  */
-    values[3] = ((PyObject *)Py_None);
-    values[4] = ((PyObject *)Py_False);
-    values[5] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
+    values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
+    values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_False));
+    values[5] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      switch (__pyx_nargs) {
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_query_pts)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query_pts)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_k);
-          if (value) { values[1] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_k);
+          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_eps);
-          if (value) { values[2] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_eps);
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_distance_upper_bound);
-          if (value) { values[3] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_distance_upper_bound);
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sqr_dists);
-          if (value) { values[4] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sqr_dists);
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mask);
-          if (value) { values[5] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mask);
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "query") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "query") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      switch (__pyx_nargs) {
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_query_pts = ((PyArrayObject *)values[0]);
     __pyx_v_k = values[1];
     __pyx_v_eps = values[2];
     __pyx_v_distance_upper_bound = values[3];
     __pyx_v_sqr_dists = values[4];
     __pyx_v_mask = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("query", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("query", 0, 1, 6, __pyx_nargs); __PYX_ERR(0, 134, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("pykdtree.kdtree.KDTree.query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_query_pts), __pyx_ptype_5numpy_ndarray, 0, "query_pts", 0))) __PYX_ERR(0, 134, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_4query(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self), __pyx_v_query_pts, __pyx_v_k, __pyx_v_eps, __pyx_v_distance_upper_bound, __pyx_v_sqr_dists, __pyx_v_mask);
 
@@ -2933,20 +5704,26 @@
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_4query(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, PyArrayObject *__pyx_v_query_pts, PyObject *__pyx_v_k, PyObject *__pyx_v_eps, PyObject *__pyx_v_distance_upper_bound, PyObject *__pyx_v_sqr_dists, PyObject *__pyx_v_mask) {
-  long __pyx_v_q_ndim;
+  npy_intp __pyx_v_q_ndim;
   uint32_t __pyx_v_num_qpoints;
   uint32_t __pyx_v_num_n;
   PyArrayObject *__pyx_v_closest_idxs = 0;
   PyArrayObject *__pyx_v_closest_dists_float = 0;
   PyArrayObject *__pyx_v_closest_dists_double = 0;
   uint32_t *__pyx_v_closest_idxs_data;
   float *__pyx_v_closest_dists_data_float;
@@ -2978,32 +5755,33 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_query_mask;
   __Pyx_Buffer __pyx_pybuffer_query_mask;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  npy_intp *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  uint32_t __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyArrayObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  uint32_t __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
   PyArrayObject *__pyx_t_11 = NULL;
-  int __pyx_t_12;
-  PyObject *__pyx_t_13 = NULL;
+  char *__pyx_t_12;
+  PyArrayObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
-  PyArrayObject *__pyx_t_16 = NULL;
+  PyObject *__pyx_t_16 = NULL;
   PyArrayObject *__pyx_t_17 = NULL;
   PyArrayObject *__pyx_t_18 = NULL;
   PyArrayObject *__pyx_t_19 = NULL;
-  float __pyx_t_20;
-  double __pyx_t_21;
+  PyArrayObject *__pyx_t_20 = NULL;
+  float __pyx_t_21;
+  double __pyx_t_22;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("query", 0);
   __pyx_pybuffer_closest_idxs.pybuffer.buf = NULL;
   __pyx_pybuffer_closest_idxs.refcount = 0;
   __pyx_pybuffernd_closest_idxs.data = NULL;
@@ -3033,26 +5811,26 @@
  * 
  *         # Check arguments
  *         if k < 1:             # <<<<<<<<<<<<<<
  *             raise ValueError('Number of neighbours must be greater than zero')
  *         elif eps < 0:
  */
   __pyx_t_1 = PyObject_RichCompare(__pyx_v_k, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
     /* "pykdtree/kdtree.pyx":163
  *         # Check arguments
  *         if k < 1:
  *             raise ValueError('Number of neighbours must be greater than zero')             # <<<<<<<<<<<<<<
  *         elif eps < 0:
  *             raise ValueError('eps must be non-negative')
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 163, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":162
  * 
@@ -3067,26 +5845,26 @@
  *         if k < 1:
  *             raise ValueError('Number of neighbours must be greater than zero')
  *         elif eps < 0:             # <<<<<<<<<<<<<<
  *             raise ValueError('eps must be non-negative')
  *         elif distance_upper_bound is not None:
  */
   __pyx_t_1 = PyObject_RichCompare(__pyx_v_eps, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
     /* "pykdtree/kdtree.pyx":165
  *             raise ValueError('Number of neighbours must be greater than zero')
  *         elif eps < 0:
  *             raise ValueError('eps must be non-negative')             # <<<<<<<<<<<<<<
  *         elif distance_upper_bound is not None:
  *             if distance_upper_bound < 0:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 165, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":164
  *         if k < 1:
@@ -3101,37 +5879,36 @@
  *         elif eps < 0:
  *             raise ValueError('eps must be non-negative')
  *         elif distance_upper_bound is not None:             # <<<<<<<<<<<<<<
  *             if distance_upper_bound < 0:
  *                 raise ValueError('distance_upper_bound must be non negative')
  */
   __pyx_t_2 = (__pyx_v_distance_upper_bound != Py_None);
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":167
  *             raise ValueError('eps must be non-negative')
  *         elif distance_upper_bound is not None:
  *             if distance_upper_bound < 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError('distance_upper_bound must be non negative')
  * 
  */
     __pyx_t_1 = PyObject_RichCompare(__pyx_v_distance_upper_bound, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(__pyx_t_3)) {
+    if (unlikely(__pyx_t_2)) {
 
       /* "pykdtree/kdtree.pyx":168
  *         elif distance_upper_bound is not None:
  *             if distance_upper_bound < 0:
  *                 raise ValueError('distance_upper_bound must be non negative')             # <<<<<<<<<<<<<<
  * 
  *         # Check dimensions
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __PYX_ERR(0, 168, __pyx_L1_error)
 
       /* "pykdtree/kdtree.pyx":167
  *             raise ValueError('eps must be non-negative')
@@ -3154,16 +5931,17 @@
   /* "pykdtree/kdtree.pyx":171
  * 
  *         # Check dimensions
  *         if query_pts.ndim == 1:             # <<<<<<<<<<<<<<
  *             q_ndim = 1
  *         else:
  */
-  __pyx_t_3 = ((__pyx_v_query_pts->nd == 1) != 0);
-  if (__pyx_t_3) {
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_query_pts); if (unlikely(__pyx_t_3 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_3 == 1);
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":172
  *         # Check dimensions
  *         if query_pts.ndim == 1:
  *             q_ndim = 1             # <<<<<<<<<<<<<<
  *         else:
  *             q_ndim = query_pts.shape[1]
@@ -3184,36 +5962,37 @@
  *             q_ndim = 1
  *         else:
  *             q_ndim = query_pts.shape[1]             # <<<<<<<<<<<<<<
  * 
  *         if self.ndim != q_ndim:
  */
   /*else*/ {
-    __pyx_v_q_ndim = (__pyx_v_query_pts->dimensions[1]);
+    __pyx_t_4 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_query_pts); if (unlikely(__pyx_t_4 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_v_q_ndim = (__pyx_t_4[1]);
   }
   __pyx_L5:;
 
   /* "pykdtree/kdtree.pyx":176
  *             q_ndim = query_pts.shape[1]
  * 
  *         if self.ndim != q_ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError('Data and query points must have same dimensions')
  * 
  */
-  __pyx_t_3 = ((__pyx_v_self->ndim != __pyx_v_q_ndim) != 0);
-  if (unlikely(__pyx_t_3)) {
+  __pyx_t_2 = (__pyx_v_self->ndim != __pyx_v_q_ndim);
+  if (unlikely(__pyx_t_2)) {
 
     /* "pykdtree/kdtree.pyx":177
  * 
  *         if self.ndim != q_ndim:
  *             raise ValueError('Data and query points must have same dimensions')             # <<<<<<<<<<<<<<
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 177, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":176
  *             q_ndim = query_pts.shape[1]
@@ -3229,56 +6008,56 @@
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:             # <<<<<<<<<<<<<<
  *             raise TypeError('Type mismatch. query points must be of type float32 when data points are of type float32')
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_1, __pyx_t_6, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__pyx_t_2) {
+  if (__pyx_t_7) {
   } else {
-    __pyx_t_3 = __pyx_t_2;
+    __pyx_t_2 = __pyx_t_7;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_5, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_3 = __pyx_t_2;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_2 = __pyx_t_7;
   __pyx_L8_bool_binop_done:;
-  if (unlikely(__pyx_t_3)) {
+  if (unlikely(__pyx_t_2)) {
 
     /* "pykdtree/kdtree.pyx":180
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:
  *             raise TypeError('Type mismatch. query points must be of type float32 when data points are of type float32')             # <<<<<<<<<<<<<<
  * 
  *         # Get query info
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 180, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":179
  *             raise ValueError('Data and query points must have same dimensions')
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:             # <<<<<<<<<<<<<<
  *             raise TypeError('Type mismatch. query points must be of type float32 when data points are of type float32')
@@ -3289,123 +6068,124 @@
   /* "pykdtree/kdtree.pyx":183
  * 
  *         # Get query info
  *         cdef uint32_t num_qpoints = query_pts.shape[0]             # <<<<<<<<<<<<<<
  *         cdef uint32_t num_n = k
  *         cdef np.ndarray[uint32_t, ndim=1] closest_idxs = np.empty(num_qpoints * k, dtype=np.uint32)
  */
-  __pyx_v_num_qpoints = (__pyx_v_query_pts->dimensions[0]);
+  __pyx_t_4 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_query_pts); if (unlikely(__pyx_t_4 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_v_num_qpoints = (__pyx_t_4[0]);
 
   /* "pykdtree/kdtree.pyx":184
  *         # Get query info
  *         cdef uint32_t num_qpoints = query_pts.shape[0]
  *         cdef uint32_t num_n = k             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[uint32_t, ndim=1] closest_idxs = np.empty(num_qpoints * k, dtype=np.uint32)
  *         cdef np.ndarray[float, ndim=1] closest_dists_float
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_k); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
-  __pyx_v_num_n = __pyx_t_6;
+  __pyx_t_8 = __Pyx_PyInt_As_uint32_t(__pyx_v_k); if (unlikely((__pyx_t_8 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_v_num_n = __pyx_t_8;
 
   /* "pykdtree/kdtree.pyx":185
  *         cdef uint32_t num_qpoints = query_pts.shape[0]
  *         cdef uint32_t num_n = k
  *         cdef np.ndarray[uint32_t, ndim=1] closest_idxs = np.empty(num_qpoints * k, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[float, ndim=1] closest_dists_float
  *         cdef np.ndarray[double, ndim=1] closest_dists_double
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyNumber_Multiply(__pyx_t_6, __pyx_v_k); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_uint32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 185, __pyx_L1_error)
-  __pyx_t_9 = ((PyArrayObject *)__pyx_t_8);
+  if (!(likely(((__pyx_t_10) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_10, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_11 = ((PyArrayObject *)__pyx_t_10);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_closest_idxs = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 185, __pyx_L1_error)
     } else {__pyx_pybuffernd_closest_idxs.diminfo[0].strides = __pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_closest_idxs.diminfo[0].shape = __pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_9 = 0;
-  __pyx_v_closest_idxs = ((PyArrayObject *)__pyx_t_8);
-  __pyx_t_8 = 0;
+  __pyx_t_11 = 0;
+  __pyx_v_closest_idxs = ((PyArrayObject *)__pyx_t_10);
+  __pyx_t_10 = 0;
 
   /* "pykdtree/kdtree.pyx":191
  * 
  *         # Set up return arrays
  *         cdef uint32_t *closest_idxs_data = <uint32_t *>closest_idxs.data             # <<<<<<<<<<<<<<
  *         cdef float *closest_dists_data_float
  *         cdef double *closest_dists_data_double
  */
-  __pyx_v_closest_idxs_data = ((uint32_t *)__pyx_v_closest_idxs->data);
+  __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_closest_idxs)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_v_closest_idxs_data = ((uint32_t *)__pyx_t_12);
 
   /* "pykdtree/kdtree.pyx":203
  *         cdef np.uint8_t *query_mask_data
  * 
  *         if mask is not None and mask.size != self.n:             # <<<<<<<<<<<<<<
  *             raise ValueError('Mask must have the same size as data points')
  *         elif mask is not None:
  */
-  __pyx_t_2 = (__pyx_v_mask != Py_None);
-  __pyx_t_10 = (__pyx_t_2 != 0);
-  if (__pyx_t_10) {
+  __pyx_t_7 = (__pyx_v_mask != Py_None);
+  if (__pyx_t_7) {
   } else {
-    __pyx_t_3 = __pyx_t_10;
+    __pyx_t_2 = __pyx_t_7;
     goto __pyx_L11_bool_binop_done;
   }
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_mask, __pyx_n_s_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 203, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_mask, __pyx_n_s_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_10, __pyx_t_5, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_3 = __pyx_t_10;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_2 = __pyx_t_7;
   __pyx_L11_bool_binop_done:;
-  if (unlikely(__pyx_t_3)) {
+  if (unlikely(__pyx_t_2)) {
 
     /* "pykdtree/kdtree.pyx":204
  * 
  *         if mask is not None and mask.size != self.n:
  *             raise ValueError('Mask must have the same size as data points')             # <<<<<<<<<<<<<<
  *         elif mask is not None:
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 204, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 204, __pyx_L1_error)
 
     /* "pykdtree/kdtree.pyx":203
  *         cdef np.uint8_t *query_mask_data
  * 
  *         if mask is not None and mask.size != self.n:             # <<<<<<<<<<<<<<
  *             raise ValueError('Mask must have the same size as data points')
@@ -3416,97 +6196,104 @@
   /* "pykdtree/kdtree.pyx":205
  *         if mask is not None and mask.size != self.n:
  *             raise ValueError('Mask must have the same size as data points')
  *         elif mask is not None:             # <<<<<<<<<<<<<<
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)
  *             query_mask_data = <uint8_t *>query_mask.data
  */
-  __pyx_t_3 = (__pyx_v_mask != Py_None);
-  __pyx_t_10 = (__pyx_t_3 != 0);
-  if (__pyx_t_10) {
+  __pyx_t_2 = (__pyx_v_mask != Py_None);
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":206
  *             raise ValueError('Mask must have the same size as data points')
  *         elif mask is not None:
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)             # <<<<<<<<<<<<<<
  *             query_mask_data = <uint8_t *>query_mask.data
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_mask, __pyx_n_s_ravel); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_mask, __pyx_n_s_ravel); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_10, function);
+        __pyx_t_3 = 1;
       }
     }
-    __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5);
-    __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    #endif
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_1, };
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_3, 0+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    }
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_6);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_6)) __PYX_ERR(0, 206, __pyx_L1_error);
+    __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 206, __pyx_L1_error)
-    __pyx_t_11 = ((PyArrayObject *)__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (!(likely(((__pyx_t_9) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_9, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 206, __pyx_L1_error)
+    __pyx_t_13 = ((PyArrayObject *)__pyx_t_9);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_query_mask.rcbuffer->pybuffer);
-      __pyx_t_12 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_mask.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_12 < 0)) {
-        PyErr_Fetch(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
+      __pyx_t_3 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_mask.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_3 < 0)) {
+        PyErr_Fetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_mask.rcbuffer->pybuffer, (PyObject*)__pyx_v_query_mask, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15);
+          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_16);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_13, __pyx_t_14, __pyx_t_15);
+          PyErr_Restore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
         }
-        __pyx_t_13 = __pyx_t_14 = __pyx_t_15 = 0;
+        __pyx_t_14 = __pyx_t_15 = __pyx_t_16 = 0;
       }
       __pyx_pybuffernd_query_mask.diminfo[0].strides = __pyx_pybuffernd_query_mask.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_query_mask.diminfo[0].shape = __pyx_pybuffernd_query_mask.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
+      if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 206, __pyx_L1_error)
     }
-    __pyx_t_11 = 0;
-    __pyx_v_query_mask = ((PyArrayObject *)__pyx_t_7);
-    __pyx_t_7 = 0;
+    __pyx_t_13 = 0;
+    __pyx_v_query_mask = ((PyArrayObject *)__pyx_t_9);
+    __pyx_t_9 = 0;
 
     /* "pykdtree/kdtree.pyx":207
  *         elif mask is not None:
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)
  *             query_mask_data = <uint8_t *>query_mask.data             # <<<<<<<<<<<<<<
  *         else:
  *             query_mask_data = NULL
  */
-    __pyx_v_query_mask_data = ((uint8_t *)__pyx_v_query_mask->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_query_mask)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_v_query_mask_data = ((uint8_t *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":205
  *         if mask is not None and mask.size != self.n:
  *             raise ValueError('Mask must have the same size as data points')
  *         elif mask is not None:             # <<<<<<<<<<<<<<
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)
  *             query_mask_data = <uint8_t *>query_mask.data
@@ -3529,204 +6316,213 @@
   /* "pykdtree/kdtree.pyx":212
  * 
  * 
  *         if query_pts.dtype == np.float32 and self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *             closest_dists_float = np.empty(num_qpoints * k, dtype=np.float32)
  *             closest_dists = closest_dists_float
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_7, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__pyx_t_3) {
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_9, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__pyx_t_7) {
   } else {
-    __pyx_t_10 = __pyx_t_3;
+    __pyx_t_2 = __pyx_t_7;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyObject_RichCompare(__pyx_t_5, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_10 = __pyx_t_3;
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_float32); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = PyObject_RichCompare(__pyx_t_6, __pyx_t_9, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_2 = __pyx_t_7;
   __pyx_L14_bool_binop_done:;
-  if (__pyx_t_10) {
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":213
  * 
  *         if query_pts.dtype == np.float32 and self.data_pts.dtype == np.float32:
  *             closest_dists_float = np.empty(num_qpoints * k, dtype=np.float32)             # <<<<<<<<<<<<<<
  *             closest_dists = closest_dists_float
  *             closest_dists_data_float = <float *>closest_dists_float.data
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = PyNumber_Multiply(__pyx_t_8, __pyx_v_k); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5);
-    __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_empty); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_6 = PyNumber_Multiply(__pyx_t_10, __pyx_v_k); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_6);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_6)) __PYX_ERR(0, 213, __pyx_L1_error);
+    __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_8, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 213, __pyx_L1_error)
-    __pyx_t_16 = ((PyArrayObject *)__pyx_t_1);
+    __pyx_t_17 = ((PyArrayObject *)__pyx_t_1);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer);
-      __pyx_t_12 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_16, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_12 < 0)) {
-        PyErr_Fetch(&__pyx_t_15, &__pyx_t_14, &__pyx_t_13);
+      __pyx_t_3 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_3 < 0)) {
+        PyErr_Fetch(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_closest_dists_float, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13);
+          Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_14);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_15, __pyx_t_14, __pyx_t_13);
+          PyErr_Restore(__pyx_t_16, __pyx_t_15, __pyx_t_14);
         }
-        __pyx_t_15 = __pyx_t_14 = __pyx_t_13 = 0;
+        __pyx_t_16 = __pyx_t_15 = __pyx_t_14 = 0;
       }
       __pyx_pybuffernd_closest_dists_float.diminfo[0].strides = __pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_closest_dists_float.diminfo[0].shape = __pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 213, __pyx_L1_error)
+      if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 213, __pyx_L1_error)
     }
-    __pyx_t_16 = 0;
+    __pyx_t_17 = 0;
     __pyx_v_closest_dists_float = ((PyArrayObject *)__pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "pykdtree/kdtree.pyx":214
  *         if query_pts.dtype == np.float32 and self.data_pts.dtype == np.float32:
  *             closest_dists_float = np.empty(num_qpoints * k, dtype=np.float32)
  *             closest_dists = closest_dists_float             # <<<<<<<<<<<<<<
  *             closest_dists_data_float = <float *>closest_dists_float.data
  *             query_array_float = np.ascontiguousarray(query_pts.ravel(), dtype=np.float32)
  */
-    __Pyx_INCREF(((PyObject *)__pyx_v_closest_dists_float));
+    __Pyx_INCREF((PyObject *)__pyx_v_closest_dists_float);
     __pyx_v_closest_dists = ((PyObject *)__pyx_v_closest_dists_float);
 
     /* "pykdtree/kdtree.pyx":215
  *             closest_dists_float = np.empty(num_qpoints * k, dtype=np.float32)
  *             closest_dists = closest_dists_float
  *             closest_dists_data_float = <float *>closest_dists_float.data             # <<<<<<<<<<<<<<
  *             query_array_float = np.ascontiguousarray(query_pts.ravel(), dtype=np.float32)
  *             query_array_data_float = <float *>query_array_float.data
  */
-    __pyx_v_closest_dists_data_float = ((float *)__pyx_v_closest_dists_float->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_closest_dists_float)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_v_closest_dists_data_float = ((float *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":216
  *             closest_dists = closest_dists_float
  *             closest_dists_data_float = <float *>closest_dists_float.data
  *             query_array_float = np.ascontiguousarray(query_pts.ravel(), dtype=np.float32)             # <<<<<<<<<<<<<<
  *             query_array_data_float = <float *>query_array_float.data
  *         else:
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_7);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_9 = NULL;
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_10, function);
+        __pyx_t_3 = 1;
       }
     }
-    __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    #endif
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_9, };
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_3, 0+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    }
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error);
     __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 216, __pyx_L1_error)
-    __pyx_t_17 = ((PyArrayObject *)__pyx_t_4);
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_18 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_query_array_float.rcbuffer->pybuffer);
-      __pyx_t_12 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_12 < 0)) {
-        PyErr_Fetch(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
+      __pyx_t_3 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_3 < 0)) {
+        PyErr_Fetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_query_array_float, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15);
+          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_16);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_13, __pyx_t_14, __pyx_t_15);
+          PyErr_Restore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
         }
-        __pyx_t_13 = __pyx_t_14 = __pyx_t_15 = 0;
+        __pyx_t_14 = __pyx_t_15 = __pyx_t_16 = 0;
       }
       __pyx_pybuffernd_query_array_float.diminfo[0].strides = __pyx_pybuffernd_query_array_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_query_array_float.diminfo[0].shape = __pyx_pybuffernd_query_array_float.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 216, __pyx_L1_error)
+      if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 216, __pyx_L1_error)
     }
-    __pyx_t_17 = 0;
-    __pyx_v_query_array_float = ((PyArrayObject *)__pyx_t_4);
-    __pyx_t_4 = 0;
+    __pyx_t_18 = 0;
+    __pyx_v_query_array_float = ((PyArrayObject *)__pyx_t_5);
+    __pyx_t_5 = 0;
 
     /* "pykdtree/kdtree.pyx":217
  *             closest_dists_data_float = <float *>closest_dists_float.data
  *             query_array_float = np.ascontiguousarray(query_pts.ravel(), dtype=np.float32)
  *             query_array_data_float = <float *>query_array_float.data             # <<<<<<<<<<<<<<
  *         else:
  *             closest_dists_double = np.empty(num_qpoints * k, dtype=np.float64)
  */
-    __pyx_v_query_array_data_float = ((float *)__pyx_v_query_array_float->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_query_array_float)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_v_query_array_data_float = ((float *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":212
  * 
  * 
  *         if query_pts.dtype == np.float32 and self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *             closest_dists_float = np.empty(num_qpoints * k, dtype=np.float32)
  *             closest_dists = closest_dists_float
@@ -3738,238 +6534,253 @@
  *             query_array_data_float = <float *>query_array_float.data
  *         else:
  *             closest_dists_double = np.empty(num_qpoints * k, dtype=np.float64)             # <<<<<<<<<<<<<<
  *             closest_dists = closest_dists_double
  *             closest_dists_data_double = <double *>closest_dists_double.data
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyNumber_Multiply(__pyx_t_4, __pyx_v_k); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_8);
-    __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_10 = PyNumber_Multiply(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_10);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_10)) __PYX_ERR(0, 219, __pyx_L1_error);
+    __pyx_t_10 = 0;
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 219, __pyx_L1_error)
-    __pyx_t_18 = ((PyArrayObject *)__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (!(likely(((__pyx_t_9) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_9, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_19 = ((PyArrayObject *)__pyx_t_9);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer);
-      __pyx_t_12 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_12 < 0)) {
-        PyErr_Fetch(&__pyx_t_15, &__pyx_t_14, &__pyx_t_13);
+      __pyx_t_3 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_3 < 0)) {
+        PyErr_Fetch(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer, (PyObject*)__pyx_v_closest_dists_double, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13);
+          Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_14);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_15, __pyx_t_14, __pyx_t_13);
+          PyErr_Restore(__pyx_t_16, __pyx_t_15, __pyx_t_14);
         }
-        __pyx_t_15 = __pyx_t_14 = __pyx_t_13 = 0;
+        __pyx_t_16 = __pyx_t_15 = __pyx_t_14 = 0;
       }
       __pyx_pybuffernd_closest_dists_double.diminfo[0].strides = __pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_closest_dists_double.diminfo[0].shape = __pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 219, __pyx_L1_error)
+      if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 219, __pyx_L1_error)
     }
-    __pyx_t_18 = 0;
-    __pyx_v_closest_dists_double = ((PyArrayObject *)__pyx_t_7);
-    __pyx_t_7 = 0;
+    __pyx_t_19 = 0;
+    __pyx_v_closest_dists_double = ((PyArrayObject *)__pyx_t_9);
+    __pyx_t_9 = 0;
 
     /* "pykdtree/kdtree.pyx":220
  *         else:
  *             closest_dists_double = np.empty(num_qpoints * k, dtype=np.float64)
  *             closest_dists = closest_dists_double             # <<<<<<<<<<<<<<
  *             closest_dists_data_double = <double *>closest_dists_double.data
  *             query_array_double = np.ascontiguousarray(query_pts.ravel(), dtype=np.float64)
  */
-    __Pyx_INCREF(((PyObject *)__pyx_v_closest_dists_double));
+    __Pyx_INCREF((PyObject *)__pyx_v_closest_dists_double);
     __pyx_v_closest_dists = ((PyObject *)__pyx_v_closest_dists_double);
 
     /* "pykdtree/kdtree.pyx":221
  *             closest_dists_double = np.empty(num_qpoints * k, dtype=np.float64)
  *             closest_dists = closest_dists_double
  *             closest_dists_data_double = <double *>closest_dists_double.data             # <<<<<<<<<<<<<<
  *             query_array_double = np.ascontiguousarray(query_pts.ravel(), dtype=np.float64)
  *             query_array_data_double = <double *>query_array_double.data
  */
-    __pyx_v_closest_dists_data_double = ((double *)__pyx_v_closest_dists_double->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_closest_dists_double)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_v_closest_dists_data_double = ((double *)__pyx_t_12);
 
     /* "pykdtree/kdtree.pyx":222
  *             closest_dists = closest_dists_double
  *             closest_dists_data_double = <double *>closest_dists_double.data
  *             query_array_double = np.ascontiguousarray(query_pts.ravel(), dtype=np.float64)             # <<<<<<<<<<<<<<
  *             query_array_data_double = <double *>query_array_double.data
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_query_pts), __pyx_n_s_ravel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_3 = 1;
       }
     }
-    __pyx_t_7 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
-    __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    #endif
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_1, };
+      __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_3, 0+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_9);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error);
+    __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_5, __pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 222, __pyx_L1_error)
-    __pyx_t_19 = ((PyArrayObject *)__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_20 = ((PyArrayObject *)__pyx_t_6);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_query_array_double.rcbuffer->pybuffer);
-      __pyx_t_12 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_12 < 0)) {
-        PyErr_Fetch(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
+      __pyx_t_3 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_3 < 0)) {
+        PyErr_Fetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_query_array_double.rcbuffer->pybuffer, (PyObject*)__pyx_v_query_array_double, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15);
+          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_16);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_13, __pyx_t_14, __pyx_t_15);
+          PyErr_Restore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
         }
-        __pyx_t_13 = __pyx_t_14 = __pyx_t_15 = 0;
+        __pyx_t_14 = __pyx_t_15 = __pyx_t_16 = 0;
       }
       __pyx_pybuffernd_query_array_double.diminfo[0].strides = __pyx_pybuffernd_query_array_double.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_query_array_double.diminfo[0].shape = __pyx_pybuffernd_query_array_double.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+      if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 222, __pyx_L1_error)
     }
-    __pyx_t_19 = 0;
-    __pyx_v_query_array_double = ((PyArrayObject *)__pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_20 = 0;
+    __pyx_v_query_array_double = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_6 = 0;
 
     /* "pykdtree/kdtree.pyx":223
  *             closest_dists_data_double = <double *>closest_dists_double.data
  *             query_array_double = np.ascontiguousarray(query_pts.ravel(), dtype=np.float64)
  *             query_array_data_double = <double *>query_array_double.data             # <<<<<<<<<<<<<<
  * 
  *         # Setup distance_upper_bound
  */
-    __pyx_v_query_array_data_double = ((double *)__pyx_v_query_array_double->data);
+    __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(((PyArrayObject *)__pyx_v_query_array_double)); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_v_query_array_data_double = ((double *)__pyx_t_12);
   }
   __pyx_L13:;
 
   /* "pykdtree/kdtree.pyx":228
  *         cdef float dub_float
  *         cdef double dub_double
  *         if distance_upper_bound is None:             # <<<<<<<<<<<<<<
  *             if self.data_pts.dtype == np.float32:
  *                 dub_float = <float>np.finfo(np.float32).max
  */
-  __pyx_t_10 = (__pyx_v_distance_upper_bound == Py_None);
-  __pyx_t_3 = (__pyx_t_10 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_2 = (__pyx_v_distance_upper_bound == Py_None);
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":229
  *         cdef double dub_double
  *         if distance_upper_bound is None:
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 dub_float = <float>np.finfo(np.float32).max
  *             else:
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_5, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (__pyx_t_3) {
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (__pyx_t_2) {
 
       /* "pykdtree/kdtree.pyx":230
  *         if distance_upper_bound is None:
  *             if self.data_pts.dtype == np.float32:
  *                 dub_float = <float>np.finfo(np.float32).max             # <<<<<<<<<<<<<<
  *             else:
  *                 dub_double = <double>np.finfo(np.float64).max
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_finfo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 230, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-          __Pyx_INCREF(__pyx_t_4);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_5, function);
-        }
-      }
-      __pyx_t_7 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 230, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_finfo); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_max); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_20 = __pyx_PyFloat_AsFloat(__pyx_t_5); if (unlikely((__pyx_t_20 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_v_dub_float = ((float)__pyx_t_20);
+      __pyx_t_5 = NULL;
+      __pyx_t_3 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_3 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_10};
+        __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_max); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_6); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_dub_float = ((float)__pyx_t_21);
 
       /* "pykdtree/kdtree.pyx":229
  *         cdef double dub_double
  *         if distance_upper_bound is None:
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 dub_float = <float>np.finfo(np.float32).max
  *             else:
@@ -3981,46 +6792,53 @@
  *                 dub_float = <float>np.finfo(np.float32).max
  *             else:
  *                 dub_double = <double>np.finfo(np.float64).max             # <<<<<<<<<<<<<<
  *         else:
  *             if self.data_pts.dtype == np.float32:
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_finfo); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-        if (likely(__pyx_t_7)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-          __Pyx_INCREF(__pyx_t_7);
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_finfo); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_9 = NULL;
+      __pyx_t_3 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_10))) {
+        __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
+        if (likely(__pyx_t_9)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+          __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
+          __Pyx_DECREF_SET(__pyx_t_10, function);
+          __pyx_t_3 = 1;
         }
       }
-      __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_max); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 232, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_v_dub_double = ((double)__pyx_t_21);
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_5};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
+        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      }
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_max); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_22 = __pyx_PyFloat_AsDouble(__pyx_t_10); if (unlikely((__pyx_t_22 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_v_dub_double = ((double)__pyx_t_22);
     }
     __pyx_L17:;
 
     /* "pykdtree/kdtree.pyx":228
  *         cdef float dub_float
  *         cdef double dub_double
  *         if distance_upper_bound is None:             # <<<<<<<<<<<<<<
@@ -4034,40 +6852,40 @@
  *                 dub_double = <double>np.finfo(np.float64).max
  *         else:
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 dub_float = <float>(distance_upper_bound * distance_upper_bound)
  *             else:
  */
   /*else*/ {
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_10, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (__pyx_t_3) {
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (__pyx_t_2) {
 
       /* "pykdtree/kdtree.pyx":235
  *         else:
  *             if self.data_pts.dtype == np.float32:
  *                 dub_float = <float>(distance_upper_bound * distance_upper_bound)             # <<<<<<<<<<<<<<
  *             else:
  *                 dub_double = <double>(distance_upper_bound * distance_upper_bound)
  */
-      __pyx_t_5 = PyNumber_Multiply(__pyx_v_distance_upper_bound, __pyx_v_distance_upper_bound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_20 = __pyx_PyFloat_AsFloat(__pyx_t_5); if (unlikely((__pyx_t_20 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_v_dub_float = ((float)__pyx_t_20);
+      __pyx_t_6 = PyNumber_Multiply(__pyx_v_distance_upper_bound, __pyx_v_distance_upper_bound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_6); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_dub_float = ((float)__pyx_t_21);
 
       /* "pykdtree/kdtree.pyx":234
  *                 dub_double = <double>np.finfo(np.float64).max
  *         else:
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 dub_float = <float>(distance_upper_bound * distance_upper_bound)
  *             else:
@@ -4079,75 +6897,76 @@
  *                 dub_float = <float>(distance_upper_bound * distance_upper_bound)
  *             else:
  *                 dub_double = <double>(distance_upper_bound * distance_upper_bound)             # <<<<<<<<<<<<<<
  * 
  *         # Set epsilon
  */
     /*else*/ {
-      __pyx_t_5 = PyNumber_Multiply(__pyx_v_distance_upper_bound, __pyx_v_distance_upper_bound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 237, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_v_dub_double = ((double)__pyx_t_21);
+      __pyx_t_6 = PyNumber_Multiply(__pyx_v_distance_upper_bound, __pyx_v_distance_upper_bound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_22 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_22 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_dub_double = ((double)__pyx_t_22);
     }
     __pyx_L18:;
   }
   __pyx_L16:;
 
   /* "pykdtree/kdtree.pyx":240
  * 
  *         # Set epsilon
  *         cdef double epsilon_float = <float>eps             # <<<<<<<<<<<<<<
  *         cdef double epsilon_double = <double>eps
  * 
  */
-  __pyx_t_20 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_20 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 240, __pyx_L1_error)
-  __pyx_v_epsilon_float = ((float)__pyx_t_20);
+  __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_v_epsilon_float = ((float)__pyx_t_21);
 
   /* "pykdtree/kdtree.pyx":241
  *         # Set epsilon
  *         cdef double epsilon_float = <float>eps
  *         cdef double epsilon_double = <double>eps             # <<<<<<<<<<<<<<
  * 
  *         # Release GIL and query tree
  */
-  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_v_eps); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L1_error)
-  __pyx_v_epsilon_double = ((double)__pyx_t_21);
+  __pyx_t_22 = __pyx_PyFloat_AsDouble(__pyx_v_eps); if (unlikely((__pyx_t_22 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_v_epsilon_double = ((double)__pyx_t_22);
 
   /* "pykdtree/kdtree.pyx":244
  * 
  *         # Release GIL and query tree
  *         if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 search_tree_float(self._kdtree_float, self._data_pts_data_float,
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__pyx_t_3) {
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_6, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":245
  *         # Release GIL and query tree
  *         if self.data_pts.dtype == np.float32:
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 search_tree_float(self._kdtree_float, self._data_pts_data_float,
  *                                   query_array_data_float, num_qpoints, num_n, dub_float, epsilon_float,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
+        _save = NULL;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
           /* "pykdtree/kdtree.pyx":246
  *         if self.data_pts.dtype == np.float32:
@@ -4195,14 +7014,15 @@
  *                 search_tree_double(self._kdtree_double, self._data_pts_data_double,
  *                                   query_array_data_double, num_qpoints, num_n, dub_double, epsilon_double,
  */
   /*else*/ {
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
+        _save = NULL;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
           /* "pykdtree/kdtree.pyx":252
  *         else:
@@ -4238,140 +7058,92 @@
   /* "pykdtree/kdtree.pyx":257
  * 
  *         # Shape result
  *         if k > 1:             # <<<<<<<<<<<<<<
  *             closest_dists_res = closest_dists.reshape(num_qpoints, k)
  *             closest_idxs_res = closest_idxs.reshape(num_qpoints, k)
  */
-  __pyx_t_4 = PyObject_RichCompare(__pyx_v_k, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 257, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__pyx_t_3) {
+  __pyx_t_5 = PyObject_RichCompare(__pyx_v_k, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 257, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":258
  *         # Shape result
  *         if k > 1:
  *             closest_dists_res = closest_dists.reshape(num_qpoints, k)             # <<<<<<<<<<<<<<
  *             closest_idxs_res = closest_idxs.reshape(num_qpoints, k)
  *         else:
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_closest_dists, __pyx_n_s_reshape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 258, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = NULL;
-    __pyx_t_12 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_7);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_closest_dists, __pyx_n_s_reshape); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_9 = NULL;
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_12 = 1;
+        __Pyx_DECREF_SET(__pyx_t_10, function);
+        __pyx_t_3 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_8)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_v_k};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_v_k};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
     #endif
     {
-      __pyx_t_1 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      if (__pyx_t_7) {
-        __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_7); __pyx_t_7 = NULL;
-      }
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_12, __pyx_t_5);
-      __Pyx_INCREF(__pyx_v_k);
-      __Pyx_GIVEREF(__pyx_v_k);
-      PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_12, __pyx_v_k);
-      __pyx_t_5 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_t_6, __pyx_v_k};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_3, 2+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_v_closest_dists_res = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_v_closest_dists_res = __pyx_t_5;
+    __pyx_t_5 = 0;
 
     /* "pykdtree/kdtree.pyx":259
  *         if k > 1:
  *             closest_dists_res = closest_dists.reshape(num_qpoints, k)
  *             closest_idxs_res = closest_idxs.reshape(num_qpoints, k)             # <<<<<<<<<<<<<<
  *         else:
  *             closest_dists_res = closest_dists
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_closest_idxs), __pyx_n_s_reshape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = NULL;
-    __pyx_t_12 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_closest_idxs), __pyx_n_s_reshape); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_num_qpoints); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_9 = NULL;
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_12 = 1;
+        __Pyx_DECREF_SET(__pyx_t_10, function);
+        __pyx_t_3 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_8)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_k};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_k};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      if (__pyx_t_5) {
-        __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-      }
-      __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_12, __pyx_t_1);
-      __Pyx_INCREF(__pyx_v_k);
-      __Pyx_GIVEREF(__pyx_v_k);
-      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_12, __pyx_v_k);
-      __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_7, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_v_closest_idxs_res = __pyx_t_4;
-    __pyx_t_4 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_t_6, __pyx_v_k};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_3, 2+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    }
+    __pyx_v_closest_idxs_res = __pyx_t_5;
+    __pyx_t_5 = 0;
 
     /* "pykdtree/kdtree.pyx":257
  * 
  *         # Shape result
  *         if k > 1:             # <<<<<<<<<<<<<<
  *             closest_dists_res = closest_dists.reshape(num_qpoints, k)
  *             closest_idxs_res = closest_idxs.reshape(num_qpoints, k)
@@ -4393,64 +7165,63 @@
     /* "pykdtree/kdtree.pyx":262
  *         else:
  *             closest_dists_res = closest_dists
  *             closest_idxs_res = closest_idxs             # <<<<<<<<<<<<<<
  * 
  *         if distance_upper_bound is not None: # Mark out of bounds results
  */
-    __Pyx_INCREF(((PyObject *)__pyx_v_closest_idxs));
+    __Pyx_INCREF((PyObject *)__pyx_v_closest_idxs);
     __pyx_v_closest_idxs_res = ((PyObject *)__pyx_v_closest_idxs);
   }
   __pyx_L26:;
 
   /* "pykdtree/kdtree.pyx":264
  *             closest_idxs_res = closest_idxs
  * 
  *         if distance_upper_bound is not None: # Mark out of bounds results             # <<<<<<<<<<<<<<
  *             if self.data_pts.dtype == np.float32:
  *                 idx_out = (closest_dists_res >= dub_float)
  */
-  __pyx_t_3 = (__pyx_v_distance_upper_bound != Py_None);
-  __pyx_t_10 = (__pyx_t_3 != 0);
-  if (__pyx_t_10) {
+  __pyx_t_2 = (__pyx_v_distance_upper_bound != Py_None);
+  if (__pyx_t_2) {
 
     /* "pykdtree/kdtree.pyx":265
  * 
  *         if distance_upper_bound is not None: # Mark out of bounds results
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 idx_out = (closest_dists_res >= dub_float)
  *             else:
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyObject_RichCompare(__pyx_t_4, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (__pyx_t_10) {
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->data_pts), __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (__pyx_t_2) {
 
       /* "pykdtree/kdtree.pyx":266
  *         if distance_upper_bound is not None: # Mark out of bounds results
  *             if self.data_pts.dtype == np.float32:
  *                 idx_out = (closest_dists_res >= dub_float)             # <<<<<<<<<<<<<<
  *             else:
  *                 idx_out = (closest_dists_res >= dub_double)
  */
-      __pyx_t_8 = PyFloat_FromDouble(__pyx_v_dub_float); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 266, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_7 = PyObject_RichCompare(__pyx_v_closest_dists_res, __pyx_t_8, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_v_idx_out = __pyx_t_7;
-      __pyx_t_7 = 0;
+      __pyx_t_10 = PyFloat_FromDouble(__pyx_v_dub_float); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __pyx_t_6 = PyObject_RichCompare(__pyx_v_closest_dists_res, __pyx_t_10, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_v_idx_out = __pyx_t_6;
+      __pyx_t_6 = 0;
 
       /* "pykdtree/kdtree.pyx":265
  * 
  *         if distance_upper_bound is not None: # Mark out of bounds results
  *             if self.data_pts.dtype == np.float32:             # <<<<<<<<<<<<<<
  *                 idx_out = (closest_dists_res >= dub_float)
  *             else:
@@ -4459,52 +7230,52 @@
     }
 
     /* "pykdtree/kdtree.pyx":268
  *                 idx_out = (closest_dists_res >= dub_float)
  *             else:
  *                 idx_out = (closest_dists_res >= dub_double)             # <<<<<<<<<<<<<<
  * 
- *             closest_dists_res[idx_out] = np.Inf
+ *             closest_dists_res[idx_out] = np.inf
  */
     /*else*/ {
-      __pyx_t_7 = PyFloat_FromDouble(__pyx_v_dub_double); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = PyObject_RichCompare(__pyx_v_closest_dists_res, __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 268, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_v_idx_out = __pyx_t_8;
-      __pyx_t_8 = 0;
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_dub_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 268, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_10 = PyObject_RichCompare(__pyx_v_closest_dists_res, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 268, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_idx_out = __pyx_t_10;
+      __pyx_t_10 = 0;
     }
     __pyx_L28:;
 
     /* "pykdtree/kdtree.pyx":270
  *                 idx_out = (closest_dists_res >= dub_double)
  * 
- *             closest_dists_res[idx_out] = np.Inf             # <<<<<<<<<<<<<<
+ *             closest_dists_res[idx_out] = np.inf             # <<<<<<<<<<<<<<
  *             closest_idxs_res[idx_out] = self.n
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 270, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_Inf); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 270, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_closest_dists_res, __pyx_v_idx_out, __pyx_t_7) < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_inf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely((PyObject_SetItem(__pyx_v_closest_dists_res, __pyx_v_idx_out, __pyx_t_6) < 0))) __PYX_ERR(0, 270, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
     /* "pykdtree/kdtree.pyx":271
  * 
- *             closest_dists_res[idx_out] = np.Inf
+ *             closest_dists_res[idx_out] = np.inf
  *             closest_idxs_res[idx_out] = self.n             # <<<<<<<<<<<<<<
  * 
  *         if not sqr_dists: # Return actual cartesian distances
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 271, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (unlikely(PyObject_SetItem(__pyx_v_closest_idxs_res, __pyx_v_idx_out, __pyx_t_7) < 0)) __PYX_ERR(0, 271, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (unlikely((PyObject_SetItem(__pyx_v_closest_idxs_res, __pyx_v_idx_out, __pyx_t_6) < 0))) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
     /* "pykdtree/kdtree.pyx":264
  *             closest_idxs_res = closest_idxs
  * 
  *         if distance_upper_bound is not None: # Mark out of bounds results             # <<<<<<<<<<<<<<
  *             if self.data_pts.dtype == np.float32:
  *                 idx_out = (closest_dists_res >= dub_float)
@@ -4514,47 +7285,54 @@
   /* "pykdtree/kdtree.pyx":273
  *             closest_idxs_res[idx_out] = self.n
  * 
  *         if not sqr_dists: # Return actual cartesian distances             # <<<<<<<<<<<<<<
  *             closest_dists_res = np.sqrt(closest_dists_res)
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_sqr_dists); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 273, __pyx_L1_error)
-  __pyx_t_3 = ((!__pyx_t_10) != 0);
-  if (__pyx_t_3) {
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_sqr_dists); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_7 = (!__pyx_t_2);
+  if (__pyx_t_7) {
 
     /* "pykdtree/kdtree.pyx":274
  * 
  *         if not sqr_dists: # Return actual cartesian distances
  *             closest_dists_res = np.sqrt(closest_dists_res)             # <<<<<<<<<<<<<<
  * 
  *         return closest_dists_res, closest_idxs_res
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 274, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_8);
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = NULL;
+    __pyx_t_3 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_3 = 1;
       }
     }
-    __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_v_closest_dists_res) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_closest_dists_res);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF_SET(__pyx_v_closest_dists_res, __pyx_t_7);
-    __pyx_t_7 = 0;
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_closest_dists_res};
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __Pyx_DECREF_SET(__pyx_v_closest_dists_res, __pyx_t_6);
+    __pyx_t_6 = 0;
 
     /* "pykdtree/kdtree.pyx":273
  *             closest_idxs_res[idx_out] = self.n
  * 
  *         if not sqr_dists: # Return actual cartesian distances             # <<<<<<<<<<<<<<
  *             closest_dists_res = np.sqrt(closest_dists_res)
  * 
@@ -4565,41 +7343,41 @@
  *             closest_dists_res = np.sqrt(closest_dists_res)
  * 
  *         return closest_dists_res, closest_idxs_res             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(KDTree self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_closest_dists_res);
   __Pyx_GIVEREF(__pyx_v_closest_dists_res);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_closest_dists_res);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_closest_dists_res)) __PYX_ERR(0, 276, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_closest_idxs_res);
   __Pyx_GIVEREF(__pyx_v_closest_idxs_res);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_closest_idxs_res);
-  __pyx_r = __pyx_t_7;
-  __pyx_t_7 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_closest_idxs_res)) __PYX_ERR(0, 276, __pyx_L1_error);
+  __pyx_r = __pyx_t_6;
+  __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "pykdtree/kdtree.pyx":134
  * 
  * 
  *     def query(KDTree self, np.ndarray query_pts not None, k=1, eps=0,             # <<<<<<<<<<<<<<
  *               distance_upper_bound=None, sqr_dists=False, mask=None):
  *         """Query the kd-tree for nearest neighbors
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_closest_dists_double.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_closest_dists_float.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_closest_idxs.rcbuffer->pybuffer);
@@ -4640,16 +7418,18 @@
  *         if self._kdtree_float != NULL:
  *             delete_tree_float(self._kdtree_float)
  */
 
 /* Python wrapper */
 static void __pyx_pw_8pykdtree_6kdtree_6KDTree_7__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_8pykdtree_6kdtree_6KDTree_7__dealloc__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_pf_8pykdtree_6kdtree_6KDTree_6__dealloc__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8pykdtree_6kdtree_6KDTree_6__dealloc__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self) {
@@ -4660,15 +7440,15 @@
   /* "pykdtree/kdtree.pyx":279
  * 
  *     def __dealloc__(KDTree self):
  *         if self._kdtree_float != NULL:             # <<<<<<<<<<<<<<
  *             delete_tree_float(self._kdtree_float)
  *         elif self._kdtree_double != NULL:
  */
-  __pyx_t_1 = ((__pyx_v_self->_kdtree_float != NULL) != 0);
+  __pyx_t_1 = (__pyx_v_self->_kdtree_float != NULL);
   if (__pyx_t_1) {
 
     /* "pykdtree/kdtree.pyx":280
  *     def __dealloc__(KDTree self):
  *         if self._kdtree_float != NULL:
  *             delete_tree_float(self._kdtree_float)             # <<<<<<<<<<<<<<
  *         elif self._kdtree_double != NULL:
@@ -4688,15 +7468,15 @@
 
   /* "pykdtree/kdtree.pyx":281
  *         if self._kdtree_float != NULL:
  *             delete_tree_float(self._kdtree_float)
  *         elif self._kdtree_double != NULL:             # <<<<<<<<<<<<<<
  *             delete_tree_double(self._kdtree_double)
  */
-  __pyx_t_1 = ((__pyx_v_self->_kdtree_double != NULL) != 0);
+  __pyx_t_1 = (__pyx_v_self->_kdtree_double != NULL);
   if (__pyx_t_1) {
 
     /* "pykdtree/kdtree.pyx":282
  *             delete_tree_float(self._kdtree_float)
  *         elif self._kdtree_double != NULL:
  *             delete_tree_double(self._kdtree_double)             # <<<<<<<<<<<<<<
  */
@@ -4730,30 +7510,32 @@
  *     cdef readonly np.ndarray data
  *     cdef float *_data_pts_data_float
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_8data_pts_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_8data_pts_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_8data_pts___get__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_8data_pts___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->data_pts));
+  __Pyx_INCREF((PyObject *)__pyx_v_self->data_pts);
   __pyx_r = ((PyObject *)__pyx_v_self->data_pts);
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -4767,30 +7549,32 @@
  *     cdef float *_data_pts_data_float
  *     cdef double *_data_pts_data_double
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_4data_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_4data_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_4data___get__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_4data___get__(struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->data));
+  __Pyx_INCREF((PyObject *)__pyx_v_self->data);
   __pyx_r = ((PyObject *)__pyx_v_self->data);
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -4804,17 +7588,19 @@
  *     cdef readonly int8_t ndim
  *     cdef readonly uint32_t leafsize
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_1n_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_1n_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_1n___get__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4851,17 +7637,19 @@
  *     cdef readonly uint32_t leafsize
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_4ndim_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_4ndim_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_4ndim___get__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4898,17 +7686,19 @@
  * 
  *     def __cinit__(KDTree self):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_8leafsize_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_8leafsize_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_8leafsize___get__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4936,1180 +7726,289 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8pykdtree_6kdtree_6KDTree_9__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(2, 1, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_8__reduce_cython__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8pykdtree_6kdtree_6KDTree_11__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_10__setstate_cython__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(2, 3, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(2, 3, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v___pyx_state = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 3, __pyx_L3_error)
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8pykdtree_6kdtree_6KDTree_10__setstate_cython__(((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8pykdtree_6kdtree_6KDTree_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8pykdtree_6kdtree_KDTree *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pykdtree.kdtree.KDTree.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":735
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":738
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":741
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":744
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":747
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":751
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
- *     else:
- *         return ()
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
-    goto __pyx_L0;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":753
- *         return <tuple>d.subarray.shape
- *     else:
- *         return ()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
-    goto __pyx_L0;
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":928
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":929
- * 
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
- *     PyArray_SetBaseObject(arr, base)
- * 
- */
-  Py_INCREF(__pyx_v_base);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":930
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object get_array_base(ndarray arr):
- */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":928
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":932
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
-  PyObject *__pyx_v_base;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":933
- * 
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
- *     if base is NULL:
- *         return None
- */
-  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":934
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":935
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- *         return None             # <<<<<<<<<<<<<<
- *     return <object>base
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-    goto __pyx_L0;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":934
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":936
- *     if base is NULL:
- *         return None
- *     return <object>base             # <<<<<<<<<<<<<<
- * 
- * # Versions of the import_* functions which are more suitable for
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_base));
-  __pyx_r = ((PyObject *)__pyx_v_base);
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":932
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":940
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":942
- * cdef inline int import_array() except -1:
- *     try:
- *         __pyx_import_array()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
- */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":943
- *     try:
- *         __pyx_import_array()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":944
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_umath() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 944, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":940
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":946
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":948
- * cdef inline int import_umath() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":949
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":950
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_ufunc() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 950, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":946
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":952
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":954
- * cdef inline int import_ufunc() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":955
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":956
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef extern from *:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 956, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":952
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":966
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":978
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":966
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":981
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":993
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":981
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":996
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1003
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":996
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1006
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1010
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1006
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1013
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1017
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1013
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 static PyObject *__pyx_tp_new_8pykdtree_6kdtree_KDTree(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8pykdtree_6kdtree_KDTree *p;
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   p = ((struct __pyx_obj_8pykdtree_6kdtree_KDTree *)o);
   p->data_pts = ((PyArrayObject *)Py_None); Py_INCREF(Py_None);
   p->data = ((PyArrayObject *)Py_None); Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_8pykdtree_6kdtree_6KDTree_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_8pykdtree_6kdtree_KDTree(PyObject *o) {
   struct __pyx_obj_8pykdtree_6kdtree_KDTree *p = (struct __pyx_obj_8pykdtree_6kdtree_KDTree *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8pykdtree_6kdtree_KDTree) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_8pykdtree_6kdtree_6KDTree_7__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->data_pts);
   Py_CLEAR(p->data);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
   (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
 }
 
 static int __pyx_tp_traverse_8pykdtree_6kdtree_KDTree(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_8pykdtree_6kdtree_KDTree *p = (struct __pyx_obj_8pykdtree_6kdtree_KDTree *)o;
   if (p->data_pts) {
     e = (*v)(((PyObject *)p->data_pts), a); if (e) return e;
@@ -6149,32 +8048,52 @@
 }
 
 static PyObject *__pyx_getprop_8pykdtree_6kdtree_6KDTree_leafsize(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_8pykdtree_6kdtree_6KDTree_8leafsize_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_8pykdtree_6kdtree_KDTree[] = {
-  {"query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_5query, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8pykdtree_6kdtree_6KDTree_4query},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__, METH_O, 0},
+  {"query", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_5query, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8pykdtree_6kdtree_6KDTree_4query},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8pykdtree_6kdtree_6KDTree_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_8pykdtree_6kdtree_KDTree[] = {
   {(char *)"data_pts", __pyx_getprop_8pykdtree_6kdtree_6KDTree_data_pts, 0, (char *)0, 0},
   {(char *)"data", __pyx_getprop_8pykdtree_6kdtree_6KDTree_data, 0, (char *)0, 0},
   {(char *)"n", __pyx_getprop_8pykdtree_6kdtree_6KDTree_n, 0, (char *)0, 0},
   {(char *)"ndim", __pyx_getprop_8pykdtree_6kdtree_6KDTree_ndim, 0, (char *)0, 0},
   {(char *)"leafsize", __pyx_getprop_8pykdtree_6kdtree_6KDTree_leafsize, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8pykdtree_6kdtree_KDTree_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8pykdtree_6kdtree_KDTree},
+  {Py_tp_doc, (void *)PyDoc_STR("kd-tree for fast nearest-neighbour lookup.\n    The interface is made to resemble the scipy.spatial kd-tree except\n    only Euclidean distance measure is supported.\n\n    :Parameters:\n    data_pts : numpy array\n        Data points with shape (n , dims)\n    leafsize : int, optional\n        Maximum number of data points in tree leaf\n    ")},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_8pykdtree_6kdtree_KDTree},
+  {Py_tp_clear, (void *)__pyx_tp_clear_8pykdtree_6kdtree_KDTree},
+  {Py_tp_methods, (void *)__pyx_methods_8pykdtree_6kdtree_KDTree},
+  {Py_tp_getset, (void *)__pyx_getsets_8pykdtree_6kdtree_KDTree},
+  {Py_tp_init, (void *)__pyx_pw_8pykdtree_6kdtree_6KDTree_3__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_8pykdtree_6kdtree_KDTree},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8pykdtree_6kdtree_KDTree_spec = {
+  "pykdtree.kdtree.KDTree",
+  sizeof(struct __pyx_obj_8pykdtree_6kdtree_KDTree),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
+  __pyx_type_8pykdtree_6kdtree_KDTree_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_8pykdtree_6kdtree_KDTree = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pykdtree.kdtree.KDTree", /*tp_name*/
+  "pykdtree.kdtree.""KDTree", /*tp_name*/
   sizeof(struct __pyx_obj_8pykdtree_6kdtree_KDTree), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8pykdtree_6kdtree_KDTree, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -6195,309 +8114,380 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  "kd-tree for fast nearest-neighbour lookup.\n    The interface is made to resemble the scipy.spatial kd-tree except\n    only Euclidean distance measure is supported.\n\n    :Parameters:\n    data_pts : numpy array\n        Data points with shape (n , dims)\n    leafsize : int, optional\n        Maximum number of data points in tree leaf\n    ", /*tp_doc*/
+  PyDoc_STR("kd-tree for fast nearest-neighbour lookup.\n    The interface is made to resemble the scipy.spatial kd-tree except\n    only Euclidean distance measure is supported.\n\n    :Parameters:\n    data_pts : numpy array\n        Data points with shape (n , dims)\n    leafsize : int, optional\n        Maximum number of data points in tree leaf\n    "), /*tp_doc*/
   __pyx_tp_traverse_8pykdtree_6kdtree_KDTree, /*tp_traverse*/
   __pyx_tp_clear_8pykdtree_6kdtree_KDTree, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_8pykdtree_6kdtree_KDTree, /*tp_methods*/
   0, /*tp_members*/
   __pyx_getsets_8pykdtree_6kdtree_KDTree, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   __pyx_pw_8pykdtree_6kdtree_6KDTree_3__init__, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_8pykdtree_6kdtree_KDTree, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_kdtree(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_kdtree},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "kdtree",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_Data_and_query_points_must_have, __pyx_k_Data_and_query_points_must_have, sizeof(__pyx_k_Data_and_query_points_must_have), 0, 1, 0, 0},
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_Inf, __pyx_k_Inf, sizeof(__pyx_k_Inf), 0, 0, 1, 1},
-  {&__pyx_n_s_KDTree, __pyx_k_KDTree, sizeof(__pyx_k_KDTree), 0, 0, 1, 1},
-  {&__pyx_kp_u_Mask_must_have_the_same_size_as, __pyx_k_Mask_must_have_the_same_size_as, sizeof(__pyx_k_Mask_must_have_the_same_size_as), 0, 1, 0, 0},
-  {&__pyx_kp_u_Max_127_dimensions_allowed, __pyx_k_Max_127_dimensions_allowed, sizeof(__pyx_k_Max_127_dimensions_allowed), 0, 1, 0, 0},
-  {&__pyx_kp_u_Number_of_neighbours_must_be_gre, __pyx_k_Number_of_neighbours_must_be_gre, sizeof(__pyx_k_Number_of_neighbours_must_be_gre), 0, 1, 0, 0},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Type_mismatch_query_points_must, __pyx_k_Type_mismatch_query_points_must, sizeof(__pyx_k_Type_mismatch_query_points_must), 0, 1, 0, 0},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_data_pts, __pyx_k_data_pts, sizeof(__pyx_k_data_pts), 0, 0, 1, 1},
-  {&__pyx_n_s_distance_upper_bound, __pyx_k_distance_upper_bound, sizeof(__pyx_k_distance_upper_bound), 0, 0, 1, 1},
-  {&__pyx_kp_u_distance_upper_bound_must_be_non, __pyx_k_distance_upper_bound_must_be_non, sizeof(__pyx_k_distance_upper_bound_must_be_non), 0, 1, 0, 0},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
-  {&__pyx_n_s_eps, __pyx_k_eps, sizeof(__pyx_k_eps), 0, 0, 1, 1},
-  {&__pyx_kp_u_eps_must_be_non_negative, __pyx_k_eps_must_be_non_negative, sizeof(__pyx_k_eps_must_be_non_negative), 0, 1, 0, 0},
-  {&__pyx_n_s_finfo, __pyx_k_finfo, sizeof(__pyx_k_finfo), 0, 0, 1, 1},
-  {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
-  {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
-  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
-  {&__pyx_n_s_leafsize, __pyx_k_leafsize, sizeof(__pyx_k_leafsize), 0, 0, 1, 1},
-  {&__pyx_kp_u_leafsize_must_be_greater_than_ze, __pyx_k_leafsize_must_be_greater_than_ze, sizeof(__pyx_k_leafsize_must_be_greater_than_ze), 0, 1, 0, 0},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_mask, __pyx_k_mask, sizeof(__pyx_k_mask), 0, 0, 1, 1},
-  {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
-  {&__pyx_n_s_query_pts, __pyx_k_query_pts, sizeof(__pyx_k_query_pts), 0, 0, 1, 1},
-  {&__pyx_n_s_ravel, __pyx_k_ravel, sizeof(__pyx_k_ravel), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
-  {&__pyx_n_s_sqr_dists, __pyx_k_sqr_dists, sizeof(__pyx_k_sqr_dists), 0, 0, 1, 1},
-  {&__pyx_n_s_sqrt, __pyx_k_sqrt, sizeof(__pyx_k_sqrt), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
-  {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_s_Data_and_query_points_must_have, __pyx_k_Data_and_query_points_must_have, sizeof(__pyx_k_Data_and_query_points_must_have), 0, 0, 1, 0},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_KDTree, __pyx_k_KDTree, sizeof(__pyx_k_KDTree), 0, 0, 1, 1},
+    {&__pyx_n_s_KDTree___reduce_cython, __pyx_k_KDTree___reduce_cython, sizeof(__pyx_k_KDTree___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_KDTree___setstate_cython, __pyx_k_KDTree___setstate_cython, sizeof(__pyx_k_KDTree___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_KDTree_query, __pyx_k_KDTree_query, sizeof(__pyx_k_KDTree_query), 0, 0, 1, 1},
+    {&__pyx_kp_s_Mask_must_have_the_same_size_as, __pyx_k_Mask_must_have_the_same_size_as, sizeof(__pyx_k_Mask_must_have_the_same_size_as), 0, 0, 1, 0},
+    {&__pyx_kp_s_Max_127_dimensions_allowed, __pyx_k_Max_127_dimensions_allowed, sizeof(__pyx_k_Max_127_dimensions_allowed), 0, 0, 1, 0},
+    {&__pyx_kp_s_Number_of_neighbours_must_be_gre, __pyx_k_Number_of_neighbours_must_be_gre, sizeof(__pyx_k_Number_of_neighbours_must_be_gre), 0, 0, 1, 0},
+    {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
+    {&__pyx_kp_s_Type_mismatch_query_points_must, __pyx_k_Type_mismatch_query_points_must, sizeof(__pyx_k_Type_mismatch_query_points_must), 0, 0, 1, 0},
+    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 1},
+    {&__pyx_n_s__19, __pyx_k__19, sizeof(__pyx_k__19), 0, 0, 1, 1},
+    {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists, __pyx_k_closest_dists, sizeof(__pyx_k_closest_dists), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists_data_double, __pyx_k_closest_dists_data_double, sizeof(__pyx_k_closest_dists_data_double), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists_data_float, __pyx_k_closest_dists_data_float, sizeof(__pyx_k_closest_dists_data_float), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists_double, __pyx_k_closest_dists_double, sizeof(__pyx_k_closest_dists_double), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists_float, __pyx_k_closest_dists_float, sizeof(__pyx_k_closest_dists_float), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_dists_res, __pyx_k_closest_dists_res, sizeof(__pyx_k_closest_dists_res), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_idxs, __pyx_k_closest_idxs, sizeof(__pyx_k_closest_idxs), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_idxs_data, __pyx_k_closest_idxs_data, sizeof(__pyx_k_closest_idxs_data), 0, 0, 1, 1},
+    {&__pyx_n_s_closest_idxs_res, __pyx_k_closest_idxs_res, sizeof(__pyx_k_closest_idxs_res), 0, 0, 1, 1},
+    {&__pyx_n_s_data_pts, __pyx_k_data_pts, sizeof(__pyx_k_data_pts), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_distance_upper_bound, __pyx_k_distance_upper_bound, sizeof(__pyx_k_distance_upper_bound), 0, 0, 1, 1},
+    {&__pyx_kp_s_distance_upper_bound_must_be_non, __pyx_k_distance_upper_bound_must_be_non, sizeof(__pyx_k_distance_upper_bound_must_be_non), 0, 0, 1, 0},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_dub_double, __pyx_k_dub_double, sizeof(__pyx_k_dub_double), 0, 0, 1, 1},
+    {&__pyx_n_s_dub_float, __pyx_k_dub_float, sizeof(__pyx_k_dub_float), 0, 0, 1, 1},
+    {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_eps, __pyx_k_eps, sizeof(__pyx_k_eps), 0, 0, 1, 1},
+    {&__pyx_kp_s_eps_must_be_non_negative, __pyx_k_eps_must_be_non_negative, sizeof(__pyx_k_eps_must_be_non_negative), 0, 0, 1, 0},
+    {&__pyx_n_s_epsilon_double, __pyx_k_epsilon_double, sizeof(__pyx_k_epsilon_double), 0, 0, 1, 1},
+    {&__pyx_n_s_epsilon_float, __pyx_k_epsilon_float, sizeof(__pyx_k_epsilon_float), 0, 0, 1, 1},
+    {&__pyx_n_s_finfo, __pyx_k_finfo, sizeof(__pyx_k_finfo), 0, 0, 1, 1},
+    {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
+    {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+    {&__pyx_n_s_idx_out, __pyx_k_idx_out, sizeof(__pyx_k_idx_out), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
+    {&__pyx_n_s_leafsize, __pyx_k_leafsize, sizeof(__pyx_k_leafsize), 0, 0, 1, 1},
+    {&__pyx_kp_s_leafsize_must_be_greater_than_ze, __pyx_k_leafsize_must_be_greater_than_ze, sizeof(__pyx_k_leafsize_must_be_greater_than_ze), 0, 0, 1, 0},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_mask, __pyx_k_mask, sizeof(__pyx_k_mask), 0, 0, 1, 1},
+    {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_num_n, __pyx_k_num_n, sizeof(__pyx_k_num_n), 0, 0, 1, 1},
+    {&__pyx_n_s_num_qpoints, __pyx_k_num_qpoints, sizeof(__pyx_k_num_qpoints), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
+    {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
+    {&__pyx_n_s_pykdtree_kdtree, __pyx_k_pykdtree_kdtree, sizeof(__pyx_k_pykdtree_kdtree), 0, 0, 1, 1},
+    {&__pyx_kp_s_pykdtree_kdtree_pyx, __pyx_k_pykdtree_kdtree_pyx, sizeof(__pyx_k_pykdtree_kdtree_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+    {&__pyx_n_s_q_ndim, __pyx_k_q_ndim, sizeof(__pyx_k_q_ndim), 0, 0, 1, 1},
+    {&__pyx_n_s_query, __pyx_k_query, sizeof(__pyx_k_query), 0, 0, 1, 1},
+    {&__pyx_n_s_query_array_data_double, __pyx_k_query_array_data_double, sizeof(__pyx_k_query_array_data_double), 0, 0, 1, 1},
+    {&__pyx_n_s_query_array_data_float, __pyx_k_query_array_data_float, sizeof(__pyx_k_query_array_data_float), 0, 0, 1, 1},
+    {&__pyx_n_s_query_array_double, __pyx_k_query_array_double, sizeof(__pyx_k_query_array_double), 0, 0, 1, 1},
+    {&__pyx_n_s_query_array_float, __pyx_k_query_array_float, sizeof(__pyx_k_query_array_float), 0, 0, 1, 1},
+    {&__pyx_n_s_query_mask, __pyx_k_query_mask, sizeof(__pyx_k_query_mask), 0, 0, 1, 1},
+    {&__pyx_n_s_query_mask_data, __pyx_k_query_mask_data, sizeof(__pyx_k_query_mask_data), 0, 0, 1, 1},
+    {&__pyx_n_s_query_pts, __pyx_k_query_pts, sizeof(__pyx_k_query_pts), 0, 0, 1, 1},
+    {&__pyx_n_s_ravel, __pyx_k_ravel, sizeof(__pyx_k_ravel), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+    {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_sqr_dists, __pyx_k_sqr_dists, sizeof(__pyx_k_sqr_dists), 0, 0, 1, 1},
+    {&__pyx_n_s_sqrt, __pyx_k_sqrt, sizeof(__pyx_k_sqrt), 0, 0, 1, 1},
+    {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
+    {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 95, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 983, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 983, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+
+  /* "../../../../../tmp/build-env-iyio0mvh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
   /* "pykdtree/kdtree.pyx":95
  *         # Check arguments
  *         if leafsize < 1:
  *             raise ValueError('leafsize must be greater than zero')             # <<<<<<<<<<<<<<
  * 
  *         # Get data content
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_leafsize_must_be_greater_than_ze); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_leafsize_must_be_greater_than_ze); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "pykdtree/kdtree.pyx":119
  *             self.ndim = 1
  *         elif data_pts.shape[1] > 127:
  *             raise ValueError('Max 127 dimensions allowed')             # <<<<<<<<<<<<<<
  *         else:
  *             self.ndim = <int8_t>data_pts.shape[1]
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Max_127_dimensions_allowed); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Max_127_dimensions_allowed); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "pykdtree/kdtree.pyx":163
  *         # Check arguments
  *         if k < 1:
  *             raise ValueError('Number of neighbours must be greater than zero')             # <<<<<<<<<<<<<<
  *         elif eps < 0:
  *             raise ValueError('eps must be non-negative')
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Number_of_neighbours_must_be_gre); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Number_of_neighbours_must_be_gre); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "pykdtree/kdtree.pyx":165
  *             raise ValueError('Number of neighbours must be greater than zero')
  *         elif eps < 0:
  *             raise ValueError('eps must be non-negative')             # <<<<<<<<<<<<<<
  *         elif distance_upper_bound is not None:
  *             if distance_upper_bound < 0:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_eps_must_be_non_negative); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 165, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_eps_must_be_non_negative); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "pykdtree/kdtree.pyx":168
  *         elif distance_upper_bound is not None:
  *             if distance_upper_bound < 0:
  *                 raise ValueError('distance_upper_bound must be non negative')             # <<<<<<<<<<<<<<
  * 
  *         # Check dimensions
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_distance_upper_bound_must_be_non); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 168, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_distance_upper_bound_must_be_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "pykdtree/kdtree.pyx":177
  * 
  *         if self.ndim != q_ndim:
  *             raise ValueError('Data and query points must have same dimensions')             # <<<<<<<<<<<<<<
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Data_and_query_points_must_have); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Data_and_query_points_must_have); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "pykdtree/kdtree.pyx":180
  * 
  *         if self.data_pts.dtype == np.float32 and query_pts.dtype != np.float32:
  *             raise TypeError('Type mismatch. query points must be of type float32 when data points are of type float32')             # <<<<<<<<<<<<<<
  * 
  *         # Get query info
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Type_mismatch_query_points_must); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Type_mismatch_query_points_must); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "pykdtree/kdtree.pyx":204
  * 
  *         if mask is not None and mask.size != self.n:
  *             raise ValueError('Mask must have the same size as data points')             # <<<<<<<<<<<<<<
  *         elif mask is not None:
  *             query_mask = np.ascontiguousarray(mask.ravel(), dtype=np.uint8)
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Mask_must_have_the_same_size_as); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Mask_must_have_the_same_size_as); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":944
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+  /* "pykdtree/kdtree.pyx":134
  * 
- * cdef inline int import_umath() except -1:
- */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":950
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
- * cdef inline int import_ufunc() except -1:
+ *     def query(KDTree self, np.ndarray query_pts not None, k=1, eps=0,             # <<<<<<<<<<<<<<
+ *               distance_upper_bound=None, sqr_dists=False, mask=None):
+ *         """Query the kd-tree for nearest neighbors
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(30, __pyx_n_s_self, __pyx_n_s_query_pts, __pyx_n_s_k, __pyx_n_s_eps, __pyx_n_s_distance_upper_bound, __pyx_n_s_sqr_dists, __pyx_n_s_mask, __pyx_n_s_q_ndim, __pyx_n_s_num_qpoints, __pyx_n_s_num_n, __pyx_n_s_closest_idxs, __pyx_n_s_closest_dists_float, __pyx_n_s_closest_dists_double, __pyx_n_s_closest_idxs_data, __pyx_n_s_closest_dists_data_float, __pyx_n_s_closest_dists_data_double, __pyx_n_s_query_array_float, __pyx_n_s_query_array_double, __pyx_n_s_query_array_data_float, __pyx_n_s_query_array_data_double, __pyx_n_s_query_mask, __pyx_n_s_query_mask_data, __pyx_n_s_closest_dists, __pyx_n_s_dub_float, __pyx_n_s_dub_double, __pyx_n_s_epsilon_float, __pyx_n_s_epsilon_double, __pyx_n_s_closest_dists_res, __pyx_n_s_closest_idxs_res, __pyx_n_s_idx_out); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pykdtree_kdtree_pyx, __pyx_n_s_query, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_int_1, __pyx_int_0, Py_None, Py_False, Py_None); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(2, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#ifndef NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -6530,24 +8520,37 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8pykdtree_6kdtree_KDTree.tp_print = 0;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8pykdtree_6kdtree_KDTree = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8pykdtree_6kdtree_KDTree_spec, NULL); if (unlikely(!__pyx_ptype_8pykdtree_6kdtree_KDTree)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8pykdtree_6kdtree_KDTree_spec, __pyx_ptype_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  #else
+  __pyx_ptype_8pykdtree_6kdtree_KDTree = &__pyx_type_8pykdtree_6kdtree_KDTree;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8pykdtree_6kdtree_KDTree->tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8pykdtree_6kdtree_KDTree.tp_dictoffset && __pyx_type_8pykdtree_6kdtree_KDTree.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8pykdtree_6kdtree_KDTree.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8pykdtree_6kdtree_KDTree->tp_dictoffset && __pyx_ptype_8pykdtree_6kdtree_KDTree->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8pykdtree_6kdtree_KDTree->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_KDTree, (PyObject *)&__pyx_type_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
-  __pyx_ptype_8pykdtree_6kdtree_KDTree = &__pyx_type_8pykdtree_6kdtree_KDTree;
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_KDTree, (PyObject *) __pyx_ptype_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8pykdtree_6kdtree_KDTree) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6557,55 +8560,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 865, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6624,14 +8613,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_kdtree(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_kdtree},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "kdtree",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -6674,42 +8712,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -6717,28 +8769,62 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_kdtree(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'kdtree' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("kdtree", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to kdtree pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -6749,141 +8835,177 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("kdtree", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pykdtree__kdtree) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pykdtree.kdtree")) {
-      if (unlikely(PyDict_SetItemString(modules, "pykdtree.kdtree", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "pykdtree.kdtree", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "pykdtree/kdtree.pyx":18
  * # with this program.  If not, see <http://www.gnu.org/licenses/>.
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * from libc.stdint cimport uint32_t, int8_t, uint8_t
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pykdtree/kdtree.pyx":134
+ * 
+ * 
+ *     def query(KDTree self, np.ndarray query_pts not None, k=1, eps=0,             # <<<<<<<<<<<<<<
+ *               distance_upper_bound=None, sqr_dists=False, mask=None):
+ *         """Query the kd-tree for nearest neighbors
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8pykdtree_6kdtree_6KDTree_5query, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_KDTree_query, NULL, __pyx_n_s_pykdtree_kdtree, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__14);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8pykdtree_6kdtree_KDTree, __pyx_n_s_query, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8pykdtree_6kdtree_KDTree);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8pykdtree_6kdtree_6KDTree_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_KDTree___reduce_cython, NULL, __pyx_n_s_pykdtree_kdtree, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8pykdtree_6kdtree_6KDTree_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_KDTree___setstate_cython, NULL, __pyx_n_s_pykdtree_kdtree, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pykdtree/kdtree.pyx":1
  * #pykdtree, Fast kd-tree implementation with OpenMP-enabled queries             # <<<<<<<<<<<<<<
  * #
  * #Copyright (C) 2013 - present  Esben S. Nielsen
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../miniconda3/envs/satpy_py310/lib/python3.10/site-packages/numpy/__init__.pxd":1013
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init pykdtree.kdtree", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init pykdtree.kdtree");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -6895,42 +9017,729 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -6951,46 +9760,80 @@
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
-    PyObject *kwdict,
+    PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
-    if (!kw_allowed && PyDict_Next(kwdict, &pos, &key, 0))
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
         goto invalid_keyword;
     return 1;
 #else
-    while (PyDict_Next(kwdict, &pos, &key, 0)) {
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        Py_ssize_t kwsize;
+#if CYTHON_ASSUME_SAFE_MACROS
+        kwsize = PyTuple_GET_SIZE(kw);
+#else
+        kwsize = PyTuple_Size(kw);
+        if (kwsize < 0) return 0;
+#endif
+        if (unlikely(kwsize == 0))
+            return 1;
+        if (!kw_allowed) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, 0);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            goto invalid_keyword;
+        }
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < kwsize; pos++) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, pos);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+        }
+#endif
+        return 1;
+    }
+    while (PyDict_Next(kw, &pos, &key, 0)) {
         #if PY_MAJOR_VERSION < 3
         if (unlikely(!PyString_Check(key)))
         #endif
             if (unlikely(!PyUnicode_Check(key)))
                 goto invalid_keyword_type;
     }
-    if ((!kw_allowed) && unlikely(key))
+    if (!kw_allowed && unlikely(key))
         goto invalid_keyword;
     return 1;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     return 0;
 #endif
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
 /* RaiseDoubleKeywords */
@@ -7006,38 +9849,83 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        Py_XDECREF(key); key = NULL;
+        Py_XDECREF(value); value = NULL;
+        if (kwds_is_tuple) {
+            Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(kwds);
+#else
+            size = PyTuple_Size(kwds);
+            if (size < 0) goto bad;
+#endif
+            if (pos >= size) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            key = __Pyx_PySequence_ITEM(kwds, pos);
+            if (!key) goto bad;
+#elif CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kwds, pos);
+#else
+            key = PyTuple_GetItem(kwds, pos);
+            if (!key) goto bad;
+#endif
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(key);
+#endif
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(value); // transfer ownership of value to values
+            Py_DECREF(key);
+#endif
+            key = NULL;
+            value = NULL;
             continue;
         }
+#if !CYTHON_AVOID_BORROWED_REFS
+        Py_INCREF(key);
+#endif
+        Py_INCREF(value);
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;  // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -7050,22 +9938,26 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL; // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -7084,259 +9976,67 @@
             goto invalid_keyword_type;
         if (kwds2) {
             if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
         } else {
             goto invalid_keyword;
         }
     }
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return 0;
 arg_passed_twice:
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return -1;
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -7372,14 +10072,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -7391,15 +10099,15 @@
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -7420,15 +10128,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -7436,15 +10143,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -7507,15 +10214,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -7529,109 +10235,113 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result = 0;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
+    Py_DECREF(argstuple);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
 #else
-    if (likely(PyCFunction_Check(func)))
+        if (PyCFunction_Check(func))
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
     }
-}
 #endif
-
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    #if Py_VERSION_HEX < 0x03090000
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    #else
+    vectorcallfunc f = PyVectorcall_Function(func);
+    #endif
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-#endif
 
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
@@ -7714,15 +10424,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -7764,15 +10474,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -7796,15 +10507,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -7961,56 +10673,62 @@
       }
     }
   } while (ctx->enc_count);
   ctx->enc_type = 0;
   ctx->is_complex = 0;
   return 0;
 }
-static PyObject *
+static int
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
     int i = 0, number, ndim;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
-        return NULL;
+        return -1;
     }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return -1;
     ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
+        if (number == -1) return -1;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i]) {
+            PyErr_Format(PyExc_ValueError,
                         "Expected a dimension of size %zu, got %d",
                         ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
+            return -1;
+        }
+        if (*ts != ',' && *ts != ')') {
+            PyErr_Format(PyExc_ValueError,
                                 "Expected a comma in format string, got '%c'", *ts);
+            return -1;
+        }
         if (*ts == ',') ts++;
         i++;
     }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+    if (i != ndim) {
+        PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
                             ctx->head->field->type->ndim, i);
+        return -1;
+    }
     if (!*ts) {
         PyErr_SetString(PyExc_ValueError,
                         "Unexpected end of format string, expected ')'");
-        return NULL;
+        return -1;
     }
     ctx->is_valid_array = 1;
     ctx->new_count = 1;
     *tsp = ++ts;
-    return Py_None;
+    return 0;
 }
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
   int got_Z = 0;
   while (1) {
     switch(*ts) {
       case 0:
         if (ctx->enc_type != 0 && ctx->head == NULL) {
@@ -8128,15 +10846,15 @@
         break;
       case ':':
         ++ts;
         while(*ts != ':') ++ts;
         ++ts;
         break;
       case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        if (__pyx_buffmt_parse_array(ctx, &ts) < 0) return NULL;
         break;
       default:
         {
           int number = __Pyx_BufFmt_ExpectNumber(&ts);
           if (number == -1) return NULL;
           ctx->new_count = (size_t)number;
         }
@@ -8193,209 +10911,396 @@
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
-/* PyObjectCall2Args */
-  static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
     }
-    return exc_info;
+#endif
+    return 0;
 }
 #endif
 
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
+/* PyObjectCallNoArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+
+/* PyObjectCallOneArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
-#endif
 
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+/* PyObjectGetMethod */
+  static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
     }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
 #endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
     }
+#endif
+    *method = attr;
     return 0;
 }
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+
+/* PyObjectCallMethod0 */
+  static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
 }
-#endif
 
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+/* ValidateBasesTuple */
+  #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n;
+#if CYTHON_ASSUME_SAFE_MACROS
+    n = PyTuple_GET_SIZE(bases);
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+    n = PyTuple_Size(bases);
+    if (n < 0) return -1;
 #endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+    for (i = 1; i < n; i++)
+    {
+#if CYTHON_AVOID_BORROWED_REFS
+        PyObject *b0 = PySequence_GetItem(bases, i);
+        if (!b0) return -1;
+#elif CYTHON_ASSUME_SAFE_MACROS
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
 #else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
+        PyObject *b0 = PyTuple_GetItem(bases, i);
+        if (!b0) return -1;
 #endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#if !CYTHON_USE_TYPE_SLOTS
+        if (dictoffset == 0) {
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%s.200s': "
+                "unable to validate whether bases have a __dict__ "
+                "when CYTHON_USE_TYPE_SLOTS is off "
+                "(likely because you are building in the limited API). "
+                "Therefore, all extension types with multiple bases "
+                "must add 'cdef dict __dict__' in this compilation mode",
+                type_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
 #else
-    if (unlikely(PyErr_Occurred()))
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+        Py_DECREF(b0);
 #endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
     }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+  static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
     {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
     #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
     #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
 #else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
 #endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
 }
 
 /* PyObject_GenericGetAttrNoDict */
   #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -8427,41 +11332,20 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
-/* PyObjectGetAttrStrNoError */
-  static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
 /* SetupReduce */
-  static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
+  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
   }
   if (unlikely(ret < 0)) {
       PyErr_Clear();
@@ -8519,15 +11403,15 @@
             reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
             if (likely(reduce_cython)) {
                 ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
             } else if (reduce == object_reduce || PyErr_Occurred()) {
                 goto __PYX_BAD;
             }
-            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
+            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
                 setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
                 if (likely(setstate_cython)) {
                     ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                     ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 } else if (!setstate || PyErr_Occurred()) {
@@ -8535,16 +11419,21 @@
                 }
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
     goto __PYX_GOOD;
 __PYX_BAD:
-    if (!PyErr_Occurred())
-        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
+    if (!PyErr_Occurred()) {
+        __Pyx_TypeName type_obj_name =
+            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
+        PyErr_Format(PyExc_RuntimeError,
+            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
+        __Pyx_DECREF_TypeName(type_obj_name);
+    }
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
     Py_XDECREF(object_getstate);
     Py_XDECREF(getstate);
@@ -8552,63 +11441,83 @@
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
+#endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_2
+#define __PYX_HAVE_RT_ImportType_3_0_2
+static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8616,99 +11525,1387 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__11;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
+        if (unlikely(!op->func_doc)) return NULL;
+#else
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+#endif
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_name = PyObject_GetAttrString(op->func, "__name__");
+#elif PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+#if CYTHON_ASSUME_SAFE_MACROS
+        PyList_SET_ITEM(fromlist, 0, marker);
+#else
+        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
+            Py_DECREF(marker);
+            Py_DECREF(fromlist);
+            return NULL;
+        }
+#endif
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *
+__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_GetAttrString(op->func, "__module__");
+}
+static int
+__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_SetAttrString(op->func, "__module__", value);
+}
+#endif
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+#if CYTHON_COMPILING_IN_LIMITED_API
+    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
+#endif
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#endif
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+#endif
+    if (unlikely(op == NULL))
+        return NULL;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
+    if (unlikely(!op->func)) return NULL;
+#endif
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+#endif
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    Py_XINCREF(module);
+    cf->m_module = module;
+#endif
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_CLEAR(m->func);
+#else
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+#endif
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(m->func);
+#else
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+#endif
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+#endif
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
+    PyObject *py_name = NULL;
+    PyCFunction meth;
+    int flags;
+    meth = PyCFunction_GetFunction(f);
+    if (unlikely(!meth)) return NULL;
+    flags = PyCFunction_GetFlags(f);
+    if (unlikely(flags < 0)) return NULL;
+#else
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    int flags = f->m_ml->ml_flags;
+#endif
+    Py_ssize_t size;
+    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+#endif
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+#endif
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+#if CYTHON_COMPILING_IN_LIMITED_API
+    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+    if (!py_name) return NULL;
+    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
+                 py_name);
+    Py_DECREF(py_name);
+#else
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+#endif
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *self, *result;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
+    if (unlikely(!self) && PyErr_Occurred()) return NULL;
+#else
+    self = ((PyCFunctionObject*)func)->m_self;
+#endif
+    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
+    return result;
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+#if CYTHON_ASSUME_SAFE_MACROS
+        argc = PyTuple_GET_SIZE(args);
+#else
+        argc = PyTuple_Size(args);
+        if (unlikely(!argc) < 0) return NULL;
+#endif
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -8722,15 +12919,16 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -8800,25 +12998,107 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyCode_Replace_For_AddTraceback(PyObject *code, PyObject *scratch_dict,
+                                                       PyObject *firstlineno, PyObject *name) {
+    PyObject *replace = NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_firstlineno", firstlineno))) return NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_name", name))) return NULL;
+    replace = PyObject_GetAttrString(code, "replace");
+    if (likely(replace)) {
+        PyObject *result;
+        result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
+        Py_DECREF(replace);
+        return result;
+    }
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
+    PyErr_Clear();
+    {
+        PyObject *compiled = NULL, *result = NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
+        compiled = Py_CompileString(
+            "out = type(code)(\n"
+            "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
+            "  code.co_flags, code.co_code, code.co_consts, code.co_names,\n"
+            "  code.co_varnames, code.co_filename, co_name, co_firstlineno,\n"
+            "  code.co_lnotab)\n", "<dummy>", Py_file_input);
+        if (!compiled) return NULL;
+        result = PyEval_EvalCode(compiled, scratch_dict, scratch_dict);
+        Py_DECREF(compiled);
+        if (!result) PyErr_Print();
+        Py_DECREF(result);
+        result = PyDict_GetItemString(scratch_dict, "out");
+        if (result) Py_INCREF(result);
+        return result;
+    }
+    #endif
+}
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
+    PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
+    PyObject *exc_type, *exc_value, *exc_traceback;
+    int success = 0;
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    PyErr_Fetch(&exc_type, &exc_value, &exc_traceback);
+    code_object = Py_CompileString("_getframe()", filename, Py_eval_input);
+    if (unlikely(!code_object)) goto bad;
+    py_py_line = PyLong_FromLong(py_line);
+    if (unlikely(!py_py_line)) goto bad;
+    py_funcname = PyUnicode_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    dict = PyDict_New();
+    if (unlikely(!dict)) goto bad;
+    {
+        PyObject *old_code_object = code_object;
+        code_object = __Pyx_PyCode_Replace_For_AddTraceback(code_object, dict, py_py_line, py_funcname);
+        Py_DECREF(old_code_object);
+    }
+    if (unlikely(!code_object)) goto bad;
+    getframe = PySys_GetObject("_getframe");
+    if (unlikely(!getframe)) goto bad;
+    if (unlikely(PyDict_SetItemString(dict, "_getframe", getframe))) goto bad;
+    frame = PyEval_EvalCode(code_object, dict, dict);
+    if (unlikely(!frame) || frame == Py_None) goto bad;
+    success = 1;
+  bad:
+    PyErr_Restore(exc_type, exc_value, exc_traceback);
+    Py_XDECREF(code_object);
+    Py_XDECREF(py_py_line);
+    Py_XDECREF(py_funcname);
+    Py_XDECREF(dict);
+    Py_XDECREF(replace);
+    if (success) {
+        PyTraceBack_Here(
+            (struct _frame*)frame);
+    }
+    Py_XDECREF(frame);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -8845,14 +13125,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -8907,19 +13188,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -8951,15 +13238,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -8971,15 +13258,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -9079,15 +13366,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -9105,15 +13392,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -9125,15 +13412,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -9233,15 +13520,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -9271,177 +13558,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9467,177 +13831,254 @@
     const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(uint32_t) < sizeof(long)) {
+        if ((sizeof(uint32_t) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(uint32_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (uint32_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (uint32_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(uint32_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(uint32_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) >= 2 * PyLong_SHIFT) {
-                            return (uint32_t) (((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(uint32_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(uint32_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) >= 2 * PyLong_SHIFT)) {
+                                return (uint32_t) (((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(uint32_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) >= 3 * PyLong_SHIFT) {
-                            return (uint32_t) (((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(uint32_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) >= 3 * PyLong_SHIFT)) {
+                                return (uint32_t) (((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(uint32_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
-                            return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(uint32_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT)) {
+                                return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (uint32_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(uint32_t) <= sizeof(unsigned long)) {
+            if ((sizeof(uint32_t) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint32_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint32_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(uint32_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint32_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (uint32_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(uint32_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(uint32_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(uint32_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint32_t) (((uint32_t)-1)*(((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(uint32_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(uint32_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (uint32_t) (((uint32_t)-1)*(((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(uint32_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint32_t) ((((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(uint32_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (uint32_t) ((((((uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint32_t) (((uint32_t)-1)*(((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(uint32_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (uint32_t) (((uint32_t)-1)*(((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(uint32_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint32_t) ((((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(uint32_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (uint32_t) ((((((((uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint32_t) (((uint32_t)-1)*(((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(uint32_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (uint32_t) (((uint32_t)-1)*(((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(uint32_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint32_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint32_t) ((((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(uint32_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint32_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (uint32_t) ((((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(uint32_t) <= sizeof(long)) {
+            if ((sizeof(uint32_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint32_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint32_t) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(uint32_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint32_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             uint32_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (uint32_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (uint32_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (uint32_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (uint32_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (uint32_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(uint32_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((uint32_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(uint32_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((uint32_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((uint32_t) 1) << (sizeof(uint32_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (uint32_t) -1;
         }
     } else {
         uint32_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (uint32_t) -1;
         val = __Pyx_PyInt_As_uint32_t(tmp);
@@ -9683,16 +14124,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(uint32_t),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(uint32_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int8_t(int8_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -9721,19 +14186,59 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(int8_t),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int8_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__19);
+    }
+    return name;
+}
+#endif
+
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -9759,16 +14264,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -9777,177 +14306,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -9964,15 +14570,15 @@
     return (long) -1;
 }
 
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -9985,14 +14591,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -10009,19 +14631,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -10090,50 +14712,60 @@
                 found_dot = 1;
             } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
                 break;
             }
             rtversion[i] = rt_from_call[i];
         }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -10187,15 +14819,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -10216,30 +14848,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -10297,21 +14933,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -10371,8 +15005,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `pykdtree-1.3.7.post0/pykdtree/kdtree.pyx` & `pykdtree-1.3.9/pykdtree/kdtree.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
         if distance_upper_bound is not None: # Mark out of bounds results
             if self.data_pts.dtype == np.float32:
                 idx_out = (closest_dists_res >= dub_float)
             else:
                 idx_out = (closest_dists_res >= dub_double)
 
-            closest_dists_res[idx_out] = np.Inf
+            closest_dists_res[idx_out] = np.inf
             closest_idxs_res[idx_out] = self.n
 
         if not sqr_dists: # Return actual cartesian distances
             closest_dists_res = np.sqrt(closest_dists_res)
 
         return closest_dists_res, closest_idxs_res
```

### Comparing `pykdtree-1.3.7.post0/pykdtree/test_tree.py` & `pykdtree-1.3.9/pykdtree/test_tree.py`

 * *Files identical despite different names*

### Comparing `pykdtree-1.3.7.post0/setup.py` & `pykdtree-1.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import sys
 import re
+
+import numpy as np
+from Cython.Build import cythonize
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 
 
 OMP_SETTING_TABLE = {
     '1': 'probe',
     '0': None,
@@ -41,22 +44,17 @@
 
 OMP_LINK_ARGS = {
     'gomp': ['-lgomp'],
     'omp': ['-lomp'],
     'msvc': []
 }
 
-def set_builtin(name, value):
-    if isinstance(__builtins__, dict):
-        __builtins__[name] = value
-    else:
-        setattr(__builtins__, name, value)
-
 
 class build_ext_subclass(build_ext):
+    """Custom extension building to have platform and compiler specific flags."""
 
     def build_extensions(self):
         comp = self.compiler.compiler_type
         omp_comp, omp_link = _omp_compile_link_args(comp)
         if comp in ('unix', 'cygwin', 'mingw32'):
             extra_compile_args = ['-std=c99', '-O3'] + omp_comp
             extra_link_args = omp_link
@@ -67,26 +65,14 @@
             # Add support for more compilers here
             raise ValueError('Compiler flags undefined for %s. Please modify setup.py and add compiler flags'
                              % comp)
         self.extensions[0].extra_compile_args = extra_compile_args
         self.extensions[0].extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
-    def finalize_options(self):
-        '''
-        In order to avoid premature import of numpy before it gets installed as a dependency
-        get numpy include directories during the extensions building process
-        http://stackoverflow.com/questions/19919905/how-to-bootstrap-numpy-installation-in-setup-py
-        '''
-        build_ext.finalize_options(self)
-        # Prevent numpy from thinking it is still in its setup process:
-        set_builtin('__NUMPY_SETUP__', False)
-        import numpy
-        self.include_dirs.append(numpy.get_include())
-
 
 def _omp_compile_link_args(compiler):
     # Get OpenMP setting from environment
     use_omp = OMP_SETTING_TABLE[os.environ.get('USE_OMP', 'probe')]
 
     compile_args = []
     link_args = []
@@ -195,30 +181,34 @@
     # only return success if there's no ambiguity
     return (inc + lib) if len(inc) == 1 and len(lib) == 1 else (None, None)
 
 
 with open('README.rst', 'r') as readme_file:
     readme = readme_file.read()
 
+extensions = [
+    Extension('pykdtree.kdtree', sources=['pykdtree/kdtree.pyx', 'pykdtree/_kdtree_core.c'],
+              include_dirs=[np.get_include()],
+              ),
+]
+
 setup(
     name='pykdtree',
-    version='1.3.7.post0',
+    version='1.3.9',
     url="https://github.com/storpipfugl/pykdtree",
     description='Fast kd-tree implementation with OpenMP-enabled queries',
     long_description=readme,
     author='Esben S. Nielsen',
     author_email='storpipfugl@gmail.com',
     packages=['pykdtree'],
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     install_requires=['numpy'],
-    setup_requires=['numpy'],
     tests_require=['pytest'],
     zip_safe=False,
-    ext_modules=[Extension('pykdtree.kdtree',
-                           ['pykdtree/kdtree.c', 'pykdtree/_kdtree_core.c'])],
+    ext_modules=cythonize(extensions),
     cmdclass={'build_ext': build_ext_subclass},
     classifiers=[
       'Development Status :: 5 - Production/Stable',
       ('License :: OSI Approved :: '
           'GNU Lesser General Public License v3 (LGPLv3)'),
       'Programming Language :: Python',
       'Operating System :: OS Independent',
```

