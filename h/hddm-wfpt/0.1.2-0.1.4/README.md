# Comparing `tmp/hddm_wfpt-0.1.2.tar.gz` & `tmp/hddm_wfpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_wfpt-0.1.2.tar", last modified: Wed Oct  4 18:19:42 2023, max compression
+gzip compressed data, was "hddm_wfpt-0.1.4.tar", last modified: Thu Apr 18 10:12:57 2024, max compression
```

## Comparing `hddm_wfpt-0.1.2.tar` & `hddm_wfpt-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 18:19:42.714189 hddm_wfpt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-10-04 18:19:42.714189 hddm_wfpt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/Readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 18:19:42.706189 hddm_wfpt-0.1.2/cython_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 18:19:42.710189 hddm_wfpt-0.1.2/cython_build/hddm_wfpt/
--rw-r--r--   0 runner    (1001) docker     (127)   460900 2023-10-04 18:19:41.000000 hddm_wfpt-0.1.2/cython_build/hddm_wfpt/cdfdif_wrapper.c
--rw-r--r--   0 runner    (1001) docker     (127)  1145312 2023-10-04 18:19:41.000000 hddm_wfpt-0.1.2/cython_build/hddm_wfpt/wfpt.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 18:19:42.714189 hddm_wfpt-0.1.2/hddm_wfpt/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/hddm_wfpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/hddm_wfpt/cdfdif.c
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/hddm_wfpt/cdfdif.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 18:19:42.714189 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-10-04 18:19:42.000000 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-04 18:19:42.000000 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 18:19:42.000000 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-04 18:19:42.000000 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-04 18:19:42.000000 hddm_wfpt-0.1.2/hddm_wfpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 18:19:42.714189 hddm_wfpt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-04 18:19:23.000000 hddm_wfpt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:12:57.171695 hddm_wfpt-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 10:12:57.171695 hddm_wfpt-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/Readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:12:57.163695 hddm_wfpt-0.1.4/cython_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:12:57.167695 hddm_wfpt-0.1.4/cython_build/hddm_wfpt/
+-rw-r--r--   0 runner    (1001) docker     (127)   466099 2024-04-18 10:12:56.000000 hddm_wfpt-0.1.4/cython_build/hddm_wfpt/cdfdif_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1153836 2024-04-18 10:12:56.000000 hddm_wfpt-0.1.4/cython_build/hddm_wfpt/wfpt.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:12:57.171695 hddm_wfpt-0.1.4/hddm_wfpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/cdfdif.c
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/cdfdif.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/cdfdif_wrapper.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/integrate.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/pdf.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/hddm_wfpt/wfpt.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:12:57.171695 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 10:12:57.000000 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-18 10:12:57.000000 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:12:57.000000 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 10:12:57.000000 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 10:12:57.000000 hddm_wfpt-0.1.4/hddm_wfpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:12:57.171695 hddm_wfpt-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-18 10:12:49.000000 hddm_wfpt-0.1.4/setup.py
```

### Comparing `hddm_wfpt-0.1.2/LICENSE` & `hddm_wfpt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_wfpt-0.1.2/PKG-INFO` & `hddm_wfpt-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_wfpt
-Version: 0.1.2
+Version: 0.1.4
 Summary: HDDM is a python module that implements Hierarchical Bayesian estimation of Drift Diffusion Models.
 Author-email: Alexander Fengler <alexander_fengler@brown.edu>, Paul Xu <yang_xu@brown.edu>, Michael Frank <michael_frank@brown.edu>
 Project-URL: Homepage, https://github.com/lnccbrown/hddm-wfpt
 Project-URL: Bug Tracker, https://github.com/lnccbrown/hddm-wfpt/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `hddm_wfpt-0.1.2/Readme.rst` & `hddm_wfpt-0.1.4/Readme.rst`

 * *Files identical despite different names*

### Comparing `hddm_wfpt-0.1.2/cython_build/hddm_wfpt/cdfdif_wrapper.c` & `hddm_wfpt-0.1.4/cython_build/hddm_wfpt/cdfdif_wrapper.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "hddm_wfpt/cdfdif.h"
         ],
@@ -34,23 +34,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -134,14 +134,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -195,14 +197,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -256,60 +260,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -392,14 +419,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -583,25 +613,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -614,15 +647,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -647,15 +679,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -733,16 +765,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -758,14 +795,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -784,14 +846,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -859,27 +923,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
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
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -915,15 +979,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1059,14 +1123,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1137,15 +1210,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1221,17 +1294,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1251,32 +1325,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1318,15 +1375,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1339,14 +1396,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1389,14 +1447,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1436,15 +1495,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1511,177 +1570,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1710,42 +1769,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2190,29 +2249,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2392,30 +2456,30 @@
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 #define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2517,25 +2581,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -2757,15 +2825,16 @@
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
@@ -3290,15 +3359,15 @@
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
@@ -3309,26 +3378,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("base", __pyx_f[1], 245, 1, __PYX_ERR(1, 245, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(248,1,__PYX_ERR(1, 248, __pyx_L1_error))
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
@@ -3343,15 +3412,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
@@ -3359,32 +3428,32 @@
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
   __Pyx_TraceCall("descr", __pyx_f[1], 251, 0, __PYX_ERR(1, 251, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(254,0,__PYX_ERR(1, 254, __pyx_L1_error))
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
@@ -3395,15 +3464,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
@@ -3414,26 +3483,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("ndim", __pyx_f[1], 257, 1, __PYX_ERR(1, 257, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(260,1,__PYX_ERR(1, 260, __pyx_L1_error))
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
@@ -3448,15 +3517,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -3467,26 +3536,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("shape", __pyx_f[1], 263, 1, __PYX_ERR(1, 263, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(268,1,__PYX_ERR(1, 268, __pyx_L1_error))
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -3501,15 +3570,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -3520,26 +3589,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("strides", __pyx_f[1], 271, 1, __PYX_ERR(1, 271, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(275,1,__PYX_ERR(1, 275, __pyx_L1_error))
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -3554,15 +3623,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
@@ -3573,26 +3642,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("size", __pyx_f[1], 278, 1, __PYX_ERR(1, 278, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(281,1,__PYX_ERR(1, 281, __pyx_L1_error))
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
@@ -3607,15 +3676,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
@@ -3626,26 +3695,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("data", __pyx_f[1], 284, 1, __PYX_ERR(1, 284, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __Pyx_TraceLine(290,1,__PYX_ERR(1, 290, __pyx_L1_error))
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
@@ -3660,15 +3729,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3676,33 +3745,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 773, 0, __PYX_ERR(1, 773, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_TraceLine(774,0,__PYX_ERR(1, 774, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3714,15 +3783,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3730,33 +3799,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 776, 0, __PYX_ERR(1, 776, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_TraceLine(777,0,__PYX_ERR(1, 777, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3768,15 +3837,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3784,33 +3853,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 779, 0, __PYX_ERR(1, 779, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_TraceLine(780,0,__PYX_ERR(1, 780, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3822,15 +3891,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3838,33 +3907,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 782, 0, __PYX_ERR(1, 782, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_TraceLine(783,0,__PYX_ERR(1, 783, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3876,15 +3945,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3892,33 +3961,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 785, 0, __PYX_ERR(1, 785, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_TraceLine(786,0,__PYX_ERR(1, 786, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3930,15 +3999,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -3946,66 +4015,66 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 788, 0, __PYX_ERR(1, 788, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __Pyx_TraceLine(789,0,__PYX_ERR(1, 789, __pyx_L1_error))
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_TraceLine(790,0,__PYX_ERR(1, 790, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(792,0,__PYX_ERR(1, 792, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -4016,70 +4085,67 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-  __Pyx_TraceCall("set_array_base", __pyx_f[1], 967, 0, __PYX_ERR(1, 967, __pyx_L1_error));
+  __Pyx_TraceCall("set_array_base", __pyx_f[1], 968, 0, __PYX_ERR(1, 968, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
-  __Pyx_TraceLine(968,0,__PYX_ERR(1, 968, __pyx_L1_error))
+  __Pyx_TraceLine(969,0,__PYX_ERR(1, 969, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __Pyx_TraceLine(969,0,__PYX_ERR(1, 969, __pyx_L1_error))
-  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 969, __pyx_L1_error)
+  __Pyx_TraceLine(970,0,__PYX_ERR(1, 970, __pyx_L1_error))
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -4088,73 +4154,73 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-  __Pyx_TraceCall("get_array_base", __pyx_f[1], 971, 0, __PYX_ERR(1, 971, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("get_array_base", 1);
+  __Pyx_TraceCall("get_array_base", __pyx_f[1], 972, 0, __PYX_ERR(1, 972, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
-  __Pyx_TraceLine(972,0,__PYX_ERR(1, 972, __pyx_L1_error))
+  __Pyx_TraceLine(973,0,__PYX_ERR(1, 973, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
-  __Pyx_TraceLine(973,0,__PYX_ERR(1, 973, __pyx_L1_error))
+  __Pyx_TraceLine(974,0,__PYX_ERR(1, 974, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
-    __Pyx_TraceLine(974,0,__PYX_ERR(1, 974, __pyx_L1_error))
+    __Pyx_TraceLine(975,0,__PYX_ERR(1, 975, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
-  __Pyx_TraceLine(975,0,__PYX_ERR(1, 975, __pyx_L1_error))
+  __Pyx_TraceLine(976,0,__PYX_ERR(1, 976, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -4165,15 +4231,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4188,91 +4254,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-  __Pyx_TraceCall("import_array", __pyx_f[1], 979, 0, __PYX_ERR(1, 979, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_array", 1);
+  __Pyx_TraceCall("import_array", __pyx_f[1], 980, 0, __PYX_ERR(1, 980, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
-  __Pyx_TraceLine(980,0,__PYX_ERR(1, 980, __pyx_L1_error))
+  __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L3_error))
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 981, __pyx_L3_error)
+      __Pyx_TraceLine(982,0,__PYX_ERR(1, 982, __pyx_L3_error))
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
-    __Pyx_TraceLine(982,0,__PYX_ERR(1, 982, __pyx_L5_except_error))
+    __Pyx_TraceLine(983,0,__PYX_ERR(1, 983, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 982, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __Pyx_TraceLine(983,0,__PYX_ERR(1, 983, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __Pyx_TraceLine(984,0,__PYX_ERR(1, 984, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4280,15 +4346,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4304,15 +4370,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4327,91 +4393,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-  __Pyx_TraceCall("import_umath", __pyx_f[1], 985, 0, __PYX_ERR(1, 985, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_umath", 1);
+  __Pyx_TraceCall("import_umath", __pyx_f[1], 986, 0, __PYX_ERR(1, 986, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(986,0,__PYX_ERR(1, 986, __pyx_L1_error))
+  __Pyx_TraceLine(987,0,__PYX_ERR(1, 987, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(987,0,__PYX_ERR(1, 987, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 987, __pyx_L3_error)
+      __Pyx_TraceLine(988,0,__PYX_ERR(1, 988, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(988,0,__PYX_ERR(1, 988, __pyx_L5_except_error))
+    __Pyx_TraceLine(989,0,__PYX_ERR(1, 989, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __Pyx_TraceLine(989,0,__PYX_ERR(1, 989, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __Pyx_TraceLine(990,0,__PYX_ERR(1, 990, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4419,15 +4485,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4443,15 +4509,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4466,91 +4532,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-  __Pyx_TraceCall("import_ufunc", __pyx_f[1], 991, 0, __PYX_ERR(1, 991, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
+  __Pyx_TraceCall("import_ufunc", __pyx_f[1], 992, 0, __PYX_ERR(1, 992, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(992,0,__PYX_ERR(1, 992, __pyx_L1_error))
+  __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 993, __pyx_L3_error)
+      __Pyx_TraceLine(994,0,__PYX_ERR(1, 994, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(994,0,__PYX_ERR(1, 994, __pyx_L5_except_error))
+    __Pyx_TraceLine(995,0,__PYX_ERR(1, 995, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(995,0,__PYX_ERR(1, 995, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __Pyx_TraceLine(996,0,__PYX_ERR(1, 996, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4558,15 +4624,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4582,109 +4648,103 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 998, 0, __PYX_ERR(1, 998, __pyx_L1_error));
+  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 999, 0, __PYX_ERR(1, 999, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1010,0,__PYX_ERR(1, 1010, __pyx_L1_error))
+  __Pyx_TraceLine(1011,0,__PYX_ERR(1, 1011, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.is_timedelta64_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-  __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 1013, 0, __PYX_ERR(1, 1013, __pyx_L1_error));
+  __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 1014, 0, __PYX_ERR(1, 1014, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1025,0,__PYX_ERR(1, 1025, __pyx_L1_error))
+  __Pyx_TraceLine(1026,0,__PYX_ERR(1, 1026, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.is_datetime64_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -4693,28 +4753,28 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 1028, 1, __PYX_ERR(1, 1028, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 1029, 1, __PYX_ERR(1, 1029, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1035,1,__PYX_ERR(1, 1035, __pyx_L1_error))
+  __Pyx_TraceLine(1036,1,__PYX_ERR(1, 1036, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -4729,15 +4789,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -4746,28 +4806,28 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1038, 1, __PYX_ERR(1, 1038, __pyx_L1_error));
+  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1039, 1, __PYX_ERR(1, 1039, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1042,1,__PYX_ERR(1, 1042, __pyx_L1_error))
+  __Pyx_TraceLine(1043,1,__PYX_ERR(1, 1043, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -4782,15 +4842,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4799,26 +4859,26 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1045, 1, __PYX_ERR(1, 1045, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1046, 1, __PYX_ERR(1, 1046, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
-  __Pyx_TraceLine(1049,1,__PYX_ERR(1, 1049, __pyx_L1_error))
+  __Pyx_TraceLine(1050,1,__PYX_ERR(1, 1050, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4844,20 +4904,18 @@
  *     return y * (1 - p_outlier) + (x + (1. / (2 * w_outlier))) * w_outlier * p_outlier
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_14cdfdif_wrapper_add_outlier_cdf(double __pyx_v_y, double __pyx_v_x, double __pyx_v_p_outlier, double __pyx_v_w_outlier) {
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   double __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("add_outlier_cdf", 0);
   __Pyx_TraceCall("add_outlier_cdf", __pyx_f[0], 11, 0, __PYX_ERR(0, 11, __pyx_L1_error));
 
   /* "cdfdif_wrapper.pyx":12
  * 
  * cdef inline double add_outlier_cdf(double y, double x, double p_outlier, double w_outlier):
  *     return y * (1 - p_outlier) + (x + (1. / (2 * w_outlier))) * w_outlier * p_outlier             # <<<<<<<<<<<<<<
  * 
@@ -4882,45 +4940,41 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("cdfdif_wrapper.add_outlier_cdf", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cdfdif_wrapper.pyx":14
  *     return y * (1 - p_outlier) + (x + (1. / (2 * w_outlier))) * w_outlier * p_outlier
  * 
  * cdef inline bint p_outlier_in_range(double p_outlier): return (p_outlier >= 0) & (p_outlier <= 1)             # <<<<<<<<<<<<<<
  * 
  * def dmat_cdf_array(np.ndarray[double, ndim=1] x, double v, double sv,
  */
 
 static CYTHON_INLINE int __pyx_f_14cdfdif_wrapper_p_outlier_in_range(double __pyx_v_p_outlier) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("p_outlier_in_range", 0);
   __Pyx_TraceCall("p_outlier_in_range", __pyx_f[0], 14, 0, __PYX_ERR(0, 14, __pyx_L1_error));
   __pyx_r = ((__pyx_v_p_outlier >= 0.0) & (__pyx_v_p_outlier <= 1.0));
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("cdfdif_wrapper.p_outlier_in_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cdfdif_wrapper.pyx":16
  * cdef inline bint p_outlier_in_range(double p_outlier): return (p_outlier >= 0) & (p_outlier <= 1)
  * 
  * def dmat_cdf_array(np.ndarray[double, ndim=1] x, double v, double sv,             # <<<<<<<<<<<<<<
@@ -4965,16 +5019,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("dmat_cdf_array (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 16, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -5127,18 +5180,19 @@
     __pyx_v_z = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_z == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
     __pyx_v_sz = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_sz == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
     __pyx_v_t = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_t == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
     __pyx_v_st = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_st == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
     __pyx_v_p_outlier = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_p_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
     __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("dmat_cdf_array", 1, 10, 10, __pyx_nargs); __PYX_ERR(0, 16, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -5196,15 +5250,15 @@
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__3)
-  __Pyx_RefNannySetupContext("dmat_cdf_array", 0);
+  __Pyx_RefNannySetupContext("dmat_cdf_array", 1);
   __Pyx_TraceCall("dmat_cdf_array", __pyx_f[0], 16, 0, __PYX_ERR(0, 16, __pyx_L1_error));
   __pyx_pybuffer_y.pybuffer.buf = NULL;
   __pyx_pybuffer_y.refcount = 0;
   __pyx_pybuffernd_y.data = NULL;
   __pyx_pybuffernd_y.rcbuffer = &__pyx_pybuffer_y;
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
@@ -5892,44 +5946,44 @@
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "cdfdif_wrapper.pyx":21
  *     #check arguments
  *     if p_outlier > 0:
  *         assert np.max(np.abs(x)) < (1./(2*w_outlier)), ValueError('1. / (2*w_outlier) must be smaller than RT')             # <<<<<<<<<<<<<<
@@ -6055,41 +6109,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 865, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6296,42 +6350,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("cdfdif_wrapper", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 2, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to cdfdif_wrapper pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "cdfdif_wrapper" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 2, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 2, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 2, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 2, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 2, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_cdfdif_wrapper(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 2, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -6389,242 +6441,242 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_cdfdif_wrapper(void)", __pyx_f[0], 2, 0, __PYX_ERR(0, 2, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
   __Pyx_TraceLine(245,0,__PYX_ERR(1, 245, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
   __Pyx_TraceLine(251,0,__PYX_ERR(1, 251, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
   __Pyx_TraceLine(257,0,__PYX_ERR(1, 257, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
   __Pyx_TraceLine(263,0,__PYX_ERR(1, 263, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
   __Pyx_TraceLine(271,0,__PYX_ERR(1, 271, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
   __Pyx_TraceLine(278,0,__PYX_ERR(1, 278, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
   __Pyx_TraceLine(284,0,__PYX_ERR(1, 284, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
   __Pyx_TraceLine(773,0,__PYX_ERR(1, 773, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
   __Pyx_TraceLine(776,0,__PYX_ERR(1, 776, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
   __Pyx_TraceLine(779,0,__PYX_ERR(1, 779, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
   __Pyx_TraceLine(782,0,__PYX_ERR(1, 782, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
   __Pyx_TraceLine(785,0,__PYX_ERR(1, 785, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
   __Pyx_TraceLine(788,0,__PYX_ERR(1, 788, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
-  __Pyx_TraceLine(967,0,__PYX_ERR(1, 967, __pyx_L1_error))
+  __Pyx_TraceLine(968,0,__PYX_ERR(1, 968, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
-  __Pyx_TraceLine(971,0,__PYX_ERR(1, 971, __pyx_L1_error))
+  __Pyx_TraceLine(972,0,__PYX_ERR(1, 972, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
-  __Pyx_TraceLine(979,0,__PYX_ERR(1, 979, __pyx_L1_error))
+  __Pyx_TraceLine(980,0,__PYX_ERR(1, 980, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(985,0,__PYX_ERR(1, 985, __pyx_L1_error))
+  __Pyx_TraceLine(986,0,__PYX_ERR(1, 986, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(991,0,__PYX_ERR(1, 991, __pyx_L1_error))
+  __Pyx_TraceLine(992,0,__PYX_ERR(1, 992, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
-  __Pyx_TraceLine(998,0,__PYX_ERR(1, 998, __pyx_L1_error))
+  __Pyx_TraceLine(999,0,__PYX_ERR(1, 999, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
-  __Pyx_TraceLine(1013,0,__PYX_ERR(1, 1013, __pyx_L1_error))
+  __Pyx_TraceLine(1014,0,__PYX_ERR(1, 1014, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
-  __Pyx_TraceLine(1028,0,__PYX_ERR(1, 1028, __pyx_L1_error))
+  __Pyx_TraceLine(1029,0,__PYX_ERR(1, 1029, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
-  __Pyx_TraceLine(1038,0,__PYX_ERR(1, 1038, __pyx_L1_error))
+  __Pyx_TraceLine(1039,0,__PYX_ERR(1, 1039, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
-  __Pyx_TraceLine(1045,0,__PYX_ERR(1, 1045, __pyx_L1_error))
+  __Pyx_TraceLine(1046,0,__PYX_ERR(1, 1046, __pyx_L1_error))
 
 
   /* "cdfdif_wrapper.pyx":3
  * 
  * cimport numpy as np
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
@@ -6804,14 +6856,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -6861,33 +6915,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -7170,16 +7231,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -7543,21 +7609,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -7642,15 +7726,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -7661,15 +7745,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -7693,15 +7777,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -8377,15 +8461,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -8456,17 +8540,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -8533,67 +8623,62 @@
 #endif
 
 /* PyObjectCallMethO */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
-  static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+  #if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
         Py_INCREF(args[i]);
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -8609,33 +8694,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* ExtTypeTest */
   static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     __Pyx_TypeName obj_type_name;
     __Pyx_TypeName type_name;
     if (unlikely(!type)) {
@@ -8657,18 +8748,18 @@
 /* BufferIndexError */
   static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -8714,23 +8805,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8759,15 +8850,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -8997,18 +9088,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
   static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
   static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -9161,15 +9249,29 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
-  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
@@ -9970,15 +10072,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -10309,16 +10411,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -10330,14 +10432,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -10427,15 +10531,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -11001,15 +11105,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -11153,38 +11257,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -11352,15 +11458,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -11572,49 +11678,58 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -11652,16 +11767,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `hddm_wfpt-0.1.2/cython_build/hddm_wfpt/wfpt.cpp` & `hddm_wfpt-0.1.4/cython_build/hddm_wfpt/wfpt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "wfpt",
@@ -29,23 +29,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -129,14 +129,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -190,14 +192,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -251,60 +255,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -387,14 +414,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -594,25 +624,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -625,15 +658,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -658,15 +690,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -744,16 +776,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -769,14 +806,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -795,14 +857,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -870,27 +934,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
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
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -926,15 +990,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1070,14 +1134,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1148,15 +1221,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1228,17 +1301,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1258,32 +1332,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1325,15 +1382,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1346,14 +1403,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1396,14 +1454,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1443,15 +1502,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1520,177 +1579,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1719,42 +1778,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2218,29 +2277,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2451,30 +2515,30 @@
 static PyObject* __Pyx_PyInt_AddCObj(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddCObj(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2579,25 +2643,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -2786,14 +2854,17 @@
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
@@ -2822,15 +2893,16 @@
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
@@ -3933,15 +4005,15 @@
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
@@ -3952,26 +4024,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("base", __pyx_f[1], 245, 1, __PYX_ERR(1, 245, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(248,1,__PYX_ERR(1, 248, __pyx_L1_error))
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
@@ -3986,15 +4058,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
@@ -4002,32 +4074,32 @@
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
   __Pyx_TraceCall("descr", __pyx_f[1], 251, 0, __PYX_ERR(1, 251, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(254,0,__PYX_ERR(1, 254, __pyx_L1_error))
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
@@ -4038,15 +4110,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
@@ -4057,26 +4129,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("ndim", __pyx_f[1], 257, 1, __PYX_ERR(1, 257, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(260,1,__PYX_ERR(1, 260, __pyx_L1_error))
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
@@ -4091,15 +4163,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -4110,26 +4182,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("shape", __pyx_f[1], 263, 1, __PYX_ERR(1, 263, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(268,1,__PYX_ERR(1, 268, __pyx_L1_error))
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -4144,15 +4216,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -4163,26 +4235,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("strides", __pyx_f[1], 271, 1, __PYX_ERR(1, 271, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(275,1,__PYX_ERR(1, 275, __pyx_L1_error))
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
@@ -4197,15 +4269,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
@@ -4216,26 +4288,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("size", __pyx_f[1], 278, 1, __PYX_ERR(1, 278, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_TraceLine(281,1,__PYX_ERR(1, 281, __pyx_L1_error))
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
@@ -4250,15 +4322,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
@@ -4269,26 +4341,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceCall("data", __pyx_f[1], 284, 1, __PYX_ERR(1, 284, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __Pyx_TraceLine(290,1,__PYX_ERR(1, 290, __pyx_L1_error))
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
@@ -4303,15 +4375,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4319,33 +4391,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 773, 0, __PYX_ERR(1, 773, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_TraceLine(774,0,__PYX_ERR(1, 774, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4357,15 +4429,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4373,33 +4445,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 776, 0, __PYX_ERR(1, 776, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_TraceLine(777,0,__PYX_ERR(1, 777, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4411,15 +4483,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4427,33 +4499,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 779, 0, __PYX_ERR(1, 779, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_TraceLine(780,0,__PYX_ERR(1, 780, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4465,15 +4537,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4481,33 +4553,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 782, 0, __PYX_ERR(1, 782, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_TraceLine(783,0,__PYX_ERR(1, 783, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4519,15 +4591,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4535,33 +4607,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 785, 0, __PYX_ERR(1, 785, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_TraceLine(786,0,__PYX_ERR(1, 786, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4573,15 +4645,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -4589,66 +4661,66 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 788, 0, __PYX_ERR(1, 788, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __Pyx_TraceLine(789,0,__PYX_ERR(1, 789, __pyx_L1_error))
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_TraceLine(790,0,__PYX_ERR(1, 790, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(792,0,__PYX_ERR(1, 792, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -4659,70 +4731,67 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-  __Pyx_TraceCall("set_array_base", __pyx_f[1], 967, 0, __PYX_ERR(1, 967, __pyx_L1_error));
+  __Pyx_TraceCall("set_array_base", __pyx_f[1], 968, 0, __PYX_ERR(1, 968, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
-  __Pyx_TraceLine(968,0,__PYX_ERR(1, 968, __pyx_L1_error))
+  __Pyx_TraceLine(969,0,__PYX_ERR(1, 969, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __Pyx_TraceLine(969,0,__PYX_ERR(1, 969, __pyx_L1_error))
-  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 969, __pyx_L1_error)
+  __Pyx_TraceLine(970,0,__PYX_ERR(1, 970, __pyx_L1_error))
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -4731,73 +4800,73 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-  __Pyx_TraceCall("get_array_base", __pyx_f[1], 971, 0, __PYX_ERR(1, 971, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("get_array_base", 1);
+  __Pyx_TraceCall("get_array_base", __pyx_f[1], 972, 0, __PYX_ERR(1, 972, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
-  __Pyx_TraceLine(972,0,__PYX_ERR(1, 972, __pyx_L1_error))
+  __Pyx_TraceLine(973,0,__PYX_ERR(1, 973, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
-  __Pyx_TraceLine(973,0,__PYX_ERR(1, 973, __pyx_L1_error))
+  __Pyx_TraceLine(974,0,__PYX_ERR(1, 974, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
-    __Pyx_TraceLine(974,0,__PYX_ERR(1, 974, __pyx_L1_error))
+    __Pyx_TraceLine(975,0,__PYX_ERR(1, 975, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
-  __Pyx_TraceLine(975,0,__PYX_ERR(1, 975, __pyx_L1_error))
+  __Pyx_TraceLine(976,0,__PYX_ERR(1, 976, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -4808,15 +4877,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4831,91 +4900,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-  __Pyx_TraceCall("import_array", __pyx_f[1], 979, 0, __PYX_ERR(1, 979, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_array", 1);
+  __Pyx_TraceCall("import_array", __pyx_f[1], 980, 0, __PYX_ERR(1, 980, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
-  __Pyx_TraceLine(980,0,__PYX_ERR(1, 980, __pyx_L1_error))
+  __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L3_error))
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 981, __pyx_L3_error)
+      __Pyx_TraceLine(982,0,__PYX_ERR(1, 982, __pyx_L3_error))
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
-    __Pyx_TraceLine(982,0,__PYX_ERR(1, 982, __pyx_L5_except_error))
+    __Pyx_TraceLine(983,0,__PYX_ERR(1, 983, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 982, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __Pyx_TraceLine(983,0,__PYX_ERR(1, 983, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __Pyx_TraceLine(984,0,__PYX_ERR(1, 984, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4923,15 +4992,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4947,15 +5016,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4970,91 +5039,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-  __Pyx_TraceCall("import_umath", __pyx_f[1], 985, 0, __PYX_ERR(1, 985, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_umath", 1);
+  __Pyx_TraceCall("import_umath", __pyx_f[1], 986, 0, __PYX_ERR(1, 986, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(986,0,__PYX_ERR(1, 986, __pyx_L1_error))
+  __Pyx_TraceLine(987,0,__PYX_ERR(1, 987, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(987,0,__PYX_ERR(1, 987, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 987, __pyx_L3_error)
+      __Pyx_TraceLine(988,0,__PYX_ERR(1, 988, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(988,0,__PYX_ERR(1, 988, __pyx_L5_except_error))
+    __Pyx_TraceLine(989,0,__PYX_ERR(1, 989, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __Pyx_TraceLine(989,0,__PYX_ERR(1, 989, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __Pyx_TraceLine(990,0,__PYX_ERR(1, 990, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5062,15 +5131,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5086,15 +5155,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5109,91 +5178,91 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-  __Pyx_TraceCall("import_ufunc", __pyx_f[1], 991, 0, __PYX_ERR(1, 991, __pyx_L1_error));
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
+  __Pyx_TraceCall("import_ufunc", __pyx_f[1], 992, 0, __PYX_ERR(1, 992, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(992,0,__PYX_ERR(1, 992, __pyx_L1_error))
+  __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 993, __pyx_L3_error)
+      __Pyx_TraceLine(994,0,__PYX_ERR(1, 994, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(994,0,__PYX_ERR(1, 994, __pyx_L5_except_error))
+    __Pyx_TraceLine(995,0,__PYX_ERR(1, 995, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(995,0,__PYX_ERR(1, 995, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __Pyx_TraceLine(996,0,__PYX_ERR(1, 996, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5201,15 +5270,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5225,109 +5294,103 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 998, 0, __PYX_ERR(1, 998, __pyx_L1_error));
+  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 999, 0, __PYX_ERR(1, 999, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1010,0,__PYX_ERR(1, 1010, __pyx_L1_error))
+  __Pyx_TraceLine(1011,0,__PYX_ERR(1, 1011, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.is_timedelta64_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-  __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 1013, 0, __PYX_ERR(1, 1013, __pyx_L1_error));
+  __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 1014, 0, __PYX_ERR(1, 1014, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1025,0,__PYX_ERR(1, 1025, __pyx_L1_error))
+  __Pyx_TraceLine(1026,0,__PYX_ERR(1, 1026, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.is_datetime64_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -5336,28 +5399,28 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 1028, 1, __PYX_ERR(1, 1028, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 1029, 1, __PYX_ERR(1, 1029, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1035,1,__PYX_ERR(1, 1035, __pyx_L1_error))
+  __Pyx_TraceLine(1036,1,__PYX_ERR(1, 1036, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -5372,15 +5435,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -5389,28 +5452,28 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1038, 1, __PYX_ERR(1, 1038, __pyx_L1_error));
+  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1039, 1, __PYX_ERR(1, 1039, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1042,1,__PYX_ERR(1, 1042, __pyx_L1_error))
+  __Pyx_TraceLine(1043,1,__PYX_ERR(1, 1043, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -5425,15 +5488,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5442,26 +5505,26 @@
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1045, 1, __PYX_ERR(1, 1045, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1046, 1, __PYX_ERR(1, 1046, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
-  __Pyx_TraceLine(1049,1,__PYX_ERR(1, 1049, __pyx_L1_error))
+  __Pyx_TraceLine(1050,1,__PYX_ERR(1, 1050, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5884,24 +5947,22 @@
  */
 
 static double __pyx_f_4wfpt_pdf(double __pyx_v_x, double __pyx_v_v, double __pyx_v_a, double __pyx_v_w, double __pyx_v_err) {
   double __pyx_v_tt;
   double __pyx_v_p;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("pdf", 1);
   __Pyx_TraceCall("pdf", __pyx_f[2], 74, 1, __PYX_ERR(2, 74, __pyx_L1_error));
 
   /* "hddm_wfpt/pdf.pxi":78
  *     and implementation of Navarro & Fuss, 2009.
  *     """
  *     if x <= 0:             # <<<<<<<<<<<<<<
  *         return 0
@@ -5979,15 +6040,14 @@
   __Pyx_AddTraceback("wfpt.pdf", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/pdf.pxi":87
  *     return p*exp(-v*a*w -(pow(v,2))*x/2.)/(pow(a,2))
  * 
  * cdef double pdf_sv(double x, double v, double sv, double a, double z, double err) nogil:             # <<<<<<<<<<<<<<
@@ -5996,24 +6056,22 @@
  */
 
 static double __pyx_f_4wfpt_pdf_sv(double __pyx_v_x, double __pyx_v_v, double __pyx_v_sv, double __pyx_v_a, double __pyx_v_z, double __pyx_v_err) {
   double __pyx_v_tt;
   double __pyx_v_p;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("pdf_sv", 1);
   __Pyx_TraceCall("pdf_sv", __pyx_f[2], 87, 1, __PYX_ERR(2, 87, __pyx_L1_error));
 
   /* "hddm_wfpt/pdf.pxi":92
  *     sv is the std of the drift rate
  *     """
  *     if x <= 0:             # <<<<<<<<<<<<<<
  *         return 0
@@ -6123,15 +6181,14 @@
   __Pyx_AddTraceback("wfpt.pdf_sv", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/pdf.pxi":104
  *     return exp(log(p) + ((a*z*sv)**2 - 2*a*v*z - (v**2)*x)/(2*(sv**2)*x+2))/sqrt((sv**2)*x+1)/(a**2)
  * 
  * cpdef double full_pdf(double x, double v, double sv, double a, double             # <<<<<<<<<<<<<<
@@ -6149,26 +6206,24 @@
 static double __pyx_f_4wfpt_full_pdf(double __pyx_v_x, double __pyx_v_v, double __pyx_v_sv, double __pyx_v_a, double __pyx_v_z, double __pyx_v_sz, double __pyx_v_t, double __pyx_v_st, double __pyx_v_err, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4wfpt_full_pdf *__pyx_optional_args) {
   int __pyx_v_n_st = ((int)2);
   int __pyx_v_n_sz = ((int)2);
   int __pyx_v_use_adaptive = ((int)1);
   double __pyx_v_simps_err = ((double)1e-3);
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_TraceFrameInit(__pyx_codeobj__3)
-  __Pyx_RefNannySetupContext("full_pdf", 1);
   __Pyx_TraceCall("full_pdf", __pyx_f[2], 104, 1, __PYX_ERR(2, 104, __pyx_L1_error));
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_n_st = __pyx_optional_args->n_st;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_n_sz = __pyx_optional_args->n_sz;
         if (__pyx_optional_args->__pyx_n > 2) {
@@ -6636,15 +6691,14 @@
   __Pyx_AddTraceback("wfpt.full_pdf", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4wfpt_1full_pdf(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -6685,16 +6739,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("full_pdf (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(2, 104, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -6899,18 +6952,19 @@
     }
     if (values[12]) {
       __pyx_v_simps_err = __pyx_PyFloat_AsDouble(values[12]); if (unlikely((__pyx_v_simps_err == (double)-1) && PyErr_Occurred())) __PYX_ERR(2, 106, __pyx_L3_error)
     } else {
       __pyx_v_simps_err = ((double)1e-3);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("full_pdf", 0, 9, 13, __pyx_nargs); __PYX_ERR(2, 104, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -6938,15 +6992,15 @@
   double __pyx_t_1;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__3)
-  __Pyx_RefNannySetupContext("full_pdf", 0);
+  __Pyx_RefNannySetupContext("full_pdf", 1);
   __Pyx_TraceCall("full_pdf (wrapper)", __pyx_f[2], 104, 0, __PYX_ERR(2, 104, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 4;
   __pyx_t_2.n_st = __pyx_v_n_st;
   __pyx_t_2.n_sz = __pyx_v_n_sz;
   __pyx_t_2.use_adaptive = __pyx_v_use_adaptive;
   __pyx_t_2.simps_err = __pyx_v_simps_err;
@@ -6984,25 +7038,23 @@
   double __pyx_v_S;
   double __pyx_v_z_tag;
   double __pyx_v_t_tag;
   double __pyx_v_y;
   int __pyx_v_i;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("simpson_1D", 1);
   __Pyx_TraceCall("simpson_1D", __pyx_f[3], 12, 1, __PYX_ERR(3, 12, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":18
  * 
  *     cdef double ht, hz
  *     cdef int n = max(n_st, n_sz)             # <<<<<<<<<<<<<<
  *     if n_st==0: #integration over z
@@ -7260,15 +7312,14 @@
   __Pyx_AddTraceback("wfpt.simpson_1D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/integrate.pxi":47
  *     return ((ht+hz) * S / 3)
  * 
  * cdef double simpson_2D(double x, double v, double sv, double a, double z, double t, double err, double lb_z, double ub_z, int n_sz, double lb_t, double ub_t, int n_st) nogil:             # <<<<<<<<<<<<<<
@@ -7280,25 +7331,23 @@
   double __pyx_v_ht;
   double __pyx_v_S;
   double __pyx_v_t_tag;
   double __pyx_v_y;
   int __pyx_v_i_t;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   double __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("simpson_2D", 1);
   __Pyx_TraceCall("simpson_2D", __pyx_f[3], 47, 1, __PYX_ERR(3, 47, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":56
  *     cdef int i_t
  * 
  *     ht = (ub_t-lb_t)/n_st             # <<<<<<<<<<<<<<
  * 
@@ -7442,15 +7491,14 @@
   __Pyx_AddTraceback("wfpt.simpson_2D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/integrate.pxi":72
  *     return (ht * S / 3)
  * 
  * cdef double adaptiveSimpsonsAux(double x, double v, double sv, double a, double z, double t, double pdf_err,             # <<<<<<<<<<<<<<
@@ -7469,26 +7517,24 @@
   double __pyx_v_fd;
   double __pyx_v_fe;
   double __pyx_v_Sleft;
   double __pyx_v_Sright;
   double __pyx_v_S2;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_t_3;
   double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("adaptiveSimpsonsAux", 1);
   __Pyx_TraceCall("adaptiveSimpsonsAux", __pyx_f[3], 72, 1, __PYX_ERR(3, 72, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":81
  *     #print "in AdaptiveSimpsAux: lb_z: %f, ub_z: %f, lb_t %f, ub_t %f, f_beg: %f, f_end: %f, bottom: %d" % (lb_z, ub_z, lb_t, ub_t, f_beg, f_end, bottom)
  * 
  *     if (ub_t-lb_t) == 0: #integration over sz             # <<<<<<<<<<<<<<
  *         h = ub_z - lb_z
@@ -7789,15 +7835,14 @@
   __Pyx_AddTraceback("wfpt.adaptiveSimpsonsAux", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/integrate.pxi":114
  *                                  Sright, f_mid, f_end, fe, bottom-1)
  * 
  * cdef double adaptiveSimpsons_1D(double x, double v, double sv, double a, double z, double t,             # <<<<<<<<<<<<<<
@@ -7813,24 +7858,22 @@
   double __pyx_v_f_beg;
   double __pyx_v_f_end;
   double __pyx_v_f_mid;
   double __pyx_v_S;
   double __pyx_v_res;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("adaptiveSimpsons_1D", 1);
   __Pyx_TraceCall("adaptiveSimpsons_1D", __pyx_f[3], 114, 1, __PYX_ERR(3, 114, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":120
  *     cdef double h
  * 
  *     if (ub_t - lb_t) == 0: #integration over z             # <<<<<<<<<<<<<<
  *         lb_t = t
@@ -8024,15 +8067,14 @@
   __Pyx_AddTraceback("wfpt.adaptiveSimpsons_1D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/integrate.pxi":143
  *     return res
  * 
  * cdef double adaptiveSimpsonsAux_2D(double x, double v, double sv,             # <<<<<<<<<<<<<<
@@ -8048,26 +8090,24 @@
   double __pyx_v_S2;
   double __pyx_v_t_c;
   double __pyx_v_t_d;
   double __pyx_v_t_e;
   double __pyx_v_h;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   double __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("adaptiveSimpsonsAux_2D", 1);
   __Pyx_TraceCall("adaptiveSimpsonsAux_2D", __pyx_f[3], 143, 1, __PYX_ERR(3, 143, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":156
  *     #print "in AdaptiveSimpsAux_2D: lb_z: %f, ub_z: %f, lb_t %f, ub_t %f, f_beg: %f, f_end: %f, bottom: %d" % (lb_z, ub_z, lb_t, ub_t, f_beg, f_end, bottom)
  * 
  *     cdef double t_c = (ub_t + lb_t)/2.             # <<<<<<<<<<<<<<
  *     cdef double t_d = (lb_t + t_c)/2.
@@ -8262,15 +8302,14 @@
   __Pyx_AddTraceback("wfpt.adaptiveSimpsonsAux_2D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "hddm_wfpt/integrate.pxi":181
  * 
  * 
  * cdef double adaptiveSimpsons_2D(double x, double v, double sv, double a, double z, double t,             # <<<<<<<<<<<<<<
@@ -8288,23 +8327,21 @@
   double __pyx_v_f_mid;
   double __pyx_v_S;
   double __pyx_v_err_1d;
   double __pyx_v_err_2d;
   double __pyx_v_res;
   double __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   double __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("adaptiveSimpsons_2D", 1);
   __Pyx_TraceCall("adaptiveSimpsons_2D", __pyx_f[3], 181, 1, __PYX_ERR(3, 181, __pyx_L1_error));
 
   /* "hddm_wfpt/integrate.pxi":185
  *                                  double simps_err, int maxRecursionDepth_sz, int maxRecursionDepth_st) nogil:
  * 
  *     cdef double h = (ub_t-lb_t)             # <<<<<<<<<<<<<<
  * 
@@ -8469,15 +8506,14 @@
   __Pyx_AddTraceback("wfpt.adaptiveSimpsons_2D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "wfpt.pyx":29
  * include 'integrate.pxi'
  * 
  * def pdf_array(np.ndarray[double, ndim=1] x, double v, double sv, double a, double z, double sz,             # <<<<<<<<<<<<<<
@@ -8529,16 +8565,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pdf_array (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 29, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_logp,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -8793,18 +8828,19 @@
     }
     if (values[15]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[15]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pdf_array", 0, 8, 16, __pyx_nargs); __PYX_ERR(0, 29, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -8859,15 +8895,15 @@
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__4)
-  __Pyx_RefNannySetupContext("pdf_array", 0);
+  __Pyx_RefNannySetupContext("pdf_array", 1);
   __Pyx_TraceCall("pdf_array", __pyx_f[0], 29, 0, __PYX_ERR(0, 29, __pyx_L1_error));
   __pyx_pybuffer_y.pybuffer.buf = NULL;
   __pyx_pybuffer_y.refcount = 0;
   __pyx_pybuffernd_y.data = NULL;
   __pyx_pybuffernd_y.rcbuffer = &__pyx_pybuffer_y;
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
@@ -9291,19 +9327,17 @@
  *     return (p_outlier >= 0) & (p_outlier <= 1)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_4wfpt_p_outlier_in_range(double __pyx_v_p_outlier) {
   int __pyx_r;
   __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("p_outlier_in_range", 0);
   __Pyx_TraceCall("p_outlier_in_range", __pyx_f[0], 47, 0, __PYX_ERR(0, 47, __pyx_L1_error));
 
   /* "wfpt.pyx":48
  * 
  * cdef inline bint p_outlier_in_range(double p_outlier):
  *     return (p_outlier >= 0) & (p_outlier <= 1)             # <<<<<<<<<<<<<<
  * 
@@ -9323,15 +9357,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("wfpt.p_outlier_in_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "wfpt.pyx":51
  * 
  * 
  * def wiener_like(np.ndarray[double, ndim=1] x, double v, double sv, double a, double z, double sz, double t,             # <<<<<<<<<<<<<<
@@ -9382,16 +9415,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 51, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -9628,18 +9660,19 @@
     }
     if (values[14]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[14]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.1));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like", 0, 9, 15, __pyx_nargs); __PYX_ERR(0, 51, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -9687,15 +9720,15 @@
   Py_ssize_t __pyx_t_9;
   double __pyx_t_10;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__5)
-  __Pyx_RefNannySetupContext("wiener_like", 0);
+  __Pyx_RefNannySetupContext("wiener_like", 1);
   __Pyx_TraceCall("wiener_like", __pyx_f[0], 51, 0, __PYX_ERR(0, 51, __pyx_L1_error));
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
   __pyx_pybuffernd_x.data = NULL;
   __pyx_pybuffernd_x.rcbuffer = &__pyx_pybuffer_x;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
@@ -9979,16 +10012,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like_rlddm (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 75, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_response,&__pyx_n_s_feedback,&__pyx_n_s_split_by,&__pyx_n_s_q,&__pyx_n_s_alpha,&__pyx_n_s_pos_alpha,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -10309,18 +10341,19 @@
     }
     if (values[20]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[20]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like_rlddm", 0, 15, 21, __pyx_nargs); __PYX_ERR(0, 75, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -10418,15 +10451,15 @@
   Py_ssize_t __pyx_t_30;
   double __pyx_t_31;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_32;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__6)
-  __Pyx_RefNannySetupContext("wiener_like_rlddm", 0);
+  __Pyx_RefNannySetupContext("wiener_like_rlddm", 1);
   __Pyx_TraceCall("wiener_like_rlddm", __pyx_f[0], 75, 0, __PYX_ERR(0, 75, __pyx_L1_error));
   __pyx_pybuffer_qs.pybuffer.buf = NULL;
   __pyx_pybuffer_qs.refcount = 0;
   __pyx_pybuffernd_qs.data = NULL;
   __pyx_pybuffernd_qs.rcbuffer = &__pyx_pybuffer_qs;
   __pyx_pybuffer_xs.pybuffer.buf = NULL;
   __pyx_pybuffer_xs.refcount = 0;
@@ -11269,16 +11302,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like_rl (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 152, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_response,&__pyx_n_s_feedback,&__pyx_n_s_split_by,&__pyx_n_s_q,&__pyx_n_s_alpha,&__pyx_n_s_pos_alpha,&__pyx_n_s_v,&__pyx_n_s_z,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -11517,18 +11549,19 @@
     }
     if (values[14]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[14]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like_rl", 0, 8, 15, __pyx_nargs); __PYX_ERR(0, 152, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -11618,15 +11651,15 @@
   Py_ssize_t __pyx_t_27;
   Py_ssize_t __pyx_t_28;
   Py_ssize_t __pyx_t_29;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__7)
-  __Pyx_RefNannySetupContext("wiener_like_rl", 0);
+  __Pyx_RefNannySetupContext("wiener_like_rl", 1);
   __Pyx_TraceCall("wiener_like_rl", __pyx_f[0], 152, 0, __PYX_ERR(0, 152, __pyx_L1_error));
   __pyx_pybuffer_qs.pybuffer.buf = NULL;
   __pyx_pybuffer_qs.refcount = 0;
   __pyx_pybuffernd_qs.data = NULL;
   __pyx_pybuffernd_qs.rcbuffer = &__pyx_pybuffer_qs;
   __pyx_pybuffer_feedbacks.pybuffer.buf = NULL;
   __pyx_pybuffer_feedbacks.refcount = 0;
@@ -12486,16 +12519,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like_multi (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 239, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_multi,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     values[9] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     if (__pyx_kwds) {
@@ -12745,18 +12777,19 @@
     }
     if (values[15]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[15]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like_multi", 0, 9, 16, __pyx_nargs); __PYX_ERR(0, 239, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -12818,15 +12851,15 @@
   PyObject *(*__pyx_t_20)(PyObject *);
   Py_ssize_t __pyx_t_21;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_22;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__8)
-  __Pyx_RefNannySetupContext("wiener_like_multi", 0);
+  __Pyx_RefNannySetupContext("wiener_like_multi", 1);
   __Pyx_TraceCall("wiener_like_multi", __pyx_f[0], 239, 0, __PYX_ERR(0, 239, __pyx_L1_error));
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
   __pyx_pybuffernd_x.data = NULL;
   __pyx_pybuffernd_x.rcbuffer = &__pyx_pybuffer_x;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
@@ -12993,37 +13026,50 @@
  *         for i in range(size):
  *             for param in multi:             # <<<<<<<<<<<<<<
  *                 params_iter[param] = params[param][i]
  *             if abs(x[i]) != 999.:
  */
       __Pyx_TraceLine(254,0,__PYX_ERR(0, 254, __pyx_L1_error))
       if (likely(PyList_CheckExact(__pyx_v_multi)) || PyTuple_CheckExact(__pyx_v_multi)) {
-        __pyx_t_12 = __pyx_v_multi; __Pyx_INCREF(__pyx_t_12); __pyx_t_19 = 0;
+        __pyx_t_12 = __pyx_v_multi; __Pyx_INCREF(__pyx_t_12);
+        __pyx_t_19 = 0;
         __pyx_t_20 = NULL;
       } else {
         __pyx_t_19 = -1; __pyx_t_12 = PyObject_GetIter(__pyx_v_multi); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 254, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __pyx_t_20 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_12); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 254, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_20)) {
           if (likely(PyList_CheckExact(__pyx_t_12))) {
-            if (__pyx_t_19 >= PyList_GET_SIZE(__pyx_t_12)) break;
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_12);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 254, __pyx_L1_error)
+              #endif
+              if (__pyx_t_19 >= __pyx_temp) break;
+            }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             __pyx_t_13 = PyList_GET_ITEM(__pyx_t_12, __pyx_t_19); __Pyx_INCREF(__pyx_t_13); __pyx_t_19++; if (unlikely((0 < 0))) __PYX_ERR(0, 254, __pyx_L1_error)
             #else
-            __pyx_t_13 = PySequence_ITEM(__pyx_t_12, __pyx_t_19); __pyx_t_19++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 254, __pyx_L1_error)
+            __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_19); __pyx_t_19++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 254, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_13);
             #endif
           } else {
-            if (__pyx_t_19 >= PyTuple_GET_SIZE(__pyx_t_12)) break;
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_12);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 254, __pyx_L1_error)
+              #endif
+              if (__pyx_t_19 >= __pyx_temp) break;
+            }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             __pyx_t_13 = PyTuple_GET_ITEM(__pyx_t_12, __pyx_t_19); __Pyx_INCREF(__pyx_t_13); __pyx_t_19++; if (unlikely((0 < 0))) __PYX_ERR(0, 254, __pyx_L1_error)
             #else
-            __pyx_t_13 = PySequence_ITEM(__pyx_t_12, __pyx_t_19); __pyx_t_19++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 254, __pyx_L1_error)
+            __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_19); __pyx_t_19++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 254, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_13);
             #endif
           }
         } else {
           __pyx_t_13 = __pyx_t_20(__pyx_t_12);
           if (unlikely(!__pyx_t_13)) {
             PyObject* exc_type = PyErr_Occurred();
@@ -13352,16 +13398,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_logp_array (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 271, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -13598,18 +13643,19 @@
     }
     if (values[14]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[14]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.1));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_logp_array", 0, 9, 15, __pyx_nargs); __PYX_ERR(0, 271, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -13692,15 +13738,15 @@
   double __pyx_t_21;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_22;
   int __pyx_t_23;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__9)
-  __Pyx_RefNannySetupContext("wiener_logp_array", 0);
+  __Pyx_RefNannySetupContext("wiener_logp_array", 1);
   __Pyx_TraceCall("wiener_logp_array", __pyx_f[0], 271, 0, __PYX_ERR(0, 271, __pyx_L1_error));
   __pyx_pybuffer_logp.pybuffer.buf = NULL;
   __pyx_pybuffer_logp.refcount = 0;
   __pyx_pybuffernd_logp.data = NULL;
   __pyx_pybuffernd_logp.rcbuffer = &__pyx_pybuffer_logp;
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
@@ -14162,16 +14208,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like_multi_rlddm (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 311, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_response,&__pyx_n_s_feedback,&__pyx_n_s_split_by,&__pyx_n_s_q,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_alpha,&__pyx_n_s_err,&__pyx_n_s_multi,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
 
     /* "wfpt.pyx":315
@@ -14499,18 +14544,19 @@
     }
     if (values[20]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[20]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like_multi_rlddm", 0, 14, 21, __pyx_nargs); __PYX_ERR(0, 311, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -14596,15 +14642,15 @@
   PyObject *(*__pyx_t_23)(PyObject *);
   Py_ssize_t __pyx_t_24;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_25;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__11)
-  __Pyx_RefNannySetupContext("wiener_like_multi_rlddm", 0);
+  __Pyx_RefNannySetupContext("wiener_like_multi_rlddm", 1);
   __Pyx_TraceCall("wiener_like_multi_rlddm", __pyx_f[0], 311, 0, __PYX_ERR(0, 311, __pyx_L1_error));
   __pyx_pybuffer_qs.pybuffer.buf = NULL;
   __pyx_pybuffer_qs.refcount = 0;
   __pyx_pybuffernd_qs.data = NULL;
   __pyx_pybuffernd_qs.rcbuffer = &__pyx_pybuffer_qs;
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
@@ -14879,38 +14925,51 @@
     __Pyx_TraceLine(334,0,__PYX_ERR(0, 334, __pyx_L1_error))
     __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
-      __pyx_t_2 = __pyx_t_4; __Pyx_INCREF(__pyx_t_2); __pyx_t_20 = 0;
+      __pyx_t_2 = __pyx_t_4; __Pyx_INCREF(__pyx_t_2);
+      __pyx_t_20 = 0;
       __pyx_t_21 = NULL;
     } else {
       __pyx_t_20 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_21 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 334, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     for (;;) {
       if (likely(!__pyx_t_21)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_20 >= PyList_GET_SIZE(__pyx_t_2)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 334, __pyx_L1_error)
+            #endif
+            if (__pyx_t_20 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_20); __Pyx_INCREF(__pyx_t_4); __pyx_t_20++; if (unlikely((0 < 0))) __PYX_ERR(0, 334, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_20); __pyx_t_20++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_20); __pyx_t_20++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
-          if (__pyx_t_20 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 334, __pyx_L1_error)
+            #endif
+            if (__pyx_t_20 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_20); __Pyx_INCREF(__pyx_t_4); __pyx_t_20++; if (unlikely((0 < 0))) __PYX_ERR(0, 334, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_20); __pyx_t_20++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_20); __pyx_t_20++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_21(__pyx_t_2);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
@@ -14930,37 +14989,50 @@
  *         for i in range(size):
  *             for param in multi:             # <<<<<<<<<<<<<<
  *                 params_iter[param] = params[param][i]
  * 
  */
       __Pyx_TraceLine(335,0,__PYX_ERR(0, 335, __pyx_L1_error))
       if (likely(PyList_CheckExact(__pyx_v_multi)) || PyTuple_CheckExact(__pyx_v_multi)) {
-        __pyx_t_4 = __pyx_v_multi; __Pyx_INCREF(__pyx_t_4); __pyx_t_22 = 0;
+        __pyx_t_4 = __pyx_v_multi; __Pyx_INCREF(__pyx_t_4);
+        __pyx_t_22 = 0;
         __pyx_t_23 = NULL;
       } else {
         __pyx_t_22 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_multi); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_23 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 335, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_23)) {
           if (likely(PyList_CheckExact(__pyx_t_4))) {
-            if (__pyx_t_22 >= PyList_GET_SIZE(__pyx_t_4)) break;
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
+              #endif
+              if (__pyx_t_22 >= __pyx_temp) break;
+            }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             __pyx_t_6 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_22); __Pyx_INCREF(__pyx_t_6); __pyx_t_22++; if (unlikely((0 < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_4, __pyx_t_22); __pyx_t_22++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
+            __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_22); __pyx_t_22++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           } else {
-            if (__pyx_t_22 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
+              #endif
+              if (__pyx_t_22 >= __pyx_temp) break;
+            }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_22); __Pyx_INCREF(__pyx_t_6); __pyx_t_22++; if (unlikely((0 < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_4, __pyx_t_22); __pyx_t_22++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
+            __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_22); __pyx_t_22++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           }
         } else {
           __pyx_t_6 = __pyx_t_23(__pyx_t_4);
           if (unlikely(!__pyx_t_6)) {
             PyObject* exc_type = PyErr_Occurred();
@@ -15373,16 +15445,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("gen_rts_from_cdf (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 356, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_samples,&__pyx_n_s_cdf_lb,&__pyx_n_s_cdf_ub,&__pyx_n_s_dt,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -15559,18 +15630,19 @@
     }
     if (values[10]) {
       __pyx_v_dt = __pyx_PyFloat_AsDouble(values[10]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L3_error)
     } else {
       __pyx_v_dt = ((double)((double)1e-2));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("gen_rts_from_cdf", 0, 7, 11, __pyx_nargs); __PYX_ERR(0, 356, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -15625,28 +15697,27 @@
   PyArrayObject *__pyx_t_8 = NULL;
   npy_intp *__pyx_t_9;
   PyArrayObject *__pyx_t_10 = NULL;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   double __pyx_t_13;
   Py_ssize_t __pyx_t_14;
-  npy_intp __pyx_t_15;
+  PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
-  PyObject *__pyx_t_18 = NULL;
+  PyArrayObject *__pyx_t_18 = NULL;
   PyArrayObject *__pyx_t_19 = NULL;
-  PyArrayObject *__pyx_t_20 = NULL;
-  int __pyx_t_21;
-  PyArrayObject *__pyx_t_22 = NULL;
-  int __pyx_t_23;
+  int __pyx_t_20;
+  PyArrayObject *__pyx_t_21 = NULL;
+  int __pyx_t_22;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__12)
-  __Pyx_RefNannySetupContext("gen_rts_from_cdf", 0);
+  __Pyx_RefNannySetupContext("gen_rts_from_cdf", 1);
   __Pyx_TraceCall("gen_rts_from_cdf", __pyx_f[0], 356, 0, __PYX_ERR(0, 356, __pyx_L1_error));
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
   __pyx_pybuffernd_x.data = NULL;
   __pyx_pybuffernd_x.rcbuffer = &__pyx_pybuffer_x;
   __pyx_pybuffer_l_cdf.pybuffer.buf = NULL;
   __pyx_pybuffer_l_cdf.refcount = 0;
@@ -15733,15 +15804,15 @@
   __Pyx_TraceLine(360,0,__PYX_ERR(0, 360, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_x)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t((__pyx_t_9[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_t_9[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
@@ -15835,35 +15906,35 @@
  * 
  *     l_cdf /= l_cdf[x.shape[0] - 1]             # <<<<<<<<<<<<<<
  * 
  *     cdef np.ndarray[double, ndim = 1] rts = np.empty(samples, dtype=np.double)
  */
   __Pyx_TraceLine(371,0,__PYX_ERR(0, 371, __pyx_L1_error))
   __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_x)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
-  __pyx_t_15 = ((__pyx_t_9[0]) - 1);
-  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_l_cdf.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_l_cdf.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_11 = ((__pyx_t_9[0]) - 1);
+  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_l_cdf.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_l_cdf.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyNumber_InPlaceDivide(((PyObject *)__pyx_v_l_cdf), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 371, __pyx_L1_error)
   __pyx_t_10 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_l_cdf.rcbuffer->pybuffer);
     __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_l_cdf.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_7 < 0)) {
-      PyErr_Fetch(&__pyx_t_16, &__pyx_t_17, &__pyx_t_18);
+      PyErr_Fetch(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_l_cdf.rcbuffer->pybuffer, (PyObject*)__pyx_v_l_cdf, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
-        Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_17); Py_XDECREF(__pyx_t_18);
+        Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_17);
         __Pyx_RaiseBufferFallbackError();
       } else {
-        PyErr_Restore(__pyx_t_16, __pyx_t_17, __pyx_t_18);
+        PyErr_Restore(__pyx_t_15, __pyx_t_16, __pyx_t_17);
       }
-      __pyx_t_16 = __pyx_t_17 = __pyx_t_18 = 0;
+      __pyx_t_15 = __pyx_t_16 = __pyx_t_17 = 0;
     }
     __pyx_pybuffernd_l_cdf.diminfo[0].strides = __pyx_pybuffernd_l_cdf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_l_cdf.diminfo[0].shape = __pyx_pybuffernd_l_cdf.rcbuffer->pybuffer.shape[0];
     if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 371, __pyx_L1_error)
   }
   __pyx_t_10 = 0;
   __Pyx_DECREF_SET(__pyx_v_l_cdf, ((PyArrayObject *)__pyx_t_1));
   __pyx_t_1 = 0;
@@ -15899,24 +15970,24 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 373, __pyx_L1_error)
-  __pyx_t_19 = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_18 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rts.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rts.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_rts = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rts.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 373, __pyx_L1_error)
     } else {__pyx_pybuffernd_rts.diminfo[0].strides = __pyx_pybuffernd_rts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rts.diminfo[0].shape = __pyx_pybuffernd_rts.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_19 = 0;
+  __pyx_t_18 = 0;
   __pyx_v_rts = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "wfpt.pyx":374
  * 
  *     cdef np.ndarray[double, ndim = 1] rts = np.empty(samples, dtype=np.double)
  *     cdef np.ndarray[double, ndim = 1] f = np.random.rand(samples)             # <<<<<<<<<<<<<<
@@ -15954,37 +16025,37 @@
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 374, __pyx_L1_error)
-  __pyx_t_20 = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_19 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_f.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_f.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_f = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_f.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 374, __pyx_L1_error)
     } else {__pyx_pybuffernd_f.diminfo[0].strides = __pyx_pybuffernd_f.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_f.diminfo[0].shape = __pyx_pybuffernd_f.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_20 = 0;
+  __pyx_t_19 = 0;
   __pyx_v_f = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "wfpt.pyx":377
  *     cdef np.ndarray[double, ndim = 1] delay
  * 
  *     if st != 0:             # <<<<<<<<<<<<<<
  *         delay = (np.random.rand(samples) * st + (t - st / 2.))
  *     for i from 0 <= i < samples:
  */
   __Pyx_TraceLine(377,0,__PYX_ERR(0, 377, __pyx_L1_error))
-  __pyx_t_21 = (__pyx_v_st != 0.0);
-  if (__pyx_t_21) {
+  __pyx_t_20 = (__pyx_v_st != 0.0);
+  if (__pyx_t_20) {
 
     /* "wfpt.pyx":378
  * 
  *     if st != 0:
  *         delay = (np.random.rand(samples) * st + (t - st / 2.))             # <<<<<<<<<<<<<<
  *     for i from 0 <= i < samples:
  *         idx = np.searchsorted(l_cdf, f[i])
@@ -16032,33 +16103,33 @@
     __pyx_t_1 = PyFloat_FromDouble((__pyx_v_t - (__pyx_v_st / 2.))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 378, __pyx_L1_error)
-    __pyx_t_22 = ((PyArrayObject *)__pyx_t_4);
+    __pyx_t_21 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_delay.rcbuffer->pybuffer);
-      __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_delay.rcbuffer->pybuffer, (PyObject*)__pyx_t_22, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_delay.rcbuffer->pybuffer, (PyObject*)__pyx_t_21, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_7 < 0)) {
-        PyErr_Fetch(&__pyx_t_18, &__pyx_t_17, &__pyx_t_16);
+        PyErr_Fetch(&__pyx_t_17, &__pyx_t_16, &__pyx_t_15);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_delay.rcbuffer->pybuffer, (PyObject*)__pyx_v_delay, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_18); Py_XDECREF(__pyx_t_17); Py_XDECREF(__pyx_t_16);
+          Py_XDECREF(__pyx_t_17); Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_15);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_18, __pyx_t_17, __pyx_t_16);
+          PyErr_Restore(__pyx_t_17, __pyx_t_16, __pyx_t_15);
         }
-        __pyx_t_18 = __pyx_t_17 = __pyx_t_16 = 0;
+        __pyx_t_17 = __pyx_t_16 = __pyx_t_15 = 0;
       }
       __pyx_pybuffernd_delay.diminfo[0].strides = __pyx_pybuffernd_delay.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_delay.diminfo[0].shape = __pyx_pybuffernd_delay.rcbuffer->pybuffer.shape[0];
       if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 378, __pyx_L1_error)
     }
-    __pyx_t_22 = 0;
+    __pyx_t_21 = 0;
     __pyx_v_delay = ((PyArrayObject *)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "wfpt.pyx":377
  *     cdef np.ndarray[double, ndim = 1] delay
  * 
  *     if st != 0:             # <<<<<<<<<<<<<<
@@ -16091,39 +16162,39 @@
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_searchsorted); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_f.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_f.diminfo[0].strides))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = NULL;
-    __pyx_t_23 = 0;
+    __pyx_t_22 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_23 = 1;
+        __pyx_t_22 = 1;
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_2, ((PyObject *)__pyx_v_l_cdf), __pyx_t_1};
-      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_23, 2+__pyx_t_23);
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_22, 2+__pyx_t_22);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 380, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_23 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_23 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_22 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_idx = __pyx_t_23;
+    __pyx_v_idx = __pyx_t_22;
 
     /* "wfpt.pyx":381
  *     for i from 0 <= i < samples:
  *         idx = np.searchsorted(l_cdf, f[i])
  *         rt = x[idx]             # <<<<<<<<<<<<<<
  *         if st == 0:
  *             rt = rt + np.sign(rt) * t
@@ -16136,16 +16207,16 @@
  *         idx = np.searchsorted(l_cdf, f[i])
  *         rt = x[idx]
  *         if st == 0:             # <<<<<<<<<<<<<<
  *             rt = rt + np.sign(rt) * t
  *         else:
  */
     __Pyx_TraceLine(382,0,__PYX_ERR(0, 382, __pyx_L1_error))
-    __pyx_t_21 = (__pyx_v_st == 0.0);
-    if (__pyx_t_21) {
+    __pyx_t_20 = (__pyx_v_st == 0.0);
+    if (__pyx_t_20) {
 
       /* "wfpt.pyx":383
  *         rt = x[idx]
  *         if st == 0:
  *             rt = rt + np.sign(rt) * t             # <<<<<<<<<<<<<<
  *         else:
  *             rt = rt + np.sign(rt) * delay[i]
@@ -16157,30 +16228,30 @@
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sign); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_3 = NULL;
-      __pyx_t_23 = 0;
+      __pyx_t_22 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
-          __pyx_t_23 = 1;
+          __pyx_t_22 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_1};
-        __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_23, 1+__pyx_t_23);
+        __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_22, 1+__pyx_t_22);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __pyx_t_2 = PyFloat_FromDouble(__pyx_v_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
@@ -16222,30 +16293,30 @@
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sign); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = PyFloat_FromDouble(__pyx_v_rt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_3 = NULL;
-      __pyx_t_23 = 0;
+      __pyx_t_22 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
-          __pyx_t_23 = 1;
+          __pyx_t_22 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
-        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_23, 1+__pyx_t_23);
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_22, 1+__pyx_t_22);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __pyx_t_11 = __pyx_v_i;
@@ -16389,16 +16460,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wiener_like_contaminant (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 390, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_cont_x,&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_t_min,&__pyx_n_s_t_max,&__pyx_n_s_err,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -16645,18 +16715,19 @@
     }
     if (values[15]) {
       __pyx_v_simps_err = __pyx_PyFloat_AsDouble(values[15]); if (unlikely((__pyx_v_simps_err == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L3_error)
     } else {
       __pyx_v_simps_err = ((double)((double)1e-8));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("wiener_like_contaminant", 0, 12, 16, __pyx_nargs); __PYX_ERR(0, 390, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -16709,15 +16780,15 @@
   int __pyx_t_10;
   double __pyx_t_11;
   struct __pyx_opt_args_4wfpt_full_pdf __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__13)
-  __Pyx_RefNannySetupContext("wiener_like_contaminant", 0);
+  __Pyx_RefNannySetupContext("wiener_like_contaminant", 1);
   __Pyx_TraceCall("wiener_like_contaminant", __pyx_f[0], 390, 0, __PYX_ERR(0, 390, __pyx_L1_error));
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
   __pyx_pybuffernd_x.data = NULL;
   __pyx_pybuffernd_x.rcbuffer = &__pyx_pybuffer_x;
   __pyx_pybuffer_cont_x.pybuffer.buf = NULL;
   __pyx_pybuffer_cont_x.refcount = 0;
@@ -17221,16 +17292,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("gen_cdf_using_pdf (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 421, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v,&__pyx_n_s_sv,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_sz,&__pyx_n_s_t,&__pyx_n_s_st,&__pyx_n_s_err,&__pyx_n_s_N,&__pyx_n_s_time,&__pyx_n_s_n_st,&__pyx_n_s_n_sz,&__pyx_n_s_use_adaptive,&__pyx_n_s_simps_err,&__pyx_n_s_p_outlier,&__pyx_n_s_w_outlier,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -17485,18 +17555,19 @@
     }
     if (values[15]) {
       __pyx_v_w_outlier = __pyx_PyFloat_AsDouble(values[15]); if (unlikely((__pyx_v_w_outlier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 423, __pyx_L3_error)
     } else {
       __pyx_v_w_outlier = ((double)((double)0.0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("gen_cdf_using_pdf", 0, 8, 16, __pyx_nargs); __PYX_ERR(0, 421, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -17550,20 +17621,20 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
   PyObject *__pyx_t_26 = NULL;
   PyObject *__pyx_t_27 = NULL;
-  npy_intp __pyx_t_28;
+  Py_ssize_t __pyx_t_28;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__14)
-  __Pyx_RefNannySetupContext("gen_cdf_using_pdf", 0);
+  __Pyx_RefNannySetupContext("gen_cdf_using_pdf", 1);
   __Pyx_TraceCall("gen_cdf_using_pdf", __pyx_f[0], 421, 0, __PYX_ERR(0, 421, __pyx_L1_error));
   __pyx_pybuffer_x.pybuffer.buf = NULL;
   __pyx_pybuffer_x.refcount = 0;
   __pyx_pybuffernd_x.data = NULL;
   __pyx_pybuffernd_x.rcbuffer = &__pyx_pybuffer_x;
   __pyx_pybuffer_cdf_array.pybuffer.buf = NULL;
   __pyx_pybuffer_cdf_array.refcount = 0;
@@ -17759,15 +17830,15 @@
   __Pyx_TraceLine(433,0,__PYX_ERR(0, 433, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_12 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_x)); if (unlikely(__pyx_t_12 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_12[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_Py_intptr_t((__pyx_t_12[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_4);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
@@ -18097,16 +18168,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("split_cdf (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 449, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_data,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -18147,18 +18217,19 @@
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_x = ((PyArrayObject *)values[0]);
     __pyx_v_data = ((PyArrayObject *)values[1]);
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("split_cdf", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 449, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -18224,15 +18295,15 @@
   PyArrayObject *__pyx_t_16 = NULL;
   PyArrayObject *__pyx_t_17 = NULL;
   Py_ssize_t __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__17)
-  __Pyx_RefNannySetupContext("split_cdf", 0);
+  __Pyx_RefNannySetupContext("split_cdf", 1);
   __Pyx_TraceCall("split_cdf", __pyx_f[0], 449, 0, __PYX_ERR(0, 449, __pyx_L1_error));
   __pyx_pybuffer_x_lb.pybuffer.buf = NULL;
   __pyx_pybuffer_x_lb.refcount = 0;
   __pyx_pybuffernd_x_lb.data = NULL;
   __pyx_pybuffernd_x_lb.rcbuffer = &__pyx_pybuffer_x_lb;
   __pyx_pybuffer_lb.pybuffer.buf = NULL;
   __pyx_pybuffer_lb.refcount = 0;
@@ -18828,44 +18899,44 @@
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 63, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 429, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "wfpt.pyx":294
  * 
  *     if not p_outlier_in_range(p_outlier):
  *         logp[:] = -np.inf             # <<<<<<<<<<<<<<
@@ -19104,14 +19175,21 @@
     "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
 }
 #endif
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
+  /* InitThreads.init */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
+PyEval_InitThreads();
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -19160,41 +19238,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 865, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -19409,42 +19487,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("wfpt", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to wfpt pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "wfpt" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_wfpt(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -19502,242 +19578,242 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_wfpt(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
   __Pyx_TraceLine(245,0,__PYX_ERR(1, 245, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
   __Pyx_TraceLine(251,0,__PYX_ERR(1, 251, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
   __Pyx_TraceLine(257,0,__PYX_ERR(1, 257, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
   __Pyx_TraceLine(263,0,__PYX_ERR(1, 263, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
   __Pyx_TraceLine(271,0,__PYX_ERR(1, 271, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
   __Pyx_TraceLine(278,0,__PYX_ERR(1, 278, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
   __Pyx_TraceLine(284,0,__PYX_ERR(1, 284, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
   __Pyx_TraceLine(773,0,__PYX_ERR(1, 773, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
   __Pyx_TraceLine(776,0,__PYX_ERR(1, 776, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
   __Pyx_TraceLine(779,0,__PYX_ERR(1, 779, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
   __Pyx_TraceLine(782,0,__PYX_ERR(1, 782, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
   __Pyx_TraceLine(785,0,__PYX_ERR(1, 785, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
   __Pyx_TraceLine(788,0,__PYX_ERR(1, 788, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
-  __Pyx_TraceLine(967,0,__PYX_ERR(1, 967, __pyx_L1_error))
+  __Pyx_TraceLine(968,0,__PYX_ERR(1, 968, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
-  __Pyx_TraceLine(971,0,__PYX_ERR(1, 971, __pyx_L1_error))
+  __Pyx_TraceLine(972,0,__PYX_ERR(1, 972, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
-  __Pyx_TraceLine(979,0,__PYX_ERR(1, 979, __pyx_L1_error))
+  __Pyx_TraceLine(980,0,__PYX_ERR(1, 980, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(985,0,__PYX_ERR(1, 985, __pyx_L1_error))
+  __Pyx_TraceLine(986,0,__PYX_ERR(1, 986, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(991,0,__PYX_ERR(1, 991, __pyx_L1_error))
+  __Pyx_TraceLine(992,0,__PYX_ERR(1, 992, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
-  __Pyx_TraceLine(998,0,__PYX_ERR(1, 998, __pyx_L1_error))
+  __Pyx_TraceLine(999,0,__PYX_ERR(1, 999, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
-  __Pyx_TraceLine(1013,0,__PYX_ERR(1, 1013, __pyx_L1_error))
+  __Pyx_TraceLine(1014,0,__PYX_ERR(1, 1014, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
-  __Pyx_TraceLine(1028,0,__PYX_ERR(1, 1028, __pyx_L1_error))
+  __Pyx_TraceLine(1029,0,__PYX_ERR(1, 1029, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
-  __Pyx_TraceLine(1038,0,__PYX_ERR(1, 1038, __pyx_L1_error))
+  __Pyx_TraceLine(1039,0,__PYX_ERR(1, 1039, __pyx_L1_error))
 
 
-  /* "../../../../../tmp/build-env-ba2wxypz/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-mg_9yzta/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
-  __Pyx_TraceLine(1045,0,__PYX_ERR(1, 1045, __pyx_L1_error))
+  __Pyx_TraceLine(1046,0,__PYX_ERR(1, 1046, __pyx_L1_error))
 
 
   /* "wfpt.pyx":16
  * # GPLv3
  * 
  * import scipy.integrate as integrate             # <<<<<<<<<<<<<<
  * from copy import copy
@@ -20765,14 +20841,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -20822,33 +20900,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -21131,16 +21216,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -21517,20 +21607,38 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
+}
+#endif
 #endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
@@ -21616,15 +21724,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -21635,15 +21743,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -21667,15 +21775,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -22351,15 +22459,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -22456,17 +22564,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -22533,67 +22647,62 @@
 #endif
 
 /* PyObjectCallMethO */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
-  static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+  #if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
         Py_INCREF(args[i]);
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -22609,33 +22718,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
@@ -22718,15 +22833,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -22753,15 +22868,17 @@
     }
     return NULL;
 }
 static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
     __Pyx_TypeName obj_type_name;
     if (likely(PyType_Check(obj))) {
         PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (meth) {
+        if (!meth) {
+            PyErr_Clear();
+        } else {
             PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
             Py_DECREF(meth);
             return result;
         }
     }
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
@@ -23142,18 +23259,18 @@
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -23199,23 +23316,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -23244,15 +23361,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -23525,18 +23642,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
   static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
   static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -23689,15 +23803,29 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
-  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
@@ -24498,15 +24626,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -24837,16 +24965,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -24858,14 +24986,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -24955,15 +25085,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -25529,15 +25659,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -25665,38 +25795,104 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
+        Py_XDECREF(kwds);
         Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(Py_intptr_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(Py_intptr_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(Py_intptr_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
@@ -25727,38 +25923,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* FormatTypeName */
   #if CYTHON_COMPILING_IN_LIMITED_API
@@ -25942,15 +26140,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -26162,49 +26360,58 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -26242,16 +26449,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `hddm_wfpt-0.1.2/hddm_wfpt/cdfdif.c` & `hddm_wfpt-0.1.4/hddm_wfpt/cdfdif.c`

 * *Files identical despite different names*

### Comparing `hddm_wfpt-0.1.2/hddm_wfpt.egg-info/PKG-INFO` & `hddm_wfpt-0.1.4/hddm_wfpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hddm-wfpt
-Version: 0.1.2
+Name: hddm_wfpt
+Version: 0.1.4
 Summary: HDDM is a python module that implements Hierarchical Bayesian estimation of Drift Diffusion Models.
 Author-email: Alexander Fengler <alexander_fengler@brown.edu>, Paul Xu <yang_xu@brown.edu>, Michael Frank <michael_frank@brown.edu>
 Project-URL: Homepage, https://github.com/lnccbrown/hddm-wfpt
 Project-URL: Bug Tracker, https://github.com/lnccbrown/hddm-wfpt/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `hddm_wfpt-0.1.2/pyproject.toml` & `hddm_wfpt-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hddm_wfpt"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
     { name = "Alexander Fengler", email = "alexander_fengler@brown.edu" },
     { name = "Paul Xu", email = "yang_xu@brown.edu" },
     { name = "Michael Frank", email = "michael_frank@brown.edu" },
 ]
 description = "HDDM is a python module that implements Hierarchical Bayesian estimation of Drift Diffusion Models."
 readme = "Readme.rst"
```

### Comparing `hddm_wfpt-0.1.2/setup.py` & `hddm_wfpt-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,34 +13,41 @@
             "wfpt",
             ["hddm_wfpt/wfpt.pyx"],
             language="c++",
             extra_compile_args=["-stdlib=libc++"],
             extra_link_args=["-stdlib=libc++", "-mmacosx-version-min=10.9"],
         )
     else:
-        ext1 = Extension("wfpt", ["hddm_wfpt/wfpt.pyx"], language="c++")
+        ext1 = Extension(
+            "wfpt",
+            ["hddm_wfpt/wfpt.pyx"],
+            language="c++",
+        )
 
     ext_modules = cythonize(
         [
             ext1,
             Extension(
                 "cdfdif_wrapper",
                 ["hddm_wfpt/cdfdif_wrapper.pyx", "hddm_wfpt/cdfdif.c"],
             ),
         ],
         build_dir="cython_build",
         compiler_directives={"language_level": "3", "linetrace": True},
     )
 
 except ImportError:
-
     ext_modules = [
-        Extension("wfpt", ["hddm_wfpt/wfpt.cpp"], language="c++"),
+        Extension("wfpt", ["cython_build/hddm_wfpt/wfpt.cpp"], language="c++"),
         Extension(
-            "cdfdif_wrapper", ["hddm_wfpt/cdfdif_wrapper.c", "hddm_wfpt/cdfdif.c"]
+            "cdfdif_wrapper",
+            [
+                "cython_build/hddm_wfpt/cdfdif_wrapper.c",
+                "cython_build/hddm_wfpt/cdfdif.c",
+            ],
         ),
     ]
 
 setup(
     packages=["hddm_wfpt"],
     include_dirs=[np.get_include()],
     ext_modules=ext_modules,
```

