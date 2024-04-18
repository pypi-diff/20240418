# Comparing `tmp/sosviz-0.2.2.tar.gz` & `tmp/sosviz-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosviz-0.2.2.tar", last modified: Fri Apr 12 15:30:16 2024, max compression
+gzip compressed data, was "sosviz-0.2.3.tar", last modified: Thu Apr 18 11:38:39 2024, max compression
```

## Comparing `sosviz-0.2.2.tar` & `sosviz-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 15:30:08.000000 sosviz-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 15:30:16.864430 sosviz-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 15:30:08.000000 sosviz-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-12 15:30:08.000000 sosviz-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:30:16.864430 sosviz-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.860430 sosviz-0.2.2/sosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/bits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz/collect/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/irq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz/output/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:38:39.993376 sosviz-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 11:38:30.000000 sosviz-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 11:38:39.993376 sosviz-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 11:38:30.000000 sosviz-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 11:38:30.000000 sosviz-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:38:39.993376 sosviz-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:38:39.989376 sosviz-0.2.3/sosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/bits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:38:39.993376 sosviz-0.2.3/sosviz/collect/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/irq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/collect/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:38:39.993376 sosviz-0.2.3/sosviz/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/output/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/output/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 11:38:30.000000 sosviz-0.2.3/sosviz/output/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:38:39.993376 sosviz-0.2.3/sosviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:38:39.000000 sosviz-0.2.3/sosviz.egg-info/top_level.txt
```

### Comparing `sosviz-0.2.2/LICENSE` & `sosviz-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/PKG-INFO` & `sosviz-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -30,14 +30,17 @@
 
 ## Installation
 
 ```
 pip install --user sosviz
 ```
 
+System dependency to [`dot`](https://command-not-found.com/dot) from the
+[`graphviz`](https://graphviz.org/) package.
+
 ## Usage
 
 ```
 usage: sosviz [-h] [-V] [-d] [-f {dot,text,json,svg}] PATH
 
 Collect information from an sos report folder and export it in other formats
 on standard output.
@@ -49,15 +52,15 @@
   -h, --help            show this help message and exit
   -V, --version         Show version and exit.
   -d, --debug           Show debug info.
   -f {dot,text,json,svg}, --format {dot,text,json,svg}
                         Output format (default: svg).
 ```
 
-## Examples
+Examples:
 
 ```
 sosviz ~/tmp/sosreport > example.svg
 ```
 
 ```
 sosviz -f dot ~/tmp/sosreport | dot -Tpng > example.png
```

### Comparing `sosviz-0.2.2/README.md` & `sosviz-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 ## Installation
 
 ```
 pip install --user sosviz
 ```
 
+System dependency to [`dot`](https://command-not-found.com/dot) from the
+[`graphviz`](https://graphviz.org/) package.
+
 ## Usage
 
 ```
 usage: sosviz [-h] [-V] [-d] [-f {dot,text,json,svg}] PATH
 
 Collect information from an sos report folder and export it in other formats
 on standard output.
@@ -24,15 +27,15 @@
   -h, --help            show this help message and exit
   -V, --version         Show version and exit.
   -d, --debug           Show debug info.
   -f {dot,text,json,svg}, --format {dot,text,json,svg}
                         Output format (default: svg).
 ```
 
-## Examples
+Examples:
 
 ```
 sosviz ~/tmp/sosreport > example.svg
 ```
 
 ```
 sosviz -f dot ~/tmp/sosreport | dot -Tpng > example.png
```

### Comparing `sosviz-0.2.2/pyproject.toml` & `sosviz-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosviz"
-version = "0.2.2"
+version = "0.2.3"
 description = "Information extractor from sos reports"
 license = {file = "LICENSE"}
 dependencies = [
 	"graphviz",
 ]
 requires-python = ">= 3.8"
 readme = "README.md"
```

### Comparing `sosviz-0.2.2/sosviz/__main__.py` & `sosviz-0.2.3/sosviz/__main__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/bits.py` & `sosviz-0.2.3/sosviz/bits.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/__init__.py` & `sosviz-0.2.3/sosviz/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/ip.py` & `sosviz-0.2.3/sosviz/collect/ip.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,16 +53,24 @@
 
 
 def parse_report(path: pathlib.Path, data: D):
     data.interfaces = parse_interfaces(
         path / "sos_commands/networking/ip_-d_address", path
     )
     data.netns = D()
-    for netns in path.glob("sos_commands/networking/namespaces/*/*_ip_-d_address_show"):
-        data.netns[netns.parent.name] = parse_interfaces(netns, path)
+    for ip_addr in path.glob(
+        "sos_commands/networking/namespaces/*/*_ip_-d_address_show"
+    ):
+        netns = re.sub(r"ip_netns_exec_(.*)_ip_-d_address_show", r"\1", ip_addr.name)
+        data.netns[ip_addr.parent.name] = parse_interfaces(ip_addr, path)
+    for ip_addr in path.glob(
+        "sos_commands/networking/ip_netns_exec_*_ip*_address_show"
+    ):
+        netns = re.sub(r"ip_netns_exec_(.*)_ip.*_address_show", r"\1", ip_addr.name)
+        data.netns[netns] = parse_interfaces(ip_addr, path)
 
 
 def parse_interfaces(ip_addr: pathlib.Path, path: pathlib.Path) -> D:
     ifaces = D()
     if not ip_addr.is_file():
         return ifaces
     for block in IFACE_BLOCK_RE.finditer(ip_addr.read_text()):
```

### Comparing `sosviz-0.2.2/sosviz/collect/irq.py` & `sosviz-0.2.3/sosviz/collect/irq.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/libvirt.py` & `sosviz-0.2.3/sosviz/collect/libvirt.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,24 @@
         numa_id = int(numa.get("id", "0"))
         vm.setdefault("numa", D())[numa_id] = D(
             id=numa_id,
             memory=int(numa.get("memory", "0")) * multiplier(numa.get("unit")),
             mem_access=numa.get("memAccess"),
             vcpus=parse_cpu_set(numa.get("cpus", str(numa_id))),
         )
+    if "numa" not in vm:
+        memory = xml.find("./memory")
+        vcpu = xml.find("./vcpu")
+        vm.numa = D()
+        vm.numa[0] = D(
+            id=0,
+            memory=int(memory.text) * multiplier(memory.get("unit")),
+            vcpus=set(range(int(vcpu.text))),
+            host_numa=set(),
+        )
 
     for vcpupin in xml.findall("./cputune/vcpupin"):
         vcpu = int(vcpupin.get("vcpu"))
         cpuset = parse_cpu_set(vcpupin.get("cpuset"))
         vm.setdefault("vcpu_pinning", D())[vcpu] = cpuset
```

### Comparing `sosviz-0.2.2/sosviz/collect/ovs.py` & `sosviz-0.2.3/sosviz/collect/ovs.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/pci.py` & `sosviz-0.2.3/sosviz/collect/pci.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/platform.py` & `sosviz-0.2.3/sosviz/collect/platform.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/software.py` & `sosviz-0.2.3/sosviz/collect/software.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/topo.py` & `sosviz-0.2.3/sosviz/collect/topo.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/collect/tuning.py` & `sosviz-0.2.3/sosviz/collect/tuning.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz/output/dot.py` & `sosviz-0.2.3/sosviz/output/dot.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.2/sosviz.egg-info/PKG-INFO` & `sosviz-0.2.3/sosviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -30,14 +30,17 @@
 
 ## Installation
 
 ```
 pip install --user sosviz
 ```
 
+System dependency to [`dot`](https://command-not-found.com/dot) from the
+[`graphviz`](https://graphviz.org/) package.
+
 ## Usage
 
 ```
 usage: sosviz [-h] [-V] [-d] [-f {dot,text,json,svg}] PATH
 
 Collect information from an sos report folder and export it in other formats
 on standard output.
@@ -49,15 +52,15 @@
   -h, --help            show this help message and exit
   -V, --version         Show version and exit.
   -d, --debug           Show debug info.
   -f {dot,text,json,svg}, --format {dot,text,json,svg}
                         Output format (default: svg).
 ```
 
-## Examples
+Examples:
 
 ```
 sosviz ~/tmp/sosreport > example.svg
 ```
 
 ```
 sosviz -f dot ~/tmp/sosreport | dot -Tpng > example.png
```

### Comparing `sosviz-0.2.2/sosviz.egg-info/SOURCES.txt` & `sosviz-0.2.3/sosviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

