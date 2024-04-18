# Comparing `tmp/arcae-0.2.2.tar.gz` & `tmp/arcae-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcae-0.2.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "arcae-0.2.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `arcae-0.2.2.tar` & `arcae-0.2.3.tar`

### file list

```diff
@@ -1,61 +1,81 @@
--rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 arcae-0.2.2/.dockerignore
--rw-r--r--   0        0        0     6293 2022-11-09 12:37:21.000000 arcae-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3534 2022-11-09 12:37:21.000000 arcae-0.2.2/.gitignore
--rw-r--r--   0        0        0      994 2022-11-09 12:37:21.000000 arcae-0.2.2/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 arcae-0.2.2/HISTORY.rst
--rw-r--r--   0        0        0     1564 2022-11-09 12:37:21.000000 arcae-0.2.2/LICENSE
--rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 arcae-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0     5709 2022-11-09 12:37:21.000000 arcae-0.2.2/README.rst
--rw-r--r--   0        0        0     2438 2022-11-09 12:37:21.000000 arcae-0.2.2/cmake_modules/FindPyArrow.cmake
--rw-r--r--   0        0        0     2555 2022-11-09 12:37:21.000000 arcae-0.2.2/cmake_modules/SetupVCPKG.cmake
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/CMakeLists.txt
--rw-r--r--   0        0        0     2517 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/casa_visitors.cc
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/casa_visitors.h
--rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/column_convert_visitor.cc
--rw-r--r--   0        0        0    16270 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/column_convert_visitor.h
--rw-r--r--   0        0        0     1285 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/complex_type.cc
--rw-r--r--   0        0        0     2420 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/complex_type.h
--rw-r--r--   0        0        0      807 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/configuration.cc
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/configuration.h
--rw-r--r--   0        0        0    11255 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/descriptor.cc
--rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/descriptor.h
--rw-r--r--   0        0        0     9040 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/safe_table_proxy.cc
--rw-r--r--   0        0        0     4534 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/safe_table_proxy.h
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/service_locator.cc
--rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/service_locator.h
--rw-r--r--   0        0        0     7316 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/table_factory.cc
--rw-r--r--   0        0        0      853 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/table_factory.h
--rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/utility.cc
--rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/arcae/utility.h
--rw-r--r--   0        0        0      504 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/tests/CMakeLists.txt
--rw-r--r--   0        0        0     1261 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/tests/basic_test.cc
--rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/tests/parallel_write_test.cc
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/tests/test_utils.cc
--rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 arcae-0.2.2/cpp/tests/test_utils.h
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 arcae-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 arcae-0.2.2/scripts/run_cibuildwheel.sh
--rw-r--r--   0        0        0     1318 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/CMakeLists.txt
--rw-r--r--   0        0        0     1020 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/applications/__init__.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/applications/entrypoint.py
--rw-r--r--   0        0        0     5436 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/applications/ms_export.py
--rw-r--r--   0        0        0     3783 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/arrow_tables.pxd
--rw-r--r--   0        0        0     9998 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/arrow_tables.pyx
--rw-r--r--   0        0        0      540 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/config.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/tests/__init__.py
--rw-r--r--   0        0        0    14076 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/tests/conftest.py
--rw-r--r--   0        0        0    10030 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/tests/test_descriptor.py
--rw-r--r--   0        0        0     3354 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/tests/test_multithreaded_read.py
--rw-r--r--   0        0        0    12851 2022-11-09 12:37:21.000000 arcae-0.2.2/src/arcae/tests/test_pytable.py
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 arcae-0.2.2/tbump.toml
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/manifest/vcpkg.json
--rw-r--r--   0        0        0    18800 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-ports/casacore/001-casacore-cmake.patch
--rw-r--r--   0        0        0     1937 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-ports/casacore/portfile.cmake
--rw-r--r--   0        0        0     1778 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-ports/casacore/vcpkg.json
--rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/arm64-osx-dynamic-cxx17-abi1-dbg.cmake
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/arm64-osx-dynamic-cxx17-abi1-rel.cmake
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/x64-linux-dynamic-cxx17-abi1-dbg.cmake
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/x64-linux-dynamic-cxx17-abi1-rel.cmake
--rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/x64-osx-dynamic-cxx17-abi1-dbg.cmake
--rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 arcae-0.2.2/vcpkg/overlay-triplets/x64-osx-dynamic-cxx17-abi1-rel.cmake
--rw-r--r--   0        0        0     8277 2022-11-09 12:37:21.000000 arcae-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2166 2022-11-09 12:37:21.000000 arcae-0.2.3/.cirrus.yml
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 arcae-0.2.3/.dockerignore
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 arcae-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     7941 2022-11-09 12:37:21.000000 arcae-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3556 2022-11-09 12:37:21.000000 arcae-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1658 2022-11-09 12:37:21.000000 arcae-0.2.3/CMakeLists.txt
+-rw-r--r--   0        0        0     2479 2022-11-09 12:37:21.000000 arcae-0.2.3/HISTORY.rst
+-rw-r--r--   0        0        0     1564 2022-11-09 12:37:21.000000 arcae-0.2.3/LICENSE
+-rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 arcae-0.2.3/MANIFEST.in
+-rw-r--r--   0        0        0     7860 2022-11-09 12:37:21.000000 arcae-0.2.3/README.rst
+-rw-r--r--   0        0        0     2498 2022-11-09 12:37:21.000000 arcae-0.2.3/cmake_modules/FindPyArrow.cmake
+-rw-r--r--   0        0        0     2657 2022-11-09 12:37:21.000000 arcae-0.2.3/cmake_modules/SetupVCPKG.cmake
+-rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      901 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/array_util.cc
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/array_util.h
+-rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/base_column_map.cc
+-rw-r--r--   0        0        0    23656 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/base_column_map.h
+-rw-r--r--   0        0        0     1743 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/casa_visitors.cc
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/casa_visitors.h
+-rw-r--r--   0        0        0    12816 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_read_map.cc
+-rw-r--r--   0        0        0     3834 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_read_map.h
+-rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_read_visitor.cc
+-rw-r--r--   0        0        0    13396 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_read_visitor.h
+-rw-r--r--   0        0        0    13568 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_write_map.cc
+-rw-r--r--   0        0        0     3463 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_write_map.h
+-rw-r--r--   0        0        0     6189 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_write_visitor.cc
+-rw-r--r--   0        0        0    13311 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/column_write_visitor.h
+-rw-r--r--   0        0        0     1285 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/complex_type.cc
+-rw-r--r--   0        0        0     2420 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/complex_type.h
+-rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/configuration.cc
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/configuration.h
+-rw-r--r--   0        0        0    11057 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/descriptor.cc
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/descriptor.h
+-rw-r--r--   0        0        0    10980 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/safe_table_proxy.cc
+-rw-r--r--   0        0        0     4757 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/safe_table_proxy.h
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/service_locator.cc
+-rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/service_locator.h
+-rw-r--r--   0        0        0     7301 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/table_factory.cc
+-rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/arcae/table_factory.h
+-rw-r--r--   0        0        0     1773 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/basic_test.cc
+-rw-r--r--   0        0        0     8987 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/column_iterator_test.cc
+-rw-r--r--   0        0        0    17986 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/column_map_test.cc
+-rw-r--r--   0        0        0    35627 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/column_rw_test.cc
+-rw-r--r--   0        0        0     5857 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/parallel_write_test.cc
+-rw-r--r--   0        0        0     6549 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/range_test.cc
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/test_utils.cc
+-rw-r--r--   0        0        0      178 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/test_utils.h
+-rw-r--r--   0        0        0    12912 2022-11-09 12:37:21.000000 arcae-0.2.3/cpp/tests/var_write_test.cc
+-rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 arcae-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 arcae-0.2.3/scripts/run_cibuildwheel.sh
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/CMakeLists.txt
+-rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/applications/__init__.py
+-rw-r--r--   0        0        0     1170 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/applications/entrypoint.py
+-rw-r--r--   0        0        0     5588 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/applications/ms_export.py
+-rw-r--r--   0        0        0     4729 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/arrow_tables.pxd
+-rw-r--r--   0        0        0    14624 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/arrow_tables.pyx
+-rw-r--r--   0        0        0      540 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/config.py
+-rw-r--r--   0        0        0     2023 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/testing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/__init__.py
+-rw-r--r--   0        0        0    14504 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/conftest.py
+-rw-r--r--   0        0        0     1589 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/test_casting.py
+-rw-r--r--   0        0        0    10030 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/test_descriptor.py
+-rw-r--r--   0        0        0     3354 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/test_multithreaded_read.py
+-rw-r--r--   0        0        0    15915 2022-11-09 12:37:21.000000 arcae-0.2.3/src/arcae/tests/test_pytable.py
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 arcae-0.2.3/tbump.toml
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/manifest/vcpkg.json
+-rw-r--r--   0        0        0    20733 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-ports/casacore/001-casacore-cmake.patch
+-rw-r--r--   0        0        0     1937 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-ports/casacore/portfile.cmake
+-rw-r--r--   0        0        0     1778 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-ports/casacore/vcpkg.json
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/arm64-linux-dynamic-cxx17-abi1-dbg.cmake
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/arm64-linux-dynamic-cxx17-abi1-rel.cmake
+-rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/arm64-osx-dynamic-cxx17-abi1-dbg.cmake
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/arm64-osx-dynamic-cxx17-abi1-rel.cmake
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/universal2-osx-dynamic-cxx17-abi1-rel.cmake
+-rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/x64-linux-dynamic-cxx17-abi1-dbg.cmake
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/x64-linux-dynamic-cxx17-abi1-rel.cmake
+-rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/x64-osx-dynamic-cxx17-abi1-dbg.cmake
+-rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 arcae-0.2.3/vcpkg/overlay-triplets/x64-osx-dynamic-cxx17-abi1-rel.cmake
+-rw-r--r--   0        0        0    10564 2022-11-09 12:37:21.000000 arcae-0.2.3/PKG-INFO
```

### Comparing `arcae-0.2.2/.github/workflows/ci.yml` & `arcae-0.2.3/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,86 +7,95 @@
     tags:
     - "*"
   pull_request:
   schedule:
     - cron: '30 2 * * 1,4' # Every Monday and Thursday @ 2h30am UTC
 
 env:
+  CIBW_BUILD_FRONTEND: build
+  CIBW_BEFORE_ALL_LINUX: yum install -y zip flex bison gcc-gfortran
+  # Need to reinstall gcc in order to get gfortran
+  CIBW_BEFORE_ALL_MACOS: |
+    brew install python llvm
+    brew reinstall gcc
+  CIBW_BEFORE_BUILD_MACOS: |
+    export PATH="/opt/homebrew/opt/llvm/bin:$PATH"
+    export LDFLAGS="-L/opt/homebrew/opt/llvm/lib"
+    export CPPFLAGS="-I/opt/homebrew/opt/llvm/include"
+  CIBW_MANYLINUX_X86_64_IMAGE: quay.io/pypa/manylinux_2_28_x86_64
+  CIBW_TEST_EXTRAS_LINUX: applications,test
+  CIBW_TEST_COMMAND_LINUX: py.test -s -vvv --pyargs arcae
+  CIBW_TEST_COMMAND_MACOS: python -c "from arcae.testing import sanity; sanity()"
+
+  HOST_PYTHON_VERSION: "3.10"
   VCPKG_INSTALLED_DIR: /tmp/vcpkg_installed
-  ARTIFACT_NAME: distribution
+  ARTIFACT_NAME: wheel
 
 jobs:
   build-sdist:
     name: Build Source Distribution
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[skip ci]')"
-    strategy:
-      matrix:
-        python: ["3.8"]
     steps:
-      - name: Set up Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+      - name: Set up Python ${{ env.HOST_PYTHON_VERSION }}
+        uses: actions/setup-python@v5
         with:
-          python-version: ${{ matrix.python }}
+          python-version: ${{ env.HOST_PYTHON_VERSION }}
 
       - name: Upgrade pip and install build
         run: python -m pip install -U pip build
 
       - name: Checkout source
         uses: actions/checkout@v4
 
       - name: Build source distribution
         run: python -m build --sdist
 
       - name: Upload wheel artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: ${{ env.ARTIFACT_NAME }}
+          name: ${{ env.ARTIFACT_NAME }}-source
           path: ./dist/*.tar.gz
 
   cpp-tests:
     name: Execute C++ test cases
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[skip ci]')"
     strategy:
       fail-fast: false
-      matrix:
-        triplet:
-          - x64-linux-dynamic-cxx17-abi1-rel
+
+    env:
+      VCPKG_TARGET_TRIPLET: "x64-linux-dynamic-cxx17-abi1-rel"
 
     steps:
       - name: Checkout source
         uses: actions/checkout@v4
 
-      - name: Set up Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+      - name: Set up Python ${{ env.HOST_PYTHON_VERSION }}
+        uses: actions/setup-python@v5
         with:
-          python-version: ${{ matrix.python }}
+          python-version: ${{ env.HOST_PYTHON_VERSION }}
+
+      - name: Expose GitHub Runtime
+        uses: crazy-max/ghaction-github-runtime@v3
 
       - name: List directory structure
         run: tree
 
       - name: Install C++ Compiler and cmake
         run: |
           sudo apt update
           sudo apt install build-essential cmake
           python -m pip install -U pip
           python -m pip install pyarrow
 
-      - name: Get Github Action Cache Variables
-        uses: actions/github-script@v6
-        with:
-          script: |
-            core.exportVariable('ACTIONS_CACHE_URL', process.env.ACTIONS_CACHE_URL || '');
-            core.exportVariable('ACTIONS_RUNTIME_TOKEN', process.env.ACTIONS_RUNTIME_TOKEN || '');
-
       - name: Build C++ libraries and tests
         env:
           VCPKG_BINARY_SOURCES: clear;x-gha,readwrite
-          VCPKG_TARGET_TRIPLET: ${{ matrix.triplet }}
+          VCPKG_TARGET_TRIPLET: ${{ env.VCPKG_TARGET_TRIPLET }}
         run: |
           cmake -S . -B build
           cmake --build build
 
       - name: Execute C++ tests
         run: |
           cd build
@@ -95,88 +104,123 @@
       # - name: Debug with tmate on failure
       #   if: ${{ failure() }}
       #   uses: mxschmitt/action-tmate@v3
 
 
   build-wheels:
     name: Build and Test Binary Wheels
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     if: "!contains(github.event.head_commit.message, '[skip ci]')"
     strategy:
       fail-fast: false
       matrix:
+        os: ["ubuntu-22.04", "macos-13", "macos-14"]
         # https://peps.python.org/pep-0425
-        python:
-          # python version, cpython tag
-          - ["3.8", "cp38"]
-          - ["3.9", "cp39"]
-          - ["3.10", "cp310"]
-          - ["3.11", "cp311"]
-        platform:
-          # platform tag, manylinux tag, vcpkg triplet
-          - [manylinux_x86_64, manylinux_2_28, x64-linux-dynamic-cxx17-abi1-rel]
-
+        cpython: ["cp39", "cp310", "cp311", "cp312"]
+        is_main:
+          - ${{ contains(github.ref, 'main') }}
+        # Avoid building all wheels in a PR
+        exclude:
+          - is_main: false
+            cpython: cp39
+          - is_main: false
+            cpython: cp310
+          - is_main: false
+            cpython: cp312
+        include:
+          - os: ubuntu-22.04
+            os_short: linux
+            arch: "x86_64"
+            triplet: "x64-linux-dynamic-cxx17-abi1-rel"
+            extra_build: "manylinux_x86_64"
+          - os: macos-13
+            os_short: macos
+            arch: "x86_64"
+            triplet: "x64-osx-dynamic-cxx17-abi1-rel"
+            extra_build: "macosx_x86_64"
+          - os: macos-14
+            os_short: macos
+            arch: "arm64"
+            triplet: "arm64-osx-dynamic-cxx17-abi1-rel"
+            extra_build: "macosx_arm64"
     steps:
-      - name: Set up Python ${{ matrix.python[0] }}
-        uses: actions/setup-python@v4
+      - name: Set up Python ${{ env.HOST_PYTHON_VERSION }}
+        uses: actions/setup-python@v5
         with:
-          python-version: ${{ matrix.python[0] }}
+          python-version: ${{ env.HOST_PYTHON_VERSION }}
 
       - name: Upgrade pip and install virtualenv
         run: python -m pip install -U pip virtualenv
 
       - name: Checkout source
         uses: actions/checkout@v4
 
-      - name: Get Github Action Cache Variables
-        uses: actions/github-script@v6
-        with:
-          script: |
-            core.exportVariable('ACTIONS_CACHE_URL', process.env.ACTIONS_CACHE_URL || '');
-            core.exportVariable('ACTIONS_RUNTIME_TOKEN', process.env.ACTIONS_RUNTIME_TOKEN || '');
+      - name: Expose GitHub Runtime
+        uses: crazy-max/ghaction-github-runtime@v3
 
-      - name: Run cibuildwheel
-        uses: pypa/cibuildwheel@v2.13.1
+      - name: Set Common Build Environment Variable
         env:
-          CIBW_BUILD: ${{ matrix.python[1] }}-${{ matrix.platform[0] }}
-          CIBW_BUILD_FRONTEND: build
-          CIBW_BEFORE_ALL_LINUX: yum install -y zip flex bison gcc-gfortran
-          CIBW_MANYLINUX_X86_64_IMAGE: quay.io/pypa/${{ matrix.platform[1] }}_x86_64
-          CIBW_ENVIRONMENT_LINUX: >
+          COMMON_ENV: >
             CMAKE_ARGS=-DBUILD_TESTING=OFF
             ACTIONS_CACHE_URL=${{ env.ACTIONS_CACHE_URL }}
             ACTIONS_RUNTIME_TOKEN=${{ env.ACTIONS_RUNTIME_TOKEN }}
             VCPKG_BINARY_SOURCES="clear;x-gha,readwrite"
-            VCPKG_TARGET_TRIPLET=${{ matrix.platform[2] }}
+            VCPKG_TARGET_TRIPLET=${{ matrix.triplet }}
             VCPKG_INSTALLED_DIR=${{ env.VCPKG_INSTALLED_DIR }}
-            LD_LIBRARY_PATH=${{ env.VCPKG_INSTALLED_DIR }}/${{ matrix.platform[2] }}/lib
+            LD_LIBRARY_PATH=${{ env.VCPKG_INSTALLED_DIR }}/${{ matrix.triplet }}/lib
+        run: echo "CIBW_ENVIRONMENT_COMMON=$COMMON_ENV" >> $GITHUB_ENV
+
+      - name: Run cibuildwheel
+        uses: pypa/cibuildwheel@v2.17
+        env:
+          CIBW_BUILD: ${{ matrix.cpython }}-${{ matrix.extra_build }}*
+          CIBW_ARCHS: ${{ matrix.arch }}
+          CIBW_ENVIRONMENT_LINUX: ${{ env.CIBW_ENVIRONMENT_COMMON }}
+          CIBW_ENVIRONMENT_MACOS: >
+            ${{ env.CIBW_ENVIRONMENT_COMMON }}
+            MACOSX_DEPLOYMENT_TARGET=11.0
           CIBW_REPAIR_WHEEL_COMMAND_LINUX: >
-            auditwheel repair -w {dest_dir} {wheel} --exclude libarrow_python.so --exclude libarrow.so.1400
-          CIBW_TEST_EXTRAS: test
-          CIBW_TEST_COMMAND: py.test -s -vvv --pyargs arcae
+            auditwheel repair
+            -w {dest_dir} {wheel}
+            --exclude libarrow_python.so
+            --exclude libarrow.so.1500
+          CIBW_REPAIR_WHEEL_COMMAND_MACOS: |
+            DYLD_LIBRARY_PATH=$LD_LIBRARY_PATH delocate-listdeps {wheel}
+            DYLD_LIBRARY_PATH=$LD_LIBRARY_PATH delocate-wheel \
+              --require-archs {delocate_archs} \
+              -w {dest_dir} \
+              -v {wheel} \
+              --exclude libarrow_python.dylib \
+              --exclude libarrow.1500.dylib \
+              --ignore-missing-dependencies
 
       - name: Upload wheel artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: ${{ env.ARTIFACT_NAME }}
+          name: ${{ env.ARTIFACT_NAME }}-${{ matrix.os_short }}-${{ matrix.cpython }}-${{ matrix.arch }}
           path: ./wheelhouse/*.whl
 
+      # - name: Debug with tmate on failure
+      #   if: ${{ failure() }}
+      #   uses: mxschmitt/action-tmate@v3
+
   upload-to-test-pypi:
     name: Upload release to Test PyPI
     needs: [build-sdist, build-wheels]
     runs-on: ubuntu-latest
     environment:
       name: release-test
     permissions:
       id-token: write
     steps:
       - name: Download distribution artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
-          name: ${{ env.ARTIFACT_NAME }}
+          pattern: ${{ env.ARTIFACT_NAME }}-*
+          merge-multiple: true
           path: dist
 
       - name: List artifacts
         run: ls -lh dist
 
       - name: Publish package distributions to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
@@ -192,17 +236,18 @@
     runs-on: ubuntu-latest
     environment:
       name: release
     permissions:
       id-token: write
     steps:
       - name: Download distribution artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
-          name: ${{ env.ARTIFACT_NAME }}
+          pattern: ${{ env.ARTIFACT_NAME }}-*
+          merge-multiple: true
           path: dist
 
       - name: List artifacts
         run: ls -lh dist
 
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `arcae-0.2.2/.gitignore` & `arcae-0.2.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -175,7 +175,10 @@
 # ruff
 .ruff_cache/
 
 # LSP config files
 pyrightconfig.json
 
 # End of https://www.toptal.com/developers/gitignore/api/python
+
+# Casa tables
+*.table
```

### Comparing `arcae-0.2.2/HISTORY.rst` & `arcae-0.2.3/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 =======
 History
 =======
 
+0.2.3 (2024-18-04)
+------------------
+* Remove unused utility code (:pr:`90`)
+* Upgrade to pyarrow 15.0.2 (:pr:`89`)
+* Fix python 3.9 typing (:pr:`87`, :pr:`88`)
+* Support table lock options (:pr:`86`)
+* Support complex indexing (:pr:`65`)
+* Configure dependabot (:pr:`85`)
+* Enable dependabot version updates (:pr:`84`)
+* Upgrade to cibuildwheel 2.17 (:pr:`83`)
+* Upgrade to pyarrow 15.0.0 (:pr:`76`)
+* Build linux arm64 and macos arm64/x86_64 wheels (:pr:`76`)
+* Upgrade vcpkg version to include wcslib 8.2.1 (:pr:`82`)
+* Export compile_commands.json by default (:pr:`81`)
+* Make export application dependencies optional (:pr:`80`)
+* Fix ENV access within cmake files (:pr:`79`)
+
 0.2.2 (2023-11-10)
 ------------------
+* Upgrade to pyarrow 14.0.1 (:pr:`77`)
 * Remove WITH_SOABI workaround (:pr:`75`)
 * Add test case demonstrating the feasibility of parallel writes to
   Tiled Storage Manager Columns (:pr:`69`)
 * Update README.rst to show that it is possible to convert
   unconstrained columns (ndim==-1) whose rows have the same rank (:pr:`74`)
 * Guard against python-casacore imports (:pr:`73`)
```

### Comparing `arcae-0.2.2/LICENSE` & `arcae-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cmake_modules/FindPyArrow.cmake` & `arcae-0.2.3/cmake_modules/FindPyArrow.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 include(FindPython3)
 
 find_package(Python COMPONENTS Interpreter)
-message("Python ${Python_EXECUTABLE}")
+message("Python_EXECUABLE=${Python_EXECUTABLE}")
+message("Python_ROOT_DIR=${Python_ROOT_DIR}")
 
 if(NOT DEFINED NUMPY_INCLUDE AND DEFINED ENV{NUMPY_INCLUDE})
-    set(NUMPY_INCLUDE ENV{NUMPY_INCLUDE})
+    set(NUMPY_INCLUDE $ENV{NUMPY_INCLUDE})
 endif()
 
 if(NOT DEFINED NUMPY_INCLUDE AND Python_Interpreter_FOUND)
     execute_process(COMMAND ${Python_EXECUTABLE} -c "import numpy; print(numpy.get_include())"
         OUTPUT_VARIABLE NUMPY_INCLUDE
         OUTPUT_STRIP_TRAILING_WHITESPACE)
 endif()
 
 if(NOT DEFINED NUMPY_INCLUDE)
     message(FATAL_ERROR "Unable to find numpy include directory. Set NUMPY_INCLUDE")
 endif()
 
 
 if(NOT DEFINED PYARROW_INCLUDE AND DEFINED ENV{PYARROW_INCLUDE})
-    set(PYARROW_INCLUDE ENV{PYARROW_INCLUDE})
+    set(PYARROW_INCLUDE $ENV{PYARROW_INCLUDE})
 endif()
 
 execute_process(COMMAND ${Python_EXECUTABLE} -c "import pyarrow; pyarrow.create_library_symlinks()")
 
 if(NOT DEFINED PYARROW_INCLUDE AND Python_Interpreter_FOUND)
     execute_process(COMMAND ${Python_EXECUTABLE} -c "import pyarrow; print(pyarrow.get_include())"
                     OUTPUT_VARIABLE PYARROW_INCLUDE
@@ -31,29 +32,29 @@
 endif()
 
 if(NOT DEFINED PYARROW_INCLUDE)
     message(FATAL_ERROR "Unable to find pyarrow include directory. Set PYARROW_INCLUDE")
 endif()
 
 if(NOT DEFINED PYARROW_LIBDIRS AND DEFINED ENV{PYARROW_LIBDIRS})
-    set(PYARROW_LIBDIRS ENV{PYARROW_LIBDIRS})
+    set(PYARROW_LIBDIRS $ENV{PYARROW_LIBDIRS})
 endif()
 
 if(NOT DEFINED PYARROW_LIBDIRS AND Python_Interpreter_FOUND)
     execute_process(COMMAND ${Python_EXECUTABLE} -c "import pyarrow; print(' '.join(pyarrow.get_library_dirs()))"
                     OUTPUT_VARIABLE PYARROW_LIBDIRS
                     OUTPUT_STRIP_TRAILING_WHITESPACE)
 endif()
 
 if(NOT DEFINED PYARROW_LIBDIRS)
     message(FATAL_ERROR "Unable to find pyarrow library directories. Set PYARROW_LIBDIRS")
 endif()
 
 if(NOT DEFINED PYARROW_LIBS AND DEFINED ENV{PYARROW_LIBS})
-    set(PYARROW_LIBS ENV{PYARROW_LIBS})
+    set(PYARROW_LIBS $ENV{PYARROW_LIBS})
 endif()
 
 if(NOT DEFINED PYARROW_LIBS AND Python_Interpreter_FOUND)
     execute_process(COMMAND ${Python_EXECUTABLE} -c "import pyarrow; print(' '.join(pyarrow.get_libraries()))"
                     OUTPUT_VARIABLE PYARROW_LIBS
                     OUTPUT_STRIP_TRAILING_WHITESPACE)
 endif()
```

### Comparing `arcae-0.2.2/cmake_modules/SetupVCPKG.cmake` & `arcae-0.2.3/cmake_modules/SetupVCPKG.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -19,49 +19,52 @@
     message(FATAL_ERROR "Unable to find VCPKG_SHA256=version in ${CMAKE_SOURCE_DIR}/.env")
 endif()
 
 set(VCPKG_HASH ${CMAKE_MATCH_1})
 
 # Discover or infer the source directory where vcpkg will be decompressed
 if(DEFINED ENV{VCPKG_SOURCE_DIR})
-    set(VCPKG_SOURCE_DIR "$ENV{VCPKG_SOURCE_DIR}")
+    set(VCPKG_SOURCE_DIR $ENV{VCPKG_SOURCE_DIR})
 else()
-    set(VCPKG_SOURCE_DIR "${CMAKE_SOURCE_DIR}/vcpkg/source")
+    set(VCPKG_SOURCE_DIR ${CMAKE_SOURCE_DIR}/vcpkg/source)
 endif()
 
 # Download and decompress vcpkg
 FetchContent_Declare(vcpkg URL ${VCPKG_URL} URL_HASH SHA256=${VCPKG_HASH} SOURCE_DIR ${VCPKG_SOURCE_DIR})
 FetchContent_MakeAvailable(vcpkg)
 
 # Discover or infer vcpkg's installation directory
 if(DEFINED ENV{VCPKG_INSTALLED_DIR})
     set(VCPKG_INSTALLED_DIR $ENV{VCPKG_INSTALLED_DIR})
 else()
-    set(VCPKG_INSTALLED_DIR "${CMAKE_SOURCE_DIR}/vcpkg/installed")
+    set(VCPKG_INSTALLED_DIR ${CMAKE_SOURCE_DIR}/vcpkg/installed)
 endif()
 
 # Set the vcpkg manifest directory and toolchain
-set(VCPKG_MANIFEST_DIR "${CMAKE_SOURCE_DIR}/vcpkg/manifest")
-set(CMAKE_TOOLCHAIN_FILE "${vcpkg_SOURCE_DIR}/scripts/buildsystems/vcpkg.cmake" CACHE FILEPATH "")
+set(VCPKG_MANIFEST_DIR ${CMAKE_SOURCE_DIR}/vcpkg/manifest)
+set(CMAKE_TOOLCHAIN_FILE ${vcpkg_SOURCE_DIR}/scripts/buildsystems/vcpkg.cmake CACHE FILEPATH "")
 
-set(VCPKG_OVERLAY_TRIPLETS "${CMAKE_SOURCE_DIR}/vcpkg/overlay-triplets")
-set(VCPKG_OVERLAY_PORTS "${CMAKE_SOURCE_DIR}/vcpkg/overlay-ports/casacore")
+set(VCPKG_OVERLAY_TRIPLETS ${CMAKE_SOURCE_DIR}/vcpkg/overlay-triplets)
+set(VCPKG_OVERLAY_PORTS ${CMAKE_SOURCE_DIR}/vcpkg/overlay-ports/casacore)
 
 # Discover or infer the vcpkg target triplet
 if(DEFINED ENV{VCPKG_TARGET_TRIPLET})
     set(VCPKG_TARGET_TRIPLET $ENV{VCPKG_TARGET_TRIPLET})
 else()
     if(UNIX)
         set(VCPKG_TARGET_TRIPLET "x64-linux-dynamic-cxx17-abi1-rel")
     else()
         message(FATAL_ERROR "Only unix currently supported")
     endif()
 endif()
 
+set(VCPKG_LIBDIRS "${VCPKG_INSTALLED_DIR}/${VCPKG_TARGET_TRIPLET}/lib")
+
 message("CMAKE_TOOLCHAIN_FILE: ${CMAKE_TOOLCHAIN_FILE}")
 message("VCPKG_SOURCE_DIR: ${VCPKG_SOURCE_DIR}")
 message("VCPKG_INSTALLED_DIR: ${VCPKG_INSTALLED_DIR}")
 message("VCPKG_MANIFEST_DIR: ${VCPKG_MANIFEST_DIR}")
 message("CMAKE_TOOLCHAIN_FILE: ${CMAKE_TOOLCHAIN_FILE}")
 message("VCPKG_OVERLAY_TRIPLETS: ${VCPKG_OVERLAY_TRIPLETS}")
 message("VCPKG_OVERLAY_PORTS: ${VCPKG_OVERLAY_PORTS}")
 message("VCPKG_TARGET_TRIPLET: ${VCPKG_TARGET_TRIPLET}")
+message("VCPKG_LIBDIRS: ${VCPKG_LIBDIRS}")
```

### Comparing `arcae-0.2.2/cpp/arcae/casa_visitors.h` & `arcae-0.2.3/cpp/arcae/casa_visitors.h`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cpp/arcae/column_convert_visitor.cc` & `arcae-0.2.3/cpp/arcae/column_write_visitor.cc`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,198 @@
+#include "arcae/column_write_visitor.h"
+
+#include <memory>
+
 #include <arrow/api.h>
+#include <arrow/compute/cast.h>
+#include <arrow/result.h>
+#include <arrow/status.h>
+#include <arrow/type.h>
 
+#include <casacore/casa/Utilities/DataType.h>
 #include <casacore/tables/Tables.h>
 
-#include "arcae/column_convert_visitor.h"
 #include "arcae/complex_type.h"
 
-using ::arrow::DataType;
-using ::arrow::Buffer;
-using ::arrow::Result;
-using ::arrow::Status;
-
 namespace arcae {
 
-ColumnConvertVisitor::ColumnConvertVisitor(
-    const casacore::TableColumn & column,
-    casacore::uInt startrow,
-    casacore::uInt nrow,
-    arrow::MemoryPool * pool)
-    : column_(column),
-      startrow_(startrow),
-      nrow_(nrow),
-      endrow_(startrow + nrow),
-      column_desc_(column.columnDesc()),
-      pool_(pool) {
-
-    assert(endrow_ <= column.nrow());
+const std::map<casacore::DataType, std::shared_ptr<arrow::DataType>>
+ColumnWriteVisitor::arrow_type_map_ = {
+    {casacore::TpBool, arrow::uint8()},
+    {casacore::TpChar, arrow::int8()},
+    {casacore::TpUChar, arrow::uint8()},
+    {casacore::TpShort, arrow::int16()},
+    {casacore::TpUShort, arrow::uint16()},
+    {casacore::TpInt, arrow::int32()},
+    {casacore::TpUInt, arrow::uint32()},
+    {casacore::TpInt64, arrow::int64()},
+    {casacore::TpFloat, arrow::float32()},
+    {casacore::TpDouble, arrow::float64()},
+    {casacore::TpComplex, complex64()},
+    {casacore::TpDComplex, complex128()},
+    {casacore::TpString, arrow::utf8()}
+};
+
+
+arrow::Status ColumnWriteVisitor::Visit() {
+    return CasaTypeVisitor::Visit(map_.get().column_.get().columnDesc().dataType());
 }
 
 
-Status ColumnConvertVisitor::ValidateArray(const std::shared_ptr<arrow::Array> & array) {
-    auto & config = ServiceLocator::configuration();
-    auto validation_level = config.GetDefault("validation-level", "basic");
-
-    if(validation_level == "basic") {
-        return array->Validate();
-    } else if(validation_level == "full") {
-        return array->ValidateFull();
-    } else if(validation_level == "none") {
-        return Status::OK();
-    } else {
-        ARROW_LOG(WARNING) << "Invalid validation-level=" << validation_level
-                            << ". No array construction validation will be performed";
-        return Status::OK();
+arrow::Result<std::shared_ptr<arrow::Array>>
+ColumnWriteVisitor::GetFlatArray(bool nulls) const {
+    auto data = map_.get().data_;
+
+    if(!nulls && data->null_count() > 0) {
+        return arrow::Status::Invalid("Null values were encountered "
+                                      "during array flattening.");
+    }
+
+    while(true) {
+        switch(data->type_id()) {
+            case arrow::Type::LARGE_LIST:
+            {
+                auto lla = std::dynamic_pointer_cast<arrow::LargeListArray>(data);
+                ARROW_ASSIGN_OR_RAISE(data, lla->Flatten(pool_));
+                break;
+            }
+            case arrow::Type::LIST:
+            {
+                auto la = std::dynamic_pointer_cast<arrow::ListArray>(data);
+                ARROW_ASSIGN_OR_RAISE(data, la->Flatten(pool_));
+                break;
+            }
+            case arrow::Type::FIXED_SIZE_LIST:
+            {
+                auto fsl = std::dynamic_pointer_cast<arrow::FixedSizeListArray>(data);
+                ARROW_ASSIGN_OR_RAISE(data, fsl->Flatten(pool_));
+                break;
+            }
+            case arrow::Type::BOOL:
+            case arrow::Type::UINT8:
+            case arrow::Type::UINT16:
+            case arrow::Type::UINT32:
+            case arrow::Type::UINT64:
+            case arrow::Type::INT8:
+            case arrow::Type::INT16:
+            case arrow::Type::INT32:
+            case arrow::Type::INT64:
+            case arrow::Type::FLOAT:
+            case arrow::Type::DOUBLE:
+            case arrow::Type::STRING:
+                return data;
+            default:
+                return arrow::Status::TypeError(
+                    "Flattening of type ", data->type(),
+                    " is not supported");
+        }
     }
 }
 
 
-Result<std::shared_ptr<arrow::Array>>
-ColumnConvertVisitor::MakeArrowPrimitiveArray(
-        const std::shared_ptr<Buffer> & buffer,
-        casacore::uInt nelements,
-        const std::shared_ptr<DataType> & arrow_dtype) {
-
-    if(auto complex_dtype = std::dynamic_pointer_cast<ComplexType>(arrow_dtype)) {
-        auto child_array = std::make_shared<arrow::PrimitiveArray>(
-            complex_dtype->value_type(), 2*nelements, buffer);
-
-        auto & config = ServiceLocator::configuration();
-        auto convert_strategy = config.GetDefault("casa.convert.strategy", "fixed");
-        auto npos = std::string::npos;
-
-        if(auto pos = convert_strategy.find("complex"); pos != npos) {
-            // NOTE(sjperkins)
-            // Check the FixedSizeListAray layout documents
-            // https://arrow.apache.org/docs/format/Columnar.html#fixed-size-list-layout
-            // A single empty buffer {nullptr} must be provided otherwise this segfaults
-            auto array_data = arrow::ArrayData::Make(
-                complex_dtype, nelements, {nullptr}, {child_array->data()});
-            return complex_dtype->MakeArray(std::move(array_data));
-        } else if(auto pos = convert_strategy.find("fixed"); pos == 0) {
-            return arrow::FixedSizeListArray::FromArrays(child_array, 2);
-        } else if(auto pos = convert_strategy.find("list"); pos == 0) {
-            arrow::Int32Builder builder(pool_);
-            ARROW_RETURN_NOT_OK(builder.Reserve(nelements + 1));
-            for(decltype(nelements) i=0; i < nelements + 1; ++i)
-                { ARROW_RETURN_NOT_OK(builder.Append(2*i)); }
-            ARROW_ASSIGN_OR_RAISE(auto offsets, builder.Finish());
-            return arrow::ListArray::FromArrays(*offsets, *child_array);
-        } else {
-            return arrow::Status::Invalid("Invalid 'casa.convert.strategy=", convert_strategy, "'");
+arrow::Result<std::shared_ptr<arrow::Array>>
+ColumnWriteVisitor::MaybeCastFlatArray(const std::shared_ptr<arrow::Array> & data) {
+    auto casa_dtype = map_.get().column_.get().columnDesc().dataType();
+
+    if(auto kv = arrow_type_map_.find(casa_dtype); kv != arrow_type_map_.end()) {
+        auto arrow_dtype = kv->second;
+
+        if(auto ct = std::dynamic_pointer_cast<ComplexFloatType>(arrow_dtype); ct) {
+            arrow_dtype = arrow::float32();
+        } else if (auto ct = std::dynamic_pointer_cast<ComplexDoubleType>(arrow_dtype); ct) {
+            arrow_dtype = arrow::float64();
+        }
+
+        // Types match, don't cast
+        if(data->type() == arrow_dtype) {
+            return data;
         }
-    } else {
-        return std::make_shared<arrow::PrimitiveArray>(arrow_dtype, nelements, buffer);
+
+        ARROW_ASSIGN_OR_RAISE(auto datum, arrow::compute::Cast(data, arrow_dtype));
+        return datum.make_array();
     }
+
+    return arrow::Status::TypeError(casa_dtype, " does not map to an arrow type");
+}
+
+
+
+arrow::Status
+ColumnWriteVisitor::CheckElements(std::size_t map_size, std::size_t data_size) const {
+    if(map_size == data_size) return arrow::Status::OK();
+    return arrow::Status::Invalid("Number of map elements ", map_size, " does not "
+                                    "match the length of the array ", data_size);
+}
+
+arrow::Status
+ColumnWriteVisitor::FailIfNotUTF8(const std::shared_ptr<arrow::DataType> & arrow_dtype) const {
+    if(arrow_dtype == arrow::utf8()) { return arrow::Status::OK(); }
+    return arrow::Status::Invalid(arrow_dtype->ToString(), " incompatible with casacore::String");
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpBool() {
+arrow::Status ColumnWriteVisitor::VisitTpBool() {
     // TODO(sjperkins)
     // Looks like casacore bool is actually a char, improve this
-    return this->ConvertColumn<casacore::Bool>(arrow::uint8());
+    return this->WriteColumn<casacore::Bool>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpChar() {
-    return this->ConvertColumn<casacore::Char>(arrow::int8());
+arrow::Status ColumnWriteVisitor::VisitTpChar() {
+    return this->WriteColumn<casacore::Char>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpUChar() {
-    return this->ConvertColumn<casacore::uChar>(arrow::uint8());
+arrow::Status ColumnWriteVisitor::VisitTpUChar() {
+    return this->WriteColumn<casacore::uChar>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpShort() {
-    return this->ConvertColumn<casacore::Short>(arrow::int16());
+arrow::Status ColumnWriteVisitor::VisitTpShort() {
+    return this->WriteColumn<casacore::Short>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpUShort() {
-    return this->ConvertColumn<casacore::uShort>(arrow::uint16());
+arrow::Status ColumnWriteVisitor::VisitTpUShort() {
+    return this->WriteColumn<casacore::uShort>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpInt() {
-    return this->ConvertColumn<casacore::Int>(arrow::int32());
+arrow::Status ColumnWriteVisitor::VisitTpInt() {
+    return this->WriteColumn<casacore::Int>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpUInt() {
-    return this->ConvertColumn<casacore::uInt>(arrow::uint32());
+arrow::Status ColumnWriteVisitor::VisitTpUInt() {
+    return this->WriteColumn<casacore::uInt>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpInt64() {
-    return this->ConvertColumn<casacore::Int64>(arrow::int64());
+arrow::Status ColumnWriteVisitor::VisitTpInt64() {
+    return this->WriteColumn<casacore::Int64>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpFloat() {
-    return this->ConvertColumn<casacore::Float>(arrow::float32());
+arrow::Status ColumnWriteVisitor::VisitTpFloat() {
+    return this->WriteColumn<casacore::Float>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpDouble() {
-    return this->ConvertColumn<casacore::Double>(arrow::float64());
+arrow::Status ColumnWriteVisitor::VisitTpDouble() {
+    return this->WriteColumn<casacore::Double>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpComplex() {
-    return this->ConvertColumn<casacore::Complex>(complex64());
+arrow::Status ColumnWriteVisitor::VisitTpComplex() {
+    return this->WriteColumn<casacore::Complex>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpDComplex() {
-    return this->ConvertColumn<casacore::DComplex>(complex128());
+arrow::Status ColumnWriteVisitor::VisitTpDComplex() {
+    return this->WriteColumn<casacore::DComplex>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpString() {
-    return this->ConvertColumn<casacore::String>(arrow::utf8());
+arrow::Status ColumnWriteVisitor::VisitTpString() {
+    return this->WriteColumn<casacore::String>();
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpQuantity() {
+arrow::Status ColumnWriteVisitor::VisitTpQuantity() {
     return arrow::Status::NotImplemented("TpQuantity");
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpRecord() {
+arrow::Status ColumnWriteVisitor::VisitTpRecord() {
     return arrow::Status::NotImplemented("TpRecord");
 }
 
-arrow::Status ColumnConvertVisitor::VisitTpTable() {
+arrow::Status ColumnWriteVisitor::VisitTpTable() {
     return arrow::Status::NotImplemented("TpTable");
 }
 
 } // namespace arcae
```

### Comparing `arcae-0.2.2/cpp/arcae/column_convert_visitor.h` & `arcae-0.2.3/cpp/arcae/column_write_visitor.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,400 +1,290 @@
-#ifndef ARCAE_COLUMN_CONVERT_VISITOR_H
-#define ARCAE_COLUMN_CONVERT_VISITOR_H
-
-#include <algorithm>
-#include <unordered_set>
+#ifndef COLUMN_WRITE_VISITOR_H
+#define COLUMN_WRITE_VISITOR_H
 
+#include <functional>
+#include <map>
+#include <memory>
+#include <type_traits>
+
+#include <arrow/array.h>
+#include <arrow/result.h>
+#include <arrow/status.h>
+#include <arrow/type.h>
+
+#include <casacore/casa/aipstype.h>
+#include <casacore/casa/aipsxtype.h>
+#include <casacore/casa/BasicSL/String.h>
+#include <casacore/casa/Exceptions/Error.h>
+#include <casacore/casa/Utilities/DataType.h>
 #include <casacore/tables/Tables.h>
 
-#include <arrow/util/logging.h>  // IWYU pragma: keep
-
 #include "arcae/casa_visitors.h"
-#include "arcae/complex_type.h"
-#include "arcae/service_locator.h"
-#include "arcae/utility.h"
+#include "arcae/column_write_map.h"
 
 namespace arcae {
 
-class ColumnConvertVisitor : public CasaTypeVisitor {
-public:
-    using ShapeVectorType = std::vector<casacore::IPosition>;
+class ColumnWriteVisitor : public CasaTypeVisitor {
+private:
+    // Map of casacore datatypes to arrow datatypes
+    static const std::map<casacore::DataType, std::shared_ptr<arrow::DataType>> arrow_type_map_;
 
 public:
-    const casacore::TableColumn & column_;
-    const casacore::ColumnDesc & column_desc_;
-    casacore::uInt startrow_;
-    casacore::uInt endrow_;
-    casacore::uInt nrow_;
-    std::shared_ptr<arrow::Array> array_;
+    std::reference_wrapper<const ColumnWriteMap> map_;
     arrow::MemoryPool * pool_;
 
 public:
-    explicit ColumnConvertVisitor(
-        const casacore::TableColumn & column,
-        casacore::uInt startrow,
-        casacore::uInt nrow,
-        arrow::MemoryPool * pool=arrow::default_memory_pool());
-    virtual ~ColumnConvertVisitor() = default;
+    explicit ColumnWriteVisitor(
+        const ColumnWriteMap & column_map,
+        arrow::MemoryPool * pool=arrow::default_memory_pool()) :
+            map_(std::cref(column_map)),
+            pool_(pool) {};
+    virtual ~ColumnWriteVisitor() = default;
+
 
 #define VISIT(CASA_TYPE) \
     virtual arrow::Status Visit##CASA_TYPE() override;
 
     VISIT_CASA_TYPES(VISIT)
 #undef VISIT
 
-private:
+    arrow::Status Visit();
+    arrow::Result<std::shared_ptr<arrow::Array>> MaybeCastFlatArray(const std::shared_ptr<arrow::Array> & data);
 
-    static arrow::Status ValidateArray(const std::shared_ptr<arrow::Array> & array);
 
-    inline casacore::uInt local_row(casacore::uInt row)
-        { assert(row >= startrow_); return row - startrow_; }
+    // Write arrow array to the CASA column
+    template <typename T>
+    arrow::Status WriteColumn() {
+        try {
+            if(map_.get().nDim() == 1) {
+                return WriteScalarColumn<T>();
+            } else if(map_.get().IsFixedShape()) {
+                return WriteFixedColumn<T>();
+            } else {
+                return WriteVariableColumn<T>();
+            }
+        } catch(casacore::AipsError & e) {
+            return arrow::Status::Invalid("WriteColumn ",
+                                          GetTableColumn().columnDesc().name(),
+                                            ": ", e.what());
+        }
+    }
 
-    inline arrow::Status FailIfNotUTF8(const std::shared_ptr<arrow::DataType> & arrow_dtype) {
-        if(arrow_dtype == arrow::utf8()) { return arrow::Status::OK(); }
-        return arrow::Status::Invalid(arrow_dtype->ToString(), " incompatible with casacore::String");
+private:
+    const casacore::TableColumn & GetTableColumn() const {
+        return map_.get().column_.get();
     }
 
-    arrow::Result<std::shared_ptr<arrow::Array>> MakeArrowPrimitiveArray(
-            const std::shared_ptr<arrow::Buffer> & buffer,
-            casacore::uInt nelements,
-            const std::shared_ptr<arrow::DataType> & arrow_dtype);
+    arrow::Result<std::shared_ptr<arrow::Array>> GetFlatArray(bool nulls=false) const;
+    arrow::Status CheckElements(std::size_t map_size, std::size_t data_size) const;
+    arrow::Status FailIfNotUTF8(const std::shared_ptr<arrow::DataType> & arrow_dtype) const;
 
     template <typename T>
-    arrow::Status ConvertScalarColumn(const std::shared_ptr<arrow::DataType> & arrow_dtype) {
-        auto column = casacore::ScalarColumn<T>(column_);
+    arrow::Status WriteScalarColumn() {
+        auto column = casacore::ScalarColumn<T>(GetTableColumn());
         column.setMaximumCacheSize(1);
-
-        if constexpr(std::is_same<T, casacore::String>::value) {
-            // Handle string cases with Arrow StringBuilders
-            ARROW_RETURN_NOT_OK(FailIfNotUTF8(arrow_dtype));
-            arrow::StringBuilder builder;
-
-            try {
-                auto strings = column.getColumnRange(casacore::Slice(startrow_, nrow_));
-                for(auto & s: strings) { ARROW_RETURN_NOT_OK(builder.Append(s)); }
-            } catch(std::exception & e) {
-                return arrow::Status::Invalid("ConvertScalarColumn ", column_desc_.name(), " ", e.what());
+        auto nelements = map_.get().nElements();
+        ARROW_ASSIGN_OR_RAISE(auto flat_array, GetFlatArray());
+        ARROW_ASSIGN_OR_RAISE(flat_array, MaybeCastFlatArray(flat_array));
+
+        if constexpr(std::is_same_v<T, casacore::String>) {
+            auto flat_strings = std::dynamic_pointer_cast<arrow::StringArray>(flat_array);
+            assert(flat_strings != nullptr && "Unable to cast array to StringArray");
+            ARROW_RETURN_NOT_OK(FailIfNotUTF8(flat_strings->type()));
+            ARROW_RETURN_NOT_OK(CheckElements(flat_strings->length(), nelements));
+
+            for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                // Copy sections of data from the Arrow Buffer and write
+                try {
+                    auto carray = casacore::Array<casacore::String>(it.GetShape());
+                    auto * chunk_ptr = carray.data();
+                    for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                        auto sv = flat_strings->GetView(mit.GlobalOffset());
+                        chunk_ptr[mit.ChunkOffset()] = casacore::String(std::begin(sv), std::end(sv));
+                    }
+                    column.putColumnRange(it.GetRowSlicer(), carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteScalarColumn ",
+                                                  GetTableColumn().columnDesc().name(),
+                                                  ": ", e.what());
+                }
             }
-
-            ARROW_ASSIGN_OR_RAISE(array_, builder.Finish());
         } else {
-            // Wrap Arrow Buffer in casacore Vector
-            ARROW_ASSIGN_OR_RAISE(auto allocation, arrow::AllocateBuffer(nrow_*sizeof(T), pool_));
-            auto buffer = std::shared_ptr<arrow::Buffer>(std::move(allocation));
-            auto * buf_ptr = reinterpret_cast<T *>(buffer->mutable_data());
-            auto casa_vector = casacore::Vector<T>(casacore::IPosition(1, nrow_), buf_ptr, casacore::SHARE);
-
-            // Dump column data into Arrow Buffer
-            try {
-                column.getColumnRange(casacore::Slice(startrow_, nrow_), casa_vector);
-            } catch(std::exception & e) {
-                return arrow::Status::Invalid("ConvertScalarColumn ", column_desc_.name(), " ", e.what());
+            // Get Arrow Array buffer
+            ARROW_ASSIGN_OR_RAISE(auto shape, map_.get().GetOutputShape());
+            auto span = flat_array->data()->buffers[1]->span_as<T>();
+            ARROW_RETURN_NOT_OK(CheckElements(span.size(), nelements));
+
+            if(map_.get().IsSimple()) {
+                auto carray = casacore::Array<T>(shape, std::remove_const_t<T *>(span.data()), casacore::SHARE);
+
+                try {
+                    // Dump column data straight from the Arrow Buffer
+                    column.putColumnRange(map_.get().RangeBegin().GetRowSlicer(),
+                                          carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteScalarColumn ",
+                                                  GetTableColumn().columnDesc().name(),
+                                                  ": ", e.what());
+                }
+            } else {
+                for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                    // Copy sections of data from the Arrow Buffer and write
+                    try {
+                        auto carray = casacore::Array<T>(it.GetShape());
+                        auto chunk_ptr = carray.data();
+                        for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                            chunk_ptr[mit.ChunkOffset()] = span[mit.GlobalOffset()];
+                        }
+                        column.putColumnRange(it.GetRowSlicer(), carray);
+                    } catch(casacore::AipsError & e) {
+                        return arrow::Status::Invalid("WriteScalarColumn ",
+                                                      GetTableColumn().columnDesc().name(),
+                                                      ": ", e.what());
+                    }
+                }
             }
 
-            ARROW_ASSIGN_OR_RAISE(array_, MakeArrowPrimitiveArray(buffer, nrow_, arrow_dtype));
         }
 
-        return ValidateArray(array_);
+        return arrow::Status::OK();
     }
 
     template <typename T>
-    arrow::Status ConvertFixedArrayColumn(const std::shared_ptr<arrow::DataType> & arrow_dtype,
-                                   const casacore::IPosition & shape) {
-        auto column = casacore::ArrayColumn<T>(column_);
+    arrow::Status WriteFixedColumn() {
+        auto column = casacore::ArrayColumn<T>(GetTableColumn());
         column.setMaximumCacheSize(1);
-
-        if constexpr(std::is_same<T, casacore::String>::value) {
-            // Handle string cases with Arrow StringBuilders
-           ARROW_RETURN_NOT_OK(FailIfNotUTF8(arrow_dtype));
-           arrow::StringBuilder builder;
-
-            for(casacore::uInt row=startrow_; row < endrow_; ++row) {
-                auto strings = column.get(row);
-                for(auto & string: strings)
-                    { ARROW_RETURN_NOT_OK(builder.Append(string)); }
-            }
-            ARROW_ASSIGN_OR_RAISE(array_, builder.Finish());
-        } else {
-            // Wrap Arrow Buffer in casacore Array
-            auto array_shape = shape;
-            array_shape.append(casacore::IPosition(1, nrow_));
-            auto nelements = array_shape.product();
-            ARROW_ASSIGN_OR_RAISE(auto allocation, arrow::AllocateBuffer(nelements*sizeof(T), pool_));
-            auto buffer = std::shared_ptr<arrow::Buffer>(std::move(allocation));
-            auto * buf_ptr = reinterpret_cast<T *>(buffer->mutable_data());
-            auto casa_array = casacore::Array<T>(array_shape, buf_ptr, casacore::SHARE);
-
-            // Dump column data into Arrow Buffer
-            try {
-                column.getColumnRange(casacore::Slice(startrow_, nrow_), casa_array);
-            } catch(std::exception & e) {
-                return arrow::Status::Invalid("MakeFixedArrayBuffer ", column_desc_.name(), " ", e.what());
-            }
-
-            ARROW_ASSIGN_OR_RAISE(array_, MakeArrowPrimitiveArray(buffer, nelements, arrow_dtype));
-        }
-
-        // Fortran ordering
-        for(auto dim_size: shape) {
-            ARROW_ASSIGN_OR_RAISE(array_, arrow::FixedSizeListArray::FromArrays(array_, dim_size));
+        ARROW_ASSIGN_OR_RAISE(auto shape, map_.get().GetOutputShape());
+        ARROW_ASSIGN_OR_RAISE(auto flat_array, GetFlatArray());
+        ARROW_ASSIGN_OR_RAISE(flat_array, MaybeCastFlatArray(flat_array));
+        auto nelements = map_.get().nElements();
+
+        if(std::size_t(shape.product()) != nelements) {
+            return arrow::Status::Invalid("Shape ", shape, " elements ", shape.nelements(),
+                                            " doesn't match map elements ", nelements);
         }
 
-        return ValidateArray(array_);
-    }
 
-    template <typename T>
-    arrow::Status ConvertVariableArrayColumn(
-            const std::shared_ptr<arrow::DataType> & arrow_dtype,
-            const std::vector<casacore::IPosition> & shapes,
-            std::shared_ptr<arrow::Buffer> & nulls,
-            int64_t null_counts,
-            casacore::uInt ndim) {
-
-        auto column = casacore::ArrayColumn<T>(column_);
-        column.setMaximumCacheSize(1);
-
-        if constexpr(std::is_same<T, casacore::String>::value) {
-            // Handle string cases with Arrow StringBuilders
-            ARROW_RETURN_NOT_OK(FailIfNotUTF8(arrow_dtype));
-            arrow::StringBuilder builder;
-
-            for(casacore::uInt row=startrow_; row < endrow_; ++row) {
-                if(arrow::bit_util::GetBit(nulls->data(), local_row(row))) {
-                    auto strings = column.get(row);
-                    for(auto & string: strings) { ARROW_RETURN_NOT_OK(builder.Append(string)); }
+        if constexpr(std::is_same_v<T, casacore::String>) {
+            auto flat_strings = std::dynamic_pointer_cast<arrow::StringArray>(flat_array);
+            assert(flat_strings != nullptr && "Unable to cast array to StringArray");
+            ARROW_RETURN_NOT_OK(FailIfNotUTF8(flat_strings->type()));
+            ARROW_RETURN_NOT_OK(CheckElements(flat_strings->length(), nelements));
+
+            for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                assert(it.GetShape().product() == flat_strings->length());
+                // Copy sections of data from the Arrow Buffer and write
+                try {
+                    auto carray = casacore::Array<casacore::String>(it.GetShape());
+                    auto * chunk_ptr = carray.data();
+                    for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                        auto sv = flat_strings->GetView(mit.GlobalOffset());
+                        chunk_ptr[mit.ChunkOffset()] = casacore::String(std::begin(sv), std::end(sv));
+                    }
+                    column.putColumnRange(it.GetRowSlicer(), it.GetSectionSlicer(), carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteFixedColumn ",
+                                                    GetTableColumn().columnDesc().name(),
+                                                    ": ", e.what());
                 }
             }
-            ARROW_ASSIGN_OR_RAISE(array_, builder.Finish());
         } else {
-            auto nelements = std::accumulate(
-                    shapes.begin(), shapes.end(), casacore::uInt(0),
-                    [](auto i, const auto & s) { return i + s.product(); });
-            ARROW_ASSIGN_OR_RAISE(auto allocation, arrow::AllocateBuffer(nelements*sizeof(T), pool_));
-            auto buffer = std::shared_ptr<arrow::Buffer>(std::move(allocation));
-            auto * buf_ptr = reinterpret_cast<T *>(buffer->mutable_data());
-            casacore::uInt offset = 0;
-
-            // Dump column data into Arrow Buffer
-            for(casacore::uInt row=startrow_; row < endrow_; ++row) {
-                auto lrow = local_row(row);
-                auto product = shapes[lrow].product();
-                if(arrow::bit_util::GetBit(nulls->data(), lrow) && product > 0) {
-                    auto casa_array = casacore::Array<T>(shapes[lrow], buf_ptr + offset, casacore::SHARE);
+            // Get Arrow Array buffer
+            std::shared_ptr<arrow::Buffer> buffer = flat_array->data()->buffers[1];
+            auto span = buffer->span_as<T>();
+            ARROW_RETURN_NOT_OK(CheckElements(span.size(), nelements));
+
+            if(map_.get().IsSimple()) {
+                auto carray = casacore::Array<T>(shape, std::remove_const_t<T *>(span.data()), casacore::SHARE);
+
+                try {
+                    // Dump column data straight into the Arrow Buffer
+                    column.putColumnRange(map_.get().RangeBegin().GetRowSlicer(),
+                                          map_.get().RangeBegin().GetSectionSlicer(),
+                                          carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteFixedColumn ",
+                                                  GetTableColumn().columnDesc().name(),
+                                                  ": ", e.what());
+                }
+            } else {
+                for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                    // Copy sections of data from the Arrow Buffer and write
                     try {
-                        column.get(row, casa_array);
-                    } catch(std::exception & e) {
-                        return arrow::Status::Invalid("ConvertVariableArrayColumn",
-                                                      column_desc_.name(), " ", e.what());
+                        auto carray = casacore::Array<T>(it.GetShape());
+                        auto chunk_ptr = carray.data();
+                        for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                            chunk_ptr[mit.ChunkOffset()] = span[mit.GlobalOffset()];
+                        }
+                        column.putColumnRange(it.GetRowSlicer(), it.GetSectionSlicer(), carray);
+                    } catch(casacore::AipsError & e) {
+                        return arrow::Status::Invalid("WriteFixedColumn ",
+                                                      GetTableColumn().columnDesc().name(),
+                                                      ": ", e.what());
                     }
-
-                    offset += product;
                 }
             }
-
-            if(offset != nelements) {
-                return arrow::Status::Invalid("offsets != nelements "
-                                       "during conversion of variably shaped column ",
-                                       column_desc_.name());
-            }
-
-            ARROW_ASSIGN_OR_RAISE(array_, MakeArrowPrimitiveArray(buffer, nelements, arrow_dtype));
-        }
-
-        // NOTE(sjperkins)
-        // See https://arrow.apache.org/docs/format/Columnar.html#variable-size-list-layout
-        // At this stage we have a flat array of values that we wish to arrange
-        // into a nested structure. It needs to be built from the fastest changing
-        // dimension towards the slowest changing dimension. This is accomplished by
-        // creating offsets for each nested layer. The dimension size at each layer
-        // must be repeated by the product of the previous elements in the shape.
-
-        // See this worked case
-        //    Here, we use casacore's FORTRAN ordering for shapes
-        //    repeats = [reduce(mul, s[d+1:], 1) for s, d in enumerate(shapes_)]
-        //    dim_sizes = [s[d] for d, s in enumerate(shapes)]
-
-        //    shapes = [(2, 5, 10), (4, 3, 10)]
-        //    products = [(50, 10, 1), (30, 10, 1)]
-        //    For d == 0
-        //    repeats = [50, 30]
-        //    dim_sizes = [2, 4]
-        //    offsets = [0] + cumsum(50*[2] + 30*[4])
-        //    For d == 1
-        //    repeats = [10, 10]
-        //    dim_sizes = [5, 3]
-        //    offsets = [0] + cumsum(10*[5] + 10+[3])
-        //    For d == 2
-        //    repeats = [1, 1]
-        //    dim_sizes = [10, 10]
-        //    offsets = [0] + cumsum((1*[10] + 1*[10]))
-
-
-
-        // Compute the products
-        auto products = std::vector<casacore::IPosition>(nrow_, casacore::IPosition(ndim, 1));
-
-        for(casacore::uInt row=startrow_; row < endrow_; ++row) {
-            auto lrow = local_row(row);
-            const auto & shape = shapes[lrow];
-            auto & product = products[lrow];
-
-            for(int d=ndim - 2; d >= 0; --d) {
-                product[d] *= product[d + 1] * shape[d + 1];
-            }
-        }
-
-        for(int d=0; d < ndim; ++d) {
-            // Precompute size of offsets for offset buffer allocation
-            unsigned int noffsets = std::accumulate(products.begin(), products.end(), 1,
-                [d](auto i, const auto & p) { return i + p[d]; });
-
-            arrow::Int32Builder builder(pool_);
-            unsigned int running_offset = 0;
-            unsigned int o = 1;
-            ARROW_RETURN_NOT_OK(builder.Reserve(noffsets));
-            ARROW_RETURN_NOT_OK(builder.Append(running_offset));
-
-            for(casacore::uInt row=startrow_; row < endrow_; ++row) {
-                auto repeats = products[local_row(row)][d];
-                auto dim_size = shapes[local_row(row)][d];
-
-                for(auto r=0; r < repeats; ++r, ++o) {
-                    running_offset += dim_size;
-                    ARROW_RETURN_NOT_OK(builder.Append(running_offset));
-                }
-            }
-
-            if(o != noffsets) { return arrow::Status::Invalid("o != noffsets"); }
-
-            ARROW_ASSIGN_OR_RAISE(auto offsets, builder.Finish());
-            ARROW_ASSIGN_OR_RAISE(array_, arrow::ListArray::FromArrays(*offsets, *array_));
-            // NOTE(sjperkins): Perhaps remove this for performance
-            ARROW_RETURN_NOT_OK(ValidateArray(array_));
-        }
-
-        if(auto list_array = std::dynamic_pointer_cast<arrow::ListArray>(array_)) {
-            // NOTE(sjperkins)
-            // Directly adding nulls to the underlying list_array->data()
-            // doesn't seem to work, recreate the array with nulls and null_count
-            ARROW_ASSIGN_OR_RAISE(array_, arrow::ListArray::FromArrays(
-                *list_array->offsets(),
-                *list_array->values(),
-                pool_,
-                nulls,
-                null_counts));
-
-            return ValidateArray(array_);
-        } else {
-            return arrow::Status::Invalid("Unable to cast final array to arrow::ListArray");
-        }
-    }
-
-    template <typename T>
-    arrow::Status CheckByteWidths(const std::shared_ptr<arrow::DataType> & arrow_dtype) {
-        // Check that the arrow type byte widths match up with the casacore byte widths
-        if(auto complex_dtype = std::dynamic_pointer_cast<ComplexType>(arrow_dtype)) {
-            auto vdt = complex_dtype->value_type();
-            if(vdt->byte_width() == -1 || 2*vdt->byte_width() != sizeof(T)) {
-                return arrow::Status::Invalid(
-                    "2 x byte width of complex value type",
-                    vdt->ToString(), " (",
-                    2*vdt->byte_width(),
-                    ") != sizeof(T) (", sizeof(T), ")");
-            }
-        } else if(arrow_dtype == arrow::utf8()) {
-            return arrow::Status::OK();
-        } else if(arrow_dtype->byte_width() == -1 || arrow_dtype->byte_width() != sizeof(T)) {
-            return arrow::Status::Invalid(
-                arrow_dtype->ToString(), " byte width (",
-                arrow_dtype->byte_width(),
-                ") != sizeof(T) (", sizeof(T), ")");
         }
 
         return arrow::Status::OK();
     }
 
-    template <typename T>
-    arrow::Status ConvertColumn(const std::shared_ptr<arrow::DataType> & arrow_dtype) {
-        ARROW_RETURN_NOT_OK(CheckByteWidths<T>(arrow_dtype));
-
-        if(nrow_ == 0) {
-            return arrow::Status::Invalid("Zero-length row request");
-        }
-
-        if(column_desc_.isScalar()) {  // ndim == 0
-            return ConvertScalarColumn<T>(arrow_dtype);
-        }
-
-        auto & config = ServiceLocator::configuration();
-        auto convert_method = config.GetDefault("casa.convert.strategy", "fixed");
-        auto list_convert = convert_method.find("list") == 0;
-
-        if(!list_convert && column_desc_.isFixedShape()) {
-            return ConvertFixedArrayColumn<T>(arrow_dtype, column_desc_.shape());
-        }
-
-        // Variably shaped, read in shapes and null values
-        auto shapes = std::vector<casacore::IPosition>(nrow_, casacore::IPosition());
-        auto shapes_set = std::unordered_set<casacore::IPosition>{};
-        auto column = casacore::ArrayColumn<T>(column_);
-        int64_t null_counts = 0;
-        ARROW_ASSIGN_OR_RAISE(auto nulls, arrow::AllocateBitmap(nrow_, pool_));
-
-        for(casacore::uInt row = startrow_; row < endrow_; ++row) {
-            auto lrow = local_row(row);
-            auto is_defined = column.isDefined(row);
-            arrow::bit_util::SetBitTo(nulls->mutable_data(), lrow, is_defined);
-            null_counts += is_defined ? 0 : 1;
-
-            if(is_defined) {
-                shapes[lrow] = column.shape(row);
-                shapes_set.insert(shapes[lrow]);
-            }
-        }
 
-        auto [shapes_equal, ndim_equal] = [&]() -> std::tuple<bool, bool> {
-            bool ndim_equal = true;
-            bool shapes_equal = true;
-
-            if(shapes_set.size() <= 1) {
-                return {shapes_equal, ndim_equal};
-            }
-
-            for(auto it = std::begin(shapes_set); it != std::end(shapes_set); ++it) {
-                if(it->size() != std::begin(shapes_set)->size()) {
-                    ndim_equal = ndim_equal && false;
-                    shapes_equal = shapes_equal && false;
-                    continue;
+    template <typename T>
+    arrow::Status WriteVariableColumn() {
+        auto column = casacore::ArrayColumn<T>(GetTableColumn());
+        column.setMaximumCacheSize(1);
+        ARROW_ASSIGN_OR_RAISE(auto flat_array, GetFlatArray());
+        ARROW_ASSIGN_OR_RAISE(flat_array, MaybeCastFlatArray(flat_array));
+        auto nelements = map_.get().nElements();
+
+        if constexpr(std::is_same_v<T, casacore::String>) {
+            auto flat_strings = std::dynamic_pointer_cast<arrow::StringArray>(flat_array);
+            assert(flat_strings != nullptr && "Unable to cast array to StringArray");
+            ARROW_RETURN_NOT_OK(FailIfNotUTF8(flat_strings->type()));
+            ARROW_RETURN_NOT_OK(CheckElements(flat_strings->length(), nelements));
+
+            for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                // Copy sections of data from the Arrow Buffer and write
+                try {
+                    auto carray = casacore::Array<casacore::String>(it.GetShape());
+                    auto * chunk_ptr = carray.data();
+                    for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                        auto sv = flat_strings->GetView(mit.GlobalOffset());
+                        chunk_ptr[mit.ChunkOffset()] = casacore::String(std::begin(sv), std::end(sv));
+                    }
+                    column.putColumnRange(it.GetRowSlicer(), it.GetSectionSlicer(), carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteVariableColumn ",
+                                                  GetTableColumn().columnDesc().name(),
+                                                  ": ", e.what());
                 }
-
-                if(*it != *std::begin(shapes_set)) {
-                    shapes_equal = shapes_equal && false;
+            }
+        } else {
+            // Get Arrow Array buffer
+            auto span = flat_array->data()->buffers[1]->span_as<T>();
+            ARROW_RETURN_NOT_OK(CheckElements(span.size(), nelements));
+
+            for(auto it = map_.get().RangeBegin(); it != map_.get().RangeEnd(); ++it) {
+                // Copy sections of data from the Arrow Buffer and write
+                try {
+                    auto carray = casacore::Array<T>(it.GetShape());
+                    auto chunk_ptr = carray.data();
+                    for(auto mit = it.MapBegin(); mit != it.MapEnd(); ++mit) {
+                        chunk_ptr[mit.ChunkOffset()] = span[mit.GlobalOffset()];
+                    }
+                    column.putColumnRange(it.GetRowSlicer(), it.GetSectionSlicer(), carray);
+                } catch(casacore::AipsError & e) {
+                    return arrow::Status::Invalid("WriteVariableColumn ",
+                                                  GetTableColumn().columnDesc().name(),
+                                                  ": ", e.what());
                 }
             }
-
-            return {shapes_equal, ndim_equal};
-        }();
-
-        if(!ndim_equal) {
-            return arrow::Status::NotImplemented(
-                column_desc_.name(), " has unconstrained dimensionality");
         }
 
-        // No nulls and all shapes are equal, we can represent this with a
-        // fixed shape list
-        if(!list_convert && null_counts == 0 && shapes_equal) {
-            return ConvertFixedArrayColumn<T>(arrow_dtype, shapes[0]);
-        }
-
-        return ConvertVariableArrayColumn<T>(
-                arrow_dtype,
-                shapes,
-                nulls,
-                null_counts,
-                shapes[0].size());
+        return arrow::Status::OK();
     }
 };
 
 } // namespace arcae
 
-#endif
+#endif // COLUMN_WRITE_VISITOR_H
```

### Comparing `arcae-0.2.2/cpp/arcae/complex_type.cc` & `arcae-0.2.3/cpp/arcae/complex_type.cc`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cpp/arcae/complex_type.h` & `arcae-0.2.3/cpp/arcae/complex_type.h`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cpp/arcae/configuration.cc` & `arcae-0.2.3/cpp/arcae/configuration.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 #include "arcae/configuration.h"
 
+#include <string>
 
 namespace arcae {
 
 arrow::Result<std::string> Configuration::Get(const std::string & key) const {
-    auto it = kvmap_.find(key);
-
-    if(it == kvmap_.end()) {
-        return arrow::Status::KeyError(key);
-    } else {
+    if(auto it = kvmap_.find(key); it != kvmap_.end()) {
         return it->second;
     }
+    return arrow::Status::KeyError(key);
 }
 
 
 std::string Configuration::GetDefault(const std::string & key, std::string default_value) const {
-    auto it = kvmap_.find(key);
-
-    if(it == kvmap_.end()) {
-        return std::move(default_value);
-    } else {
+    if(auto it = kvmap_.find(key); it != kvmap_.end()) {
         return it->second;
     }
+    return default_value;
 }
 
 
 arrow::Result<bool> Configuration::Delete(const std::string & key) {
-    auto it = kvmap_.find(key);
-
-    if(it == kvmap_.end()) {
-        return arrow::Status::KeyError(key);
-    } else {
+    if(auto it = kvmap_.find(key); it != kvmap_.end()) {
         kvmap_.erase(it);
         return true;
     }
+    return arrow::Status::KeyError(key);
 }
 
 } // namespace arcae
```

### Comparing `arcae-0.2.2/cpp/arcae/configuration.h` & `arcae-0.2.3/cpp/arcae/configuration.h`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cpp/arcae/descriptor.cc` & `arcae-0.2.3/cpp/arcae/descriptor.cc`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,37 @@
 
 #include <sstream>
 
 #include <arrow/result.h>
 
 #include <casacore/casa/Json.h>
 #include <casacore/casa/Json/JsonKVMap.h>
+#include <casacore/casa/Json/JsonParser.h>
 #include <casacore/casa/Containers/RecordInterface.h>
 #include <casacore/ms/MeasurementSets/MeasurementSet.h>
-#include <casacore/tables/Tables/TableError.h>
 #include <casacore/tables/Tables/TableRecord.h>
 #include <casacore/tables/Tables/TableDesc.h>
 #include <casacore/tables/Tables/TableProxy.h>
 #include <casacore/casa/Containers/ValueHolder.h>
 
 #include "arcae/descriptor.h"
 
 
 using ::arrow::Result;
-using ::arrow::Status;
 
-using ::casacore::JsonKVMap;
 using ::casacore::JsonParser;
 using ::casacore::JsonOut;
 using ::casacore::String;
 using ::casacore::Vector;
 
 using ::casacore::TableDesc;
 using ::casacore::SetupNewTable;
 using ::casacore::Record;
 using ::casacore::RecordInterface;
 using ::casacore::TableProxy;
-using ::casacore::TableError;
 using ::casacore::Table;
 
 using ::casacore::MeasurementSet;
 using ::casacore::MSAntenna;
 using ::casacore::MSDataDescription;
 using ::casacore::MSDoppler;
 using ::casacore::MSFeed;
@@ -172,18 +169,14 @@
         record_json.write(record.name(i), record.asValueHolder(i));
     }
 
     record_json.end();
     return json_oss.str();
 }
 
-Record JsonToRecord(const std::string & json_record) {
-    return JsonParser::parse(json_record).toRecord();
-}
-
 
 // Get the required table descriptions for the given table.
 // If "" or "MAIN", the table descriptions for a Measurement Set
 // will be supplied, otherwise table should be some valid
 // MeasurementSet subtable
 Result<TableDesc> MSTableDescriptor(const String & table, bool complete)
 {
```

### Comparing `arcae-0.2.2/cpp/arcae/safe_table_proxy.cc` & `arcae-0.2.3/cpp/arcae/safe_table_proxy.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 #include <memory>
 #include <sstream>
 
 #include <arrow/util/logging.h>  // IWYU pragma: keep
+#include <arrow/result.h>
+#include <arrow/status.h>
 
 #include <casacore/casa/Json.h>
+#include <casacore/tables/Tables/TableColumn.h>
 #include <casacore/tables/Tables/TableIterProxy.h>
 
 #include "arcae/safe_table_proxy.h"
+#include "arcae/base_column_map.h"
+#include "arcae/column_read_map.h"
+#include "arcae/column_read_visitor.h"
+#include "arcae/column_write_map.h"
+#include "arcae/column_write_visitor.h"
 
 
-using ::arrow::DataType;
-using ::arrow::Buffer;
-using ::arrow::Future;
 using ::arrow::Result;
 using ::arrow::Status;
 
 using ::casacore::Record;
-using ::casacore::Table;
 using ::casacore::TableColumn;
 using ::casacore::TableIterProxy;
-using ::casacore::TableLock;
 using ::casacore::TableProxy;
 
 namespace arcae {
 namespace {
 // https://stackoverflow.com/a/25069711
 struct enable_make_shared_stp : public SafeTableProxy {};
+
+Status FailIfClosed(const SafeTableProxy & proxy) {
+    if(!proxy.IsClosed()) return Status::OK();
+    return Status::Invalid("Table is closed");
+};
+
+
+Status FailIfColumnDoesntExist(const casacore::Table & table, const std::string & column) {
+    if(!table.tableDesc().isColumn(column)) {
+        return Status::Invalid("Column ", column, " does not exist");
+    }
+    return Status::OK();
+}
+
 } // namespace
 
 
 std::tuple<casacore::uInt, casacore::uInt>
 SafeTableProxy::ClampRows(const casacore::Table & table, casacore::uInt startrow, casacore::uInt nrow) {
     if(startrow > table.nrow()) {
         return {table.nrow(), 0};
@@ -38,98 +55,142 @@
     if(startrow + nrow >= table.nrow()) {
         nrow = std::min(table.nrow(), table.nrow() - startrow);
     }
 
     return {startrow, nrow};
 }
 
-arrow::Result<std::string>
+Result<std::string>
 SafeTableProxy::GetTableDescriptor() const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
-    return run_isolated([this]() -> arrow::Result<std::string> {
+    return run_isolated([this]() -> Result<std::string> {
         std::ostringstream json_oss;
         casacore::JsonOut table_json(json_oss);
 
         table_json.start();
         table_json.write(CASA_DESCRIPTOR, table_proxy->getTableDescription(true, true));
         table_json.end();
 
         return json_oss.str();
     });
 }
 
-arrow::Result<std::string>
+Result<std::string>
 SafeTableProxy::GetColumnDescriptor(const std::string & column) const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
-
-    return run_isolated([this, &column]() -> arrow::Result<std::string> {
-        const auto & table_desc = this->table_proxy->table().tableDesc();
-
-        if(!table_desc.isColumn(column)) {
-            return arrow::Status::UnknownError(column, " does not exist");
-        }
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
+    return run_isolated([this, &column]() -> Result<std::string> {
+        ARROW_RETURN_NOT_OK(FailIfColumnDoesntExist(this->table_proxy->table(), column));
         std::ostringstream json_oss;
         casacore::JsonOut column_json(json_oss);
 
         column_json.start();
         column_json.write(column, table_proxy->getColumnDescription(column, true, true));
         column_json.end();
 
         return json_oss.str();
     });
 }
 
 
-arrow::Result<std::shared_ptr<arrow::Array>>
-SafeTableProxy::GetColumn(const std::string & column, casacore::uInt startrow, casacore::uInt nrow) const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+Result<std::shared_ptr<arrow::Array>>
+SafeTableProxy::GetColumn(const std::string & column, const ColumnSelection & selection) const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
-    return run_isolated([this, &column, startrow, nrow]() -> arrow::Result<std::shared_ptr<arrow::Array>> {
+    return run_isolated([this, &column, &selection]() -> Result<std::shared_ptr<arrow::Array>> {
         auto & casa_table = this->table_proxy->table();
-
-        if(!casa_table.tableDesc().isColumn(column)) {
-            return arrow::Status::UnknownError(column, " does not exist");
-        }
+        ARROW_RETURN_NOT_OK(FailIfColumnDoesntExist(casa_table, column));
 
         auto table_column = TableColumn(casa_table, column);
-        const auto & column_desc = table_column.columnDesc();
-        auto [start_row, n_row] = ClampRows(casa_table, startrow, nrow);
-        auto visitor = ColumnConvertVisitor(table_column, start_row, n_row);
-        auto visit_status = visitor.Visit(column_desc.dataType());
-        ARROW_RETURN_NOT_OK(visit_status);
+        ARROW_ASSIGN_OR_RAISE(auto map, ColumnReadMap::Make(table_column, selection));
+        auto visitor = ColumnReadVisitor(map);
+        ARROW_RETURN_NOT_OK(visitor.Visit());
         return std::move(visitor.array_);
     });
 }
 
-arrow::Result<std::shared_ptr<arrow::Table>>
-SafeTableProxy::ToArrow(casacore::uInt startrow, casacore::uInt nrow, const std::vector<std::string> & columns) const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+Result<bool>
+SafeTableProxy::PutColumn(const std::string & column,
+                          const ColumnSelection & selection,
+                          const std::shared_ptr<arrow::Array> & data) const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
+
+    return run_isolated([this, &column, &selection, &data]() -> Result<bool> {
+        auto & casa_table = this->table_proxy->table();
+        ARROW_RETURN_NOT_OK(FailIfColumnDoesntExist(casa_table, column));
+        auto table_column = TableColumn(casa_table, column);
+        ARROW_ASSIGN_OR_RAISE(auto map, ColumnWriteMap::Make(table_column, selection, data))
+        auto visitor = ColumnWriteVisitor(map);
+        ARROW_RETURN_NOT_OK(visitor.Visit());
+        return true;
+    });
+}
+
+Result<std::string>
+SafeTableProxy::GetLockOptions() const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
+    return run_isolated([this]() -> Result<std::string> {
+        std::ostringstream json_oss;
+        casacore::JsonOut lock_json(json_oss);
+        const auto & lockoptions = this->table_proxy->lockOptions();
+        lock_json.put(lockoptions);
+        return json_oss.str();
+    });
+}
+
+Result<bool>
+SafeTableProxy::ReopenRW() const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
+    return run_isolated([this]() -> Result<bool> {
+        this->table_proxy->table().reopenRW();
+        return true;
+    });
+}
 
-    return run_isolated([this, startrow, nrow, &columns]() -> arrow::Result<std::shared_ptr<arrow::Table>> {
+Result<bool>
+SafeTableProxy::IsWriteable() const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
+    return run_isolated([this]() -> Result<bool> {
+        return this->table_proxy->table().isWritable();
+    });
+}
+
+
+Result<std::shared_ptr<arrow::Table>>
+SafeTableProxy::ToArrow(const ColumnSelection & selection, const std::vector<std::string> & columns) const {
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
+
+    return run_isolated([this, &selection, &columns]() -> Result<std::shared_ptr<arrow::Table>> {
         const auto & casa_table = this->table_proxy->table();
         const auto & table_desc = casa_table.tableDesc();
         auto column_names = columns.size() == 0 ? table_desc.columnNames() : casacore::Vector<casacore::String>(columns);
-        auto [start_row, n_row] = ClampRows(casa_table, startrow, nrow);
         auto fields = arrow::FieldVector();
         auto arrays = arrow::ArrayVector();
 
         for(casacore::uInt i=0; i < column_names.size(); ++i) {
             auto column_name = column_names[i];
 
             if(!table_desc.isColumn(column_name)) {
                 ARROW_LOG(WARNING) << column_name << " is not a valid column";
                 continue;
             }
 
             auto table_column = TableColumn(casa_table, column_name);
             auto column_desc = table_column.columnDesc();
-            auto visitor = ColumnConvertVisitor(table_column, start_row, n_row);
-            auto visit_status = visitor.Visit(column_desc.dataType());
+            auto map_result = ColumnReadMap::Make(table_column, selection);
+
+            if(!map_result.ok()) {
+                ARROW_LOG(WARNING)
+                    << "Ignoring " << column_name << " " << map_result.status();
+                    continue;
+            }
+
+            auto visitor = ColumnReadVisitor(map_result.ValueOrDie());
+            auto visit_status = visitor.Visit();
 
             if(!visit_status.ok()) {
                 ARROW_LOG(WARNING)
                     << "Ignoring " << column_name << " " << visit_status;
                 continue;
             }
 
@@ -164,49 +225,49 @@
         table_json.write(CASA_DESCRIPTOR, table_proxy->getTableDescription(true, true));
         table_json.end();
 
         auto table_metadata = arrow::KeyValueMetadata::Make(
             {ARCAE_METADATA}, {json_oss.str()});
 
         auto schema = arrow::schema(fields, std::move(table_metadata));
-        auto table = arrow::Table::Make(std::move(schema), arrays, n_row);
+        auto table = arrow::Table::Make(std::move(schema), std::move(arrays));
         auto status = table->Validate();
 
         if(!status.ok()) {
             return status;
         }
 
         return table;
     });
 }
 
 
 Result<std::vector<std::string>>
 SafeTableProxy::Columns() const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
     return run_isolated([this]() -> Result<std::vector<std::string>> {
         const auto& column_names = this->table_proxy->table().tableDesc().columnNames();
         return std::vector<std::string>(column_names.begin(), column_names.end());
     });
 }
 
 
 Result<casacore::uInt>
 SafeTableProxy::nColumns() const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
     return run_isolated([this]() -> Result<casacore::uInt> {
         return this->table_proxy->table().tableDesc().ncolumn();
     });
 }
 
 Result<casacore::uInt>
 SafeTableProxy::nRow() const {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
     return run_isolated([this]() -> Result<casacore::uInt> {
         return this->table_proxy->table().nrow();
     });
 }
 
 Result<std::vector<std::shared_ptr<SafeTableProxy>>>
@@ -214,15 +275,15 @@
     const std::vector<std::string> & partition_columns,
     const std::vector<std::string> & sort_columns) const {
 
     if(partition_columns.size() == 0) {
         return Status::Invalid("No partitioning columns provided");
     }
 
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
     return run_isolated([this, &partition_columns, &sort_columns]() -> Result<std::vector<std::shared_ptr<SafeTableProxy>>> {
         casacore::Block<casacore::String> casa_sort_cols(sort_columns.size());
         for(casacore::uInt i=0; i < sort_columns.size(); ++i)
             { casa_sort_cols[i] = sort_columns[i]; }
 
         auto casa_part_cols = casacore::Vector<casacore::String>(partition_columns);
@@ -246,15 +307,15 @@
         return result;
     });
 }
 
 
 Result<bool>
 SafeTableProxy::AddRows(casacore::uInt nrows) {
-    ARROW_RETURN_NOT_OK(FailIfClosed());
+    ARROW_RETURN_NOT_OK(FailIfClosed(*this));
 
     return run_isolated([this, nrows]() -> Result<bool> {
         this->table_proxy->addRow(nrows);
         return true;
     });
 }
```

### Comparing `arcae-0.2.2/cpp/arcae/safe_table_proxy.h` & `arcae-0.2.3/cpp/arcae/safe_table_proxy.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,125 @@
 #ifndef ARCAE_SAFE_TABLE_PROXY_H
 #define ARCAE_SAFE_TABLE_PROXY_H
 
 #include <climits>
 #include <functional>
+#include <type_traits>
 
 #include <casacore/tables/Tables.h>
 #include <casacore/tables/Tables/TableProxy.h>
 
+#include <arrow/util/logging.h>
 #include <arrow/util/thread_pool.h>
 
-#include "arcae/column_convert_visitor.h"
-
+#include "arcae/base_column_map.h"
 
 namespace arcae {
 
 static constexpr char ARCAE_METADATA[]  = "__arcae_metadata__";
 static constexpr char CASA_DESCRIPTOR[]  = "__casa_descriptor__";
 
 /// @class SafeTableProxy
 /// @brief Constrains Table access to an arrow::ThreadPool containing a single thread.
 class SafeTableProxy {
 private:
     std::shared_ptr<casacore::TableProxy> table_proxy;
     std::shared_ptr<arrow::internal::ThreadPool> io_pool;
     bool is_closed;
 
-private:
-    inline arrow::Status FailIfClosed() const {
-        return is_closed ? arrow::Status::Invalid("Table is closed")
-                         : arrow::Status::OK();
-    };
-
 protected:
     SafeTableProxy() = default;
     SafeTableProxy(const SafeTableProxy & rhs) = delete;
     SafeTableProxy(SafeTableProxy && rhs) = delete;
     SafeTableProxy& operator=(const SafeTableProxy & rhs) = delete;
     SafeTableProxy& operator=(SafeTableProxy && rhs) = delete;
 
     /// Run the given functor in the isolated Threadpool
     template <typename Fn>
     std::invoke_result_t<Fn> run_isolated(Fn && functor) {
-        return arrow::DeferNotOk(this->io_pool->Submit(std::move(functor))).result();
+        return arrow::DeferNotOk(this->io_pool->Submit(std::forward<Fn>(functor))).MoveResult();
     }
 
     /// Run the given functor in the isolated Threadpool
     template <typename Fn>
     std::invoke_result_t<Fn> run_isolated(Fn && functor) const {
-        return arrow::DeferNotOk(this->io_pool->Submit(std::move(functor))).result();
+        return arrow::DeferNotOk(this->io_pool->Submit(std::forward<Fn>(functor))).MoveResult();
     }
 
 public:
     virtual ~SafeTableProxy() {
         auto result = Close();
         if(!result.ok()) {
             ARROW_LOG(WARNING) << "Error closing file " << result.status();
         }
     };
 
-    template <typename Fn>
-    static arrow::Result<std::shared_ptr<SafeTableProxy>> Make(Fn && functor) {
-        struct enable_make_shared_stp : public SafeTableProxy {};
-        auto proxy = std::make_shared<enable_make_shared_stp>();
-        ARROW_ASSIGN_OR_RAISE(proxy->io_pool, ::arrow::internal::ThreadPool::Make(1));
-
-        // Mark as closed so that if construction fails, we don't try to close it
-        proxy->is_closed = true;
-        ARROW_ASSIGN_OR_RAISE(proxy->table_proxy, proxy->run_isolated(std::move(functor)));
-        proxy->is_closed = false;
-
-        return proxy;
-    }
-
     template <typename Fn,
               typename = std::enable_if_t<
                 std::is_invocable_v<Fn, const casacore::TableProxy &>>>
     std::invoke_result_t<Fn, const casacore::TableProxy &> run(Fn && functor) const {
-        return run_isolated([this, functor = std::move(functor)]() mutable {
+        return run_isolated([this, functor = std::forward<Fn>(functor)]() mutable {
             return std::invoke(std::forward<Fn>(functor),
                                static_cast<const casacore::TableProxy &>(*this->table_proxy));
         });
     }
 
     template <typename Fn,
               typename = std::enable_if_t<
                 std::is_invocable_v<Fn, casacore::TableProxy &>>>
     std::invoke_result_t<Fn, casacore::TableProxy &> run(Fn && functor) {
-        return run_isolated([this, functor = std::move(functor)]() mutable {
+        return run_isolated([this, functor = std::forward<Fn>(functor)]() mutable {
             return std::invoke(std::forward<Fn>(functor),
                                static_cast<casacore::TableProxy &>(*this->table_proxy));
         });
     }
 
+
+    template <typename Fn>
+    static arrow::Result<std::shared_ptr<SafeTableProxy>> Make(Fn && functor) {
+        struct enable_make_shared_stp : public SafeTableProxy {};
+        auto proxy = std::make_shared<enable_make_shared_stp>();
+        ARROW_ASSIGN_OR_RAISE(proxy->io_pool, ::arrow::internal::ThreadPool::Make(1));
+
+        // Mark as closed so that if construction fails, we don't try to close it
+        proxy->is_closed = true;
+        ARROW_ASSIGN_OR_RAISE(proxy->table_proxy, proxy->run_isolated(std::move(functor)));
+        proxy->is_closed = false;
+
+        return proxy;
+    }
+
     static std::tuple<casacore::uInt, casacore::uInt>
     ClampRows(const casacore::Table & table,
               casacore::uInt startrow,
               casacore::uInt nrow);
 
+    bool IsClosed() const { return is_closed; }
+
     arrow::Result<std::shared_ptr<arrow::Table>> ToArrow(
-        casacore::uInt startrow=0,
-        casacore::uInt nrow=UINT_MAX,
+        const ColumnSelection & selection={},
         const std::vector<std::string> & columns = {}) const;
 
     arrow::Result<std::shared_ptr<arrow::Array>> GetColumn(
         const std::string & column,
-        casacore::uInt startrow,
-        casacore::uInt nrow) const;
+        const ColumnSelection & selection) const;
+
+    arrow::Result<bool> PutColumn(
+        const std::string & column,
+        const ColumnSelection & selection,
+        const std::shared_ptr<arrow::Array> & data) const;
 
     arrow::Result<std::string> GetTableDescriptor() const;
     arrow::Result<std::string> GetColumnDescriptor(const std::string & column) const;
 
+    arrow::Result<std::string> GetLockOptions() const;
+
+    arrow::Result<bool> ReopenRW() const;
+    arrow::Result<bool> IsWriteable() const;
+
     arrow::Result<std::vector<std::string>> Columns() const;
     arrow::Result<casacore::uInt> nColumns() const;
     arrow::Result<casacore::uInt> nRow() const;
     arrow::Result<std::vector<std::shared_ptr<SafeTableProxy>>> Partition(
         const std::vector<std::string> & partition_columns={},
         const std::vector<std::string> & sort_columns={}) const;
```

### Comparing `arcae-0.2.2/cpp/arcae/service_locator.cc` & `arcae-0.2.3/cpp/arcae/service_locator.cc`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/cpp/arcae/table_factory.cc` & `arcae-0.2.3/cpp/arcae/table_factory.cc`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 #include "arcae/descriptor.h"
 #include "arcae/safe_table_proxy.h"
 #include "arcae/table_factory.h"
 
 #include <arrow/api.h>
 
+#include <casacore/casa/Json.h>
+#include <casacore/casa/Json/JsonKVMap.h>
+#include <casacore/casa/Json/JsonParser.h>
 #include <casacore/tables/Tables/SetupNewTab.h>
 #include <casacore/tables/Tables.h>
 #include <casacore/tables/Tables/TableProxy.h>
 #include <casacore/tables/Tables/TableLock.h>
 #include <casacore/ms/MeasurementSets/MeasurementSet.h>
 
 using namespace std::literals;
 
 using ::arrow::Result;
 using ::arrow::Status;
 
-using ::casacore::String;
+using ::casacore::JsonParser;
 
-using ::casacore::SetupNewTable;
 using ::casacore::TableProxy;
 using ::casacore::TableLock;
 using ::casacore::Table;
 using ::casacore::Record;
 
 using ::casacore::MeasurementSet;
 using ::casacore::MSAntenna;
@@ -78,28 +80,24 @@
 static constexpr char kSyscal[] = "SYSCAL";
 static constexpr char kWeather[] = "WEATHER";
 
 } // namespace
 
 Result<std::shared_ptr<SafeTableProxy>> OpenTable(
         const std::string & filename,
-        bool readonly) {
-    return SafeTableProxy::Make([&filename, &readonly]() -> Result<std::shared_ptr<TableProxy>> {
-        Record record;
-        TableLock lock(TableLock::LockOption::AutoNoReadLocking);
-
-        record.define("option", "auto");
-        record.define("internal", lock.interval());
-        record.define("maxwait", casacore::Int(lock.maxWait()));
+        bool readonly,
+        const std::string & json_lockoptions) {
+    return SafeTableProxy::Make([&filename, &readonly, &json_lockoptions]() -> Result<std::shared_ptr<TableProxy>> {
+        auto lock_record = JsonParser::parse(json_lockoptions).toRecord();
 
         std::shared_ptr<TableProxy> proxy;
 
         try {
             proxy = std::make_shared<TableProxy>(
-                filename, record, Table::TableOption::Old);
+                filename, lock_record, Table::TableOption::Old);
 
             if(!readonly) {
                 proxy->reopenRW();
             }
         } catch(std::exception & e) {
             return Status::Invalid(e.what());
         }
```

### Comparing `arcae-0.2.2/cpp/arcae/table_factory.h` & `arcae-0.2.3/cpp/arcae/table_factory.h`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 #include "arcae/safe_table_proxy.h"
 
 namespace arcae {
 
 arrow::Result<std::shared_ptr<SafeTableProxy>> OpenTable(
                                 const std::string & filename,
-                                bool readonly=true);
+                                bool readonly=true,
+                                const std::string & json_lockoptions=R"({"option": "auto"})");
 arrow::Result<std::shared_ptr<SafeTableProxy>> DefaultMS(
                                 const std::string & name,
                                 const std::string & subtable="MAIN",
                                 const std::string & json_table_desc="{}",
                                 const std::string & json_dminfo="{}");
 arrow::Result<std::shared_ptr<SafeTableProxy>> Taql(
                                 const std::string & taql);
```

### Comparing `arcae-0.2.2/cpp/tests/basic_test.cc` & `arcae-0.2.3/cpp/tests/basic_test.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-#include <iostream>
-
 #include <arcae/safe_table_proxy.h>
-#include <tests/test_utils.h>
+
 #include <arrow/testing/gtest_util.h>
+
 #include <casacore/tables/Tables.h>
 #include <casacore/ms/MeasurementSets/MeasurementSet.h>
+
 #include <gtest/gtest.h>
 
+#include <tests/test_utils.h>
+
 using namespace std::string_literals;
 
 class BasicTableTests : public ::testing::Test {
   protected:
     std::shared_ptr<arcae::SafeTableProxy> table_proxy_;
 
     void SetUp() override {
@@ -27,8 +29,17 @@
     }
 };
 
 // Basic creation of a SafeTableProxy
 TEST_F(BasicTableTests, CasaTable) {
   ASSERT_TRUE(table_proxy_);
   ASSERT_EQ(table_proxy_->nRow(), 100);
+}
+
+
+TEST_F(BasicTableTests, RunFunctor) {
+  auto nrows = table_proxy_->run([](casacore::TableProxy & proxy) {
+    return arrow::Result(proxy.table().nrow());
+  });
+
+  EXPECT_EQ(nrows, 100);
 }
```

### Comparing `arcae-0.2.2/cpp/tests/parallel_write_test.cc` & `arcae-0.2.3/cpp/tests/parallel_write_test.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#include <iostream>
-
 #include <arcae/safe_table_proxy.h>
 #include <arcae/table_factory.h>
-#include <tests/test_utils.h>
+
 #include <arrow/util/thread_pool.h>
 #include <arrow/testing/gtest_util.h>
+
 #include <casacore/tables/Tables.h>
 #include <casacore/ms/MeasurementSets/MeasurementSet.h>
+
 #include <gtest/gtest.h>
 
+#include <tests/test_utils.h>
+
 using casacore::Array;
 using casacore::ArrayColumn;
 using casacore::ArrayColumnDesc;
 using casacore::ColumnDesc;
 using CasaComplex = casacore::Complex;
 using MS = casacore::MeasurementSet;
 using MSColumns = casacore::MSMainEnums::PredefinedColumns;
 using casacore::SetupNewTable;
-using casacore::ScalarColumn;
 using casacore::Slice;
-using casacore::Slicer;
 using casacore::Table;
 using casacore::TableDesc;
 using casacore::TableColumn;
 using casacore::TableProxy;
 using casacore::TiledColumnStMan;
 using IPos = casacore::IPosition;
```

### Comparing `arcae-0.2.2/cpp/tests/test_utils.cc` & `arcae-0.2.3/cpp/tests/test_utils.cc`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/scripts/run_cibuildwheel.sh` & `arcae-0.2.3/scripts/run_cibuildwheel.sh`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 export VCPKG_TARGET_TRIPLET=x64-linux-dynamic-cxx17-abi1-rel
 export CIBW_ENVIRONMENT_LINUX="\
 CMAKE_ARGS=-DBUILD_TESTING=OFF \
 VCPKG_DEFAULT_BINARY_CACHE=/host$VCPKG_HOST_BINARY_CACHE \
 VCPKG_INSTALLED_DIR=$VCPKG_INSTALLED_DIR \
 VCPKG_TARGET_TRIPLET=$VCPKG_TARGET_TRIPLET \
 LD_LIBRARY_PATH=$VCPKG_INSTALLED_DIR/$VCPKG_TARGET_TRIPLET/lib"
-export CIBW_REPAIR_WHEEL_COMMAND_LINUX="auditwheel repair -w {dest_dir} {wheel} --exclude libarrow_python.so --exclude libarrow.so.1400"
+export CIBW_REPAIR_WHEEL_COMMAND_LINUX="auditwheel repair -w {dest_dir} {wheel} --exclude libarrow_python.so --exclude libarrow.so.1500"
 export CIBW_TEST_SKIP="*"
 export CIBW_TEST_EXTRAS=
 export CIBW_TEST_COMMAND="python -c 'from arcae.lib.arrow_tables import Table'"
 export CIBW_VERBOSITY=3
 
 echo "Creating VCPKG Binary Cache in $VCPKG_HOST_BINARY_CACHE"
 mkdir -p $VCPKG_HOST_BINARY_CACHE
```

### Comparing `arcae-0.2.2/src/arcae/CMakeLists.txt` & `arcae-0.2.3/src/arcae/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
+find_package(absl CONFIG REQUIRED)
 find_package(PkgConfig REQUIRED)
 find_program(CYTHON_FOUND "cython" REQUIRED)
 
 pkg_check_modules(casacore REQUIRED IMPORTED_TARGET casacore)
 
 add_custom_command(
     OUTPUT arrow_tables.cc
     VERBATIM
+    DEPENDS ${CMAKE_CURRENT_SOURCE_DIR}/arrow_tables.pyx
     COMMAND cython ${CMAKE_CURRENT_SOURCE_DIR}/arrow_tables.pyx
             --output-file ${CMAKE_CURRENT_BINARY_DIR}/arrow_tables.cc
             --cplus -vvv)
 
 python_add_library(arrow_tables MODULE WITH_SOABI arrow_tables.cc)
 
 target_link_libraries(arrow_tables PUBLIC arcae PkgConfig::casacore)
 target_link_directories(arrow_tables PUBLIC ${PYARROW_LIBDIRS})
 target_include_directories(arrow_tables PUBLIC
                             PkgConfig::casacore
+                            absl::span
                             ${PYARROW_INCLUDE}
                             ${NUMPY_INCLUDE}
                             ${CMAKE_SOURCE_DIR}/cpp)
-target_compile_options(arrow_tables PUBLIC "-D_GLIBCXX_USE_CXX11_ABI=1")
 
 string(REPLACE " " ";" _PYARROW_LIBS ${PYARROW_LIBS})
 
 foreach(PYARROW_LIB ${_PYARROW_LIBS})
     message("Linking arrow_tables against ${PYARROW_LIB}")
     target_link_libraries(arrow_tables PUBLIC ${PYARROW_LIB})
 endforeach()
```

### Comparing `arcae-0.2.2/src/arcae/__init__.py` & `arcae-0.2.3/src/arcae/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Needed to load in the arrow c++ shared libraries
 import pyarrow as pa  # noqa
 import os
 import sys
-from typing import TYPE_CHECKING
-
-__version__ = "0.2.2"
+from typing import Union, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from arcae.lib.arrow_tables import Table
 
+__version__ = "0.2.3"
+
 PYTHON_CASACORE_FOUND = "casacore" in sys.modules
 COEXIST_WITH_PYTHON_CASACORE = int(os.environ.get("ARCAE_WITH_CASACORE", 0)) != 0
 
 if PYTHON_CASACORE_FOUND and not COEXIST_WITH_PYTHON_CASACORE:
     raise RuntimeError(
         "python-casacore has already been imported and "
         "this may lead to extension module symbol conflicts "
         "and segfaults."
         "See https://github.com/ratt-ru/arcae/issues/72 "
         "for further information. "
         "Set ARCAE_WITH_CASACORE=1 if you wish to "
         "continue regardless.")
 
 
-def table(filename: str) -> "Table":
+def table(filename: str, readonly: bool = True, lockoptions: Union[str, dict] = "auto") -> "Table":
     # Defer cython module import, to avoid conflicts between arcae casacore libraries
     # and python-casacore casacore libraries
     from arcae.lib.arrow_tables import Table
-    return Table.from_filename(filename)
+    return Table.from_filename(filename, readonly, lockoptions)
```

### Comparing `arcae-0.2.2/src/arcae/applications/entrypoint.py` & `arcae-0.2.3/src/arcae/applications/entrypoint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import click
+try:
+    import click
+except ImportError as e:
+    raise ImportError("click is not installed.\n"
+                      "pip install arcae[applications]") from e
 
 from arcae.applications.ms_export import MSExporter
 
 @click.group()
 @click.pass_context
 @click.option("--debug/--no-debug", default=False)
 def main(ctx, debug):
```

### Comparing `arcae-0.2.2/src/arcae/applications/ms_export.py` & `arcae-0.2.3/src/arcae/applications/ms_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import json
 import os
 import os.path
 import shutil
 
-from rich.live import Live
-from rich.console import Group
-from rich.panel import Panel
-from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn, TextColumn
+try:
+    from rich.live import Live
+    from rich.console import Group
+    from rich.panel import Panel
+    from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn, TextColumn
+except ImportError as e:
+    raise ImportError("rich is not installed.\n"
+                      "pip install arcae[applications]")
 
 import arcae
 import pyarrow.parquet as pq
 
 
 class MSExporter:
     class UserInterface:
```

### Comparing `arcae-0.2.2/src/arcae/arrow_tables.pxd` & `arcae-0.2.3/src/arcae/arrow_tables.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,29 @@
 from libcpp.memory import shared_ptr
 from pyarrow.includes.common cimport *
 from pyarrow.includes.libarrow cimport *
 
 cdef extern from "<climits>" nogil:
     cdef unsigned int UINT_MAX
 
+cdef extern from "<casacore/casa/aipsxtype.h>" namespace "casacore" nogil:
+    ctypedef unsigned long long uInt64
+    ctypedef uInt64 rownr_t
+
+cdef extern from "<absl/types/span.h>" namespace "absl" nogil:
+    cdef cppclass Span[T]:
+        Span() except +
+        Span(T * array, size_t length) except +
+        Span(Span&) except +
+        size()
+
+cdef extern from "arcae/base_column_map.h" namespace "arcae" nogil:
+    ctypedef int64_t RowId
+    ctypedef Span[RowId] RowIds
+    ctypedef vector[RowIds] ColumnSelection
 
 cdef extern from "arcae/service_locator.h" namespace "arcae" nogil:
     cdef cppclass CServiceLocator" arcae::ServiceLocator":
         @staticmethod
         CConfiguration & configuration" ServiceLocator::configuration"()
 
 cdef extern from "arcae/configuration.h" namespace "arcae" nogil:
@@ -30,28 +45,33 @@
     cdef CResult[string] CMSDescriptor" arcae::MSDescriptor"(const string & table, bool complete)
 
 cdef extern from "arcae/safe_table_proxy.h" namespace "arcae" nogil:
     cdef cppclass CCasaTable" arcae::SafeTableProxy":
         @staticmethod
         CResult[bool] Close" SafeTableProxy::Close"()
 
-        CResult[shared_ptr[CTable]] ToArrow " SafeTableProxy::ToArrow"(unsigned int startrow, unsigned int nrow, const vector[string] & columns)
-        CResult[shared_ptr[CArray]] GetColumn " SafeTableProxy::GetColumn"(const string & column, unsigned int startrow, unsigned int nrow)
+        CResult[shared_ptr[CTable]] ToArrow " SafeTableProxy::ToArrow"( const ColumnSelection & selection, const vector[string] & columns)
+        CResult[shared_ptr[CArray]] GetColumn " SafeTableProxy::GetColumn"(const string & column, const ColumnSelection & selection)
+        CResult[bool] PutColumn " SafeTableProxy::PutColumn"(const string & column, const ColumnSelection & selection, const shared_ptr[CArray] & data)
         CResult[string] GetTableDescriptor " SafeTableProxy::GetTableDescriptor"()
         CResult[string] GetColumnDescriptor "SafeTableProxy::GetColumnDescriptor"(const string & column)
+        CResult[string] GetLockOptions "SafeTableProxy::GetLockOptions"()
+        CResult[bool] ReopenRW "SafeTableProxy::ReopenRW"()
         CResult[unsigned int] nRow " SafeTableProxy::nRow"()
         CResult[unsigned int] nColumns " SafeTableProxy::nColumns"()
         CResult[vector[string]] Columns " SafeTableProxy::Columns"()
         CResult[vector[shared_ptr[CCasaTable]]] Partition " SafeTableProxy::Partition"(const vector[string] & partition_columns, const vector[string] & sort_columns)
         CResult[bool] AddRows " SafeTableProxy::AddRows"(unsigned int nrows)
 
 
 cdef extern from "arcae/table_factory.h" namespace "arcae" nogil:
     cdef CResult[shared_ptr[CCasaTable]] COpenTable" arcae::OpenTable"(
-                                                    const string & filename)
+                                                    const string & filename,
+                                                    bool readonly,
+                                                    const string & json_lockoptions)
     cdef CResult[shared_ptr[CCasaTable]] CDefaultMS" arcae::DefaultMS"(
                                                     const string & name,
                                                     const string & subtable,
                                                     const string & json_table_desc,
                                                     const string & json_dminfo)
     cdef CResult[shared_ptr[CCasaTable]] CTaql" arcae::Taql"(
                                                     const string & taql)
```

### Comparing `arcae-0.2.2/src/arcae/config.py` & `arcae-0.2.3/src/arcae/config.py`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/src/arcae/tests/conftest.py` & `arcae-0.2.3/src/arcae/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,18 @@
             assert T.iscelldefined("UNCONSTRAINED", i)
 
     return table_name
 
 
 def casa_table_at_path(factory, *args):
     with mp.get_context("spawn").Pool(1) as pool:
-        return pool.apply(factory, args)
+        try:
+            return pool.apply_async(factory, args).get()
+        except ImportError as e:
+            pytest.importorskip(e.name)
 
 
 @pytest.fixture
 def column_case_table(tmp_path_factory):
     return casa_table_at_path(generate_column_cases_table,
                               tmp_path_factory.mktemp("column_cases"))
 
@@ -366,14 +369,24 @@
                 "valueType": "dcomplex",
             },
             "name": "VARDATA",
         },
         {
             "desc": {
                 "_c_order": True,
+                "comment": "FLAG column",
+                "ndim": 2,
+                "option": 0,
+                "valueType": "boolean",
+            },
+            "name": "FLAG",
+        },
+        {
+            "desc": {
+                "_c_order": True,
                 "comment": "TIME column",
                 "option": 0,
                 "valueType": "double",
             },
             "name": "TIME",
         },
         {
@@ -402,18 +415,19 @@
     table_name = os.path.join(path, "test.table")
     nrow = 3
 
     with pt.table(table_name, table_desc, nrow=nrow, ack=False) as T:
         for i in range(nrow):
             T.putcell("COMPLEX_DATA", i, np.full((2, 4), i + i*1j))
             T.putcell("FLOAT_DATA", i, np.full((2, 4), i))
-            T.putcell("VARDATA", i, np.full((2, i + 1), i))
+            T.putcell("VARDATA", i, np.full((i + 1, i + 1), i))
             T.putcell("TIME", i, i)
             T.putcell("STRING", i, str(i))
             T.putcell("NESTED_STRING", i, {"shape": (2, 4), "array": [str(i)] * 2 * 4})
+            T.putcell("FLAG", i, np.full((2, 4), (i % 2) != 1))
 
     return table_name
 
 
 @pytest.fixture
 def getcol_table(tmp_path_factory):
     return casa_table_at_path(generate_getcol_table,
```

### Comparing `arcae-0.2.2/src/arcae/tests/test_descriptor.py` & `arcae-0.2.3/src/arcae/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/src/arcae/tests/test_multithreaded_read.py` & `arcae-0.2.3/src/arcae/tests/test_multithreaded_read.py`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/src/arcae/tests/test_pytable.py` & `arcae-0.2.3/src/arcae/tests/test_pytable.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,31 +35,29 @@
             # Even though the column is unconstrained, ndim is the same
             "UNCONSTRAINED_SAME_NDIM",
             "VARIABLE",
             "VARIABLE_STRING"
         ]
 
     with arcae.table(column_case_table) as T:
-        assert sorted(T.to_arrow(0, 1).column_names) == [
+        assert sorted(T.to_arrow([[0, 1]]).column_names) == [
             "FIXED",
             "FIXED_STRING",
             "SCALAR",
             "SCALAR_STRING",
-            # When retrieving a single row, we can get values from an unconstrained column
-            "UNCONSTRAINED",
             "UNCONSTRAINED_SAME_NDIM",
             "VARIABLE",
             "VARIABLE_STRING"
         ]
 
     with arcae.table(column_case_table) as T:
-        assert sorted(T.to_arrow(0, 1, "VARIABLE").column_names) == ["VARIABLE"]
+        assert sorted(T.to_arrow([[0, 1]], "VARIABLE").column_names) == ["VARIABLE"]
 
     with arcae.table(column_case_table) as T:
-        assert sorted(T.to_arrow(0, 1, ["VARIABLE", "FIXED"]).column_names) == ["FIXED", "VARIABLE"]
+        assert sorted(T.to_arrow([[0, 1]], ["VARIABLE", "FIXED"]).column_names) == ["FIXED", "VARIABLE"]
 
 
 def test_column_cases(column_case_table, capfd):
     """ Test code paths """
     T = arcae.table(column_case_table).to_arrow()
 
     assert T.column("VARIABLE").to_pylist() == [
@@ -111,58 +109,145 @@
         assert T.column("COMPLEX").type == pa.list_(pa.list_(ComplexDoubleType()))
 
     with config.set(**{"casa.convert.strategy": "list"}):
         T = table.to_arrow()
         assert T.column("COMPLEX").type == pa.list_(pa.list_(pa.list_(pa.float64())))
 
 
+def test_unordered_select_roundtrip(tmp_path):
+    """ Tests writing and reading using indexing """
+    from arcae.lib.arrow_tables import ms_descriptor
+    from arcae.lib.arrow_tables import Table
+
+    ms = str(tmp_path / "unorded_select.ms")
+    table_desc = ms_descriptor("MAIN", complete=False)
+
+    table_desc["DATA"] = {
+        "comment": "Antenna number",
+        "dataManagerGroup": "StandardStMan",
+        "dataManagerType": "StandardStMan",
+        "keywords": {},
+        "ndim": 2,
+        "shape": [3, 3],
+        "maxlen": 0,
+        "option": 0,
+        "valueType": "float",
+    }
+
+    with Table.ms_from_descriptor(ms, table_desc=table_desc) as T:
+        T.addrows(3)
+        zeros = np.zeros((3, 3, 3), dtype=np.float32)
+        T.putcol("DATA", np.arange(3*3*3, dtype=np.float32).reshape(3, 3, 3))
+
+        assert_array_equal(T.getcol("DATA"), [
+            [[0, 1, 2], [3, 4, 5], [6, 7, 8]],
+            [[9, 10, 11], [12, 13, 14], [15, 16, 17]],
+            [[18, 19, 20], [21, 22, 23], [24, 25, 26]],
+        ])
+
+        index = (np.array([2, 0]), np.array([2, 0]), np.array([2, 0]))
+        expected = np.array([
+            [[26, 24], [20, 18]],
+            [[8, 6], [2, 0]]], np.float32)
+        assert_array_equal(T.getcol("DATA", index=index), expected)
+
+        T.putcol("DATA", zeros)
+        assert_array_equal(T.getcol("DATA"), 0)
+
+        T.putcol("DATA", expected, index=index)
+        assert_array_equal(T.getcol("DATA"), [
+            [[0, 0, 2], [0, 0, 0], [6, 0, 8]],
+            [[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+            [[18, 0, 20], [0, 0, 0], [24, 0, 26]],
+        ])
+
+        T.putcol("DATA", zeros)
+        assert_array_equal(T.getcol("DATA"), 0)
+
+        index = (np.array([0, 2]),)*3
+        T.putcol("DATA", expected, index=index)
+        assert_array_equal(T.getcol("DATA"), [
+            [[26, 0, 24], [0, 0, 0], [20, 0, 18]],
+            [[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+            [[8, 0, 6], [0, 0, 0], [2, 0, 0]],
+        ])
+
 def test_getcol(getcol_table):
-    T = arcae.table(getcol_table)
+    T = arcae.table(getcol_table, readonly=False)
 
     assert_array_equal(T.getcol("TIME"), [0, 1, 2])
+    assert_array_equal(T.getcol("TIME", (slice(0, 2),)), [0, 1])
+    assert_array_equal(T.getcol("TIME", (np.array([0, 1]),)), [0, 1])
+    assert_array_equal(T.getcol("TIME", (np.array([2, 0]),)), [2, 0])
+    assert_array_equal(T.getcol("TIME", (np.array([0, 2]),)), [0, 2])
     assert_array_equal(T.getcol("STRING"), ["0", "1", "2"])
 
     assert_array_equal(T.getcol("FLOAT_DATA"), [
         [[0, 0, 0, 0], [0, 0, 0, 0]],
         [[1, 1, 1, 1], [1, 1, 1, 1]],
         [[2, 2, 2, 2], [2, 2, 2, 2]]])
 
-    assert_array_equal(T.getcol("NESTED_STRING"), [
-        [["0", "0", "0", "0"], ["0", "0", "0", "0"]],
-        [["1", "1", "1", "1"], ["1", "1", "1", "1"]],
-        [["2", "2", "2", "2"], ["2", "2", "2", "2"]]])
-
-    assert_array_equal(T.getcol("COMPLEX_DATA"), [
-        [[0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j], [0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j]],
-        [[1 + 1j, 1 + 1j, 1 + 1j, 1 + 1j], [1 + 1j, 1 + 1j, 1 + 1j, 1 + 1j]],
-        [[2 + 2j, 2 + 2j, 2 + 2j, 2 + 2j], [2 + 2j, 2 + 2j, 2 + 2j, 2 + 2j]]])
-
-
-    for r in range(0, T.nrow(), 2):
-        assert_array_equal(
-            T.getcol("COMPLEX_DATA", startrow=r, nrow=1),
-            [[[r + r*1j]*4]*2])
+    assert_array_equal(T.getcol("FLOAT_DATA",
+        (slice(0, 2), slice(0, 2))), [
+            [[0, 0, 0, 0], [0, 0, 0, 0]],
+            [[1, 1, 1, 1], [1, 1, 1, 1]]])
+
+    assert_array_equal(T.getcol("FLOAT_DATA",
+            (np.array([0, 1]), np.array([0, 1]), np.array([0, 1]))), [
+                [[0, 0], [0, 0]],
+                [[1, 1], [1, 1]]])
+
+    # Test partial round-trip
+    index = (np.array([0, 1]), np.array([0, 1]), np.array([0, 1]))
+    float_data = np.array([
+        [[2, 3], [4, 5]],
+        [[9, 8], [7, 6]]], np.float32)
+
+    T.putcol("FLOAT_DATA", float_data + 1, index)
+    assert_array_equal(T.getcol("FLOAT_DATA", index), float_data + 1)
+
+    # Test complete round-trips
+    float_data = np.array([
+        [[3, 2, 1, 0], [3, 2, 1, 0]],
+        [[0, 1, 2, 3], [0, 1, 2, 3]],
+        [[2, 2, 2, 2], [2, 2, 2, 2]]], np.float32)
+
+    complex_data = np.array([
+        [[3 + 3j, 2 + 2j, 1 + 1j, 0 + 0j], [3 + 3j, 2 + 2j, 1 + 1j, 0 + 0j]],
+        [[0 + 0j, 1 + 1j, 2 + 2j, 3 + 3j], [0 + 0j, 1 + 1j, 2 + 2j, 3 + 3j]],
+        [[2 + 2j, 2 + 2j, 2 + 2j, 2 + 2j], [2 + 2j, 2 + 2j, 2 + 2j, 2 + 2j]]], np.complex128)
+
+    T.putcol("FLOAT_DATA", float_data + 1)
+    assert_array_equal(T.getcol("FLOAT_DATA"), float_data + 1)
+
+    T.putcol("COMPLEX_DATA", complex_data + 1 + 1j)
+    assert_array_equal(T.getcol("COMPLEX_DATA"), complex_data + 1 + 1j)
+
+    for r in range(T.nrow()):
+        row_data = T.getcol("VARDATA", index=(slice(r, r + 1),))
+        assert_array_equal(row_data, np.full((1, r + 1, r + 1), r))
 
     with pytest.raises(TypeError, match="variably shaped column VARDATA"):
         T.getcol("VARDATA")
 
     with pytest.raises(pa.lib.ArrowException, match="NONEXISTENT does not exist"):
         T.getcol("NONEXISTENT")
 
+
 def test_partial_read(sorting_table):
     """ Tests that partial reads work """
     T = arcae.table(sorting_table)
     full = T.to_arrow()
     nrows = [1, 2, 3, 4]
     assert sum(nrows) == len(full) == 10
 
     start = 0
 
     for nrow in nrows:
-        assert full.take(list(range(start, start + nrow))) == T.to_arrow(start, nrow)
+        assert full.take(list(range(start, start + nrow))) == T.to_arrow([slice(start, start+nrow)])
         start += nrow
 
 def test_table_taql(sorting_table):
     """ Tests that basic taql queries work """
     with arcae.table(sorting_table) as T:
         AT = T.to_arrow()
```

### Comparing `arcae-0.2.2/vcpkg/overlay-ports/casacore/001-casacore-cmake.patch` & `arcae-0.2.3/vcpkg/overlay-ports/casacore/001-casacore-cmake.patch`

 * *Files 6% similar despite different names*

```diff
@@ -111,14 +111,40 @@
  
  install (
  TARGETS casa_casa
 +EXPORT casacore
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib${LIB_SUFFIX}
  ARCHIVE DESTINATION lib${LIB_SUFFIX}
+diff --git a/casa/Json/JsonOut.h b/casa/Json/JsonOut.h
+index 460325102..becb19eec 100644
+--- a/casa/Json/JsonOut.h
++++ b/casa/Json/JsonOut.h
+@@ -176,6 +176,10 @@ namespace casacore { //# NAMESPACE CASACORE - BEGIN
+     void put (const DComplex& value);
+     void put (const char* value);
+     void put (const String& value);
++    // Put a Record which is written as a {} structure.
++    // The Record can be nested.
++    void put (const Record&);
++
+     // </group>
+ 
+     // Put a line defining an array value. Multi-dim arrays are written as
+@@ -217,10 +221,6 @@ namespace casacore { //# NAMESPACE CASACORE - BEGIN
+     // Write a key and valueholder.
+     void writeKV (const String& name, const ValueHolder& vh);
+ 
+-    // Put a Record which is written as a {} structure.
+-    // The Record can be nested.
+-    void put (const Record&);
+-
+     // Get the indentation after a name.
+     // It indents with the length of the name (including quotes and colon)
+     // with a maximum of 20 spaces.
 diff --git a/cmake/FindFFTW3.cmake b/cmake/FindFFTW3.cmake
 index 886f3bebb..66d117674 100644
 --- a/cmake/FindFFTW3.cmake
 +++ b/cmake/FindFFTW3.cmake
 @@ -58,15 +58,6 @@ foreach(_comp ${_components})
    endif(_comp STREQUAL "single")
  endforeach(_comp ${_components})
@@ -559,7 +585,35 @@
      TSMOption      tsmOption_p;
      //# cache of open (plain) tables
 -    static TableCache theirTableCache;
 +    static thread_local TableCache theirTableCache;
  };
  
  
+diff --git a/tables/Tables/TableProxy.cc b/tables/Tables/TableProxy.cc
+index 66865e52d..4bd489373 100644
+--- a/tables/Tables/TableProxy.cc
++++ b/tables/Tables/TableProxy.cc
+@@ -273,6 +273,9 @@ Record TableProxy::lockOptions()
+       option = "autonoread";
+     }
+     break;
++  case TableLock::NoLocking:
++    option = "nolock";
++    break;
+   default:
+     option = "unknown";
+   }
+@@ -3405,10 +3408,12 @@ TableLock TableProxy::makeLockOptions (const Record& options)
+     opt = TableLock::PermanentLocking;
+   } else if (str == "permanentwait") {
+     opt = TableLock::PermanentLockingWait;
++  } else if (str == "nolock") {
++    opt = TableLock::NoLocking;
+   } else {
+     throw TableError ("'" + str + "' is an unknown lock option; valid are "
+ 		      "default,auto,autonoread,user,usernoread,permanent,"
+-		      "permanentwait");
++		      "permanentwait,lock");
+   }
+   if (options.nfields() == 1) {
+     return TableLock(opt);
```

### Comparing `arcae-0.2.2/vcpkg/overlay-ports/casacore/portfile.cmake` & `arcae-0.2.3/vcpkg/overlay-ports/casacore/portfile.cmake`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/vcpkg/overlay-ports/casacore/vcpkg.json` & `arcae-0.2.3/vcpkg/overlay-ports/casacore/vcpkg.json`

 * *Files identical despite different names*

### Comparing `arcae-0.2.2/PKG-INFO` & `arcae-0.2.3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,117 @@
-Metadata-Version: 2.1
-Name: arcae
-Version: 0.2.2
-Summary: Arrow bindings for casacore
-Author-Email: Simon Perkins <simon.perkins@gmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, Rhodes University Centre for Radio Astronomy Techniques & Technologies (RATT)
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Project-URL: Repository, https://github.com/ratt-ru/arcae
-Requires-Dist: appdirs
-Requires-Dist: click
-Requires-Dist: rich
-Requires-Dist: pyarrow==14.0.1
-Requires-Dist: black==22.1.0; extra == "dev"
-Requires-Dist: flake8==4.0.1; extra == "dev"
-Requires-Dist: tbump; extra == "dev"
-Requires-Dist: duckdb; extra == "test"
-Requires-Dist: pytest>=7.0.0; extra == "test"
-Requires-Dist: python-casacore>=3.5.0; extra == "test"
-Requires-Dist: requests; extra == "test"
-Provides-Extra: dev
-Provides-Extra: test
-Description-Content-Type: text/x-rst
-
 C++ and Python Arrow Bindings for casacore
 ==========================================
 
+``arcae`` implements a limited subset of functionality from the more mature python-casacore_ package. It bypasses some existing limitations in python-casacore to provide safe, multi-threadded access to CASA formats, thereby enabling export into newer cloud native formats such as Apache Arrow and Zarr.
 
 Rationale
 ---------
 
-* The structure of Apache Arrow Tables is highly similar to that of CASA Tables
+``casacore`` and the ``python-casacore`` Python bindings provide access to the CASA Table Data System (CTDS) and Measurement Sets created within this system. The CTDS, as of casacore 3.5.0 is subject to the following limitations:
+
+* Access from multiple threads is unsafe.
+
+    - https://github.com/casacore/casacore/issues/1038
+    - https://github.com/casacore/casacore/issues/1163
+
+* ``python-casacore`` doesn't drop the Global Interpreter Lock
+
+    - https://github.com/casacore/python-casacore/pull/209
+
+Resolving these concerns is potentially a major effort, involving invasive changes across the CTDS system.
+
+In the time since the CTDS was developed, newer, open-source formats such as Apache Arrow and Zarr have been developed that are suitable for representing Radio Astronomy data.
+
+* The Apache Arrow project defines a programming language portable in-memory columnar storage format.
+* Translating CTDS data to Arrow is relatively simple, with some limitations mentioned below.
 * It's easy to convert Arrow Tables between many different languages
-* Once in Apache Arrow format, it is easy to store data in modern, cloud-native disk formats such as parquet and orc.
+* Once in Apache Arrow format, it is easy to store data in modern, cloud-native disk formats such as parquet and Zarr.
 * Converting CASA Tables to Arrow in the C++ layer avoids the GIL
 * Access to non thread-safe CASA Tables is constrained to a ThreadPool containing a single thread
-* It also allows us to write astrometric routines in C++, potentially side-stepping thread-safety
-  and GIL issues with the CASA Measures server.
+* It also allows us to write astrometric routines in C++, potentially side-stepping thread-safety and GIL issues with the CASA Measures server.
+
+Limitations
+-----------
 
+Arrow supports both 1D arrays and nested structures:
 
-Build Wheel Locally
--------------------
+1. Fixed shape multi-dimensional data (i.e. visibility data) is currently represented as nested `FixedSizeListArrays <fixed_size_list_layout_>`_ .
+2. Variably-shaped multi-dimensional (i.e. subtable data) is currently represented as nested `ListArrays <variable_size_list_layout_>`_.
+3. Complex values are represented as an extra `FixedSizeListArray <fixed_size_list_layout_>`_ nesting of two floats.
+4. Currently, it is not trivially trivial (repitition intendead here) to convert between the above and numpy via ``to_numpy`` calls on Arrow Arrays, but it is relatively trivial to reinterpret the underlying data buffers from either API. This is done transparently in ``getcol`` and ``putcol`` funcions (see usage below).
 
-In the user or, even better, a virtual environment:
+Going forward, `FixedShapeTensorArray <fixed_shape_tensor_array_>`_ and `VariableShapeTensorArray <variable_shape_tensor_array_>`_ will provide more ergonomic structures for representing multi-dimensional data. First class support for complex values in Apache Arrow will require implementing a `C++ extension type <cpp_extension_type_>`_ within Arrow itself:
 
-.. code-block:: python
+Some other edge cases have not yet been implemented, but could be with some thought.
 
-  $ pip install -U pip cibuildwheel
-  $ bash scripts/run_cbuildwheel.sh -p 3.10
+* Columns with unconstrained rank (ndim == -1) whose rows, in practice, have differing dimensions.
+  Unconstrained rank columns whose rows actually have the same rank are catered for.
+* Not yet able to handle TpRecord columns. Probably simplest to convert these rows to json and store as a string.
+* Not yet able to handle TpQuantity columns. Possible to represent as a run-time parametric Arrow DataType.
 
-.. warning::
-  Only linux wheels are currently supported.
 
-Local Development
------------------
+Installation
+------------
 
-In the directory containing the source, setup your development environment as follows:
+Binary wheels are providing for Linux and MacOSX for both x86_64 and arm64 architectures
 
-.. code-block:: python
+.. code-block:: bash
 
-  $ pip install -U pip virtualenv
-  $ virtualenv -p python3.10 /venv/arcaedev
-  $ . /venv/arcaedev/bin/activate
-  (arcaedev) export VCPKG_TARGET_TRIPLET=x64-linux-dynamic-cxx17-abi1-dbg
-  (arcaedev) pip install -e .[test]
-  (arcaedev) export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$(pwd)/vcpkg/installed/$VCPKG_TARGET_TRIPLET/lib
-  (arcaedev) py.test -s -vvv --pyargs arcae
+  $ pip install arcae
 
 Usage
 -----
 
-Example Usage:
+Example usage with Arrow Tables:
 
   .. code-block:: python
 
     import json
     from pprint import pprint
 
     import arcae
-    import pandas as pd
     import pyarrow as pa
     import pyarrow.parquet as pq
 
     # Obtain (partial) Apache Arrow Table from a CASA Table
     casa_table = arcae.table("/path/to/measurementset.ms")
     arrow_table = casa_table.to_arrow()        # read entire table
-    arrow_table = casa_table.to_arrow(10, 20)  # startrow, nrow
+    arrow_table = casa_table.to_arrow(index=(slice(10, 20),)
     assert isinstance(arrow_table, pa.Table)
 
     # Print JSON-encoded Table and Column keywords
     pprint(json.loads(arrow_table.schema.metadata[b"__arcae_metadata__"]))
     pprint(json.loads(arrow_table.schema.field("DATA").metadata[b"__arcae_metadata__"]))
 
-    # Extract Arrow Table columns into numpy arrays
-    time = arrow_table.column("TIME").to_numpy()
-    data = arrow_table.column("DATA").to_numpy()   # currently, arrays of object arrays, overly slow and memory hungry
-    df = arrow_table.to_pandas()                   # currently slow, memory hungry due to arrays of object arrays
-
-    # Write Arrow Table to parquet file
     pq.write_table(arrow_table, "measurementset.parquet")
 
+Some reading and writing functionality from python-casacore_ is replicated,
+with added support for some `NumPy Advanced Indexing <numpy_advanced_indexing_>`_.
+
+  .. code-block:: python
+
+    casa_table = arcae.table("/path/to/measurementset.ms", readonly=False)
+    # Get rows 10 and 2, and channels 16 to 32, and all correlations
+    data = casa_table.getcol("DATA", index=([10, 2], slice(16, 32), None)
+    # Write some modified data back
+    casa_table.putcol("DATA", data + 1*1j, index=([10, 2], slice(16, 32), None)
 
 See the test cases for further use cases.
 
 
 Exporting Measurement Sets to Arrow Parquet Datasets
 ----------------------------------------------------
 
-An export script is available:
+Install the ``applications`` optional extra.
+
+  .. code-block:: bash
+
+    pip install arcae[applications]
+
+Then, an export script is available:
 
 .. code-block:: bash
 
   $ arcae export /path/to/the.ms --nrow 50000
   $ tree output.arrow/
   output.arrow/
   ├── ANTENNA
@@ -180,34 +154,24 @@
 .. code-block:: python
 
     >>> import pyarrow as pa
     >>> import pyarrow.dataset as pad
     >>> main_ds = pad.dataset("output.arrow/MAIN")
     >>> spw_ds = pad.dataset("output.arrow/SPECTRAL_WINDOW")
 
-Limitations
------------
-
-Some edge cases have not yet been implemented, but could be with some thought.
-
-* Columns with unconstrained rank (ndim == -1) whose rows, in practice, have differing dimensions.
-  Unconstrained rank columns whose rows actually have the same rank are catered for.
-* Not yet able to handle TpRecord columns. Probably simplest to convert these rows to json and store as a string.
-* Not yet able to handle TpQuantity columns. Possible to represent as a run-time parametric Arrow DataType.
-* `to_numpy()` conversion of nested lists produces nested numpy arrays, instead of tensors.
-  This is `possible <daskms_ext_types_>`_ but requires some changes to how
-  `C++ Extension Types are exposed in Python <arrow_python_expose_cpp_ext_types_>`_.
-
-
-
 Etymology
 ---------
 
 Noun: **arca** f (genitive **arcae**); first declension
 A chest, box, coffer, safe (safe place for storing items, or anything of a similar shape)
 
 Pronounced: `ar-ki <arcae_pronounce_>`_.
 
 
-.. _daskms_ext_types: https://github.com/ratt-ru/dask-ms/blob/1ff73ce3a60ea6479e40fc8cf440fd8d077e3d26/daskms/experimental/arrow/extension_types.py#L120-L152
-.. _arrow_python_expose_cpp_ext_types: https://github.com/apache/arrow/issues/33997
+.. _python-casacore: https://github.com/casacore/python-cascore
+.. _fixed_size_list_layout: https://arrow.apache.org/docs/format/Columnar.html#fixed-size-list-layout
+.. _variable_size_list_layout: https://arrow.apache.org/docs/format/Columnar.html#variable-size-list-layout
+.. _fixed_shape_tensor_array: https://arrow.apache.org/docs/python/generated/pyarrow.FixedShapeTensorArray.html
+.. _variable_shape_tensor_array: https://github.com/apache/arrow/pull/38008
+.. _numpy_advanced_indexing: https://numpy.org/doc/stable/user/basics.indexing.html#advanced-indexing
+.. _cpp_extension_type: https://arrow.apache.org/docs/cpp/api/datatype.html#extension-types
 .. _arcae_pronounce: https://translate.google.com/?sl=la&tl=en&text=arcae%0A&op=translate
```

