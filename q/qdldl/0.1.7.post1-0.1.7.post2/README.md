# Comparing `tmp/qdldl-0.1.7.post1.tar.gz` & `tmp/qdldl-0.1.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/qdldl-0.1.7.post1.tar", last modified: Fri Apr  5 10:15:35 2024, max compression
+gzip compressed data, was "qdldl-0.1.7.post2.tar", last modified: Thu Apr 18 17:44:21 2024, max compression
```

## Comparing `qdldl-0.1.7.post1.tar` & `qdldl-0.1.7.post2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/amd/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/amd/include/
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/include/SuiteSparse_config.h
--rw-r--r--   0 runner    (1001) docker     (127)    17829 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/include/amd.h
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/include/amd_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/include/perm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/amd/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/SuiteSparse_config.c
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_1.c
--rw-r--r--   0 runner    (1001) docker     (127)    64841 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_aat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_control.c
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_defaults.c
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_info.c
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_order.c
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_post_tree.c
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_postorder.c
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_preprocess.c
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/amd_valid.c
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/c/amd/src/perm.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/.git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/configure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/configure/qdldl_types.h.in
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/configure/qdldl_version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/examples/example.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/include/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/include/qdldl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/src/qdldl.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/c/qdldl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/minunit.h
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/qdldl_tester.c
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_basic.h
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_identity.h
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_osqp_kkt.h
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_rank_deficient.h
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_singleton.h
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_sym_structure.h
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_tril_structure.h
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_two_by_two.h
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 10:11:31.000000 qdldl-0.1.7.post1/c/qdldl/tests/test_zero_on_diag.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/cpp/qdldl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/cpp/qdldl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/cpp/wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/qdldl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:15:35.000000 qdldl-0.1.7.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/tests/test_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/tests/test_solve_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 10:11:30.000000 qdldl-0.1.7.post1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.961969 qdldl-0.1.7.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-18 17:44:21.961969 qdldl-0.1.7.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.949968 qdldl-0.1.7.post2/c/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.949968 qdldl-0.1.7.post2/c/amd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.953969 qdldl-0.1.7.post2/c/amd/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/include/SuiteSparse_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17829 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/include/amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/include/amd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/include/perm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.953969 qdldl-0.1.7.post2/c/amd/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/SuiteSparse_config.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_1.c
+-rw-r--r--   0 runner    (1001) docker     (127)    64841 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_aat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_control.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_info.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_order.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/amd_valid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/c/amd/src/perm.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.953969 qdldl-0.1.7.post2/c/qdldl/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/.git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.949968 qdldl-0.1.7.post2/c/qdldl/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/configure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/configure/qdldl_types.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/configure/qdldl_version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/examples/example.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/include/qdldl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/src/qdldl.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/c/qdldl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/minunit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/qdldl_tester.c
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_basic.h
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_identity.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_osqp_kkt.h
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_rank_deficient.h
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_singleton.h
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_sym_structure.h
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_tril_structure.h
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_two_by_two.h
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-18 17:39:50.000000 qdldl-0.1.7.post2/c/qdldl/tests/test_zero_on_diag.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.957969 qdldl-0.1.7.post2/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/cpp/qdldl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/cpp/qdldl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/cpp/wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.961969 qdldl-0.1.7.post2/qdldl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-18 17:44:21.000000 qdldl-0.1.7.post2/qdldl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-18 17:44:21.000000 qdldl-0.1.7.post2/qdldl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:44:21.000000 qdldl-0.1.7.post2/qdldl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 17:44:21.000000 qdldl-0.1.7.post2/qdldl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 17:44:21.000000 qdldl-0.1.7.post2/qdldl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:44:21.961969 qdldl-0.1.7.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:21.961969 qdldl-0.1.7.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/tests/test_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/tests/test_solve_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 17:39:49.000000 qdldl-0.1.7.post2/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qdldl-0.1.7.post1/LICENSE` & `qdldl-0.1.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/PKG-INFO` & `qdldl-0.1.7.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 Metadata-Version: 2.1
 Name: qdldl
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: QDLDL, a free LDL factorization routine.
 Home-page: https://github.com/oxfordcontrol/qdldl-python/
 Author: Bartolomeo Stellato, Paul Goulart, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
-Description: # qdldl-python
-        
-        ![github actions](https://github.com/oxfordcontrol/qdldl-python/workflows/Build/badge.svg?branch=master)
-        
-        Python interface to the [QDLDL](https://github.com/oxfordcontrol/qdldl/)
-        free LDL factorization routine for quasi-definite linear systems: `Ax =
-        b`.
-        
-        ## Installation
-        
-        This package can be directly installed via pip,
-        
-        ```
-        pip install qdldl
-        ```
-        
-        ## Usage
-        
-        Initialize the factorization with
-        
-        ```
-        import qdldl
-        F = qdldl.Solver(A)
-        ```
-        
-        where `A` must be a square quasi-definite matrix in [scipy sparse CSC
-        format](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html).
-        
-        The algorithm internally converts the matrix into upper triangular format. If `A` is already upper-triangular, you can specify it with the argument `upper=True` to the `qdldl.Solver` constructor.
-        
-        To solve the linear system for a right-hand side `b`, just write
-        
-        ```
-        x = F.solve(b)
-        ```
-        
-        To update the factorization without changing the sparsity pattern of `A` you can run
-        
-        ```
-        F.update(A_new)
-        ```
-        
-        where `A_new` is a sparse matrix in CSR format with the same sparsity pattern as `A`.
-        
-        The algorithm internally converts `A_new` into upper triangular format. If `A_new` is already upper-triangular, you can specify it with the argument `upper=True` to the `F.update` function.
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.7
+Requires-Dist: scipy>=0.13.2
+
+# qdldl-python
+
+![github actions](https://github.com/oxfordcontrol/qdldl-python/workflows/Build/badge.svg?branch=master)
+
+Python interface to the [QDLDL](https://github.com/oxfordcontrol/qdldl/)
+free LDL factorization routine for quasi-definite linear systems: `Ax =
+b`.
+
+## Installation
+
+This package can be directly installed via pip,
+
+```
+pip install qdldl
+```
+
+## Usage
+
+Initialize the factorization with
+
+```
+import qdldl
+F = qdldl.Solver(A)
+```
+
+where `A` must be a square quasi-definite matrix in [scipy sparse CSC
+format](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html).
+
+The algorithm internally converts the matrix into upper triangular format. If `A` is already upper-triangular, you can specify it with the argument `upper=True` to the `qdldl.Solver` constructor.
+
+To solve the linear system for a right-hand side `b`, just write
+
+```
+x = F.solve(b)
+```
+
+To update the factorization without changing the sparsity pattern of `A` you can run
+
+```
+F.update(A_new)
+```
+
+where `A_new` is a sparse matrix in CSR format with the same sparsity pattern as `A`.
+
+The algorithm internally converts `A_new` into upper triangular format. If `A_new` is already upper-triangular, you can specify it with the argument `upper=True` to the `F.update` function.
+
```

### Comparing `qdldl-0.1.7.post1/README.md` & `qdldl-0.1.7.post2/README.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/CMakeLists.txt` & `qdldl-0.1.7.post2/c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/LICENSE` & `qdldl-0.1.7.post2/c/amd/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/include/SuiteSparse_config.h` & `qdldl-0.1.7.post2/c/amd/include/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/include/amd.h` & `qdldl-0.1.7.post2/c/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/include/amd_internal.h` & `qdldl-0.1.7.post2/c/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/include/perm.h` & `qdldl-0.1.7.post2/c/amd/include/perm.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/SuiteSparse_config.c` & `qdldl-0.1.7.post2/c/amd/src/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_1.c` & `qdldl-0.1.7.post2/c/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_2.c` & `qdldl-0.1.7.post2/c/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_aat.c` & `qdldl-0.1.7.post2/c/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_control.c` & `qdldl-0.1.7.post2/c/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_defaults.c` & `qdldl-0.1.7.post2/c/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_info.c` & `qdldl-0.1.7.post2/c/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_order.c` & `qdldl-0.1.7.post2/c/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_post_tree.c` & `qdldl-0.1.7.post2/c/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_postorder.c` & `qdldl-0.1.7.post2/c/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_preprocess.c` & `qdldl-0.1.7.post2/c/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/amd_valid.c` & `qdldl-0.1.7.post2/c/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/amd/src/perm.c` & `qdldl-0.1.7.post2/c/amd/src/perm.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/.github/workflows/ci.yml` & `qdldl-0.1.7.post2/c/qdldl/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/CHANGELOG.md` & `qdldl-0.1.7.post2/c/qdldl/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/CMakeLists.txt` & `qdldl-0.1.7.post2/c/qdldl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/LICENSE` & `qdldl-0.1.7.post2/c/qdldl/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/README.md` & `qdldl-0.1.7.post2/c/qdldl/README.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/configure/cmake/cmake_uninstall.cmake.in` & `qdldl-0.1.7.post2/c/qdldl/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/configure/qdldl_types.h.in` & `qdldl-0.1.7.post2/c/qdldl/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/examples/example.c` & `qdldl-0.1.7.post2/c/qdldl/examples/example.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/include/qdldl.h` & `qdldl-0.1.7.post2/c/qdldl/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/src/qdldl.c` & `qdldl-0.1.7.post2/c/qdldl/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/tests/CMakeLists.txt` & `qdldl-0.1.7.post2/c/qdldl/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/tests/qdldl_tester.c` & `qdldl-0.1.7.post2/c/qdldl/tests/qdldl_tester.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/tests/test_basic.h` & `qdldl-0.1.7.post2/c/qdldl/tests/test_basic.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/tests/test_osqp_kkt.h` & `qdldl-0.1.7.post2/c/qdldl/tests/test_osqp_kkt.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/c/qdldl/tests/test_zero_on_diag.h` & `qdldl-0.1.7.post2/c/qdldl/tests/test_zero_on_diag.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/cpp/qdldl.cpp` & `qdldl-0.1.7.post2/cpp/qdldl.cpp`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/cpp/qdldl.hpp` & `qdldl-0.1.7.post2/cpp/qdldl.hpp`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/cpp/wrapper.cpp` & `qdldl-0.1.7.post2/cpp/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/qdldl.egg-info/PKG-INFO` & `qdldl-0.1.7.post2/qdldl.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 Metadata-Version: 2.1
 Name: qdldl
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: QDLDL, a free LDL factorization routine.
 Home-page: https://github.com/oxfordcontrol/qdldl-python/
 Author: Bartolomeo Stellato, Paul Goulart, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
-Description: # qdldl-python
-        
-        ![github actions](https://github.com/oxfordcontrol/qdldl-python/workflows/Build/badge.svg?branch=master)
-        
-        Python interface to the [QDLDL](https://github.com/oxfordcontrol/qdldl/)
-        free LDL factorization routine for quasi-definite linear systems: `Ax =
-        b`.
-        
-        ## Installation
-        
-        This package can be directly installed via pip,
-        
-        ```
-        pip install qdldl
-        ```
-        
-        ## Usage
-        
-        Initialize the factorization with
-        
-        ```
-        import qdldl
-        F = qdldl.Solver(A)
-        ```
-        
-        where `A` must be a square quasi-definite matrix in [scipy sparse CSC
-        format](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html).
-        
-        The algorithm internally converts the matrix into upper triangular format. If `A` is already upper-triangular, you can specify it with the argument `upper=True` to the `qdldl.Solver` constructor.
-        
-        To solve the linear system for a right-hand side `b`, just write
-        
-        ```
-        x = F.solve(b)
-        ```
-        
-        To update the factorization without changing the sparsity pattern of `A` you can run
-        
-        ```
-        F.update(A_new)
-        ```
-        
-        where `A_new` is a sparse matrix in CSR format with the same sparsity pattern as `A`.
-        
-        The algorithm internally converts `A_new` into upper triangular format. If `A_new` is already upper-triangular, you can specify it with the argument `upper=True` to the `F.update` function.
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.7
+Requires-Dist: scipy>=0.13.2
+
+# qdldl-python
+
+![github actions](https://github.com/oxfordcontrol/qdldl-python/workflows/Build/badge.svg?branch=master)
+
+Python interface to the [QDLDL](https://github.com/oxfordcontrol/qdldl/)
+free LDL factorization routine for quasi-definite linear systems: `Ax =
+b`.
+
+## Installation
+
+This package can be directly installed via pip,
+
+```
+pip install qdldl
+```
+
+## Usage
+
+Initialize the factorization with
+
+```
+import qdldl
+F = qdldl.Solver(A)
+```
+
+where `A` must be a square quasi-definite matrix in [scipy sparse CSC
+format](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html).
+
+The algorithm internally converts the matrix into upper triangular format. If `A` is already upper-triangular, you can specify it with the argument `upper=True` to the `qdldl.Solver` constructor.
+
+To solve the linear system for a right-hand side `b`, just write
+
+```
+x = F.solve(b)
+```
+
+To update the factorization without changing the sparsity pattern of `A` you can run
+
+```
+F.update(A_new)
+```
+
+where `A_new` is a sparse matrix in CSR format with the same sparsity pattern as `A`.
+
+The algorithm internally converts `A_new` into upper triangular format. If `A_new` is already upper-triangular, you can specify it with the argument `upper=True` to the `F.update` function.
+
```

### Comparing `qdldl-0.1.7.post1/qdldl.egg-info/SOURCES.txt` & `qdldl-0.1.7.post2/qdldl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/setup.py` & `qdldl-0.1.7.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='qdldl',
-      version='0.1.7.post1',
+      version='0.1.7.post2',
       author='Bartolomeo Stellato, Paul Goulart, Goran Banjac',
       author_email='bartolomeo.stellato@gmail.com',
       description='QDLDL, a free LDL factorization routine.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       package_dir={'qdldl': 'module'},
       include_package_data=True,  # Include package data from MANIFEST.in
```

### Comparing `qdldl-0.1.7.post1/tests/test_errors.py` & `qdldl-0.1.7.post2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/tests/test_factors.py` & `qdldl-0.1.7.post2/tests/test_factors.py`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7.post1/tests/test_solve_ls.py` & `qdldl-0.1.7.post2/tests/test_solve_ls.py`

 * *Files identical despite different names*

