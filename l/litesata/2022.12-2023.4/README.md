# Comparing `tmp/litesata-2022.12.tar.gz` & `tmp/litesata-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesata-2022.12.tar", last modified: Thu Apr 18 20:13:10 2024, max compression
+gzip compressed data, was "litesata-2023.4.tar", last modified: Thu Apr 18 20:13:34 2024, max compression
```

## Comparing `litesata-2022.12.tar` & `litesata-2023.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.705442 litesata-2022.12/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1745 2024-04-18 20:12:31.000000 litesata-2022.12/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)     5316 2024-04-18 20:13:10.705179 litesata-2022.12/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4955 2024-04-18 20:12:31.000000 litesata-2022.12/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.695559 litesata-2022.12/litesata/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7647 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.697517 litesata-2022.12/litesata/core/
--rw-r--r--   0 timkpaine   (501) staff       (20)      746 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/core/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10326 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/core/command.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    24128 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/core/link.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8055 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/core/transport.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.700359 litesata-2022.12/litesata/frontend/
--rw-r--r--   0 timkpaine   (501) staff       (20)      225 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/frontend/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5057 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/frontend/arbitration.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7922 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/frontend/bist.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6877 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/frontend/dma.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2555 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/frontend/identify.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11946 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/frontend/raid.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8795 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/gen.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.702359 litesata-2022.12/litesata/phy/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5063 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    38040 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/a7sataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6412 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/ctrl.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8289 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/datapath.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    35625 2024-04-18 20:12:31.000000 litesata-2022.12/litesata/phy/k7sataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    45714 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/uspsataphy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    37974 2024-04-18 20:12:45.000000 litesata-2022.12/litesata/phy/ussataphy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.704917 litesata-2022.12/litesata.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5316 2024-04-18 20:13:10.000000 litesata-2022.12/litesata.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      866 2024-04-18 20:13:10.000000 litesata-2022.12/litesata.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:13:10.000000 litesata-2022.12/litesata.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:13:10.000000 litesata-2022.12/litesata.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:13:10.000000 litesata-2022.12/litesata.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:13:10.705491 litesata-2022.12/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)      864 2024-04-18 20:13:06.000000 litesata-2022.12/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:10.704651 litesata-2022.12/test/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2695 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_bist.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5802 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_command.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2660 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_link.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4092 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_link_cont.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2124 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_link_crc.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2031 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_link_scrambler.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4076 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_mirroring.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3344 2024-04-18 20:12:31.000000 litesata-2022.12/test/test_striping.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.108341 litesata-2023.4/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1745 2024-04-18 20:12:31.000000 litesata-2023.4/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:34.108081 litesata-2023.4/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4955 2024-04-18 20:12:31.000000 litesata-2023.4/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.098056 litesata-2023.4/litesata/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7647 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.100089 litesata-2023.4/litesata/core/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      746 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10326 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/command.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    24128 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/core/link.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8055 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/core/transport.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.102157 litesata-2023.4/litesata/frontend/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      225 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5057 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/arbitration.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7922 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/bist.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6877 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/frontend/dma.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2555 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/identify.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11946 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/frontend/raid.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8795 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/gen.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.104809 litesata-2023.4/litesata/phy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5085 2024-04-18 20:13:25.000000 litesata-2023.4/litesata/phy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    38261 2024-04-18 20:13:25.000000 litesata-2023.4/litesata/phy/a7sataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6412 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/ctrl.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8289 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/datapath.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    35625 2024-04-18 20:12:31.000000 litesata-2023.4/litesata/phy/k7sataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    45714 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/uspsataphy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    37974 2024-04-18 20:12:45.000000 litesata-2023.4/litesata/phy/ussataphy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.107805 litesata-2023.4/litesata.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5315 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      866 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:13:34.000000 litesata-2023.4/litesata.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:13:34.108388 litesata-2023.4/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)      864 2024-04-18 20:13:31.000000 litesata-2023.4/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:13:34.107576 litesata-2023.4/test/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2695 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_bist.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5802 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_command.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2660 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4092 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_cont.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2124 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_crc.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2031 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_link_scrambler.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4076 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_mirroring.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3344 2024-04-18 20:12:31.000000 litesata-2023.4/test/test_striping.py
```

### Comparing `litesata-2022.12/LICENSE` & `litesata-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/PKG-INFO` & `litesata-2023.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesata
-Version: 2022.12
+Version: 2023.4
 Summary: Small footprint and configurable SATA core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litesata
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litesata-2022.12/README.md` & `litesata-2023.4/README.md`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/common.py` & `litesata-2023.4/litesata/common.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/core/__init__.py` & `litesata-2023.4/litesata/core/__init__.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/core/command.py` & `litesata-2023.4/litesata/core/command.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/core/link.py` & `litesata-2023.4/litesata/core/link.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/core/transport.py` & `litesata-2023.4/litesata/core/transport.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/frontend/arbitration.py` & `litesata-2023.4/litesata/frontend/arbitration.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/frontend/bist.py` & `litesata-2023.4/litesata/frontend/bist.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/frontend/dma.py` & `litesata-2023.4/litesata/frontend/dma.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/frontend/identify.py` & `litesata-2023.4/litesata/frontend/identify.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/frontend/raid.py` & `litesata-2023.4/litesata/frontend/raid.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/gen.py` & `litesata-2023.4/litesata/gen.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/phy/__init__.py` & `litesata-2023.4/litesata/phy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - Transceiver and clocking (vendor specific)
     - Control (vendor agnostic)
     - Datapath (vendor agnostic)
 
     For now, the Kintex7/Zynq(with PL based on K7) PHY is the only one available,
     but the achitecture is modular enough to accept others PHYs.
     """
-    def __init__(self, device, pads, gen, clk_freq, refclk=None, data_width=16, with_csr=True):
+    def __init__(self, device, pads, gen, clk_freq, refclk=None, data_width=16, qpll=None, with_csr=True):
         self.pads   = pads
         self.gen    = gen
         self.refclk = refclk
 
         # Control/Status
         self.enable = Signal()
         self.ready  = Signal()
@@ -37,15 +37,15 @@
             from litesata.phy.k7sataphy import K7LiteSATAPHYCRG, K7LiteSATAPHY
             self.submodules.phy = K7LiteSATAPHY(pads, gen, clk_freq, data_width)
             self.submodules.crg = K7LiteSATAPHYCRG(refclk, pads, self.phy, gen)
 
         # Artix7
         elif re.match("^xc7a", device):
             from litesata.phy.a7sataphy import A7LiteSATAPHYCRG, A7LiteSATAPHY
-            self.submodules.phy = A7LiteSATAPHY(pads, gen, clk_freq, data_width, tx_buffer_enable=True)
+            self.submodules.phy = A7LiteSATAPHY(pads, gen, clk_freq, data_width, tx_buffer_enable=True, qpll=qpll)
             self.submodules.crg = A7LiteSATAPHYCRG(refclk, pads, self.phy, gen,  tx_buffer_enable=True)
 
         # Kintex/Virtex Ultrascale
         elif re.match("^xc[kv]u[0-9]+-", device):
             from litesata.phy.ussataphy import USLiteSATAPHYCRG, USLiteSATAPHY
             self.submodules.phy = USLiteSATAPHY(pads, gen, clk_freq, data_width)
             self.submodules.crg = USLiteSATAPHYCRG(refclk, pads, self.phy, gen)
```

### Comparing `litesata-2022.12/litesata/phy/a7sataphy.py` & `litesata-2023.4/litesata/phy/a7sataphy.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             AsyncResetSynchronizer(self.cd_sata_tx, ~gtp.qplllock | self.tx_reset),
             AsyncResetSynchronizer(self.cd_sata_rx, ~gtp.qplllock | self.rx_reset)
         ]
 
 # --------------------------------------------------------------------------------------------------
 
 class A7LiteSATAPHY(Module):
-    def __init__(self, pads, gen, clk_freq, data_width=16, tx_buffer_enable=False, rx_buffer_enable=False):
+    def __init__(self, pads, gen, clk_freq, data_width=16, tx_buffer_enable=False, rx_buffer_enable=False, qpll=None):
         assert data_width in [16, 32]
         # Common signals
         self.data_width     = data_width
 
         # Control
         self.ready          = Signal() # o
 
@@ -236,17 +236,19 @@
 
         # QPLL ------------------------------------------------------------------------------------
         linerate_config = {
             "gen1": 1.5e9,
             "gen2": 3.0e9,
             "gen3": 6.0e9
         }
-        self.submodules.qpll = GTPQuadPLL(self.gtrefclk0, 150e6, linerate_config[gen])
-        self.comb += self.qplllock.eq(self.qpll.lock)
-        self.comb += self.qpll.reset.eq(tx_init.pllreset)
+        if qpll is None:
+            self.submodules.qpll = qpll = GTPQuadPLL(self.gtrefclk0, 150e6, linerate_config[gen])
+            qpll.index = 0
+        self.comb += self.qplllock.eq(qpll.lock)
+        self.comb += qpll.reset.eq(tx_init.pllreset)
 
         # OOB clock (75MHz) ------------------------------------------------------------------------
         oobclk = Signal()
         self.specials += Instance("FDPE",
             p_INIT = 1,
             i_CE   = 1,
             i_PRE  = 0,
@@ -581,25 +583,25 @@
             i_DRPDI                = rx_init.drp.di,
             o_DRPDO                = rx_init.drp.do,
             i_DRPEN                = rx_init.drp.en,
             o_DRPRDY               = rx_init.drp.rdy,
             i_DRPWE                = rx_init.drp.we,
 
             # Clocking Ports
-            i_RXSYSCLKSEL          = 0b00,
-            i_TXSYSCLKSEL          = 0b00,
+            i_RXSYSCLKSEL          = {0: 0b00, 1: 0b11}[qpll.index],
+            i_TXSYSCLKSEL          = {0: 0b00, 1: 0b11}[qpll.index],
 
             # FPGA TX Interface Datapath Configuration
             i_TX8B10BEN            = 1,
 
             # GTPE2_CHANNEL Clocking Ports
-            i_PLL0CLK              = self.qpll.clk,
-            i_PLL0REFCLK           = self.qpll.refclk,
-            i_PLL1CLK              = 0,
-            i_PLL1REFCLK           = 0,
+            i_PLL0CLK              = {0: qpll.clk,    1: 0}[qpll.index],
+            i_PLL0REFCLK           = {0: qpll.refclk, 1: 0}[qpll.index],
+            i_PLL1CLK              = {0: 0, 1: qpll.clk,  }[qpll.index],
+            i_PLL1REFCLK           = {0: 0, 1: qpll.refclk}[qpll.index],
 
             # Loopback Ports
             i_LOOPBACK             = 0b000,
 
             # PCI Express Ports
             o_PHYSTATUS            = Open(),
             i_RXRATE               = 0,
```

### Comparing `litesata-2022.12/litesata/phy/ctrl.py` & `litesata-2023.4/litesata/phy/ctrl.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/phy/datapath.py` & `litesata-2023.4/litesata/phy/datapath.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/phy/k7sataphy.py` & `litesata-2023.4/litesata/phy/k7sataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/phy/uspsataphy.py` & `litesata-2023.4/litesata/phy/uspsataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata/phy/ussataphy.py` & `litesata-2023.4/litesata/phy/ussataphy.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/litesata.egg-info/PKG-INFO` & `litesata-2023.4/litesata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesata
-Version: 2022.12
+Version: 2023.4
 Summary: Small footprint and configurable SATA core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litesata
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litesata-2022.12/litesata.egg-info/SOURCES.txt` & `litesata-2023.4/litesata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/setup.py` & `litesata-2023.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = fp.read()
 
 setup(
     name="litesata",
     description="Small footprint and configurable SATA core",
     long_description              = long_description,
     long_description_content_type = "text/markdown",
-    version="2022.12",
+    version="2023.04",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/litesata",
     test_suite="test",
     license="BSD",
     python_requires="~=3.6",
```

### Comparing `litesata-2022.12/test/test_bist.py` & `litesata-2023.4/test/test_bist.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_command.py` & `litesata-2023.4/test/test_command.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_link.py` & `litesata-2023.4/test/test_link.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_link_cont.py` & `litesata-2023.4/test/test_link_cont.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_link_crc.py` & `litesata-2023.4/test/test_link_crc.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_link_scrambler.py` & `litesata-2023.4/test/test_link_scrambler.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_mirroring.py` & `litesata-2023.4/test/test_mirroring.py`

 * *Files identical despite different names*

### Comparing `litesata-2022.12/test/test_striping.py` & `litesata-2023.4/test/test_striping.py`

 * *Files identical despite different names*

