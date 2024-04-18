# Comparing `tmp/ridepy-2.6.2.tar.gz` & `tmp/ridepy-2.6.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridepy-2.6.2.tar", last modified: Thu Apr 18 11:51:57 2024, max compression
+gzip compressed data, was "ridepy-2.6.2.post1.tar", last modified: Thu Apr 18 11:55:24 2024, max compression
```

## Comparing `ridepy-2.6.2.tar` & `ridepy-2.6.2.post1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.582462 ridepy-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 11:51:05.000000 ridepy-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 11:51:05.000000 ridepy-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-18 11:51:57.582462 ridepy-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-18 11:51:05.000000 ridepy-2.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-18 11:51:05.000000 ridepy-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:51:57.582462 ridepy-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-18 11:51:05.000000 ridepy-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.558462 ridepy-2.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.558462 ridepy-2.6.2/src/lru-cache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.558462 ridepy-2.6.2/src/lru-cache/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.562462 ridepy-2.6.2/src/lru-cache/include/lru/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/cache-tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/cache.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/entry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/error.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/insertion-result.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.566462 ridepy-2.6.2/src/lru-cache/include/lru/internal/
--rw-r--r--   0 runner    (1001) docker     (127)    57507 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/base-cache.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/base-iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/base-ordered-iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/base-unordered-iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/callback-manager.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/definitions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/hash.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/information.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/last-accessed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/optional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/statistics-mutator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/timed-information.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/internal/utility.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/iterator-tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/key-statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/lowercase.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/lru.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/timed-cache.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-18 11:51:06.000000 ridepy-2.6.2/src/lru-cache/include/lru/wrap.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.566462 ridepy-2.6.2/src/ridepy/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.570462 ridepy-2.6.2/src/ridepy/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/main.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.570462 ridepy-2.6.2/src/ridepy/cpp/ridepy/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/ridepy/datastructures.h
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/ridepy/dispatchers.h
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/ridepy/spaces.h
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/ridepy/transportspace.h
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/cpp/ridepy/vehiclestate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.570462 ridepy-2.6.2/src/ridepy/data_structures_cython/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures_cython/cdata_structures.h
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures_cython/cdata_structures.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures_cython/data_structures.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    35654 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/data_structures_cython/data_structures.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.570462 ridepy-2.6.2/src/ridepy/extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/extras/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35133 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/extras/simulation_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/extras/spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/fleet_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.574462 ridepy-2.6.2/src/ridepy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.574462 ridepy-2.6.2/src/ridepy/util/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/stops.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/analytics/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.574462 ridepy-2.6.2/src/ridepy/util/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers/dispatcher_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers/ridepooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers/taxicab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.574462 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers.h
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/dispatchers.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/dispatchers_cython/dispatchers.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/request_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.578462 ridepy-2.6.2/src/ridepy/util/spaces_cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/boost_graph_space.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/boost_graph_space.h
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.h
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/ctransport_space.h
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/spaces.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/spaces_cython/spaces.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/testing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.578462 ridepy-2.6.2/src/ridepy/util/testing_utils_cython/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/testing_utils_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/util/testing_utils_cython/dispatchers.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/vehicle_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.578462 ridepy-2.6.2/src/ridepy/vehicle_state_cython/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/vehicle_state_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/vehicle_state_cython/cvehicle_state.h
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/vehicle_state_cython/cvehicle_state.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-18 11:51:05.000000 ridepy-2.6.2/src/ridepy/vehicle_state_cython/vehicle_state.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:57.578462 ridepy-2.6.2/src/ridepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:51:56.000000 ridepy-2.6.2/src/ridepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 11:51:57.000000 ridepy-2.6.2/src/ridepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.614847 ridepy-2.6.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-18 11:55:24.614847 ridepy-2.6.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:55:24.614847 ridepy-2.6.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.594847 ridepy-2.6.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.594847 ridepy-2.6.2.post1/src/lru-cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.594847 ridepy-2.6.2.post1/src/lru-cache/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.598847 ridepy-2.6.2.post1/src/lru-cache/include/lru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/cache-tags.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/cache.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/entry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/error.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/insertion-result.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.602847 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)    57507 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-cache.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-ordered-iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-unordered-iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/callback-manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/definitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/hash.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/information.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/last-accessed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/statistics-mutator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/timed-information.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/utility.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/iterator-tags.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/key-statistics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/lowercase.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/lru.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/statistics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/timed-cache.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-18 11:54:45.000000 ridepy-2.6.2.post1/src/lru-cache/include/lru/wrap.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.602847 ridepy-2.6.2.post1/src/ridepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.602847 ridepy-2.6.2.post1/src/ridepy/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/main.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.606847 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/datastructures.h
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/dispatchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/spaces.h
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/transportspace.h
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/cpp/ridepy/vehiclestate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.606847 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/cdata_structures.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/cdata_structures.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/data_structures.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    35654 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/data_structures_cython/data_structures.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.606847 ridepy-2.6.2.post1/src/ridepy/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/extras/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35133 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/extras/simulation_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/extras/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/fleet_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.606847 ridepy-2.6.2.post1/src/ridepy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.606847 ridepy-2.6.2.post1/src/ridepy/util/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/stops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/analytics/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.610847 ridepy-2.6.2.post1/src/ridepy/util/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers/dispatcher_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers/ridepooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers/taxicab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.610847 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/dispatchers.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/dispatchers.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/request_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.610847 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/boost_graph_space.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/boost_graph_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/ctransport_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/spaces.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/spaces.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.610847 ridepy-2.6.2.post1/src/ridepy/util/testing_utils_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/testing_utils_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/util/testing_utils_cython/dispatchers.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/vehicle_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.614847 ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/cvehicle_state.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/cvehicle_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-18 11:54:44.000000 ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/vehicle_state.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:55:24.614847 ridepy-2.6.2.post1/src/ridepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:55:23.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 11:55:24.000000 ridepy-2.6.2.post1/src/ridepy.egg-info/top_level.txt
```

### Comparing `ridepy-2.6.2/LICENSE` & `ridepy-2.6.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/PKG-INFO` & `ridepy-2.6.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ridepy
-Version: 2.6.2
+Version: 2.6.2.post1
 Summary: Simulates a dispatching algorithm serving exogenous transportation requests with a fleet of vehicles. Does not simulate the universe, unlike MATSim. Batteries are included.
 Author-email: Felix Jung <felix.jung@tu-dresden.de>, Debsankha Manik <dmanik@debsankha.net>
 Project-URL: Homepage, https://ridepy.org/
 Project-URL: Documentation, https://ridepy.org/
 Project-URL: Repository, https://github.com/PhysicsOfMobility/ridepy/
 Keywords: simulation,ridepooling,mobility,transport,physics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ridepy-2.6.2/README.rst` & `ridepy-2.6.2.post1/README.rst`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/pyproject.toml` & `ridepy-2.6.2.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Cython==3.0a6",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ridepy"
-version = "2.6.2"
+version = "2.6.2.post1"
 authors = [
     { name = "Felix Jung", email = "felix.jung@tu-dresden.de" },
     { name = "Debsankha Manik", email = "dmanik@debsankha.net" },
 ]
 description = "Simulates a dispatching algorithm serving exogenous transportation requests with a fleet of vehicles. Does not simulate the universe, unlike MATSim. Batteries are included."
 keywords = [
     "simulation",
```

### Comparing `ridepy-2.6.2/setup.py` & `ridepy-2.6.2.post1/setup.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/cache-tags.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/cache-tags.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/cache.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/cache.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/entry.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/entry.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/error.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/error.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/insertion-result.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/insertion-result.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/base-cache.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-cache.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/base-iterator.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-iterator.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/base-ordered-iterator.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-ordered-iterator.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/base-unordered-iterator.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/base-unordered-iterator.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/callback-manager.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/callback-manager.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/definitions.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/definitions.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/hash.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/hash.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/information.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/information.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/last-accessed.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/last-accessed.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/optional.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/optional.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/statistics-mutator.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/statistics-mutator.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/timed-information.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/timed-information.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/internal/utility.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/internal/utility.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/iterator-tags.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/iterator-tags.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/key-statistics.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/key-statistics.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/lowercase.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/lowercase.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/lru.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/lru.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/statistics.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/statistics.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/timed-cache.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/timed-cache.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/lru-cache/include/lru/wrap.hpp` & `ridepy-2.6.2.post1/src/lru-cache/include/lru/wrap.hpp`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/cli.py` & `ridepy-2.6.2.post1/src/ridepy/cli.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/data_structures.py` & `ridepy-2.6.2.post1/src/ridepy/data_structures.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/data_structures_cython/cdata_structures.h` & `ridepy-2.6.2.post1/src/ridepy/data_structures_cython/cdata_structures.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/data_structures_cython/cdata_structures.pxd` & `ridepy-2.6.2.post1/src/ridepy/data_structures_cython/cdata_structures.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/data_structures_cython/data_structures.pxd` & `ridepy-2.6.2.post1/src/ridepy/data_structures_cython/data_structures.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/data_structures_cython/data_structures.pyx` & `ridepy-2.6.2.post1/src/ridepy/data_structures_cython/data_structures.pyx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/events.py` & `ridepy-2.6.2.post1/src/ridepy/events.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/extras/io.py` & `ridepy-2.6.2.post1/src/ridepy/extras/io.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/extras/io_utils.py` & `ridepy-2.6.2.post1/src/ridepy/extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/extras/simulation_set.py` & `ridepy-2.6.2.post1/src/ridepy/extras/simulation_set.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/extras/spaces.py` & `ridepy-2.6.2.post1/src/ridepy/extras/spaces.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/fleet_state.py` & `ridepy-2.6.2.post1/src/ridepy/fleet_state.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/__init__.py` & `ridepy-2.6.2.post1/src/ridepy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/events.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/events.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/plotting.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/plotting.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/requests.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/requests.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/stops.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/stops.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/system.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/system.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/analytics/vehicle.py` & `ridepy-2.6.2.post1/src/ridepy/util/analytics/vehicle.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers/__init__.py` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers/dispatcher_class.py` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers/dispatcher_class.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers/ridepooling.py` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers/ridepooling.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers/taxicab.py` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers/taxicab.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers.h` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers.pxd` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers_cython/cdispatchers_utils.h` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/cdispatchers_utils.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/dispatchers_cython/dispatchers.pyx` & `ridepy-2.6.2.post1/src/ridepy/util/dispatchers_cython/dispatchers.pyx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/request_generators.py` & `ridepy-2.6.2.post1/src/ridepy/util/request_generators.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces.py` & `ridepy-2.6.2.post1/src/ridepy/util/spaces.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/boost_graph_space.cxx` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/boost_graph_space.cxx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/boost_graph_space.h` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/boost_graph_space.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.cxx` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.cxx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.h` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/cspaces.pxd` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/cspaces.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/ctransport_space.h` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/ctransport_space.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/spaces.pxd` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/spaces.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/spaces_cython/spaces.pyx` & `ridepy-2.6.2.post1/src/ridepy/util/spaces_cython/spaces.pyx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/testing_utils.py` & `ridepy-2.6.2.post1/src/ridepy/util/testing_utils.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/util/testing_utils_cython/dispatchers.pyx` & `ridepy-2.6.2.post1/src/ridepy/util/testing_utils_cython/dispatchers.pyx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/vehicle_state.py` & `ridepy-2.6.2.post1/src/ridepy/vehicle_state.py`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/vehicle_state_cython/cvehicle_state.h` & `ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/cvehicle_state.h`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/vehicle_state_cython/cvehicle_state.pxd` & `ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/cvehicle_state.pxd`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy/vehicle_state_cython/vehicle_state.pyx` & `ridepy-2.6.2.post1/src/ridepy/vehicle_state_cython/vehicle_state.pyx`

 * *Files identical despite different names*

### Comparing `ridepy-2.6.2/src/ridepy.egg-info/PKG-INFO` & `ridepy-2.6.2.post1/src/ridepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ridepy
-Version: 2.6.2
+Version: 2.6.2.post1
 Summary: Simulates a dispatching algorithm serving exogenous transportation requests with a fleet of vehicles. Does not simulate the universe, unlike MATSim. Batteries are included.
 Author-email: Felix Jung <felix.jung@tu-dresden.de>, Debsankha Manik <dmanik@debsankha.net>
 Project-URL: Homepage, https://ridepy.org/
 Project-URL: Documentation, https://ridepy.org/
 Project-URL: Repository, https://github.com/PhysicsOfMobility/ridepy/
 Keywords: simulation,ridepooling,mobility,transport,physics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ridepy-2.6.2/src/ridepy.egg-info/SOURCES.txt` & `ridepy-2.6.2.post1/src/ridepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

