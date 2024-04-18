# Comparing `tmp/liteiclink-2023.4.tar.gz` & `tmp/liteiclink-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteiclink-2023.4.tar", last modified: Thu Apr 18 20:32:02 2024, max compression
+gzip compressed data, was "liteiclink-2023.8.tar", last modified: Thu Apr 18 20:32:22 2024, max compression
```

## Comparing `liteiclink-2023.4.tar` & `liteiclink-2023.8.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:02.924673 liteiclink-2023.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)      760 2024-04-18 20:31:56.000000 liteiclink-2023.4/CONTRIBUTORS
--rw-r--r--   0 timkpaine   (501) staff       (20)     1685 2024-04-18 20:28:10.000000 liteiclink-2023.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      105 2024-04-18 20:28:10.000000 liteiclink-2023.4/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     5065 2024-04-18 20:32:02.924421 liteiclink-2023.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4161 2024-04-18 20:28:10.000000 liteiclink-2023.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:02.919004 liteiclink-2023.4/liteiclink/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.4/liteiclink/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:02.922294 liteiclink-2023.4/liteiclink/serdes/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.4/liteiclink/serdes/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4080 2024-04-18 20:28:10.000000 liteiclink-2023.4/liteiclink/serdes/clock_aligner.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1303 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    75986 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gth_ultrascale.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5691 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gth_ultrascale_init.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    49838 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gtp_7series.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10495 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gtp_7series_init.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    50286 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gtx_7series.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5384 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gtx_7series_init.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    66473 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gty_ultrascale.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5680 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/gty_ultrascale_init.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    32626 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serdes/serdes_ecp5.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:02.923840 liteiclink-2023.4/liteiclink/serwb/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.4/liteiclink/serwb/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1905 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/core.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4587 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/datapath.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    18522 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/etherbone.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11566 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/genphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5932 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/kuserdes.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5253 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/packet.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    13682 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/phy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7181 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/s7serdes.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3131 2024-04-18 20:31:56.000000 liteiclink-2023.4/liteiclink/serwb/scrambler.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      105 2024-04-18 20:28:10.000000 liteiclink-2023.4/liteiclink/transceiver.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:02.924042 liteiclink-2023.4/liteiclink.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5065 2024-04-18 20:32:02.000000 liteiclink-2023.4/liteiclink.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      970 2024-04-18 20:32:02.000000 liteiclink-2023.4/liteiclink.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:32:02.000000 liteiclink-2023.4/liteiclink.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       55 2024-04-18 20:32:02.000000 liteiclink-2023.4/liteiclink.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       11 2024-04-18 20:32:02.000000 liteiclink-2023.4/liteiclink.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:32:02.924726 liteiclink-2023.4/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     1337 2024-04-18 20:31:56.000000 liteiclink-2023.4/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:22.718871 liteiclink-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      760 2024-04-18 20:31:56.000000 liteiclink-2023.8/CONTRIBUTORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1685 2024-04-18 20:28:10.000000 liteiclink-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      105 2024-04-18 20:28:10.000000 liteiclink-2023.8/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5065 2024-04-18 20:32:22.718584 liteiclink-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4161 2024-04-18 20:28:10.000000 liteiclink-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:22.712262 liteiclink-2023.8/liteiclink/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.8/liteiclink/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:22.716020 liteiclink-2023.8/liteiclink/serdes/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.8/liteiclink/serdes/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4080 2024-04-18 20:28:10.000000 liteiclink-2023.8/liteiclink/serdes/clock_aligner.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1362 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    54054 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gth3_ultrascale.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    62658 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gth4_ultrascale.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      467 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gth_ultrascale.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6021 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gth_ultrascale_init.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    50742 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gtp_7series.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10467 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gtp_7series_init.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    51195 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gtx_7series.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5385 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gtx_7series_init.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    67328 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gty_ultrascale.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5690 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/gty_ultrascale_init.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    32491 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serdes/serdes_ecp5.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:22.717676 liteiclink-2023.8/liteiclink/serwb/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:28:10.000000 liteiclink-2023.8/liteiclink/serwb/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1905 2024-04-18 20:31:56.000000 liteiclink-2023.8/liteiclink/serwb/core.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5170 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/datapath.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    18522 2024-04-18 20:31:56.000000 liteiclink-2023.8/liteiclink/serwb/etherbone.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11601 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/genphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5952 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/kuserdes.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5257 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/packet.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    13691 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/phy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7202 2024-04-18 20:32:12.000000 liteiclink-2023.8/liteiclink/serwb/s7serdes.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3131 2024-04-18 20:31:56.000000 liteiclink-2023.8/liteiclink/serwb/scrambler.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      105 2024-04-18 20:28:10.000000 liteiclink-2023.8/liteiclink/transceiver.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:32:22.718129 liteiclink-2023.8/liteiclink.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5065 2024-04-18 20:32:22.000000 liteiclink-2023.8/liteiclink.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1044 2024-04-18 20:32:22.000000 liteiclink-2023.8/liteiclink.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:32:22.000000 liteiclink-2023.8/liteiclink.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       55 2024-04-18 20:32:22.000000 liteiclink-2023.8/liteiclink.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2024-04-18 20:32:22.000000 liteiclink-2023.8/liteiclink.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:32:22.718927 liteiclink-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     1337 2024-04-18 20:32:17.000000 liteiclink-2023.8/setup.py
```

### Comparing `liteiclink-2023.4/CONTRIBUTORS` & `liteiclink-2023.8/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/LICENSE` & `liteiclink-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/PKG-INFO` & `liteiclink-2023.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteiclink
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable Inter-Chip communication cores
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/liteiclink
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `liteiclink-2023.4/README.md` & `liteiclink-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/liteiclink/serdes/clock_aligner.py` & `liteiclink-2023.8/liteiclink/serdes/clock_aligner.py`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/liteiclink/serdes/common.py` & `liteiclink-2023.8/liteiclink/serdes/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
+from litex.gen import *
+
 # DRP ----------------------------------------------------------------------------------------------
 
 _drp_layout = [
     ("clk",                1, DIR_M_TO_S),
     ("en",                 1, DIR_M_TO_S),
     ("we",                 1, DIR_M_TO_S),
     ("rdy",                1, DIR_S_TO_M),
@@ -18,18 +20,20 @@
     ("do",      "data_width", DIR_S_TO_M),
 ]
 
 
 class DRPInterface(Record):
     def __init__(self, address_width=9, data_width=16):
         Record.__init__(self, set_layout_parameters(_drp_layout,
-            address_width=address_width, data_width=data_width))
+            address_width = address_width,
+            data_width    = data_width,
+        ))
 
 
-class DRPMux(Module, DRPInterface):
+class DRPMux(LiteXModule, DRPInterface):
     def __init__(self, **kwargs):
         DRPInterface.__init__(self, **kwargs)
         self.sel = Signal(4)
         self.interfaces = []
 
     def add_interface(self, interface):
         self.interfaces.append(interface)
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gth_ultrascale.py` & `liteiclink-2023.8/liteiclink/serdes/gth4_ultrascale.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 # This file is part of LiteICLink.
 #
-# Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2017-2023 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2021 Sylvain Munaut <tnt@246tNt.com>
 # Copyright (c) 2017 Sebastien Bourdeauducq <sb@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
@@ -19,15 +20,15 @@
 from liteiclink.serdes.gth_ultrascale_init import GTHTXInit, GTHRXInit
 from liteiclink.serdes.clock_aligner import BruteforceClockAligner
 
 from liteiclink.serdes.common import *
 
 # GTH Channel PLL ----------------------------------------------------------------------------------
 
-class GTHChannelPLL(Module):
+class GTHChannelPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.refclk = refclk
         self.reset  = Signal()
         self.lock   = Signal()
         self.config = self.compute_config(refclk_freq, linerate)
 
     @staticmethod
@@ -83,15 +84,15 @@
            vco_freq = config["vco_freq"]/1e9,
            d        = config["d"],
            linerate = config["linerate"]/1e9)
         return r
 
 # GTH Quad PLL -------------------------------------------------------------------------------------
 
-class GTHQuadPLLBase(Module):
+class GTHQuadPLLBase(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.clk       = Signal()
         self.refclk    = Signal()
         self.reset     = Signal()
         self.lock      = Signal()
         self.powerdown = Signal()
         self.config = config = self.compute_config(refclk_freq, linerate)
@@ -220,62 +221,14 @@
            clkout   = config["clkout"]/1e9,
            vco_freq = config["vco_freq"]/1e9,
            qpll     = config["qpll"].upper(),
            d        = config["d"],
            linerate = config["linerate"]/1e9)
         return r
 
-
-class GTH3QuadPLL(GTHQuadPLLBase):
-    name = "GTHE3_COMMON"
-
-    def __init__(self, refclk, refclk_freq, linerate):
-        super().__init__(refclk, refclk_freq, linerate)
-
-        # Update params common to GTHE3/4 but that have different
-        # values and differs from the default ones
-        self.gth_params.update(
-            # QPLL0
-            p_QPLL0_CFG0        = 0b0011001000011100,
-            p_QPLL0_CFG1        = 0b0001000000011000,
-            p_QPLL0_CFG1_G3     = 0b0001000000011000,
-            p_QPLL0_CFG2        = 0b0000000001001000,
-            p_QPLL0_CFG2_G3     = 0b0000000001001000,
-            p_QPLL0_CFG3        = 0b0000000100100000,
-            p_QPLL0_CFG4        = 0b0000000000001001,
-            p_QPLL0_CP          = 0b0111111111,
-            p_QPLL0_CP_G3       = 0b1111111111,
-            p_QPLL0_FBDIV_G3    = self.config["n"], # ?
-            p_QPLL0_INIT_CFG0   = 0b0000001010110010,
-            p_QPLL0_INIT_CFG1   = 0b00000000,
-            p_QPLL0_LOCK_CFG    = 0b0010000111101000,
-            p_QPLL0_LOCK_CFG_G3 = 0b0010000111101000,
-            p_QPLL0_LPF         = 0b1111111100,
-            p_QPLL0_LPF_G3      = 0b0000010101,
-
-            # QPLL1
-            p_QPLL1_CFG0        = 0b0011001000011100,
-            p_QPLL1_CFG1        = 0b0001000000011000,
-            p_QPLL1_CFG1_G3     = 0b0001000000011000,
-            p_QPLL1_CFG2        = 0b0000000001000000,
-            p_QPLL1_CFG2_G3     = 0b0000000001000000,
-            p_QPLL1_CFG3        = 0b0000000100100000,
-            p_QPLL1_CFG4        = 0b0000000000001001,
-            p_QPLL1_CP          = 0b0001111111,
-            p_QPLL1_CP_G3       = 0b1111111111,
-            p_QPLL1_FBDIV_G3    = self.config["n"], # ?
-            p_QPLL1_INIT_CFG0   = 0b0000001010110010,
-            p_QPLL1_INIT_CFG1   = 0b00000000,
-            p_QPLL1_LOCK_CFG    = 0b0010000111101000,
-            p_QPLL1_LOCK_CFG_G3 = 0b0010000111101000,
-            p_QPLL1_LPF         = 0b1111111100,
-            p_QPLL1_LPF_G3      = 0b0000010101,
-        )
-
-
 class GTH4QuadPLL(GTHQuadPLLBase):
     name = "GTHE4_COMMON"
 
     def __init__(self, refclk, refclk_freq, linerate):
         super().__init__(refclk, refclk_freq, linerate)
 
         # Update params common to GTHE3/4 but that have different
@@ -345,19 +298,18 @@
             i_SDM1DATA              = 0b0000000000000000000000000,
             i_SDM0WIDTH             = 0b00,
             i_SDM1WIDTH             = 0b00,
             i_QPLL0FBDIV            = 0b00000000,
             i_QPLL1FBDIV            = 0b00000000,
         )
 
+# GTH4 ---------------------------------------------------------------------------------------------
 
-# GTH ----------------------------------------------------------------------------------------------
-
-class GTHBase(Module, AutoCSR):
-    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq,
+class GTH4(LiteXModule):
+    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq, tx_clk=None, rx_clk=None,
         data_width          = 20,
         tx_buffer_enable    = False,
         rx_buffer_enable    = False,
         clock_aligner       = True,
         clock_aligner_comma = 0b0101111100,
         tx_polarity         = 0,
         rx_polarity         = 0,
@@ -391,15 +343,15 @@
 
         use_cpll  = isinstance(pll, GTHChannelPLL)
         use_qpll0 = isinstance(pll, GTHQuadPLLBase) and pll.config["qpll"] == "qpll0"
         use_qpll1 = isinstance(pll, GTHQuadPLLBase) and pll.config["qpll"] == "qpll1"
 
         self.nwords = nwords = data_width//10
 
-        self.submodules.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
+        self.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
         self.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
         self.submodules += self.decoders
 
         # Transceiver direct clock outputs (useful to specify clock constraints)
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
@@ -428,74 +380,93 @@
             MultiReg(self.rx_prbs_pause, rx_prbs_pause, "rx"),
             MultiReg(rx_prbs_errors, self.rx_prbs_errors, "sys"),
         ]
 
         # # #
 
         # TX init ----------------------------------------------------------------------------------
-        self.submodules.tx_init = tx_init = GTHTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
+        self.tx_init = tx_init = GTHTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
         self.comb += [
             self.tx_ready.eq(tx_init.done),
             tx_init.restart.eq(~self.tx_enable)
         ]
 
         # RX init ----------------------------------------------------------------------------------
-        self.submodules.rx_init = rx_init = GTHRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
+        self.rx_init = rx_init = GTHRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
         self.comb += [
             self.rx_ready.eq(rx_init.done),
             rx_init.restart.eq(~self.rx_enable)
         ]
 
         # PLL ----------------------------------------------------------------------------------
         self.comb += [
             tx_init.plllock.eq(pll.lock),
             rx_init.plllock.eq(pll.lock)
         ]
         if pll_master:
             self.comb += pll.reset.eq(tx_init.pllreset)
 
         # DRP mux ----------------------------------------------------------------------------------
-        self.submodules.drp_mux = drp_mux = DRPMux()
+        self.drp_mux = drp_mux = DRPMux()
         drp_mux.add_interface(self.drp)
 
         # GTHE3_CHANNEL instance -------------------------------------------------------------------
         txdata = Signal(data_width)
         rxdata = Signal(data_width)
         rxphaligndone = Signal()
 
         self.gth_params = dict(
             p_ACJTAG_DEBUG_MODE            = 0b0,
             p_ACJTAG_MODE                  = 0b0,
             p_ACJTAG_RESET                 = 0b0,
+            p_ADAPT_CFG0                   = 0b0001000000000000,
+            p_ADAPT_CFG1                   = 0b1100100000000000,
+            p_ADAPT_CFG2                   = 0b0000000000000000,
             p_ALIGN_COMMA_DOUBLE           = "FALSE",
             p_ALIGN_COMMA_ENABLE           = 0b1111111111,
             p_ALIGN_COMMA_WORD             = 2 if data_width == 20 else 4,
             p_ALIGN_MCOMMA_DET             = "TRUE",
             p_ALIGN_MCOMMA_VALUE           = 0b1010000011,
             p_ALIGN_PCOMMA_DET             = "TRUE",
             p_ALIGN_PCOMMA_VALUE           = 0b0101111100,
             p_A_RXOSCALRESET               = 0b0,
             p_A_RXPROGDIVRESET             = 0b0,
+            p_A_RXTERMINATION              = 0b1,
+            p_A_TXDIFFCTRL                 = 0b01100,
             p_A_TXPROGDIVRESET             = 0b0,
+            p_CAPBYPASS_FORCE              = 0b0,
             p_CBCC_DATA_SOURCE_SEL         = "ENCODED",
             p_CDR_SWAP_MODE_EN             = 0b0,
+            p_CFOK_PWRSVE_EN               = 0b1,
             p_CHAN_BOND_KEEP_ALIGN         = "FALSE",
             p_CHAN_BOND_MAX_SKEW           = 1,
             p_CHAN_BOND_SEQ_1_1            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_2            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_3            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_4            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_ENABLE       = 0b1111,
             p_CHAN_BOND_SEQ_2_1            = 0b0000000000,
             p_CHAN_BOND_SEQ_2_2            = 0b0000000000,
             p_CHAN_BOND_SEQ_2_3            = 0b0000000000,
             p_CHAN_BOND_SEQ_2_4            = 0b0000000000,
             p_CHAN_BOND_SEQ_2_ENABLE       = 0b1111,
             p_CHAN_BOND_SEQ_2_USE          = "FALSE",
             p_CHAN_BOND_SEQ_LEN            = 1,
+            p_CH_HSPMUX                    = 0b0010010000100100,
+            p_CKCAL1_CFG_0                 = 0b1100000011000000,
+            p_CKCAL1_CFG_1                 = 0b0101000011000000,
+            p_CKCAL1_CFG_2                 = 0b0000000000001010,
+            p_CKCAL1_CFG_3                 = 0b0000000000000000,
+            p_CKCAL2_CFG_0                 = 0b1100000011000000,
+            p_CKCAL2_CFG_1                 = 0b1000000011000000,
+            p_CKCAL2_CFG_2                 = 0b0000000000000000,
+            p_CKCAL2_CFG_3                 = 0b0000000000000000,
+            p_CKCAL2_CFG_4                 = 0b0000000000000000,
+            p_CKCAL_RSVD0                  = 0b0000000010000000,
+            p_CKCAL_RSVD1                  = 0b0000010000000000,
             p_CLK_CORRECT_USE              = "FALSE",
             p_CLK_COR_KEEP_IDLE            = "FALSE",
             p_CLK_COR_PRECEDENCE           = "TRUE",
             p_CLK_COR_REPEAT_WAIT          = 0,
             p_CLK_COR_SEQ_1_1              = 0b0000000000,
             p_CLK_COR_SEQ_1_2              = 0b0000000000,
             p_CLK_COR_SEQ_1_3              = 0b0000000000,
@@ -504,189 +475,434 @@
             p_CLK_COR_SEQ_2_1              = 0b0000000000,
             p_CLK_COR_SEQ_2_2              = 0b0000000000,
             p_CLK_COR_SEQ_2_3              = 0b0000000000,
             p_CLK_COR_SEQ_2_4              = 0b0000000000,
             p_CLK_COR_SEQ_2_ENABLE         = 0b1111,
             p_CLK_COR_SEQ_2_USE            = "FALSE",
             p_CLK_COR_SEQ_LEN              = 1,
+            p_CPLL_CFG0                    = 0b0000000111111010,
+            p_CPLL_CFG1                    = 0b0000000000100011,
+            p_CPLL_CFG2                    = 0b0000000000000010,
+            p_CPLL_CFG3                    = 0b0000000000000000,
             p_CPLL_INIT_CFG0               = 0b0000001010110010,
             p_CPLL_LOCK_CFG                = 0b0000000111101000,
+            p_CTLE3_OCAP_EXT_CTRL          = 0b000,
+            p_CTLE3_OCAP_EXT_EN            = 0b0,
             p_DDI_CTRL                     = 0b00,
             p_DDI_REALIGN_WAIT             = 15,
             p_DEC_MCOMMA_DETECT            = "TRUE",
             p_DEC_PCOMMA_DETECT            = "TRUE",
             p_DEC_VALID_COMMA_ONLY         = "TRUE",
+            p_DELAY_ELEC                   = 0b0,
             p_DMONITOR_CFG0                = 0b0000000000,
             p_DMONITOR_CFG1                = 0b00000000,
             p_ES_CLK_PHASE_SEL             = 0b0,
             p_ES_CONTROL                   = 0b000000,
             p_ES_ERRDET_EN                 = "FALSE",
             p_ES_EYE_SCAN_EN               = "FALSE",
             p_ES_HORZ_OFFSET               = 0b000000000000,
             p_ES_PRESCALE                  = 0b00000,
             p_ES_QUALIFIER0                = 0b0000000000000000,
             p_ES_QUALIFIER1                = 0b0000000000000000,
             p_ES_QUALIFIER2                = 0b0000000000000000,
             p_ES_QUALIFIER3                = 0b0000000000000000,
             p_ES_QUALIFIER4                = 0b0000000000000000,
+            p_ES_QUALIFIER5                = 0b0000000000000000,
+            p_ES_QUALIFIER6                = 0b0000000000000000,
+            p_ES_QUALIFIER7                = 0b0000000000000000,
+            p_ES_QUALIFIER8                = 0b0000000000000000,
+            p_ES_QUALIFIER9                = 0b0000000000000000,
             p_ES_QUAL_MASK0                = 0b0000000000000000,
             p_ES_QUAL_MASK1                = 0b0000000000000000,
             p_ES_QUAL_MASK2                = 0b0000000000000000,
             p_ES_QUAL_MASK3                = 0b0000000000000000,
             p_ES_QUAL_MASK4                = 0b0000000000000000,
+            p_ES_QUAL_MASK5                = 0b0000000000000000,
+            p_ES_QUAL_MASK6                = 0b0000000000000000,
+            p_ES_QUAL_MASK7                = 0b0000000000000000,
+            p_ES_QUAL_MASK8                = 0b0000000000000000,
+            p_ES_QUAL_MASK9                = 0b0000000000000000,
             p_ES_SDATA_MASK0               = 0b0000000000000000,
             p_ES_SDATA_MASK1               = 0b0000000000000000,
             p_ES_SDATA_MASK2               = 0b0000000000000000,
             p_ES_SDATA_MASK3               = 0b0000000000000000,
             p_ES_SDATA_MASK4               = 0b0000000000000000,
+            p_ES_SDATA_MASK5               = 0b0000000000000000,
+            p_ES_SDATA_MASK6               = 0b0000000000000000,
+            p_ES_SDATA_MASK7               = 0b0000000000000000,
+            p_ES_SDATA_MASK8               = 0b0000000000000000,
+            p_ES_SDATA_MASK9               = 0b0000000000000000,
             p_EYE_SCAN_SWAP_EN             = 0b0,
             p_FTS_DESKEW_SEQ_ENABLE        = 0b1111,
             p_FTS_LANE_DESKEW_CFG          = 0b1111,
             p_FTS_LANE_DESKEW_EN           = "FALSE",
             p_GEARBOX_MODE                 = 0b00000,
+            p_ISCAN_CK_PH_SEL2             = 0b0,
             p_LOCAL_MASTER                 = 0b1,
+            p_LPBK_BIAS_CTRL               = 0b100,
+            p_LPBK_EN_RCAL_B               = 0b0,
+            p_LPBK_EXT_RCAL                = 0b1000,
+            p_LPBK_IND_CTRL0               = 0b000,
+            p_LPBK_IND_CTRL1               = 0b000,
+            p_LPBK_IND_CTRL2               = 0b000,
+            p_LPBK_RG_CTRL                 = 0b1110,
             p_OOBDIVCTL                    = 0b00,
             p_OOB_PWRUP                    = 0b0,
             p_PCI3_AUTO_REALIGN            = "OVR_1K_BLK",
             p_PCI3_PIPE_RX_ELECIDLE        = 0b0,
             p_PCI3_RX_ASYNC_EBUF_BYPASS    = 0b00,
             p_PCI3_RX_ELECIDLE_EI2_ENABLE  = 0b0,
             p_PCI3_RX_ELECIDLE_H2L_COUNT   = 0b000000,
             p_PCI3_RX_ELECIDLE_H2L_DISABLE = 0b000,
             p_PCI3_RX_ELECIDLE_HI_COUNT    = 0b000000,
             p_PCI3_RX_ELECIDLE_LP4_DISABLE = 0b0,
             p_PCI3_RX_FIFO_DISABLE         = 0b0,
+            p_PCIE3_CLK_COR_EMPTY_THRSH    = 0b00000,
+            p_PCIE3_CLK_COR_FULL_THRSH     = 0b010000,
+            p_PCIE3_CLK_COR_MAX_LAT        = 0b00100,
+            p_PCIE3_CLK_COR_MIN_LAT        = 0b00000,
+            p_PCIE3_CLK_COR_THRSH_TIMER    = 0b001000,
+            p_PCIE_BUFG_DIV_CTRL           = 0b0011010100000000,
+            p_PCIE_PLL_SEL_MODE_GEN12      = 0b10,
+            p_PCIE_PLL_SEL_MODE_GEN3       = 0b10,
+            p_PCIE_PLL_SEL_MODE_GEN4       = 0b10,
+            p_PCIE_RXPCS_CFG_GEN3          = 0b0000101010100101,
+            p_PCIE_RXPMA_CFG               = 0b0010100000001010,
             p_PCIE_TXPCS_CFG_GEN3          = 0b0010010010100100,
+            p_PCIE_TXPMA_CFG               = 0b0010100000001010,
             p_PCS_PCIE_EN                  = "FALSE",
             p_PCS_RSVD0                    = 0b0000000000000000,
             p_PD_TRANS_TIME_FROM_P2        = 0b000000111100,
             p_PD_TRANS_TIME_NONE_P2        = 0b00011001,
             p_PD_TRANS_TIME_TO_P2          = 0b01100100,
+            p_PREIQ_FREQ_BST               = 0,
             p_PROCESS_PAR                  = 0b010,
             p_RATE_SW_USE_DRP              = 0b1,
+            p_RCLK_SIPO_DLY_ENB            = 0b0,
+            p_RCLK_SIPO_INV_EN             = 0b0,
             p_RESET_POWERSAVE_DISABLE      = 0b0,
+            p_RTX_BUF_CML_CTRL             = 0b010,
+            p_RTX_BUF_TERM_CTRL            = 0b00,
             p_RXBUFRESET_TIME              = 0b00011,
             p_RXBUF_ADDR_MODE              = "FAST",
             p_RXBUF_EIDLE_HI_CNT           = 0b1000,
             p_RXBUF_EIDLE_LO_CNT           = 0b0000,
             p_RXBUF_RESET_ON_CB_CHANGE     = "TRUE",
             p_RXBUF_RESET_ON_COMMAALIGN    = "FALSE",
             p_RXBUF_RESET_ON_EIDLE         = "FALSE",
             p_RXBUF_RESET_ON_RATE_CHANGE   = "TRUE",
             p_RXCDRFREQRESET_TIME          = 0b00001,
             p_RXCDRPHRESET_TIME            = 0b00001,
+            p_RXCDR_CFG0                   = 0b0000000000000011,
+            p_RXCDR_CFG0_GEN3              = 0b0000000000000011,
+            p_RXCDR_CFG1                   = 0b0000000000000000,
+            p_RXCDR_CFG1_GEN3              = 0b0000000000000000,
+            p_RXCDR_CFG2                   = 0b0000001001101001,
+            p_RXCDR_CFG2_GEN2              = 0b1001101001,
+            p_RXCDR_CFG2_GEN3              = 0b0000001001101001,
+            p_RXCDR_CFG2_GEN4              = 0b0000000101100100,
+            p_RXCDR_CFG3                   = 0b0000000000010000,
+            p_RXCDR_CFG3_GEN2              = 0b010000,
+            p_RXCDR_CFG3_GEN3              = 0b0000000000010000,
+            p_RXCDR_CFG3_GEN4              = 0b0000000000010010,
+            p_RXCDR_CFG4                   = 0b0101110011110110,
+            p_RXCDR_CFG4_GEN3              = 0b0101110011110110,
+            p_RXCDR_CFG5                   = 0b1011010001101011,
+            p_RXCDR_CFG5_GEN3              = 0b0001010001101011,
             p_RXCDR_FR_RESET_ON_EIDLE      = 0b0,
             p_RXCDR_HOLD_DURING_EIDLE      = 0b0,
+            p_RXCDR_LOCK_CFG0              = 0b0010001000000001,
+            p_RXCDR_LOCK_CFG1              = 0b1001111111111111,
+            p_RXCDR_LOCK_CFG2              = 0b0111011111000011,
+            p_RXCDR_LOCK_CFG3              = 0b0000000000000001,
+            p_RXCDR_LOCK_CFG4              = 0b0000000000000000,
             p_RXCDR_PH_RESET_ON_EIDLE      = 0b0,
+            p_RXCFOK_CFG0                  = 0b0000000000000000,
+            p_RXCFOK_CFG1                  = 0b1000000000010101,
+            p_RXCFOK_CFG2                  = 0b0000001010101110,
+            p_RXCKCAL1_IQ_LOOP_RST_CFG     = 0b0000000000000100,
+            p_RXCKCAL1_I_LOOP_RST_CFG      = 0b0000000000000100,
+            p_RXCKCAL1_Q_LOOP_RST_CFG      = 0b0000000000000100,
+            p_RXCKCAL2_DX_LOOP_RST_CFG     = 0b0000000000000100,
+            p_RXCKCAL2_D_LOOP_RST_CFG      = 0b0000000000000100,
+            p_RXCKCAL2_S_LOOP_RST_CFG      = 0b0000000000000100,
+            p_RXCKCAL2_X_LOOP_RST_CFG      = 0b0000000000000100,
             p_RXDFELPMRESET_TIME           = 0b0001111,
+            p_RXDFELPM_KL_CFG0             = 0b0000000000000000,
+            p_RXDFELPM_KL_CFG1             = 0b1010000011100010,
+            p_RXDFELPM_KL_CFG2             = 0b0000000100000000,
             p_RXDFE_CFG0                   = 0b0000101000000000,
             p_RXDFE_CFG1                   = 0b0000000000000000,
+            p_RXDFE_GC_CFG0                = 0b0000000000000000,
+            p_RXDFE_GC_CFG1                = 0b1000000000000000,
+            p_RXDFE_GC_CFG2                = 0b1111111111100000,
+            p_RXDFE_H2_CFG0                = 0b0000000000000000,
+            p_RXDFE_H2_CFG1                = 0b0000000000000010,
+            p_RXDFE_H3_CFG0                = 0b0000000000000000,
+            p_RXDFE_H3_CFG1                = 0b1000000000000010,
+            p_RXDFE_H4_CFG0                = 0b0000000000000000,
+            p_RXDFE_H4_CFG1                = 0b1000000000000010,
+            p_RXDFE_H5_CFG0                = 0b0000000000000000,
+            p_RXDFE_H5_CFG1                = 0b1000000000000010,
+            p_RXDFE_H6_CFG0                = 0b0000000000000000,
+            p_RXDFE_H6_CFG1                = 0b1000000000000010,
+            p_RXDFE_H7_CFG0                = 0b0000000000000000,
+            p_RXDFE_H7_CFG1                = 0b1000000000000010,
+            p_RXDFE_H8_CFG0                = 0b0000000000000000,
+            p_RXDFE_H8_CFG1                = 0b1000000000000010,
+            p_RXDFE_H9_CFG0                = 0b0000000000000000,
+            p_RXDFE_H9_CFG1                = 0b1000000000000010,
+            p_RXDFE_HA_CFG0                = 0b0000000000000000,
+            p_RXDFE_HA_CFG1                = 0b1000000000000010,
+            p_RXDFE_HB_CFG0                = 0b0000000000000000,
+            p_RXDFE_HB_CFG1                = 0b1000000000000010,
+            p_RXDFE_HC_CFG0                = 0b0000000000000000,
+            p_RXDFE_HC_CFG1                = 0b1000000000000010,
+            p_RXDFE_HD_CFG0                = 0b0000000000000000,
+            p_RXDFE_HD_CFG1                = 0b1000000000000010,
+            p_RXDFE_HE_CFG0                = 0b0000000000000000,
+            p_RXDFE_HE_CFG1                = 0b1000000000000010,
+            p_RXDFE_HF_CFG0                = 0b0000000000000000,
+            p_RXDFE_HF_CFG1                = 0b1000000000000010,
+            p_RXDFE_KH_CFG0                = 0b0000000000000000,
+            p_RXDFE_KH_CFG1                = 0b1000000000000000,
+            p_RXDFE_KH_CFG2                = 0b0010011000010011,
+            p_RXDFE_KH_CFG3                = 0b0100000100011100,
+            p_RXDFE_OS_CFG0                = 0b0000000000000000,
+            p_RXDFE_OS_CFG1                = 0b1000000000000010,
+            p_RXDFE_PWR_SAVING             = 0b1,
+            p_RXDFE_UT_CFG0                = 0b0000000000000000,
+            p_RXDFE_UT_CFG1                = 0b0000000000000011,
+            p_RXDFE_UT_CFG2                = 0b0000000000000000,
+            p_RXDFE_VP_CFG0                = 0b0000000000000000,
+            p_RXDFE_VP_CFG1                = 0b1000000000110011,
+            p_RXDLY_CFG                    = 0b0000000000010000,
             p_RXDLY_LCFG                   = 0b0000000000110000,
+            p_RXELECIDLE_CFG               = "SIGCFG_4",
             p_RXGBOX_FIFO_INIT_RD_ADDR     = 4,
             p_RXGEARBOX_EN                 = "FALSE",
             p_RXISCANRESET_TIME            = 0b00001,
             p_RXLPM_CFG                    = 0b0000000000000000,
+            p_RXLPM_GC_CFG                 = 0b1000000000000000,
             p_RXLPM_KH_CFG0                = 0b0000000000000000,
             p_RXLPM_KH_CFG1                = 0b0000000000000010,
+            p_RXLPM_OS_CFG0                = 0b0000000000000000,
+            p_RXLPM_OS_CFG1                = 0b1000000000000010,
             p_RXOOB_CFG                    = 0b000000110,
             p_RXOOB_CLK_CFG                = "PMA",
             p_RXOSCALRESET_TIME            = 0b00011,
             p_RXPCSRESET_TIME              = 0b00011,
             p_RXPHBEACON_CFG               = 0b0000000000000000,
+            p_RXPHDLY_CFG                  = 0b0010000001110000,
             p_RXPHSAMP_CFG                 = 0b0010000100000000,
+            p_RXPHSLIP_CFG                 = 0b1001100100110011,
             p_RXPH_MONITOR_SEL             = 0b00000,
+            p_RXPI_AUTO_BW_SEL_BYPASS      = 0b0,
+            p_RXPI_CFG0                    = 0b0000000000000010,
+            p_RXPI_CFG1                    = 0b0000000000010101,
             p_RXPI_LPM                     = 0b0,
+            p_RXPI_SEL_LC                  = 0b00,
+            p_RXPI_STARTCODE               = 0b00,
             p_RXPI_VREFSEL                 = 0b0,
             p_RXPMACLK_SEL                 = "DATA",
             p_RXPMARESET_TIME              = 0b00011,
             p_RXPRBS_ERR_LOOPBACK          = 0b0,
             p_RXPRBS_LINKACQ_CNT           = 15,
+            p_RXREFCLKDIV2_SEL             = 0b0,
             p_RXSLIDE_AUTO_WAIT            = 7,
             p_RXSLIDE_MODE                 = "OFF" if rx_buffer_enable else "PCS",
             p_RXSYNC_MULTILANE             = 0b0,
             p_RXSYNC_OVRD                  = 0b0,
             p_RXSYNC_SKIP_DA               = 0b0,
             p_RX_AFE_CM_EN                 = 0b0,
+            p_RX_BIAS_CFG0                 = 0b0001010101010100,
             p_RX_BUFFER_CFG                = 0b000000,
             p_RX_CAPFF_SARC_ENB            = 0b0,
             p_RX_CLK25_DIV                 = 3,
             p_RX_CLKMUX_EN                 = 0b1,
             p_RX_CLK_SLIP_OVRD             = 0b00000,
             p_RX_CM_BUF_CFG                = 0b1010,
             p_RX_CM_BUF_PD                 = 0b0,
+            p_RX_CM_SEL                    = 3,
+            p_RX_CM_TRIM                   = 10,
+            p_RX_CTLE3_LPF                 = 0b11111111,
             p_RX_DDI_SEL                   = 0b000000,
             p_RX_DEFER_RESET_BUF_EN        = "TRUE",
+            p_RX_DEGEN_CTRL                = 0b011,
+            p_RX_DFELPM_CFG0               = 6,
+            p_RX_DFELPM_CFG1               = 0b1,
             p_RX_DFELPM_KLKH_AGC_STUP_EN   = 0b1,
+            p_RX_DFE_AGC_CFG0              = 0b10,
+            p_RX_DFE_AGC_CFG1              = 4,
+            p_RX_DFE_KL_LPM_KH_CFG0        = 1,
+            p_RX_DFE_KL_LPM_KH_CFG1        = 4,
+            p_RX_DFE_KL_LPM_KL_CFG0        = 0b01,
+            p_RX_DFE_KL_LPM_KL_CFG1        = 4,
             p_RX_DFE_LPM_HOLD_DURING_EIDLE = 0b0,
             p_RX_DISPERR_SEQ_MATCH         = "TRUE",
+            p_RX_DIV2_MODE_B               = 0b0,
             p_RX_DIVRESET_TIME             = 0b00001,
+            p_RX_EN_CTLE_RCAL_B            = 0b0,
             p_RX_EN_HI_LR                  = 0b1,
+            p_RX_EXT_RL_CTRL               = 0b000000000,
             p_RX_EYESCAN_VS_CODE           = 0b0000000,
             p_RX_EYESCAN_VS_NEG_DIR        = 0b0,
             p_RX_EYESCAN_VS_RANGE          = 0b00,
             p_RX_EYESCAN_VS_UT_SIGN        = 0b0,
             p_RX_FABINT_USRCLK_FLOP        = 0b0,
             p_RX_PMA_POWER_SAVE            = 0b0,
+            p_RX_PMA_RSV0                  = 0b0000000000000000,
             p_RX_PROGDIV_CFG               = 0,
+            p_RX_PROGDIV_RATE              = 0b0000000000000001,
+            p_RX_RESLOAD_CTRL              = 0b0000,
+            p_RX_RESLOAD_OVRD              = 0b0,
             p_RX_SAMPLE_PERIOD             = 0b111,
             p_RX_SIG_VALID_DLY             = 11,
             p_RX_SUM_DFETAPREP_EN          = 0b0,
+            p_RX_SUM_IREF_TUNE             = 0b1001,
+            p_RX_SUM_RESLOAD_CTRL          = 0b0011,
+            p_RX_SUM_VCMTUNE               = 0b1010,
             p_RX_SUM_VCM_OVWR              = 0b0,
+            p_RX_SUM_VREF_TUNE             = 0b100,
+            p_RX_TUNE_AFE_OS               = 0b00,
+            p_RX_VREG_CTRL                 = 0b101,
+            p_RX_VREG_PDB                  = 0b1,
+            p_RX_WIDEMODE_CDR              = 0b01,
+            p_RX_WIDEMODE_CDR_GEN3         = 0b00,
+            p_RX_WIDEMODE_CDR_GEN4         = 0b01,
+            p_RX_XMODE_SEL                 = 0b0,
+            p_SAMPLE_CLK_PHASE             = 0b0,
+            p_SAS_12G_MODE                 = 0b0,
+            p_SATA_BURST_SEQ_LEN           = 0b1111,
             p_SATA_CPLL_CFG                = "VCO_3000MHZ",
             p_SHOW_REALIGN_COMMA           = "TRUE",
+            p_SIM_DEVICE                   = "ULTRASCALE_PLUS",
+            p_SIM_MODE                     = "FAST",
             p_SIM_RECEIVER_DETECT_PASS     = "TRUE",
             p_SIM_RESET_SPEEDUP            = "TRUE",
+            p_SIM_TX_EIDLE_DRIVE_LEVEL     = "Z",
+            p_SRSTMODE                     = 0b0,
             p_TAPDLY_SET_TX                = 0b00,
+            p_TEMPERATURE_PAR              = 0b0010,
+            p_TERM_RCAL_CFG                = 0b100001000010001,
             p_TERM_RCAL_OVRD               = 0b000,
             p_TRANS_TIME_RATE              = 0b00001110,
             p_TST_RSV0                     = 0b00000000,
             p_TST_RSV1                     = 0b00000000,
             p_TXBUF_RESET_ON_RATE_CHANGE   = "TRUE",
+            p_TXDLY_CFG                    = 0b1000000000010000,
+            p_TXDLY_LCFG                   = 0b0000000000110000,
             p_TXDRVBIAS_N                  = 0b1010,
             p_TXFIFO_ADDR_CFG              = "LOW",
             p_TXGBOX_FIFO_INIT_RD_ADDR     = 4,
             p_TXGEARBOX_EN                 = "FALSE",
             p_TXPCSRESET_TIME              = 0b00011,
+            p_TXPHDLY_CFG0                 = 0b0110000001110000,
+            p_TXPHDLY_CFG1                 = 0b0000000000001110,
+            p_TXPH_CFG                     = 0b0000001100100011,
+            p_TXPH_CFG2                    = 0b0000000000000000,
             p_TXPH_MONITOR_SEL             = 0b00000,
+            p_TXPI_CFG                     = 0b0000000001010100,
+            p_TXPI_CFG0                    = 0b00,
+            p_TXPI_CFG1                    = 0b00,
+            p_TXPI_CFG2                    = 0b00,
+            p_TXPI_CFG3                    = 0b0,
+            p_TXPI_CFG4                    = 0b0,
+            p_TXPI_CFG5                    = 0b000,
             p_TXPI_GRAY_SEL                = 0b0,
+            p_TXPI_INVSTROBE_SEL           = 0b0,
             p_TXPI_LPM                     = 0b0,
+            p_TXPI_PPM                     = 0b0,
             p_TXPI_PPMCLK_SEL              = "TXUSRCLK2",
             p_TXPI_PPM_CFG                 = 0b00000000,
             p_TXPI_SYNFREQ_PPM             = 0b001,
             p_TXPI_VREFSEL                 = 0b0,
             p_TXPMARESET_TIME              = 0b00011,
+            p_TXREFCLKDIV2_SEL             = 0b0,
             p_TXSYNC_MULTILANE             = 0b0,
             p_TXSYNC_OVRD                  = 0b0,
             p_TXSYNC_SKIP_DA               = 0b0,
             p_TX_CLK25_DIV                 = 3,
             p_TX_CLKMUX_EN                 = 0b1,
+            p_TX_DCC_LOOP_RST_CFG          = 0b0000000000000100,
             p_TX_DEEMPH0                   = 0b000000,
             p_TX_DEEMPH1                   = 0b000000,
+            p_TX_DEEMPH2                   = 0b000000,
+            p_TX_DEEMPH3                   = 0b000000,
             p_TX_DIVRESET_TIME             = 0b00001,
             p_TX_DRIVE_MODE                = "DIRECT",
+            p_TX_DRVMUX_CTRL               = 2,
             p_TX_EIDLE_ASSERT_DELAY        = 0b100,
             p_TX_EIDLE_DEASSERT_DELAY      = 0b011,
             p_TX_FABINT_USRCLK_FLOP        = 0b0,
+            p_TX_FIFO_BYP_EN               = 0b0,
             p_TX_IDLE_DATA_ZERO            = 0b0,
             p_TX_LOOPBACK_DRIVE_HIZ        = "FALSE",
             p_TX_MAINCURSOR_SEL            = 0b0,
+            p_TX_MARGIN_FULL_0             = 0b1011111,
+            p_TX_MARGIN_FULL_1             = 0b1011110,
+            p_TX_MARGIN_FULL_2             = 0b1011100,
+            p_TX_MARGIN_FULL_3             = 0b1011010,
+            p_TX_MARGIN_FULL_4             = 0b1011000,
             p_TX_MARGIN_LOW_0              = 0b1000110,
             p_TX_MARGIN_LOW_1              = 0b1000101,
             p_TX_MARGIN_LOW_2              = 0b1000011,
             p_TX_MARGIN_LOW_3              = 0b1000010,
             p_TX_MARGIN_LOW_4              = 0b1000000,
+            p_TX_PHICAL_CFG0               = 0b0000000000000000,
+            p_TX_PHICAL_CFG1               = 0b0111111000000000,
+            p_TX_PHICAL_CFG2               = 0b0000001000000001,
+            p_TX_PI_BIASSET                = 1,
+            p_TX_PI_IBIAS_MID              = 0b00,
             p_TX_PMADATA_OPT               = 0b0,
             p_TX_PMA_POWER_SAVE            = 0b0,
+            p_TX_PMA_RSV0                  = 0b0000000000001000,
+            p_TX_PREDRV_CTRL               = 2,
             p_TX_PROGCLK_SEL               = "PREPI",
             p_TX_PROGDIV_CFG               = 0,
+            p_TX_PROGDIV_RATE              = 0b0000000000000001,
             p_TX_QPI_STATUS_EN             = 0b0,
             p_TX_RXDETECT_CFG              = 0b00000000110010,
+            p_TX_RXDETECT_REF              = 4,
             p_TX_SAMPLE_PERIOD             = 0b111,
             p_TX_SARC_LPBK_ENB             = 0b0,
+            p_TX_SW_MEAS                   = 0b00,
+            p_TX_VREG_CTRL                 = 0b000,
+            p_TX_VREG_PDB                  = 0b0,
+            p_TX_VREG_VREFSEL              = 0b00,
+            p_USB_BOTH_BURST_IDLE          = 0b0,
+            p_USB_BURSTMAX_U3WAKE          = 0b1111111,
+            p_USB_BURSTMIN_U3WAKE          = 0b1100011,
+            p_USB_CLK_COR_EQ_EN            = 0b0,
+            p_USB_EXT_CNTL                 = 0b1,
+            p_USB_IDLEMAX_POLLING          = 0b1010111011,
+            p_USB_IDLEMIN_POLLING          = 0b0100101011,
+            p_USB_LFPSPING_BURST           = 0b000000101,
+            p_USB_LFPSPOLLING_BURST        = 0b000110001,
+            p_USB_LFPSPOLLING_IDLE_MS      = 0b000000100,
+            p_USB_LFPSU1EXIT_BURST         = 0b000011101,
+            p_USB_LFPSU2LPEXIT_BURST_MS    = 0b001100011,
+            p_USB_LFPSU3WAKE_BURST_MS      = 0b111110011,
+            p_USB_LFPS_TPERIOD             = 0b0011,
+            p_USB_LFPS_TPERIOD_ACCURATE    = 0b1,
+            p_USB_MODE                     = 0b0,
+            p_USB_PCIE_ERR_REP_DIS         = 0b0,
+            p_USB_PING_SATA_MAX_INIT       = 21,
+            p_USB_PING_SATA_MIN_INIT       = 12,
+            p_USB_POLL_SATA_MAX_BURST      = 8,
+            p_USB_POLL_SATA_MIN_BURST      = 4,
+            p_USB_RAW_ELEC                 = 0b0,
+            p_USB_RXIDLE_P0_CTRL           = 0b1,
+            p_USB_TXIDLE_TUNE_ENABLE       = 0b1,
+            p_USB_U1_SATA_MAX_WAKE         = 7,
+            p_USB_U1_SATA_MIN_WAKE         = 4,
+            p_USB_U2_SAS_MAX_COM           = 64,
+            p_USB_U2_SAS_MIN_COM           = 36,
             p_USE_PCS_CLK_PHASE_SEL        = 0b0,
+            p_Y_ALL_MODE                   = 0b0,
         )
 
         self.gth_params.update(
             p_CLK_COR_MAX_LAT              = 12 if rx_buffer_enable else 20,
             p_CLK_COR_MIN_LAT              = 8 if rx_buffer_enable else 18,
             p_CPLL_FBDIV                   = 1 if (use_qpll0 | use_qpll1) else pll.config["n2"],
             p_CPLL_FBDIV_45                = 4 if (use_qpll0 | use_qpll1) else pll.config["n1"],
@@ -711,22 +927,34 @@
         )
 
         self.gth_params.update(
             # Reset modes
             i_RESETOVRD       = 0,
 
             # DRP
+            i_DRPRST          = 0,
             i_DRPADDR         = drp_mux.addr,
             i_DRPCLK          = drp_mux.clk,
             i_DRPDI           = drp_mux.di,
             o_DRPDO           = drp_mux.do,
             i_DRPEN           = drp_mux.en,
             o_DRPRDY          = drp_mux.rdy,
             i_DRPWE           = drp_mux.we,
 
+            # CDR
+            i_INCPCTRL        = 0,
+            i_CDRSTEPDIR      = 0,
+            i_CDRSTEPSQ       = 0,
+            i_CDRSTEPSX       = 0,
+
+            # PCIe related
+            i_CPLLFREQLOCK    = 0,
+            i_QPLL0FREQLOCK   = 0,
+            i_QPLL1FREQLOCK   = 0,
+
             # CPLL
             i_CPLLRESET       = 0,
             i_CPLLPD          = 0 if (use_qpll0 | use_qpll1) else pll.reset,
             o_CPLLLOCK        = Signal() if (use_qpll0 | use_qpll1) else pll.lock,
             i_CPLLLOCKEN      = 1,
             i_CPLLREFCLKSEL   = 0b001,
             i_TSTIN           = 2**20-1,
@@ -741,16 +969,19 @@
             # TX clock
             o_TXOUTCLK        = self.txoutclk,
             i_TXSYSCLKSEL     = 0b00 if use_cpll else 0b10 if use_qpll0 else 0b11,
             i_TXPLLCLKSEL     = 0b00 if use_cpll else 0b11 if use_qpll0 else 0b10,
             i_TXOUTCLKSEL     = 0b010 if tx_buffer_enable else 0b011,
 
             # TX Startup/Reset
+            i_GTTXRESETSEL    = 0,
             i_GTTXRESET       = tx_init.gtXxreset,
             o_TXRESETDONE     = tx_init.Xxresetdone,
+            i_TXDCCFORCESTART = 0,
+            i_TXDCCRESET      = 0,
             i_TXDLYSRESET     = tx_init.Xxdlysreset,
             o_TXDLYSRESETDONE = tx_init.Xxdlysresetdone,
             o_TXPHALIGNDONE   = tx_init.Xxphaligndone,
             i_TXUSERRDY       = tx_init.Xxuserrdy,
             i_TXSYNCMODE      = 1,
             i_TXDLYBYPASS     = 1 if tx_buffer_enable else 0,
             i_TXPHDLYPD       = 1 if tx_buffer_enable else 0,
@@ -767,15 +998,18 @@
             i_TXDIFFCTRL      = 0b1100,
             i_TXINHIBIT       = self.tx_inhibit,
 
             # Internal Loopback
             i_LOOPBACK        = self.loopback,
 
             # RX Startup/Reset
+            i_GTRXRESETSEL    = 0,
             i_GTRXRESET       = rx_init.gtXxreset,
+            i_RXCKCALRESET    = 0,
+            i_RXCKCALSTART    = 0,
             o_RXRESETDONE     = rx_init.Xxresetdone,
             i_RXDLYSRESET     = rx_init.Xxdlysreset,
             o_RXPHALIGNDONE   = rxphaligndone,
             i_RXSYNCALLIN     = rxphaligndone,
             i_RXUSERRDY       = rx_init.Xxuserrdy,
             i_RXSYNCIN        = 0,
             i_RXSYNCMODE      = 1,
@@ -783,32 +1017,44 @@
             i_RXDLYBYPASS     = 1 if rx_buffer_enable else 0,
             i_RXPHDLYPD       = 1 if rx_buffer_enable else 0,
 
             # RX AFE
             i_RXDFEAGCCTRL    = 1,
             i_RXDFEXYDEN      = 1,
             i_RXLPMEN         = 1,
+            i_RXTERMINATION   = 0,
+
+            # RX Equalizer
+            i_FREQOS          = 0,
+            i_RXDFECFOKFCNUM  = 0xD,
+            i_RXDFECFOKFEN    = 0,
+            i_RXDFECFOKFPULSE = 0,
+            i_RXDFECFOKHOLD   = 0,
+            i_RXDFECFOKOVREN  = 0,
+            i_RXDFEKHHOLD     = 0,
+            i_RXDFEKHOVRDEN   = 0,
+            i_RXAFECFOKEN     = 1,
 
             # RX clock
             i_RXRATE          = 0,
             i_RXSYSCLKSEL     = 0b00,
             i_RXOUTCLKSEL     = 0b010,
             i_RXPLLCLKSEL     = 0b00 if use_cpll else 0b11 if use_qpll0 else 0b10,
             o_RXOUTCLK        = self.rxoutclk,
             i_RXUSRCLK        = ClockSignal("rx"),
             i_RXUSRCLK2       = ClockSignal("rx"),
 
             # RX Byte and Word Alignment Ports
-            o_RXBYTEISALIGNED      = Open(),
-            o_RXBYTEREALIGN        = Open(),
-            o_RXCOMMADET           = Open(),
-            i_RXCOMMADETEN         = 1,
-            i_RXMCOMMAALIGNEN      = (~clock_aligner & self.rx_align & (rx_prbs_config == 0b00)) if rx_buffer_enable else 0,
-            i_RXPCOMMAALIGNEN      = (~clock_aligner & self.rx_align & (rx_prbs_config == 0b00)) if rx_buffer_enable else 0,
-            i_RXSLIDE              = 0,
+            o_RXBYTEISALIGNED = Open(),
+            o_RXBYTEREALIGN   = Open(),
+            o_RXCOMMADET      = Open(),
+            i_RXCOMMADETEN    = 1,
+            i_RXMCOMMAALIGNEN = (~clock_aligner & self.rx_align & (rx_prbs_config == 0b00)) if rx_buffer_enable else 0,
+            i_RXPCOMMAALIGNEN = (~clock_aligner & self.rx_align & (rx_prbs_config == 0b00)) if rx_buffer_enable else 0,
+            i_RXSLIDE         = 0,
 
             # RX data
             o_RXCTRL0         = Cat(*[rxdata[10*i+8] for i in range(nwords)]),
             o_RXCTRL1         = Cat(*[rxdata[10*i+9] for i in range(nwords)]),
             o_RXDATA          = Cat(*[rxdata[10*i:10*i+8] for i in range(nwords)]),
 
             # RX electrical
@@ -826,66 +1072,87 @@
             o_GTHTXN          = tx_pads.n
         )
 
         # TX clocking ------------------------------------------------------------------------------
         tx_reset_deglitched = Signal()
         tx_reset_deglitched.attr.add("no_retiming")
         self.sync += tx_reset_deglitched.eq(~tx_init.done)
-        self.clock_domains.cd_tx = ClockDomain()
-        if not tx_buffer_enable:
-            tx_bufg_div = pll.config["clkin"]/self.tx_clk_freq
+        self.cd_tx = ClockDomain()
+
+        # Use/generate local tx_clk.
+        # --------------------------
+        if tx_clk is None:
+            if not tx_buffer_enable:
+                tx_bufg_div = pll.config["clkin"]/self.tx_clk_freq
+            else:
+                tx_bufg_div = 1
+            assert tx_bufg_div == int(tx_bufg_div)
+            self.specials += [
+                Instance("BUFG_GT", i_I=self.txoutclk, o_O=self.cd_tx.clk,
+                    i_DIV=int(tx_bufg_div)-1),
+                AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+            ]
+
+        # Use provided/shared tx_clk.
+        # ---------------------------
         else:
-            tx_bufg_div = 1
-        assert tx_bufg_div == int(tx_bufg_div)
-        self.specials += [
-            Instance("BUFG_GT", i_I=self.txoutclk, o_O=self.cd_tx.clk,
-                i_DIV=int(tx_bufg_div)-1),
-            AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-        ]
+            assert tx_buffer_enable
+            self.cd_tx.clk = tx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
 
         # RX clocking ------------------------------------------------------------------------------
         rx_reset_deglitched = Signal()
         rx_reset_deglitched.attr.add("no_retiming")
         self.sync.tx += rx_reset_deglitched.eq(~rx_init.done)
-        self.clock_domains.cd_rx = ClockDomain()
-        self.specials += [
-            Instance("BUFG_GT", i_I=self.rxoutclk, o_O=self.cd_rx.clk),
-            AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
-        ]
+        self.cd_rx = ClockDomain()
+
+        # Use/generate local rx_clk.
+        # --------------------------
+        if rx_clk is None:
+            self.specials += [
+                Instance("BUFG_GT", i_I=self.rxoutclk, o_O=self.cd_rx.clk),
+                AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
+            ]
+        # Use provided/shared rx_clk.
+        # ---------------------------
+        else:
+            assert rx_buffer_enable
+            self.cd_rx.clk = rx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
 
         # TX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
+        self.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
         self.comb += self.tx_prbs.config.eq(tx_prbs_config)
         self.comb += [
             self.tx_prbs.i.eq(Cat(*[self.encoder.output[i] for i in range(nwords)])),
             If(tx_produce_square_wave,
                 # square wave @ linerate/data_width for scope observation
                 txdata.eq(Signal(data_width, reset=(1<<(data_width//2))-1))
             ).Elif(tx_produce_pattern,
                 txdata.eq(tx_pattern)
             ).Else(
                 txdata.eq(self.tx_prbs.o)
             )
         ]
 
         # RX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
+        self.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
         self.comb += [
             self.rx_prbs.config.eq(rx_prbs_config),
             self.rx_prbs.pause.eq(rx_prbs_pause),
             rx_prbs_errors.eq(self.rx_prbs.errors)
         ]
         for i in range(nwords):
             self.comb += self.decoders[i].input.eq(rxdata[10*i:10*(i+1)])
         self.sync.rx += self.rx_prbs.i.eq(rxdata)
 
         # Clock Aligner ----------------------------------------------------------------------------
         if clock_aligner:
             clock_aligner = BruteforceClockAligner(clock_aligner_comma, self.tx_clk_freq)
-            self.submodules.clock_aligner = clock_aligner
+            self.clock_aligner = clock_aligner
             ps_restart = PulseSynchronizer("tx", "sys")
             self.submodules += ps_restart
             self.comb += [
                 clock_aligner.rxdata.eq(rxdata),
                 ps_restart.i.eq(clock_aligner.restart),
                 rx_init.restart.eq((ps_restart.o & self.rx_align) | ~self.rx_enable),
                 self.rx_ready.eq(clock_aligner.ready)
@@ -1045,579 +1312,8 @@
 
         self.sync += If(self.clock_latch.re,
             self.clock_tx_cycles.storage.eq(tx_cycles),
             self.clock_rx_cycles.storage.eq(rx_cycles),
         )
 
     def do_finalize(self):
-        self.specials += Instance(self.name, **self.gth_params)
-
-
-class GTH3(GTHBase):
-    name = "GTHE3_CHANNEL"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Ultrascale only params
-        self.gth_params.update(
-            p_ADAPT_CFG0                   = 0b1111100000000000,
-            p_ADAPT_CFG1                   = 0b0000000000000000,
-            p_CPLL_CFG0                    = 0b0110011111111000,
-            p_CPLL_CFG1                    = 0b1010010010101100,
-            p_CPLL_CFG2                    = 0b0101000000000111,
-            p_CPLL_CFG3                    = 0b000000,
-            p_CPLL_INIT_CFG1               = 0b00000000,
-            p_DFE_D_X_REL_POS              = 0b0,
-            p_DFE_VCM_COMP_EN              = 0b0,
-            p_ES_PMA_CFG                   = 0b0000000000,
-            p_EVODD_PHI_CFG                = 0b00000000000,
-            p_GM_BIAS_SELECT               = 0b0,
-            p_PCIE_BUFG_DIV_CTRL           = 0b0001000000000000,
-            p_PCIE_RXPCS_CFG_GEN3          = 0b0000001010100100,
-            p_PCIE_RXPMA_CFG               = 0b0000000000001010,
-            p_PCIE_TXPMA_CFG               = 0b0000000000001010,
-            p_PCS_RSVD1                    = 0b000,
-            p_PLL_SEL_MODE_GEN12           = 0b11,
-            p_PLL_SEL_MODE_GEN3            = 0b11,
-            p_PMA_RSV1                     = 0b1111000000000000,
-            p_RXCDR_CFG0                   = 0b0000000000000000,
-            p_RXCDR_CFG0_GEN3              = 0b0000000000000000,
-            p_RXCDR_CFG1                   = 0b0000000000000000,
-            p_RXCDR_CFG1_GEN3              = 0b0000000000000000,
-            p_RXCDR_CFG2                   = 0b0000011111100110,
-            p_RXCDR_CFG2_GEN3              = 0b0000011111100110,
-            p_RXCDR_CFG3                   = 0b0000000000000000,
-            p_RXCDR_CFG3_GEN3              = 0b0000000000000000,
-            p_RXCDR_CFG4                   = 0b0000000000000000,
-            p_RXCDR_CFG4_GEN3              = 0b0000000000000000,
-            p_RXCDR_CFG5                   = 0b0000000000000000,
-            p_RXCDR_CFG5_GEN3              = 0b0000000000000000,
-            p_RXCDR_LOCK_CFG0              = 0b0100010010000000,
-            p_RXCDR_LOCK_CFG1              = 0b0101111111111111,
-            p_RXCDR_LOCK_CFG2              = 0b0111011111000011,
-            p_RXCFOK_CFG0                  = 0b0100000000000000,
-            p_RXCFOK_CFG1                  = 0b0000000001100101,
-            p_RXCFOK_CFG2                  = 0b0000000000101110,
-            p_RXDFELPM_KL_CFG0             = 0b0000000000000000,
-            p_RXDFELPM_KL_CFG1             = 0b0000000000000010,
-            p_RXDFELPM_KL_CFG2             = 0b0000000000000000,
-            p_RXDFE_GC_CFG0                = 0b0000000000000000,
-            p_RXDFE_GC_CFG1                = 0b0111100001110000,
-            p_RXDFE_GC_CFG2                = 0b0000000000000000,
-            p_RXDFE_H2_CFG0                = 0b0000000000000000,
-            p_RXDFE_H2_CFG1                = 0b0000000000000000,
-            p_RXDFE_H3_CFG0                = 0b0100000000000000,
-            p_RXDFE_H3_CFG1                = 0b0000000000000000,
-            p_RXDFE_H4_CFG0                = 0b0010000000000000,
-            p_RXDFE_H4_CFG1                = 0b0000000000000011,
-            p_RXDFE_H5_CFG0                = 0b0010000000000000,
-            p_RXDFE_H5_CFG1                = 0b0000000000000011,
-            p_RXDFE_H6_CFG0                = 0b0010000000000000,
-            p_RXDFE_H6_CFG1                = 0b0000000000000000,
-            p_RXDFE_H7_CFG0                = 0b0010000000000000,
-            p_RXDFE_H7_CFG1                = 0b0000000000000000,
-            p_RXDFE_H8_CFG0                = 0b0010000000000000,
-            p_RXDFE_H8_CFG1                = 0b0000000000000000,
-            p_RXDFE_H9_CFG0                = 0b0010000000000000,
-            p_RXDFE_H9_CFG1                = 0b0000000000000000,
-            p_RXDFE_HA_CFG0                = 0b0010000000000000,
-            p_RXDFE_HA_CFG1                = 0b0000000000000000,
-            p_RXDFE_HB_CFG0                = 0b0010000000000000,
-            p_RXDFE_HB_CFG1                = 0b0000000000000000,
-            p_RXDFE_HC_CFG0                = 0b0000000000000000,
-            p_RXDFE_HC_CFG1                = 0b0000000000000000,
-            p_RXDFE_HD_CFG0                = 0b0000000000000000,
-            p_RXDFE_HD_CFG1                = 0b0000000000000000,
-            p_RXDFE_HE_CFG0                = 0b0000000000000000,
-            p_RXDFE_HE_CFG1                = 0b0000000000000000,
-            p_RXDFE_HF_CFG0                = 0b0000000000000000,
-            p_RXDFE_HF_CFG1                = 0b0000000000000000,
-            p_RXDFE_OS_CFG0                = 0b1000000000000000,
-            p_RXDFE_OS_CFG1                = 0b0000000000000000,
-            p_RXDFE_UT_CFG0                = 0b1000000000000000,
-            p_RXDFE_UT_CFG1                = 0b0000000000000011,
-            p_RXDFE_VP_CFG0                = 0b1010101000000000,
-            p_RXDFE_VP_CFG1                = 0b0000000000110011,
-            p_RXDLY_CFG                    = 0b0000000000011111,
-            p_RXELECIDLE_CFG               = "SIGCFG_4",
-            p_RXLPM_GC_CFG                 = 0b0001000000000000,
-            p_RXLPM_OS_CFG0                = 0b1000000000000000,
-            p_RXLPM_OS_CFG1                = 0b0000000000000010,
-            p_RXPHDLY_CFG                  = 0b0010000000100000,
-            p_RXPHSLIP_CFG                 = 0b0110011000100010,
-            p_RXPI_CFG0                    = 0b00,
-            p_RXPI_CFG1                    = 0b00,
-            p_RXPI_CFG2                    = 0b00,
-            p_RXPI_CFG3                    = 0b00,
-            p_RXPI_CFG4                    = 0b0,
-            p_RXPI_CFG5                    = 0b1,
-            p_RXPI_CFG6                    = 0b000,
-            p_RX_BIAS_CFG0                 = 0b0000101010110100,
-            p_RX_CM_SEL                    = 0b11,
-            p_RX_CM_TRIM                   = 0b1010,
-            p_RX_CTLE3_LPF                 = 0b00000001,
-            p_RX_DFELPM_CFG0               = 0b0110,
-            p_RX_DFELPM_CFG1               = 0b1,
-            p_RX_DFE_AGC_CFG0              = 0b10,
-            p_RX_DFE_AGC_CFG1              = 0b100,
-            p_RX_DFE_KL_LPM_KH_CFG0        = 0b01,
-            p_RX_DFE_KL_LPM_KH_CFG1        = 0b100,
-            p_RX_DFE_KL_LPM_KL_CFG0        = 0b01,
-            p_RX_DFE_KL_LPM_KL_CFG1        = 0b100,
-            p_RX_SUM_IREF_TUNE             = 0b0000,
-            p_RX_SUM_RES_CTRL              = 0b00,
-            p_RX_SUM_VCMTUNE               = 0b0000,
-            p_RX_SUM_VREF_TUNE             = 0b000,
-            p_RX_TUNE_AFE_OS               = 0b10,
-            p_RX_WIDEMODE_CDR              = 0b1,
-            p_SAS_MAX_COM                  = 64,
-            p_SAS_MIN_COM                  = 36,
-            p_SATA_BURST_SEQ_LEN           = 0b1110,
-            p_SATA_MAX_BURST               = 8,
-            p_SATA_MAX_INIT                = 21,
-            p_SATA_MAX_WAKE                = 7,
-            p_SATA_MIN_BURST               = 4,
-            p_SATA_MIN_INIT                = 12,
-            p_SATA_MIN_WAKE                = 4,
-            p_SIM_TX_EIDLE_DRIVE_LEVEL     = 0b0,
-            p_SIM_VERSION                  = 2,
-            p_TEMPERATUR_PAR               = 0b0010,
-            p_TERM_RCAL_CFG                = 0b100001000010000,
-            p_TXDLY_CFG                    = 0b0000000000001001,
-            p_TXDLY_LCFG                   = 0b0000000001010000,
-            p_TXDRVBIAS_P                  = 0b1010,
-            p_TXPHDLY_CFG0                 = 0b0010000000100000,
-            p_TXPHDLY_CFG1                 = 0b0000000001110101,
-            p_TXPH_CFG                     = 0b0000100110000000,
-            p_TXPI_CFG0                    = 0b00,
-            p_TXPI_CFG1                    = 0b00,
-            p_TXPI_CFG2                    = 0b00,
-            p_TXPI_CFG3                    = 0b1,
-            p_TXPI_CFG4                    = 0b1,
-            p_TXPI_CFG5                    = 0b000,
-            p_TXPI_INVSTROBE_SEL           = 0b1,
-            p_TX_DCD_CFG                   = 0b000010,
-            p_TX_DCD_EN                    = 0b0,
-            p_TX_EML_PHI_TUNE              = 0b0,
-            p_TX_MARGIN_FULL_0             = 0b1001111,
-            p_TX_MARGIN_FULL_1             = 0b1001110,
-            p_TX_MARGIN_FULL_2             = 0b1001100,
-            p_TX_MARGIN_FULL_3             = 0b1001010,
-            p_TX_MARGIN_FULL_4             = 0b1001000,
-            p_TX_MODE_SEL                  = 0b000,
-            p_TX_RXDETECT_REF              = 0b100,
-            p_WB_MODE                      = 0b00,
-        )
-
-        # Ultrascale only ports
-        self.gth_params.update(
-            # Reset modes
-            i_GTRESETSEL      = 0,
-
-            # RX AFE
-            i_RXOSINTCFG      = 0xd,
-            i_RXOSINTEN       = 1,
-
-            # TX Electrical
-            i_TXBUFDIFFCTRL   = 0b000,
-        )
-
-        # Full list of Ultrascale only ports
-            # EVODDPHICALDONE
-            # EVODDPHICALSTART
-            # EVODDPHIDRDEN
-            # EVODDPHIDWREN
-            # EVODDPHIXRDEN
-            # EVODDPHIXWREN
-            # EYESCANMODE
-            # GTRESETSEL
-            # LPBKRXTXSEREN
-            # LPBKTXRXSEREN
-            # PCSRSVDIN2
-            # PMARSVDIN
-            # RSTCLKENTX
-            # RXCDRRESETRSV
-            # RXDFEVSEN
-            # RXOSINTCFG
-            # RXOSINTEN
-            # RXOSINTHOLD
-            # RXOSINTOVRDEN
-            # RXOSINTSTROBE
-            # RXOSINTTESTOVRDEN
-            # TXBUFDIFFCTRL
-            # TXDIFFPD
-            # TXPOSTCURSORINV
-            # TXPRECURSORINV
-            # TXQPISTRONGPDOWN
-
-    def add_electrical_control(self):
-        super().add_electrical_control()
-
-        self._tx_postcursor_inv = CSRStorage(1, reset=0b0,     description="TX Post Cursor Polarity, see UG576.")
-        self._tx_precursor_inv  = CSRStorage(1, reset=0b0,     description="Invert polarity of TX Pre Cursor, see UG576.")
-        self.gth_params.update(
-            i_TXPOSTCURSORINV = self._tx_postcursor_inv.storage,
-            i_TXPRECURSORINV  = self._tx_precursor_inv.storage,
-        )
-
-
-class GTH4(GTHBase):
-    name = "GTHE4_CHANNEL"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Ultrascale+ only params 1/2
-        self.gth_params.update(
-            p_ADAPT_CFG0                   = 0b0001000000000000,
-            p_ADAPT_CFG1                   = 0b1100100000000000,
-            p_ADAPT_CFG2                   = 0b0000000000000000,
-            p_A_RXTERMINATION              = 0b1,
-            p_A_TXDIFFCTRL                 = 0b01100,
-            p_CAPBYPASS_FORCE              = 0b0,
-            p_CFOK_PWRSVE_EN               = 0b1,
-            p_CH_HSPMUX                    = 0b0010010000100100,
-            p_CKCAL1_CFG_0                 = 0b1100000011000000,
-            p_CKCAL1_CFG_1                 = 0b0101000011000000,
-            p_CKCAL1_CFG_2                 = 0b0000000000001010,
-            p_CKCAL1_CFG_3                 = 0b0000000000000000,
-            p_CKCAL2_CFG_0                 = 0b1100000011000000,
-            p_CKCAL2_CFG_1                 = 0b1000000011000000,
-            p_CKCAL2_CFG_2                 = 0b0000000000000000,
-            p_CKCAL2_CFG_3                 = 0b0000000000000000,
-            p_CKCAL2_CFG_4                 = 0b0000000000000000,
-            p_CKCAL_RSVD0                  = 0b0000000010000000,
-            p_CKCAL_RSVD1                  = 0b0000010000000000,
-            p_CPLL_CFG0                    = 0b0000000111111010,
-            p_CPLL_CFG1                    = 0b0000000000100011,
-            p_CPLL_CFG2                    = 0b0000000000000010,
-            p_CPLL_CFG3                    = 0b0000000000000000,
-            p_CTLE3_OCAP_EXT_CTRL          = 0b000,
-            p_CTLE3_OCAP_EXT_EN            = 0b0,
-            p_DELAY_ELEC                   = 0b0,
-            p_ES_QUALIFIER5                = 0b0000000000000000,
-            p_ES_QUALIFIER6                = 0b0000000000000000,
-            p_ES_QUALIFIER7                = 0b0000000000000000,
-            p_ES_QUALIFIER8                = 0b0000000000000000,
-            p_ES_QUALIFIER9                = 0b0000000000000000,
-            p_ES_QUAL_MASK5                = 0b0000000000000000,
-            p_ES_QUAL_MASK6                = 0b0000000000000000,
-            p_ES_QUAL_MASK7                = 0b0000000000000000,
-            p_ES_QUAL_MASK8                = 0b0000000000000000,
-            p_ES_QUAL_MASK9                = 0b0000000000000000,
-            p_ES_SDATA_MASK5               = 0b0000000000000000,
-            p_ES_SDATA_MASK6               = 0b0000000000000000,
-            p_ES_SDATA_MASK7               = 0b0000000000000000,
-            p_ES_SDATA_MASK8               = 0b0000000000000000,
-            p_ES_SDATA_MASK9               = 0b0000000000000000,
-            p_ISCAN_CK_PH_SEL2             = 0b0,
-            p_LPBK_BIAS_CTRL               = 0b100,
-            p_LPBK_EN_RCAL_B               = 0b0,
-            p_LPBK_EXT_RCAL                = 0b1000,
-            p_LPBK_IND_CTRL0               = 0b000,
-            p_LPBK_IND_CTRL1               = 0b000,
-            p_LPBK_IND_CTRL2               = 0b000,
-            p_LPBK_RG_CTRL                 = 0b1110,
-            p_PCIE3_CLK_COR_EMPTY_THRSH    = 0b00000,
-            p_PCIE3_CLK_COR_FULL_THRSH     = 0b010000,
-            p_PCIE3_CLK_COR_MAX_LAT        = 0b00100,
-            p_PCIE3_CLK_COR_MIN_LAT        = 0b00000,
-            p_PCIE3_CLK_COR_THRSH_TIMER    = 0b001000,
-            p_PCIE_BUFG_DIV_CTRL           = 0b0011010100000000,
-            p_PCIE_PLL_SEL_MODE_GEN12      = 0b10,
-            p_PCIE_PLL_SEL_MODE_GEN3       = 0b10,
-            p_PCIE_PLL_SEL_MODE_GEN4       = 0b10,
-            p_PCIE_RXPCS_CFG_GEN3          = 0b0000101010100101,
-            p_PCIE_RXPMA_CFG               = 0b0010100000001010,
-            p_PCIE_TXPMA_CFG               = 0b0010100000001010,
-            p_PREIQ_FREQ_BST               = 0,
-            p_RCLK_SIPO_DLY_ENB            = 0b0,
-            p_RCLK_SIPO_INV_EN             = 0b0,
-            p_RTX_BUF_CML_CTRL             = 0b010,
-            p_RTX_BUF_TERM_CTRL            = 0b00,
-            p_RXCDR_CFG0                   = 0b0000000000000011,
-            p_RXCDR_CFG0_GEN3              = 0b0000000000000011,
-            p_RXCDR_CFG1                   = 0b0000000000000000,
-            p_RXCDR_CFG1_GEN3              = 0b0000000000000000,
-            p_RXCDR_CFG2                   = 0b0000001001101001,
-            p_RXCDR_CFG2_GEN2              = 0b1001101001,
-            p_RXCDR_CFG2_GEN3              = 0b0000001001101001,
-            p_RXCDR_CFG2_GEN4              = 0b0000000101100100,
-            p_RXCDR_CFG3                   = 0b0000000000010000,
-            p_RXCDR_CFG3_GEN2              = 0b010000,
-            p_RXCDR_CFG3_GEN3              = 0b0000000000010000,
-            p_RXCDR_CFG3_GEN4              = 0b0000000000010010,
-            p_RXCDR_CFG4                   = 0b0101110011110110,
-            p_RXCDR_CFG4_GEN3              = 0b0101110011110110,
-            p_RXCDR_CFG5                   = 0b1011010001101011,
-            p_RXCDR_CFG5_GEN3              = 0b0001010001101011,
-            p_RXCDR_LOCK_CFG0              = 0b0010001000000001,
-            p_RXCDR_LOCK_CFG1              = 0b1001111111111111,
-            p_RXCDR_LOCK_CFG2              = 0b0111011111000011,
-            p_RXCDR_LOCK_CFG3              = 0b0000000000000001,
-            p_RXCDR_LOCK_CFG4              = 0b0000000000000000,
-            p_RXCFOK_CFG0                  = 0b0000000000000000,
-            p_RXCFOK_CFG1                  = 0b1000000000010101,
-            p_RXCFOK_CFG2                  = 0b0000001010101110,
-            p_RXCKCAL1_IQ_LOOP_RST_CFG     = 0b0000000000000100,
-            p_RXCKCAL1_I_LOOP_RST_CFG      = 0b0000000000000100,
-            p_RXCKCAL1_Q_LOOP_RST_CFG      = 0b0000000000000100,
-            p_RXCKCAL2_DX_LOOP_RST_CFG     = 0b0000000000000100,
-            p_RXCKCAL2_D_LOOP_RST_CFG      = 0b0000000000000100,
-            p_RXCKCAL2_S_LOOP_RST_CFG      = 0b0000000000000100,
-            p_RXCKCAL2_X_LOOP_RST_CFG      = 0b0000000000000100,
-            p_RXDFELPM_KL_CFG0             = 0b0000000000000000,
-            p_RXDFELPM_KL_CFG1             = 0b1010000011100010,
-            p_RXDFELPM_KL_CFG2             = 0b0000000100000000,
-            p_RXDFE_GC_CFG0                = 0b0000000000000000,
-            p_RXDFE_GC_CFG1                = 0b1000000000000000,
-            p_RXDFE_GC_CFG2                = 0b1111111111100000,
-            p_RXDFE_H2_CFG0                = 0b0000000000000000,
-            p_RXDFE_H2_CFG1                = 0b0000000000000010,
-            p_RXDFE_H3_CFG0                = 0b0000000000000000,
-            p_RXDFE_H3_CFG1                = 0b1000000000000010,
-            p_RXDFE_H4_CFG0                = 0b0000000000000000,
-            p_RXDFE_H4_CFG1                = 0b1000000000000010,
-            p_RXDFE_H5_CFG0                = 0b0000000000000000,
-            p_RXDFE_H5_CFG1                = 0b1000000000000010,
-            p_RXDFE_H6_CFG0                = 0b0000000000000000,
-            p_RXDFE_H6_CFG1                = 0b1000000000000010,
-            p_RXDFE_H7_CFG0                = 0b0000000000000000,
-            p_RXDFE_H7_CFG1                = 0b1000000000000010,
-            p_RXDFE_H8_CFG0                = 0b0000000000000000,
-            p_RXDFE_H8_CFG1                = 0b1000000000000010,
-            p_RXDFE_H9_CFG0                = 0b0000000000000000,
-            p_RXDFE_H9_CFG1                = 0b1000000000000010,
-            p_RXDFE_HA_CFG0                = 0b0000000000000000,
-            p_RXDFE_HA_CFG1                = 0b1000000000000010,
-            p_RXDFE_HB_CFG0                = 0b0000000000000000,
-            p_RXDFE_HB_CFG1                = 0b1000000000000010,
-            p_RXDFE_HC_CFG0                = 0b0000000000000000,
-            p_RXDFE_HC_CFG1                = 0b1000000000000010,
-            p_RXDFE_HD_CFG0                = 0b0000000000000000,
-            p_RXDFE_HD_CFG1                = 0b1000000000000010,
-            p_RXDFE_HE_CFG0                = 0b0000000000000000,
-            p_RXDFE_HE_CFG1                = 0b1000000000000010,
-            p_RXDFE_HF_CFG0                = 0b0000000000000000,
-            p_RXDFE_HF_CFG1                = 0b1000000000000010,
-            p_RXDFE_KH_CFG0                = 0b0000000000000000,
-            p_RXDFE_KH_CFG1                = 0b1000000000000000,
-            p_RXDFE_KH_CFG2                = 0b0010011000010011,
-            p_RXDFE_KH_CFG3                = 0b0100000100011100,
-            p_RXDFE_OS_CFG0                = 0b0000000000000000,
-            p_RXDFE_OS_CFG1                = 0b1000000000000010,
-            p_RXDFE_PWR_SAVING             = 0b1,
-            p_RXDFE_UT_CFG0                = 0b0000000000000000,
-            p_RXDFE_UT_CFG1                = 0b0000000000000011,
-            p_RXDFE_UT_CFG2                = 0b0000000000000000,
-            p_RXDFE_VP_CFG0                = 0b0000000000000000,
-            p_RXDFE_VP_CFG1                = 0b1000000000110011,
-            p_RXDLY_CFG                    = 0b0000000000010000,
-            p_RXELECIDLE_CFG               = "SIGCFG_4",
-            p_RXLPM_GC_CFG                 = 0b1000000000000000,
-            p_RXLPM_OS_CFG0                = 0b0000000000000000,
-            p_RXLPM_OS_CFG1                = 0b1000000000000010,
-            p_RXPHDLY_CFG                  = 0b0010000001110000,
-            p_RXPHSLIP_CFG                 = 0b1001100100110011,
-            p_RXPI_AUTO_BW_SEL_BYPASS      = 0b0,
-            p_RXPI_CFG0                    = 0b0000000000000010,
-            p_RXPI_CFG1                    = 0b0000000000010101,
-            p_RXPI_SEL_LC                  = 0b00,
-            p_RXPI_STARTCODE               = 0b00,
-            p_RXREFCLKDIV2_SEL             = 0b0,
-            p_RX_BIAS_CFG0                 = 0b0001010101010100,
-            p_RX_CM_SEL                    = 3,
-            p_RX_CM_TRIM                   = 10,
-            p_RX_CTLE3_LPF                 = 0b11111111,
-            p_RX_DEGEN_CTRL                = 0b011,
-            p_RX_DFELPM_CFG0               = 6,
-            p_RX_DFELPM_CFG1               = 0b1,
-            p_RX_DFE_AGC_CFG0              = 0b10,
-            p_RX_DFE_AGC_CFG1              = 4,
-            p_RX_DFE_KL_LPM_KH_CFG0        = 1,
-            p_RX_DFE_KL_LPM_KH_CFG1        = 4,
-            p_RX_DFE_KL_LPM_KL_CFG0        = 0b01,
-            p_RX_DFE_KL_LPM_KL_CFG1        = 4,
-            p_RX_DIV2_MODE_B               = 0b0,
-            p_RX_EN_CTLE_RCAL_B            = 0b0,
-            p_RX_EXT_RL_CTRL               = 0b000000000,
-            p_RX_PMA_RSV0                  = 0b0000000000000000,
-            p_RX_PROGDIV_RATE              = 0b0000000000000001,
-            p_RX_RESLOAD_CTRL              = 0b0000,
-            p_RX_RESLOAD_OVRD              = 0b0,
-            p_RX_SUM_IREF_TUNE             = 0b1001,
-            p_RX_SUM_RESLOAD_CTRL          = 0b0011,
-            p_RX_SUM_VCMTUNE               = 0b1010,
-            p_RX_SUM_VREF_TUNE             = 0b100,
-            p_RX_TUNE_AFE_OS               = 0b00,
-            p_RX_VREG_CTRL                 = 0b101,
-            p_RX_VREG_PDB                  = 0b1,
-            p_RX_WIDEMODE_CDR              = 0b01,
-            p_RX_WIDEMODE_CDR_GEN3         = 0b00,
-            p_RX_WIDEMODE_CDR_GEN4         = 0b01,
-            p_RX_XMODE_SEL                 = 0b0,
-            p_SAMPLE_CLK_PHASE             = 0b0,
-            p_SAS_12G_MODE                 = 0b0,
-            p_SATA_BURST_SEQ_LEN           = 0b1111,
-            p_SIM_DEVICE                   = "ULTRASCALE_PLUS",
-            p_SIM_MODE                     = "FAST",
-            p_SIM_TX_EIDLE_DRIVE_LEVEL     = "Z",
-            p_SRSTMODE                     = 0b0,
-            p_TEMPERATURE_PAR              = 0b0010,
-            p_TERM_RCAL_CFG                = 0b100001000010001,
-            p_TXDLY_CFG                    = 0b1000000000010000,
-            p_TXDLY_LCFG                   = 0b0000000000110000,
-            p_TXPHDLY_CFG0                 = 0b0110000001110000,
-            p_TXPHDLY_CFG1                 = 0b0000000000001110,
-            p_TXPH_CFG                     = 0b0000001100100011,
-            p_TXPH_CFG2                    = 0b0000000000000000,
-            p_TXPI_CFG                     = 0b0000000001010100,
-            p_TXPI_CFG0                    = 0b00,
-            p_TXPI_CFG1                    = 0b00,
-            p_TXPI_CFG2                    = 0b00,
-            p_TXPI_CFG3                    = 0b0,
-            p_TXPI_CFG4                    = 0b0,
-            p_TXPI_CFG5                    = 0b000,
-            p_TXPI_INVSTROBE_SEL           = 0b0,
-            p_TXPI_PPM                     = 0b0,
-            p_TXREFCLKDIV2_SEL             = 0b0,
-            p_TX_DCC_LOOP_RST_CFG          = 0b0000000000000100,
-            p_TX_DEEMPH2                   = 0b000000,
-            p_TX_DEEMPH3                   = 0b000000,
-            p_TX_DRVMUX_CTRL               = 2,
-            p_TX_FIFO_BYP_EN               = 0b0,
-            p_TX_MARGIN_FULL_0             = 0b1011111,
-            p_TX_MARGIN_FULL_1             = 0b1011110,
-            p_TX_MARGIN_FULL_2             = 0b1011100,
-            p_TX_MARGIN_FULL_3             = 0b1011010,
-            p_TX_MARGIN_FULL_4             = 0b1011000,
-            p_TX_PHICAL_CFG0               = 0b0000000000000000,
-            p_TX_PHICAL_CFG1               = 0b0111111000000000,
-            p_TX_PHICAL_CFG2               = 0b0000001000000001,
-            p_TX_PI_BIASSET                = 1,
-            p_TX_PI_IBIAS_MID              = 0b00,
-            p_TX_PMA_RSV0                  = 0b0000000000001000,
-            p_TX_PREDRV_CTRL               = 2,
-            p_TX_PROGDIV_RATE              = 0b0000000000000001,
-            p_TX_RXDETECT_REF              = 4,
-            p_TX_SW_MEAS                   = 0b00,
-            p_TX_VREG_CTRL                 = 0b000,
-            p_TX_VREG_PDB                  = 0b0,
-            p_TX_VREG_VREFSEL              = 0b00,
-        )
-
-        # Ultrascale+ only params 2/2
-        self.gth_params.update(
-            p_USB_BOTH_BURST_IDLE          = 0b0,
-            p_USB_BURSTMAX_U3WAKE          = 0b1111111,
-            p_USB_BURSTMIN_U3WAKE          = 0b1100011,
-            p_USB_CLK_COR_EQ_EN            = 0b0,
-            p_USB_EXT_CNTL                 = 0b1,
-            p_USB_IDLEMAX_POLLING          = 0b1010111011,
-            p_USB_IDLEMIN_POLLING          = 0b0100101011,
-            p_USB_LFPSPING_BURST           = 0b000000101,
-            p_USB_LFPSPOLLING_BURST        = 0b000110001,
-            p_USB_LFPSPOLLING_IDLE_MS      = 0b000000100,
-            p_USB_LFPSU1EXIT_BURST         = 0b000011101,
-            p_USB_LFPSU2LPEXIT_BURST_MS    = 0b001100011,
-            p_USB_LFPSU3WAKE_BURST_MS      = 0b111110011,
-            p_USB_LFPS_TPERIOD             = 0b0011,
-            p_USB_LFPS_TPERIOD_ACCURATE    = 0b1,
-            p_USB_MODE                     = 0b0,
-            p_USB_PCIE_ERR_REP_DIS         = 0b0,
-            p_USB_PING_SATA_MAX_INIT       = 21,
-            p_USB_PING_SATA_MIN_INIT       = 12,
-            p_USB_POLL_SATA_MAX_BURST      = 8,
-            p_USB_POLL_SATA_MIN_BURST      = 4,
-            p_USB_RAW_ELEC                 = 0b0,
-            p_USB_RXIDLE_P0_CTRL           = 0b1,
-            p_USB_TXIDLE_TUNE_ENABLE       = 0b1,
-            p_USB_U1_SATA_MAX_WAKE         = 7,
-            p_USB_U1_SATA_MIN_WAKE         = 4,
-            p_USB_U2_SAS_MAX_COM           = 64,
-            p_USB_U2_SAS_MIN_COM           = 36,
-            p_Y_ALL_MODE                   = 0b0,
-        )
-
-        # Ultrascale+ only ports (only inputs mentionned in UG576)
-        self.gth_params.update(
-            # Reset modes
-            i_GTRXRESETSEL      = 0,
-            i_GTTXRESETSEL      = 0,
-
-            # CDR
-            i_INCPCTRL          = 0,
-            i_CDRSTEPDIR        = 0,
-            i_CDRSTEPSQ         = 0,
-            i_CDRSTEPSX         = 0,
-
-            # PCIe related
-            i_CPLLFREQLOCK      = 0,
-            i_QPLL0FREQLOCK     = 0,
-            i_QPLL1FREQLOCK     = 0,
-
-            # DRP
-            i_DRPRST            = 0,
-
-            # RX Startup/Reset
-            i_RXCKCALRESET      = 0,
-            i_RXCKCALSTART      = 0,
-
-            # RX AFE
-            i_RXTERMINATION     = 0,
-
-            # RX Equalizer
-            i_FREQOS            = 0,
-            i_RXDFECFOKFCNUM    = 0xD,
-            i_RXDFECFOKFEN      = 0,
-            i_RXDFECFOKFPULSE   = 0,
-            i_RXDFECFOKHOLD     = 0,
-            i_RXDFECFOKOVREN    = 0,
-            i_RXDFEKHHOLD       = 0,
-            i_RXDFEKHOVRDEN     = 0,
-            i_RXAFECFOKEN       = 1,
-
-            # TX Startup/Reset
-            i_TXDCCFORCESTART   = 0,
-            i_TXDCCRESET        = 0,
-        )
-
-        # Full list of Ultrascale+ only ports
-            # CDRSTEPDIR
-            # CDRSTEPSQ
-            # CDRSTEPSX
-            # CPLLFREQLOCK
-            # DRPRST
-            # FREQOS
-            # GTRXRESETSEL
-            # GTTXRESETSEL
-            # INCPCTRL
-            # QPLL0FREQLOCK
-            # QPLL1FREQLOCK
-            # RXAFECFOKEN
-            # RXCKCALRESET
-            # RXCKCALSTART
-            # RXDFECFOKFCNUM
-            # RXDFECFOKFEN
-            # RXDFECFOKFPULSE
-            # RXDFECFOKHOLD
-            # RXDFECFOKOVREN
-            # RXDFEKHHOLD
-            # RXDFEKHOVRDEN
-            # RXEQTRAINING
-            # RXTERMINATION
-            # TXDCCFORCESTART
-            # TXDCCRESET
-            # TXLFPSTRESET
-            # TXLFPSU2LPEXIT
-            # TXLFPSU3WAKE
-            # TXMUXDCDEXHOLD
-            # TXMUXDCDORWREN
-            # TXONESZEROS
-            # DMONITOROUTCLK
-            # POWERPRESENT
-            # RXCKCALDONE
-            # RXLFPSTRESETDET
-            # RXLFPSU2LPEXITDET
-            # RXLFPSU3WAKEDET
-            # TXDCCDONE
+        self.specials += Instance("GTHE4_CHANNEL", **self.gth_params)
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gth_ultrascale_init.py` & `liteiclink-2023.8/liteiclink/serdes/gth_ultrascale_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
 from migen.genlib.cdc import MultiReg
-from migen.genlib.misc import WaitTimer
+
+from litex.gen import *
+
+from litex.gen.genlib.misc import WaitTimer
 
 
 __all__ = ["GTHTXInit", "GTHRXInit"]
 
 # GTH Init -----------------------------------------------------------------------------------------
 
-class GTHInit(Module):
+class GTHInit(LiteXModule):
     def __init__(self, sys_clk_freq, rx, buffer_enable):
         self.done            = Signal() # o
         self.restart         = Signal() # i
 
         # GTH signals
         self.plllock         = Signal() # i
         self.pllreset        = Signal() # o
@@ -27,14 +30,18 @@
         self.Xxresetdone     = Signal() # i
         self.Xxdlysreset     = Signal() # o
         self.Xxdlysresetdone = Signal() # i
         self.Xxphaligndone   = Signal() # i
         self.Xxsyncdone      = Signal() # i
         self.Xxuserrdy       = Signal() # o
 
+        # DRP (optional)
+        self.drp_start       = Signal()        # o
+        self.drp_done        = Signal(reset=1) # i
+
         # # #
 
         # Double-latch transceiver asynch outputs
         plllock         = Signal()
         Xxresetdone     = Signal()
         Xxdlysresetdone = Signal()
         Xxphaligndone   = Signal()
@@ -58,19 +65,18 @@
         ]
 
         # PLL reset must be at least 2us
         pll_reset_cycles = ceil(2e-6*sys_clk_freq)
         pll_reset_timer  = WaitTimer(pll_reset_cycles)
         self.submodules += pll_reset_timer
 
-        fsm = ResetInserter()(FSM(reset_state="RESET_ALL"))
-        self.submodules.fsm = fsm
+        self.fsm = fsm = ResetInserter()(FSM(reset_state="RESET_ALL"))
 
-        ready_timer = WaitTimer(int(10e-3*sys_clk_freq))
-        self.submodules.ready_timer = ready_timer
+        ready_timer = WaitTimer(10e-3*sys_clk_freq)
+        self.ready_timer = ready_timer
         self.comb += [
             ready_timer.wait.eq(~self.done & ~fsm.reset),
             fsm.reset.eq(self.restart | ready_timer.done)
         ]
 
         if rx:
             cdr_stable_timer = WaitTimer(1024)
@@ -82,14 +88,22 @@
         self.comb += Xxphaligndone_rising.eq(Xxphaligndone & ~Xxphaligndone_r)
 
         fsm.act("RESET_ALL",
             gtXxreset.eq(1),
             self.pllreset.eq(1),
             pll_reset_timer.wait.eq(1),
             If(pll_reset_timer.done,
+                NextState("DRP")
+            )
+        )
+        fsm.act("DRP",
+            gtXxreset.eq(1),
+            self.pllreset.eq(1),
+            self.drp_start.eq(1),
+            If(self.drp_done,
                 NextState("RELEASE_PLL_RESET")
             )
         )
         fsm.act("RELEASE_PLL_RESET",
             gtXxreset.eq(1),
             If(plllock, NextState("RELEASE_GTH_RESET"))
         )
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gtp_7series.py` & `liteiclink-2023.8/liteiclink/serdes/gtp_7series.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from liteiclink.serdes.gtp_7series_init import GTPTXInit, GTPRXInit
 from liteiclink.serdes.clock_aligner import BruteforceClockAligner
 
 from liteiclink.serdes.common import *
 
 # GTP Quad PLL -------------------------------------------------------------------------------------
 
-class GTPQuadPLL(Module):
+class GTPQuadPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate, channel=0, shared=False):
         assert channel in [0, 1]
         self.channel = channel
         self.clk     = Signal()
         self.refclk  = Signal()
         self.reset   = Signal()
         self.lock    = Signal()
@@ -152,16 +152,16 @@
            vco_freq = config["vco_freq"]/1e9,
            d        = config["d"],
            linerate = config["linerate"]/1e9)
         return r
 
 # GTP ----------------------------------------------------------------------------------------------
 
-class GTP(Module, AutoCSR):
-    def __init__(self, qpll, tx_pads, rx_pads, sys_clk_freq, qpll_reset=True,
+class GTP(LiteXModule):
+    def __init__(self, qpll, tx_pads, rx_pads, sys_clk_freq, qpll_reset=True, tx_clk=None, rx_clk=None,
         data_width          = 20,
         tx_buffer_enable    = False,
         rx_buffer_enable    = False,
         clock_aligner       = True,
         clock_aligner_comma = 0b0101111100,
         tx_polarity         = 0,
         rx_polarity         = 0):
@@ -190,15 +190,15 @@
         # Loopback
         self.loopback = Signal(3)
 
         # # #
 
         self.nwords = nwords = data_width//10
 
-        self.submodules.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
+        self.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
         self.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
         self.submodules += self.decoders
 
         # Transceiver direct clock outputs (useful to specify clock constraints)
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
@@ -236,37 +236,37 @@
             2 : 0x0000107FE206001041010,
             4 : 0x0000107FE106001041010,
             8 : 0x0000107FE086001041010,
            16 : 0x0000107FE086001041010,
         }
 
         # TX init ----------------------------------------------------------------------------------
-        self.submodules.tx_init = tx_init = GTPTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
+        self.tx_init = tx_init = GTPTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
         self.comb += [
             self.tx_ready.eq(tx_init.done),
             tx_init.restart.eq(~self.tx_enable)
         ]
 
         # RX init ----------------------------------------------------------------------------------
-        self.submodules.rx_init = rx_init = GTPRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
+        self.rx_init = rx_init = GTPRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
         self.comb += [
             self.rx_ready.eq(rx_init.done),
             rx_init.restart.eq(~self.rx_enable)
         ]
 
         # PLL --------------------------------------------------------------------------------------
         self.comb += [
             tx_init.plllock.eq(qpll.lock),
             rx_init.plllock.eq(qpll.lock)
         ]
         if qpll_reset:
             self.comb += qpll.reset.eq(tx_init.pllreset)
 
         # DRP mux ----------------------------------------------------------------------------------
-        self.submodules.drp_mux = drp_mux = DRPMux()
+        self.drp_mux = drp_mux = DRPMux()
         drp_mux.add_interface(rx_init.drp)
         drp_mux.add_interface(self.drp)
 
         # GTPE2_CHANNEL instance -------------------------------------------------------------------
         txdata = Signal(data_width)
         rxdata = Signal(data_width)
         rxphaligndone = Signal()
@@ -928,97 +928,117 @@
             i_TXPRBSSEL            = 0,
         )
 
         # TX clocking ------------------------------------------------------------------------------
         tx_reset_deglitched = Signal()
         tx_reset_deglitched.attr.add("no_retiming")
         self.sync += tx_reset_deglitched.eq(~tx_init.done)
-        self.clock_domains.cd_tx = ClockDomain()
+        self.cd_tx = ClockDomain()
 
-        txoutclk_bufg = Signal()
-        self.specials += Instance("BUFG",
-            i_I = self.txoutclk,
-            o_O = txoutclk_bufg,
-        )
+        # Use/generate local tx_clk.
+        # --------------------------
+        if tx_clk is None:
+            txoutclk_bufg = Signal()
+            self.specials += Instance("BUFG",
+                i_I = self.txoutclk,
+                o_O = txoutclk_bufg,
+            )
+
+            if not tx_buffer_enable:
+                txoutclk_div = qpll.config["clkin"]/self.tx_clk_freq
+            else:
+                txoutclk_div = 1
+            # Use txoutclk_bufg when divider is 1
+            if txoutclk_div == 1:
+                self.comb += self.cd_tx.clk.eq(txoutclk_bufg)
+                self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+            # Use a BUFR when integer divider (with BUFR_DIVIDE)
+            elif txoutclk_div == int(txoutclk_div):
+                txoutclk_bufr = Signal()
+                self.specials += [
+                    Instance("BUFR",
+                        p_BUFR_DIVIDE = str(int(txoutclk_div)),
+                        i_CE = 1,
+                        i_I  = txoutclk_bufg,
+                        o_O  = txoutclk_bufr,
+                    ),
+                    Instance("BUFG",
+                        i_I = txoutclk_bufr,
+                        o_O = self.cd_tx.clk,
+                    ),
+                    AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+                ]
+            # Use a PLL when non-integer divider
+            else:
+                txoutclk_pll = S7PLL()
+                self.comb += txoutclk_pll.reset.eq(tx_reset_deglitched)
+                self.submodules += txoutclk_pll
+                txoutclk_pll.register_clkin(txoutclk_bufg, qpll.config["clkin"])
+                txoutclk_pll.create_clkout(self.cd_tx, self.tx_clk_freq)
 
-        if not tx_buffer_enable:
-            txoutclk_div = qpll.config["clkin"]/self.tx_clk_freq
+        # Use provided/shared tx_clk.
+        # ---------------------------
         else:
-            txoutclk_div = 1
-        # Use txoutclk_bufg when divider is 1
-        if txoutclk_div == 1:
-            self.comb += self.cd_tx.clk.eq(txoutclk_bufg)
+            assert tx_buffer_enable
+            self.cd_tx.clk = tx_clk # Override instead of assign to only keep one real clk.
             self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-        # Use a BUFR when integer divider (with BUFR_DIVIDE)
-        elif txoutclk_div == int(txoutclk_div):
-            txoutclk_bufr = Signal()
-            self.specials += [
-                Instance("BUFR",
-                    p_BUFR_DIVIDE = str(int(txoutclk_div)),
-                    i_CE = 1,
-                    i_I  = txoutclk_bufg,
-                    o_O  = txoutclk_bufr,
-                ),
-                Instance("BUFG",
-                    i_I = txoutclk_bufr,
-                    o_O = self.cd_tx.clk,
-                ),
-                AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-            ]
-        # Use a PLL when non-integer divider
-        else:
-            txoutclk_pll = S7PLL()
-            self.comb += txoutclk_pll.reset.eq(tx_reset_deglitched)
-            self.submodules += txoutclk_pll
-            txoutclk_pll.register_clkin(txoutclk_bufg, qpll.config["clkin"])
-            txoutclk_pll.create_clkout(self.cd_tx, self.tx_clk_freq)
 
         # RX clocking ------------------------------------------------------------------------------
         rx_reset_deglitched = Signal()
         rx_reset_deglitched.attr.add("no_retiming")
         self.sync.tx += rx_reset_deglitched.eq(~rx_init.done)
-        self.clock_domains.cd_rx = ClockDomain()
-        self.specials += [
-            Instance("BUFG",
-                i_I = self.rxoutclk,
-                o_O = self.cd_rx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
-        ]
+        self.cd_rx = ClockDomain()
+
+        # Use/generate local rx_clk.
+        # --------------------------
+        if rx_clk is None:
+            self.specials += [
+                Instance("BUFG",
+                    i_I = self.rxoutclk,
+                    o_O = self.cd_rx.clk,
+                ),
+                AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
+            ]
+        # Use provided/shared rx_clk.
+        # ---------------------------
+        else:
+            assert rx_buffer_enable
+            self.cd_rx.clk = rx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
 
         # TX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
+        self.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
         self.comb += self.tx_prbs.config.eq(tx_prbs_config)
         self.comb += [
             self.tx_prbs.i.eq(Cat(*[self.encoder.output[i] for i in range(nwords)])),
             If(tx_produce_square_wave,
                 # square wave @ linerate/data_width for scope observation
                 txdata.eq(Signal(data_width, reset=(1<<(data_width//2))-1))
             ).Elif(tx_produce_pattern,
                 txdata.eq(tx_pattern)
             ).Else(
                 txdata.eq(self.tx_prbs.o)
             )
         ]
 
         # RX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
+        self.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
         self.comb += [
             self.rx_prbs.config.eq(rx_prbs_config),
             self.rx_prbs.pause.eq(rx_prbs_pause),
             rx_prbs_errors.eq(self.rx_prbs.errors)
         ]
         for i in range(nwords):
             self.comb += self.decoders[i].input.eq(rxdata[10*i:10*(i+1)])
         self.sync.rx += self.rx_prbs.i.eq(rxdata)
 
         # Clock Aligner ----------------------------------------------------------------------------
         if clock_aligner:
             clock_aligner = BruteforceClockAligner(clock_aligner_comma, self.tx_clk_freq, check_period=10e-3)
-            self.submodules.clock_aligner = clock_aligner
+            self.clock_aligner = clock_aligner
             ps_restart = PulseSynchronizer("tx", "sys")
             self.submodules += ps_restart
             self.comb += [
                 clock_aligner.rxdata.eq(rxdata),
                 ps_restart.i.eq(clock_aligner.restart),
                 rx_init.restart.eq((ps_restart.o & self.rx_align) | ~self.rx_enable),
                 self.rx_ready.eq(clock_aligner.ready)
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gtp_7series_init.py` & `liteiclink-2023.8/liteiclink/serdes/gtp_7series_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
-from migen.genlib.misc import WaitTimer
+
+from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
 
 from liteiclink.serdes.common import *
 
 
 __all__ = ["GTPTXInit", "GTPRXInit"]
 
 # GTP TX Init --------------------------------------------------------------------------------------
 
-class GTPTXInit(Module):
+class GTPTXInit(LiteXModule):
     def __init__(self, sys_clk_freq, buffer_enable):
         self.done            = Signal() # o
         self.restart         = Signal() # i
 
         # GTP signals
         self.plllock         = Signal() # i
         self.pllreset        = Signal() # o
@@ -78,16 +80,15 @@
         # Detect txphaligndone rising edge
         txphaligndone_r = Signal(reset=1)
         txphaligndone_rising = Signal()
         self.sync += txphaligndone_r.eq(txphaligndone)
         self.comb += txphaligndone_rising.eq(txphaligndone & ~txphaligndone_r)
 
         # FSM
-        fsm = ResetInserter()(FSM(reset_state="POWER-DOWN"))
-        self.submodules.fsm = fsm
+        self.fsm = fsm =ResetInserter()(FSM(reset_state="POWER-DOWN"))
         fsm.act("POWER-DOWN",
             gttxreset.eq(1),
             gttxpd.eq(1),
             self.pllreset.eq(1),
             NextState("DRP")
         )
         fsm.act("DRP",
@@ -101,15 +102,15 @@
         fsm.act("WAIT-PLL-RESET",
             gttxreset.eq(1),
             If(plllock,
                 NextState("WAIT-INIT-DELAY")
             )
         )
         # Wait 500ns after configuration before releasing GTP reset (to follow AR43482)
-        init_delay = WaitTimer(int(500e-9*sys_clk_freq))
+        init_delay = WaitTimer(500e-9*sys_clk_freq)
         self.submodules += init_delay
         self.comb += init_delay.wait.eq(1)
         fsm.act("WAIT-INIT-DELAY",
             gttxreset.eq(1),
             If(init_delay.done,
                 NextState("WAIT-GTP-RESET")
             )
@@ -159,24 +160,24 @@
             self.done.eq(1),
             If(self.restart,
                 NextState("POWER-DOWN")
             )
         )
 
         # FSM watchdog / restart
-        watchdog = WaitTimer(int(1e-3*sys_clk_freq))
+        watchdog = WaitTimer(1e-3*sys_clk_freq)
         self.submodules += watchdog
         self.comb += [
             watchdog.wait.eq(~fsm.reset & ~self.done),
             fsm.reset.eq(self.restart | watchdog.done)
         ]
 
 # GTP RX Init --------------------------------------------------------------------------------------
 
-class GTPRXInit(Module):
+class GTPRXInit(LiteXModule):
     def __init__(self, sys_clk_freq, buffer_enable):
         self.done            = Signal()
         self.restart         = Signal()
 
         # GTP signals
         self.plllock         = Signal()
         self.gtrxreset       = Signal()
@@ -232,23 +233,22 @@
             self.gtrxreset.eq(gtrxreset),
             self.gtrxpd.eq(gtrxpd),
             self.rxdlysreset.eq(rxdlysreset),
             self.rxphalign.eq(rxphalign),
             self.rxuserrdy.eq(rxuserrdy)
         ]
 
-        fsm = ResetInserter()(FSM(reset_state="POWER-DOWN"))
-        self.submodules.fsm = fsm
+        self.fsm = fsm = ResetInserter()(FSM(reset_state="POWER-DOWN"))
         fsm.act("POWER-DOWN",
             gtrxreset.eq(1),
             gtrxpd.eq(1),
             NextState("WAIT-INIT-DELAY")
         )
         # Wait 500ns after configuration before releasing GTP reset (to follow AR43482)
-        init_delay = WaitTimer(int(500e-9*sys_clk_freq))
+        init_delay = WaitTimer(500e-9*sys_clk_freq)
         self.submodules += init_delay
         self.comb += init_delay.wait.eq(1)
         fsm.act("WAIT-INIT-DELAY",
             gtrxreset.eq(1),
             If(plllock & init_delay.done,
                 NextState("DRP_READ_ISSUE")
             )
@@ -324,13 +324,13 @@
             self.done.eq(1),
             If(self.restart,
                 NextState("POWER-DOWN")
             )
         )
 
         # FSM watchdog / restart
-        watchdog = WaitTimer(int(4e-3*sys_clk_freq))
+        watchdog = WaitTimer(4e-3*sys_clk_freq)
         self.submodules += watchdog
         self.comb += [
             watchdog.wait.eq(~fsm.reset & ~self.done),
             fsm.reset.eq(self.restart | watchdog.done)
         ]
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gtx_7series.py` & `liteiclink-2023.8/liteiclink/serdes/gtx_7series.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from liteiclink.serdes.gtx_7series_init import GTXTXInit, GTXRXInit
 from liteiclink.serdes.clock_aligner import BruteforceClockAligner
 
 from liteiclink.serdes.common import *
 
 # GTX Channel PLL ----------------------------------------------------------------------------------
 
-class GTXChannelPLL(Module):
+class GTXChannelPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.refclk = refclk
         self.reset  = Signal()
         self.lock   = Signal()
         self.config = self.compute_config(refclk_freq, linerate)
 
     @staticmethod
@@ -83,15 +83,15 @@
            vco_freq = config["vco_freq"]/1e9,
            d        = config["d"],
            linerate = config["linerate"]/1e9)
         return r
 
 # GTX Quad PLL -------------------------------------------------------------------------------------
 
-class GTXQuadPLL(Module):
+class GTXQuadPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.clk       = Signal()
         self.refclk    = Signal()
         self.reset     = Signal()
         self.lock      = Signal()
         self.powerdown = Signal()
         self.config    = self.compute_config(refclk_freq, linerate)
@@ -208,16 +208,16 @@
            vco_band = self.config["vco_band"],
            d        = self.config["d"],
            linerate = self.config["linerate"]/1e9)
         return r
 
 # GTX ----------------------------------------------------------------------------------------------
 
-class GTX(Module, AutoCSR):
-    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq,
+class GTX(LiteXModule):
+    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq, tx_clk=None, rx_clk=None,
         data_width          = 20,
         tx_buffer_enable    = False,
         rx_buffer_enable    = False,
         clock_aligner       = True,
         clock_aligner_comma = 0b0101111100,
         tx_polarity         = 0,
         rx_polarity         = 0,
@@ -247,15 +247,15 @@
         # Loopback
         self.loopback = Signal(3)
 
         # # #
 
         self.nwords = nwords = data_width//10
 
-        self.submodules.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
+        self.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
         self.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
         self.submodules += self.decoders
 
         # Transceiver direct clock outputs (useful to specify clock constraints)
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
@@ -295,37 +295,37 @@
             2 : 0x03000023ff10200020,
             4 : 0x03000023ff10100020,
             8 : 0x03000023ff10080020,
            16 : 0x03000023ff10080020,
         }
 
         # TX init ----------------------------------------------------------------------------------
-        self.submodules.tx_init = tx_init = GTXTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
+        self.tx_init = tx_init = GTXTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
         self.comb += [
             self.tx_ready.eq(tx_init.done),
             tx_init.restart.eq(~self.tx_enable)
         ]
 
         # RX init ----------------------------------------------------------------------------------
-        self.submodules.rx_init = rx_init = GTXRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
+        self.rx_init = rx_init = GTXRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
         self.comb += [
             self.rx_ready.eq(rx_init.done),
             rx_init.restart.eq(~self.rx_enable)
         ]
 
         # PLL ----------------------------------------------------------------------------------
         self.comb += [
             tx_init.plllock.eq(pll.lock),
             rx_init.plllock.eq(pll.lock)
         ]
         if pll_master:
             self.comb += pll.reset.eq(tx_init.pllreset)
 
         # DRP mux ----------------------------------------------------------------------------------
-        self.submodules.drp_mux = drp_mux = DRPMux()
+        self.drp_mux = drp_mux = DRPMux()
         drp_mux.add_interface(self.drp)
 
         # GTXE2_CHANNEL instance -------------------------------------------------------------------
         txdata = Signal(data_width)
         rxdata = Signal(data_width)
         self.gtx_params = dict(
             # Simulation-Only Attributes
@@ -959,97 +959,117 @@
             o_TXQPISENP        = Open(),
         )
 
         # TX clocking ------------------------------------------------------------------------------
         tx_reset_deglitched = Signal()
         tx_reset_deglitched.attr.add("no_retiming")
         self.sync += tx_reset_deglitched.eq(~tx_init.done)
-        self.clock_domains.cd_tx = ClockDomain()
+        self.cd_tx = ClockDomain()
 
-        txoutclk_bufg = Signal()
-        self.specials += Instance("BUFG",
-            i_I = self.txoutclk,
-            o_O = txoutclk_bufg,
-        )
+        # Use/generate local tx_clk.
+        # --------------------------
+        if tx_clk is None:
+            txoutclk_bufg = Signal()
+            self.specials += Instance("BUFG",
+                i_I = self.txoutclk,
+                o_O = txoutclk_bufg,
+            )
+
+            if not tx_buffer_enable:
+                txoutclk_div = pll.config["clkin"]/self.tx_clk_freq
+            else:
+                txoutclk_div = 1
+            # Use txoutclk_bufg when divider is 1
+            if txoutclk_div == 1:
+                self.comb += self.cd_tx.clk.eq(txoutclk_bufg)
+                self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+            # Use a BUFR when integer divider (with BUFR_DIVIDE)
+            elif txoutclk_div == int(txoutclk_div):
+                txoutclk_bufr = Signal()
+                self.specials += [
+                    Instance("BUFR",
+                        p_BUFR_DIVIDE = str(int(txoutclk_div)),
+                        i_CE = 1,
+                        i_I  = txoutclk_bufg,
+                        o_O  = txoutclk_bufr,
+                    ),
+                    Instance("BUFG",
+                        i_I = txoutclk_bufr,
+                        o_O = self.cd_tx.clk,
+                    ),
+                    AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+                ]
+            # Use a PLL when non-integer divider
+            else:
+                txoutclk_pll = S7PLL()
+                self.comb += txoutclk_pll.reset.eq(tx_reset_deglitched)
+                self.submodules += txoutclk_pll
+                txoutclk_pll.register_clkin(txoutclk_bufg, pll.config["clkin"])
+                txoutclk_pll.create_clkout(self.cd_tx, self.tx_clk_freq)
 
-        if not tx_buffer_enable:
-            txoutclk_div = pll.config["clkin"]/self.tx_clk_freq
+        # Use provided/shared tx_clk.
+        # ---------------------------
         else:
-            txoutclk_div = 1
-        # Use txoutclk_bufg when divider is 1
-        if txoutclk_div == 1:
-            self.comb += self.cd_tx.clk.eq(txoutclk_bufg)
+            assert tx_buffer_enable
+            self.cd_tx.clk = tx_clk # Override instead of assign to only keep one real clk.
             self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-        # Use a BUFR when integer divider (with BUFR_DIVIDE)
-        elif txoutclk_div == int(txoutclk_div):
-            txoutclk_bufr = Signal()
-            self.specials += [
-                Instance("BUFR",
-                    p_BUFR_DIVIDE = str(int(txoutclk_div)),
-                    i_CE = 1,
-                    i_I  = txoutclk_bufg,
-                    o_O  = txoutclk_bufr,
-                ),
-                Instance("BUFG",
-                    i_I = txoutclk_bufr,
-                    o_O = self.cd_tx.clk,
-                ),
-                AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-            ]
-        # Use a PLL when non-integer divider
-        else:
-            txoutclk_pll = S7PLL()
-            self.comb += txoutclk_pll.reset.eq(tx_reset_deglitched)
-            self.submodules += txoutclk_pll
-            txoutclk_pll.register_clkin(txoutclk_bufg, pll.config["clkin"])
-            txoutclk_pll.create_clkout(self.cd_tx, self.tx_clk_freq)
 
         # RX clocking ------------------------------------------------------------------------------
         rx_reset_deglitched = Signal()
         rx_reset_deglitched.attr.add("no_retiming")
         self.sync.tx += rx_reset_deglitched.eq(~rx_init.done)
-        self.clock_domains.cd_rx = ClockDomain()
-        self.specials += [
-            Instance("BUFG",
-                i_I = self.rxoutclk,
-                o_O = self.cd_rx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
-        ]
+        self.cd_rx = ClockDomain()
+
+        # Use/generate local rx_clk.
+        # --------------------------
+        if rx_clk is None:
+            self.specials += [
+                Instance("BUFG",
+                    i_I = self.rxoutclk,
+                    o_O = self.cd_rx.clk,
+                ),
+                AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
+            ]
+        # Use provided/shared rx_clk.
+        # ---------------------------
+        else:
+            assert rx_buffer_enable
+            self.cd_rx.clk = rx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
 
         # TX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
+        self.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
         self.comb += self.tx_prbs.config.eq(tx_prbs_config)
         self.comb += [
             self.tx_prbs.i.eq(Cat(*[self.encoder.output[i] for i in range(nwords)])),
             If(tx_produce_square_wave,
                 # square wave @ linerate/data_width for scope observation
                 txdata.eq(Signal(data_width, reset=(1<<(data_width//2))-1))
             ).Elif(tx_produce_pattern,
                 txdata.eq(tx_pattern)
             ).Else(
                 txdata.eq(self.tx_prbs.o)
             )
         ]
 
         # RX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
+        self.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
         self.comb += [
             self.rx_prbs.config.eq(rx_prbs_config),
             self.rx_prbs.pause.eq(rx_prbs_pause),
             rx_prbs_errors.eq(self.rx_prbs.errors)
         ]
         for i in range(nwords):
             self.comb += self.decoders[i].input.eq(rxdata[10*i:10*(i+1)])
         self.sync.rx += self.rx_prbs.i.eq(rxdata)
 
         # Clock Aligner ----------------------------------------------------------------------------
         if clock_aligner:
             clock_aligner = BruteforceClockAligner(clock_aligner_comma, self.tx_clk_freq)
-            self.submodules.clock_aligner = clock_aligner
+            self.clock_aligner = clock_aligner
             ps_restart = PulseSynchronizer("tx", "sys")
             self.submodules += ps_restart
             self.comb += [
                 clock_aligner.rxdata.eq(rxdata),
                 ps_restart.i.eq(clock_aligner.restart),
                 rx_init.restart.eq((ps_restart.o & self.rx_align) | ~self.rx_enable),
                 self.rx_ready.eq(clock_aligner.ready)
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gtx_7series_init.py` & `liteiclink-2023.8/liteiclink/serdes/gtx_7series_init.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
-from migen.genlib.misc import WaitTimer
+
+from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
 
 
 __all__ = ["GTXTXInit", "GTXRXInit"]
 
 # GTX Init -----------------------------------------------------------------------------------------
 
-class GTXInit(Module):
+class GTXInit(LiteXModule):
     def __init__(self, sys_clk_freq, buffer_enable):
         self.done            = Signal() # o
         self.restart         = Signal() # i
 
         # GTX signals
         self.plllock         = Signal() # i
         self.pllreset        = Signal() # o
@@ -64,16 +66,15 @@
             self.gtXxreset.eq(gtXxreset),
             self.gtXxpd.eq(gtXxpd),
             self.Xxdlysreset.eq(Xxdlysreset),
             self.Xxuserrdy.eq(Xxuserrdy)
         ]
 
         # FSM
-        fsm = ResetInserter()(FSM(reset_state="POWER-DOWN"))
-        self.submodules.fsm = fsm
+        self.fsm = fsm = ResetInserter()(FSM(reset_state="POWER-DOWN"))
         fsm.act("POWER-DOWN",
             gtXxreset.eq(1),
             gtXxpd.eq(1),
             self.pllreset.eq(1),
             NextState("DRP")
         )
         fsm.act("DRP",
@@ -87,15 +88,15 @@
         fsm.act("WAIT-PLL-RESET",
             gtXxreset.eq(1),
             If(plllock,
                 NextState("WAIT-INIT-DELAY")
             )
         )
         # Wait 500ns after configuration before releasing GTX reset (to follow AR43482)
-        init_delay = WaitTimer(int(500e-9*sys_clk_freq))
+        init_delay = WaitTimer(500e-9*sys_clk_freq)
         self.submodules += init_delay
         self.comb += init_delay.wait.eq(1)
         fsm.act("WAIT-INIT-DELAY",
             gtXxreset.eq(1),
             If(init_delay.done,
                 NextState("WAIT-GTX-RESET")
             )
@@ -149,15 +150,15 @@
             self.done.eq(1),
             If(self.restart,
                 NextState("POWER-DOWN")
             )
         )
 
         # FSM watchdog / restart
-        watchdog = WaitTimer(int(1e-3*sys_clk_freq))
+        watchdog = WaitTimer(1e-3*sys_clk_freq)
         self.submodules += watchdog
         self.comb += [
             watchdog.wait.eq(~fsm.reset & ~self.done),
             fsm.reset.eq(self.restart | watchdog.done)
         ]
 
 # GTX TX Init --------------------------------------------------------------------------------------
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gty_ultrascale.py` & `liteiclink-2023.8/liteiclink/serdes/gty_ultrascale.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 
 from litex.gen import *
 
 from migen import *
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from litex.soc.interconnect.csr import *
 from litex.soc.interconnect import stream
 from litex.soc.cores.prbs import PRBSTX, PRBSRX
 from litex.soc.cores.code_8b10b import Encoder, Decoder
 
 from liteiclink.serdes.gty_ultrascale_init import GTYRXInit, GTYTXInit
 from liteiclink.serdes.clock_aligner import BruteforceClockAligner
 
 from liteiclink.serdes.common import *
 
 # GTY Channel PLL ----------------------------------------------------------------------------------
 
-class GTYChannelPLL(Module):
+class GTYChannelPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.refclk = refclk
         self.reset  = Signal()
         self.lock   = Signal()
         self.config = self.compute_config(refclk_freq, linerate)
 
     @staticmethod
@@ -84,15 +86,15 @@
            vco_freq = config["vco_freq"]/1e9,
            d        = config["d"],
            linerate = config["linerate"]/1e9)
         return r
 
 # GTY Quad PLL -------------------------------------------------------------------------------------
 
-class GTYQuadPLL(Module):
+class GTYQuadPLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.clk       = Signal()
         self.refclk    = Signal()
         self.reset     = Signal()
         self.lock      = Signal()
         self.powerdown = Signal()
         self.config = config = self.compute_config(refclk_freq, linerate)
@@ -316,23 +318,24 @@
            qpll           = config["qpll"].upper(),
            d              = config["d"],
            linerate       = config["linerate"]/1e9)
         return r
 
 # GTY ----------------------------------------------------------------------------------------------
 
-class GTY(Module, AutoCSR):
-    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq,
+class GTY(LiteXModule):
+    def __init__(self, pll, tx_pads, rx_pads, sys_clk_freq, tx_clk=None, rx_clk=None,
         data_width          = 20,
         tx_buffer_enable    = False,
         rx_buffer_enable    = False,
         clock_aligner       = True,
         clock_aligner_comma = 0b0101111100,
         tx_polarity         = 0,
-        rx_polarity         = 0):
+        rx_polarity         = 0,
+        pll_master          = True):
         assert data_width in [20, 40, 80]
 
         # TX controls
         self.tx_enable              = Signal(reset=1)
         self.tx_ready               = Signal()
         self.tx_inhibit             = Signal()
         self.tx_produce_square_wave = Signal()
@@ -358,15 +361,15 @@
 
         use_cpll  = isinstance(pll, GTYChannelPLL)
         use_qpll0 = isinstance(pll, GTYQuadPLL) and pll.config["qpll"] == "qpll0"
         use_qpll1 = isinstance(pll, GTYQuadPLL) and pll.config["qpll"] == "qpll1"
 
         self.nwords = nwords = data_width//10
 
-        self.submodules.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
+        self.encoder = ClockDomainsRenamer("tx")(Encoder(nwords, True))
         self.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
         self.submodules += self.decoders
 
         # Transceiver direct clock outputs (useful to specify clock constraints)
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
@@ -395,37 +398,37 @@
             MultiReg(self.rx_prbs_pause, rx_prbs_pause, "rx"),
             MultiReg(rx_prbs_errors, self.rx_prbs_errors, "sys"),
         ]
 
         # # #
 
         # TX init ----------------------------------------------------------------------------------
-        self.submodules.tx_init = tx_init = GTYTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
+        self.tx_init = tx_init = GTYTXInit(sys_clk_freq, buffer_enable=tx_buffer_enable)
         self.comb += [
             self.tx_ready.eq(tx_init.done),
             tx_init.restart.eq(~self.tx_enable)
         ]
 
         # RX init ----------------------------------------------------------------------------------
-        self.submodules.rx_init = rx_init = GTYRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
+        self.rx_init = rx_init = GTYRXInit(sys_clk_freq, buffer_enable=rx_buffer_enable)
         self.comb += [
             self.rx_ready.eq(rx_init.done),
             rx_init.restart.eq(~self.rx_enable)
         ]
 
         # PLL ----------------------------------------------------------------------------------
         self.comb += [
             tx_init.plllock.eq(pll.lock),
             rx_init.plllock.eq(pll.lock)
         ]
         if pll_master:
             self.comb += pll.reset.eq(tx_init.pllreset)
 
         # DRP mux ----------------------------------------------------------------------------------
-        self.submodules.drp_mux = drp_mux = DRPMux()
+        self.drp_mux = drp_mux = DRPMux()
         drp_mux.add_interface(self.drp)
 
         # GTYE4_CHANNEL instance -------------------------------------------------------------------
         txdata = Signal(data_width)
         rxdata = Signal(data_width)
         rxphaligndone = Signal()
 
@@ -1115,66 +1118,87 @@
             o_GTYTXN          = tx_pads.n
         )
 
         # TX clocking ------------------------------------------------------------------------------
         tx_reset_deglitched = Signal()
         tx_reset_deglitched.attr.add("no_retiming")
         self.sync += tx_reset_deglitched.eq(~tx_init.done)
-        self.clock_domains.cd_tx = ClockDomain()
-        if not tx_buffer_enable:
-            tx_bufg_div = pll.config["clkin"]/self.tx_clk_freq
+        self.cd_tx = ClockDomain()
+
+        # Use/generate local tx_clk.
+        # --------------------------
+        if tx_clk is None:
+            if not tx_buffer_enable:
+                tx_bufg_div = pll.config["clkin"]/self.tx_clk_freq
+            else:
+                tx_bufg_div = 1
+            assert tx_bufg_div == int(tx_bufg_div)
+            self.specials += [
+                Instance("BUFG_GT", i_I=self.txoutclk, o_O=self.cd_tx.clk,
+                    i_DIV=int(tx_bufg_div)-1),
+                AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
+            ]
+
+        # Use provided/shared tx_clk.
+        # ---------------------------
         else:
-            tx_bufg_div = 1
-        assert tx_bufg_div == int(tx_bufg_div)
-        self.specials += [
-            Instance("BUFG_GT", i_I=self.txoutclk, o_O=self.cd_tx.clk,
-                i_DIV=int(tx_bufg_div)-1),
-            AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
-        ]
+            assert tx_buffer_enable
+            self.cd_tx.clk = tx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_tx, tx_reset_deglitched)
 
         # RX clocking ------------------------------------------------------------------------------
         rx_reset_deglitched = Signal()
         rx_reset_deglitched.attr.add("no_retiming")
         self.sync.tx += rx_reset_deglitched.eq(~rx_init.done)
-        self.clock_domains.cd_rx = ClockDomain()
-        self.specials += [
-            Instance("BUFG_GT", i_I=self.rxoutclk, o_O=self.cd_rx.clk),
-            AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
-        ]
+        self.cd_rx = ClockDomain()
+
+        # Use/generate local rx_clk.
+        # --------------------------
+        if rx_clk is None:
+            self.specials += [
+                Instance("BUFG_GT", i_I=self.rxoutclk, o_O=self.cd_rx.clk),
+                AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
+            ]
+        # Use provided/shared rx_clk.
+        # ---------------------------
+        else:
+            assert rx_buffer_enable
+            self.cd_rx.clk = rx_clk # Override instead of assign to only keep one real clk.
+            self.specials += AsyncResetSynchronizer(self.cd_rx, rx_reset_deglitched)
 
         # TX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
+        self.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
         self.comb += self.tx_prbs.config.eq(tx_prbs_config)
         self.comb += [
             self.tx_prbs.i.eq(Cat(*[self.encoder.output[i] for i in range(nwords)])),
             If(tx_produce_square_wave,
                 # square wave @ linerate/data_width for scope observation
                 txdata.eq(Signal(data_width, reset=(1<<(data_width//2))-1))
             ).Elif(tx_produce_pattern,
                 txdata.eq(tx_pattern)
             ).Else(
                 txdata.eq(self.tx_prbs.o)
             )
         ]
 
         # RX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
+        self.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
         self.comb += [
             self.rx_prbs.config.eq(rx_prbs_config),
             self.rx_prbs.pause.eq(rx_prbs_pause),
             rx_prbs_errors.eq(self.rx_prbs.errors)
         ]
         for i in range(nwords):
             self.comb += self.decoders[i].input.eq(rxdata[10*i:10*(i+1)])
         self.sync.rx += self.rx_prbs.i.eq(rxdata)
 
         # Clock Aligner ----------------------------------------------------------------------------
         if clock_aligner:
             clock_aligner = BruteforceClockAligner(clock_aligner_comma, self.tx_clk_freq)
-            self.submodules.clock_aligner = clock_aligner
+            self.clock_aligner = clock_aligner
             ps_restart = PulseSynchronizer("tx", "sys")
             self.submodules += ps_restart
             self.comb += [
                 clock_aligner.rxdata.eq(rxdata),
                 ps_restart.i.eq(clock_aligner.restart),
                 rx_init.restart.eq((ps_restart.o & self.rx_align) | ~self.rx_enable),
                 self.rx_ready.eq(clock_aligner.ready)
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/gty_ultrascale_init.py` & `liteiclink-2023.8/liteiclink/serdes/gty_ultrascale_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
-from migen.genlib.cdc import MultiReg
-from migen.genlib.misc import WaitTimer
+
+from litex.gen import *
+from litex.gen.genlib.cdc import MultiReg
+from litex.gen.genlib.misc import WaitTimer
 
 
 __all__ = ["GTYTXInit", "GTYRXInit"]
 
 # GTY Init -----------------------------------------------------------------------------------------
 
-class GTYInit(Module):
+class GTYInit(LiteXModule):
     def __init__(self, sys_clk_freq, rx, buffer_enable):
         self.done            = Signal() # o
         self.restart         = Signal() # i
 
         # GTH signals
         self.plllock         = Signal() # i
         self.pllreset        = Signal() # o
@@ -58,18 +60,17 @@
         ]
 
         # PLL reset must be at least 2us
         pll_reset_cycles = ceil(2e-6*sys_clk_freq)
         pll_reset_timer  = WaitTimer(pll_reset_cycles)
         self.submodules += pll_reset_timer
 
-        fsm = ResetInserter()(FSM(reset_state="RESET_ALL"))
-        self.submodules.fsm = fsm
+        self.fsm = fsm = ResetInserter()(FSM(reset_state="RESET_ALL"))
 
-        ready_timer = WaitTimer(int(10e-3*sys_clk_freq))
+        ready_timer = WaitTimer(10e-3*sys_clk_freq)
         self.submodules += ready_timer
         self.comb += [
             ready_timer.wait.eq(~self.done & ~fsm.reset),
             fsm.reset.eq(self.restart | ready_timer.done)
         ]
 
         if rx:
```

### Comparing `liteiclink-2023.4/liteiclink/serdes/serdes_ecp5.py` & `liteiclink-2023.8/liteiclink/serdes/serdes_ecp5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2019-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import WaitTimer
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
+
 from litex.soc.interconnect.csr import *
 from litex.soc.interconnect import stream
 from litex.soc.cores.prbs import PRBSTX, PRBSRX
 from litex.soc.cores.code_8b10b import Encoder, Decoder
 
 # SerDesECP5PLL ------------------------------------------------------------------------------------
 
-class SerDesECP5PLL(Module):
+class SerDesECP5PLL(LiteXModule):
     def __init__(self, refclk, refclk_freq, linerate):
         self.refclk = refclk
         self.config = self.compute_config(refclk_freq, linerate)
 
     @staticmethod
     def compute_config(refclk_freq, linerate):
         multipliers = [8, 10, 16, 20]
@@ -77,15 +79,15 @@
            d        = config["d"],
            vco_freq = config["vco_freq"]/1e9,
            linerate = config["linerate"]/1e9)
         return r
 
 # SerDesSCI ----------------------------------------------------------------------------------------
 
-class SerDesECP5SCI(Module):
+class SerDesECP5SCI(LiteXModule):
     def __init__(self, serdes):
         self.dual_sel = Signal()
         self.chan_sel = Signal()
         self.re       = Signal()
         self.we       = Signal()
         self.done     = Signal()
         self.adr      = Signal(6)
@@ -96,15 +98,15 @@
 
         self.sci_rd    = sci_rd    = Signal()
         self.sci_wrn   = sci_wrn   = Signal(reset=1)
         self.sci_addr  = sci_addr  = Signal(6)
         self.sci_wdata = sci_wdata = Signal(8)
         self.sci_rdata = sci_rdata = Signal(8)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             self.done.eq(1),
             If(self.we,
                 NextState("WRITE")
             ).Elif(self.re,
                 sci_rd.eq(1),
                 NextState("READ")
@@ -133,15 +135,15 @@
              i_CHX_SCIEN   = self.chan_sel,
              i_CHX_SCISEL  = self.chan_sel,
              i_D_SCIRD     = sci_rd,
              i_D_SCIWSTN   = sci_wrn,
         )
 
 @ResetInserter()
-class SerDesECP5SCIReconfig(Module, AutoCSR):
+class SerDesECP5SCIReconfig(LiteXModule):
     def __init__(self, serdes):
         self.loopback    = Signal()
         self.rx_polarity = Signal()
         self.tx_idle     = Signal()
         self.tx_polarity = Signal()
         self.rx_cdr_hold = Signal()
 
@@ -152,21 +154,20 @@
         self.done  = CSRStatus(    description="Access is Done")
         self.adr   = CSRStorage(6, description="Access address")
         self.dat_w = CSRStorage(8, description="Access Write data")
         self.dat_r = CSRStatus(8,  description="Access Read data")
 
         # # #
 
-        sci = SerDesECP5SCI(serdes)
-        self.submodules.sci = sci
+        self.sci = sci = SerDesECP5SCI(serdes)
 
         first = Signal()
         data  = Signal(8)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             self.done.status.eq(1),
             If(self.pause.storage,
                 If(self.we.re,
                     NextState("WRITE")
                 ),
                 If(self.re.re,
@@ -289,15 +290,15 @@
 
         last_fsm_state = Signal(4)
         self.sync += last_fsm_state.eq(fsm.state)
         self.comb += first.eq(fsm.state != last_fsm_state)
 
 # SerdesInit ---------------------------------------------------------------------------------------
 
-class SerdesInit(Module):
+class SerdesInit(LiteXModule):
     def __init__(self, tx_lol, rx_lol, rx_los):
         self.rst     = Signal()
         self.tx_rst  = Signal()
         self.rx_rst  = Signal()
         self.pcs_rst = Signal()
         self.ready   = Signal()
 
@@ -312,15 +313,15 @@
 
         timer = WaitTimer(1024)
         self.submodules += timer
         self.comb += timer.wait.eq(~self.rst)
 
         fsm = FSM(reset_state="RESET-ALL")
         fsm = ResetInserter()(fsm)
-        self.submodules.fsm = fsm
+        self.fsm = fsm
         self.comb += fsm.reset.eq(self.rst)
         fsm.act("RESET-ALL",
             # Reset TX Serdes, RX Serdes and PCS.
             self.tx_rst.eq(1),
             self.rx_rst.eq(1),
             self.pcs_rst.eq(1),
             If(timer.done,
@@ -354,15 +355,15 @@
             If(_rx_los,
                 NextState("RESET-RX-PCS-WAIT-TX-PLL-LOCK")
             )
         )
 
 # SerDesECP5 ---------------------------------------------------------------------------------------
 
-class SerDesECP5(Module, AutoCSR):
+class SerDesECP5(LiteXModule):
     def __init__(self, pll, tx_pads, rx_pads,
         dual        = 0,
         channel     = 0,
         data_width  = 20,
         tx_polarity = 0,
         rx_polarity = 0):
         assert dual       in [0, 1]
@@ -394,16 +395,16 @@
         # Loopback
         self.loopback               = Signal() # FIXME: reconfigure lb_ctl to 0b0001 but does not seem enough
 
         # # #
 
         self.nwords = nwords = data_width//10
 
-        self.submodules.encoder  = ClockDomainsRenamer("tx")(Encoder(nwords, True))
-        self.submodules.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
+        self.encoder  = ClockDomainsRenamer("tx")(Encoder(nwords, True))
+        self.decoders = [ClockDomainsRenamer("rx")(Decoder(True)) for _ in range(nwords)]
 
         # Transceiver direct clock outputs (useful to specify clock constraints)
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
         self.tx_clk_freq = pll.config["linerate"]/data_width
         self.rx_clk_freq = pll.config["linerate"]/data_width
@@ -442,23 +443,23 @@
             MultiReg(self.rx_prbs_config, rx_prbs_config, "rx"),
             MultiReg(self.rx_prbs_pause, rx_prbs_pause, "rx"),
             MultiReg(rx_los, self.rx_idle, "sys"),
             MultiReg(rx_prbs_errors, self.rx_prbs_errors, "sys"),
         ]
 
         # DCU init ---------------------------------------------------------------------------------
-        self.submodules.init = init = SerdesInit(tx_lol, rx_lol, rx_los)
+        self.init = init = SerdesInit(tx_lol, rx_lol, rx_los)
 
         # Clocking ---------------------------------------------------------------------------------
-        self.clock_domains.cd_tx = ClockDomain()
+        self.cd_tx = ClockDomain()
         self.comb += self.cd_tx.clk.eq(self.txoutclk)
         self.specials += AsyncResetSynchronizer(self.cd_tx, ~init.ready)
         self.comb += self.tx_ready.eq(init.ready)
 
-        self.clock_domains.cd_rx = ClockDomain()
+        self.cd_rx = ClockDomain()
         self.comb += self.cd_rx.clk.eq(self.rxoutclk)
         self.specials += AsyncResetSynchronizer(self.cd_rx, ~init.ready)
         self.comb += self.rx_ready.eq(init.ready)
 
         # DCU instance -----------------------------------------------------------------------------
         self.serdes_params = dict(
             # ECP5's DCU parameters/signals/instance have been documented by whitequark as part of
@@ -669,26 +670,25 @@
             p_CHX_FF_TX_F_CLK_DIS   = "0b1",    # disable DIV/1 output clock
 
             # CHX TX — data
             **{"i_CHX_FF_TX_D_%d" % n: tx_bus[n] for n in range(tx_bus.nbits)}
         )
 
         # SCI Reconfiguration ----------------------------------------------------------------------
-        sci_reconfig = SerDesECP5SCIReconfig(self)
-        self.submodules.sci_reconfig = sci_reconfig
+        self.sci_reconfig = sci_reconfig = SerDesECP5SCIReconfig(self)
         self.comb += sci_reconfig.reset.eq(~self.init.ready)
         self.comb += sci_reconfig.sci.dual_sel.eq(dual)
         self.comb += sci_reconfig.loopback.eq(self.loopback)
         self.comb += sci_reconfig.tx_idle.eq(self.tx_idle)
         self.comb += sci_reconfig.rx_polarity.eq(rx_polarity)
         self.comb += sci_reconfig.tx_polarity.eq(tx_polarity)
         self.comb += sci_reconfig.rx_cdr_hold.eq(self.rx_cdr_hold)
 
         # TX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
+        self.tx_prbs = ClockDomainsRenamer("tx")(PRBSTX(data_width, reverse=True))
         self.comb += self.tx_prbs.config.eq(tx_prbs_config)
         self.comb += [
             self.tx_prbs.i.eq(Cat(*[self.encoder.output[i] for i in range(nwords)])),
             If(tx_produce_square_wave,
                 # square wave @ linerate/data_width for scope observation
                 tx_data.eq(Signal(data_width, reset=(1<<(data_width//2))-1))
             ).Elif(tx_produce_pattern,
@@ -697,15 +697,15 @@
                 tx_data.eq(self.tx_prbs.o)
             ),
             tx_bus[ 0:10].eq(tx_data[ 0:10]),
             tx_bus[12:22].eq(tx_data[10:20]),
         ]
 
         # RX Datapath and PRBS ---------------------------------------------------------------------
-        self.submodules.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
+        self.rx_prbs = ClockDomainsRenamer("rx")(PRBSRX(data_width, reverse=True))
         self.comb += [
             self.rx_prbs.config.eq(rx_prbs_config),
             self.rx_prbs.pause.eq(rx_prbs_pause),
             rx_prbs_errors.eq(self.rx_prbs.errors),
             rx_data[ 0:10].eq(rx_bus[ 0:10]),
             rx_data[10:20].eq(rx_bus[12:22]),
         ]
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/core.py` & `liteiclink-2023.8/liteiclink/serwb/core.py`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/liteiclink/serwb/datapath.py` & `liteiclink-2023.8/liteiclink/serwb/datapath.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.io import *
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import WaitTimer
 
 from litex.soc.interconnect import stream
 from litex.soc.cores.code_8b10b import K, StreamEncoder, StreamDecoder
 
 from liteiclink.serwb.scrambler import Scrambler, Descrambler
 
 # TXDatapath ---------------------------------------------------------------------------------------
@@ -56,26 +57,41 @@
         self.comb += If(idle,
             sink.ready.eq(0),
             converter.sink.valid.eq(1),
             converter.sink.data.eq(0),
         )
 
 # RXAligner ----------------------------------------------------------------------------------------
-
+"""
+RXAligner
+*********
+
+This module aligns the data stream. When shifting is enabled, this module stops
+forwarding data from `sink` to `source` while accepting and ignoring new data on the `sink`.
+
+This module guarantees the removal of one data element (phy_dw bits) from the stream
+when shift_inc is asserted for one cycle.
+
+There must be data on the stream between successive shift_inc operations, otherwise
+this module will shift less than expected.
+
+ * ``phy_dw`` the width of the data signal.
+ * ``shift_inc`` enable the shifting if != 0
+"""
 class RXAligner(Module):
-    def __init__(self, phy_dw, shift=None):
-        self.shift  = Signal() if shift is None else shift
+    def __init__(self, phy_dw, shift_inc=None):
+        self.shift_inc  = Signal() if shift_inc is None else shift_inc
         self.sink   = sink   = stream.Endpoint([("data", phy_dw)])
         self.source = source = stream.Endpoint([("data", phy_dw)])
 
         # # #
 
         _shift = Signal()
         self.sync += [
-            If(self.shift,
+            If(self.shift_inc,
                 _shift.eq(1),
             ).Elif(sink.valid & sink.ready,
                 _shift.eq(0),
             )
         ]
 
         self.comb += sink.connect(source)
@@ -85,24 +101,24 @@
         )
 
 
 # RXDatapath ---------------------------------------------------------------------------------------
 
 class RXDatapath(Module):
     def __init__(self, phy_dw, with_scrambling=False):
-        self.shift  = shift  = Signal(6)
+        self.shift_inc  = shift_inc  = Signal()
         self.sink   = sink   = stream.Endpoint([("data", phy_dw)])
         self.source = source = stream.Endpoint([("data", 32)])
         self.idle   = idle   = Signal()
         self.comma  = comma  = Signal()
 
         # # #
 
         # Aligner
-        self.submodules.aligner = aligner = RXAligner(phy_dw, shift)
+        self.submodules.aligner = aligner = RXAligner(phy_dw, shift_inc)
 
         # Converter
         self.submodules.converter = converter = stream.Converter(phy_dw, 40)
 
         # Line Coding
         self.submodules.decoder = decoder = StreamDecoder(nwords=4)
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/etherbone.py` & `liteiclink-2023.8/liteiclink/serwb/etherbone.py`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/liteiclink/serwb/genphy.py` & `liteiclink-2023.8/liteiclink/serwb/genphy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import WaitTimer
 
 from litex.build.io import *
 
+from litex.gen.genlib.misc import WaitTimer
+
 from litex.soc.interconnect import stream
 from litex.soc.interconnect.csr import *
 
 from liteiclink.serwb.datapath import TXDatapath, RXDatapath
 
 # SerDes Clocking ----------------------------------------------------------------------------------
 
@@ -97,26 +98,26 @@
             self.sync += data.eq(pads.rx)
 
         # Datapath
         self.submodules.datapath = datapath = RXDatapath(1)
         self.comb += [
             datapath.sink.valid.eq(1),
             datapath.sink.data.eq(data),
-            datapath.shift.eq(self.shift),
+            datapath.shift_inc.eq(self.shift),
             datapath.source.connect(source),
             idle.eq(datapath.idle),
             comma.eq(datapath.comma)
         ]
 
 # SerDes -------------------------------------------------------------------------------------------
 
 @ResetInserter()
 class _Serdes(Module):
     def __init__(self, pads, mode="master"):
-        if hasattr(pads, "clk"):
+        if hasattr(pads, "clk") or hasattr(pads, "clk_p"):
             self.submodules.clocking = _SerdesClocking(pads, mode)
         self.submodules.tx       = _SerdesTX(pads)
         self.submodules.rx       = _SerdesRX(pads)
 
 
 # SerDes Initialization/Synchronisation ------------------------------------------------------------
 #
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/kuserdes.py` & `liteiclink-2023.8/liteiclink/serwb/kuserdes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import BitSlip, WaitTimer
+
+from litex.gen.genlib.misc import BitSlip, WaitTimer
 
 from litex.build.io import *
 
 from litex.soc.interconnect import stream
 from litex.soc.cores.code_8b10b import Encoder, Decoder
 
 from liteiclink.serwb.datapath import TXDatapath, RXDatapath
@@ -98,15 +99,15 @@
 # KU SerDes RX -------------------------------------------------------------------------------------
 
 class _KUSerdesRX(Module):
     def __init__(self, pads):
         # Control
         self.delay_rst     = Signal()
         self.delay_inc     = Signal()
-        self.shift = shift = Signal(6)
+        self.shift_inc = shift_inc = Signal()
 
         # Status
         self.idle  = idle = Signal()
         self.comma = comma = Signal()
 
         # Datapath
         self.source = source = stream.Endpoint([("data", 32)])
@@ -154,15 +155,15 @@
         ]
 
         # Datapath
         self.submodules.datapath = datapath = RXDatapath(8)
         self.comb += [
             datapath.sink.valid.eq(1),
             datapath.sink.data.eq(data),
-            datapath.shift.eq(shift),
+            datapath.shift_inc.eq(shift_inc),
             datapath.source.connect(source),
             idle.eq(datapath.idle),
             comma.eq(datapath.comma)
         ]
 
 # KU SerDes ----------------------------------------------------------------------------------------
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/packet.py` & `liteiclink-2023.8/liteiclink/serwb/packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
-from migen.genlib.misc import WaitTimer
 
 from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
 
 from litex.soc.interconnect import stream
 
 # Layouts ------------------------------------------------------------------------------------------
 
 def phy_description(dw):
     layout = [("data", dw)]
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/phy.py` & `liteiclink-2023.8/liteiclink/serwb/phy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import WaitTimer
 
 from litex.soc.interconnect import stream
 from litex.soc.interconnect.csr import *
 
 from liteiclink.serwb.kuserdes import KUSerdes
 from liteiclink.serwb.s7serdes import S7Serdes
 
@@ -101,26 +102,26 @@
                     NextState("CHECK-SAMPLING-WINDOW")
                 ).Else(
                     NextState("INC-DELAY-SHIFT")
                 )
             ),
             serdes.tx.comma.eq(1)
         )
-        self.comb += serdes.rx.shift.eq(shift)
         fsm.act("INC-DELAY-SHIFT",
             NextState("WAIT-STABLE"),
             If(delay == (taps - 1),
                 If(shift == (40 - 1),
                     NextState("ERROR")
                 ).Else(
                     NextValue(delay_min_found, 0),
                     NextValue(delay_min,       0),
                     NextValue(delay_max_found, 0),
                     NextValue(delay_max,       0),
-                    NextValue(shift, shift + 1)
+                    NextValue(shift, shift + 1),
+                    serdes.rx.shift_inc.eq(1)
                 ),
                 NextValue(delay, 0),
                 serdes.rx.delay_rst.eq(1)
             ).Else(
                 NextValue(delay, delay + 1),
                 serdes.rx.delay_inc.eq(1)
             ),
@@ -167,15 +168,15 @@
         # # #
 
         self.delay           = delay           = Signal(max=taps)
         self.delay_min       = delay_min       = Signal(max=taps)
         self.delay_min_found = delay_min_found = Signal()
         self.delay_max       = delay_max       = Signal(max=taps)
         self.delay_max_found = delay_max_found = Signal()
-        self.shift         = shift         = Signal(max=40)
+        self.shift           = shift           = Signal(max=40)
 
         # Timer
         self.submodules.timer = timer = WaitTimer(timeout)
 
         # FSM
         self.submodules.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
@@ -220,26 +221,26 @@
                     NextState("CHECK-SAMPLING-WINDOW")
                 ).Else(
                     NextState("INC-DELAY-SHIFT")
                 )
             ),
             serdes.tx.idle.eq(1)
         )
-        self.comb += serdes.rx.shift.eq(shift)
         fsm.act("INC-DELAY-SHIFT",
             NextState("WAIT-STABLE"),
             If(delay == (taps - 1),
                 If(shift == (40 - 1),
                     NextState("ERROR")
                 ).Else(
                     NextValue(delay_min_found, 0),
                     NextValue(delay_min,       0),
                     NextValue(delay_max_found, 0),
                     NextValue(delay_max,       0),
-                    NextValue(shift, shift + 1)
+                    NextValue(shift, shift + 1),
+                    serdes.rx.shift_inc.eq(1)
                 ),
                 NextValue(delay, 0),
                 serdes.rx.delay_rst.eq(1)
             ).Else(
                 NextValue(delay, delay + 1),
                 serdes.rx.delay_inc.eq(1)
             ),
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/s7serdes.py` & `liteiclink-2023.8/liteiclink/serwb/s7serdes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # This file is part of LiteICLink.
 #
 # Copyright (c) 2017-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import BitSlip, WaitTimer
+
+from litex.gen.genlib.misc import BitSlip, WaitTimer
 
 from litex.build.io import *
 
 from litex.soc.interconnect import stream
 from litex.soc.cores.code_8b10b import Encoder, Decoder
 
 from liteiclink.serwb.datapath import TXDatapath, RXDatapath
@@ -114,27 +115,27 @@
 # S7 SerDes RX -------------------------------------------------------------------------------------
 
 class _S7SerdesRX(Module):
     def __init__(self, pads):
         # Control
         self.delay_rst     = Signal()
         self.delay_inc     = Signal()
-        self.shift         = Signal()
+        self.shift_inc     = Signal()
 
         # Status
         self.idle  = idle = Signal()
         self.comma = comma = Signal()
 
         # Datapath
         self.source = source = stream.Endpoint([("data", 32)])
 
         # # #
 
         _shift = Signal(3)
-        self.sync += If(self.shift, _shift.eq(_shift + 1))
+        self.sync += If(self.shift_inc, _shift.eq(_shift + 1))
 
         # Data input (DDR with sys4x)
         data_nodelay      = Signal()
         data_delayed      = Signal()
         self.data = data  = Signal(8)
         self.specials += [
             DifferentialInput(pads.rx_p, pads.rx_n, data_nodelay),
@@ -166,15 +167,15 @@
 
                 i_DDLY    = data_delayed,
                 i_CE1     = 1,
                 i_RST     = ResetSignal("sys"),
                 i_CLK     = ClockSignal("sys4x"),
                 i_CLKB    =~ClockSignal("sys4x"),
                 i_CLKDIV  = ClockSignal("sys"),
-                i_BITSLIP = self.shift,
+                i_BITSLIP = self.shift_inc,
                 o_Q8      = data[0],
                 o_Q7      = data[1],
                 o_Q6      = data[2],
                 o_Q5      = data[3],
                 o_Q4      = data[4],
                 o_Q3      = data[5],
                 o_Q2      = data[6],
@@ -183,15 +184,15 @@
         ]
 
         # Datapath
         self.submodules.datapath = datapath = RXDatapath(8)
         self.comb += [
             datapath.sink.valid.eq(1),
             datapath.sink.data.eq(data),
-            datapath.shift.eq(self.shift & (_shift == 0b111)),
+            datapath.shift_inc.eq(self.shift_inc & (_shift == 0b111)),
             datapath.source.connect(source),
             idle.eq(datapath.idle),
             comma.eq(datapath.comma)
         ]
 
 # S7 SerDes ----------------------------------------------------------------------------------------
```

### Comparing `liteiclink-2023.4/liteiclink/serwb/scrambler.py` & `liteiclink-2023.8/liteiclink/serwb/scrambler.py`

 * *Files identical despite different names*

### Comparing `liteiclink-2023.4/liteiclink.egg-info/PKG-INFO` & `liteiclink-2023.8/liteiclink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteiclink
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable Inter-Chip communication cores
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/liteiclink
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `liteiclink-2023.4/liteiclink.egg-info/SOURCES.txt` & `liteiclink-2023.8/liteiclink.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 liteiclink.egg-info/SOURCES.txt
 liteiclink.egg-info/dependency_links.txt
 liteiclink.egg-info/requires.txt
 liteiclink.egg-info/top_level.txt
 liteiclink/serdes/__init__.py
 liteiclink/serdes/clock_aligner.py
 liteiclink/serdes/common.py
+liteiclink/serdes/gth3_ultrascale.py
+liteiclink/serdes/gth4_ultrascale.py
 liteiclink/serdes/gth_ultrascale.py
 liteiclink/serdes/gth_ultrascale_init.py
 liteiclink/serdes/gtp_7series.py
 liteiclink/serdes/gtp_7series_init.py
 liteiclink/serdes/gtx_7series.py
 liteiclink/serdes/gtx_7series_init.py
 liteiclink/serdes/gty_ultrascale.py
```

### Comparing `liteiclink-2023.4/setup.py` & `liteiclink-2023.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(
     name="liteiclink",
-    version="2023.04",
+    version="2023.08",
     description="Small footprint and configurable Inter-Chip communication cores",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/liteiclink",
```

