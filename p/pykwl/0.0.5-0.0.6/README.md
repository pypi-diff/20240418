# Comparing `tmp/pykwl-0.0.5.tar.gz` & `tmp/pykwl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.5.tar", last modified: Wed Apr 17 23:19:03 2024, max compression
+gzip compressed data, was "pykwl-0.0.6.tar", last modified: Thu Apr 18 11:30:58 2024, max compression
```

## Comparing `pykwl-0.0.5.tar` & `pykwl-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 23:18:54.000000 pykwl-0.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 23:18:54.000000 pykwl-0.0.5/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 23:18:54.000000 pykwl-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 23:18:54.000000 pykwl-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 23:19:03.133856 pykwl-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 23:18:54.000000 pykwl-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 23:18:54.000000 pykwl-0.0.5/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 23:18:54.000000 pykwl-0.0.5/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 23:18:54.000000 pykwl-0.0.5/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 23:18:54.000000 pykwl-0.0.5/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 23:18:54.000000 pykwl-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.129856 pykwl-0.0.5/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 23:18:54.000000 pykwl-0.0.5/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 23:19:03.000000 pykwl-0.0.5/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:19:03.133856 pykwl-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 23:18:54.000000 pykwl-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-17 23:18:54.000000 pykwl-0.0.5/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:19:03.133856 pykwl-0.0.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:18:54.000000 pykwl-0.0.5/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-18 11:30:48.000000 pykwl-0.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 11:30:48.000000 pykwl-0.0.6/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 11:30:48.000000 pykwl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 11:30:48.000000 pykwl-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 11:30:58.489852 pykwl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 11:30:48.000000 pykwl-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-18 11:30:48.000000 pykwl-0.0.6/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 11:30:48.000000 pykwl-0.0.6/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 11:30:48.000000 pykwl-0.0.6/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-18 11:30:48.000000 pykwl-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:30:58.489852 pykwl-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-18 11:30:48.000000 pykwl-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.5/CMakeLists.txt` & `pykwl-0.0.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/Config.cmake.in` & `pykwl-0.0.6/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/LICENSE` & `pykwl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/README.md` & `pykwl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/cmake/configure_ccache.cmake` & `pykwl-0.0.6/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.6/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/include/wl/details/graph.hpp` & `pykwl-0.0.6/include/wl/details/graph.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,25 @@
 private:
     std::vector<std::vector<int>> m_outgoing_edges;
     std::vector<std::vector<int>> m_ingoing_edges;
     std::vector<std::vector<int>> m_outgoing_adjacent;
     std::vector<std::vector<int>> m_ingoing_adjacent;
     std::vector<std::unordered_map<int, std::vector<int>>> m_outgoing_edges_between;
     std::vector<std::unordered_map<int, std::vector<int>>> m_ingoing_edges_between;
-    std::vector<int> m_edge_sources;
-    std::vector<int> m_edge_destinations;
     std::vector<int> m_node_labels;
     std::vector<int> m_edge_labels;
     bool m_directed;
 
 public:
     explicit Graph(bool directed);
 
     int add_node(int label = 0);
 
     void add_edge(int src_node, int dst_node, int label = 0);
 
-    int get_source(int edge) const;
-
-    int get_destination(int edge) const;
-
     const std::vector<int>& get_outbound_edges(int node) const;
 
     const std::vector<int>& get_inbound_edges(int node) const;
 
     const std::vector<int>& get_outbound_adjacent(int node) const;
 
     const std::vector<int>& get_inbound_adjacent(int node) const;
@@ -50,12 +44,14 @@
     int get_edge_label(int edge) const;
 
     const std::vector<int>& get_node_labels() const;
 
     const std::vector<int>& get_edge_labels() const;
 
     const std::vector<int>& get_edges(int src_node, int dst_node) const;
+
+    bool is_directed() const;
 };
 
 }
 
 #endif
```

### Comparing `pykwl-0.0.5/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.6/include/wl/details/weisfeiler_leman.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {
 private:
     using ColorMultiset = std::tuple<int, std::vector<int>, std::vector<int>, std::vector<int>, std::vector<int>>;
 
     std::map<ColorMultiset, int> m_color_function;
     int m_k;
 
-    int get_color(ColorMultiset&& key);
+    int get_color(ColorMultiset&& color_multiset);
 
     int get_subgraph_color(int src_node, int dst_node, const Graph& graph);
 
     std::tuple<int, std::vector<int>, std::vector<int>> k1_fwl(const Graph& graph);
 
     std::tuple<int, std::vector<int>, std::vector<int>> k2_fwl(const Graph& graph);
```

### Comparing `pykwl-0.0.5/pyproject.toml` & `pykwl-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/python/src/pykwl/bindings.cpp` & `pykwl-0.0.6/python/src/pykwl/bindings.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 void init_kwl(py::module_& m)
 {
     py::class_<Graph>(m, "Graph")  //
         .def(py::init<bool>())
         .def("add_node", &Graph::add_node, py::arg("label") = 0)
         .def("add_edge", &Graph::add_edge, py::arg("src_node"), py::arg("dst_node"), py::arg("label") = 0);
 
-    py::class_<WeisfeilerLeman>(m, "WeisfeilerLehman")  //
+    py::class_<WeisfeilerLeman>(m, "WeisfeilerLeman")  //
         .def(py::init<int>())
         .def("compute_coloring", &WeisfeilerLeman::compute_coloring);
 }
```

### Comparing `pykwl-0.0.5/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.6/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/setup.py` & `pykwl-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.5/src/CMakeLists.txt` & `pykwl-0.0.6/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.5/src/graph.cpp` & `pykwl-0.0.6/src/graph.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 Graph::Graph(bool directed) :
     m_outgoing_edges(),
     m_ingoing_edges(),
     m_outgoing_adjacent(),
     m_ingoing_adjacent(),
     m_outgoing_edges_between(),
     m_ingoing_edges_between(),
-    m_edge_sources(),
-    m_edge_destinations(),
     m_node_labels(),
     m_edge_labels(),
     m_directed(directed)
 {
 }
 
 int Graph::add_node(int label)
@@ -63,38 +61,30 @@
         int edge = get_num_edges();
         m_outgoing_edges.at(src_node).emplace_back(edge);
         m_ingoing_edges.at(dst_node).emplace_back(edge);
         m_outgoing_adjacent.at(src_node).emplace_back(dst_node);
         m_ingoing_adjacent.at(dst_node).emplace_back(src_node);
         m_outgoing_edges_between.at(src_node).at(dst_node).emplace_back(edge);
         m_ingoing_edges_between.at(dst_node).at(src_node).emplace_back(edge);
-        m_edge_sources.emplace_back(src_node);
-        m_edge_destinations.emplace_back(dst_node);
         m_edge_labels.emplace_back(label);
     }
 
     if (!m_directed)  // Add dst_node -> src_node
     {
         int edge = get_num_edges();
         m_outgoing_edges.at(dst_node).emplace_back(edge);
         m_ingoing_edges.at(src_node).emplace_back(edge);
         m_outgoing_adjacent.at(dst_node).emplace_back(src_node);
         m_ingoing_adjacent.at(src_node).emplace_back(dst_node);
         m_outgoing_edges_between.at(dst_node).at(src_node).emplace_back(edge);
         m_ingoing_edges_between.at(src_node).at(dst_node).emplace_back(edge);
-        m_edge_sources.emplace_back(dst_node);
-        m_edge_destinations.emplace_back(src_node);
         m_edge_labels.emplace_back(label);
     }
 }
 
-int Graph::get_source(int edge) const { return m_edge_sources.at(edge); }
-
-int Graph::get_destination(int edge) const { return m_edge_destinations.at(edge); }
-
 const std::vector<int>& Graph::get_outbound_edges(int node) const { return m_outgoing_edges.at(node); }
 
 const std::vector<int>& Graph::get_inbound_edges(int node) const { return m_ingoing_edges.at(node); }
 
 const std::vector<int>& Graph::get_outbound_adjacent(int node) const { return m_outgoing_adjacent.at(node); }
 
 const std::vector<int>& Graph::get_inbound_adjacent(int node) const { return m_ingoing_adjacent.at(node); }
@@ -108,8 +98,10 @@
 int Graph::get_edge_label(int edge) const { return m_edge_labels.at(edge); }
 
 const std::vector<int>& Graph::get_node_labels() const { return m_node_labels; }
 
 const std::vector<int>& Graph::get_edge_labels() const { return m_edge_labels; }
 
 const std::vector<int>& Graph::get_edges(int src_node, int dst_node) const { return m_outgoing_edges_between.at(src_node).at(dst_node); }
+
+bool Graph::is_directed() const { return m_directed; }
 }
```

### Comparing `pykwl-0.0.5/src/weisfeiler_leman.cpp` & `pykwl-0.0.6/src/weisfeiler_leman.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #include "wl/details/weisfeiler_leman.hpp"
 
 #include <algorithm>
 #include <cassert>
+#include <cstdlib>
 #include <stdexcept>
 #include <tuple>
 #include <unordered_map>
 #include <utility>
 #include <vector>
 
 namespace wl
 {
 
 inline static int pairing_function(int x, int y)
 {
     // Szudzik's pairing function
-    return x >= y ? x * x + x + y : y * y + x;
+    return std::abs(x >= y ? x * x + x + y : y * y + x);
 }
 
 inline static std::vector<int> get_colors_from_indices(const std::vector<int>& colors, const std::vector<int>& indices)
 {
     auto result = std::vector<int>(indices.size());
 
     for (const auto& i : indices)
@@ -90,25 +91,22 @@
 {
     if (k < 1 || k > 2)
     {
         throw std::invalid_argument("k must be either 1 or 2");
     }
 }
 
-int WeisfeilerLeman::get_color(ColorMultiset&& key)
+int WeisfeilerLeman::get_color(ColorMultiset&& color_multiset)
 {
-    // TODO: Try out Cantor's Pairing Function instead.
-    // https://en.wikipedia.org/wiki/Pairing_function
-
-    auto it = m_color_function.find(key);
+    auto it = m_color_function.find(color_multiset);
 
     if (it == m_color_function.end())
     {
         int color = static_cast<int>(m_color_function.size());
-        m_color_function.emplace(std::move(key), color);
+        m_color_function.emplace(std::move(color_multiset), color);
         return color;
     }
 
     return it->second;
 }
 
 std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k1_fwl(const Graph& graph)
@@ -130,30 +128,29 @@
 
     while (true)
     {
         ++num_iterations;
 
         for (int node = 0; node < num_nodes; ++node)
         {
-            auto ingoing_edge_colors = get_colors_from_indices(graph.get_edge_labels(), graph.get_inbound_edges(node));
             auto outgoing_edge_colors = get_colors_from_indices(graph.get_edge_labels(), graph.get_outbound_edges(node));
-
-            auto ingoing_node_colors = get_colors_from_indices(current_coloring, graph.get_inbound_adjacent(node));
             auto outgoing_node_colors = get_colors_from_indices(current_coloring, graph.get_outbound_adjacent(node));
+            auto ingoing_edge_colors = graph.is_directed() ? get_colors_from_indices(graph.get_edge_labels(), graph.get_inbound_edges(node)) : std::vector<int>();
+            auto ingoing_node_colors = graph.is_directed() ? get_colors_from_indices(current_coloring, graph.get_inbound_adjacent(node)) : std::vector<int>();
 
             // Sort the vectors using lexical sorting to ensure that the actual order of retrieval is irrelevant.
 
-            lexical_sort(ingoing_node_colors, ingoing_edge_colors);
             lexical_sort(outgoing_node_colors, outgoing_edge_colors);
+            lexical_sort(ingoing_node_colors, ingoing_edge_colors);
 
             next_coloring[node] = get_color({ current_coloring[node],
-                                              std::move(ingoing_edge_colors),
                                               std::move(outgoing_edge_colors),
-                                              std::move(ingoing_node_colors),
-                                              std::move(outgoing_node_colors) });
+                                              std::move(outgoing_node_colors),
+                                              std::move(ingoing_edge_colors),
+                                              std::move(ingoing_node_colors) });
         }
 
         if (test_fixpoint(current_coloring, next_coloring))
         {
             break;
         }
         else
@@ -174,31 +171,30 @@
     const auto& node_labels = graph.get_node_labels();
     const auto& edge_labels = graph.get_edge_labels();
 
     auto src_label = node_labels[src_node];
     auto dst_label = node_labels[dst_node];
 
     auto forward_edge_labels = get_colors_from_indices(edge_labels, graph.get_edges(src_node, dst_node));
-    auto backward_edge_labels = get_colors_from_indices(edge_labels, graph.get_edges(dst_node, src_node));
     auto self_src_edge_labels = get_colors_from_indices(edge_labels, graph.get_edges(src_node, src_node));
-    auto self_dst_edge_labels = get_colors_from_indices(edge_labels, graph.get_edges(dst_node, dst_node));
+    auto backward_edge_labels = graph.is_directed() ? get_colors_from_indices(edge_labels, graph.get_edges(dst_node, src_node)) : std::vector<int>();
+    auto self_dst_edge_labels = graph.is_directed() ? get_colors_from_indices(edge_labels, graph.get_edges(dst_node, dst_node)) : std::vector<int>();
 
     std::sort(forward_edge_labels.begin(), forward_edge_labels.end());
-    std::sort(backward_edge_labels.begin(), backward_edge_labels.end());
     std::sort(self_src_edge_labels.begin(), self_src_edge_labels.end());
+    std::sort(backward_edge_labels.begin(), backward_edge_labels.end());
     std::sort(self_dst_edge_labels.begin(), self_dst_edge_labels.end());
 
     // Graph labels must be non-negative and colors will always be positive.
     // We make the graph labels negative so that they are not confused with colors.
 
-    const auto max_node_label = *std::max(node_labels.begin(), node_labels.end());
-    return get_color({ -index_of_pair(src_label, dst_label, max_node_label + 1) - 1,
+    return get_color({ -pairing_function(src_label, dst_label) - 1,
                        std::move(forward_edge_labels),
-                       std::move(backward_edge_labels),
                        std::move(self_src_edge_labels),
+                       std::move(backward_edge_labels),
                        std::move(self_dst_edge_labels) });
 }
 
 std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k2_fwl(const Graph& graph)
 {
     const auto num_nodes = graph.get_num_nodes();
     auto current_coloring = std::vector<int>(num_nodes * num_nodes);
```

