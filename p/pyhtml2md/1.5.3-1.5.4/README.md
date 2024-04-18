# Comparing `tmp/pyhtml2md-1.5.3.tar.gz` & `tmp/pyhtml2md-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml2md-1.5.3.tar", last modified: Mon Aug 21 17:47:00 2023, max compression
+gzip compressed data, was "pyhtml2md-1.5.4.tar", last modified: Thu Apr 18 07:59:18 2024, max compression
```

## Comparing `pyhtml2md-1.5.3.tar` & `pyhtml2md-1.5.4.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.559317 pyhtml2md-1.5.3/include/
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/include/html2md.h
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/include/table.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.559317 pyhtml2md-1.5.3/pyhtml2md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-21 17:47:00.000000 pyhtml2md-1.5.3/pyhtml2md.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.559317 pyhtml2md-1.5.3/python/
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/python/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/python/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.559317 pyhtml2md-1.5.3/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.559317 pyhtml2md-1.5.3/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.563317 pyhtml2md-1.5.3/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.563317 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    53759 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    48364 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (123)    32135 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79725 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126706 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    98078 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-21 17:46:49.000000 pyhtml2md-1.5.3/python/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/src/html2md.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/src/table.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 17:47:00.567317 pyhtml2md-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/tests/test_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-21 17:46:47.000000 pyhtml2md-1.5.3/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/include/html2md.h
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/include/table.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/pyhtml2md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.705184 pyhtml2md-1.5.4/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71139 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53818 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29071 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49998 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84243 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   129569 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98953 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28463 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/typing.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    23244 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/src/html2md.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/src/table.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/tests/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/tests/test_basic.py
```

### Comparing `pyhtml2md-1.5.3/CMakeLists.txt` & `pyhtml2md-1.5.4/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.8)
-project(html2md VERSION 1.5.3 LANGUAGES CXX)
+project(html2md VERSION 1.5.4 LANGUAGES CXX)
 
 set(PROJECT_HOMEPAGE_URL "https://tim-gromeyer.github.io/html2md/")
 set(html2md_HOMEPAGE_URL "${PROJECT_HOMEPAGE_URL}")
 
 set(PROJECT_DESCRIPTION "Transform your HTML into clean, easy-to-read markdown with html2md")
 set(html2md_DESCRIPTION "${PROJECT_DESCRIPTION}")
```

### Comparing `pyhtml2md-1.5.3/COPYING` & `pyhtml2md-1.5.4/COPYING`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/PKG-INFO` & `pyhtml2md-1.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyhtml2md
-Version: 1.5.3
+Version: 1.5.4
 Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
 Home-page: https://github.com/tim-gromeyer/html2md
 Author: Tim Gromeyer
 Author-email: sakul8826@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: COPYING
+Provides-Extra: test
+Requires-Dist: pytest>=6.0; extra == "test"
 
 # pyhtml2md
 
 pyhtml2md provides a way to use the html2md C++ library in Python. html2md is a fast and reliable library for converting HTML content into markdown.
 
 <div class="hidable-toc">
```

### Comparing `pyhtml2md-1.5.3/README.md` & `pyhtml2md-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/include/html2md.h` & `pyhtml2md-1.5.4/include/html2md.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/pyhtml2md.egg-info/PKG-INFO` & `pyhtml2md-1.5.4/pyhtml2md.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyhtml2md
-Version: 1.5.3
+Version: 1.5.4
 Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
 Home-page: https://github.com/tim-gromeyer/html2md
 Author: Tim Gromeyer
 Author-email: sakul8826@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: COPYING
+Provides-Extra: test
+Requires-Dist: pytest>=6.0; extra == "test"
 
 # pyhtml2md
 
 pyhtml2md provides a way to use the html2md C++ library in Python. html2md is a fast and reliable library for converting HTML content into markdown.
 
 <div class="hidable-toc">
```

### Comparing `pyhtml2md-1.5.3/pyhtml2md.egg-info/SOURCES.txt` & `pyhtml2md-1.5.4/pyhtml2md.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 python/pybind11/include/pybind11/common.h
 python/pybind11/include/pybind11/complex.h
 python/pybind11/include/pybind11/eigen.h
 python/pybind11/include/pybind11/embed.h
 python/pybind11/include/pybind11/eval.h
 python/pybind11/include/pybind11/functional.h
 python/pybind11/include/pybind11/gil.h
+python/pybind11/include/pybind11/gil_safe_call_once.h
 python/pybind11/include/pybind11/iostream.h
 python/pybind11/include/pybind11/numpy.h
 python/pybind11/include/pybind11/operators.h
 python/pybind11/include/pybind11/options.h
 python/pybind11/include/pybind11/pybind11.h
 python/pybind11/include/pybind11/pytypes.h
 python/pybind11/include/pybind11/stl.h
 python/pybind11/include/pybind11/stl_bind.h
 python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+python/pybind11/include/pybind11/typing.h
 python/pybind11/include/pybind11/detail/class.h
 python/pybind11/include/pybind11/detail/common.h
 python/pybind11/include/pybind11/detail/descr.h
 python/pybind11/include/pybind11/detail/init.h
 python/pybind11/include/pybind11/detail/internals.h
 python/pybind11/include/pybind11/detail/type_caster_base.h
 python/pybind11/include/pybind11/detail/typeid.h
```

### Comparing `pyhtml2md-1.5.3/pyproject.toml` & `pyhtml2md-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/README.md` & `pyhtml2md-1.5.4/python/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/bindings.cpp` & `pyhtml2md-1.5.4/python/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/CMakeLists.txt` & `pyhtml2md-1.5.4/python/pybind11/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # CMakeLists.txt -- Build system for the pybind11 modules
 #
 # Copyright (c) 2015 Wenzel Jakob <wenzel@inf.ethz.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
-cmake_minimum_required(VERSION 3.4)
+# Propagate this policy (FindPythonInterp removal) so it can be detected later
+if(NOT CMAKE_VERSION VERSION_LESS "3.27")
+  cmake_policy(GET CMP0148 _pybind11_cmp0148)
+endif()
+
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.22)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.29)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.22)
+if(${CMAKE_VERSION} VERSION_LESS 3.29)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.22)
+  cmake_policy(VERSION 3.29)
+endif()
+
+if(_pybind11_cmp0148)
+  cmake_policy(SET CMP0148 ${_pybind11_cmp0148})
+  unset(_pybind11_cmp0148)
 endif()
 
 # Avoid infinite recursion if tests include this as a subdirectory
 if(DEFINED PYBIND11_MASTER_PROJECT)
   return()
 endif()
 
@@ -78,41 +88,66 @@
     set(CMAKE_CXX_EXTENSIONS OFF)
     set(CMAKE_CXX_STANDARD_REQUIRED ON)
   endif()
 
   set(pybind11_system "")
 
   set_property(GLOBAL PROPERTY USE_FOLDERS ON)
+  if(CMAKE_VERSION VERSION_LESS "3.18")
+    set(_pybind11_findpython_default OFF)
+  else()
+    set(_pybind11_findpython_default ON)
+  endif()
 else()
   set(PYBIND11_MASTER_PROJECT OFF)
   set(pybind11_system SYSTEM)
+  set(_pybind11_findpython_default OFF)
 endif()
 
 # Options
 option(PYBIND11_INSTALL "Install pybind11 header files?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_TEST "Build pybind11 test suite?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_NOPYTHON "Disable search for Python" OFF)
+option(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION
+       "To enforce that a handle_type_name<> specialization exists" OFF)
 option(PYBIND11_SIMPLE_GIL_MANAGEMENT
        "Use simpler GIL management logic that does not support disassociation" OFF)
+option(PYBIND11_NUMPY_1_ONLY
+       "Disable NumPy 2 support to avoid changes to previous pybind11 versions." OFF)
 set(PYBIND11_INTERNALS_VERSION
     ""
     CACHE STRING "Override the ABI version, may be used to enable the unstable ABI.")
 
+if(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION)
+  add_compile_definitions(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION)
+endif()
 if(PYBIND11_SIMPLE_GIL_MANAGEMENT)
   add_compile_definitions(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 endif()
+if(PYBIND11_NUMPY_1_ONLY)
+  add_compile_definitions(PYBIND11_NUMPY_1_ONLY)
+endif()
 
 cmake_dependent_option(
   USE_PYTHON_INCLUDE_DIR
   "Install pybind11 headers in Python include directory instead of default installation prefix"
   OFF "PYBIND11_INSTALL" OFF)
 
-cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" OFF
+cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" ${_pybind11_findpython_default}
                        "NOT CMAKE_VERSION VERSION_LESS 3.12" OFF)
 
+# Allow PYTHON_EXECUTABLE if in FINDPYTHON mode and building pybind11's tests
+# (makes transition easier while we support both modes).
+if(PYBIND11_MASTER_PROJECT
+   AND PYBIND11_FINDPYTHON
+   AND DEFINED PYTHON_EXECUTABLE
+   AND NOT DEFINED Python_EXECUTABLE)
+  set(Python_EXECUTABLE "${PYTHON_EXECUTABLE}")
+endif()
+
 # NB: when adding a header don't forget to also add it to setup.py
 set(PYBIND11_HEADERS
     include/pybind11/detail/class.h
     include/pybind11/detail/common.h
     include/pybind11/detail/descr.h
     include/pybind11/detail/init.h
     include/pybind11/detail/internals.h
@@ -128,24 +163,26 @@
     include/pybind11/eigen.h
     include/pybind11/eigen/common.h
     include/pybind11/eigen/matrix.h
     include/pybind11/eigen/tensor.h
     include/pybind11/embed.h
     include/pybind11/eval.h
     include/pybind11/gil.h
+    include/pybind11/gil_safe_call_once.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
     include/pybind11/stl_bind.h
     include/pybind11/stl/filesystem.h
-    include/pybind11/type_caster_pyobject_ptr.h)
+    include/pybind11/type_caster_pyobject_ptr.h
+    include/pybind11/typing.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
@@ -273,15 +310,29 @@
   install(
     EXPORT "${PYBIND11_EXPORT_NAME}"
     NAMESPACE "pybind11::"
     DESTINATION ${PYBIND11_CMAKECONFIG_INSTALL_DIR})
 
   # pkg-config support
   if(NOT prefix_for_pc_file)
-    set(prefix_for_pc_file "${CMAKE_INSTALL_PREFIX}")
+    if(IS_ABSOLUTE "${CMAKE_INSTALL_DATAROOTDIR}")
+      set(prefix_for_pc_file "${CMAKE_INSTALL_PREFIX}")
+    else()
+      set(pc_datarootdir "${CMAKE_INSTALL_DATAROOTDIR}")
+      if(CMAKE_VERSION VERSION_LESS 3.20)
+        set(prefix_for_pc_file "\${pcfiledir}/..")
+        while(pc_datarootdir)
+          get_filename_component(pc_datarootdir "${pc_datarootdir}" DIRECTORY)
+          string(APPEND prefix_for_pc_file "/..")
+        endwhile()
+      else()
+        cmake_path(RELATIVE_PATH CMAKE_INSTALL_PREFIX BASE_DIRECTORY CMAKE_INSTALL_DATAROOTDIR
+                   OUTPUT_VARIABLE prefix_for_pc_file)
+      endif()
+    endif()
   endif()
   join_paths(includedir_for_pc_file "\${prefix}" "${CMAKE_INSTALL_INCLUDEDIR}")
   configure_file("${CMAKE_CURRENT_SOURCE_DIR}/tools/pybind11.pc.in"
                  "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc" @ONLY)
   install(FILES "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc"
           DESTINATION "${CMAKE_INSTALL_DATAROOTDIR}/pkgconfig/")
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/LICENSE` & `pyhtml2md-1.5.4/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/attr.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/buffer_info.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/buffer_info.h`

 * *Files 0% similar despite different names*

```diff
@@ -98,30 +98,30 @@
     template <typename T>
     buffer_info(T *ptr, ssize_t size, bool readonly = false)
         : buffer_info(ptr, sizeof(T), format_descriptor<T>::format(), size, readonly) {}
 
     template <typename T>
     buffer_info(const T *ptr, ssize_t size, bool readonly = true)
         : buffer_info(
-            const_cast<T *>(ptr), sizeof(T), format_descriptor<T>::format(), size, readonly) {}
+              const_cast<T *>(ptr), sizeof(T), format_descriptor<T>::format(), size, readonly) {}
 
     explicit buffer_info(Py_buffer *view, bool ownview = true)
         : buffer_info(
-            view->buf,
-            view->itemsize,
-            view->format,
-            view->ndim,
-            {view->shape, view->shape + view->ndim},
-            /* Though buffer::request() requests PyBUF_STRIDES, ctypes objects
-             * ignore this flag and return a view with NULL strides.
-             * When strides are NULL, build them manually.  */
-            view->strides
-                ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
-                : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
-            (view->readonly != 0)) {
+              view->buf,
+              view->itemsize,
+              view->format,
+              view->ndim,
+              {view->shape, view->shape + view->ndim},
+              /* Though buffer::request() requests PyBUF_STRIDES, ctypes objects
+               * ignore this flag and return a view with NULL strides.
+               * When strides are NULL, build them manually.  */
+              view->strides
+                  ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
+                  : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
+              (view->readonly != 0)) {
         // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         this->m_view = view;
         // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         this->ownview = ownview;
     }
 
     buffer_info(const buffer_info &) = delete;
@@ -172,15 +172,15 @@
                 ssize_t itemsize,
                 const std::string &format,
                 ssize_t ndim,
                 detail::any_container<ssize_t> &&shape_in,
                 detail::any_container<ssize_t> &&strides_in,
                 bool readonly)
         : buffer_info(
-            ptr, itemsize, format, ndim, std::move(shape_in), std::move(strides_in), readonly) {}
+              ptr, itemsize, format, ndim, std::move(shape_in), std::move(strides_in), readonly) {}
 
     Py_buffer *m_view = nullptr;
     bool ownview = false;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/cast.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/cast.h`

 * *Files 6% similar despite different names*

```diff
@@ -38,21 +38,23 @@
 class type_caster : public type_caster_base<type> {};
 template <typename type>
 using make_caster = type_caster<intrinsic_t<type>>;
 
 // Shortcut for calling a caster's `cast_op_type` cast operator for casting a type_caster to a T
 template <typename T>
 typename make_caster<T>::template cast_op_type<T> cast_op(make_caster<T> &caster) {
-    return caster.operator typename make_caster<T>::template cast_op_type<T>();
+    using result_t = typename make_caster<T>::template cast_op_type<T>; // See PR #4893
+    return caster.operator result_t();
 }
 template <typename T>
 typename make_caster<T>::template cast_op_type<typename std::add_rvalue_reference<T>::type>
 cast_op(make_caster<T> &&caster) {
-    return std::move(caster).operator typename make_caster<T>::
-        template cast_op_type<typename std::add_rvalue_reference<T>::type>();
+    using result_t = typename make_caster<T>::template cast_op_type<
+        typename std::add_rvalue_reference<T>::type>; // See PR #4893
+    return std::move(caster).operator result_t();
 }
 
 template <typename type>
 class type_caster<std::reference_wrapper<type>> {
 private:
     using caster_t = make_caster<type>;
     caster_t subcaster;
@@ -321,16 +323,17 @@
             value = true;
             return true;
         }
         if (src.ptr() == Py_False) {
             value = false;
             return true;
         }
-        if (convert || (std::strcmp("numpy.bool_", Py_TYPE(src.ptr())->tp_name) == 0)) {
-            // (allow non-implicit conversion for numpy booleans)
+        if (convert || is_numpy_bool(src)) {
+            // (allow non-implicit conversion for numpy booleans), use strncmp
+            // since NumPy 1.x had an additional trailing underscore.
 
             Py_ssize_t res = -1;
             if (src.is_none()) {
                 res = 0; // None is implicitly converted to False
             }
 #if defined(PYPY_VERSION)
             // On PyPy, check that "__bool__" attr exists
@@ -354,14 +357,23 @@
         }
         return false;
     }
     static handle cast(bool src, return_value_policy /* policy */, handle /* parent */) {
         return handle(src ? Py_True : Py_False).inc_ref();
     }
     PYBIND11_TYPE_CASTER(bool, const_name("bool"));
+
+private:
+    // Test if an object is a NumPy boolean (without fetching the type).
+    static inline bool is_numpy_bool(handle object) {
+        const char *type_name = Py_TYPE(object.ptr())->tp_name;
+        // Name changed to `numpy.bool` in NumPy 2, `numpy.bool_` is needed for 1.x support
+        return std::strcmp("numpy.bool", type_name) == 0
+               || std::strcmp("numpy.bool_", type_name) == 0;
+    }
 };
 
 // Helper class for UTF-{8,16,32} C++ stl strings:
 template <typename StringType, bool IsView = false>
 struct string_caster {
     using CharT = typename StringType::value_type;
 
@@ -656,16 +668,17 @@
             auto h = cast(std::move(*src), policy, parent);
             delete src;
             return h;
         }
         return cast(*src, policy, parent);
     }
 
-    static constexpr auto name
-        = const_name("Tuple[") + concat(make_caster<Ts>::name...) + const_name("]");
+    static constexpr auto name = const_name("tuple[")
+                                 + ::pybind11::detail::concat(make_caster<Ts>::name...)
+                                 + const_name("]");
 
     template <typename T>
     using cast_op_type = type;
 
     explicit operator type() & { return implicit_cast(indices{}); }
     explicit operator type() && { return std::move(*this).implicit_cast(indices{}); }
 
@@ -865,27 +878,74 @@
 template <typename base, typename holder>
 struct is_holder_type
     : std::is_base_of<detail::type_caster_holder<base, holder>, detail::type_caster<holder>> {};
 // Specialization for always-supported unique_ptr holders:
 template <typename base, typename deleter>
 struct is_holder_type<base, std::unique_ptr<base, deleter>> : std::true_type {};
 
+#ifdef PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION // See PR #4888
+
+// This leads to compilation errors if a specialization is missing.
+template <typename T>
+struct handle_type_name;
+
+#else
+
 template <typename T>
 struct handle_type_name {
     static constexpr auto name = const_name<T>();
 };
+
+#endif
+
+template <>
+struct handle_type_name<object> {
+    static constexpr auto name = const_name("object");
+};
+template <>
+struct handle_type_name<list> {
+    static constexpr auto name = const_name("list");
+};
+template <>
+struct handle_type_name<dict> {
+    static constexpr auto name = const_name("dict");
+};
+template <>
+struct handle_type_name<anyset> {
+    static constexpr auto name = const_name("Union[set, frozenset]");
+};
+template <>
+struct handle_type_name<set> {
+    static constexpr auto name = const_name("set");
+};
+template <>
+struct handle_type_name<frozenset> {
+    static constexpr auto name = const_name("frozenset");
+};
+template <>
+struct handle_type_name<str> {
+    static constexpr auto name = const_name("str");
+};
+template <>
+struct handle_type_name<tuple> {
+    static constexpr auto name = const_name("tuple");
+};
 template <>
 struct handle_type_name<bool_> {
     static constexpr auto name = const_name("bool");
 };
 template <>
 struct handle_type_name<bytes> {
     static constexpr auto name = const_name(PYBIND11_BYTES_NAME);
 };
 template <>
+struct handle_type_name<buffer> {
+    static constexpr auto name = const_name("Buffer");
+};
+template <>
 struct handle_type_name<int_> {
     static constexpr auto name = const_name("int");
 };
 template <>
 struct handle_type_name<iterable> {
     static constexpr auto name = const_name("Iterable");
 };
@@ -894,25 +954,89 @@
     static constexpr auto name = const_name("Iterator");
 };
 template <>
 struct handle_type_name<float_> {
     static constexpr auto name = const_name("float");
 };
 template <>
+struct handle_type_name<function> {
+    static constexpr auto name = const_name("Callable");
+};
+template <>
+struct handle_type_name<handle> {
+    static constexpr auto name = handle_type_name<object>::name;
+};
+template <>
 struct handle_type_name<none> {
     static constexpr auto name = const_name("None");
 };
 template <>
+struct handle_type_name<sequence> {
+    static constexpr auto name = const_name("Sequence");
+};
+template <>
+struct handle_type_name<bytearray> {
+    static constexpr auto name = const_name("bytearray");
+};
+template <>
+struct handle_type_name<memoryview> {
+    static constexpr auto name = const_name("memoryview");
+};
+template <>
+struct handle_type_name<slice> {
+    static constexpr auto name = const_name("slice");
+};
+template <>
+struct handle_type_name<type> {
+    static constexpr auto name = const_name("type");
+};
+template <>
+struct handle_type_name<capsule> {
+    static constexpr auto name = const_name("capsule");
+};
+template <>
+struct handle_type_name<ellipsis> {
+    static constexpr auto name = const_name("ellipsis");
+};
+template <>
+struct handle_type_name<weakref> {
+    static constexpr auto name = const_name("weakref");
+};
+template <>
 struct handle_type_name<args> {
     static constexpr auto name = const_name("*args");
 };
 template <>
 struct handle_type_name<kwargs> {
     static constexpr auto name = const_name("**kwargs");
 };
+template <>
+struct handle_type_name<obj_attr_accessor> {
+    static constexpr auto name = const_name<obj_attr_accessor>();
+};
+template <>
+struct handle_type_name<str_attr_accessor> {
+    static constexpr auto name = const_name<str_attr_accessor>();
+};
+template <>
+struct handle_type_name<item_accessor> {
+    static constexpr auto name = const_name<item_accessor>();
+};
+template <>
+struct handle_type_name<sequence_accessor> {
+    static constexpr auto name = const_name<sequence_accessor>();
+};
+template <>
+struct handle_type_name<list_accessor> {
+    static constexpr auto name = const_name<list_accessor>();
+};
+template <>
+struct handle_type_name<tuple_accessor> {
+    static constexpr auto name = const_name<tuple_accessor>();
+};
 
 template <typename type>
 struct pyobject_caster {
     template <typename T = type, enable_if_t<std::is_same<T, handle>::value, int> = 0>
     pyobject_caster() : value() {}
 
     // `type` may not be default constructible (e.g. frozenset, anyset).  Initializing `value`
@@ -1373,15 +1497,23 @@
 template <typename /*unused*/>
 using arg_t = arg_v;
 
 inline namespace literals {
 /** \rst
     String literal version of `arg`
  \endrst */
-constexpr arg operator"" _a(const char *name, size_t) { return arg(name); }
+constexpr arg
+#if !defined(__clang__) && defined(__GNUC__) && __GNUC__ < 5
+operator"" _a // gcc 4.8.5 insists on having a space (hard error).
+#else
+operator""_a // clang 17 generates a deprecation warning if there is a space.
+#endif
+    (const char *name, size_t) {
+    return arg(name);
+}
 } // namespace literals
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename T>
 using is_kw_only = std::is_same<intrinsic_t<T>, kw_only>;
 template <typename T>
@@ -1434,15 +1566,16 @@
 
     // py::args argument position; -1 if not present.
     static constexpr int args_pos = constexpr_last<argument_is_args, Args...>();
 
     static_assert(args_pos == -1 || args_pos == constexpr_first<argument_is_args, Args...>(),
                   "py::args cannot be specified more than once");
 
-    static constexpr auto arg_names = concat(type_descr(make_caster<Args>::name)...);
+    static constexpr auto arg_names
+        = ::pybind11::detail::concat(type_descr(make_caster<Args>::name)...);
 
     bool load_args(function_call &call) { return load_impl_sequence(call, indices{}); }
 
     template <typename Return, typename Guard, typename Func>
     // NOLINTNEXTLINE(readability-const-return-type)
     enable_if_t<!std::is_void<Return>::value, Return> call(Func &&f) && {
         return std::move(*this).template call_impl<remove_cv_t<Return>>(
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/chrono.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/complex.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/class.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/class.h`

 * *Files 1% similar despite different names*

```diff
@@ -82,25 +82,24 @@
     auto *type = &heap_type->ht_type;
     type->tp_name = name;
     type->tp_base = type_incref(&PyProperty_Type);
     type->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
     type->tp_descr_get = pybind11_static_get;
     type->tp_descr_set = pybind11_static_set;
 
-    if (PyType_Ready(type) < 0) {
-        pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
-    }
-
 #    if PY_VERSION_HEX >= 0x030C0000
-    // PRE 3.12 FEATURE FREEZE. PLEASE REVIEW AFTER FREEZE.
     // Since Python-3.12 property-derived types are required to
     // have dynamic attributes (to set `__doc__`)
     enable_dynamic_attributes(heap_type);
 #    endif
 
+    if (PyType_Ready(type) < 0) {
+        pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
+    }
+
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     return type;
 }
 
 #else // PYPY
@@ -185,20 +184,18 @@
 
     // use the default metaclass call to create/initialize the object
     PyObject *self = PyType_Type.tp_call(type, args, kwargs);
     if (self == nullptr) {
         return nullptr;
     }
 
-    // This must be a pybind11 instance
-    auto *instance = reinterpret_cast<detail::instance *>(self);
-
     // Ensure that the base __init__ function(s) were called
-    for (const auto &vh : values_and_holders(instance)) {
-        if (!vh.holder_constructed()) {
+    values_and_holders vhs(self);
+    for (const auto &vh : vhs) {
+        if (!vh.holder_constructed() && !vhs.is_redundant_value_and_holder(vh)) {
             PyErr_Format(PyExc_TypeError,
                          "%.200s.__init__() must be called when overriding __init__",
                          get_fully_qualified_tp_name(vh.type->type).c_str());
             Py_DECREF(self);
             return nullptr;
         }
     }
@@ -371,15 +368,15 @@
 
 /// An `__init__` function constructs the C++ object. Users should provide at least one
 /// of these using `py::init` or directly with `.def(__init__, ...)`. Otherwise, the
 /// following default function will be used which simply throws an exception.
 extern "C" inline int pybind11_object_init(PyObject *self, PyObject *, PyObject *) {
     PyTypeObject *type = Py_TYPE(self);
     std::string msg = get_fully_qualified_tp_name(type) + ": No constructor defined!";
-    PyErr_SetString(PyExc_TypeError, msg.c_str());
+    set_error(PyExc_TypeError, msg.c_str());
     return -1;
 }
 
 inline void add_patient(PyObject *nurse, PyObject *patient) {
     auto &internals = get_internals();
     auto *instance = reinterpret_cast<detail::instance *>(nurse);
     instance->has_patients = true;
@@ -518,27 +515,35 @@
 
     assert(!PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
     return (PyObject *) heap_type;
 }
 
 /// dynamic_attr: Allow the garbage collector to traverse the internal instance `__dict__`.
 extern "C" inline int pybind11_traverse(PyObject *self, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030D0000
+    PyObject_VisitManagedDict(self, visit, arg);
+#else
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_VISIT(dict);
+#endif
 // https://docs.python.org/3/c-api/typeobj.html#c.PyTypeObject.tp_traverse
 #if PY_VERSION_HEX >= 0x03090000
     Py_VISIT(Py_TYPE(self));
 #endif
     return 0;
 }
 
 /// dynamic_attr: Allow the GC to clear the dictionary.
 extern "C" inline int pybind11_clear(PyObject *self) {
+#if PY_VERSION_HEX >= 0x030D0000
+    PyObject_ClearManagedDict(self);
+#else
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_CLEAR(dict);
+#endif
     return 0;
 }
 
 /// Give instances of this type a `__dict__` and opt into garbage collection.
 inline void enable_dynamic_attributes(PyHeapTypeObject *heap_type) {
     auto *type = &heap_type->ht_type;
     type->tp_flags |= Py_TPFLAGS_HAVE_GC;
@@ -575,23 +580,23 @@
             break;
         }
     }
     if (view == nullptr || !tinfo || !tinfo->get_buffer) {
         if (view) {
             view->obj = nullptr;
         }
-        PyErr_SetString(PyExc_BufferError, "pybind11_getbuffer(): Internal error");
+        set_error(PyExc_BufferError, "pybind11_getbuffer(): Internal error");
         return -1;
     }
     std::memset(view, 0, sizeof(Py_buffer));
     buffer_info *info = tinfo->get_buffer(obj, tinfo->get_buffer_data);
     if ((flags & PyBUF_WRITABLE) == PyBUF_WRITABLE && info->readonly) {
         delete info;
         // view->obj = nullptr;  // Was just memset to 0, so not necessary
-        PyErr_SetString(PyExc_BufferError, "Writable buffer requested for readonly storage");
+        set_error(PyExc_BufferError, "Writable buffer requested for readonly storage");
         return -1;
     }
     view->obj = obj;
     view->ndim = 1;
     view->internal = info;
     view->buf = info->ptr;
     view->itemsize = info->itemsize;
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/common.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 11
+#define PYBIND11_VERSION_MINOR 13
 #define PYBIND11_VERSION_PATCH 0.dev1
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020B00D1
+#define PYBIND11_VERSION_HEX 0x020D00D1
 
 // Define some generic pybind11 helper macros for warning management.
 //
 // Note that compiler-specific push/pop pairs are baked into the
 // PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
 // PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
 //
@@ -114,14 +114,22 @@
 #            if _MSVC_LANG >= 202002L
 #                define PYBIND11_CPP20
 #            endif
 #        endif
 #    endif
 #endif
 
+#if defined(PYBIND11_CPP20)
+#    define PYBIND11_CONSTINIT constinit
+#    define PYBIND11_DTOR_CONSTEXPR constexpr
+#else
+#    define PYBIND11_CONSTINIT
+#    define PYBIND11_DTOR_CONSTEXPR
+#endif
+
 // Compiler version assertions
 #if defined(__INTEL_COMPILER)
 #    if __INTEL_COMPILER < 1800
 #        error pybind11 requires Intel C++ compiler v18 or newer
 #    elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
 #        error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
 #    endif
@@ -284,14 +292,18 @@
 #    undef toupper
 #endif
 
 #if defined(copysign)
 #    undef copysign
 #endif
 
+#if defined(PYBIND11_NUMPY_1_ONLY)
+#    define PYBIND11_INTERNAL_NUMPY_1_ONLY_DETECTED
+#endif
+
 #if defined(PYPY_VERSION) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 #    define PYBIND11_SIMPLE_GIL_MANAGEMENT
 #endif
 
 #if defined(_MSC_VER)
 #    if defined(PYBIND11_DEBUG_MARKER)
 #        define _DEBUG
@@ -320,19 +332,16 @@
 
 // Must be after including <version> or one of the other headers specified by the standard
 #if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
 #    define PYBIND11_HAS_U8STRING
 #endif
 
 // See description of PR #4246:
-#if !defined(NDEBUG) && !defined(PY_ASSERT_GIL_HELD_INCREF_DECREF)                                \
-    && !(defined(PYPY_VERSION)                                                                    \
-         && defined(_MSC_VER)) /* PyPy Windows: pytest hangs indefinitely at the end of the       \
-                                  process (see PR #4268) */                                       \
-    && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
+#if !defined(PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF) && !defined(NDEBUG)                       \
+    && !defined(PYPY_VERSION) && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
 #    define PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
 #endif
 
 // #define PYBIND11_STR_LEGACY_PERMISSIVE
 // If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
 //             (probably surprising and never documented, but this was the
 //             legacy behavior until and including v2.6.x). As a side-effect,
@@ -398,15 +407,15 @@
 
 #define PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     catch (pybind11::error_already_set & e) {                                                     \
         pybind11::raise_from(e, PyExc_ImportError, "initialization failed");                      \
         return nullptr;                                                                           \
     }                                                                                             \
     catch (const std::exception &e) {                                                             \
-        PyErr_SetString(PyExc_ImportError, e.what());                                             \
+        ::pybind11::set_error(PyExc_ImportError, e.what());                                       \
         return nullptr;                                                                           \
     }
 
 /** \rst
     ***Deprecated in favor of PYBIND11_MODULE***
 
     This macro creates the entry point that will be invoked when the Python interpreter
@@ -912,16 +921,15 @@
 // Sadly, all MSVC versions incl. 2022 need the workaround, even in C++20 mode.
 // See also: https://github.com/pybind/pybind11/pull/3741
 #if !defined(_MSC_VER)
 using is_template_base_of
     = decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T> *) nullptr));
 #else
 struct is_template_base_of
-    : decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T> *) nullptr)) {
-};
+    : decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T> *) nullptr)){};
 #endif
 
 /// Check if T is an instantiation of the template `Class`. For example:
 /// `is_instantiation<shared_ptr, T>` is true if `T == shared_ptr<U>` where U can be anything.
 template <template <typename...> class Class, typename T>
 struct is_instantiation : std::false_type {};
 template <template <typename...> class Class, typename... Us>
@@ -1095,22 +1103,22 @@
 struct overload_cast_impl {
     template <typename Return>
     constexpr auto operator()(Return (*pf)(Args...)) const noexcept -> decltype(pf) {
         return pf;
     }
 
     template <typename Return, typename Class>
-    constexpr auto operator()(Return (Class::*pmf)(Args...), std::false_type = {}) const noexcept
-        -> decltype(pmf) {
+    constexpr auto operator()(Return (Class::*pmf)(Args...),
+                              std::false_type = {}) const noexcept -> decltype(pmf) {
         return pmf;
     }
 
     template <typename Return, typename Class>
-    constexpr auto operator()(Return (Class::*pmf)(Args...) const, std::true_type) const noexcept
-        -> decltype(pmf) {
+    constexpr auto operator()(Return (Class::*pmf)(Args...) const,
+                              std::true_type) const noexcept -> decltype(pmf) {
         return pmf;
     }
 };
 PYBIND11_NAMESPACE_END(detail)
 
 // overload_cast requires variable templates: C++14
 #if defined(PYBIND11_CPP14)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/descr.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/descr.h`

 * *Files 1% similar despite different names*

```diff
@@ -152,16 +152,17 @@
 
 template <size_t N, typename... Ts, typename... Args>
 constexpr auto concat(const descr<N, Ts...> &d, const Args &...args) {
     return (d, ..., args);
 }
 #else
 template <size_t N, typename... Ts, typename... Args>
-constexpr auto concat(const descr<N, Ts...> &d, const Args &...args)
-    -> decltype(std::declval<descr<N + 2, Ts...>>() + concat(args...)) {
+constexpr auto concat(const descr<N, Ts...> &d,
+                      const Args &...args) -> decltype(std::declval<descr<N + 2, Ts...>>()
+                                                       + concat(args...)) {
     return d + const_name(", ") + concat(args...);
 }
 #endif
 
 template <size_t N, typename... Ts>
 constexpr descr<N + 2, Ts...> type_descr(const descr<N, Ts...> &descr) {
     return const_name("{") + descr + const_name("}");
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/init.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/init.h`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 // Failing fallback version of the above for a no-alias class (always returns false)
 template <typename /*Class*/>
 constexpr bool is_alias(void *) {
     return false;
 }
 
 // Constructs and returns a new object; if the given arguments don't map to a constructor, we fall
-// back to brace aggregate initiailization so that for aggregate initialization can be used with
+// back to brace aggregate initialization so that for aggregate initialization can be used with
 // py::init, e.g.  `py::init<int, int>` to initialize a `struct T { int a; int b; }`.  For
 // non-aggregate types, we need to use an ordinary T(...) constructor (invoking as `T{...}` usually
 // works, but will not do the expected thing when `T` has an `initializer_list<T>` constructor).
 template <typename Class,
           typename... Args,
           detail::enable_if_t<std::is_constructible<Class, Args...>::value, int> = 0>
 inline Class *construct_or_initialize(Args &&...args) {
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/internals.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/internals.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 /// newer ABI.
 ///
 /// WARNING: If you choose to manually increase the ABI version, note that
 /// pybind11 may not be tested as thoroughly with a non-default ABI version, and
 /// further ABI-incompatible changes may be made before the ABI is officially
 /// changed to the new version.
 #ifndef PYBIND11_INTERNALS_VERSION
-#    if PY_VERSION_HEX >= 0x030C0000
+#    if PY_VERSION_HEX >= 0x030C0000 || defined(_MSC_VER)
 // Version bump for Python 3.12+, before first 3.12 beta release.
+// Version bump for MSVC piggy-backed on PR #4779. See comments there.
 #        define PYBIND11_INTERNALS_VERSION 5
 #    else
 #        define PYBIND11_INTERNALS_VERSION 4
 #    endif
 #endif
 
 // This requirement is mainly to reduce the support burden (see PR #4570).
@@ -62,17 +63,22 @@
 // The old Python Thread Local Storage (TLS) API is deprecated in Python 3.7 in favor of the new
 // Thread Specific Storage (TSS) API.
 #if PY_VERSION_HEX >= 0x03070000
 // Avoid unnecessary allocation of `Py_tss_t`, since we cannot use
 // `Py_LIMITED_API` anyway.
 #    if PYBIND11_INTERNALS_VERSION > 4
 #        define PYBIND11_TLS_KEY_REF Py_tss_t &
-#        if defined(__GNUC__) && !defined(__INTEL_COMPILER)
-// Clang on macOS warns due to `Py_tss_NEEDS_INIT` not specifying an initializer
-// for every field.
+#        if defined(__clang__)
+#            define PYBIND11_TLS_KEY_INIT(var)                                                    \
+                _Pragma("clang diagnostic push")                                         /**/     \
+                    _Pragma("clang diagnostic ignored \"-Wmissing-field-initializers\"") /**/     \
+                    Py_tss_t var                                                                  \
+                    = Py_tss_NEEDS_INIT;                                                          \
+                _Pragma("clang diagnostic pop")
+#        elif defined(__GNUC__) && !defined(__INTEL_COMPILER)
 #            define PYBIND11_TLS_KEY_INIT(var)                                                    \
                 _Pragma("GCC diagnostic push")                                         /**/       \
                     _Pragma("GCC diagnostic ignored \"-Wmissing-field-initializers\"") /**/       \
                     Py_tss_t var                                                                  \
                     = Py_tss_NEEDS_INIT;                                                          \
                 _Pragma("GCC diagnostic pop")
 #        else
@@ -287,17 +293,20 @@
 #        define PYBIND11_STDLIB "_libstdcpp"
 #    else
 #        define PYBIND11_STDLIB ""
 #    endif
 #endif
 
 /// On Linux/OSX, changes in __GXX_ABI_VERSION__ indicate ABI incompatibility.
+/// On MSVC, changes in _MSC_VER may indicate ABI incompatibility (#2898).
 #ifndef PYBIND11_BUILD_ABI
 #    if defined(__GXX_ABI_VERSION)
 #        define PYBIND11_BUILD_ABI "_cxxabi" PYBIND11_TOSTRING(__GXX_ABI_VERSION)
+#    elif defined(_MSC_VER)
+#        define PYBIND11_BUILD_ABI "_mscver" PYBIND11_TOSTRING(_MSC_VER)
 #    else
 #        define PYBIND11_BUILD_ABI ""
 #    endif
 #endif
 
 #ifndef PYBIND11_INTERNALS_KIND
 #    if defined(WITH_THREAD)
@@ -305,21 +314,21 @@
 #    else
 #        define PYBIND11_INTERNALS_KIND "_without_thread"
 #    endif
 #endif
 
 #define PYBIND11_INTERNALS_ID                                                                     \
     "__pybind11_internals_v" PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION)                        \
-        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI         \
-            PYBIND11_BUILD_TYPE "__"
+        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB                            \
+            PYBIND11_BUILD_ABI PYBIND11_BUILD_TYPE "__"
 
 #define PYBIND11_MODULE_LOCAL_ID                                                                  \
     "__pybind11_module_local_v" PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION)                     \
-        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI         \
-            PYBIND11_BUILD_TYPE "__"
+        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB                            \
+            PYBIND11_BUILD_ABI PYBIND11_BUILD_TYPE "__"
 
 /// Each module locally stores a pointer to the `internals` data. The data
 /// itself is shared among modules with the same `PYBIND11_INTERNALS_ID`.
 inline internals **&get_internals_pp() {
     static internals **internals_pp = nullptr;
     return internals_pp;
 }
@@ -348,15 +357,15 @@
 }
 
 inline bool raise_err(PyObject *exc_type, const char *msg) {
     if (PyErr_Occurred()) {
         raise_from(exc_type, msg);
         return true;
     }
-    PyErr_SetString(exc_type, msg);
+    set_error(exc_type, msg);
     return false;
 }
 
 inline void translate_exception(std::exception_ptr p) {
     if (!p) {
         return;
     }
@@ -443,26 +452,28 @@
 #    endif
     if (istate) {
         state_dict = reinterpret_borrow<object>(PyInterpreterState_GetDict(istate));
     }
 #endif
     if (!state_dict) {
         raise_from(PyExc_SystemError, "pybind11::detail::get_python_state_dict() FAILED");
+        throw error_already_set();
     }
     return state_dict;
 }
 
 inline object get_internals_obj_from_state_dict(handle state_dict) {
     return reinterpret_borrow<object>(dict_getitemstring(state_dict.ptr(), PYBIND11_INTERNALS_ID));
 }
 
 inline internals **get_internals_pp_from_capsule(handle obj) {
     void *raw_ptr = PyCapsule_GetPointer(obj.ptr(), /*name=*/nullptr);
     if (raw_ptr == nullptr) {
         raise_from(PyExc_SystemError, "pybind11::detail::get_internals_pp_from_capsule() FAILED");
+        throw error_already_set();
     }
     return static_cast<internals **>(raw_ptr);
 }
 
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/type_caster_base.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,30 @@
 
 // Gets the cache entry for the given type, creating it if necessary.  The return value is the pair
 // returned by emplace, i.e. an iterator for the entry and a bool set to `true` if the entry was
 // just created.
 inline std::pair<decltype(internals::registered_types_py)::iterator, bool>
 all_type_info_get_cache(PyTypeObject *type);
 
+// Band-aid workaround to fix a subtle but serious bug in a minimalistic fashion. See PR #4762.
+inline void all_type_info_add_base_most_derived_first(std::vector<type_info *> &bases,
+                                                      type_info *addl_base) {
+    for (auto it = bases.begin(); it != bases.end(); it++) {
+        type_info *existing_base = *it;
+        if (PyType_IsSubtype(addl_base->type, existing_base->type) != 0) {
+            bases.insert(it, addl_base);
+            return;
+        }
+    }
+    bases.push_back(addl_base);
+}
+
 // Populates a just-created cache entry.
 PYBIND11_NOINLINE void all_type_info_populate(PyTypeObject *t, std::vector<type_info *> &bases) {
+    assert(bases.empty());
     std::vector<PyTypeObject *> check;
     for (handle parent : reinterpret_borrow<tuple>(t->tp_bases)) {
         check.push_back((PyTypeObject *) parent.ptr());
     }
 
     auto const &type_dict = get_internals().registered_types_py;
     for (size_t i = 0; i < check.size(); i++) {
@@ -132,15 +146,15 @@
                 for (auto *known : bases) {
                     if (known == tinfo) {
                         found = true;
                         break;
                     }
                 }
                 if (!found) {
-                    bases.push_back(tinfo);
+                    all_type_info_add_base_most_derived_first(bases, tinfo);
                 }
             }
         } else if (type->tp_bases) {
             // It's some python type, so keep follow its bases classes to look for one or more
             // registered types
             if (i + 1 == check.size()) {
                 // When we're at the end, we can pop off the current element to avoid growing
@@ -318,26 +332,37 @@
     using type_vec = std::vector<detail::type_info *>;
     const type_vec &tinfo;
 
 public:
     explicit values_and_holders(instance *inst)
         : inst{inst}, tinfo(all_type_info(Py_TYPE(inst))) {}
 
+    explicit values_and_holders(PyObject *obj)
+        : inst{nullptr}, tinfo(all_type_info(Py_TYPE(obj))) {
+        if (!tinfo.empty()) {
+            inst = reinterpret_cast<instance *>(obj);
+        }
+    }
+
     struct iterator {
     private:
         instance *inst = nullptr;
         const type_vec *types = nullptr;
         value_and_holder curr;
         friend struct values_and_holders;
-        iterator(instance *inst, const type_vec *tinfo)
-            : inst{inst}, types{tinfo},
-              curr(inst /* instance */,
-                   types->empty() ? nullptr : (*types)[0] /* type info */,
-                   0, /* vpos: (non-simple types only): the first vptr comes first */
-                   0 /* index */) {}
+        iterator(instance *inst, const type_vec *tinfo) : inst{inst}, types{tinfo} {
+            if (inst != nullptr) {
+                assert(!types->empty());
+                curr = value_and_holder(
+                    inst /* instance */,
+                    (*types)[0] /* type info */,
+                    0, /* vpos: (non-simple types only): the first vptr comes first */
+                    0 /* index */);
+            }
+        }
         // Past-the-end iterator:
         explicit iterator(size_t end) : curr(end) {}
 
     public:
         bool operator==(const iterator &other) const { return curr.index == other.curr.index; }
         bool operator!=(const iterator &other) const { return curr.index != other.curr.index; }
         iterator &operator++() {
@@ -360,14 +385,24 @@
         while (it != endit && it->type != find_type) {
             ++it;
         }
         return it;
     }
 
     size_t size() { return tinfo.size(); }
+
+    // Band-aid workaround to fix a subtle but serious bug in a minimalistic fashion. See PR #4762.
+    bool is_redundant_value_and_holder(const value_and_holder &vh) {
+        for (size_t i = 0; i < vh.index; i++) {
+            if (PyType_IsSubtype(tinfo[i]->type, tinfo[vh.index]->type) != 0) {
+                return true;
+            }
+        }
+        return false;
+    }
 };
 
 /**
  * Extracts C++ value and holder pointer references from an instance (which may contain multiple
  * values/holders for python-side multiple inheritance) that match the given type.  Throws an error
  * if the given type (or ValueType, if omitted) is not a pybind11 base of the given instance.  If
  * `find_type` is omitted (or explicitly specified as nullptr) the first value/holder are returned,
@@ -482,16 +517,18 @@
     }
     return handle();
 }
 
 inline PyThreadState *get_thread_state_unchecked() {
 #if defined(PYPY_VERSION)
     return PyThreadState_GET();
-#else
+#elif PY_VERSION_HEX < 0x030D0000
     return _PyThreadState_UncheckedGet();
+#else
+    return PyThreadState_GetUnchecked();
 #endif
 }
 
 // Forward declarations
 void keep_alive_impl(handle nurse, handle patient);
 inline PyObject *make_new_instance(PyTypeObject *type);
 
@@ -782,15 +819,15 @@
             return {src, const_cast<const type_info *>(tpi)};
         }
 
         // Not found, set error:
         std::string tname = rtti_type ? rtti_type->name() : cast_type.name();
         detail::clean_type_id(tname);
         std::string msg = "Unregistered type : " + tname;
-        PyErr_SetString(PyExc_TypeError, msg.c_str());
+        set_error(PyExc_TypeError, msg.c_str());
         return {nullptr, nullptr};
     }
 
     const type_info *typeinfo = nullptr;
     const std::type_info *cpptype = nullptr;
     void *value = nullptr;
 };
@@ -1143,35 +1180,39 @@
 protected:
     using Constructor = void *(*) (const void *);
 
     /* Only enabled when the types are {copy,move}-constructible *and* when the type
        does not have a private operator new implementation. A comma operator is used in the
        decltype argument to apply SFINAE to the public copy/move constructors.*/
     template <typename T, typename = enable_if_t<is_copy_constructible<T>::value>>
-    static auto make_copy_constructor(const T *)
-        -> decltype(new T(std::declval<const T>()), Constructor{}) {
+    static auto make_copy_constructor(const T *) -> decltype(new T(std::declval<const T>()),
+                                                             Constructor{}) {
         return [](const void *arg) -> void * { return new T(*reinterpret_cast<const T *>(arg)); };
     }
 
     template <typename T, typename = enable_if_t<is_move_constructible<T>::value>>
-    static auto make_move_constructor(const T *)
-        -> decltype(new T(std::declval<T &&>()), Constructor{}) {
+    static auto make_move_constructor(const T *) -> decltype(new T(std::declval<T &&>()),
+                                                             Constructor{}) {
         return [](const void *arg) -> void * {
             return new T(std::move(*const_cast<T *>(reinterpret_cast<const T *>(arg))));
         };
     }
 
     static Constructor make_copy_constructor(...) { return nullptr; }
     static Constructor make_move_constructor(...) { return nullptr; }
 };
 
+inline std::string quote_cpp_type_name(const std::string &cpp_type_name) {
+    return cpp_type_name; // No-op for now. See PR #4888
+}
+
 PYBIND11_NOINLINE std::string type_info_description(const std::type_info &ti) {
     if (auto *type_data = get_type_info(ti)) {
         handle th((PyObject *) type_data->type);
         return th.attr("__module__").cast<std::string>() + '.'
                + th.attr("__qualname__").cast<std::string>();
     }
-    return clean_type_id(ti.name());
+    return quote_cpp_type_name(clean_type_id(ti.name()));
 }
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/detail/typeid.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/matrix.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/eigen/tensor.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/tensor.h`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     }
 
     template <typename T>
     struct helper {};
 
     template <size_t... Is>
     struct helper<index_sequence<Is...>> {
-        static constexpr auto value = concat(const_name(((void) Is, "?"))...);
+        static constexpr auto value = ::pybind11::detail::concat(const_name(((void) Is, "?"))...);
     };
 
     static constexpr auto dimensions_descriptor
         = helper<decltype(make_index_sequence<Type::NumIndices>())>::value;
 
     template <typename... Args>
     static Type *alloc(Args &&...args) {
@@ -100,15 +100,16 @@
     }
 
     static bool
     is_correct_shape(const Eigen::DSizes<typename Type::Index, Type::NumIndices> &shape) {
         return get_shape() == shape;
     }
 
-    static constexpr auto dimensions_descriptor = concat(const_name<Indices>()...);
+    static constexpr auto dimensions_descriptor
+        = ::pybind11::detail::concat(const_name<Indices>()...);
 
     template <typename... Args>
     static Type *alloc(Args &&...args) {
         Eigen::aligned_allocator<Type> allocator;
         return ::new (allocator.allocate(1)) Type(std::forward<Args>(args)...);
     }
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/embed.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/eval.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/functional.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/functional.h`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         if (result) {
             return cpp_function(*result, policy).release();
         }
         return cpp_function(std::forward<Func>(f_), policy).release();
     }
 
     PYBIND11_TYPE_CASTER(type,
-                         const_name("Callable[[") + concat(make_caster<Args>::name...)
+                         const_name("Callable[[")
+                             + ::pybind11::detail::concat(make_caster<Args>::name...)
                              + const_name("], ") + make_caster<retval_type>::name
                              + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/gil.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil.h`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
 
+#include <cassert>
+
 #if defined(WITH_THREAD) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 #    include "detail/internals.h"
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
@@ -133,15 +135,17 @@
     PyThreadState *tstate = nullptr;
     bool release = true;
     bool active = true;
 };
 
 class gil_scoped_release {
 public:
+    // PRECONDITION: The GIL must be held when this constructor is called.
     explicit gil_scoped_release(bool disassoc = false) : disassoc(disassoc) {
+        assert(PyGILState_Check());
         // `get_internals()` must be called here unconditionally in order to initialize
         // `internals.tstate` for subsequent `gil_scoped_acquire` calls. Otherwise, an
         // initialization race could occur as multiple threads try `gil_scoped_acquire`.
         auto &internals = detail::get_internals();
         // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         tstate = PyEval_SaveThread();
         if (disassoc) {
@@ -197,15 +201,19 @@
     void disarm() {}
 };
 
 class gil_scoped_release {
     PyThreadState *state;
 
 public:
-    gil_scoped_release() : state{PyEval_SaveThread()} {}
+    // PRECONDITION: The GIL must be held when this constructor is called.
+    gil_scoped_release() {
+        assert(PyGILState_Check());
+        state = PyEval_SaveThread();
+    }
     gil_scoped_release(const gil_scoped_release &) = delete;
     gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
 
 #    endif // PYBIND11_SIMPLE_GIL_MANAGEMENT
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/iostream.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/numpy.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/numpy.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+#include "detail/common.h"
 #include "complex.h"
+#include "gil_safe_call_once.h"
+#include "pytypes.h"
 
 #include <algorithm>
 #include <array>
 #include <cstdint>
 #include <cstdlib>
 #include <cstring>
 #include <functional>
@@ -22,53 +25,102 @@
 #include <sstream>
 #include <string>
 #include <type_traits>
 #include <typeindex>
 #include <utility>
 #include <vector>
 
+#if defined(PYBIND11_NUMPY_1_ONLY) && !defined(PYBIND11_INTERNAL_NUMPY_1_ONLY_DETECTED)
+#    error PYBIND11_NUMPY_1_ONLY must be defined before any pybind11 header is included.
+#endif
+
 /* This will be true on all flat address space platforms and allows us to reduce the
    whole npy_intp / ssize_t / Py_intptr_t business down to just ssize_t for all size
    and dimension types (e.g. shape, strides, indexing), instead of inflicting this
-   upon the library user. */
+   upon the library user.
+   Note that NumPy 2 now uses ssize_t for `npy_intp` to simplify this. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
 // We now can reinterpret_cast between py::ssize_t and Py_intptr_t (MSVC + PyPy cares)
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 PYBIND11_WARNING_DISABLE_MSVC(4127)
 
+class dtype; // Forward declaration
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
+struct handle_type_name<dtype> {
+    static constexpr auto name = const_name("numpy.dtype");
+};
+
+template <>
 struct handle_type_name<array> {
     static constexpr auto name = const_name("numpy.ndarray");
 };
 
 template <typename type, typename SFINAE = void>
 struct npy_format_descriptor;
 
-struct PyArrayDescr_Proxy {
+/* NumPy 1 proxy (always includes legacy fields) */
+struct PyArrayDescr1_Proxy {
     PyObject_HEAD
     PyObject *typeobj;
     char kind;
     char type;
     char byteorder;
     char flags;
     int type_num;
     int elsize;
     int alignment;
     char *subarray;
     PyObject *fields;
     PyObject *names;
 };
 
+#ifndef PYBIND11_NUMPY_1_ONLY
+struct PyArrayDescr_Proxy {
+    PyObject_HEAD
+    PyObject *typeobj;
+    char kind;
+    char type;
+    char byteorder;
+    char _former_flags;
+    int type_num;
+    /* Additional fields are NumPy version specific. */
+};
+#else
+/* NumPy 1.x only, we can expose all fields */
+using PyArrayDescr_Proxy = PyArrayDescr1_Proxy;
+#endif
+
+/* NumPy 2 proxy, including legacy fields */
+struct PyArrayDescr2_Proxy {
+    PyObject_HEAD
+    PyObject *typeobj;
+    char kind;
+    char type;
+    char byteorder;
+    char _former_flags;
+    int type_num;
+    std::uint64_t flags;
+    ssize_t elsize;
+    ssize_t alignment;
+    PyObject *metadata;
+    Py_hash_t hash;
+    void *reserved_null[2];
+    /* The following fields only exist if 0 <= type_num < 2056 */
+    char *subarray;
+    PyObject *fields;
+    PyObject *names;
+};
+
 struct PyArray_Proxy {
     PyObject_HEAD
     char *data;
     int nd;
     ssize_t *dimensions;
     ssize_t *strides;
     PyObject *base;
@@ -116,14 +168,36 @@
     static numpy_internals *ptr = nullptr;
     if (!ptr) {
         load_numpy_internals(ptr);
     }
     return *ptr;
 }
 
+PYBIND11_NOINLINE module_ import_numpy_core_submodule(const char *submodule_name) {
+    module_ numpy = module_::import("numpy");
+    str version_string = numpy.attr("__version__");
+
+    module_ numpy_lib = module_::import("numpy.lib");
+    object numpy_version = numpy_lib.attr("NumpyVersion")(version_string);
+    int major_version = numpy_version.attr("major").cast<int>();
+
+#ifdef PYBIND11_NUMPY_1_ONLY
+    if (major_version >= 2) {
+        throw std::runtime_error(
+            "This extension was built with PYBIND11_NUMPY_1_ONLY defined, "
+            "but NumPy 2 is used in this process. For NumPy2 compatibility, "
+            "this extension needs to be rebuilt without the PYBIND11_NUMPY_1_ONLY define.");
+    }
+#endif
+    /* `numpy.core` was renamed to `numpy._core` in NumPy 2.0 as it officially
+        became a private module. */
+    std::string numpy_core_path = major_version >= 2 ? "numpy._core" : "numpy.core";
+    return module_::import((numpy_core_path + "." + submodule_name).c_str());
+}
+
 template <typename T>
 struct same_size {
     template <typename U>
     using as = bool_constant<sizeof(T) == sizeof(U)>;
 };
 
 template <typename Concrete>
@@ -182,22 +256,24 @@
         NPY_INT64_
         = platform_lookup<std::int64_t, long, long long, int>(NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
         NPY_UINT64_
         = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
             NPY_ULONG_, NPY_ULONGLONG_, NPY_UINT_),
     };
 
+    unsigned int PyArray_RUNTIME_VERSION_;
+
     struct PyArray_Dims {
         Py_intptr_t *ptr;
         int len;
     };
 
     static npy_api &get() {
-        static npy_api api = lookup();
-        return api;
+        PYBIND11_CONSTINIT static gil_safe_call_once_and_store<npy_api> storage;
+        return storage.call_once_and_store_result(lookup).get_stored();
     }
 
     bool PyArray_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArray_Type_) != 0;
     }
     bool PyArrayDescr_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArrayDescr_Type_) != 0;
@@ -220,22 +296,24 @@
     PyTypeObject *PyArray_Type_;
     PyTypeObject *PyVoidArrType_Type_;
     PyTypeObject *PyArrayDescr_Type_;
     PyObject *(*PyArray_DescrFromScalar_)(PyObject *);
     PyObject *(*PyArray_FromAny_)(PyObject *, PyObject *, int, int, int, PyObject *);
     int (*PyArray_DescrConverter_)(PyObject *, PyObject **);
     bool (*PyArray_EquivTypes_)(PyObject *, PyObject *);
+#ifdef PYBIND11_NUMPY_1_ONLY
     int (*PyArray_GetArrayParamsFromObject_)(PyObject *,
                                              PyObject *,
                                              unsigned char,
                                              PyObject **,
                                              int *,
                                              Py_intptr_t *,
                                              PyObject **,
                                              PyObject *);
+#endif
     PyObject *(*PyArray_Squeeze_)(PyObject *);
     // Unused. Not removed because that affects ABI of the class.
     int (*PyArray_SetBaseObject_)(PyObject *, PyObject *);
     PyObject *(*PyArray_Resize_)(PyObject *, PyArray_Dims *, int, int);
     PyObject *(*PyArray_Newshape_)(PyObject *, PyArray_Dims *, int);
     PyObject *(*PyArray_View_)(PyObject *, PyObject *, PyObject *);
 
@@ -245,35 +323,43 @@
         API_PyArray_Type = 2,
         API_PyArrayDescr_Type = 3,
         API_PyVoidArrType_Type = 39,
         API_PyArray_DescrFromType = 45,
         API_PyArray_DescrFromScalar = 57,
         API_PyArray_FromAny = 69,
         API_PyArray_Resize = 80,
-        API_PyArray_CopyInto = 82,
+        // CopyInto was slot 82 and 50 was effectively an alias. NumPy 2 removed 82.
+        API_PyArray_CopyInto = 50,
         API_PyArray_NewCopy = 85,
         API_PyArray_NewFromDescr = 94,
         API_PyArray_DescrNewFromType = 96,
         API_PyArray_Newshape = 135,
         API_PyArray_Squeeze = 136,
         API_PyArray_View = 137,
         API_PyArray_DescrConverter = 174,
         API_PyArray_EquivTypes = 182,
+#ifdef PYBIND11_NUMPY_1_ONLY
         API_PyArray_GetArrayParamsFromObject = 278,
+#endif
         API_PyArray_SetBaseObject = 282
     };
 
     static npy_api lookup() {
-        module_ m = module_::import("numpy.core.multiarray");
+        module_ m = detail::import_numpy_core_submodule("multiarray");
         auto c = m.attr("_ARRAY_API");
         void **api_ptr = (void **) PyCapsule_GetPointer(c.ptr(), nullptr);
+        if (api_ptr == nullptr) {
+            raise_from(PyExc_SystemError, "FAILURE obtaining numpy _ARRAY_API pointer.");
+            throw error_already_set();
+        }
         npy_api api;
 #define DECL_NPY_API(Func) api.Func##_ = (decltype(api.Func##_)) api_ptr[API_##Func];
         DECL_NPY_API(PyArray_GetNDArrayCFeatureVersion);
-        if (api.PyArray_GetNDArrayCFeatureVersion_() < 0x7) {
+        api.PyArray_RUNTIME_VERSION_ = api.PyArray_GetNDArrayCFeatureVersion_();
+        if (api.PyArray_RUNTIME_VERSION_ < 0x7) {
             pybind11_fail("pybind11 numpy support requires numpy >= 1.7.0");
         }
         DECL_NPY_API(PyArray_Type);
         DECL_NPY_API(PyVoidArrType_Type);
         DECL_NPY_API(PyArrayDescr_Type);
         DECL_NPY_API(PyArray_DescrFromType);
         DECL_NPY_API(PyArray_DescrFromScalar);
@@ -284,15 +370,17 @@
         DECL_NPY_API(PyArray_NewFromDescr);
         DECL_NPY_API(PyArray_DescrNewFromType);
         DECL_NPY_API(PyArray_Newshape);
         DECL_NPY_API(PyArray_Squeeze);
         DECL_NPY_API(PyArray_View);
         DECL_NPY_API(PyArray_DescrConverter);
         DECL_NPY_API(PyArray_EquivTypes);
+#ifdef PYBIND11_NUMPY_1_ONLY
         DECL_NPY_API(PyArray_GetArrayParamsFromObject);
+#endif
         DECL_NPY_API(PyArray_SetBaseObject);
 
 #undef DECL_NPY_API
         return api;
     }
 };
 
@@ -306,14 +394,22 @@
     return reinterpret_cast<PyArrayDescr_Proxy *>(ptr);
 }
 
 inline const PyArrayDescr_Proxy *array_descriptor_proxy(const PyObject *ptr) {
     return reinterpret_cast<const PyArrayDescr_Proxy *>(ptr);
 }
 
+inline const PyArrayDescr1_Proxy *array_descriptor1_proxy(const PyObject *ptr) {
+    return reinterpret_cast<const PyArrayDescr1_Proxy *>(ptr);
+}
+
+inline const PyArrayDescr2_Proxy *array_descriptor2_proxy(const PyObject *ptr) {
+    return reinterpret_cast<const PyArrayDescr2_Proxy *>(ptr);
+}
+
 inline bool check_flags(const void *ptr, int flag) {
     return (flag == (array_proxy(ptr)->flags & flag));
 }
 
 template <typename T>
 struct is_std_array : std::false_type {};
 template <typename T, size_t N>
@@ -346,15 +442,15 @@
     // appends the extents to shape
     static void append_extents(list &shape) {
         shape.append(N);
         array_info<T>::append_extents(shape);
     }
 
     static constexpr auto extents = const_name<array_info<T>::is_array>(
-        concat(const_name<N>(), array_info<T>::extents), const_name<N>());
+        ::pybind11::detail::concat(const_name<N>(), array_info<T>::extents), const_name<N>());
 };
 // For numpy we have special handling for arrays of characters, so we don't include
 // the size in the array extents.
 template <size_t N>
 struct array_info<char[N]> : array_info_scalar<char[N]> {};
 template <size_t N>
 struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> {};
@@ -585,18 +681,40 @@
     /// Return dtype associated with a C++ type.
     template <typename T>
     static dtype of() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::dtype();
     }
 
     /// Size of the data type in bytes.
+#ifdef PYBIND11_NUMPY_1_ONLY
     ssize_t itemsize() const { return detail::array_descriptor_proxy(m_ptr)->elsize; }
+#else
+    ssize_t itemsize() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->elsize;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->elsize;
+    }
+#endif
 
     /// Returns true for structured data types.
+#ifdef PYBIND11_NUMPY_1_ONLY
     bool has_fields() const { return detail::array_descriptor_proxy(m_ptr)->names != nullptr; }
+#else
+    bool has_fields() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->names != nullptr;
+        }
+        const auto *proxy = detail::array_descriptor2_proxy(m_ptr);
+        if (proxy->type_num < 0 || proxy->type_num >= 2056) {
+            return false;
+        }
+        return proxy->names != nullptr;
+    }
+#endif
 
     /// Single-character code for dtype's kind.
     /// For example, floating point types are 'f' and integral types are 'i'.
     char kind() const { return detail::array_descriptor_proxy(m_ptr)->kind; }
 
     /// Single-character for dtype's type.
     /// For example, ``float`` is 'f', ``double`` 'd', ``int`` 'i', and ``long`` 'l'.
@@ -614,28 +732,47 @@
         // C API (``PyArray_Descr::type_num``).
         return detail::array_descriptor_proxy(m_ptr)->type_num;
     }
 
     /// Single character for byteorder
     char byteorder() const { return detail::array_descriptor_proxy(m_ptr)->byteorder; }
 
-    /// Alignment of the data type
+/// Alignment of the data type
+#ifdef PYBIND11_NUMPY_1_ONLY
     int alignment() const { return detail::array_descriptor_proxy(m_ptr)->alignment; }
+#else
+    ssize_t alignment() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->alignment;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->alignment;
+    }
+#endif
 
-    /// Flags for the array descriptor
+/// Flags for the array descriptor
+#ifdef PYBIND11_NUMPY_1_ONLY
     char flags() const { return detail::array_descriptor_proxy(m_ptr)->flags; }
+#else
+    std::uint64_t flags() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return (unsigned char) detail::array_descriptor1_proxy(m_ptr)->flags;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->flags;
+    }
+#endif
 
 private:
-    static object _dtype_from_pep3118() {
-        static PyObject *obj = module_::import("numpy.core._internal")
-                                   .attr("_dtype_from_pep3118")
-                                   .cast<object>()
-                                   .release()
-                                   .ptr();
-        return reinterpret_borrow<object>(obj);
+    static object &_dtype_from_pep3118() {
+        PYBIND11_CONSTINIT static gil_safe_call_once_and_store<object> storage;
+        return storage
+            .call_once_and_store_result([]() {
+                return detail::import_numpy_core_submodule("_internal")
+                    .attr("_dtype_from_pep3118");
+            })
+            .get_stored();
     }
 
     dtype strip_padding(ssize_t itemsize) {
         // Recursively strip all void fields with empty names that are generated for
         // padding fields (as of NumPy v1.11).
         if (!has_fields()) {
             return *this;
@@ -784,17 +921,15 @@
 
     /// Total number of elements
     ssize_t size() const {
         return std::accumulate(shape(), shape() + ndim(), (ssize_t) 1, std::multiplies<ssize_t>());
     }
 
     /// Byte size of a single element
-    ssize_t itemsize() const {
-        return detail::array_descriptor_proxy(detail::array_proxy(m_ptr)->descr)->elsize;
-    }
+    ssize_t itemsize() const { return dtype().itemsize(); }
 
     /// Total number of bytes
     ssize_t nbytes() const { return size() * itemsize(); }
 
     /// Number of dimensions
     ssize_t ndim() const { return detail::array_proxy(m_ptr)->nd; }
 
@@ -1004,15 +1139,15 @@
         }
         check_dimensions_impl(axis + 1, shape + 1, index...);
     }
 
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array(PyObject *ptr, int ExtraFlags = 0) {
         if (ptr == nullptr) {
-            PyErr_SetString(PyExc_ValueError, "cannot create a pybind11::array from a nullptr");
+            set_error(PyExc_ValueError, "cannot create a pybind11::array from a nullptr");
             return nullptr;
         }
         return detail::npy_api::get().PyArray_FromAny_(
             ptr, nullptr, 0, 0, detail::npy_api::NPY_ARRAY_ENSUREARRAY_ | ExtraFlags, nullptr);
     }
 };
 
@@ -1151,15 +1286,15 @@
                && detail::check_flags(h.ptr(), ExtraFlags & (array::c_style | array::f_style));
     }
 
 protected:
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array_t(PyObject *ptr) {
         if (ptr == nullptr) {
-            PyErr_SetString(PyExc_ValueError, "cannot create a pybind11::array_t from a nullptr");
+            set_error(PyExc_ValueError, "cannot create a pybind11::array_t from a nullptr");
             return nullptr;
         }
         return detail::npy_api::get().PyArray_FromAny_(ptr,
                                                        dtype::of<T>().release().ptr(),
                                                        0,
                                                        0,
                                                        detail::npy_api::NPY_ARRAY_ENSUREARRAY_
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/operators.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/options.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/pybind11.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/pybind11.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 #pragma once
 
 #include "detail/class.h"
 #include "detail/init.h"
 #include "attr.h"
 #include "gil.h"
+#include "gil_safe_call_once.h"
 #include "options.h"
+#include "typing.h"
 
 #include <cstdlib>
 #include <cstring>
 #include <memory>
 #include <new>
 #include <string>
 #include <utility>
@@ -48,14 +50,55 @@
 PYBIND11_WARNING_DISABLE_GCC("-Wnoexcept-type")
 #endif
 
 PYBIND11_WARNING_DISABLE_MSVC(4127)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
+inline std::string replace_newlines_and_squash(const char *text) {
+    const char *whitespaces = " \t\n\r\f\v";
+    std::string result(text);
+    bool previous_is_whitespace = false;
+
+    if (result.size() >= 2) {
+        // Do not modify string representations
+        char first_char = result[0];
+        char last_char = result[result.size() - 1];
+        if (first_char == last_char && first_char == '\'') {
+            return result;
+        }
+    }
+    result.clear();
+
+    // Replace characters in whitespaces array with spaces and squash consecutive spaces
+    while (*text != '\0') {
+        if (std::strchr(whitespaces, *text)) {
+            if (!previous_is_whitespace) {
+                result += ' ';
+                previous_is_whitespace = true;
+            }
+        } else {
+            result += *text;
+            previous_is_whitespace = false;
+        }
+        ++text;
+    }
+
+    // Strip leading and trailing whitespaces
+    const size_t str_begin = result.find_first_not_of(whitespaces);
+    if (str_begin == std::string::npos) {
+        return "";
+    }
+
+    const size_t str_end = result.find_last_not_of(whitespaces);
+    const size_t str_range = str_end - str_begin + 1;
+
+    return result.substr(str_begin, str_range);
+}
+
 // Apply all the extensions translators from a list
 // Return true if one of the translators completed without raising an exception
 // itself. Return of false indicates that if there are other translators
 // available, they should be tried.
 inline bool apply_exception_translators(std::forward_list<ExceptionTranslator> &translators) {
     auto last_exception = std::current_exception();
 
@@ -420,15 +463,15 @@
                     signature += "arg" + std::to_string(arg_index - (rec->is_method ? 1 : 0));
                 }
                 signature += ": ";
             } else if (c == '}') {
                 // Write default value if available.
                 if (!is_starred && arg_index < rec->args.size() && rec->args[arg_index].descr) {
                     signature += " = ";
-                    signature += rec->args[arg_index].descr;
+                    signature += detail::replace_newlines_and_squash(rec->args[arg_index].descr);
                 }
                 // Separator for positional-only arguments (placed after the
                 // argument, rather than before like *
                 if (rec->nargs_pos_only > 0 && (arg_index + 1) == rec->nargs_pos_only) {
                     signature += ", /";
                 }
                 if (!is_starred) {
@@ -445,17 +488,15 @@
                                  + th.attr("__qualname__").cast<std::string>();
                 } else if (rec->is_new_style_constructor && arg_index == 0) {
                     // A new-style `__init__` takes `self` as `value_and_holder`.
                     // Rewrite it to the proper class type.
                     signature += rec->scope.attr("__module__").cast<std::string>() + "."
                                  + rec->scope.attr("__qualname__").cast<std::string>();
                 } else {
-                    std::string tname(t->name());
-                    detail::clean_type_id(tname);
-                    signature += tname;
+                    signature += detail::quote_cpp_type_name(detail::clean_type_id(t->name()));
                 }
             } else {
                 signature += c;
             }
         }
 
         if (arg_index != args - rec->has_args - rec->has_kwargs || types[type_index] != nullptr) {
@@ -676,31 +717,30 @@
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
         assert(isinstance<capsule>(self));
 
         /* Iterator over the list of potentially admissible overloads */
         const function_record *overloads = reinterpret_cast<function_record *>(
                                   PyCapsule_GetPointer(self, get_function_record_capsule_name())),
-                              *it = overloads;
+                              *current_overload = overloads;
         assert(overloads != nullptr);
 
         /* Need to know how many arguments + keyword arguments there are to pick the right
            overload */
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
 
         auto self_value_and_holder = value_and_holder();
         if (overloads->is_constructor) {
             if (!parent
                 || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
-                PyErr_SetString(
-                    PyExc_TypeError,
-                    "__init__(self, ...) called with invalid or missing `self` argument");
+                set_error(PyExc_TypeError,
+                          "__init__(self, ...) called with invalid or missing `self` argument");
                 return nullptr;
             }
 
             auto *const tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
             auto *const pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder = pi->get_value_and_holder(tinfo, true);
 
@@ -715,17 +755,18 @@
             // We do this in two passes: in the first pass, we load arguments with `convert=false`;
             // in the second, we allow conversion (except for arguments with an explicit
             // py::arg().noconvert()).  This lets us prefer calls without conversion, with
             // conversion as a fallback.
             std::vector<function_call> second_pass;
 
             // However, if there are no overloads, we can just skip the no-convert pass entirely
-            const bool overloaded = it != nullptr && it->next != nullptr;
+            const bool overloaded
+                = current_overload != nullptr && current_overload->next != nullptr;
 
-            for (; it != nullptr; it = it->next) {
+            for (; current_overload != nullptr; current_overload = current_overload->next) {
 
                 /* For each overload:
                    1. Copy all positional arguments we were given, also checking to make sure that
                       named positional arguments weren't *also* specified via kwarg.
                    2. If we weren't given enough, try to make up the omitted ones by checking
                       whether they were provided by a kwarg matching the `py::arg("name")` name. If
                       so, use it (and remove it from kwargs); if not, see if the function binding
@@ -738,15 +779,15 @@
                       extra tuple or dict at the end of the positional arguments.
                    6. Call the function call dispatcher (function_record::impl)
 
                    If one of these fail, move on to the next overload and keep trying until we get
                    a result other than PYBIND11_TRY_NEXT_OVERLOAD.
                  */
 
-                const function_record &func = *it;
+                const function_record &func = *current_overload;
                 size_t num_args = func.nargs; // Number of positional arguments that we need
                 if (func.has_args) {
                     --num_args; // (but don't count py::args
                 }
                 if (func.has_kwargs) {
                     --num_args; //  or py::kwargs)
                 }
@@ -976,18 +1017,18 @@
                         loader_life_support guard{};
                         result = call.func.impl(call);
                     } catch (reference_cast_error &) {
                         result = PYBIND11_TRY_NEXT_OVERLOAD;
                     }
 
                     if (result.ptr() != PYBIND11_TRY_NEXT_OVERLOAD) {
-                        // The error reporting logic below expects 'it' to be valid, as it would be
-                        // if we'd encountered this failure in the first-pass loop.
+                        // The error reporting logic below expects 'current_overload' to be valid,
+                        // as it would be if we'd encountered this failure in the first-pass loop.
                         if (!result) {
-                            it = &call.func;
+                            current_overload = &call.func;
                         }
                         break;
                     }
                 }
             }
         } catch (error_already_set &e) {
             e.restore();
@@ -1003,15 +1044,15 @@
                registration. If none of the module-locale translators handle
                the exception (or there are no module-locale translators) then
                the global translators will be tried, also in reverse order of
                registration.
 
                A translator may choose to do one of the following:
 
-                - catch the exception and call PyErr_SetString or PyErr_SetObject
+                - catch the exception and call py::set_error()
                   to set a standard (or custom) Python exception, or
                 - do nothing and let the exception fall through to the next translator, or
                 - delegate translation to the next translator by throwing a new type of exception.
              */
 
             auto &local_exception_translators
                 = get_local_internals().registered_exception_translators;
@@ -1019,16 +1060,15 @@
                 return nullptr;
             }
             auto &exception_translators = get_internals().registered_exception_translators;
             if (detail::apply_exception_translators(exception_translators)) {
                 return nullptr;
             }
 
-            PyErr_SetString(PyExc_SystemError,
-                            "Exception escaped from default exception translator!");
+            set_error(PyExc_SystemError, "Exception escaped from default exception translator!");
             return nullptr;
         }
 
         auto append_note_if_missing_header_is_suspected = [](std::string &msg) {
             if (msg.find("std::") != std::string::npos) {
                 msg += "\n\n"
                        "Did you forget to `#include <pybind11/stl.h>`? Or <pybind11/complex.h>,\n"
@@ -1098,15 +1138,15 @@
                 auto kwargs = reinterpret_borrow<dict>(kwargs_in);
                 if (!kwargs.empty()) {
                     if (some_args) {
                         msg += "; ";
                     }
                     msg += "kwargs: ";
                     bool first = true;
-                    for (auto kwarg : kwargs) {
+                    for (const auto &kwarg : kwargs) {
                         if (first) {
                             first = false;
                         } else {
                             msg += ", ";
                         }
                         msg += pybind11::str("{}=").format(kwarg.first);
                         try {
@@ -1121,38 +1161,48 @@
             append_note_if_missing_header_is_suspected(msg);
             // Attach additional error info to the exception if supported
             if (PyErr_Occurred()) {
                 // #HelpAppreciated: unit test coverage for this branch.
                 raise_from(PyExc_TypeError, msg.c_str());
                 return nullptr;
             }
-            PyErr_SetString(PyExc_TypeError, msg.c_str());
+            set_error(PyExc_TypeError, msg.c_str());
             return nullptr;
         }
         if (!result) {
             std::string msg = "Unable to convert function return value to a "
                               "Python type! The signature was\n\t";
-            msg += it->signature;
+            assert(current_overload != nullptr);
+            msg += current_overload->signature;
             append_note_if_missing_header_is_suspected(msg);
             // Attach additional error info to the exception if supported
             if (PyErr_Occurred()) {
                 raise_from(PyExc_TypeError, msg.c_str());
                 return nullptr;
             }
-            PyErr_SetString(PyExc_TypeError, msg.c_str());
+            set_error(PyExc_TypeError, msg.c_str());
             return nullptr;
         }
         if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
             auto *pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder.type->init_instance(pi, nullptr);
         }
         return result.ptr();
     }
 };
 
+PYBIND11_NAMESPACE_BEGIN(detail)
+
+template <>
+struct handle_type_name<cpp_function> {
+    static constexpr auto name = const_name("Callable");
+};
+
+PYBIND11_NAMESPACE_END(detail)
+
 /// Wrapper for Python extension modules
 class module_ : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(module_, object, PyModule_Check)
 
     /// Create a new top-level Python module with the given name and docstring
     PYBIND11_DEPRECATED("Use PYBIND11_MODULE or module_::create_extension_module instead")
@@ -1272,14 +1322,23 @@
         // TODO: Should be reinterpret_steal for Python 3, but Python also steals it again when
         //       returned from PyInit_...
         //       For Python 2, reinterpret_borrow was correct.
         return reinterpret_borrow<module_>(m);
     }
 };
 
+PYBIND11_NAMESPACE_BEGIN(detail)
+
+template <>
+struct handle_type_name<module_> {
+    static constexpr auto name = const_name("module");
+};
+
+PYBIND11_NAMESPACE_END(detail)
+
 // When inside a namespace (or anywhere as long as it's not the first item on a line),
 // C++20 allows "module" to be used. This is provided for backward compatibility, and for
 // simplicity, if someone wants to use py::module for example, that is perfectly safe.
 using module = module_;
 
 /// \ingroup python_builtins
 /// Return a dictionary representing the global variables in the current execution frame,
@@ -1973,15 +2032,15 @@
         m_base.attr("name") = property(cpp_function(&enum_name, name("name"), is_method(m_base)));
 
         m_base.attr("__str__") = cpp_function(
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(std::move(type_name), enum_name(arg));
             },
-            name("name"),
+            name("__str__"),
             is_method(m_base));
 
         if (options::show_enum_members_docstring()) {
             m_base.attr("__doc__") = static_property(
                 cpp_function(
                     [](handle arg) -> std::string {
                         std::string docstring;
@@ -2391,92 +2450,104 @@
                     return Access()(s.it);
                     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
                 },
                 std::forward<Extra>(extra)...,
                 Policy);
     }
 
-    return cast(state{first, last, true});
+    return cast(state{std::forward<Iterator>(first), std::forward<Sentinel>(last), true});
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_access<Iterator>::result_type,
           typename... Extra>
-iterator make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<ValueType> make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the keys (`.first`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename KeyType = typename detail::iterator_key_access<Iterator>::result_type,
           typename... Extra>
-iterator make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<KeyType> make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_key_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       KeyType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the values (`.second`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_value_access<Iterator>::result_type,
           typename... Extra>
-iterator make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<ValueType> make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_value_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over values of an stl container or other container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename ValueType = typename detail::iterator_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<ValueType> make_iterator(Type &value, Extra &&...extra) {
     return make_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over the keys (`.first`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename KeyType = typename detail::iterator_key_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_key_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<KeyType> make_key_iterator(Type &value, Extra &&...extra) {
     return make_key_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over the values (`.second`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename ValueType = typename detail::iterator_value_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_value_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<ValueType> make_value_iterator(Type &value, Extra &&...extra) {
     return make_value_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 template <typename InputType, typename OutputType>
 void implicitly_convertible() {
     struct set_flag {
@@ -2524,15 +2595,15 @@
     detail::get_local_internals().registered_exception_translators.push_front(
         std::forward<ExceptionTranslator>(translator));
 }
 
 /**
  * Wrapper to generate a new Python exception type.
  *
- * This should only be used with PyErr_SetString for now.
+ * This should only be used with py::set_error() for now.
  * It is not (yet) possible to use as a py::base.
  * Template type argument is reserved for future use.
  */
 template <typename type>
 class exception : public object {
 public:
     exception() = default;
@@ -2545,50 +2616,48 @@
                           "definitions with name \""
                           + std::string(name) + "\"");
         }
         scope.attr(name) = *this;
     }
 
     // Sets the current python exception to this exception object with the given message
-    void operator()(const char *message) { PyErr_SetString(m_ptr, message); }
+    PYBIND11_DEPRECATED("Please use py::set_error() instead "
+                        "(https://github.com/pybind/pybind11/pull/4772)")
+    void operator()(const char *message) const { set_error(*this, message); }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-// Returns a reference to a function-local static exception object used in the simple
-// register_exception approach below.  (It would be simpler to have the static local variable
-// directly in register_exception, but that makes clang <3.5 segfault - issue #1349).
-template <typename CppException>
-exception<CppException> &get_exception_object() {
-    static exception<CppException> ex;
-    return ex;
-}
+
+template <>
+struct handle_type_name<exception<void>> {
+    static constexpr auto name = const_name("Exception");
+};
 
 // Helper function for register_exception and register_local_exception
 template <typename CppException>
 exception<CppException> &
 register_exception_impl(handle scope, const char *name, handle base, bool isLocal) {
-    auto &ex = detail::get_exception_object<CppException>();
-    if (!ex) {
-        ex = exception<CppException>(scope, name, base);
-    }
+    PYBIND11_CONSTINIT static gil_safe_call_once_and_store<exception<CppException>> exc_storage;
+    exc_storage.call_once_and_store_result(
+        [&]() { return exception<CppException>(scope, name, base); });
 
     auto register_func
         = isLocal ? &register_local_exception_translator : &register_exception_translator;
 
     register_func([](std::exception_ptr p) {
         if (!p) {
             return;
         }
         try {
             std::rethrow_exception(p);
         } catch (const CppException &e) {
-            detail::get_exception_object<CppException>()(e.what());
+            set_error(exc_storage.get_stored(), e.what());
         }
     });
-    return ex;
+    return exc_storage.get_stored();
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /**
  * Registers a Python exception in `m` of the given `name` and installs a translator to
  * translate the C++ exception to the created Python exception using the what() method.
@@ -2699,15 +2768,19 @@
     PyFrameObject *frame = PyThreadState_GetFrame(PyThreadState_Get());
     if (frame != nullptr) {
         PyCodeObject *f_code = PyFrame_GetCode(frame);
         // f_code is guaranteed to not be NULL
         if ((std::string) str(f_code->co_name) == name && f_code->co_argcount > 0) {
             PyObject *locals = PyEval_GetLocals();
             if (locals != nullptr) {
+#        if PY_VERSION_HEX >= 0x030b0000
+                PyObject *co_varnames = PyCode_GetVarnames(f_code);
+#        else
                 PyObject *co_varnames = PyObject_GetAttrString((PyObject *) f_code, "co_varnames");
+#        endif
                 PyObject *self_arg = PyTuple_GET_ITEM(co_varnames, 0);
                 Py_DECREF(co_varnames);
                 PyObject *self_caller = dict_getitem(locals, self_arg);
                 if (self_caller == self.ptr()) {
                     Py_DECREF(f_code);
                     Py_DECREF(frame);
                     return function();
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/pytypes.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/pytypes.h`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 struct obj_attr;
 struct str_attr;
 struct generic_item;
 struct sequence_item;
 struct list_item;
 struct tuple_item;
 } // namespace accessor_policies
+// PLEASE KEEP handle_type_name SPECIALIZATIONS IN SYNC.
 using obj_attr_accessor = accessor<accessor_policies::obj_attr>;
 using str_attr_accessor = accessor<accessor_policies::str_attr>;
 using item_accessor = accessor<accessor_policies::generic_item>;
 using sequence_accessor = accessor<accessor_policies::sequence_item>;
 using list_accessor = accessor<accessor_policies::list_item>;
 using tuple_accessor = accessor<accessor_policies::tuple_item>;
 
@@ -299,24 +300,29 @@
 private:
 #ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
     void throw_gilstate_error(const std::string &function_name) const {
         fprintf(
             stderr,
             "%s is being called while the GIL is either not held or invalid. Please see "
             "https://pybind11.readthedocs.io/en/stable/advanced/"
-            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n",
+            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n"
+            "If you are convinced there is no bug in your code, you can #define "
+            "PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF "
+            "to disable this check. In that case you have to ensure this #define is consistently "
+            "used for all translation units linked into a given pybind11 extension, otherwise "
+            "there will be ODR violations.",
             function_name.c_str());
-        fflush(stderr);
         if (Py_TYPE(m_ptr)->tp_name != nullptr) {
             fprintf(stderr,
-                    "The failing %s call was triggered on a %s object.\n",
+                    " The failing %s call was triggered on a %s object.",
                     function_name.c_str(),
                     Py_TYPE(m_ptr)->tp_name);
-            fflush(stderr);
         }
+        fprintf(stderr, "\n");
+        fflush(stderr);
         throw std::runtime_error(function_name + " PyGILState_Check() failure.");
     }
 #endif
 
 #ifdef PYBIND11_HANDLE_REF_DEBUG
     static std::size_t inc_ref_counter(std::size_t add) {
         thread_local std::size_t counter = 0;
@@ -325,14 +331,22 @@
     }
 
 public:
     static std::size_t inc_ref_counter() { return inc_ref_counter(0); }
 #endif
 };
 
+inline void set_error(const handle &type, const char *message) {
+    PyErr_SetString(type.ptr(), message);
+}
+
+inline void set_error(const handle &type, const handle &value) {
+    PyErr_SetObject(type.ptr(), value.ptr());
+}
+
 /** \rst
     Holds a reference to a Python object (with reference counting)
 
     Like `handle`, the `object` class is a thin wrapper around an arbitrary Python
     object (i.e. a ``PyObject *`` in Python's C API). In contrast to `handle`, it
     optionally increases the object's reference count upon construction, and it
     *always* decreases the reference count when the `object` instance goes out of
@@ -1603,15 +1617,23 @@
 };
 /// @} pytypes
 
 inline namespace literals {
 /** \rst
     String literal version of `str`
  \endrst */
-inline str operator"" _s(const char *s, size_t size) { return {s, size}; }
+inline str
+#if !defined(__clang__) && defined(__GNUC__) && __GNUC__ < 5
+operator"" _s // gcc 4.8.5 insists on having a space (hard error).
+#else
+operator""_s // clang 17 generates a deprecation warning if there is a space.
+#endif
+    (const char *s, size_t size) {
+    return {s, size};
+}
 } // namespace literals
 
 /// \addtogroup pytypes
 /// @{
 class bytes : public object {
 public:
     PYBIND11_OBJECT(bytes, object, PYBIND11_BYTES_CHECK)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl/filesystem.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl.h`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             if (!value_ || !s.add(std::move(value_))) {
                 return handle();
             }
         }
         return s.release();
     }
 
-    PYBIND11_TYPE_CASTER(type, const_name("Set[") + key_conv::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(type, const_name("set[") + key_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Key, typename Value>
 struct map_caster {
     using key_conv = make_caster<Key>;
     using value_conv = make_caster<Value>;
 
@@ -153,30 +153,30 @@
             }
             d[std::move(key)] = std::move(value);
         }
         return d.release();
     }
 
     PYBIND11_TYPE_CASTER(Type,
-                         const_name("Dict[") + key_conv::name + const_name(", ") + value_conv::name
+                         const_name("dict[") + key_conv::name + const_name(", ") + value_conv::name
                              + const_name("]"));
 };
 
 template <typename Type, typename Value>
 struct list_caster {
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
         if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src)) {
             return false;
         }
         auto s = reinterpret_borrow<sequence>(src);
         value.clear();
         reserve_maybe(s, &value);
-        for (auto it : s) {
+        for (const auto &it : s) {
             value_conv conv;
             if (!conv.load(it, convert)) {
                 return false;
             }
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
@@ -204,15 +204,15 @@
                 return handle();
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, const_name("List[") + value_conv::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("list[") + value_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Alloc>
 struct type_caster<std::vector<Type, Alloc>> : list_caster<std::vector<Type, Alloc>, Type> {};
 
 template <typename Type, typename Alloc>
 struct type_caster<std::deque<Type, Alloc>> : list_caster<std::deque<Type, Alloc>, Type> {};
@@ -243,15 +243,15 @@
             return false;
         }
         auto l = reinterpret_borrow<sequence>(src);
         if (!require_size(l.size())) {
             return false;
         }
         size_t ctr = 0;
-        for (auto it : l) {
+        for (const auto &it : l) {
             value_conv conv;
             if (!conv.load(it, convert)) {
                 return false;
             }
             value[ctr++] = cast_op<Value &&>(std::move(conv));
         }
         return true;
@@ -270,15 +270,15 @@
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(ArrayType,
                          const_name<Resizable>(const_name(""), const_name("Annotated["))
-                             + const_name("List[") + value_conv::name + const_name("]")
+                             + const_name("list[") + value_conv::name + const_name("]")
                              + const_name<Resizable>(const_name(""),
                                                      const_name(", FixedSize(")
                                                          + const_name<Size>() + const_name(")]")));
 };
 
 template <typename Type, size_t Size>
 struct type_caster<std::array<Type, Size>>
@@ -417,15 +417,16 @@
     static handle cast(Variant &&src, return_value_policy policy, handle parent) {
         return visit_helper<V>::call(variant_caster_visitor{policy, parent},
                                      std::forward<Variant>(src));
     }
 
     using Type = V<Ts...>;
     PYBIND11_TYPE_CASTER(Type,
-                         const_name("Union[") + detail::concat(make_caster<Ts>::name...)
+                         const_name("Union[")
+                             + ::pybind11::detail::concat(make_caster<Ts>::name...)
                              + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_VARIANT)
 template <typename... Ts>
 struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> {};
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/stl_bind.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl_bind.h`

 * *Files 6% similar despite different names*

```diff
@@ -154,16 +154,15 @@
         v->reserve(len_hint(it));
         for (handle h : it) {
             v->push_back(h.cast<T>());
         }
         return v.release();
     }));
 
-    cl.def(
-        "clear", [](Vector &v) { v.clear(); }, "Clear the contents");
+    cl.def("clear", [](Vector &v) { v.clear(); }, "Clear the contents");
 
     cl.def(
         "extend",
         [](Vector &v, const Vector &src) { v.insert(v.end(), src.begin(), src.end()); },
         arg("L"),
         "Extend the list by appending all the items in the given list");
 
@@ -521,15 +520,15 @@
     detail::vector_accessor<Vector, Class_>(cl);
 
     cl.def(
         "__bool__",
         [](const Vector &v) -> bool { return !v.empty(); },
         "Check whether the list is nonempty");
 
-    cl.def("__len__", &Vector::size);
+    cl.def("__len__", [](const Vector &vec) { return vec.size(); });
 
 #if 0
     // C++ style functions deprecated, leaving it here as an example
     cl.def(init<size_type>());
 
     cl.def("resize",
          (void (Vector::*) (size_type count)) & Vector::resize,
@@ -641,132 +640,109 @@
             }
             s << '}';
             return s.str();
         },
         "Return the canonical string representation of this map.");
 }
 
-template <typename KeyType>
 struct keys_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
-    virtual bool contains(const KeyType &k) = 0;
-    virtual bool contains(const object &k) = 0;
+    virtual bool contains(const handle &k) = 0;
     virtual ~keys_view() = default;
 };
 
-template <typename MappedType>
 struct values_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
     virtual ~values_view() = default;
 };
 
-template <typename KeyType, typename MappedType>
 struct items_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
     virtual ~items_view() = default;
 };
 
-template <typename Map, typename KeysView>
-struct KeysViewImpl : public KeysView {
+template <typename Map>
+struct KeysViewImpl : public detail::keys_view {
     explicit KeysViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_key_iterator(map.begin(), map.end()); }
-    bool contains(const typename Map::key_type &k) override { return map.find(k) != map.end(); }
-    bool contains(const object &) override { return false; }
+    bool contains(const handle &k) override {
+        try {
+            return map.find(k.template cast<typename Map::key_type>()) != map.end();
+        } catch (const cast_error &) {
+            return false;
+        }
+    }
     Map &map;
 };
 
-template <typename Map, typename ValuesView>
-struct ValuesViewImpl : public ValuesView {
+template <typename Map>
+struct ValuesViewImpl : public detail::values_view {
     explicit ValuesViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_value_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
-template <typename Map, typename ItemsView>
-struct ItemsViewImpl : public ItemsView {
+template <typename Map>
+struct ItemsViewImpl : public detail::items_view {
     explicit ItemsViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
 class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args &&...args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
-    using StrippedKeyType = detail::remove_cvref_t<KeyType>;
-    using StrippedMappedType = detail::remove_cvref_t<MappedType>;
-    using KeysView = detail::keys_view<StrippedKeyType>;
-    using ValuesView = detail::values_view<StrippedMappedType>;
-    using ItemsView = detail::items_view<StrippedKeyType, StrippedMappedType>;
+    using KeysView = detail::keys_view;
+    using ValuesView = detail::values_view;
+    using ItemsView = detail::items_view;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
     auto *tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
-    static constexpr auto key_type_descr = detail::make_caster<KeyType>::name;
-    static constexpr auto mapped_type_descr = detail::make_caster<MappedType>::name;
-    std::string key_type_name(key_type_descr.text), mapped_type_name(mapped_type_descr.text);
-
-    // If key type isn't properly wrapped, fall back to C++ names
-    if (key_type_name == "%") {
-        key_type_name = detail::type_info_description(typeid(KeyType));
-    }
-    // Similarly for value type:
-    if (mapped_type_name == "%") {
-        mapped_type_name = detail::type_info_description(typeid(MappedType));
-    }
 
-    // Wrap KeysView[KeyType] if it wasn't already wrapped
+    // Wrap KeysView if it wasn't already wrapped
     if (!detail::get_type_info(typeid(KeysView))) {
-        class_<KeysView> keys_view(
-            scope, ("KeysView[" + key_type_name + "]").c_str(), pybind11::module_local(local));
+        class_<KeysView> keys_view(scope, "KeysView", pybind11::module_local(local));
         keys_view.def("__len__", &KeysView::len);
         keys_view.def("__iter__",
                       &KeysView::iter,
                       keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
-        keys_view.def("__contains__",
-                      static_cast<bool (KeysView::*)(const KeyType &)>(&KeysView::contains));
-        // Fallback for when the object is not of the key type
-        keys_view.def("__contains__",
-                      static_cast<bool (KeysView::*)(const object &)>(&KeysView::contains));
+        keys_view.def("__contains__", &KeysView::contains);
     }
     // Similarly for ValuesView:
     if (!detail::get_type_info(typeid(ValuesView))) {
-        class_<ValuesView> values_view(scope,
-                                       ("ValuesView[" + mapped_type_name + "]").c_str(),
-                                       pybind11::module_local(local));
+        class_<ValuesView> values_view(scope, "ValuesView", pybind11::module_local(local));
         values_view.def("__len__", &ValuesView::len);
         values_view.def("__iter__",
                         &ValuesView::iter,
                         keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
     }
     // Similarly for ItemsView:
     if (!detail::get_type_info(typeid(ItemsView))) {
-        class_<ItemsView> items_view(
-            scope,
-            ("ItemsView[" + key_type_name + ", ").append(mapped_type_name + "]").c_str(),
-            pybind11::module_local(local));
+        class_<ItemsView> items_view(scope, "ItemsView", pybind11::module_local(local));
         items_view.def("__len__", &ItemsView::len);
         items_view.def("__iter__",
                        &ItemsView::iter,
                        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
     }
 
@@ -784,33 +760,27 @@
         "__iter__",
         [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
         keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
     );
 
     cl.def(
         "keys",
-        [](Map &m) {
-            return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map, KeysView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "values",
-        [](Map &m) {
-            return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map, ValuesView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "items",
-        [](Map &m) {
-            return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map, ItemsView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
@@ -839,13 +809,14 @@
         auto it = m.find(k);
         if (it == m.end()) {
             throw key_error();
         }
         m.erase(it);
     });
 
-    cl.def("__len__", &Map::size);
+    // Always use a lambda in case of `using` declaration
+    cl.def("__len__", [](const Map &m) { return m.size(); });
 
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `pyhtml2md-1.5.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/FindCatch.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/FindEigen3.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/FindPythonLibsNew.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,30 @@
 endif()
 
 # Use the Python interpreter to find the libs.
 if(NOT PythonLibsNew_FIND_VERSION)
   set(PythonLibsNew_FIND_VERSION "3.6")
 endif()
 
+if(NOT CMAKE_VERSION VERSION_LESS "3.27")
+  cmake_policy(GET CMP0148 _pybind11_cmp0148)
+  if(NOT _pybind11_cmp0148)
+    message(
+      AUTHOR_WARNING
+        "Policy CMP0148 is not set: The FindPythonInterp and FindPythonLibs "
+        "modules are removed.  Run \"cmake --help-policy CMP0148\" for policy "
+        "details.  Use the cmake_policy command to set the policy and suppress "
+        "this warning, or preferably upgrade to using FindPython, either by "
+        "calling it explicitly before pybind11, or by setting "
+        "PYBIND11_FINDPYTHON ON before pybind11.")
+  endif()
+  cmake_policy(SET CMP0148 OLD)
+  unset(_pybind11_cmp0148)
+endif()
+
 find_package(PythonInterp ${PythonLibsNew_FIND_VERSION} ${_pythonlibs_required}
              ${_pythonlibs_quiet})
 
 if(NOT PYTHONINTERP_FOUND)
   set(PYTHONLIBS_FOUND FALSE)
   set(PythonLibsNew_FOUND FALSE)
   return()
@@ -168,21 +184,28 @@
 endif()
 string(REGEX REPLACE ";" "\\\\;" _PYTHON_VALUES ${_PYTHON_VALUES})
 string(REGEX REPLACE "\n" ";" _PYTHON_VALUES ${_PYTHON_VALUES})
 _pybind11_get_if_undef(_PYTHON_VALUES 0 _PYTHON_VERSION_LIST)
 _pybind11_get_if_undef(_PYTHON_VALUES 1 PYTHON_PREFIX)
 _pybind11_get_if_undef(_PYTHON_VALUES 2 PYTHON_INCLUDE_DIR)
 _pybind11_get_if_undef(_PYTHON_VALUES 3 PYTHON_SITE_PACKAGES)
-_pybind11_get_if_undef(_PYTHON_VALUES 4 PYTHON_MODULE_EXTENSION)
 _pybind11_get_if_undef(_PYTHON_VALUES 5 PYTHON_IS_DEBUG)
 _pybind11_get_if_undef(_PYTHON_VALUES 6 PYTHON_SIZEOF_VOID_P)
 _pybind11_get_if_undef(_PYTHON_VALUES 7 PYTHON_LIBRARY_SUFFIX)
 _pybind11_get_if_undef(_PYTHON_VALUES 8 PYTHON_LIBDIR)
 _pybind11_get_if_undef(_PYTHON_VALUES 9 PYTHON_MULTIARCH)
 
+list(GET _PYTHON_VALUES 4 _PYTHON_MODULE_EXT_SUFFIX)
+if(PYBIND11_PYTHONLIBS_OVERWRITE OR NOT DEFINED PYTHON_MODULE_DEBUG_POSTFIX)
+  get_filename_component(PYTHON_MODULE_DEBUG_POSTFIX "${_PYTHON_MODULE_EXT_SUFFIX}" NAME_WE)
+endif()
+if(PYBIND11_PYTHONLIBS_OVERWRITE OR NOT DEFINED PYTHON_MODULE_EXTENSION)
+  get_filename_component(PYTHON_MODULE_EXTENSION "${_PYTHON_MODULE_EXT_SUFFIX}" EXT)
+endif()
+
 # Make sure the Python has the same pointer-size as the chosen compiler
 # Skip if CMAKE_SIZEOF_VOID_P is not defined
 # This should be skipped for (non-Apple) cross-compiles (like EMSCRIPTEN)
 if(NOT CMAKE_CROSSCOMPILING
    AND CMAKE_SIZEOF_VOID_P
    AND (NOT "${PYTHON_SIZEOF_VOID_P}" STREQUAL "${CMAKE_SIZEOF_VOID_P}"))
   if(PythonLibsNew_FIND_REQUIRED)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/JoinPaths.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/check-style.sh` & `pyhtml2md-1.5.4/python/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/cmake_uninstall.cmake.in` & `pyhtml2md-1.5.4/python/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pyhtml2md-1.5.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/libsize.py` & `pyhtml2md-1.5.4/python/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/pybind11Common.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Common.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -159,22 +159,34 @@
                           "(last two chars: ${VAL} not understood as a valid CXX std)")
     endif()
   endif()
 endif()
 
 # --------------------- Python specifics -------------------------
 
+# CMake 3.27 removes the classic FindPythonInterp if CMP0148 is NEW
+if(CMAKE_VERSION VERSION_LESS "3.27")
+  set(_pybind11_missing_old_python "OLD")
+else()
+  cmake_policy(GET CMP0148 _pybind11_missing_old_python)
+endif()
+
 # Check to see which Python mode we are in, new, old, or no python
 if(PYBIND11_NOPYTHON)
   set(_pybind11_nopython ON)
+  # We won't use new FindPython if PYBIND11_FINDPYTHON is defined and falselike
+  # Otherwise, we use if FindPythonLibs is missing or if FindPython was already used
 elseif(
-  PYBIND11_FINDPYTHON
-  OR Python_FOUND
-  OR Python2_FOUND
-  OR Python3_FOUND)
+  (NOT DEFINED PYBIND11_FINDPYTHON OR PYBIND11_FINDPYTHON)
+  AND (_pybind11_missing_old_python STREQUAL "NEW"
+       OR PYBIND11_FINDPYTHON
+       OR Python_FOUND
+       OR Python3_FOUND
+      ))
+
   # New mode
   include("${CMAKE_CURRENT_LIST_DIR}/pybind11NewTools.cmake")
 
 else()
 
   # Classic mode
   include("${CMAKE_CURRENT_LIST_DIR}/pybind11Tools.cmake")
@@ -206,16 +218,23 @@
       set(status_level FATAL_ERROR)
     else()
       set(status_level WARNING)
     endif()
 
     execute_process(
       COMMAND
-        ${${_Python}_EXECUTABLE} -c
-        "from pkg_resources import get_distribution; print(get_distribution('${PYPI_NAME}').version)"
+        ${${_Python}_EXECUTABLE} -c "
+try:
+    from importlib.metadata import version
+except ImportError:
+    from pkg_resources import get_distribution
+    def version(s):
+        return get_distribution(s).version
+print(version('${PYPI_NAME}'))
+        "
       RESULT_VARIABLE RESULT_PRESENT
       OUTPUT_VARIABLE PKG_VERSION
       ERROR_QUIET)
 
     string(STRIP "${PKG_VERSION}" PKG_VERSION)
 
     # If a result is present, this failed
@@ -288,29 +307,32 @@
     if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND NOT APPLE)
       # Clang Gold plugin does not support -Os; append -O3 to MinSizeRel builds to override it
       set(linker_append ";$<$<CONFIG:MinSizeRel>:-O3>")
     elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU" AND NOT MINGW)
       set(cxx_append ";-fno-fat-lto-objects")
     endif()
 
-    if(CMAKE_SYSTEM_PROCESSOR MATCHES "ppc64le" OR CMAKE_SYSTEM_PROCESSOR MATCHES "mips64")
-      set(NO_FLTO_ARCH TRUE)
+    if(prefer_thin_lto)
+      set(thin "=thin")
     else()
-      set(NO_FLTO_ARCH FALSE)
+      set(thin "")
     endif()
 
-    if(CMAKE_CXX_COMPILER_ID MATCHES "Clang"
-       AND prefer_thin_lto
-       AND NOT NO_FLTO_ARCH)
+    if(CMAKE_SYSTEM_PROCESSOR MATCHES "ppc64le" OR CMAKE_SYSTEM_PROCESSOR MATCHES "mips64")
+      # Do nothing
+    elseif(CMAKE_SYSTEM_PROCESSOR MATCHES emscripten)
+      # This compile is very costly when cross-compiling, so set this without checking
+      set(PYBIND11_LTO_CXX_FLAGS "-flto${thin}${cxx_append}")
+      set(PYBIND11_LTO_LINKER_FLAGS "-flto${thin}${linker_append}")
+    elseif(CMAKE_CXX_COMPILER_ID MATCHES "Clang")
       _pybind11_return_if_cxx_and_linker_flags_work(
-        HAS_FLTO_THIN "-flto=thin${cxx_append}" "-flto=thin${linker_append}"
+        HAS_FLTO_THIN "-flto${thin}${cxx_append}" "-flto=${thin}${linker_append}"
         PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
     endif()
-
-    if(NOT HAS_FLTO_THIN AND NOT NO_FLTO_ARCH)
+    if(NOT HAS_FLTO_THIN)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO "-flto${cxx_append}" "-flto${linker_append}" PYBIND11_LTO_CXX_FLAGS
         PYBIND11_LTO_LINKER_FLAGS)
     endif()
   elseif(CMAKE_CXX_COMPILER_ID MATCHES "IntelLLVM")
     # IntelLLVM equivalent to LTO is called IPO; also IntelLLVM is WIN32/UNIX
     # WARNING/HELP WANTED: This block of code is currently not covered by pybind11 GitHub Actions!
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/pybind11Config.cmake.in` & `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Config.cmake.in`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,17 @@
   Adds bigobj and mp for MSVC.
 
 Modes
 =====
 
 There are two modes provided; classic, which is built on the old Python
 discovery packages in CMake, or the new FindPython mode, which uses FindPython
-from 3.12+ forward (3.15+ _highly_ recommended).
+from 3.12+ forward (3.15+ _highly_ recommended). If you set the minimum or
+maximum version of CMake to 3.27+, then FindPython is the default (since
+FindPythonInterp/FindPythonLibs has been removed via policy `CMP0148`).
 
 New FindPython mode
 ^^^^^^^^^^^^^^^^^^^
 
 To activate this mode, either call ``find_package(Python COMPONENTS Interpreter Development)``
 before finding this package, or set the ``PYBIND11_FINDPYTHON`` variable to ON. In this mode,
 you can either use the basic targets, or use the FindPython tools:
@@ -143,15 +145,15 @@
 
 Add a module and setup all helpers. You can select the type of the library; the
 default is ``MODULE``. There are several options:
 
 ``OPT_SIZE``
   Optimize for size, even if the ``CMAKE_BUILD_TYPE`` is not ``MinSizeRel``.
 ``THIN_LTO``
-  Use thin TLO instead of regular if there's a choice (pybind11's selection
+  Use thin LTO instead of regular if there's a choice (pybind11's selection
   is disabled if ``CMAKE_INTERPROCEDURAL_OPTIMIZATIONS`` is set).
 ``WITHOUT_SOABI``
   Disable the SOABI component (``PYBIND11_NEWPYTHON`` mode only).
 ``NO_EXTRAS``
   Disable all extras, exit immediately after making the module.
 
 pybind11_strip
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/pybind11Tools.cmake` & `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Tools.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   set(PYBIND11_PYTHON_VERSION
       ""
       CACHE STRING "Python version to use for compiling modules")
 endif()
 
 # A user can set versions manually too
 set(Python_ADDITIONAL_VERSIONS
-    "3.11;3.10;3.9;3.8;3.7;3.6"
+    "3.12;3.11;3.10;3.9;3.8;3.7;3.6"
     CACHE INTERNAL "")
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}")
 find_package(PythonLibsNew ${PYBIND11_PYTHON_VERSION} MODULE REQUIRED ${_pybind11_quiet})
 list(REMOVE_AT CMAKE_MODULE_PATH -1)
 
 # Makes a normal variable a cached variable
@@ -61,14 +61,15 @@
 endmacro()
 
 # Cache variables so pybind11_add_module can be used in parent projects
 _pybind11_promote_to_cache(PYTHON_INCLUDE_DIRS)
 _pybind11_promote_to_cache(PYTHON_LIBRARIES)
 _pybind11_promote_to_cache(PYTHON_MODULE_PREFIX)
 _pybind11_promote_to_cache(PYTHON_MODULE_EXTENSION)
+_pybind11_promote_to_cache(PYTHON_MODULE_DEBUG_POSTFIX)
 _pybind11_promote_to_cache(PYTHON_VERSION_MAJOR)
 _pybind11_promote_to_cache(PYTHON_VERSION_MINOR)
 _pybind11_promote_to_cache(PYTHON_VERSION)
 _pybind11_promote_to_cache(PYTHON_IS_DEBUG)
 
 if(PYBIND11_MASTER_PROJECT)
   if(PYTHON_MODULE_EXTENSION MATCHES "pypy")
@@ -144,16 +145,19 @@
 
   target_link_libraries(pybind11::embed INTERFACE pybind11::pybind11
                                                   pybind11::_ClassicPythonLibraries)
 endif()
 
 function(pybind11_extension name)
   # The prefix and extension are provided by FindPythonLibsNew.cmake
-  set_target_properties(${name} PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
-                                           SUFFIX "${PYTHON_MODULE_EXTENSION}")
+  set_target_properties(
+    ${name}
+    PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
+               DEBUG_POSTFIX "${PYTHON_MODULE_DEBUG_POSTFIX}"
+               SUFFIX "${PYTHON_MODULE_EXTENSION}")
 endfunction()
 
 # Build a Python extension module:
 # pybind11_add_module(<name> [MODULE | SHARED] [EXCLUDE_FROM_ALL]
 #                     [NO_EXTRAS] [THIN_LTO] [OPT_SIZE] source1 [source2 ...])
 #
 function(pybind11_add_module target_name)
@@ -208,18 +212,20 @@
     if(ARG_THIN_LTO)
       target_link_libraries(${target_name} PRIVATE pybind11::thin_lto)
     else()
       target_link_libraries(${target_name} PRIVATE pybind11::lto)
     endif()
   endif()
 
-  # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
-  string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
-  if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
-    pybind11_strip(${target_name})
+  if(DEFINED CMAKE_BUILD_TYPE) # see https://github.com/pybind/pybind11/issues/4454
+    # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
+    string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
+    if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
+      pybind11_strip(${target_name})
+    endif()
   endif()
 
   if(MSVC)
     target_link_libraries(${target_name} PRIVATE pybind11::windows_extras)
   endif()
 
   if(ARG_OPT_SIZE)
```

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/setup_global.py.in` & `pyhtml2md-1.5.4/python/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/python/pybind11/tools/setup_main.py.in` & `pyhtml2md-1.5.4/python/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/setup.py` & `pyhtml2md-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         )
 
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyhtml2md",
-    version="1.5.3",
+    version="1.5.4",
     author="Tim Gromeyer",
     author_email="sakul8826@gmail.com",
     description="Transform your HTML into clean, easy-to-read markdown with pyhtml2md.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tim-gromeyer/html2md",
     ext_modules=[CMakeExtension("pyhtml2md")],
```

### Comparing `pyhtml2md-1.5.3/src/html2md.cpp` & `pyhtml2md-1.5.4/src/html2md.cpp`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.3/src/table.cpp` & `pyhtml2md-1.5.4/src/table.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,18 @@
       tableData.push_back(std::move(rowData)); // Move rowData to avoid copying
     }
   }
 
   // Determine maximum width of each column
   vector<size_t> columnWidths(tableData[0].size(), 0);
   for (const auto &row : tableData) {
+    if (columnWidths.size() < row.size()) {
+      columnWidths.resize(row.size(), 0);
+    }
+
     for (size_t i = 0; i < row.size(); ++i) {
       columnWidths[i] = std::max(columnWidths[i], row[i].size());
     }
   }
 
   // Build the formatted table
   std::ostringstream formattedTable;
```

