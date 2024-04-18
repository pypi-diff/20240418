# Comparing `tmp/litesata-2023.4.tar.gz` & `tmp/litesata-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesata-2023.4.tar", last modified: Thu Apr 18 20:13:34 2024, max compression
+gzip compressed data, was "litesata-2023.8.tar", last modified: Thu Apr 18 20:13:55 2024, max compression
```

## Comparing `litesata-2023.4.tar` & `litesata-2023.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.108341 litesata-2023.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1745 2024-04-18 20:12:31.000000 litesata-2023.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:34.108081 litesata-2023.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4955 2024-04-18 20:12:31.000000 litesata-2023.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.098056 litesata-2023.4/litesata/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7647 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.100089 litesata-2023.4/litesata/core/
--rw-r--r--   0 timkpaine   (501) staff       (20)      746 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10326 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/command.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    24128 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/core/link.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8055 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/transport.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.102157 litesata-2023.4/litesata/frontend/
--rw-r--r--   0 timkpaine   (501) staff       (20)      225 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5057 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/arbitration.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7922 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/bist.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6877 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/frontend/dma.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2555 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/identify.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11946 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/raid.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8795 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/gen.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.104809 litesata-2023.4/litesata/phy/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5085 2024-04-18 20:13:25.000000 litesata-2023.4/litesata/phy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    38261 2024-04-18 20:13:25.000000 litesata-2023.4/litesata/phy/a7sataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6412 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/ctrl.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8289 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/datapath.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    35625 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/phy/k7sataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    45714 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/uspsataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    37974 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/ussataphy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.107805 litesata-2023.4/litesata.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      866 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:13:34.108388 litesata-2023.4/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)      864 2024-04-18 20:13:31.000000 litesata-2023.4/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.107576 litesata-2023.4/test/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2695 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_bist.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5802 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_command.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2660 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4092 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_cont.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2124 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_crc.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2031 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_scrambler.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4076 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_mirroring.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3344 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_striping.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.477918 litesata-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1745 2024-04-18 20:12:31.000000 litesata-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:55.477611 litesata-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4955 2024-04-18 20:12:31.000000 litesata-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.470121 litesata-2023.8/litesata/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7620 2024-04-18 20:13:48.000000 litesata-2023.8/litesata/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.471594 litesata-2023.8/litesata/core/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      746 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/core/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10326 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/core/command.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    24166 2024-04-18 20:13:48.000000 litesata-2023.8/litesata/core/link.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8055 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/core/transport.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.474680 litesata-2023.8/litesata/frontend/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      225 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/frontend/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5057 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/frontend/arbitration.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7922 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/frontend/bist.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8186 2024-04-18 20:13:48.000000 litesata-2023.8/litesata/frontend/dma.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2555 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/frontend/identify.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11946 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/frontend/raid.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8795 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/gen.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.475946 litesata-2023.8/litesata/phy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5085 2024-04-18 20:13:25.000000 litesata-2023.8/litesata/phy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    38261 2024-04-18 20:13:25.000000 litesata-2023.8/litesata/phy/a7sataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6411 2024-04-18 20:13:48.000000 litesata-2023.8/litesata/phy/ctrl.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8293 2024-04-18 20:13:48.000000 litesata-2023.8/litesata/phy/datapath.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    35625 2024-04-18 20:12:31.000000 litesata-2023.8/litesata/phy/k7sataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    45714 2024-04-18 20:12:45.000000 litesata-2023.8/litesata/phy/uspsataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    37974 2024-04-18 20:12:45.000000 litesata-2023.8/litesata/phy/ussataphy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.477290 litesata-2023.8/litesata.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:55.000000 litesata-2023.8/litesata.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      866 2024-04-18 20:13:55.000000 litesata-2023.8/litesata.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:13:55.000000 litesata-2023.8/litesata.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:13:55.000000 litesata-2023.8/litesata.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:13:55.000000 litesata-2023.8/litesata.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:13:55.477986 litesata-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)      864 2024-04-18 20:13:52.000000 litesata-2023.8/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:55.477078 litesata-2023.8/test/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2695 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_bist.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5802 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_command.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2660 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_link.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4092 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_link_cont.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2124 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_link_crc.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2031 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_link_scrambler.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4076 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_mirroring.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3344 2024-04-18 20:12:31.000000 litesata-2023.8/test/test_striping.py
```

### Comparing `litesata-2023.4/LICENSE` & `litesata-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/PKG-INFO` & `litesata-2023.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesata
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable SATA core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litesata
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litesata-2023.4/README.md` & `litesata-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/common.py` & `litesata-2023.8/litesata/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     "CONT":    0x9999aa7c,
     "SYNC":    0xb5b5957c,
     "R_RDY":   0x4a4a957c,
     "R_OK":    0x3535b57c,
     "R_ERR":   0x5656b57c,
     "R_IP":    0x5555b57c,
     "X_RDY":   0x5757b57c,
-    "CONT":    0x9999aa7c,
     "WTRM":    0x5858b57c,
     "SOF":     0x3737b57c,
     "EOF":     0xd5d5b57c,
     "HOLD":    0xd5d5aa7c,
     "HOLDA":   0x9595aa7c
 }
```

### Comparing `litesata-2023.4/litesata/core/__init__.py` & `litesata-2023.8/litesata/core/__init__.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/core/command.py` & `litesata-2023.8/litesata/core/command.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/core/link.py` & `litesata-2023.8/litesata/core/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
             If(data_valid,
                 NextState("COPY")
             )
         )
         fsm.act("COPY",
             pipeline.sink.valid.eq(data_valid),
             insert.eq(primitives["R_IP"]),
-            If(primitive_valid,
+            If(primitive_valid & (primitive != primitives["HOLDA"]),
                 If(primitive == primitives["HOLD"],
                     insert.eq(primitives["HOLDA"])
                 ).Elif(primitive == primitives["EOF"],
                     # 1 clock cycle latency
                     pipeline.sink.valid.eq(1),
                     pipeline.sink.last.eq(1),
                     NextState("WTRM")
@@ -765,17 +765,17 @@
         self.submodules.tx_align = LiteSATAALIGNInserter(phy_description(32))
         self.submodules.tx_pipeline = Pipeline(self.tx, self.tx_align, phy)
 
         # RX ---------------------------------------------------------------------------------------
         self.submodules.rx_align = LiteSATAALIGNRemover(phy_description(32))
         self.submodules.rx_cont = LiteSATACONTRemover(phy_description(32))
         self.submodules.rx = BufferizeEndpoints({"sink": DIR_SINK})(LiteSATALinkRX())
-        self.submodules.rx_buffer = stream.SyncFIFO(link_description(32), 128)
+        self.submodules.rx_buffer = stream.SyncFIFO(link_description(32), 256)
         self.submodules.rx_pipeline = Pipeline(phy, self.rx_align, self.rx_cont, self.rx, self.rx_buffer)
 
         # RX --> TX --------------------------------------------------------------------------------
         self.comb += self.rx.to_tx.connect(self.tx.from_rx)
 
         self.sink, self.source = self.tx_pipeline.sink, self.rx_pipeline.source
 
         # Hold -------------------------------------------------------------------------------------
-        self.comb += self.rx.hold.eq(self.rx_buffer.level > 64)
+        self.comb += self.rx.hold.eq(self.rx_buffer.level > 128)
```

### Comparing `litesata-2023.4/litesata/core/transport.py` & `litesata-2023.8/litesata/core/transport.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/frontend/arbitration.py` & `litesata-2023.8/litesata/frontend/arbitration.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/frontend/bist.py` & `litesata-2023.8/litesata/frontend/bist.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/frontend/dma.py` & `litesata-2023.8/litesata/frontend/dma.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 # This file is part of LiteSATA.
 #
 # Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2023 Gabriel L. Somlo <gsomlo@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import log2
 
 from migen import *
 
 from litex.gen import *
@@ -20,28 +21,31 @@
 
 class LiteSATASector2MemDMA(Module, AutoCSR):
     """Sector to Memory DMA
 
     Read a sector from the SATA core and write it to memory through DMA.
     """
     def __init__(self, port, bus, endianness="little"):
-        self.port   = port
-        self.bus    = bus
-        self.sector = CSRStorage(48)
-        self.base   = CSRStorage(64)
-        self.start  = CSR()
-        self.done   = CSRStatus()
-        self.error  = CSRStatus()
-        self.irq    = Signal()
+        self.port     = port
+        self.bus      = bus
+        self.sector   = CSRStorage(48)
+        self.nsectors = CSRStorage(16)
+        self.base     = CSRStorage(64)
+        self.start    = CSR()
+        self.done     = CSRStatus()
+        self.error    = CSRStatus()
+        self.irq      = Signal()
 
         # # #
 
         port_bytes = port.dw//8
         dma_bytes  = bus.data_width//8
         count      = Signal(max=logical_sector_size//dma_bytes)
+        crt_sec    = Signal(48)
+        crt_base   = Signal(64)
 
         # Sector buffer
         buf = stream.SyncFIFO([("data", port.dw)], logical_sector_size//port_bytes)
         self.submodules.buf = buf
 
         # Converter
         conv = stream.Converter(nbits_from=port.dw, nbits_to=bus.data_width)
@@ -58,79 +62,95 @@
         self.submodules.dma = dma
 
         # Control FSM
         self.submodules.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(self.start.re,
                 NextValue(count,             0),
+                NextValue(crt_sec,           self.sector.storage),
+                NextValue(crt_base,          self.base.storage),
                 NextValue(self.error.status, 0),
                 NextState("SEND-CMD")
             ).Else(
                 self.done.status.eq(1)
             ),
             conv.source.ready.eq(1)
         )
         fsm.act("SEND-CMD",
             # Send read command for 1 Sector.
             port.sink.valid.eq(1),
             port.sink.last.eq(1),
             port.sink.read.eq(1),
-            port.sink.sector.eq(self.sector.storage),
+            port.sink.sector.eq(crt_sec),
             port.sink.count.eq(1),
             If(port.sink.ready,
                 NextState("RECEIVE-DATA-DMA")
             )
         )
         fsm.act("RECEIVE-DATA-DMA",
             # Connect Converter to DMA.
             dma.sink.valid.eq(conv.source.valid),
             dma.sink.last.eq(conv.source.last),
-            dma.sink.address.eq(self.base.storage[int(log2(dma_bytes)):] + count),
+            dma.sink.address.eq(crt_base[int(log2(dma_bytes)):] + count),
             dma.sink.data.eq(reverse_bytes(conv.source.data)),
             conv.source.ready.eq(dma.sink.ready),
             If(dma.sink.valid & dma.sink.ready,
                 NextValue(count, count + 1),
                 If(dma.sink.last,
                     self.irq.eq(1),
-                    NextState("IDLE")
+                    NextState("SECTOR-LOOP")
                 )
             ),
 
             # Monitor errors
-            If(port.source.valid & port.source.ready,
-                If(port.source.failed,
-                    self.irq.eq(1),
-                    NextValue(self.error.status, 1),
-                    NextState("IDLE"),
-                )
+            If(port.source.valid & port.source.ready & port.source.failed,
+                self.irq.eq(1),
+                NextValue(self.error.status, 1),
+                NextState("IDLE"),
+            )
+        )
+        fsm.act("SECTOR-LOOP",
+            If(crt_sec == (self.sector.storage + self.nsectors.storage - 1),
+                self.irq.eq(1),
+                NextState("IDLE")
+            ).Else(
+                NextValue(count,    0),
+                NextValue(crt_sec,  crt_sec + 1),
+                NextValue(crt_base, crt_base + 512),
+                NextValue(self.error.status, 0),
+                conv.source.ready.eq(1),
+                NextState("SEND-CMD")
             )
         )
 
 # SATA Mem2Sector DMA ------------------------------------------------------------------------------
 
 class LiteSATAMem2SectorDMA(Module, AutoCSR):
     """Memory 2 Sector DMA
 
     Read memory through DMA and write it to a sector of the SATA core.
     """
     def __init__(self, bus, port, endianness="little"):
-        self.bus    = bus
-        self.port   = port
-        self.sector = CSRStorage(48)
-        self.base   = CSRStorage(64)
-        self.start  = CSR()
-        self.done   = CSRStatus()
-        self.error  = CSRStatus()
-        self.irq    = Signal()
+        self.bus      = bus
+        self.port     = port
+        self.sector   = CSRStorage(48)
+        self.nsectors = CSRStorage(16)
+        self.base     = CSRStorage(64)
+        self.start    = CSR()
+        self.done     = CSRStatus()
+        self.error    = CSRStatus()
+        self.irq      = Signal()
 
         # # #
 
         dma_bytes  = bus.data_width//8
         port_bytes = port.dw//8
         count      = Signal(max=logical_sector_size//min(dma_bytes, port_bytes))
+        crt_sec    = Signal(48)
+        crt_base   = Signal(64)
 
         # DMA
         dma = WishboneDMAReader(bus, with_csr=False, endianness=endianness)
         self.submodules.dma = dma
 
         # Sector buffer
         buf = stream.SyncFIFO([("data", port.dw)], logical_sector_size//dma_bytes)
@@ -147,62 +167,70 @@
         self.comb += buf.source.connect(conv.sink)
 
         # Control FSM
         self.submodules.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(self.start.re,
                 NextValue(count,             0),
+                NextValue(crt_sec,           self.sector.storage),
+                NextValue(crt_base,          self.base.storage),
                 NextValue(self.error.status, 0),
                 NextState("READ-DATA-DMA")
             ).Else(
                 self.done.status.eq(1)
             ),
             conv.source.ready.eq(1)
         )
         fsm.act("READ-DATA-DMA",
             # Read Sector data over DMA.
             dma.sink.valid.eq(1),
-            dma.sink.address.eq(self.base.storage[int(log2(dma_bytes)):] + count),
+            dma.sink.address.eq(crt_base[int(log2(dma_bytes)):] + count),
             If(dma.sink.valid & dma.sink.ready,
                 NextValue(count, count + 1),
                 If(count == (logical_sector_size//dma_bytes - 1),
                     NextValue(count, 0),
                     NextState("SEND-CMD-AND-DATA")
                 )
             )
         )
         fsm.act("SEND-CMD-AND-DATA",
             # Send write command/data for 1 Sector.
             port.sink.valid.eq(1),
             port.sink.last.eq(count == (logical_sector_size//port_bytes - 1)),
             port.sink.write.eq(1),
-            port.sink.sector.eq(self.sector.storage),
+            port.sink.sector.eq(crt_sec),
             port.sink.count.eq(1),
             port.sink.data.eq(reverse_bytes(conv.source.data)),
             If(port.sink.ready,
                 conv.source.ready.eq(1),
                 NextValue(count, count + 1),
                 If(port.sink.last,
                     NextState("WAIT-ACK")
                 )
             ),
 
             # Monitor errors
             port.source.ready.eq(1),
-            If(port.source.valid & port.source.ready,
-                If(port.source.failed,
-                    self.irq.eq(1),
-                    NextValue(self.error.status, 1),
-                    NextState("IDLE"),
-                )
+            If(port.source.valid & port.source.ready & port.source.failed,
+                self.irq.eq(1),
+                NextValue(self.error.status, 1),
+                NextState("IDLE"),
             )
         )
         fsm.act("WAIT-ACK",
             port.source.ready.eq(1),
             If(port.source.valid,
                 If(port.source.failed,
                     NextValue(self.error.status, 1),
-                ),
-                self.irq.eq(1),
-                NextState("IDLE")
+                    self.irq.eq(1),
+                    NextState("IDLE")
+                ).Elif(crt_sec == (self.sector.storage + self.nsectors.storage - 1),
+                    self.irq.eq(1),
+                    NextState("IDLE")
+                ).Else(
+                    NextValue(count,    0),
+                    NextValue(crt_sec,  crt_sec + 1),
+                    NextValue(crt_base, crt_base + 512),
+                    NextState("READ-DATA-DMA")
+                )
             )
         )
```

### Comparing `litesata-2023.4/litesata/frontend/identify.py` & `litesata-2023.8/litesata/frontend/identify.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/frontend/raid.py` & `litesata-2023.8/litesata/frontend/raid.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/gen.py` & `litesata-2023.8/litesata/gen.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/phy/__init__.py` & `litesata-2023.8/litesata/phy/__init__.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/phy/a7sataphy.py` & `litesata-2023.8/litesata/phy/a7sataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/phy/ctrl.py` & `litesata-2023.8/litesata/phy/ctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2017 Johan Klockars <Johan.Klockars@hasselblad.com>
 # Copyright (c) 2016 Olof Kindgren <olof.kindgren@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litesata.common import *
 
-from migen.genlib.misc import WaitTimer
+from litex.gen.genlib.misc import WaitTimer
 
 # LiteSATAPHYCtrl ----------------------------------------------------------------------------------
 
 class LiteSATAPHYCtrl(Module):
     """SATA PHY Controller
 
     Manages link reset/initialization and OOB sequence.
@@ -157,15 +157,15 @@
             If(align_count == 0,
                 NextState("READY")
             )
         )
 
         # Wait alignment stability for 5ms before declaring ctrl is ready, reset the RX part of
         # the transceiver when misalignment is detected.
-        stability_timer = WaitTimer(int(5e-3*clk_freq))
+        stability_timer = WaitTimer(5e-3*clk_freq)
         self.submodules += stability_timer
 
         fsm.act("READY",
             source.data.eq(primitives["SYNC"]),
             source.charisk.eq(0b0001),
             stability_timer.wait.eq(1),
             self.ready.eq(stability_timer.done),
```

### Comparing `litesata-2023.4/litesata/phy/datapath.py` & `litesata-2023.8/litesata/phy/datapath.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is part of LiteSATA.
 #
 # Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litesata.common import *
 
-from migen.genlib.misc import WaitTimer
+from litex.gen.genlib.misc import WaitTimer
 
 # LiteSATAPHYDatapathRX ----------------------------------------------------------------------------
 
 class LiteSATAPHYDatapathRX(Module):
     """SATA PHY RX datapath
 
     Manages the RX datapath between the transceiver and the SATA core.
```

### Comparing `litesata-2023.4/litesata/phy/k7sataphy.py` & `litesata-2023.8/litesata/phy/k7sataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/phy/uspsataphy.py` & `litesata-2023.8/litesata/phy/uspsataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata/phy/ussataphy.py` & `litesata-2023.8/litesata/phy/ussataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/litesata.egg-info/PKG-INFO` & `litesata-2023.8/litesata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesata
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable SATA core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litesata
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litesata-2023.4/litesata.egg-info/SOURCES.txt` & `litesata-2023.8/litesata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/setup.py` & `litesata-2023.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = fp.read()
 
 setup(
     name="litesata",
     description="Small footprint and configurable SATA core",
     long_description              = long_description,
     long_description_content_type = "text/markdown",
-    version="2023.04",
+    version="2023.08",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/litesata",
     test_suite="test",
     license="BSD",
     python_requires="~=3.6",
```

### Comparing `litesata-2023.4/test/test_bist.py` & `litesata-2023.8/test/test_bist.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_command.py` & `litesata-2023.8/test/test_command.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_link.py` & `litesata-2023.8/test/test_link.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_link_cont.py` & `litesata-2023.8/test/test_link_cont.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_link_crc.py` & `litesata-2023.8/test/test_link_crc.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_link_scrambler.py` & `litesata-2023.8/test/test_link_scrambler.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_mirroring.py` & `litesata-2023.8/test/test_mirroring.py`

 * *Files identical despite different names*

### Comparing `litesata-2023.4/test/test_striping.py` & `litesata-2023.8/test/test_striping.py`

 * *Files identical despite different names*

