# Comparing `tmp/onboardapis-1.3.2.tar.gz` & `tmp/onboardapis-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardapis-1.3.2.tar", last modified: Tue Feb 27 19:47:04 2024, max compression
+gzip compressed data, was "onboardapis-2.0.0rc1.tar", last modified: Wed Apr 17 22:39:26 2024, max compression
```

## Comparing `onboardapis-1.3.2.tar` & `onboardapis-2.0.0rc1.tar`

### file list

```diff
@@ -1,27 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-27 19:46:49.000000 onboardapis-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-02-27 19:47:04.278535 onboardapis-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-27 19:46:49.000000 onboardapis-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis/trains/
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis/trains/austria/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/austria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/austria/oebb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis/trains/germany/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/germany/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/germany/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/trains/germany/flx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-02-27 19:46:49.000000 onboardapis-1.3.2/onboardapis/utils/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 19:47:04.278535 onboardapis-1.3.2/onboardapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-02-27 19:47:04.000000 onboardapis-1.3.2/onboardapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-27 19:47:04.000000 onboardapis-1.3.2/onboardapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 19:47:04.000000 onboardapis-1.3.2/onboardapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-27 19:47:04.000000 onboardapis-1.3.2/onboardapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 19:47:04.278535 onboardapis-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-27 19:46:49.000000 onboardapis-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.278626 onboardapis-2.0.0rc1/onboardapis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/other/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/ship/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/ship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/at/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/bth/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/bth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/flix/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/me/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/it/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/it/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/setup.cfg
```

### Comparing `onboardapis-1.3.2/LICENSE` & `onboardapis-2.0.0rc1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Felix Zenk
+Copyright (c) 2022 - 2024 Felix Zenk and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `onboardapis-1.3.2/onboardapis/utils/conversions.py` & `onboardapis-2.0.0rc1/onboardapis/units.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
 Convert between different units
 """
 
-from typing import Tuple
+from __future__ import annotations
 
+from geopy.units import kilometers, meters, miles, feet, nautical, km, m, mi, ft, nm
 
-def coordinates_to_distance(start: Tuple[float, float], end: Tuple[float, float]) -> float:
-    """
-    Convert the two tuples ``start`` and ``end`` of coordinates
-    into the ``distance`` in meters that lies between those two positions
-
-    Currently not implemented!
-
-    :param start: The start coordinates
-    :type start: Tuple[float, float]
-    :param end: The end coordinates
-    :type end: Tuple[float, float]
-    :return: The distance in meters between 'start' and 'end'
-    :rtype: float
-    """
-    raise NotImplementedError()
+__all__ = [
+    'kilometers',
+    'meters',
+    'miles',
+    'feet',
+    'nautical',
+    'km',
+    'm',
+    'mi',
+    'ft',
+    'nm',
+    'seconds',
+    'minutes',
+    'hours',
+    'coordinates_decimal_to_dms',
+    'coordinates_dms_to_decimal',
+    'kmh',
+    'ms',
+]
 
 
 def coordinates_decimal_to_dms(
-        coordinates: Tuple[float, float]
-) -> Tuple[Tuple[int, int, float], Tuple[int, int, float]]:
+        coordinates: tuple[float, float]
+) -> tuple[tuple[int, int, float], tuple[int, int, float]]:
     """
     Convert the tuple ``coordinates`` of coordinates to degrees, minutes, seconds
 
     :param coordinates: The decimal coordinates to convert to degrees, minutes, seconds
     :type coordinates: Tuple[float, float]
     :return: The coordinates in degrees, minutes, seconds
     :rtype: Tuple[Tuple[int, int, float], Tuple[int, int, float]]
@@ -36,20 +41,24 @@
     lat, lon = coordinates
     lat_deg = int(abs(lat))
     lat_min = int((abs(lat) - lat_deg) * 60)
     lat_sec = ((abs(lat) - lat_deg) * 60 - lat_min) * 60
     lon_deg = int(abs(lon))
     lon_min = int((abs(lon) - lon_deg) * 60)
     lon_sec = ((abs(lon) - lon_deg) * 60 - lon_min) * 60
-    return (-lat_deg if lat < 0 else lat_deg, lat_min, lat_sec), (-lon_deg if lon < 0 else lon_deg, lon_min, lon_sec)
+    return (-lat_deg if lat < 0 else lat_deg, lat_min, lat_sec), (
+        -lon_deg if lon < 0 else lon_deg,
+        lon_min,
+        lon_sec,
+    )
 
 
 def coordinates_dms_to_decimal(
-        coordinates: Tuple[Tuple[int, int, float], Tuple[int, int, float]]
-) -> Tuple[float, float]:
+        coordinates: tuple[tuple[int, int, float], tuple[int, int, float]]
+) -> tuple[float, float]:
     """
     Convert the tuple ``coordinates`` of degrees, minutes, seconds to decimal degrees
 
     :param coordinates: The degrees, minutes, seconds coordinates to convert to decimal degrees
     :type coordinates: Tuple[Tuple[int, int, float], Tuple[int, int, float]]
     :return: The coordinates in decimal degrees
     :rtype: Tuple[float, float]
@@ -59,77 +68,51 @@
     lon = lon_deg + lon_min / 60 + lon_sec / 3600
     return lat, lon
 
 
 # Convert between different units
 
 
-def ms_to_kmh(meters_per_second: float) -> float:
-    """
-    Convert meters/second into kilometers/hour
-
-    :param meters_per_second: The value in meters/second
-    :type meters_per_second: float
-    :return: The result in kilometers/hour
-    :rtype: float
-    """
-    return meters_per_second * 3.6
-
-
-def kmh_to_ms(kilometers_per_hour: float) -> float:
-    """
-    Convert kilometers/hour into meters/second
-
-    :param kilometers_per_hour: The value in kilometers/hour
-    :type kilometers_per_hour: float
-    :return: The result in meters/second
-    :rtype: float
-    """
-    return kilometers_per_hour / 3.6
-
-
-def ms_to_mph(meters_per_second) -> float:
-    """
-    Convert meters/second into miles/hour
-
-    :param meters_per_second: The value in meters/second
-    :type meters_per_second: float
-    :return: The result in miles/hour
-    :rtype: float
-    """
-    return meters_per_second / 0.44704
-
-
-def mph_to_ms(miles_per_hour):
-    """
-    Convert miles/hour into meters/second
-
-    :param miles_per_hour: The value in miles/hour
-    :type miles_per_hour: float
-    :return: The result in meters/second
-    :rtype: float
-    """
-    return miles_per_hour * 0.44704
-
-
-def ms_to_kn(meters_per_second):
-    """
-    Convert meters/second into knots (nautical miles/hour)
-
-    :param meters_per_second: The value in meters/second
-    :type meters_per_second: float
-    :return: The result in knots (nautical miles/hour)
-    :rtype: float
-    """
-    return meters_per_second * 3600 / 1852
-
-
-def kn_to_ms(knots):
-    """
-    Convert knots (nautical miles/hour) into meters/second
-
-    :param knots: The value in knots (nautical miles/hour)
-    :type knots: float
-    :return: The result in meters/second
-    :rtype: float
-    """
-    return knots * 1852 / 3600
+def seconds(hours: float = 0, minutes: float = 0) -> float:  # noqa: F402
+    """Convert to seconds"""
+    ret = 0
+    if hours:
+        ret += hours * 3600
+    if minutes:
+        ret += minutes * 60
+    return ret
+
+
+def minutes(hours: float = 0, seconds: float = 0) -> float:  # noqa: F402
+    """Convert to minutes"""
+    ret = 0
+    if hours:
+        ret += hours * 60
+    if seconds:
+        ret += seconds / 60
+    return ret
+
+
+def hours(minutes: float = 0, seconds: float = 0) -> float:  # noqa: F402
+    """Convert to hours"""
+    ret = 0
+    if minutes:
+        ret += minutes / 60
+    if seconds:
+        ret += seconds / 3600
+    return ret
+
+
+def kmh(ms: float = None) -> float:  # noqa: F402
+    """Convert to kilometers per hour"""
+    ret = 0
+    if ms:
+        ret += kilometers(meters=ms) / hours(seconds=1)
+    return ret
+
+
+def ms(kmh: float = None) -> float:  # noqa: F402
+    """Convert to meters per second"""
+    ret = 0
+    if kmh:
+        ret += meters(kilometers=kmh) / seconds(hours=1)
+    return ret
```

