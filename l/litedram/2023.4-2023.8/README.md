# Comparing `tmp/litedram-2023.4.tar.gz` & `tmp/litedram-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litedram-2023.4.tar", last modified: Sun Sep 17 22:02:02 2023, max compression
+gzip compressed data, was "litedram-2023.8.tar", last modified: Sun Sep 17 22:02:24 2023, max compression
```

## Comparing `litedram-2023.4.tar` & `litedram-2023.8.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.697567 litedram-2023.4/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2651 2023-09-17 21:44:26.000000 litedram-2023.4/CONTRIBUTORS
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1764 2023-09-17 21:44:26.000000 litedram-2023.4/LICENSE
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       91 2023-09-17 21:44:26.000000 litedram-2023.4/MANIFEST.in
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5110 2023-09-17 22:02:02.697567 litedram-2023.4/PKG-INFO
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4339 2023-09-17 21:44:26.000000 litedram-2023.4/README.md
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.689567 litedram-2023.4/doc/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4211 2023-09-17 21:44:26.000000 litedram-2023.4/doc/architecture.dia
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    35801 2023-09-17 21:44:26.000000 litedram-2023.4/doc/architecture.png
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4280 2023-09-17 21:44:26.000000 litedram-2023.4/doc/enjoy_digital.png
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    74067 2023-09-17 21:44:26.000000 litedram-2023.4/doc/litedram_logo_full.png
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    93603 2023-09-17 21:44:26.000000 litedram-2023.4/doc/litedram_logo_full.svg
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.689567 litedram-2023.4/litedram/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15147 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/common.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.689567 litedram-2023.4/litedram/core/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1431 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/core/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3178 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/core/bandwidth.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9594 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/core/bankmachine.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3988 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/core/controller.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9762 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/core/crossbar.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16755 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/core/multiplexer.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9992 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/core/refresher.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4850 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/dfii.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.693567 litedram-2023.4/litedram/frontend/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16612 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/adapter.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14786 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/axi.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    26689 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/bist.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10049 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/frontend/dma.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7150 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/ecc.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14510 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/fifo.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2977 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/frontend/wishbone.py
--rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    38251 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/gen.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    39699 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/init.py
--rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    47108 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/modules.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.693567 litedram-2023.4/litedram/phy/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      512 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14408 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/dfi.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    19836 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/phy/ecp5ddrphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6961 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/gensdrphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    20430 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/phy/gw2ddrphy.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.693567 litedram-2023.4/litedram/phy/lpddr4/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    13324 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/README.md
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      255 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18491 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/basephy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8969 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/commands.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10708 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/s7phy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    23061 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/sim.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6681 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/simphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15323 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr4/simsoc.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.697567 litedram-2023.4/litedram/phy/lpddr5/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      203 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/__init__.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    24623 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/basephy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12637 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/commands.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12092 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/s7phy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    35713 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/sim.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5201 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/simphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    17396 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/lpddr5/simsoc.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    25302 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/model.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.697567 litedram-2023.4/litedram/phy/rpc/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4273 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/README.md
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/__init__.py
--rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    17842 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/phy/rpc/arty.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    27423 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/phy/rpc/basephy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9617 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/commands.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8710 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/s7phy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9857 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/simphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14359 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/rpc/simsoc.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18237 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/s6ddrphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5869 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/s7common.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    26309 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/s7ddrphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11517 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/sim_utils.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    23841 2023-09-17 22:01:55.000000 litedram-2023.4/litedram/phy/usddrphy.py
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12569 2023-09-17 21:44:26.000000 litedram-2023.4/litedram/phy/utils.py
-drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:02.689567 litedram-2023.4/litedram.egg-info/
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5110 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/PKG-INFO
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1845 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/SOURCES.txt
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        1 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/dependency_links.txt
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       51 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/entry_points.txt
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       55 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/requires.txt
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        9 2023-09-17 22:02:02.000000 litedram-2023.4/litedram.egg-info/top_level.txt
--rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       38 2023-09-17 22:02:02.697567 litedram-2023.4/setup.cfg
--rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     1424 2023-09-17 21:44:26.000000 litedram-2023.4/setup.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.074105 litedram-2023.8/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2651 2023-09-17 21:44:26.000000 litedram-2023.8/CONTRIBUTORS
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1764 2023-09-17 21:44:26.000000 litedram-2023.8/LICENSE
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       91 2023-09-17 21:44:26.000000 litedram-2023.8/MANIFEST.in
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5110 2023-09-17 22:02:24.074105 litedram-2023.8/PKG-INFO
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4339 2023-09-17 21:44:26.000000 litedram-2023.8/README.md
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.066105 litedram-2023.8/doc/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4211 2023-09-17 21:44:26.000000 litedram-2023.8/doc/architecture.dia
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    35801 2023-09-17 21:44:26.000000 litedram-2023.8/doc/architecture.png
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4280 2023-09-17 21:44:26.000000 litedram-2023.8/doc/enjoy_digital.png
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    74067 2023-09-17 21:44:26.000000 litedram-2023.8/doc/litedram_logo_full.png
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    93603 2023-09-17 21:44:26.000000 litedram-2023.8/doc/litedram_logo_full.svg
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.070105 litedram-2023.8/litedram/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15188 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/common.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.070105 litedram-2023.8/litedram/core/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1497 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/core/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3178 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/core/bandwidth.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10009 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/core/bankmachine.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3988 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/core/controller.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9762 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/core/crossbar.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16755 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/core/multiplexer.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9997 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/core/refresher.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5732 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/dfii.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.070105 litedram-2023.8/litedram/frontend/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16612 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/adapter.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8578 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/frontend/avalon.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14786 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/axi.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    26689 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/bist.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9914 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/frontend/dma.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7150 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/ecc.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14510 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/fifo.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2977 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/frontend/wishbone.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    40339 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/gen.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    41481 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/init.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    47446 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/modules.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.074105 litedram-2023.8/litedram/phy/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      512 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14408 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/dfi.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    19802 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/phy/ecp5ddrphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6961 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/gensdrphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    20140 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/phy/gw2ddrphy.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.074105 litedram-2023.8/litedram/phy/lpddr4/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    13324 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/README.md
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      255 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18491 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/basephy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8969 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/commands.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10708 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/s7phy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    23061 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/sim.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6681 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/simphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15323 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr4/simsoc.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.074105 litedram-2023.8/litedram/phy/lpddr5/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      203 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    24623 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/basephy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12637 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/commands.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12092 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/s7phy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    35713 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/sim.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5201 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/simphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    17396 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/lpddr5/simsoc.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    25302 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/model.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.074105 litedram-2023.8/litedram/phy/rpc/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4273 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/README.md
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/__init__.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    17827 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/phy/rpc/arty.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    27428 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/phy/rpc/basephy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9617 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/commands.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8710 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/s7phy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9857 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/simphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14359 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/rpc/simsoc.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18237 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/s6ddrphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5869 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/s7common.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    26309 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/s7ddrphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11517 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/sim_utils.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    23967 2023-09-17 22:02:13.000000 litedram-2023.8/litedram/phy/usddrphy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12569 2023-09-17 21:44:26.000000 litedram-2023.8/litedram/phy/utils.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 22:02:24.070105 litedram-2023.8/litedram.egg-info/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5110 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/PKG-INFO
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1873 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/SOURCES.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        1 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/dependency_links.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       51 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/entry_points.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       55 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/requires.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        9 2023-09-17 22:02:24.000000 litedram-2023.8/litedram.egg-info/top_level.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       38 2023-09-17 22:02:24.074105 litedram-2023.8/setup.cfg
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     1424 2023-09-17 22:02:20.000000 litedram-2023.8/setup.py
```

### Comparing `litedram-2023.4/CONTRIBUTORS` & `litedram-2023.8/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/LICENSE` & `litedram-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/PKG-INFO` & `litedram-2023.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litedram
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable DRAM core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litedram
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `litedram-2023.4/README.md` & `litedram-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/doc/architecture.dia` & `litedram-2023.8/doc/architecture.dia`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/doc/architecture.png` & `litedram-2023.8/doc/architecture.png`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/doc/enjoy_digital.png` & `litedram-2023.8/doc/enjoy_digital.png`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/doc/litedram_logo_full.png` & `litedram-2023.8/doc/litedram_logo_full.png`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/doc/litedram_logo_full.svg` & `litedram-2023.8/doc/litedram_logo_full.svg`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/common.py` & `litedram-2023.8/litedram/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,15 @@
             bitslips: int = 0,  # number of write/read bitslip taps
             delays: int = 0,  # number of write/read delay taps
             # PHY training capabilities
             write_leveling: bool = False,
             write_dq_dqs_training: bool = False,
             write_latency_calibration: bool = False,
             read_leveling: bool = False,
+            is_clam_shell: bool = False,
         ):
         if strobes is None:
             strobes = databits // 8
         self.set_attributes(locals())
         self.cwl = cl if cwl is None else cwl
         self.is_rdimm = False
```

### Comparing `litedram-2023.4/litedram/core/__init__.py` & `litedram-2023.8/litedram/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 from litedram.core.crossbar import LiteDRAMCrossbar
 
 # Core ---------------------------------------------------------------------------------------------
 
 class LiteDRAMCore(Module, AutoCSR):
     def __init__(self, phy, geom_settings, timing_settings, clk_freq, **kwargs):
         self.submodules.dfii = DFIInjector(
-            addressbits = max(geom_settings.addressbits, getattr(phy, "addressbits", 0)),
-            bankbits    = max(geom_settings.bankbits, getattr(phy, "bankbits", 0)),
-            nranks      = phy.settings.nranks,
-            databits    = phy.settings.dfi_databits,
-            nphases     = phy.settings.nphases)
+            addressbits   = max(geom_settings.addressbits, getattr(phy, "addressbits", 0)),
+            bankbits      = max(geom_settings.bankbits, getattr(phy, "bankbits", 0)),
+            nranks        = phy.settings.nranks,
+            databits      = phy.settings.dfi_databits,
+            nphases       = phy.settings.nphases,
+            is_clam_shell = phy.settings.is_clam_shell)
         self.comb += self.dfii.master.connect(phy.dfi)
 
         self.submodules.controller = controller = LiteDRAMController(
             phy_settings    = phy.settings,
             geom_settings   = geom_settings,
             timing_settings = timing_settings,
             clk_freq        = clk_freq,
```

### Comparing `litedram-2023.4/litedram/core/bandwidth.py` & `litedram-2023.8/litedram/core/bandwidth.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/core/bankmachine.py` & `litedram-2023.8/litedram/core/bankmachine.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,27 @@
 
     def row(self, address):
         split = self.colbits - self.address_align
         return address[split:]
 
     def col(self, address):
         split = self.colbits - self.address_align
-        return Cat(Replicate(0, self.address_align), address[:split])
+        if self.colbits > 10:
+            # A10 is reserved for auto-precharge, this bit needs to be skipped for col addresses.
+            return Cat(
+                Replicate(0, self.address_align),
+                address[:10-self.address_align],
+                Replicate(0, 1),
+                address[10-self.address_align:split]
+            )
+        else:
+            return Cat(
+                Replicate(0, self.address_align),
+                address[:split]
+            )
 
 # BankMachine --------------------------------------------------------------------------------------
 
 class BankMachine(Module):
     """Converts requests from ports into DRAM commands
 
     BankMachine abstracts single DRAM bank by keeping track of the currently
```

### Comparing `litedram-2023.4/litedram/core/controller.py` & `litedram-2023.8/litedram/core/controller.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/core/crossbar.py` & `litedram-2023.8/litedram/core/crossbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 address_width = port.address_width,
                 data_width    = port.data_width,
                 clock_domain  = clock_domain,
                 id            = port.id)
             self.submodules += LiteDRAMNativePortCDC(new_port, port)
             port = new_port
 
-        # Data width convertion --------------------------------------------------------------------
+        # Data width conversion --------------------------------------------------------------------
         if data_width != self.controller.data_width:
             if data_width > self.controller.data_width:
                 addr_shift = -log2_int(data_width//self.controller.data_width)
             else:
                 addr_shift = log2_int(self.controller.data_width//data_width)
             new_port = LiteDRAMNativePort(
                 mode          = mode,
```

### Comparing `litedram-2023.4/litedram/core/multiplexer.py` & `litedram-2023.8/litedram/core/multiplexer.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/core/refresher.py` & `litedram-2023.8/litedram/core/refresher.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Copyright (c) 2016-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2015 Sebastien Bourdeauducq <sb@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
 """LiteDRAM Refresher."""
 
 from migen import *
-from migen.genlib.misc import timeline
+
+from litex.gen.genlib.misc import timeline
 
 from litex.soc.interconnect import stream
 
 from litedram.core.multiplexer import *
 
 # RefreshExecuter ----------------------------------------------------------------------------------
```

### Comparing `litedram-2023.4/litedram/dfii.py` & `litedram-2023.8/litedram/dfii.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,38 @@
         self._command       = CSRStorage(fields=[
             CSRField("cs",   size=1, description="DFI chip select bus"),
             CSRField("we",   size=1, description="DFI write enable bus"),
             CSRField("cas",  size=1, description="DFI column address strobe bus"),
             CSRField("ras",  size=1, description="DFI row address strobe bus"),
             CSRField("wren", size=1, description="DFI write data enable bus"),
             CSRField("rden", size=1, description="DFI read data enable bus"),
+            # Separate cs for clam shell topology
+            CSRField("cs_top",   size=1, description="DFI chip select bus for top half only"),
+            CSRField("cs_bottom",   size=1, description="DFI chip select bus for bottom half only"),
         ], description="Control DFI signals on a single phase")
 
         self._command_issue = CSR() # description="The command gets commited on a write to this register"
         self._address       = CSRStorage(len(phase.address), reset_less=True,  description="DFI address bus")
         self._baddress      = CSRStorage(len(phase.bank),    reset_less=True,  description="DFI bank address bus")
         self._wrdata        = CSRStorage(len(phase.wrdata),  reset_less=True,  description="DFI write data bus")
         self._rddata        = CSRStatus(len(phase.rddata), description="DFI read data bus")
 
         # # #
 
         self.comb += [
             If(self._command_issue.re,
-                phase.cs_n.eq(Replicate(~self._command.fields.cs, len(phase.cs_n))),
+                If(self._command.fields.cs_top,
+                    phase.cs_n.eq(2), # cs_n=0b10
+                ).Else(
+                    If(self._command.fields.cs_bottom,
+                        phase.cs_n.eq(1), # cs_n=0b01
+                    ).Else(
+                        phase.cs_n.eq(Replicate(~self._command.fields.cs, len(phase.cs_n))),
+                    ),
+                ),
                 phase.we_n.eq(~self._command.fields.we),
                 phase.cas_n.eq(~self._command.fields.cas),
                 phase.ras_n.eq(~self._command.fields.ras)
             ).Else(
                 phase.cs_n.eq(Replicate(1, len(phase.cs_n))),
                 phase.we_n.eq(1),
                 phase.cas_n.eq(1),
@@ -51,18 +62,18 @@
             phase.wrdata_mask.eq(0)
         ]
         self.sync += If(phase.rddata_valid, self._rddata.status.eq(phase.rddata))
 
 # DFIInjector --------------------------------------------------------------------------------------
 
 class DFIInjector(Module, AutoCSR):
-    def __init__(self, addressbits, bankbits, nranks, databits, nphases=1):
+    def __init__(self, addressbits, bankbits, nranks, databits, nphases=1, is_clam_shell=False):
         self.slave   = dfi.Interface(addressbits, bankbits, nranks, databits, nphases)
-        self.master  = dfi.Interface(addressbits, bankbits, nranks, databits, nphases)
-        csr_dfi      = dfi.Interface(addressbits, bankbits, nranks, databits, nphases)
+        self.master  = dfi.Interface(addressbits, bankbits, nranks*2 if is_clam_shell else nranks, databits, nphases)
+        csr_dfi      = dfi.Interface(addressbits, bankbits, nranks*2 if is_clam_shell else nranks, databits, nphases)
 
         self.ext_dfi     = dfi.Interface(addressbits, bankbits, nranks, databits, nphases)
         self.ext_dfi_sel = Signal()
 
         self._control = CSRStorage(fields=[
             CSRField("sel",     size=1, values=[
                 ("``0b0``", "Software (CPU) control."),
@@ -83,15 +94,19 @@
             # -----------------
             If(self._control.fields.sel,
                 # Through External DFI.
                 If(self.ext_dfi_sel,
                     self.ext_dfi.connect(self.master)
                 # Through LiteDRAM controller.
                 ).Else(
-                    self.slave.connect(self.master)
+                    self.slave.connect(self.master),
+                    # Broadcast cs_n for clam shell topology
+                    If(is_clam_shell,
+                        [self.master.phases[i].cs_n.eq(Replicate(self.slave.phases[i].cs_n, 2)) for i in range(nphases)],
+                    )
                 )
             # Software Control (through CSRs).
             # --------------------------------
             ).Else(
                 csr_dfi.connect(self.master)
             )
         ]
```

### Comparing `litedram-2023.4/litedram/frontend/adapter.py` & `litedram-2023.8/litedram/frontend/adapter.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/frontend/axi.py` & `litedram-2023.8/litedram/frontend/axi.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/frontend/bist.py` & `litedram-2023.8/litedram/frontend/bist.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/frontend/dma.py` & `litedram-2023.8/litedram/frontend/dma.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,53 +66,50 @@
         if is_native:
             (cmd, rdata) = port.cmd, port.rdata
         elif is_axi:
             (cmd, rdata) = port.ar, port.r
         else:
             raise NotImplementedError
 
+        # Reservation FIFO -------------------------------------------------------------------------
+
+        res_fifo = stream.SyncFIFO([("dummy", 1)], fifo_depth)
+        self.submodules += res_fifo
+
         # Request issuance -------------------------------------------------------------------------
-        request_enable = Signal()
-        request_issued = Signal()
 
         if is_native:
             self.comb += cmd.we.eq(0)
         if is_axi:
             self.comb += cmd.size.eq(int(log2(port.data_width//8)))
         self.comb += [
             cmd.addr.eq(sink.address),
-            cmd.valid.eq(enable & sink.valid & request_enable),
-            sink.ready.eq(enable & cmd.ready & request_enable),
-            request_issued.eq(cmd.valid & cmd.ready)
+            cmd.last.eq(sink.last),
+            cmd.valid.eq(enable & sink.valid & res_fifo.sink.ready),
+            sink.ready.eq(enable & cmd.ready & res_fifo.sink.ready),
         ]
-
-        # FIFO reservation level counter -----------------------------------------------------------
-        # - Incremented when data is planned to be queued.
-        # - Decremented when data is dequeued.
-        data_dequeued = Signal()
-        self.rsv_level = rsv_level = Signal(max=fifo_depth+1)
-        self.sync += [
-            If(request_issued,
-                If(~data_dequeued, rsv_level.eq(self.rsv_level + 1))
-            ).Elif(data_dequeued,
-                rsv_level.eq(rsv_level - 1)
-            )
+        self.comb += [
+            res_fifo.sink.valid.eq(cmd.valid & cmd.ready),
+            res_fifo.sink.last.eq(cmd.last),
         ]
-        self.comb += request_enable.eq(rsv_level != fifo_depth)
 
         # FIFO -------------------------------------------------------------------------------------
         fifo = stream.SyncFIFO([("data", port.data_width)], fifo_depth, fifo_buffered)
         self.submodules += fifo
 
         self.comb += [
             rdata.connect(fifo.sink, omit={"id", "resp", "dest", "user"}),
-            fifo.source.connect(source, omit={"ready"}),
+            fifo.source.connect(source, omit={"valid", "ready", "last"}),
+            If(res_fifo.source.valid,
+                source.valid.eq(fifo.source.valid),
+                source.last.eq(res_fifo.source.last),
+            ),
             fifo.source.ready.eq(source.ready | ~enable), # Flush FIFO/Reservation counter when disabled.
-            data_dequeued.eq(fifo.source.valid & fifo.source.ready)
         ]
+        self.comb += res_fifo.source.ready.eq(fifo.source.valid & fifo.source.ready)
 
         if with_csr:
             self.add_csr()
 
     def add_csr(self, default_base=0, default_length=0, default_enable=0, default_loop=0):
         self._base   = CSRStorage(32, reset=default_base)
         self._length = CSRStorage(32, reset=default_length)
```

### Comparing `litedram-2023.4/litedram/frontend/ecc.py` & `litedram-2023.8/litedram/frontend/ecc.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/frontend/fifo.py` & `litedram-2023.8/litedram/frontend/fifo.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/frontend/wishbone.py` & `litedram-2023.8/litedram/frontend/wishbone.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/gen.py` & `litedram-2023.8/litedram/gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,28 @@
 from litex.build.lattice import LatticePlatform
 from litex.build.sim import SimPlatform
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.interconnect import wishbone
+from litex.soc.interconnect import avalon
 from litex.soc.cores.uart import *
 
 from litedram import modules as litedram_modules
 from litedram import phy as litedram_phys
 from litedram.phy.ecp5ddrphy import ECP5DDRPHY
 from litedram.phy.s7ddrphy import S7DDRPHY
 from litedram.phy.model import SDRAMPHYModel
 
 from litedram.core.controller import ControllerSettings
 
 from litedram.frontend.axi import *
 from litedram.frontend.wishbone import *
+from litedram.frontend.avalon import *
 from litedram.frontend.bist import LiteDRAMBISTGenerator
 from litedram.frontend.bist import LiteDRAMBISTChecker
 from litedram.frontend.fifo import LiteDRAMFIFO
 from litedram.frontend.ecc import LiteDRAMNativePortECC
 
 # IOs/Interfaces -----------------------------------------------------------------------------------
 
@@ -211,14 +213,29 @@
             Subsignal("stb",   Pins(1)),
             Subsignal("ack",   Pins(1)),
             Subsignal("we",    Pins(1)),
             Subsignal("err",   Pins(1)),
         ),
     ]
 
+def get_avalon_user_port_ios(_id, aw, dw):
+    return [
+        ("user_port_{}".format(_id), 0,
+            Subsignal("address",          Pins(aw)),
+            Subsignal("writedata",        Pins(dw)),
+            Subsignal("readdata",         Pins(dw)),
+            Subsignal("readdatavalid",    Pins(1)),
+            Subsignal("byteenable",       Pins(dw//8)),
+            Subsignal("read",             Pins(1)),
+            Subsignal("write",            Pins(1)),
+            Subsignal("waitrequest",      Pins(1)),
+            Subsignal("burstcount",       Pins(8)),
+        ),
+    ]
+
 def get_axi_user_port_ios(_id, aw, dw, iw):
     return [
         ("user_port_{}".format(_id), 0,
             # aw
             Subsignal("awvalid", Pins(1)),
             Subsignal("awready", Pins(1)),
             Subsignal("awaddr",  Pins(aw)),
@@ -663,15 +680,15 @@
             if port.get("block_until_ready", True):
                 self.sync += user_enable.eq(self.ddrctrl.init_done.storage & ~self.ddrctrl.init_error.storage)
             # Else never block.
             else:
                 self.comb += user_enable.eq(1)
 
             # Request user port on crossbar and add optional ECC.
-            if port["type"] in ["native", "wishbone", "axi"]:
+            if port["type"] in ["native", "wishbone", "avalon", "axi"]:
                 # With ECC.
                 if port.get("ecc", False):
                     assert port.get("data_width", None) is not None
                     ecc_port  = self.sdram.crossbar.get_port()
                     user_port = LiteDRAMNativePort(
                         mode          = ecc_port.mode,
                         address_width = ecc_port.address_width,
@@ -725,14 +742,36 @@
                     wb_port.sel.eq(_wb_port_io.sel),
                     wb_port.cyc.eq(_wb_port_io.cyc & user_enable),
                     wb_port.stb.eq(_wb_port_io.stb & user_enable),
                     _wb_port_io.ack.eq(wb_port.ack & user_enable),
                     wb_port.we.eq(_wb_port_io.we),
                     _wb_port_io.err.eq(wb_port.err),
                 ]
+            # Avalon -----------------------------------------------------------------------------
+            elif port["type"] == "avalon":
+                avalon_port = avalon.AvalonMMInterface(
+                    user_port.data_width,
+                    user_port.address_width)
+                avalon2native = LiteDRAMAvalonMM2Native(avalon_port, user_port)
+                self.submodules += avalon2native
+                platform.add_extension(get_avalon_user_port_ios(name,
+                        len(avalon_port.address),
+                        len(avalon_port.writedata)))
+                _avalon_port_io = platform.request("user_port_{}".format(name))
+                self.comb += [
+                    avalon_port.address.eq(_avalon_port_io.address),
+                    avalon_port.writedata.eq(_avalon_port_io.writedata),
+                    _avalon_port_io.readdata.eq(avalon_port.readdata),
+                    _avalon_port_io.readdatavalid.eq(avalon_port.readdatavalid),
+                    avalon_port.burstcount.eq(_avalon_port_io.burstcount),
+                    avalon_port.byteenable.eq(_avalon_port_io.byteenable),
+                    avalon_port.write.eq(_avalon_port_io.write & user_enable),
+                    avalon_port.read.eq(_avalon_port_io.read & user_enable),
+                    _avalon_port_io.waitrequest.eq(avalon_port.waitrequest | ~user_enable),
+                ]
             # AXI ----------------------------------------------------------------------------------
             elif port["type"] == "axi":
                 axi_port  = LiteDRAMAXIPort(
                     data_width    = user_port.data_width,
                     address_width = user_port.address_width + log2_int(user_port.data_width//8),
                     id_width      = port["id_width"])
                 axi2native = LiteDRAMAXI2Native(
```

### Comparing `litedram-2023.4/litedram/init.py` & `litedram-2023.8/litedram/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,22 @@
     "PRECHARGE_ALL": "DFII_COMMAND_RAS|DFII_COMMAND_WE|DFII_COMMAND_CS",
     "MODE_REGISTER": "DFII_COMMAND_RAS|DFII_COMMAND_CAS|DFII_COMMAND_WE|DFII_COMMAND_CS",
     "AUTO_REFRESH":  "DFII_COMMAND_RAS|DFII_COMMAND_CAS|DFII_COMMAND_CS",
     "UNRESET":       "DFII_CONTROL_ODT|DFII_CONTROL_RESET_N",
     "CKE":           "DFII_CONTROL_CKE|DFII_CONTROL_ODT|DFII_CONTROL_RESET_N"
 }
 
+# Swap two bits in num
+# https://www.techiedelight.com/swap-two-bits-given-position-integer/
+def swap_bit(num, a, b):
+    if ((num >> a) & 1) != ((num >> b) & 1):
+        num = num ^ (1 << a)
+        num = num ^ (1 << b)
+    return num
+
 def reg(fields):
     # takes a list of tuples: [(bit_offset, bit_width, value), ...]
     regval = 0
     written = 0
     for shift, width, val in fields:
         mask = (2**width - 1) << shift
         assert written & mask == 0, "Would overwrite another field, xor=0b{:032b}".format(mask ^ written)
@@ -890,14 +898,17 @@
 
     r.define("DFII_COMMAND_CS",     "0x01")
     r.define("DFII_COMMAND_WE",     "0x02")
     r.define("DFII_COMMAND_CAS",    "0x04")
     r.define("DFII_COMMAND_RAS",    "0x08")
     r.define("DFII_COMMAND_WRDATA", "0x10")
     r.define("DFII_COMMAND_RDDATA", "0x20")
+    if phy_settings.is_clam_shell:
+        r.define("DFII_COMMAND_CS_TOP",  "0x40")
+        r.define("DFII_COMMAND_CS_BOTTOM",  "0x80")
     r.newline()
 
     phytype = phy_settings.phytype.upper()
     nphases = phy_settings.nphases
 
     # Define PHY type and number of phases
     r.define(f"SDRAM_PHY_{phytype}")
@@ -937,19 +948,22 @@
     if phy_settings.bitslips > 0:
         r.define("SDRAM_PHY_BITSLIPS", phy_settings.bitslips)
 
     r.define(f"SDRAM_PHY_{phy_settings.memtype}")
     if phy_settings.is_rdimm:
         assert phy_settings.memtype == "DDR4"
         r.define("SDRAM_PHY_DDR4_RDIMM")
+    if phy_settings.is_clam_shell:
+        assert phy_settings.memtype == "DDR4"
+        r.define("SDRAM_PHY_CLAM_SHELL")
 
-    # litedram doesn't support multiple ranks
-    supported_memory = 2 ** (geom_settings.bankbits +
-                        geom_settings.rowbits +
-                        geom_settings.colbits) * phy_settings.databits // 8
+    # Define memory size.
+    supported_memory = 2**(geom_settings.bankbits +
+                           geom_settings.rowbits +
+                           geom_settings.colbits)*phy_settings.nranks*phy_settings.databits//8
     r.define("SDRAM_PHY_SUPPORTED_MEMORY", f"0x{supported_memory:016x}ULL")
 
     r.newline()
 
     r += "void cdelay(int i);"
     r.newline()
 
@@ -1006,14 +1020,41 @@
                 #
                 # The 'ba != 7' is because we don't do this to writes to the RCD
                 # itself.
                 if ba != 7:
                     invert_masks.append((0b10101111111000, 0b1111))
 
             for a_inv, ba_inv in invert_masks:
+                # handle clam shell topology
+                if cmd == cmds["MODE_REGISTER"] and phy_settings.is_clam_shell:
+                    b += f"/* {comment} for top */"
+                    b += f"sdram_dfii_pi0_address_write({a ^ a_inv:#x});"
+                    b += f"sdram_dfii_pi0_baddress_write({ba ^ ba_inv:d});"
+                    b += f"command_p0({cmd}|DFII_COMMAND_CS_TOP);"
+                    if delay:
+                        b += f"cdelay({delay});\n"
+                    b.newline()
+
+                    # swap addr and pass to bottom
+                    b += f"/* {comment} for bottom */"
+                    addr = a ^ a_inv
+                    addr = swap_bit(addr, 3, 4)
+                    addr = swap_bit(addr, 5, 6)
+                    addr = swap_bit(addr, 7, 8)
+                    addr = swap_bit(addr, 11, 13)
+                    b += f"sdram_dfii_pi0_address_write({addr:#x});"
+                    baddr = ba ^ ba_inv
+                    baddr = swap_bit(baddr, 0, 1)
+                    b += f"sdram_dfii_pi0_baddress_write({baddr:d});"
+                    b += f"command_p0({cmd}|DFII_COMMAND_CS_BOTTOM);"
+                    if delay:
+                        b += f"cdelay({delay});\n"
+                    b.newline()
+                    continue
+
                 b += f"/* {comment} */"
                 b += f"sdram_dfii_pi0_address_write({a ^ a_inv:#x});"
                 b += f"sdram_dfii_pi0_baddress_write({ba ^ ba_inv:d});"
                 if cmd.startswith("DFII_CONTROL"):
                     b += f"sdram_dfii_control_write({cmd});"
                 else:
                     b += f"command_p0({cmd});"
```

### Comparing `litedram-2023.4/litedram/modules.py` & `litedram-2023.8/litedram/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,14 +586,22 @@
     nbanks = 4
     nrows  = 16384
     ncols  = 1024
     # timings
     technology_timings = _TechnologyTimings(tREFI=64e6/8192, tWTR=(2, None), tCCD=(1, None), tRRD=None)
     speedgrade_timings = {"default": _SpeedgradeTimings(tRP=15, tRCD=15, tWR=15, tRFC=(None, 72), tFAW=None, tRAS=None)}
 
+class MT46H128M16(LPDDRModule):
+    # geometry
+    nbanks = 4
+    nrows  = 16384
+    ncols  = 2048
+    # timings
+    technology_timings = _TechnologyTimings(tREFI=64e6/8192, tWTR=(2, None), tCCD=(1, None), tRRD=None)
+    speedgrade_timings = {"default": _SpeedgradeTimings(tRP=15, tRCD=15, tWR=15, tRFC=(None, 72), tFAW=None, tRAS=None)}
 
 class MT46H32M32(LPDDRModule):
     # geometry
     nbanks = 4
     nrows  = 8192
     ncols  = 1024
     # timings
```

### Comparing `litedram-2023.4/litedram/phy/__init__.py` & `litedram-2023.8/litedram/phy/__init__.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/dfi.py` & `litedram-2023.8/litedram/phy/dfi.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/ecp5ddrphy.py` & `litedram-2023.8/litedram/phy/ecp5ddrphy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 from functools import reduce
 from operator import or_
 
 import math
 
 from migen import *
-from migen.genlib.misc import timeline
+
 from migen.fhdl.specials import Tristate
 from migen.genlib.cdc import MultiReg
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import timeline
 
 from litex.soc.interconnect.csr import *
 
 from litedram.common import *
 from litedram.phy.dfi import *
 
 # BitSlip ------------------------------------------------------------------------------------------
```

### Comparing `litedram-2023.4/litedram/phy/gensdrphy.py` & `litedram-2023.8/litedram/phy/gensdrphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/gw2ddrphy.py` & `litedram-2023.8/litedram/phy/gw2ddrphy.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 from functools import reduce
 from operator import or_
 
 import math
 
 from migen import *
-from migen.genlib.misc import timeline
+
+from litex.gen import *
+
 from migen.fhdl.specials import Tristate
 from migen.genlib.cdc import MultiReg
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import timeline
 
 from litex.soc.interconnect.csr import *
 
 from litedram.common import *
 from litedram.phy.dfi import *
 
-class Open(Signal): pass
-
 # BitSlip ------------------------------------------------------------------------------------------
 
 # FIXME: Use BitSlip from litedram.common.
 
 class BitSlip(Module):
     def __init__(self, dw, rst=None, slp=None, cycles=1):
         self.i = Signal(dw)
@@ -169,16 +170,16 @@
             dfi_databits  = 4*databits,
             nranks        = nranks,
             nphases       = nphases,
             rdphase       = rdphase,
             wrphase       = wrphase,
             cl            = cl,
             cwl           = cwl,
-            read_latency  = cl_sys_latency + 10,
-            write_latency = cwl_sys_latency,
+            read_latency  = cl_sys_latency + 9,
+            write_latency = cwl_sys_latency - 1,
             read_leveling = True,
             bitslips      = 4,
             delays        = 8,
         )
 
         # DFI Interface ----------------------------------------------------------------------------
         self.dfi = dfi = Interface(addressbits, bankbits, nranks, 4*databits, nphases)
@@ -197,15 +198,15 @@
                 pad_oddrx2f = Signal()
                 pad_clk = Signal()
                 self.specials += Instance("OSER4",
                     p_TXCLK_POL = 0b0,
                     i_RESET = ResetSignal("sys"),
                     i_PCLK  = ClockSignal("sys"),
                     i_FCLK  = ClockSignal("sys2x"),
-                    **{f"i_TX{n}": 0b0 for n in range(2)}, # CHECKME: Polarity
+                    **{f"i_TX{n}": 0b0 for n in range(2)},
                     **{f"i_D{n}": (clk_pattern >> n) & 0b1 for n in range(4)},
                     o_Q0    = pad_oddrx2f,
                     o_Q1    = Open()
                 )
                 self.specials += Instance("IODELAY",
                     p_C_STATIC_DLY = cmd_delay,
                     i_SDTAP = 0,
@@ -243,15 +244,15 @@
                 for i in range(len(pad)):
                     pad_oddrx2f = Signal()
                     self.specials += Instance("OSER4",
                         p_TXCLK_POL = 0b0,
                         i_RESET = ResetSignal("sys"),
                         i_PCLK = ClockSignal("sys"),
                         i_FCLK = ClockSignal("sys2x"),
-                        **{f"i_TX{n}": 0b0 for n in range(2)}, # CHECKME: Polarity
+                        **{f"i_TX{n}": 0b0 for n in range(2)},
                         **{f"i_D{n}": getattr(dfi.phases[n//2], dfi_name)[i] for n in range(4)},
                         o_Q0   = pad_oddrx2f,
                         o_Q1   = Open()
                     )
                     self.specials += Instance("IODELAY",
                         p_C_STATIC_DLY = cmd_delay,
                         i_SDTAP     = 0,
@@ -309,15 +310,15 @@
                 o_DQSR90   = dqsr90,
                 o_RPOINT   = rdpntr,
                 o_WPOINT   = wrpntr,
                 o_RVALID   = self.datavalid[i],
                 o_RBURST   = burstdet,
 
                 # Writes (generate shifted ECLK clock for writes)
-                i_WSTEP    = Constant(0, 8), # CHECKME: Useful?
+                i_WSTEP    = Constant(0, 8),
                 o_DQSW270  = dqsw270,
                 o_DQSW0    = dqsw
             )
             burstdet_d = Signal()
             self.sync += [
                 burstdet_d.eq(burstdet),
                 If(self._burstdet_clr.re,  self._burstdet_seen.status[i].eq(0)),
@@ -331,16 +332,16 @@
                 Instance("OSER4_MEM",
                     p_TCLK_SOURCE = "DQSW",
                     p_TXCLK_POL   = 0b1,
                     i_RESET = ResetSignal("sys"),
                     i_PCLK  = ClockSignal("sys"),
                     i_FCLK  = ClockSignal("sys2x"),
                     i_TCLK  = dqsw,
-                    i_TX0   = ~(dqs_oe | dqs_postamble), # CHECKME: Polarity + Latency.
-                    i_TX1   = ~(dqs_oe | dqs_preamble),  # CHECKME: Polatiry + Latency.
+                    i_TX0   = ~(dqs_oe | dqs_postamble),
+                    i_TX1   = ~(dqs_oe | dqs_preamble),
                     **{f"i_D{n}": (0b1010 >> n) & 0b1 for n in range(4)},
                     o_Q0    = dqs_o,
                     o_Q1    = dqs_o_oen
                 ),
                 Instance("ELVDS_IOBUF",
                     i_I    = dqs_o,
                     i_OEN  = dqs_o_oen,
@@ -364,15 +365,15 @@
             self.specials += Instance("OSER4_MEM",
                 p_TCLK_SOURCE = "DQSW270",
                 p_TXCLK_POL   = 0b0,
                 i_RESET = ResetSignal("sys"),
                 i_PCLK  = ClockSignal("sys"),
                 i_FCLK  = ClockSignal("sys2x"),
                 i_TCLK  = dqsw270,
-                **{f"i_TX{n}": 0b0 for n in range(2)}, # CHECKME: Polarity
+                **{f"i_TX{n}": 0b0 for n in range(2)},
                 **{f"i_D{n}": dm_o_data_muxed[n] for n in range(4)},
                 o_Q0    = pads.dm[i],
                 o_Q1    = Open()
             )
 
             # DQ -----------------------------------------------------------------------------------
             for j in range(8*i, 8*(i+1)):
@@ -393,16 +394,16 @@
                 self.specials += Instance("OSER4_MEM",
                     p_TCLK_SOURCE = "DQSW270",
                     p_TXCLK_POL   = 0b0,
                     i_RESET = ResetSignal("sys"),
                     i_PCLK  = ClockSignal("sys"),
                     i_FCLK  = ClockSignal("sys2x"),
                     i_TCLK  = dqsw270,
-                    i_TX0   = ~dq_oe, # CHECKME: Polarity + Latency.
-                    i_TX1   = ~dq_oe, # CHECKME: Polarity + Latency.
+                    i_TX0   = ~dq_oe,
+                    i_TX1   = ~dq_oe,
                     **{f"i_D{n}": dq_o_data_muxed[n] for n in range(4)},
                     o_Q0    = dq_o,
                     o_Q1    = dq_o_oen,
                 )
                 dq_i_bitslip = BitSlip(4,
                     rst    = self._dly_sel.storage[i] & self._rdly_dq_bitslip_rst.re,
                     slp    = self._dly_sel.storage[i] & self._rdly_dq_bitslip.re,
@@ -428,15 +429,15 @@
                     i_I   = dq_o,
                     i_OEN = dq_o_oen,
                     o_O   = dq_i,
                     io_IO = pads.dq[j]
                 )
 
         # Read Control Path ------------------------------------------------------------------------
-        rdtap = cl_sys_latency # CHECKME: Latency.
+        rdtap = cl_sys_latency - 1
 
         # Creates a delay line of read commands coming from the DFI interface. The taps are used to
         # control DQS read (internal read pulse of the DQSBUF) and the output of the delay is used
         # signal a valid read data to the DFI interface.
         #
         # The DQS read must be asserted for 2 sys_clk cycles before the read data is coming back from
         # the DRAM (see 6.2.4 READ Pulse Positioning Optimization of FPGA-TN-02035-1.2)
@@ -449,24 +450,24 @@
         )
         self.submodules += rddata_en
 
         self.comb += [phase.rddata_valid.eq(rddata_en.output) for phase in dfi.phases]
         self.comb += dqs_re.eq(rddata_en.taps[rdtap] | rddata_en.taps[rdtap + 1])
 
         # Write Control Path -----------------------------------------------------------------------
-        wrtap = cwl_sys_latency  # CHECKME: Latency.
+        wrtap = cwl_sys_latency - 1
 
         # Create a delay line of write commands coming from the DFI interface. This taps are used to
         # control DQ/DQS tristates and to select write data of the DRAM burst from the DFI interface.
         # The PHY is operating in halfrate mode (so provide 4 datas every sys_clk cycles: 2x for DDR,
         # 2x for halfrate) but DDR3 requires a burst of 8 datas (BL8) for best efficiency. Writes are
         # then performed in 2 sys_clk cycles and data needs to be selected for each cycle.
         wrdata_en = TappedDelayLine(
             signal = reduce(or_, [dfi.phases[i].wrdata_en for i in range(nphases)]),
-            ntaps  = wrtap + 4  # CHECKME: Latency.
+            ntaps  = wrtap + 4
         )
         self.submodules += wrdata_en
 
         self.comb += dq_oe.eq(wrdata_en.taps[wrtap] | wrdata_en.taps[wrtap + 1])
         self.comb += bl8_chunk.eq(wrdata_en.taps[wrtap])
         self.comb += dqs_oe.eq(dq_oe)
```

### Comparing `litedram-2023.4/litedram/phy/lpddr4/README.md` & `litedram-2023.8/litedram/phy/lpddr4/README.md`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/basephy.py` & `litedram-2023.8/litedram/phy/lpddr4/basephy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/commands.py` & `litedram-2023.8/litedram/phy/lpddr4/commands.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/s7phy.py` & `litedram-2023.8/litedram/phy/lpddr4/s7phy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/sim.py` & `litedram-2023.8/litedram/phy/lpddr4/sim.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/simphy.py` & `litedram-2023.8/litedram/phy/lpddr4/simphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr4/simsoc.py` & `litedram-2023.8/litedram/phy/lpddr4/simsoc.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/basephy.py` & `litedram-2023.8/litedram/phy/lpddr5/basephy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/commands.py` & `litedram-2023.8/litedram/phy/lpddr5/commands.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/s7phy.py` & `litedram-2023.8/litedram/phy/lpddr5/s7phy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/sim.py` & `litedram-2023.8/litedram/phy/lpddr5/sim.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/simphy.py` & `litedram-2023.8/litedram/phy/lpddr5/simphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/lpddr5/simsoc.py` & `litedram-2023.8/litedram/phy/lpddr5/simsoc.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/model.py` & `litedram-2023.8/litedram/phy/model.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/rpc/README.md` & `litedram-2023.8/litedram/phy/rpc/README.md`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/rpc/arty.py` & `litedram-2023.8/litedram/phy/rpc/arty.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             (0xa3, 0x78),
             # Vbuck2B / 1.5V.
             (0xb4, 0x78),
         ])
 
         if dynamic_freq:
             # UartBone -----------------------------------------------------------------------------
-            self.add_uartbone(name="serial", clk_freq=100e6, baudrate=1e6, cd="uart")
+            self.add_uartbone(clk_freq=100e6, baudrate=1e6, cd="uart")
         else:
             # Etherbone ----------------------------------------------------------------------------
             self.submodules.ethphy = LiteEthPHYMII(
                 clock_pads = self.platform.request("eth_clocks"),
                 pads       = self.platform.request("eth"))
             self.add_etherbone(phy=self.ethphy, ip_address=ip_address)
```

### Comparing `litedram-2023.4/litedram/phy/rpc/basephy.py` & `litedram-2023.8/litedram/phy/rpc/basephy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Copyright (c) 2020-2021 Antmicro <www.antmicro.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 from operator import and_
 
 from migen import *
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import WaitTimer
 
 from litex.soc.interconnect.csr import AutoCSR, CSR, CSRStatus, CSRStorage
 
 from litedram.common import *
 from litedram.phy.utils import chunks, bitpattern
 from litedram.phy.dfi import Interface as DFIInterface
 from litedram.phy.rpc.commands import DFIAdapter
```

### Comparing `litedram-2023.4/litedram/phy/rpc/commands.py` & `litedram-2023.8/litedram/phy/rpc/commands.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/rpc/s7phy.py` & `litedram-2023.8/litedram/phy/rpc/s7phy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/rpc/simphy.py` & `litedram-2023.8/litedram/phy/rpc/simphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/rpc/simsoc.py` & `litedram-2023.8/litedram/phy/rpc/simsoc.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/s6ddrphy.py` & `litedram-2023.8/litedram/phy/s6ddrphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/s7common.py` & `litedram-2023.8/litedram/phy/s7common.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/s7ddrphy.py` & `litedram-2023.8/litedram/phy/s7ddrphy.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/sim_utils.py` & `litedram-2023.8/litedram/phy/sim_utils.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram/phy/usddrphy.py` & `litedram-2023.8/litedram/phy/usddrphy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from functools import reduce
 from operator import or_
 
 import math
 
 from migen import *
-from migen.genlib.misc import WaitTimer
+
+from litex.gen.genlib.misc import WaitTimer
 
 from litex.soc.interconnect.csr import *
 
 from litedram.common import *
 from litedram.phy.dfi import *
 
 # Xilinx Ultrascale (Plus) DDR3/DDR4 PHY -----------------------------------------------------------
@@ -28,15 +29,16 @@
         memtype          = "DDR3",
         sys_clk_freq     = 100e6,
         iodelay_clk_freq = 200e6,
         cl               = None,
         cwl              = None,
         cmd_latency      = 0,
         cmd_delay        = None,
-        is_rdimm         = False):
+        is_rdimm         = False,
+        is_clam_shell    = False):
         phytype     = self.__class__.__name__
         device      = {"USDDRPHY": "ULTRASCALE", "USPDDRPHY": "ULTRASCALE_PLUS"}[phytype]
         pads        = PHYPadsCombiner(pads)
         tck         = 2/(2*4*sys_clk_freq)
         addressbits = len(pads.a)
         if memtype == "DDR4":
             addressbits += 3 # cas_n/ras_n/we_n multiplexed with address
@@ -93,29 +95,30 @@
 
         # PHY settings -----------------------------------------------------------------------------
         self.settings = PhySettings(
             phytype                   = phytype,
             memtype                   = memtype,
             databits                  = databits,
             dfi_databits              = 2*databits,
-            nranks                    = nranks,
+            nranks                    = nranks//2 if is_clam_shell else nranks,
             nphases                   = nphases,
             rdphase                   = self._rdphase.storage,
             wrphase                   = self._wrphase.storage,
             cl                        = cl,
             cwl                       = cwl,
             read_latency              = cl_sys_latency + 5,
             write_latency             = cwl_sys_latency - 1,
             cmd_latency               = cmd_latency,
             cmd_delay                 = cmd_delay,
             write_leveling            = True,
             write_latency_calibration = True,
             read_leveling             = True,
             delays                    = 512,
             bitslips                  = 8,
+            is_clam_shell             = is_clam_shell,
         )
 
         if is_rdimm:
             # All drive settings for an 8-chip load
             self.settings.set_rdimm(
                 tck               = tck,
                 rcd_pll_bypass    = False,
```

### Comparing `litedram-2023.4/litedram/phy/utils.py` & `litedram-2023.8/litedram/phy/utils.py`

 * *Files identical despite different names*

### Comparing `litedram-2023.4/litedram.egg-info/PKG-INFO` & `litedram-2023.8/litedram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litedram
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable DRAM core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litedram
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `litedram-2023.4/litedram.egg-info/SOURCES.txt` & `litedram-2023.8/litedram.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 litedram/core/bankmachine.py
 litedram/core/controller.py
 litedram/core/crossbar.py
 litedram/core/multiplexer.py
 litedram/core/refresher.py
 litedram/frontend/__init__.py
 litedram/frontend/adapter.py
+litedram/frontend/avalon.py
 litedram/frontend/axi.py
 litedram/frontend/bist.py
 litedram/frontend/dma.py
 litedram/frontend/ecc.py
 litedram/frontend/fifo.py
 litedram/frontend/wishbone.py
 litedram/phy/__init__.py
```

### Comparing `litedram-2023.4/setup.py` & `litedram-2023.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(
     name="litedram",
-    version="2023.04",
+    version="2023.08",
     description="Small footprint and configurable DRAM core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/litedram",
```

