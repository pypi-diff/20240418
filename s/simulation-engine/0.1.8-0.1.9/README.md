# Comparing `tmp/simulation_engine-0.1.8.tar.gz` & `tmp/simulation_engine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation_engine-0.1.8.tar", last modified: Sun Nov 26 17:59:27 2023, max compression
+gzip compressed data, was "simulation_engine-0.1.9.tar", last modified: Thu Dec  7 22:20:22 2023, max compression
```

## Comparing `simulation_engine-0.1.8.tar` & `simulation_engine-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-11-26 17:59:27.617658 simulation_engine-0.1.8/
--rw-rw-rw-   0        0        0      409 2023-11-26 17:59:27.617159 simulation_engine-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-11-26 17:59:27.617658 simulation_engine-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-11-26 17:59:21.000000 simulation_engine-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-26 17:59:27.613133 simulation_engine-0.1.8/simulation_engine/
--rw-rw-rw-   0        0        0     4938 2023-11-26 17:59:03.000000 simulation_engine-0.1.8/simulation_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-26 17:59:27.616659 simulation_engine-0.1.8/simulation_engine.egg-info/
--rw-rw-rw-   0        0        0      409 2023-11-26 17:59:27.000000 simulation_engine-0.1.8/simulation_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-11-26 17:59:27.000000 simulation_engine-0.1.8/simulation_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-26 17:59:27.000000 simulation_engine-0.1.8/simulation_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-26 17:59:27.000000 simulation_engine-0.1.8/simulation_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-11-26 17:59:27.000000 simulation_engine-0.1.8/simulation_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.774011 simulation_engine-0.1.9/
+-rw-rw-rw-   0        0        0      409 2023-12-07 22:20:22.774011 simulation_engine-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-12-07 22:20:22.774510 simulation_engine-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-12-07 22:20:17.000000 simulation_engine-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.770507 simulation_engine-0.1.9/simulation_engine/
+-rw-rw-rw-   0        0        0     4947 2023-12-07 22:19:18.000000 simulation_engine-0.1.9/simulation_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.773010 simulation_engine-0.1.9/simulation_engine.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/top_level.txt
```

### Comparing `simulation_engine-0.1.8/setup.py` & `simulation_engine-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.8' 
+VERSION = '0.1.9' 
 DESCRIPTION = 'Engine for simulating relic drops in Warframe.'
 LONG_DESCRIPTION = 'Engine for simulating relic drops in Warframe, has several features and is very extensible.'
 
 setup(
         name="simulation_engine", 
         version=VERSION,
         author="Jacob McBride",
```

### Comparing `simulation_engine-0.1.8/simulation_engine/__init__.py` & `simulation_engine-0.1.9/simulation_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     '3b3': (4 / 3),
     '4b4': 1,
     '8b8': 1,
 }
 
 
 def get_set_price(prime_part):
-    set_name = relic_engine.get_set_name(prime_part)
+    set_name = relic_engine.get_set_name(prime_part) + " Set"
 
     return relic_engine.get_price(set_name)
 
 
 def get_drop_priority(relics, min_price=30):
     plat_list = []
     ducat_list = []
```

