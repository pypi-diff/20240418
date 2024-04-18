# Comparing `tmp/sosviz-0.2.4.tar.gz` & `tmp/sosviz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosviz-0.2.4.tar", last modified: Thu Apr 18 12:18:35 2024, max compression
+gzip compressed data, was "sosviz-0.2.5.tar", last modified: Thu Apr 18 12:33:59 2024, max compression
```

## Comparing `sosviz-0.2.4.tar` & `sosviz-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:35.174321 sosviz-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 12:18:29.000000 sosviz-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:18:35.170321 sosviz-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 12:18:29.000000 sosviz-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 12:18:29.000000 sosviz-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:18:35.174321 sosviz-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:35.166321 sosviz-0.2.4/sosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/bits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:35.170321 sosviz-0.2.4/sosviz/collect/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/irq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/collect/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:35.170321 sosviz-0.2.4/sosviz/output/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/output/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/output/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 12:18:29.000000 sosviz-0.2.4/sosviz/output/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:35.170321 sosviz-0.2.4/sosviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:18:35.000000 sosviz-0.2.4/sosviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.447200 sosviz-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 12:33:50.000000 sosviz-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:33:59.447200 sosviz-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 12:33:50.000000 sosviz-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 12:33:50.000000 sosviz-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:33:59.447200 sosviz-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.439200 sosviz-0.2.5/sosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/bits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz/collect/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/irq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24165 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/top_level.txt
```

### Comparing `sosviz-0.2.4/LICENSE` & `sosviz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/PKG-INFO` & `sosviz-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.4/README.md` & `sosviz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/pyproject.toml` & `sosviz-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosviz"
-version = "0.2.4"
+version = "0.2.5"
 description = "Information extractor from sos reports"
 license = {file = "LICENSE"}
 dependencies = [
 	"graphviz",
 ]
 requires-python = ">= 3.8"
 readme = "README.md"
```

### Comparing `sosviz-0.2.4/sosviz/__main__.py` & `sosviz-0.2.5/sosviz/__main__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/bits.py` & `sosviz-0.2.5/sosviz/bits.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/__init__.py` & `sosviz-0.2.5/sosviz/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/ip.py` & `sosviz-0.2.5/sosviz/collect/ip.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/irq.py` & `sosviz-0.2.5/sosviz/collect/irq.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/libvirt.py` & `sosviz-0.2.5/sosviz/collect/libvirt.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/ovs.py` & `sosviz-0.2.5/sosviz/collect/ovs.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/pci.py` & `sosviz-0.2.5/sosviz/collect/pci.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/platform.py` & `sosviz-0.2.5/sosviz/collect/platform.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/software.py` & `sosviz-0.2.5/sosviz/collect/software.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/topo.py` & `sosviz-0.2.5/sosviz/collect/topo.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/collect/tuning.py` & `sosviz-0.2.5/sosviz/collect/tuning.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.4/sosviz/output/dot.py` & `sosviz-0.2.5/sosviz/output/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,16 @@
             host_cpus.update(vm.vcpu_pinning.get(vcpu, set()))
         if host_cpus:
             labels.append(f"host CPUs {bit_list(host_cpus)}")
         cpu_numas = set()
         for n in self.report.numa.values():
             if host_cpus & n.cpus:
                 cpu_numas.add(n.id)
-        labels.append(f'<font color="blue">host NUMA {bit_list(cpu_numas)}</font>')
+        if cpu_numas:
+            labels.append(f'<font color="blue">host NUMA {bit_list(cpu_numas)}</font>')
         self.node(self.vm_cpu_node_id(vm, numa), labels, color="blue")
 
         labels = [f"<b>memory {human_readable(numa.memory, 1024)}</b>"]
         for h in numa.get("host_numa", []):
             labels.append(f'<font color="red">host NUMA {h}</font>')
         self.node(self.vm_memory_node_id(vm, numa), labels, color="red")
```

### Comparing `sosviz-0.2.4/sosviz.egg-info/PKG-INFO` & `sosviz-0.2.5/sosviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.4/sosviz.egg-info/SOURCES.txt` & `sosviz-0.2.5/sosviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

