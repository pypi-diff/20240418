# Comparing `tmp/pykwl-0.0.4.tar.gz` & `tmp/pykwl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.4.tar", last modified: Wed Apr 17 16:47:56 2024, max compression
+gzip compressed data, was "pykwl-0.0.5.tar", last modified: Wed Apr 17 23:19:03 2024, max compression
```

## Comparing `pykwl-0.0.4.tar` & `pykwl-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 16:47:44.000000 pykwl-0.0.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 16:47:44.000000 pykwl-0.0.4/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 16:47:44.000000 pykwl-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 16:47:44.000000 pykwl-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 16:47:56.826912 pykwl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 16:47:44.000000 pykwl-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 16:47:44.000000 pykwl-0.0.4/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 16:47:44.000000 pykwl-0.0.4/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 16:47:44.000000 pykwl-0.0.4/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 16:47:44.000000 pykwl-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:47:56.826912 pykwl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 16:47:44.000000 pykwl-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 23:18:54.000000 pykwl-0.0.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 23:18:54.000000 pykwl-0.0.5/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 23:18:54.000000 pykwl-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 23:18:54.000000 pykwl-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 23:19:03.133856 pykwl-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 23:18:54.000000 pykwl-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 23:18:54.000000 pykwl-0.0.5/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 23:18:54.000000 pykwl-0.0.5/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 23:18:54.000000 pykwl-0.0.5/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 23:18:54.000000 pykwl-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:19:03.133856 pykwl-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 23:18:54.000000 pykwl-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.4/CMakeLists.txt` & `pykwl-0.0.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/Config.cmake.in` & `pykwl-0.0.5/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/LICENSE` & `pykwl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/README.md` & `pykwl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/cmake/configure_ccache.cmake` & `pykwl-0.0.5/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.5/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/include/wl/details/graph.hpp` & `pykwl-0.0.5/include/wl/details/graph.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.5/include/wl/details/weisfeiler_leman.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/pyproject.toml` & `pykwl-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/python/src/pykwl/bindings.cpp` & `pykwl-0.0.5/python/src/pykwl/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.5/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/setup.py` & `pykwl-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.4/src/CMakeLists.txt` & `pykwl-0.0.5/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/src/graph.cpp` & `pykwl-0.0.5/src/graph.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.4/src/weisfeiler_leman.cpp` & `pykwl-0.0.5/src/weisfeiler_leman.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #include "wl/details/weisfeiler_leman.hpp"
 
 #include <algorithm>
 #include <cassert>
-#include <numeric>
 #include <stdexcept>
 #include <tuple>
 #include <unordered_map>
 #include <utility>
 #include <vector>
 
 namespace wl
@@ -30,30 +29,26 @@
     return result;
 }
 
 inline static void lexical_sort(std::vector<int>& items1, std::vector<int>& items2)
 {
     assert(items1.size() == items2.size());
 
-    std::vector<size_t> indices(items1.size());
-    std::iota(indices.begin(), indices.end(), 0);
+    std::vector<std::pair<int, int>> paired_items(items1.size());
+    for (size_t i = 0; i < items1.size(); ++i)
+    {
+        paired_items[i] = { items1[i], items2[i] };
+    }
 
-    // Sort the indices based on corresponding values in items1 and items2
-    std::sort(indices.begin(), indices.end(), [&](size_t i, size_t j) { return std::tie(items1[i], items2[i]) < std::tie(items1[j], items2[j]); });
+    std::sort(paired_items.begin(), paired_items.end());
 
-    // Reorder items1 and items2 according to the sorted indices in-place
-    for (size_t i = 0; i < indices.size(); ++i)
+    for (size_t i = 0; i < items1.size(); ++i)
     {
-        while (i != indices[i])
-        {
-            size_t next = indices[i];
-            std::swap(items1[i], items1[next]);
-            std::swap(items2[i], items2[next]);
-            std::swap(indices[i], indices[next]);
-        }
+        items1[i] = paired_items[i].first;
+        items2[i] = paired_items[i].second;
     }
 }
 
 inline static std::pair<std::vector<int>, std::vector<int>> get_frequencies(const std::vector<int>& items)
 {
     std::unordered_map<int, int> frequencies;
```

