# Comparing `tmp/sosviz-0.2.5.tar.gz` & `tmp/sosviz-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosviz-0.2.5.tar", last modified: Thu Apr 18 12:33:59 2024, max compression
+gzip compressed data, was "sosviz-0.2.6.tar", last modified: Thu Apr 18 15:57:39 2024, max compression
```

## Comparing `sosviz-0.2.5.tar` & `sosviz-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.447200 sosviz-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 12:33:50.000000 sosviz-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:33:59.447200 sosviz-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 12:33:50.000000 sosviz-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 12:33:50.000000 sosviz-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:33:59.447200 sosviz-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.439200 sosviz-0.2.5/sosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/bits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz/collect/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/irq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/collect/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz/output/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24165 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 12:33:50.000000 sosviz-0.2.5/sosviz/output/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:33:59.443200 sosviz-0.2.5/sosviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:33:59.000000 sosviz-0.2.5/sosviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 15:57:29.000000 sosviz-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 15:57:39.992165 sosviz-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 15:57:29.000000 sosviz-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 15:57:29.000000 sosviz-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:57:39.992165 sosviz-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.988165 sosviz-0.2.6/sosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/bits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz/collect/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/irq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/collect/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26693 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 15:57:29.000000 sosviz-0.2.6/sosviz/output/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:57:39.992165 sosviz-0.2.6/sosviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:57:39.000000 sosviz-0.2.6/sosviz.egg-info/top_level.txt
```

### Comparing `sosviz-0.2.5/LICENSE` & `sosviz-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/PKG-INFO` & `sosviz-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.5
+Version: 0.2.6
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.5/README.md` & `sosviz-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/pyproject.toml` & `sosviz-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosviz"
-version = "0.2.5"
+version = "0.2.6"
 description = "Information extractor from sos reports"
 license = {file = "LICENSE"}
 dependencies = [
 	"graphviz",
 ]
 requires-python = ">= 3.8"
 readme = "README.md"
```

### Comparing `sosviz-0.2.5/sosviz/__main__.py` & `sosviz-0.2.6/sosviz/__main__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/bits.py` & `sosviz-0.2.6/sosviz/bits.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/__init__.py` & `sosviz-0.2.6/sosviz/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/ip.py` & `sosviz-0.2.6/sosviz/collect/ip.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,38 +49,83 @@
 ADDR_RE = re.compile(
     r"inet6? (?P<addr>(?:\d+(?:\.\d+){3}|[a-f\d:]+)/\d+) .*scope global",
 )
 IFACE_BLOCK_RE = re.compile(r"^\d+:\s.*\n(\s{4}.+\n)+", re.VERBOSE | re.MULTILINE)
 
 
 def parse_report(path: pathlib.Path, data: D):
+    stats = get_netdev_stats(path)
     data.interfaces = parse_interfaces(
-        path / "sos_commands/networking/ip_-d_address", path
+        path / "sos_commands/networking/ip_-d_address", path, stats
     )
     data.netns = D()
     for ip_addr in path.glob(
         "sos_commands/networking/namespaces/*/*_ip_-d_address_show"
     ):
         netns = re.sub(r"ip_netns_exec_(.*)_ip_-d_address_show", r"\1", ip_addr.name)
-        data.netns[ip_addr.parent.name] = parse_interfaces(ip_addr, path)
+        data.netns[ip_addr.parent.name] = parse_interfaces(ip_addr, path, D())
     for ip_addr in path.glob(
         "sos_commands/networking/ip_netns_exec_*_ip*_address_show"
     ):
         netns = re.sub(r"ip_netns_exec_(.*)_ip.*_address_show", r"\1", ip_addr.name)
-        data.netns[netns] = parse_interfaces(ip_addr, path)
+        data.netns[netns] = parse_interfaces(ip_addr, path, D())
 
 
-def parse_interfaces(ip_addr: pathlib.Path, path: pathlib.Path) -> D:
+def parse_interfaces(ip_addr: pathlib.Path, path: pathlib.Path, stats: D) -> D:
     ifaces = D()
     if not ip_addr.is_file():
         return ifaces
     for block in IFACE_BLOCK_RE.finditer(ip_addr.read_text()):
         match = IFACE_RE.search(block.group())
         if not match:
             continue
         d = D({k: v for (k, v) in match.groupdict().items() if v is not None})
         for dev in path.glob(f"sys/class/net/{d.name}/device"):
             d.device = dev.resolve().name
         ifaces[d.name] = d
         for m in ADDR_RE.finditer(block.group()):
             d.setdefault("ip", []).append(m.group("addr"))
+        if d.name in stats:
+            d.stats = stats[d.name]
     return ifaces
+
+
+STATS_RE = re.compile(
+    r"""
+    ^
+    \s*
+    (?P<name>[^:]+):\s+
+    (?P<rx_bytes>\d+)\s+
+    (?P<rx_packets>\d+)\s+
+    (?P<rx_errors>\d+)\s+
+    (?P<rx_dropped>\d+)\s+
+    (?P<rx_fifo>\d+)\s+
+    (?P<rx_frame>\d+)\s+
+    (?P<rx_compressed>\d+)\s+
+    (?P<rx_multicast>\d+)\s+
+    (?P<tx_bytes>\d+)\s+
+    (?P<tx_packets>\d+)\s+
+    (?P<tx_errors>\d+)\s+
+    (?P<tx_dropped>\d+)\s+
+    (?P<tx_fifo>\d+)\s+
+    (?P<tx_colls>\d+)\s+
+    (?P<tx_carrier>\d+)\s+
+    (?P<tx_compressed>\d+)
+    \s*
+    $
+    """,
+    re.VERBOSE | re.MULTILINE,
+)
+
+
+def get_netdev_stats(path: pathlib.Path) -> D:
+    stats = D()
+    dev = path / "proc/net/dev"
+    if not dev.is_file():
+        return stats
+
+    for match in STATS_RE.finditer(dev.read_text()):
+        dic = match.groupdict()
+        name = dic.pop("name")
+        stats[name] = D({k: int(v) for k, v in dic.items()})
+
+    return stats
```

### Comparing `sosviz-0.2.5/sosviz/collect/irq.py` & `sosviz-0.2.6/sosviz/collect/irq.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/libvirt.py` & `sosviz-0.2.6/sosviz/collect/libvirt.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/ovs.py` & `sosviz-0.2.6/sosviz/collect/ovs.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,29 +71,46 @@
                     name = strip_quotes(m.group("name"))
                     ifaces[name] = D(name=name, type=m.group("type") or "")
                     if m.group("options"):
                         ifaces[name].options = cast_value(m.group("options"))
                 if not ifaces:
                     continue
                 port_name = strip_quotes(match.group("name"))
-                port = D(name=port_name, bridge=br_name)
+                port = D(name=port_name, bridge=br_name, stats=D())
                 if len(ifaces) == 1 and port_name in ifaces:
                     port.update(ifaces[port_name])
                 else:
                     port.type = "bond"
                     port.members = ifaces
                 if match.group("tag"):
                     port.tag = int(match.group("tag"))
 
                 ports[port_name] = port
                 bridges.setdefault(
                     br_name, D(name=br_name, ports=0, of_rules=0)
                 ).ports += 1
                 bridges[br_name].datapath = datapath
 
+    for f in path.glob("sos_commands/openvswitch/ovs-vsctl*_list_interface"):
+        for block in f.read_text().split("\n\n"):
+            d = {}
+            ovs_to_dict(block, d)
+            if d.get("name") in ovs.ports:
+                p = ovs.ports[d["name"]]
+            else:
+                for port in ovs.ports.values():
+                    if "members" in port and d["name"] in port.members:
+                        p = port.members[d["name"]]
+                        break
+                else:
+                    continue
+            p.admin_state = d.get("admin_state", "?")
+            p.link_state = d.get("link_state", "?")
+            p.stats = D(d.get("statistics", {}))
+
     for name, br in bridges.items():
         for f in path.glob(f"sos_commands/openvswitch/ovs-ofctl*_dump-flows_{name}"):
             br.of_rules = len(f.read_text().splitlines()) - 1
 
 
 def strip_quotes(s: str) -> str:
     return s.strip("\"' \t")
```

### Comparing `sosviz-0.2.5/sosviz/collect/pci.py` & `sosviz-0.2.6/sosviz/collect/pci.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/platform.py` & `sosviz-0.2.6/sosviz/collect/platform.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/software.py` & `sosviz-0.2.6/sosviz/collect/software.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/topo.py` & `sosviz-0.2.6/sosviz/collect/topo.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/collect/tuning.py` & `sosviz-0.2.6/sosviz/collect/tuning.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.5/sosviz/output/dot.py` & `sosviz-0.2.6/sosviz/output/dot.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,14 +216,26 @@
         self.node(self.vm_iface_node_id(name), labels, color=color)
         if peer:
             self.edge(self.vm_iface_node_id(name), peer, style="dashed", color=color)
 
     def iface_node_id(self, name, netns):
         return f"net_{netns}_{name}"
 
+    NETDEV_ERRORS = {
+        "rx_dropped",
+        "rx_errors",
+        "rx_fifo",
+        "rx_frame",
+        "tx_carrier",
+        "tx_colls",
+        "tx_dropped",
+        "tx_errors",
+        "tx_fifo",
+    }
+
     def phy_iface(self, iface: D, netns: str = ""):
         if netns == "" and iface.name in self.report.ovs.bridges:
             return
         if iface.name in "ovs-system" or re.match(r"(genev|vxlan)_sys_\d+", iface.name):
             return
 
         labels = [f"<b>{iface.name}</b>"]
@@ -251,14 +263,32 @@
 
         tooltips = [iface["flags"]]
         if "mac" in iface:
             tooltips.append(f"mac {iface.mac}")
         if "mtu" in iface:
             tooltips.append(f"mtu {iface.mtu}")
 
+        state = []
+        if "DOWN" in iface["flags"]:
+            state.append('<font color="darkorange">DOWN</font>')
+        else:
+            state.append('<font color="forestgreen">UP</font>')
+        if "NO-CARRIER" in iface["flags"]:
+            state.append('<font color="red">NO-CARRIER</font>')
+        elif "LOWER_UP" in iface["flags"]:
+            state.append('<font color="forestgreen">LOWER_UP</font>')
+        labels.append(f"state {','.join(state)}")
+
+        for name, value in iface.get("stats", {}).items():
+            tooltips.append(f"{name} {human_readable(value)}")
+            if "RUNNING" in iface["flags"] and name in self.NETDEV_ERRORS:
+                labels.append(
+                    f'<font color="red">{name} {human_readable(value)}</font>'
+                )
+
         color = "salmon" if netns else "hotpink"
         self.node(
             self.iface_node_id(iface.name, netns),
             labels,
             color=color,
             tooltip=tooltips,
         )
@@ -381,14 +411,33 @@
                 color="forestgreen",
                 style="solid",
             )
 
     def ovs_port_node_id(self, name):
         return f"ovs_port_{name}"
 
+    def ovs_port_state(self, state: str) -> str:
+        if state == "up":
+            return '<font color="forestgreen">up</font>'
+        return '<font color="red">DOWN</font>'
+
+    def ovs_base_labels(self, port: D):
+        labels = [
+            f"<b>{port.name}</b>",
+            f"OVS {port.type}",
+        ]
+        if "admin_state" in port and "link_state" in port:
+            state = ",".join(
+                self.ovs_port_state(s) for s in (port.admin_state, port.link_state)
+            )
+            labels.append(f"state {state}")
+        if "tag" in port:
+            labels.append(f'<font color="forestgreen">VLAN {port.tag}</font>')
+        return labels
+
     def ovs_dpdk_labels(self, port: D):
         if "dpdk_devargs" in port.options:
             numa_id = "N/A"
             for numa in self.report.numa.values():
                 if port.options.dpdk_devargs in numa.pci_nics:
                     numa_id = numa.id
                     break
@@ -406,39 +455,62 @@
 
         for rxq, core, numa in sorted(rxqs):
             yield f"rxq {rxq} cpu {core} NUMA {numa}"
         if disabled:
             s = "s" if len(disabled) > 1 else ""
             yield f'<font color="gray">rxq{s} {bit_list(disabled)} disabled</font>'
 
+    OVS_ERRORS = {
+        "collisions",
+        "ovs_rx_qos_drops",
+        "ovs_tx_failure_drops",
+        "ovs_tx_invalid_hwol_drops",
+        "ovs_tx_mtu_exceeded_drops",
+        "ovs_tx_qos_drops",
+        "rx_crc_err",
+        "rx_dropped",
+        "rx_errors",
+        "rx_frame_err",
+        "rx_missed_errors",
+        "rx_over_err",
+        "tx_dropped",
+        "tx_errors",
+    }
+
+    def ovs_stats_labels(self, port: D):
+        for name, value in port.get("stats", {}).items():
+            if value and port.get("admin_state") == "up" and name in self.OVS_ERRORS:
+                yield f'<font color="red">{name} {human_readable(value)}</font>'
+
+    def ovs_stats_tooltip(self, port: D):
+        tip = []
+        for name, value in port.get("stats", {}).items():
+            tip.append(f"{name} {human_readable(value)}")
+        return tip
+
     def ovs_port(self, port: D):
         if port.name in self.report.interfaces:
             self.edge(
                 self.iface_node_id(port.name, ""),
                 self.ovs_br_node_id(port.bridge),
                 color="forestgreen",
             )
             return
 
-        labels = [
-            f"<b>{port.name}</b>",
-            f"OVS {port.type}",
-        ]
+        labels = self.ovs_base_labels(port)
         if port.type in ("dpdk", "dpdkvhostuserclient"):
             labels.extend(self.ovs_dpdk_labels(port))
             if "dpdk_devargs" in port.options:
                 self.edge(
                     self.ovs_port_node_id(port.name),
                     pci_node_id(port.options.dpdk_devargs),
                     style="dashed",
                     color="darkorange",
                 )
 
-        if "tag" in port:
-            labels.append(f'<font color="forestgreen">VLAN {port.tag}</font>')
         iface = self.report.interfaces.get(port.name, None)
         if iface is not None:
             for ip in self.report.interfaces[port.name].get("ip", []):
                 labels.append(f'<font color="purple">{ip}</font>')
             if "link" in iface:
                 link_ns = ""
                 if "link_netns" in iface:
@@ -455,18 +527,20 @@
             if "master" in iface:
                 self.edge(
                     self.iface_node_id(iface.master, ""),
                     self.ovs_port_node_id(port.name),
                     style="solid",
                     color="forestgreen",
                 )
+        labels.extend(self.ovs_stats_labels(port))
 
         self.node(
             self.ovs_port_node_id(port.name),
             labels,
+            tooltip=self.ovs_stats_tooltip(port),
             color="forestgreen",
         )
         self.edge(
             self.ovs_br_node_id(port.bridge),
             self.ovs_port_node_id(port.name),
             color="forestgreen",
         )
@@ -478,29 +552,28 @@
                         self.ovs_port_node_id(port.name),
                         self.iface_node_id(member.name, ""),
                         style="solid",
                         color="forestgreen",
                     )
                     continue
 
-                labels = [
-                    f"<b>{member.name}</b>",
-                    f"OVS {member.type}",
-                ]
+                labels = self.ovs_base_labels(member)
                 if member.type == "dpdk":
                     labels.extend(self.ovs_dpdk_labels(member))
                     self.edge(
                         self.ovs_port_node_id(member.name),
                         pci_node_id(member.options.dpdk_devargs),
                         style="dashed",
                         color="darkorange",
                     )
+                labels.extend(self.ovs_stats_labels(member))
                 self.node(
                     self.ovs_port_node_id(member.name),
                     labels,
+                    tooltip=self.ovs_stats_tooltip(member),
                     color="forestgreen",
                 )
                 self.edge(
                     self.ovs_port_node_id(port.name),
                     self.ovs_port_node_id(member.name),
                     style="solid",
                     color="forestgreen",
```

### Comparing `sosviz-0.2.5/sosviz.egg-info/PKG-INFO` & `sosviz-0.2.6/sosviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosviz
-Version: 0.2.5
+Version: 0.2.6
 Summary: Information extractor from sos reports
 Author-email: Robin Jarry <rjarry@redhat.com>
 License: Copyright 2024 Robin Jarry
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `sosviz-0.2.5/sosviz.egg-info/SOURCES.txt` & `sosviz-0.2.6/sosviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

