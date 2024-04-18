# Comparing `tmp/sosviz-0.2.6.tar.gz` & `tmp/sosviz-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosviz-0.2.6.tar", last modified: Thu Apr 18 15:57:39 2024, max compression
+gzip compressed data, was "sosviz-0.2.7.tar", last modified: Thu Apr 18 20:32:29 2024, max compression
```

## Comparing `sosviz-0.2.6.tar` & `sosviz-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 15:57:29.000000 sosviz-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 15:57:39.992165 sosviz-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 15:57:29.000000 sosviz-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 15:57:29.000000 sosviz-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:57:39.992165 sosviz-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.988165 sosviz-0.2.6/sosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/bits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz/collect/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/irq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz/output/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26693 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:32:29.931512 sosviz-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 20:32:23.000000 sosviz-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 20:32:29.931512 sosviz-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 20:32:23.000000 sosviz-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 20:32:23.000000 sosviz-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:32:29.931512 sosviz-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:32:29.927512 sosviz-0.2.7/sosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/bits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:32:29.927512 sosviz-0.2.7/sosviz/collect/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/irq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/collect/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:32:29.931512 sosviz-0.2.7/sosviz/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26704 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/output/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/output/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 20:32:23.000000 sosviz-0.2.7/sosviz/output/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:32:29.931512 sosviz-0.2.7/sosviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 20:32:29.000000 sosviz-0.2.7/sosviz.egg-info/top_level.txt
```

### Comparing `sosviz-0.2.6/LICENSE` & `sosviz-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/PKG-INFO` & `sosviz-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.6
+Version: 0.2.7
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.6/README.md` & `sosviz-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/pyproject.toml` & `sosviz-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosviz"
-version = "0.2.6"
+version = "0.2.7"
 description = "Information extractor from sos reports"
 license = {file = "LICENSE"}
 dependencies = [
 	"graphviz",
 ]
 requires-python = ">= 3.8"
 readme = "README.md"
```

### Comparing `sosviz-0.2.6/sosviz/__main__.py` & `sosviz-0.2.7/sosviz/__main__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/bits.py` & `sosviz-0.2.7/sosviz/bits.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/__init__.py` & `sosviz-0.2.7/sosviz/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/ip.py` & `sosviz-0.2.7/sosviz/collect/ip.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/irq.py` & `sosviz-0.2.7/sosviz/collect/irq.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/libvirt.py` & `sosviz-0.2.7/sosviz/collect/libvirt.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/ovs.py` & `sosviz-0.2.7/sosviz/collect/ovs.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/pci.py` & `sosviz-0.2.7/sosviz/collect/pci.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/platform.py` & `sosviz-0.2.7/sosviz/collect/platform.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/software.py` & `sosviz-0.2.7/sosviz/collect/software.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/topo.py` & `sosviz-0.2.7/sosviz/collect/topo.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/collect/tuning.py` & `sosviz-0.2.7/sosviz/collect/tuning.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.6/sosviz/output/dot.py` & `sosviz-0.2.7/sosviz/output/dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             state.append('<font color="red">NO-CARRIER</font>')
         elif "LOWER_UP" in iface["flags"]:
             state.append('<font color="forestgreen">LOWER_UP</font>')
         labels.append(f"state {','.join(state)}")
 
         for name, value in iface.get("stats", {}).items():
             tooltips.append(f"{name} {human_readable(value)}")
-            if "RUNNING" in iface["flags"] and name in self.NETDEV_ERRORS:
+            if value and "LOWER_UP" in iface["flags"] and name in self.NETDEV_ERRORS:
                 labels.append(
                     f'<font color="red">{name} {human_readable(value)}</font>'
                 )
 
         color = "salmon" if netns else "hotpink"
         self.node(
             self.iface_node_id(iface.name, netns),
```

### Comparing `sosviz-0.2.6/sosviz.egg-info/PKG-INFO` & `sosviz-0.2.7/sosviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.6
+Version: 0.2.7
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.6/sosviz.egg-info/SOURCES.txt` & `sosviz-0.2.7/sosviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

