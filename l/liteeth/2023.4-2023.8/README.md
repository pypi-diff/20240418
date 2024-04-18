# Comparing `tmp/liteeth-2023.4.tar.gz` & `tmp/liteeth-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteeth-2023.4.tar", last modified: Thu Apr 18 20:04:16 2024, max compression
+gzip compressed data, was "liteeth-2023.8.tar", last modified: Thu Apr 18 20:04:55 2024, max compression
```

## Comparing `liteeth-2023.4.tar` & `liteeth-2023.8.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.852095 liteeth-2023.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1858 2024-04-18 20:04:12.000000 liteeth-2023.4/CONTRIBUTORS
--rw-r--r--   0 timkpaine   (501) staff       (20)     1682 2024-04-18 20:04:02.000000 liteeth-2023.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      102 2024-04-18 20:04:02.000000 liteeth-2023.4/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     4608 2024-04-18 20:04:16.851790 liteeth-2023.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     3720 2024-04-18 20:04:12.000000 liteeth-2023.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.843175 liteeth-2023.4/doc/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3408 2024-04-18 20:04:02.000000 liteeth-2023.4/doc/architecture.dia
--rw-r--r--   0 timkpaine   (501) staff       (20)    31809 2024-04-18 20:04:02.000000 liteeth-2023.4/doc/architecture.png
--rw-r--r--   0 timkpaine   (501) staff       (20)     4280 2024-04-18 20:04:02.000000 liteeth-2023.4/doc/enjoy_digital.png
--rw-r--r--   0 timkpaine   (501) staff       (20)    56337 2024-04-18 20:04:02.000000 liteeth-2023.4/doc/liteeth_logo_full.png
--rw-r--r--   0 timkpaine   (501) staff       (20)    93602 2024-04-18 20:04:02.000000 liteeth-2023.4/doc/liteeth_logo_full.svg
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.843999 liteeth-2023.4/liteeth/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9812 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.845723 liteeth-2023.4/liteeth/core/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2907 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/core/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11355 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/core/arp.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5440 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/core/icmp.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9912 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/core/ip.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8276 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/core/udp.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1237 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/crossbar.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.846151 liteeth-2023.4/liteeth/frontend/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/frontend/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17703 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/frontend/etherbone.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4728 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/frontend/stream.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    16863 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/gen.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.847652 liteeth-2023.4/liteeth/mac/
--rw-r--r--   0 timkpaine   (501) staff       (20)     7097 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1819 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/mac/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9273 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/core.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12638 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/crc.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1166 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/mac/gap.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1890 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/mac/last_be.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2846 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/mac/padding.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3983 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/preamble.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11460 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/sram.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2653 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/mac/wishbone.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17251 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/packet.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.850796 liteeth-2023.4/liteeth/phy/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1678 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    39575 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/a7_1000basex.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6752 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/a7_gtp.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1451 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6778 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/ecp5rgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3731 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/gmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5818 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/gmii_mii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    37801 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/k7_1000basex.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    40870 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/ku_1000basex.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3552 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/mii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1387 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/model.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    13973 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/pcs_1000basex.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4870 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/rmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8816 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/s6rgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7433 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/s7rgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8038 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/titaniumrgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7100 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/trionrgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    47101 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/usp_1000basex.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7576 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/usrgmii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    31387 2024-04-18 20:04:12.000000 liteeth-2023.4/liteeth/phy/xgmii.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.850956 liteeth-2023.4/liteeth/software/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/software/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.851059 liteeth-2023.4/liteeth/software/dissector/
--rw-r--r--   0 timkpaine   (501) staff       (20)    13701 2024-04-18 20:04:02.000000 liteeth-2023.4/liteeth/software/dissector/etherbone.lua
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:16.851294 liteeth-2023.4/liteeth.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4608 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     1409 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       49 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       46 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        8 2024-04-18 20:04:16.000000 liteeth-2023.4/liteeth.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:04:16.852147 liteeth-2023.4/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     1379 2024-04-18 20:04:12.000000 liteeth-2023.4/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.523784 liteeth-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1858 2024-04-18 20:04:12.000000 liteeth-2023.8/CONTRIBUTORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1682 2024-04-18 20:04:02.000000 liteeth-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      102 2024-04-18 20:04:02.000000 liteeth-2023.8/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5205 2024-04-18 20:04:55.523522 liteeth-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4317 2024-04-18 20:04:28.000000 liteeth-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.510187 liteeth-2023.8/doc/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3408 2024-04-18 20:04:02.000000 liteeth-2023.8/doc/architecture.dia
+-rw-r--r--   0 timkpaine   (501) staff       (20)    31809 2024-04-18 20:04:02.000000 liteeth-2023.8/doc/architecture.png
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4280 2024-04-18 20:04:02.000000 liteeth-2023.8/doc/enjoy_digital.png
+-rw-r--r--   0 timkpaine   (501) staff       (20)    56337 2024-04-18 20:04:02.000000 liteeth-2023.8/doc/liteeth_logo_full.png
+-rw-r--r--   0 timkpaine   (501) staff       (20)    93602 2024-04-18 20:04:02.000000 liteeth-2023.8/doc/liteeth_logo_full.svg
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.511193 liteeth-2023.8/liteeth/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     9826 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.513098 liteeth-2023.8/liteeth/core/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3824 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    13751 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/arp.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    20899 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/dhcp.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5691 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/icmp.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     9887 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/ip.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8212 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/core/udp.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1250 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/crossbar.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.516137 liteeth-2023.8/liteeth/frontend/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/frontend/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    17545 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/frontend/etherbone.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5193 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/frontend/stream.py
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)    24526 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/gen.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.518286 liteeth-2023.8/liteeth/mac/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7667 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/mac/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1819 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/mac/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     9624 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/mac/core.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    12642 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/mac/crc.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1166 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/mac/gap.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1890 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/mac/last_be.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2846 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/mac/padding.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3987 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/mac/preamble.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11460 2024-04-18 20:04:12.000000 liteeth-2023.8/liteeth/mac/sram.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2756 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/mac/wishbone.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    17219 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/packet.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.522410 liteeth-2023.8/liteeth/phy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1830 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    32732 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/a7_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    32802 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/a7_2500basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6752 2024-04-18 20:04:12.000000 liteeth-2023.8/liteeth/phy/a7_gtp.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1684 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7290 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/ecp5rgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4090 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/gmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6207 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/gmii_mii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6461 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/gw5rgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    30816 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/k7_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    40210 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/ku_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3581 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/mii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1561 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/model.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    16056 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/pcs_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5263 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/rmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     9140 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/s6rgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7775 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/s7rgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6031 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/titaniumrgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6025 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/trionrgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    44908 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/usp_gth_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    46883 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/usp_gty_1000basex.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     8128 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/usrgmii.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    31910 2024-04-18 20:04:28.000000 liteeth-2023.8/liteeth/phy/xgmii.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.522578 liteeth-2023.8/liteeth/software/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/software/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.522694 liteeth-2023.8/liteeth/software/dissector/
+-rw-r--r--   0 timkpaine   (501) staff       (20)    13701 2024-04-18 20:04:02.000000 liteeth-2023.8/liteeth/software/dissector/etherbone.lua
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:04:55.523079 liteeth-2023.8/liteeth.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5205 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1519 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       49 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       46 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        8 2024-04-18 20:04:55.000000 liteeth-2023.8/liteeth.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:04:55.523833 liteeth-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     1379 2024-04-18 20:04:52.000000 liteeth-2023.8/setup.py
```

### Comparing `liteeth-2023.4/CONTRIBUTORS` & `liteeth-2023.8/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/LICENSE` & `liteeth-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/PKG-INFO` & `liteeth-2023.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteeth
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable Ethernet core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/liteeth
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
@@ -26,15 +26,15 @@
 
 ```
                                       __   _ __      ______  __
                                      / /  (_) /____ / __/ /_/ /
                                     / /__/ / __/ -_) _// __/ _ \
                                    /____/_/\__/\__/___/\__/_//_/
 
-                                 Copyright 2012-2022 / EnjoyDigital
+                                 Copyright 2012-2023 / EnjoyDigital
 
                              A small footprint and configurable Ethernet core
                                       powered by Migen & LiteX
 ```
 
 [![](https://github.com/enjoy-digital/liteeth/workflows/ci/badge.svg)](https://github.com/enjoy-digital/liteeth/actions) ![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)
 
@@ -52,22 +52,32 @@
 LiteEth can be used as LiteX library or can be integrated with your standard
 design flow by generating the verilog rtl that you will use as a standard core.
 
 [> Features
 -----------
 PHY:
   - MII, RMII 100Mbps PHYs.
-  - GMII / RGMII /1000BaseX 1Gbps PHYs.
+  - GMII / RGMII / SGMII / 1000BaseX 1Gbps PHYs.
+
+| -     | All | ECP5 | Spartan6 | Trion | Titanium | 7-Series | Ultrascale(+) |
+|-------|-----|------|----------|-------|----------|----------|---------------|
+| MII   |  X  |  X  |      X    |   X   |     X    |     X    |       X       |
+| RMII  |  X  |  X  |      X    |   X   |     X    |     X    |       X       |
+| GMII  |     |     |      X    |       |          |     X    |       X       |
+| RGMII |     |  X  |      X    |   X   |     X    |     X    |       X       |
+| SGMII |     |     |           |       |          |     X    |       X       |
+
 
 Core:
   - Configurable MAC (HW or SW interface)
-  - ARP / ICMP / UDP (HW or SW)
+  - ARP / ICMP / UDP (HW or SW) / DHCP
 
 Frontend:
   - Etherbone (Wishbone over UDP: Slave or Master support)
+  - UDP Streaming.
 
 [> FPGA Proven
 ---------------
 LiteEth is already used in commercial and open-source designs:
 - MiSoC: http://m-labs.hk/gateware.html
 - ARTIQ: http://m-labs.hk/artiq/index.html
 - HDMI2USB: http://hdmi2usb.tv/home/
```

### Comparing `liteeth-2023.4/doc/architecture.dia` & `liteeth-2023.8/doc/architecture.dia`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/doc/architecture.png` & `liteeth-2023.8/doc/architecture.png`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/doc/enjoy_digital.png` & `liteeth-2023.8/doc/enjoy_digital.png`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/doc/liteeth_logo_full.png` & `liteeth-2023.8/doc/liteeth_logo_full.png`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/doc/liteeth_logo_full.svg` & `liteeth-2023.8/doc/liteeth_logo_full.svg`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/common.py` & `liteeth-2023.8/liteeth/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,19 +84,19 @@
     "sender_ip":      HeaderField(12, 0, 32),
     "target_ip":      HeaderField(16, 0, 32)
 }
 ipv4_header = Header(ipv4_header_fields, ipv4_header_length, swap_field_bytes=True)
 
 # ICMP Constants/Header ----------------------------------------------------------------------------
 
-icmp_protocol      = 0x01
-icmp_type_ping_reply = 0
+icmp_protocol          = 0x01
+icmp_type_ping_reply   = 0
 icmp_type_ping_request = 8
-icmp_header_length = 8
-icmp_header_fields = {
+icmp_header_length     = 8
+icmp_header_fields     = {
     "msgtype":  HeaderField(0, 0,  8),
     "code":     HeaderField(1, 0,  8),
     "checksum": HeaderField(2, 0, 16),
     "quench":   HeaderField(4, 0, 32)
 }
 icmp_header  = Header(icmp_header_fields, icmp_header_length, swap_field_bytes=True)
```

### Comparing `liteeth-2023.4/liteeth/core/__init__.py` & `liteeth-2023.8/liteeth/core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 #
 # This file is part of LiteEth.
 #
 # Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2023 LumiGuide Fietsdetectie B.V. <goemansrowan@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
-from liteeth.common import *
-from liteeth.mac import LiteEthMAC
-from liteeth.core.arp import LiteEthARP
-from liteeth.core.ip import LiteEthIP
-from liteeth.core.udp import LiteEthUDP
+from liteeth.common    import *
+from liteeth.mac       import LiteEthMAC
+from liteeth.core.arp  import LiteEthARP
+from liteeth.core.ip   import LiteEthIP
+from liteeth.core.udp  import LiteEthUDP
 from liteeth.core.icmp import LiteEthICMP
 
 # IP Core ------------------------------------------------------------------------------------------
 
 class LiteEthIPCore(Module, AutoCSR):
-    def __init__(self, phy, mac_address, ip_address, clk_freq, dw=8,
+    def __init__(self, phy, mac_address, ip_address, clk_freq, arp_entries=1, dw=8,
         with_icmp         = True,
         with_ip_broadcast = True,
-        with_sys_datapath = False):
+        with_sys_datapath = False,
+        tx_cdc_depth      = 32,
+        tx_cdc_buffered   = True,
+        rx_cdc_depth      = 32,
+        rx_cdc_buffered   = True,
+    ):
         # Parameters.
         # -----------
         ip_address = convert_ip(ip_address)
 
         # MAC.
         # ----
         self.submodules.mac = LiteEthMAC(
-            phy       = phy,
-            dw        = dw,
-            interface = "crossbar",
+            phy               = phy,
+            dw                = dw,
+            interface         = "crossbar",
             with_preamble_crc = True,
             with_sys_datapath = with_sys_datapath,
+            tx_cdc_depth      = tx_cdc_depth,
+            tx_cdc_buffered   = tx_cdc_buffered,
+            rx_cdc_depth      = rx_cdc_depth,
+            rx_cdc_buffered   = rx_cdc_buffered
         )
 
         # ARP.
         # ----
         self.submodules.arp = LiteEthARP(
             mac         = self.mac,
             mac_address = mac_address,
             ip_address  = ip_address,
             clk_freq    = clk_freq,
+            entries     = arp_entries,
             dw          = dw,
         )
 
         # IP.
         # ---
         self.submodules.ip  = LiteEthIP(
             mac            = self.mac,
@@ -60,33 +71,43 @@
                 ip_address = ip_address,
                 dw         = dw,
             )
 
 # UDP IP Core --------------------------------------------------------------------------------------
 
 class LiteEthUDPIPCore(LiteEthIPCore):
-    def __init__(self, phy, mac_address, ip_address, clk_freq, dw=8,
+    def __init__(self, phy, mac_address, ip_address, clk_freq, arp_entries=1, dw=8,
         with_icmp         = True,
         with_ip_broadcast = True,
-        with_sys_datapath = False):
+        with_sys_datapath = False,
+        tx_cdc_depth      = 32,
+        tx_cdc_buffered   = True,
+        rx_cdc_depth      = 32,
+        rx_cdc_buffered   = True,
+    ):
         # Parameters.
         # -----------
         ip_address = convert_ip(ip_address)
 
         # Core: MAC + ARP + IP + (ICMP).
         # ------------------------------
         LiteEthIPCore.__init__(self,
-            phy         = phy,
-            mac_address = mac_address,
-            ip_address  = ip_address,
-            clk_freq    = clk_freq,
-            with_icmp   = with_icmp,
-            dw          = dw,
+            phy               = phy,
+            mac_address       = mac_address,
+            ip_address        = ip_address,
+            clk_freq          = clk_freq,
+            arp_entries       = arp_entries,
+            with_icmp         = with_icmp,
+            dw                = dw,
             with_ip_broadcast = with_ip_broadcast,
             with_sys_datapath = with_sys_datapath,
+            tx_cdc_depth      = tx_cdc_depth,
+            tx_cdc_buffered   = tx_cdc_buffered,
+            rx_cdc_depth      = rx_cdc_depth,
+            rx_cdc_buffered   = rx_cdc_buffered,
         )
         # UDP.
         # ----
         self.submodules.udp = LiteEthUDP(
             ip         = self.ip,
             ip_address = ip_address,
             dw         = dw,
```

### Comparing `liteeth-2023.4/liteeth/core/arp.py` & `liteeth-2023.8/liteeth/core/arp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-from liteeth.common import *
-
-from migen.genlib.misc import WaitTimer
+from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
 
+from liteeth.common import *
 from liteeth.packet import Depacketizer, Packetizer
 
 # ARP Layouts --------------------------------------------------------------------------------------
 
 _arp_table_layout = [
         ("reply",        1),
         ("request",      1),
@@ -22,42 +22,43 @@
 # ARP TX -------------------------------------------------------------------------------------------
 
 class LiteEthARPPacketizer(Packetizer):
     def __init__(self, dw=8):
         Packetizer.__init__(self,
             eth_arp_description(dw),
             eth_mac_description(dw),
-            arp_header)
+            arp_header
+        )
 
 
-class LiteEthARPTX(Module):
+class LiteEthARPTX(LiteXModule):
     def __init__(self, mac_address, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(_arp_table_layout)
         self.source = source = stream.Endpoint(eth_mac_description(dw))
 
         # # #
 
         packet_length = max(arp_header.length, arp_min_length)
         packet_words  = packet_length//(dw//8)
         counter       = Signal(max=packet_words, reset_less=True)
 
-        self.submodules.packetizer = packetizer = LiteEthARPPacketizer(dw)
+        self.packetizer = packetizer = LiteEthARPPacketizer(dw)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(counter, 0),
             If(sink.valid,
                 NextState("SEND")
             )
         )
         self.comb += [
             packetizer.sink.last.eq(counter == (packet_words - 1)),
             If(packetizer.sink.last,
-                packetizer.sink.last_be.eq(
-                    1 if len(packetizer.sink.last_be) == 1 else 2**(packet_length % (dw // 8) - 1)
+                packetizer.sink.last_be.eq(1 if len(packetizer.sink.last_be) == 1 else
+                                           2**(packet_length % (dw // 8) - 1)
                 ),
             ),
             packetizer.sink.hwtype.eq(arp_hwtype_ethernet),
             packetizer.sink.proto.eq(arp_proto_ip),
             packetizer.sink.hwsize.eq(6),
             packetizer.sink.protosize.eq(4),
             packetizer.sink.sender_mac.eq(mac_address),
@@ -92,51 +93,52 @@
 # ARP RX -------------------------------------------------------------------------------------------
 
 class LiteEthARPDepacketizer(Depacketizer):
     def __init__(self, dw=8):
         Depacketizer.__init__(self,
             eth_mac_description(dw),
             eth_arp_description(dw),
-            arp_header)
+            arp_header
+        )
 
 
-class LiteEthARPRX(Module):
+class LiteEthARPRX(LiteXModule):
     def __init__(self, mac_address, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_mac_description(dw))
         self.source = source = stream.Endpoint(_arp_table_layout)
 
-        # # #s
+        # # #
 
-        self.submodules.depacketizer = depacketizer = LiteEthARPDepacketizer(dw)
+        self.depacketizer = depacketizer = LiteEthARPDepacketizer(dw)
         self.comb += sink.connect(depacketizer.sink)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             depacketizer.source.ready.eq(1),
             If(depacketizer.source.valid,
                 depacketizer.source.ready.eq(0),
                 NextState("CHECK")
             )
         )
         valid = Signal(reset_less=True)
         self.sync += valid.eq(
             depacketizer.source.valid &
-            (depacketizer.source.hwtype == arp_hwtype_ethernet) &
-            (depacketizer.source.proto == arp_proto_ip) &
-            (depacketizer.source.hwsize == 6) &
+            (depacketizer.source.hwtype    == arp_hwtype_ethernet) &
+            (depacketizer.source.proto     == arp_proto_ip) &
+            (depacketizer.source.hwsize    == 6) &
             (depacketizer.source.protosize == 4) &
             (depacketizer.source.target_ip == ip_address)
         )
-        reply = Signal()
+        reply   = Signal()
         request = Signal()
         self.comb += Case(depacketizer.source.opcode, {
-            arp_opcode_request: [request.eq(1)],
-            arp_opcode_reply:   [reply.eq(1)],
-            "default":          []
-            })
+            arp_opcode_request : [request.eq(1)],
+            arp_opcode_reply   : [reply.eq(1)],
+            "default"          : []
+        })
         self.comb += [
             source.ip_address.eq(depacketizer.source.sender_ip),
             source.mac_address.eq(depacketizer.source.sender_mac)
         ]
         fsm.act("CHECK",
             If(valid,
                 source.valid.eq(1),
@@ -148,160 +150,226 @@
         fsm.act("TERMINATE",
             depacketizer.source.ready.eq(1),
             If(depacketizer.source.valid & depacketizer.source.last,
                 NextState("IDLE")
             )
         )
 
+# ARP Cache ----------------------------------------------------------------------------------------
+
+class LiteEthARPCache(LiteXModule):
+    def __init__(self, entries, clk_freq):
+        # Update interface.
+        self.update = stream.Endpoint([("ip_address", 32), ("mac_address", 48)])
+
+        # Request/Response interface.
+        self.request  = stream.Endpoint([("ip_address", 32)])
+        self.response = stream.Endpoint([("mac_address", 48), ("error", 1)])
+
+        # Enable.
+        self.enable       = Signal(reset=1)
+        self.clear_enable = Signal(reset=1)
+
+        # # #
+
+        # Parameters.
+        entries = max(entries, 2) # Minimal number of entries is 2.
+
+        # Signals.
+        update_count = Signal(max=entries)
+        search_count = Signal(max=entries)
+        error        = Signal()
+
+        # Memory
+        mem_width   = 32 + 48 + 1 # IP + MAC + Valid.
+        mem         = Memory(mem_width, entries)
+        mem_wr_port = mem.get_port(write_capable=True)
+        mem_rd_port = mem.get_port(async_read=True) # FIXME: Avoid async_read.
+        self.specials += mem, mem_wr_port, mem_rd_port
+
+        # Memory wr_port aliases.
+        mem_wr_port_valid       = mem_wr_port.dat_w[80]
+        mem_wr_port_ip_address  = mem_wr_port.dat_w[0:32]
+        mem_wr_port_mac_address = mem_wr_port.dat_w[32:80]
+
+        # Memory rd_port aliases.
+        mem_rd_port_valid       = mem_rd_port.dat_r[80]
+        mem_rd_port_ip_address  = mem_rd_port.dat_r[0:32]
+        mem_rd_port_mac_address = mem_rd_port.dat_r[32:80]
+
+        # Clear Timer to clear table every 1s.
+        self.clear_timer = WaitTimer(1e-0*clk_freq)
+
+        # FSM.
+        self.fsm = fsm = FSM(reset_state="CLEAR")
+        fsm.act("CLEAR",
+            mem_wr_port.we.eq(1),
+            mem_wr_port.adr.eq(update_count),
+            mem_wr_port_valid.eq(0),
+            NextValue(update_count, update_count + 1),
+            If(update_count == (entries - 1),
+                NextState("IDLE")
+            )
+        )
+        fsm.act("IDLE",
+            If(self.enable & self.update.valid,
+                NextState("MEM_UPDATE")
+            ),
+            If(self.enable & self.request.valid,
+                NextValue(search_count, 0),
+                NextState("MEM_SEARCH")
+            ),
+            self.clear_timer.wait.eq(self.clear_enable),
+            If(self.clear_timer.done,
+                NextValue(update_count, 0),
+                NextState("CLEAR")
+            )
+        )
+        fsm.act("MEM_UPDATE",
+            mem_wr_port.we.eq(1),
+            mem_wr_port.adr.eq(update_count),
+            mem_wr_port_valid.eq(1),
+            mem_wr_port_ip_address.eq( self.update.ip_address),
+            mem_wr_port_mac_address.eq(self.update.mac_address),
+            self.update.ready.eq(1),
+            If(update_count == (entries - 1),
+                NextValue(update_count, 0)
+            ).Else(
+                NextValue(update_count, update_count + 1)
+            ),
+            NextState("IDLE")
+        )
+        fsm.act("MEM_SEARCH",
+           mem_rd_port.adr.eq(search_count),
+           If(mem_rd_port_valid & (mem_rd_port_ip_address == self.request.ip_address),
+               NextValue(error, 0),
+               NextState("RESPONSE")
+           ).Elif(search_count == (entries - 1),
+               NextValue(error, 1),
+               NextState("RESPONSE")
+           ).Else(
+               NextValue(search_count, search_count + 1)
+           )
+        )
+        fsm.act("RESPONSE",
+           self.request.ready.eq(1),
+           self.response.valid.eq(1),
+           self.response.error.eq(error),
+           self.response.mac_address.eq(mem_rd_port_mac_address),
+           NextState("IDLE")
+       )
+
 # ARP Table ----------------------------------------------------------------------------------------
 
-class LiteEthARPTable(Module):
-    def __init__(self, clk_freq, max_requests=8):
+class LiteEthARPTable(LiteXModule):
+    def __init__(self, clk_freq, entries=1, max_requests=8):
         self.sink   = sink   = stream.Endpoint(_arp_table_layout)  # from arp_rx
         self.source = source = stream.Endpoint(_arp_table_layout)  # to arp_tx
 
         # Request/Response interface
         self.request  = request  = stream.Endpoint(arp_table_request_layout)
         self.response = response = stream.Endpoint(arp_table_response_layout)
 
         # # #
 
-        request_pending     = Signal()
-        request_pending_clr = Signal()
-        request_pending_set = Signal()
-        self.sync += \
-            If(request_pending_clr,
-                request_pending.eq(0)
-            ).Elif(request_pending_set,
-                request_pending.eq(1)
-            )
-
-        request_ip_address        = Signal(32, reset_less=True)
-        request_ip_address_reset  = Signal()
-        request_ip_address_update = Signal()
-        self.sync += \
-            If(request_ip_address_reset,
-                request_ip_address.eq(0)
-            ).Elif(request_ip_address_update,
-                request_ip_address.eq(request.ip_address)
-            )
-
-        request_timer = WaitTimer(clk_freq//10)
-        self.submodules += request_timer
-        request_counter       = Signal(max=max_requests)
-        request_counter_reset = Signal()
-        request_counter_ce    = Signal()
-        self.sync += \
-            If(request_counter_reset,
-                request_counter.eq(0)
-            ).Elif(request_counter_ce,
-                request_counter.eq(request_counter + 1)
-            )
-        self.comb += request_timer.wait.eq(request_pending & ~request_counter_ce)
-
-        # Note: Store only 1 IP/MAC couple, can be improved with a real
-        # table in the future to improve performance when packets are
-        # targeting multiple destinations.
-        update = Signal()
-        cached_valid       = Signal()
-        cached_ip_address  = Signal(32, reset_less=True)
-        cached_mac_address = Signal(48, reset_less=True)
-        cached_timer       = WaitTimer(clk_freq*10)
-        self.submodules += cached_timer
+        request_pending    = Signal()
+        request_counter    = Signal(max=max_requests)
+        request_ip_address = Signal(32, reset_less=True)
+
+        self.request_timer = WaitTimer(100e-3*clk_freq)
+        self.comb += self.request_timer.wait.eq(request_pending & ~self.request_timer.done)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.cache = cache = LiteEthARPCache(entries=entries, clk_freq=clk_freq)
+
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
-            # Note: for simplicicy, if ARP table is busy response from arp_rx
-            # is lost. This is compensated by the protocol (retries)
+            # Note: for simplicicy, if ARP table is busy response from arp_rx is lost. This is
+            # compensated by the protocol (retries)
             If(sink.valid & sink.request,
                 NextState("SEND_REPLY")
-            ).Elif(sink.valid & sink.reply & request_pending,
+            ).Elif(sink.valid & sink.reply,
                 NextState("UPDATE_TABLE"),
-            ).Elif(request_counter == max_requests-1,
-                NextState("PRESENT_RESPONSE")
-            ).Elif(request.valid | (request_pending & request_timer.done),
+            ).Elif(request.valid,
                 NextState("CHECK_TABLE")
+            ).Elif(self.request_timer.done,
+                NextState("CHECK_REQUEST")
             )
         )
         fsm.act("SEND_REPLY",
             source.valid.eq(1),
             source.reply.eq(1),
             source.ip_address.eq(sink.ip_address),
             source.mac_address.eq(sink.mac_address),
             If(source.ready,
                 NextState("IDLE")
             )
         )
         fsm.act("UPDATE_TABLE",
-            request_pending_clr.eq(1),
-            update.eq(1),
-            NextState("CHECK_TABLE")
-        )
-        self.sync += \
-            If(update,
-                cached_valid.eq(1),
-                cached_ip_address.eq(sink.ip_address),
-                cached_mac_address.eq(sink.mac_address),
-            ).Else(
-                If(cached_timer.done,
-                    cached_valid.eq(0)
+            If(request_pending & (request_ip_address == sink.ip_address),
+                cache.update.valid.eq(1),
+                cache.update.ip_address.eq(sink.ip_address),
+                cache.update.mac_address.eq(sink.mac_address),
+                If(cache.update.ready,
+                    NextValue(request_pending, 0),
+                    NextState("PRESENT_RESPONSE")
                 )
+            ).Else(
+                NextState("IDLE")
+            )
+        )
+        fsm.act("CHECK_REQUEST",
+            If(request_counter == (max_requests - 1),
+                NextValue(response.failed, 1),
+                NextValue(request_counter, 0),
+                NextValue(request_pending, 0),
+                NextState("PRESENT_RESPONSE")
+            ).Else(
+                NextState("SEND_REQUEST")
             )
-        self.comb += cached_timer.wait.eq(~update)
+        )
         fsm.act("CHECK_TABLE",
-            If(cached_valid,
-                If(request_ip_address == cached_ip_address,
-                    request_ip_address_reset.eq(1),
-                    NextState("PRESENT_RESPONSE"),
-                ).Elif(request.ip_address == cached_ip_address,
-                    request.ready.eq(request.valid),
-                    NextState("PRESENT_RESPONSE"),
-                ).Else(
-                    request_ip_address_update.eq(request.valid),
+            cache.request.valid.eq(1),
+            cache.request.ip_address.eq(request.ip_address),
+            If(cache.response.valid,
+                request.ready.eq(1),
+                If(cache.response.error,
+                    NextValue(request_counter, 0),
+                    NextValue(request_pending, 1),
+                    NextValue(request_ip_address, request.ip_address),
                     NextState("SEND_REQUEST")
+                ).Else(
+                    NextValue(response.mac_address, cache.response.mac_address),
+                    NextState("PRESENT_RESPONSE"),
                 )
-            ).Else(
-                request_ip_address_update.eq(request.valid),
-                NextState("SEND_REQUEST")
             )
         )
         fsm.act("SEND_REQUEST",
             source.valid.eq(1),
             source.request.eq(1),
             source.ip_address.eq(request_ip_address),
             If(source.ready,
-                request_counter_reset.eq(request.valid),
-                request_counter_ce.eq(1),
-                request_pending_set.eq(1),
-                request.ready.eq(1),
+                NextValue(request_counter, request_counter + 1),
                 NextState("IDLE")
             )
         )
-        self.comb += [
-            If(request_counter == max_requests - 1,
-                response.failed.eq(1),
-                request_counter_reset.eq(1),
-                request_pending_clr.eq(1)
-            ),
-            response.mac_address.eq(cached_mac_address)
-        ]
         fsm.act("PRESENT_RESPONSE",
             response.valid.eq(1),
             If(response.ready,
+                NextValue(response.failed, 0),
                 NextState("IDLE")
             )
         )
 
 # ARP ----------------------------------------------------------------------------------------------
 
-class LiteEthARP(Module):
-    def __init__(self, mac, mac_address, ip_address, clk_freq, dw=8):
-        self.submodules.tx    = tx    = LiteEthARPTX(mac_address, ip_address, dw)
-        self.submodules.rx    = rx    = LiteEthARPRX(mac_address, ip_address, dw)
-        self.submodules.table = table = LiteEthARPTable(clk_freq)
+class LiteEthARP(LiteXModule):
+    def __init__(self, mac, mac_address, ip_address, clk_freq, entries=1, dw=8):
+        self.tx    = tx    = LiteEthARPTX(mac_address, ip_address, dw)
+        self.rx    = rx    = LiteEthARPRX(mac_address, ip_address, dw)
+        self.table = table = LiteEthARPTable(clk_freq, entries=entries)
         self.comb += [
             rx.source.connect(table.sink),
             table.source.connect(tx.sink)
         ]
         mac_port = mac.crossbar.get_port(ethernet_type_arp, dw=dw)
         self.comb += [
             tx.source.connect(mac_port.sink),
```

### Comparing `liteeth-2023.4/liteeth/core/icmp.py` & `liteeth-2023.8/liteeth/core/icmp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-from liteeth.common import *
+from litex.gen import *
 
 from litex.soc.interconnect.packet import PacketFIFO
+
+from liteeth.common import *
 from liteeth.packet import Depacketizer, Packetizer
 
 # ICMP TX ------------------------------------------------------------------------------------------
 
 class LiteEthICMPPacketizer(Packetizer):
     def __init__(self, dw=8):
         Packetizer.__init__(self,
             eth_icmp_description(dw),
             eth_ipv4_user_description(dw),
-            icmp_header)
+            icmp_header
+        )
 
 
-class LiteEthICMPTX(Module):
+class LiteEthICMPTX(LiteXModule):
     def __init__(self, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_icmp_user_description(dw))
         self.source = source = stream.Endpoint(eth_ipv4_user_description(dw))
 
         # # #
 
         # Packetizer.
-        self.submodules.packetizer = packetizer = LiteEthICMPPacketizer(dw)
+        self.packetizer = packetizer = LiteEthICMPPacketizer(dw)
         self.comb += sink.connect(packetizer.sink, keep={
             "valid",
             "last",
             "ready",
             "msgtype",
             "code",
             "checksum",
             "quench",
             "data",
-            "last_be"})
+            "last_be"
+        })
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(packetizer.source.valid,
                 NextState("SEND")
             )
         )
         self.comb += [
             packetizer.source.connect(source, omit={"valid", "ready"}),
@@ -65,27 +69,27 @@
     def __init__(self, dw=8):
         Depacketizer.__init__(self,
             eth_ipv4_user_description(dw),
             eth_icmp_description(dw),
             icmp_header)
 
 
-class LiteEthICMPRX(Module):
+class LiteEthICMPRX(LiteXModule):
     def __init__(self, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_ipv4_user_description(dw))
         self.source = source = stream.Endpoint(eth_icmp_user_description(dw))
 
         # # #
 
         # Depacketizer.
-        self.submodules.depacketizer = depacketizer = LiteEthICMPDepacketizer(dw)
+        self.depacketizer = depacketizer = LiteEthICMPDepacketizer(dw)
         self.comb += sink.connect(depacketizer.sink)
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(depacketizer.source.valid,
                 NextState("DROP"),
                 If(sink.protocol == icmp_protocol,
                     If(depacketizer.source.msgtype == icmp_type_ping_request,
                         NextState("RECEIVE")
                     )
@@ -97,15 +101,16 @@
                 "last",
                 "msgtype",
                 "code",
                 "checksum",
                 "quench",
                 "data",
                 "error",
-                "last_be"}),
+                "last_be"
+            }),
             source.ip_address.eq(sink.ip_address),
             source.length.eq(sink.length - icmp_header.length),
         ]
         fsm.act("RECEIVE",
             depacketizer.source.connect(source, keep={"valid", "ready"}),
             If(source.valid & source.ready,
                 If(source.last,
@@ -120,40 +125,46 @@
                depacketizer.source.ready,
                 NextState("IDLE")
             )
         )
 
 # ICMP Echo ----------------------------------------------------------------------------------------
 
-class LiteEthICMPEcho(Module):
-    def __init__(self, dw=8):
+class LiteEthICMPEcho(LiteXModule):
+    def __init__(self, dw=8, fifo_depth=128):
         self.sink   = sink   = stream.Endpoint(eth_icmp_user_description(dw))
         self.source = source = stream.Endpoint(eth_icmp_user_description(dw))
 
         # # #
 
-        self.submodules.buffer = PacketFIFO(eth_icmp_user_description(dw),
-            payload_depth = 128//(dw//8),
+        self.buffer = PacketFIFO(eth_icmp_user_description(dw),
+            payload_depth = fifo_depth//(dw//8),
             param_depth   = 1,
             buffered      = True
         )
         self.comb += [
-            sink.connect(self.buffer.sink),
+            # Connect to buffer when length <= buffer's depth.
+            If(sink.length <= fifo_depth,
+                sink.connect(self.buffer.sink)
+            # Else drop.
+            ).Else(
+                sink.ready.eq(1)
+            ),
             self.buffer.source.connect(source, omit={"checksum"}),
             self.source.msgtype.eq(icmp_type_ping_reply),
             self.source.checksum.eq(self.buffer.source.checksum + 0x800 + (self.buffer.source.checksum >= 0xf800))
         ]
 
 # ICMP ---------------------------------------------------------------------------------------------
 
-class LiteEthICMP(Module):
-    def __init__(self, ip, ip_address, dw=8):
-        self.submodules.tx   = tx   = LiteEthICMPTX(ip_address, dw)
-        self.submodules.rx   = rx   = LiteEthICMPRX(ip_address, dw)
-        self.submodules.echo = echo = LiteEthICMPEcho(dw)
+class LiteEthICMP(LiteXModule):
+    def __init__(self, ip, ip_address, dw=8, fifo_depth=128):
+        self.tx   = tx   = LiteEthICMPTX(ip_address, dw)
+        self.rx   = rx   = LiteEthICMPRX(ip_address, dw)
+        self.echo = echo = LiteEthICMPEcho(dw, fifo_depth=fifo_depth)
         self.comb += [
             rx.source.connect(echo.sink),
             echo.source.connect(tx.sink)
         ]
         ip_port = ip.crossbar.get_port(icmp_protocol, dw)
         self.comb += [
             tx.source.connect(ip_port.sink),
```

### Comparing `liteeth-2023.4/liteeth/core/ip.py` & `liteeth-2023.8/liteeth/core/ip.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.crossbar import LiteEthCrossbar
 
 from liteeth.packet import Depacketizer, Packetizer
 
 # IP Crossbar --------------------------------------------------------------------------------------
 
@@ -41,15 +43,15 @@
         self.users[protocol] = port
         return port
 
 # IP Checksum --------------------------------------------------------------------------------------
 
 @ResetInserter()
 @CEInserter()
-class LiteEthIPV4Checksum(Module):
+class LiteEthIPV4Checksum(LiteXModule):
     def __init__(self, words_per_clock_cycle=1, skip_checksum=False):
         self.header = Signal(ipv4_header.length*8)
         self.value  = Signal(16)
         self.done   = Signal()
 
         # # #
 
@@ -83,32 +85,33 @@
 # IP TX --------------------------------------------------------------------------------------------
 
 class LiteEthIPV4Packetizer(Packetizer):
     def __init__(self, dw=8):
         Packetizer.__init__(self,
             eth_ipv4_description(dw),
             eth_mac_description(dw),
-            ipv4_header)
+            ipv4_header
+        )
 
 
-class LiteEthIPTX(Module):
+class LiteEthIPTX(LiteXModule):
     def __init__(self, mac_address, ip_address, arp_table, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_ipv4_user_description(dw))
         self.source = source = stream.Endpoint(eth_mac_description(dw))
         self.target_unreachable = Signal()
 
         # # #
 
         # Checksum.
-        self.submodules.checksum = checksum = LiteEthIPV4Checksum(skip_checksum=True)
+        self.checksum = checksum = LiteEthIPV4Checksum(skip_checksum=True)
         self.comb += checksum.ce.eq(sink.valid)
         self.comb += checksum.reset.eq(source.valid & source.last & source.ready)
 
         # Packetizer.
-        self.submodules.packetizer = packetizer = LiteEthIPV4Packetizer(dw)
+        self.packetizer = packetizer = LiteEthIPV4Packetizer(dw)
         self.comb += [
             sink.connect(packetizer.sink, keep={
                 "last",
                 "last_be",
                 "protocol",
                 "data",
             }),
@@ -124,15 +127,15 @@
             checksum.header.eq(packetizer.header),
             packetizer.sink.checksum.eq(checksum.value)
         ]
 
         target_mac = Signal(48, reset_less=True)
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(packetizer.source.valid,
                 # Broadcast.
                 If(sink.ip_address[0:8] == bcast_ip_mask,
                     NextValue(target_mac, bcast_mac_address),
                     NextState("SEND")
                 # Multicast.
@@ -185,38 +188,39 @@
 # IP RX --------------------------------------------------------------------------------------------
 
 class LiteEthIPV4Depacketizer(Depacketizer):
     def __init__(self, dw=8):
         Depacketizer.__init__(self,
             eth_mac_description(dw),
             eth_ipv4_description(dw),
-            ipv4_header)
+            ipv4_header
+        )
 
 
-class LiteEthIPRX(Module):
+class LiteEthIPRX(LiteXModule):
     def __init__(self, mac_address, ip_address, with_broadcast=True, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_mac_description(dw))
         self.source = source = stream.Endpoint(eth_ipv4_user_description(dw))
 
         # # #
 
         # Depacketizer.
-        self.submodules.depacketizer = depacketizer = LiteEthIPV4Depacketizer(dw)
+        self.depacketizer = depacketizer = LiteEthIPV4Depacketizer(dw)
         self.comb += sink.connect(depacketizer.sink)
 
         # Checksum.
-        self.submodules.checksum = checksum = LiteEthIPV4Checksum(skip_checksum=False)
+        self.checksum = checksum = LiteEthIPV4Checksum(skip_checksum=False)
         self.comb += [
             checksum.header.eq(depacketizer.header),
             checksum.reset.eq(~depacketizer.source.valid),
             checksum.ce.eq(1)
         ]
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(depacketizer.source.valid & checksum.done,
                 NextState("DROP"),
                 If(((depacketizer.source.target_ip == ip_address) | with_broadcast) &
                    (depacketizer.source.version == 0x4) &
                    (depacketizer.source.ihl == 0x5) &
                    (checksum.value == 0),
@@ -227,15 +231,15 @@
         self.comb += [
             depacketizer.source.connect(source, keep={
                 "last",
                 "protocol",
                 "data",
                 "error",
                 "last_be"}),
-            source.length.eq(depacketizer.source.total_length - (0x5*4)),
+            source.length.eq(depacketizer.source.total_length - ipv4_header_length),
             source.ip_address.eq(depacketizer.source.sender_ip),
         ]
         fsm.act("RECEIVE",
             depacketizer.source.connect(source, keep={"valid", "ready"}),
             If(source.valid & source.ready,
                 If(source.last,
                     NextState("IDLE")
@@ -249,21 +253,21 @@
                depacketizer.source.ready,
                 NextState("IDLE")
             )
         )
 
 # IP -----------------------------------------------------------------------------------------------
 
-class LiteEthIP(Module):
+class LiteEthIP(LiteXModule):
     def __init__(self, mac, mac_address, ip_address, arp_table, with_broadcast=True, dw=8):
-        self.submodules.tx = tx = LiteEthIPTX(mac_address, ip_address, arp_table, dw=dw)
-        self.submodules.rx = rx = LiteEthIPRX(mac_address, ip_address, with_broadcast, dw=dw)
+        self.tx = tx = LiteEthIPTX(mac_address, ip_address, arp_table, dw=dw)
+        self.rx = rx = LiteEthIPRX(mac_address, ip_address, with_broadcast, dw=dw)
         mac_port = mac.crossbar.get_port(ethernet_type_ip, dw)
         self.comb += [
             tx.source.connect(mac_port.sink),
             mac_port.source.connect(rx.sink)
         ]
-        self.submodules.crossbar = crossbar = LiteEthIPV4Crossbar(dw)
+        self.crossbar = crossbar = LiteEthIPV4Crossbar(dw)
         self.comb += [
             crossbar.master.source.connect(tx.sink),
             rx.source.connect(crossbar.master.sink)
         ]
```

### Comparing `liteeth-2023.4/liteeth/core/udp.py` & `liteeth-2023.8/liteeth/core/udp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-from liteeth.common import *
-from liteeth.crossbar import LiteEthCrossbar
+from litex.gen import *
 
 from litex.soc.interconnect import stream
 
+from liteeth.common import *
+from liteeth.crossbar import LiteEthCrossbar
 from liteeth.packet import Depacketizer, Packetizer
 
 # UDP Crossbar -------------------------------------------------------------------------------------
 
 class LiteEthUDPMasterPort:
     def __init__(self, dw):
         self.dw     = dw
@@ -44,42 +45,42 @@
         user_port     = LiteEthUDPUserPort(dw)
         internal_port = LiteEthUDPUserPort(self.dw)
 
         # TX
         # ---
 
         # CDC.
-        self.submodules.tx_cdc = tx_cdc = stream.ClockDomainCrossing(
+        self.tx_cdc = tx_cdc = stream.ClockDomainCrossing(
             layout  = eth_udp_user_description(user_port.dw),
             cd_from = cd,
             cd_to   ="sys"
         )
         self.comb += user_port.sink.connect(tx_cdc.sink)
 
         # Data-Width Conversion.
-        self.submodules.tx_converter = tx_converter = stream.StrideConverter(
+        self.tx_converter = tx_converter = stream.StrideConverter(
             description_from = eth_udp_user_description(user_port.dw),
             description_to   = eth_udp_user_description(self.dw)
         )
         self.comb += tx_cdc.source.connect(tx_converter.sink)
 
         # Interface.
         self.comb += tx_converter.source.connect(internal_port.sink)
 
         # RX
         # --
         # Data-Width Conversion.
-        self.submodules.rx_converter = rx_converter = stream.StrideConverter(
+        self.rx_converter = rx_converter = stream.StrideConverter(
             description_from = eth_udp_user_description(self.dw),
             description_to   = eth_udp_user_description(user_port.dw)
         )
         self.comb += internal_port.source.connect(rx_converter.sink)
 
         # CDC.
-        self.submodules.rx_cdc = rx_cdc = stream.ClockDomainCrossing(
+        self.rx_cdc = rx_cdc = stream.ClockDomainCrossing(
             layout  = eth_udp_user_description(user_port.dw),
             cd_from = "sys",
             cd_to   = cd
         )
         self.comb += rx_converter.source.connect(rx_cdc.sink)
 
         # Interface.
@@ -94,26 +95,27 @@
 # UDP TX -------------------------------------------------------------------------------------------
 
 class LiteEthUDPPacketizer(Packetizer):
     def __init__(self, dw=8):
         Packetizer.__init__(self,
             eth_udp_description(dw),
             eth_ipv4_user_description(dw),
-            udp_header)
+            udp_header
+        )
 
 
-class LiteEthUDPTX(Module):
+class LiteEthUDPTX(LiteXModule):
     def __init__(self, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_udp_user_description(dw))
         self.source = source = stream.Endpoint(eth_ipv4_user_description(dw))
 
         # # #
 
         # Packetizer.
-        self.submodules.packetizer = packetizer = LiteEthUDPPacketizer(dw=dw)
+        self.packetizer = packetizer = LiteEthUDPPacketizer(dw=dw)
 
         # Data-Path.
         self.comb += [
             sink.connect(packetizer.sink, keep={
                 "valid",
                 "ready",
                 "last",
@@ -122,15 +124,15 @@
                 "dst_port",
                 "data"}),
             packetizer.sink.length.eq(sink.length + udp_header.length),
             packetizer.sink.checksum.eq(0), # UDP Checksum is not used, we only rely on MAC CRC.
         ]
 
         # Control-Path (FSM).
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(packetizer.source.valid,
                 NextState("SEND")
             )
         )
         fsm.act("SEND",
             packetizer.source.connect(source),
@@ -147,26 +149,27 @@
 # UDP RX -------------------------------------------------------------------------------------------
 
 class LiteEthUDPDepacketizer(Depacketizer):
     def __init__(self, dw=8):
         Depacketizer.__init__(self,
             eth_ipv4_user_description(dw),
             eth_udp_description(dw),
-            udp_header)
+            udp_header
+        )
 
 
-class LiteEthUDPRX(Module):
+class LiteEthUDPRX(LiteXModule):
     def __init__(self, ip_address, dw=8):
         self.sink   = sink   = stream.Endpoint(eth_ipv4_user_description(dw))
         self.source = source = stream.Endpoint(eth_udp_user_description(dw))
 
         # # #
 
         # Depacketizer.
-        self.submodules.depacketizer = depacketizer = LiteEthUDPDepacketizer(dw)
+        self.depacketizer = depacketizer = LiteEthUDPDepacketizer(dw)
 
         # Data-Path.
         self.comb += [
             sink.connect(depacketizer.sink),
             depacketizer.source.connect(source, keep={
                 "src_port",
                 "dst_port",
@@ -174,15 +177,15 @@
                 "error"}),
             source.ip_address.eq(sink.ip_address),
             source.length.eq(depacketizer.source.length - udp_header.length),
         ]
 
         # Control-Path (FSM).
         count = Signal(16)
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(count, dw//8),
             If(depacketizer.source.valid,
                 NextState("DROP"),
                 If(sink.protocol == udp_protocol,
                     NextState("RECEIVE")
                 )
@@ -223,21 +226,21 @@
                depacketizer.source.ready,
                 NextState("IDLE")
             )
         )
 
 # UDP ----------------------------------------------------------------------------------------------
 
-class LiteEthUDP(Module):
+class LiteEthUDP(LiteXModule):
     def __init__(self, ip, ip_address, dw=8):
-        self.submodules.tx = tx = LiteEthUDPTX(ip_address, dw)
-        self.submodules.rx = rx = LiteEthUDPRX(ip_address, dw)
+        self.tx = tx = LiteEthUDPTX(ip_address, dw)
+        self.rx = rx = LiteEthUDPRX(ip_address, dw)
         ip_port = ip.crossbar.get_port(udp_protocol, dw)
         self.comb += [
             tx.source.connect(ip_port.sink),
             ip_port.source.connect(rx.sink)
         ]
-        self.submodules.crossbar = crossbar = LiteEthUDPCrossbar(dw)
+        self.crossbar = crossbar = LiteEthUDPCrossbar(dw)
         self.comb += [
             crossbar.master.source.connect(tx.sink),
             rx.source.connect(crossbar.master.sink)
         ]
```

### Comparing `liteeth-2023.4/liteeth/crossbar.py` & `liteeth-2023.8/liteeth/crossbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from collections import OrderedDict
 
+from litex.gen import *
+
 from liteeth.common import *
 
 from litex.soc.interconnect.packet import Arbiter, Dispatcher
 
 # Crossbar -----------------------------------------------------------------------------------------
 
-class LiteEthCrossbar(Module):
+class LiteEthCrossbar(LiteXModule):
     def __init__(self, master_port, dispatch_param, dw=8):
         self.users  = OrderedDict()
         self.master = master_port(dw)
         self.dispatch_param = dispatch_param
 
     # overload this in derived classes
     def get_port(self, *args, **kwargs):
         pass
 
     def do_finalize(self):
         # TX arbitrate
         sinks = [port.sink for port in self.users.values()]
-        self.submodules.arbiter = Arbiter(sinks, self.master.source)
+        self.arbiter = Arbiter(sinks, self.master.source)
 
         # RX dispatch
         sources = [port.source for port in self.users.values()]
-        self.submodules.dispatcher = Dispatcher(self.master.sink, sources, one_hot=True)
+        self.dispatcher = Dispatcher(self.master.sink, sources, one_hot=True)
         dispatch_sig = getattr(self.master.sink, self.dispatch_param)
         for i, (k, v) in enumerate(self.users.items()):
             self.comb += If(dispatch_sig == k, self.dispatcher.sel.eq(2**i))
```

### Comparing `liteeth-2023.4/liteeth/frontend/etherbone.py` & `liteeth-2023.8/liteeth/frontend/etherbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 """
 Etherbone
 
 CERN's Etherbone protocol is initially used to run a Wishbone bus over an
 ethernet network. This re-implementation is meant to be run over ethernet
 and introduces some limitations:
 - no address spaces (rca/bca/wca/wff)
 - 32bits data and address
 - 1 record per frame
 """
 
+from litex.gen import *
+
 from liteeth.common import *
 
 from litex.soc.interconnect import wishbone
 from litex.soc.interconnect.packet import *
 
 from liteeth.packet import Depacketizer, Packetizer
 
 # Etherbone Packet ---------------------------------------------------------------------------------
 
 class LiteEthEtherbonePacketPacketizer(Packetizer):
     def __init__(self):
         Packetizer.__init__(self,
             eth_etherbone_packet_description(32),
             eth_udp_user_description(32),
-            etherbone_packet_header)
+            etherbone_packet_header
+        )
 
 
-class LiteEthEtherbonePacketTX(Module):
+class LiteEthEtherbonePacketTX(LiteXModule):
     def __init__(self, udp_port):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_packet_user_description(32))
         self.source = source = stream.Endpoint(eth_udp_user_description(32))
 
         # # #
 
-        self.submodules.packetizer = packetizer = LiteEthEtherbonePacketPacketizer()
+        self.packetizer = packetizer = LiteEthEtherbonePacketPacketizer()
         self.comb += [
             sink.connect(packetizer.sink, keep={"valid", "last", "last_be", "ready", "data"}),
             sink.connect(packetizer.sink, keep={"pf", "pr", "nr"}),
             packetizer.sink.version.eq(etherbone_version),
             packetizer.sink.magic.eq(etherbone_magic),
             packetizer.sink.port_size.eq(32//8),
             packetizer.sink.addr_size.eq(32//8),
         ]
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(packetizer.source.valid,
                 NextState("SEND")
             )
         )
         fsm.act("SEND",
             packetizer.source.connect(source),
@@ -70,25 +73,25 @@
     def __init__(self):
         Depacketizer.__init__(self,
             eth_udp_user_description(32),
             eth_etherbone_packet_description(32),
             etherbone_packet_header)
 
 
-class LiteEthEtherbonePacketRX(Module):
+class LiteEthEtherbonePacketRX(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(eth_udp_user_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_packet_user_description(32))
 
         # # #
 
-        self.submodules.depacketizer = depacketizer = LiteEthEtherbonePacketDepacketizer()
+        self.depacketizer = depacketizer = LiteEthEtherbonePacketDepacketizer()
         self.comb += sink.connect(depacketizer.sink)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(depacketizer.source.valid,
                 NextState("DROP"),
                 If(depacketizer.source.magic == etherbone_magic,
                     NextState("RECEIVE")
                 )
             )
@@ -114,43 +117,43 @@
                depacketizer.source.last &
                depacketizer.source.ready,
                 NextState("IDLE")
             )
         )
 
 
-class LiteEthEtherbonePacket(Module):
+class LiteEthEtherbonePacket(LiteXModule):
     def __init__(self, udp, udp_port, cd="sys"):
-        self.submodules.tx = tx = LiteEthEtherbonePacketTX(udp_port)
-        self.submodules.rx = rx = LiteEthEtherbonePacketRX()
+        self.tx = tx = LiteEthEtherbonePacketTX(udp_port)
+        self.rx = rx = LiteEthEtherbonePacketRX()
         udp_port = udp.crossbar.get_port(udp_port, dw=32, cd=cd)
         self.comb += [
             tx.source.connect(udp_port.sink),
             udp_port.source.connect(rx.sink)
         ]
         self.sink, self.source = self.tx.sink, self.rx.source
 
 
 # Etherbone Probe ----------------------------------------------------------------------------------
 
-class LiteEthEtherboneProbe(Module):
+class LiteEthEtherboneProbe(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_packet_user_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_packet_user_description(32))
 
         # # #
 
-        self.submodules.fifo = fifo = PacketFIFO(eth_etherbone_packet_user_description(32),
+        self.fifo = fifo = PacketFIFO(eth_etherbone_packet_user_description(32),
             payload_depth = 1,
             param_depth   = 1,
             buffered      = False
         )
         self.comb += sink.connect(fifo.sink)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(fifo.source.valid,
                 NextState("PROBE_RESPONSE")
             )
         )
         fsm.act("PROBE_RESPONSE",
             fifo.source.connect(source),
@@ -177,36 +180,36 @@
     def __init__(self):
         Depacketizer.__init__(self,
             eth_etherbone_packet_user_description(32),
             eth_etherbone_record_description(32),
             etherbone_record_header)
 
 
-class LiteEthEtherboneRecordReceiver(Module):
+class LiteEthEtherboneRecordReceiver(LiteXModule):
     def __init__(self, buffer_depth=4):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_record_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_mmap_description(32))
 
         # # #
 
         assert buffer_depth <= 256
-        self.submodules.fifo = fifo = PacketFIFO(eth_etherbone_record_description(32),
+        self.fifo = fifo = PacketFIFO(eth_etherbone_record_description(32),
             payload_depth = buffer_depth,
             param_depth   = 1,
             buffered      = True
         )
         self.comb += sink.connect(fifo.sink)
 
         base_addr = Signal(32, reset_less=True)
         base_addr_update = Signal()
         self.sync += If(base_addr_update, base_addr.eq(fifo.source.data))
 
         count = Signal(max=512, reset_less=True)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             fifo.source.ready.eq(1),
             NextValue(count, 0),
             If(fifo.source.valid,
                 base_addr_update.eq(1),
                 If(fifo.source.wcount,
                     NextState("RECEIVE_WRITES")
@@ -256,30 +259,30 @@
                 If(source.last,
                     NextState("IDLE")
                 )
             )
         )
 
 
-class LiteEthEtherboneRecordSender(Module):
+class LiteEthEtherboneRecordSender(LiteXModule):
     def __init__(self, buffer_depth=4):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_mmap_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_record_description(32))
 
         # # #
 
         assert buffer_depth <= 256
-        self.submodules.fifo = fifo = PacketFIFO(eth_etherbone_mmap_description(32),
+        self.fifo = fifo = PacketFIFO(eth_etherbone_mmap_description(32),
             payload_depth = buffer_depth,
             param_depth   = 1,
             buffered      = True
         )
         self.comb += sink.connect(fifo.sink)
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(fifo.source.valid,
                 NextState("SEND_BASE_ADDRESS")
             )
         )
         self.comb += [
             source.byte_enable.eq(fifo.source.be),
@@ -307,24 +310,24 @@
                 If(source.last,
                     NextState("IDLE")
                 )
             )
         )
 
 
-class LiteEthEtherboneRecord(Module):
+class LiteEthEtherboneRecord(LiteXModule):
     def __init__(self, endianness="big", buffer_depth=4):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_packet_user_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_packet_user_description(32))
 
         # # #
 
         # Receive record, decode it and generate mmap stream
-        self.submodules.depacketizer = depacketizer = LiteEthEtherboneRecordDepacketizer()
-        self.submodules.receiver = receiver = LiteEthEtherboneRecordReceiver(buffer_depth)
+        self.depacketizer = depacketizer = LiteEthEtherboneRecordDepacketizer()
+        self.receiver = receiver = LiteEthEtherboneRecordReceiver(buffer_depth)
         self.comb += [
             sink.connect(depacketizer.sink),
             depacketizer.source.connect(receiver.sink)
         ]
         if endianness == "big":
             self.comb += receiver.sink.data.eq(reverse_bytes(depacketizer.source.data))
 
@@ -335,40 +338,40 @@
             If(sink.valid & sink.ready,
                 If(first, last_ip_address.eq(sink.ip_address)),
                 first.eq(sink.last)
             )
         ]
 
         # Receive MMAP stream, encode it and send records
-        self.submodules.sender     = sender     = LiteEthEtherboneRecordSender(buffer_depth)
-        self.submodules.packetizer = packetizer = LiteEthEtherboneRecordPacketizer()
+        self.sender     = sender     = LiteEthEtherboneRecordSender(buffer_depth)
+        self.packetizer = packetizer = LiteEthEtherboneRecordPacketizer()
         self.comb += [
             sender.source.connect(packetizer.sink),
             packetizer.source.connect(source),
             source.length.eq(etherbone_record_header.length +
                 (sender.source.wcount != 0)*4 + sender.source.wcount*4 +
                 (sender.source.rcount != 0)*4 + sender.source.rcount*4),
             source.ip_address.eq(last_ip_address)
         ]
         if endianness == "big":
             self.comb += packetizer.sink.data.eq(reverse_bytes(sender.source.data))
 
 # Etherbone Wishbone Master ------------------------------------------------------------------------
 
-class LiteEthEtherboneWishboneMaster(Module):
+class LiteEthEtherboneWishboneMaster(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(eth_etherbone_mmap_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_mmap_description(32))
         self.bus    = bus    = wishbone.Interface()
 
         # # #
 
         data_update = Signal()
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             sink.ready.eq(1),
             If(sink.valid,
                 sink.ready.eq(0),
                 If(sink.we,
                     NextState("WRITE_DATA")
                 ).Else(
@@ -418,23 +421,23 @@
                     NextState("READ_DATA")
                 )
             )
         )
 
 # Etherbone Wishbone Slave -------------------------------------------------------------------------
 
-class LiteEthEtherboneWishboneSlave(Module):
+class LiteEthEtherboneWishboneSlave(LiteXModule):
     def __init__(self):
         self.bus    = bus    = wishbone.Interface()
         self.sink   = sink   = stream.Endpoint(eth_etherbone_mmap_description(32))
         self.source = source = stream.Endpoint(eth_etherbone_mmap_description(32))
 
         # # #
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             sink.ready.eq(1),
             If(bus.stb & bus.cyc,
                 If(bus.we,
                     NextState("SEND_WRITE")
                 ).Else(
                     NextState("SEND_READ")
@@ -476,31 +479,31 @@
                 NextState("IDLE")
             )
         )
 
 
 # Etherbone ----------------------------------------------------------------------------------------
 
-class LiteEthEtherbone(Module):
+class LiteEthEtherbone(LiteXModule):
     def __init__(self, udp, udp_port, mode="master", buffer_depth=4, cd="sys"):
         # Encode/encode etherbone packets
-        self.submodules.packet = packet = LiteEthEtherbonePacket(udp, udp_port, cd)
+        self.packet = packet = LiteEthEtherbonePacket(udp, udp_port, cd)
 
         # Packets can be probe (etherbone discovering) or records with writes and reads
-        self.submodules.probe  = probe = LiteEthEtherboneProbe()
-        self.submodules.record = record = LiteEthEtherboneRecord(buffer_depth=buffer_depth)
+        self.probe  = probe = LiteEthEtherboneProbe()
+        self.record = record = LiteEthEtherboneRecord(buffer_depth=buffer_depth)
 
         # Arbitrate/dispatch probe/records packets
         dispatcher = Dispatcher(packet.source, [probe.sink, record.sink])
         self.comb += dispatcher.sel.eq(~packet.source.pf)
         arbiter = Arbiter([probe.source, record.source], packet.sink)
         self.submodules += dispatcher, arbiter
 
         # Create MMAP wishbone
-        self.submodules.wishbone = {
+        self.wishbone = {
             "master": LiteEthEtherboneWishboneMaster(),
             "slave":  LiteEthEtherboneWishboneSlave(),
         }[mode]
         self.comb += [
             record.receiver.source.connect(self.wishbone.sink),
             self.wishbone.source.connect(record.sender.sink)
         ]
```

### Comparing `liteeth-2023.4/liteeth/frontend/stream.py` & `liteeth-2023.8/liteeth/frontend/stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2021 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
+from litex.gen import *
+
 from liteeth.common import *
 
 # Stream to UDP TX -----------------------------------------------------------------------------------
 
-class LiteEthStream2UDPTX(Module):
+class LiteEthStream2UDPTX(LiteXModule):
     def __init__(self, ip_address, udp_port, data_width=8, fifo_depth=None):
         self.sink   = sink   = stream.Endpoint(eth_tty_tx_description(data_width))
         self.source = source = stream.Endpoint(eth_udp_user_description(data_width))
 
         # # #
 
         ip_address = convert_ip(ip_address)
@@ -26,47 +28,62 @@
                 source.ip_address.eq(ip_address),
                 source.length.eq(data_width//8)
             ]
         else:
             level   = Signal(max=fifo_depth+1)
             counter = Signal(max=fifo_depth+1)
 
-            self.submodules.fifo = fifo = stream.SyncFIFO([("data", data_width)], fifo_depth, buffered=True)
+            _ip_address = Signal(32)
+            _udp_port   = Signal(16)
+
+            self.fifo = fifo = stream.SyncFIFO([("data", data_width)], fifo_depth, buffered=True)
             self.comb += sink.connect(fifo.sink)
 
-            self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+            self.fsm = fsm = FSM(reset_state="IDLE")
             fsm.act("IDLE",
-                # Send FIFO contents when we have a full-packet or when FIFO is full.
-                If((fifo.source.valid & fifo.source.last) | ~fifo.sink.ready,
-                    NextValue(level, fifo.level),
-                    NextValue(counter, 0),
+                NextValue(counter, 0),
+                NextValue(_ip_address, ip_address),
+                NextValue(_udp_port,     udp_port),
+                # Send FIFO contenst when:
+                # - We have a full packet:
+                If(fifo.sink.valid & fifo.sink.ready & fifo.sink.last,
+                    NextValue(level, fifo.level + 1), # +1 for level latency.
                     NextState("SEND")
-                )
+                ),
+                # - Or when FIFO is full.
+                If(~fifo.sink.ready,
+                    NextValue(level, fifo_depth),
+                    NextState("SEND")
+                ),
             )
             fsm.act("SEND",
                 source.valid.eq(1),
                 source.last.eq(counter == (level - 1)),
-                source.src_port.eq(udp_port),
-                source.dst_port.eq(udp_port),
-                source.ip_address.eq(ip_address),
+                source.src_port.eq(_udp_port),
+                source.dst_port.eq(_udp_port),
+                source.ip_address.eq(_ip_address),
                 source.length.eq(level * (data_width//8)),
                 source.data.eq(fifo.source.data),
-                source.last_be.eq({32:0b1000, 8:0b1}[data_width]),
+                source.last_be.eq({
+                    32 : 0b1000,
+                    16 : 0b10,
+                    8  : 0b1}[data_width]
+                ),
                 If(source.ready,
                     fifo.source.ready.eq(1),
                     NextValue(counter, counter + 1),
                     If(source.last,
                         NextState("IDLE")
                     )
                 )
             )
 
 # UDP to Stream RX ---------------------------------------------------------------------------------
 
-class LiteEthUDP2StreamRX(Module):
+class LiteEthUDP2StreamRX(LiteXModule):
     def __init__(self, ip_address=None, udp_port=None, data_width=8, fifo_depth=None, with_broadcast=True):
         self.sink   = sink   = stream.Endpoint(eth_udp_user_description(data_width))
         self.source = source = stream.Endpoint(eth_tty_rx_description(data_width))
 
         # # #
 
         valid = Signal(reset=1)
@@ -84,31 +101,31 @@
         if fifo_depth is None:
             self.comb += [
                 sink.connect(source, keep={"last", "data", "error"}),
                 source.valid.eq(sink.valid & valid),
                 sink.ready.eq(source.ready | ~valid)
             ]
         else:
-            self.submodules.fifo = fifo = stream.SyncFIFO(
+            self.fifo = fifo = stream.SyncFIFO(
                 layout   = [("data", data_width), ("error", 1)],
                 depth    = fifo_depth,
                 buffered = True,
             )
             self.comb += [
                 sink.connect(fifo.sink, keep={"last", "data", "error"}),
                 fifo.sink.valid.eq(sink.valid & valid),
                 sink.ready.eq(fifo.sink.ready | ~valid),
                 fifo.source.connect(source)
             ]
 
 # UDP Streamer -------------------------------------------------------------------------------------
 
-class LiteEthUDPStreamer(Module):
+class LiteEthUDPStreamer(LiteXModule):
     def __init__(self, udp, ip_address, udp_port, data_width=8, rx_fifo_depth=64, tx_fifo_depth=64, with_broadcast=True, cd="sys"):
-        self.submodules.tx = tx = LiteEthStream2UDPTX(ip_address, udp_port, data_width, tx_fifo_depth)
-        self.submodules.rx = rx = LiteEthUDP2StreamRX(ip_address, udp_port, data_width, rx_fifo_depth, with_broadcast)
+        self.tx = tx = LiteEthStream2UDPTX(ip_address, udp_port, data_width, tx_fifo_depth)
+        self.rx = rx = LiteEthUDP2StreamRX(ip_address, udp_port, data_width, rx_fifo_depth, with_broadcast)
         udp_port = udp.crossbar.get_port(udp_port, dw=data_width, cd=cd)
         self.comb += [
             tx.source.connect(udp_port.sink),
             udp_port.source.connect(rx.sink)
         ]
         self.sink, self.source = self.tx.sink, self.rx.source
```

### Comparing `liteeth-2023.4/liteeth/mac/__init__.py` & `liteeth-2023.8/liteeth/mac/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 #
 # This file is part of LiteEth.
 #
 # Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2023 LumiGuide Fietsdetectie B.V. <goemansrowan@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from liteeth.common import *
 from liteeth.mac.common import *
 from liteeth.mac.core import LiteEthMACCore
 from liteeth.mac.wishbone import LiteEthMACWishboneInterface
 
 # MAC ----------------------------------------------------------------------------------------------
 
 class LiteEthMAC(Module, AutoCSR):
     def __init__(self, phy, dw,
-        interface         = "crossbar",
-        endianness        = "big",
-        with_preamble_crc = True,
-        nrxslots          = 2,
-        ntxslots          = 2,
-        hw_mac            = None,
-        timestamp         = None,
-        full_memory_we    = False,
-        with_sys_datapath = False):
-
+        interface          = "crossbar",
+        endianness         = "big",
+        with_preamble_crc  = True,
+        nrxslots           = 2,
+        rxslots_read_only  = True,
+        ntxslots           = 2,
+        txslots_write_only = False,
+        hw_mac             = None,
+        timestamp          = None,
+        full_memory_we     = False,
+        with_sys_datapath  = False,
+        tx_cdc_depth       = 32,
+        tx_cdc_buffered    = False,
+        rx_cdc_depth       = 32,
+        rx_cdc_buffered    = False,
+    ):
         assert dw%8 == 0
         assert interface  in ["crossbar", "wishbone", "hybrid"]
         assert endianness in ["big", "little"]
 
         self.submodules.core = LiteEthMACCore(
             phy               = phy,
             dw                = dw,
             with_sys_datapath = with_sys_datapath,
-            with_preamble_crc = with_preamble_crc
+            with_preamble_crc = with_preamble_crc,
+            tx_cdc_depth      = tx_cdc_depth,
+            tx_cdc_buffered   = tx_cdc_buffered,
+            rx_cdc_depth      = rx_cdc_depth,
+            rx_cdc_buffered   = rx_cdc_buffered,
         )
         self.csrs = []
         if interface == "crossbar":
             self.submodules.crossbar     = LiteEthMACCrossbar(dw)
             self.submodules.packetizer   = LiteEthMACPacketizer(dw)
             self.submodules.depacketizer = LiteEthMACDepacketizer(dw)
             self.comb += [
@@ -47,16 +58,16 @@
         else:
             # Wishbone MAC
             self.rx_slots  = CSRConstant(nrxslots)
             self.tx_slots  = CSRConstant(ntxslots)
             self.slot_size = CSRConstant(2**bits_for(eth_mtu))
             wishbone_interface = LiteEthMACWishboneInterface(
                 dw         = dw,
-                nrxslots   = nrxslots,
-                ntxslots   = ntxslots,
+                nrxslots   = nrxslots, rxslots_read_only  = rxslots_read_only,
+                ntxslots   = ntxslots, txslots_write_only = txslots_write_only,
                 endianness = endianness,
                 timestamp  = timestamp,
             )
             # On some targets (Intel/Altera), the complex ports aren't inferred
             # as block ram, but are created with LUTs.  FullMemoryWe splits such
             # `Memory` instances up into 4 separate memory blocks, each
             # containing 8 bits which gets inferred correctly on intel/altera.
```

### Comparing `liteeth-2023.4/liteeth/mac/common.py` & `liteeth-2023.8/liteeth/mac/common.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/mac/core.py` & `liteeth-2023.8/liteeth/mac/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 #
 # This file is part of LiteEth.
 #
 # Copyright (c) 2015-2021 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2015-2017 Sebastien Bourdeauducq <sb@m-labs.hk>
 # Copyright (c) 2021 David Sawatzke <d-git@sawatzke.dev>
 # Copyright (c) 2017-2018 whitequark <whitequark@whitequark.org>
+# Copyright (c) 2023 LumiGuide Fietsdetectie B.V. <goemansrowan@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from liteeth.common import *
 from liteeth.mac import gap, preamble, crc, padding, last_be
 from liteeth.phy.model import LiteEthPHYModel
 
 from migen.genlib.cdc import PulseSynchronizer
 
 from litex.soc.interconnect.stream import BufferizeEndpoints, DIR_SOURCE, DIR_SINK
 
 # MAC Core -----------------------------------------------------------------------------------------
 
 class LiteEthMACCore(Module, AutoCSR):
     def __init__(self, phy, dw,
-                 with_sys_datapath = False,
-                 with_preamble_crc = True,
-                 with_padding      = True):
+        with_sys_datapath = False,
+        with_preamble_crc = True,
+        with_padding      = True,
+        tx_cdc_depth      = 32,
+        tx_cdc_buffered   = False,
+        rx_cdc_depth      = 32,
+        rx_cdc_buffered   = False,
+        ):
 
         # Endpoints.
         self.sink   = stream.Endpoint(eth_phy_description(dw))
         self.source = stream.Endpoint(eth_phy_description(dw))
 
         # Parameters.
         core_dw = dw
@@ -51,17 +57,19 @@
         # ------------------------------------------------------------------------------------------
         class TXDatapath(Module, AutoCSR):
             def __init__(self):
                 self.pipeline = []
 
             def add_cdc(self):
                 tx_cdc = stream.ClockDomainCrossing(eth_phy_description(core_dw),
-                    cd_from = "sys",
-                    cd_to   = "eth_tx",
-                    depth   = 32)
+                    cd_from  = "sys",
+                    cd_to    = "eth_tx",
+                    depth    = tx_cdc_depth,
+                    buffered = tx_cdc_buffered,
+                )
                 self.submodules += tx_cdc
                 self.pipeline.append(tx_cdc)
 
             def add_converter(self):
                 tx_converter = stream.StrideConverter(
                     description_from = eth_phy_description(core_dw),
                     description_to   = eth_phy_description(phy_dw))
@@ -120,15 +128,15 @@
         if with_sys_datapath:
             # CHECKME: Verify converter/cdc order for the different cases.
             tx_datapath.add_cdc()
             if core_dw != phy_dw:
                 tx_datapath.add_converter()
             if core_dw != 8:
                 tx_datapath.add_last_be()
-        # Gap insertion has to occurr in phy tx domain to ensure gap is correctly maintained
+        # Gap insertion has to occurr in phy tx domain to ensure gap is correctly maintained.
         if not getattr(phy, "integrated_ifg_inserter", False):
             tx_datapath.add_gap()
         tx_datapath.pipeline.append(phy)
         self.submodules.tx_datapath = tx_datapath
 
         # RX Data-Path (PHY --> Core).
         # ------------------------------------------------------------------------------------------
@@ -180,17 +188,19 @@
                     description_to   = eth_phy_description(core_dw))
                 rx_converter = ClockDomainsRenamer("eth_rx")(rx_converter)
                 self.submodules += rx_converter
                 self.pipeline.append(rx_converter)
 
             def add_cdc(self):
                 rx_cdc = stream.ClockDomainCrossing(eth_phy_description(core_dw),
-                    cd_from = "eth_rx",
-                    cd_to   = "sys",
-                    depth   = 32)
+                    cd_from  = "eth_rx",
+                    cd_to    = "sys",
+                    depth    = rx_cdc_depth,
+                    buffered = rx_cdc_buffered,
+                )
                 self.submodules += rx_cdc
                 self.pipeline.append(rx_cdc)
 
             def do_finalize(self):
                 self.submodules += stream.Pipeline(*self.pipeline)
 
         rx_datapath = RXDatapath()
```

### Comparing `liteeth-2023.4/liteeth/mac/crc.py` & `liteeth-2023.8/liteeth/mac/crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from functools import reduce
 from operator import xor
 from collections import OrderedDict
 from math import ceil
 
 from liteeth.common import *
 
-from migen.genlib.misc import chooser, WaitTimer
+from litex.gen.genlib.misc import chooser, WaitTimer
 
 # MAC CRC Engine -----------------------------------------------------------------------------------
 
 class LiteEthMACCRCEngine(Module):
     """Cyclic Redundancy Check Engine
 
     Compute next CRC value from last CRC value and data input using
```

### Comparing `liteeth-2023.4/liteeth/mac/gap.py` & `liteeth-2023.8/liteeth/mac/gap.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/mac/last_be.py` & `liteeth-2023.8/liteeth/mac/last_be.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/mac/padding.py` & `liteeth-2023.8/liteeth/mac/padding.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/mac/preamble.py` & `liteeth-2023.8/liteeth/mac/preamble.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright (c) 2021 David Sawatzke <d-git@sawatzke.dev>
 # Copyright (c) 2015-2017 Sebastien Bourdeauducq <sb@m-labs.hk>
 # Copyright (c) 2017-2018 whitequark <whitequark@whitequark.org>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from liteeth.common import *
 
-from migen.genlib.misc import chooser
+from litex.gen.genlib.misc import chooser
 
 # MAC Preamble Inserter ----------------------------------------------------------------------------
 
 class LiteEthMACPreambleInserter(Module):
     """Preamble inserter
 
     Inserts preamble at the beginning of each packet.
```

### Comparing `liteeth-2023.4/liteeth/mac/sram.py` & `liteeth-2023.8/liteeth/mac/sram.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/mac/wishbone.py` & `liteeth-2023.8/liteeth/mac/wishbone.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from liteeth.mac import sram
 
 from litex.soc.interconnect import wishbone
 
 # MAC Wishbone Interface ---------------------------------------------------------------------------
 
 class LiteEthMACWishboneInterface(Module, AutoCSR):
-    def __init__(self, dw, nrxslots=2, ntxslots=2, endianness="big", timestamp=None):
+    def __init__(self, dw, nrxslots=2, ntxslots=2, endianness="big", timestamp=None,
+        rxslots_read_only  = True,
+        txslots_write_only = False,
+    ):
         self.sink   = stream.Endpoint(eth_phy_description(dw))
         self.source = stream.Endpoint(eth_phy_description(dw))
         self.bus    = wishbone.Interface(data_width=dw)
 
         # # #
 
         # Storage in SRAM.
@@ -30,24 +33,24 @@
         self.comb += self.sram.source.connect(self.source)
 
         # Wishbone SRAM interfaces for the writer SRAM (i.e. Ethernet RX).
         wb_rx_sram_ifs = []
         for n in range(nrxslots):
             wb_rx_sram_ifs.append(wishbone.SRAM(
                 mem_or_size = self.sram.writer.mems[n],
-                read_only   = True,
+                read_only   = rxslots_read_only,
                 bus         = wishbone.Interface(data_width = dw)
             ))
 
         # Wishbone SRAM interfaces for the reader SRAM (i.e. Ethernet TX).
         wb_tx_sram_ifs = []
         for n in range(ntxslots):
             wb_tx_sram_ifs.append(wishbone.SRAM(
                 mem_or_size = self.sram.reader.mems[n],
-                read_only   = False,
+                write_only  = txslots_write_only,
                 bus         = wishbone.Interface(data_width = dw)
             ))
 
         # Expose Wishbone SRAMs on a single Wishbone bus.
         # CHECKME: Check Decoder width for 64-bit.
         wb_slaves      = []
         decoderoffset  = log2_int(sram_depth, need_pow2=False)
```

### Comparing `liteeth-2023.4/liteeth/packet.py` & `liteeth-2023.8/liteeth/packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 # Copyright (c) 2019 Vamsi K Vytla <vkvytla@lbl.gov>
 # Copyright (c) 2021 Leon Schuermann <leon@is.currently.online>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import log2
 
 from migen import *
+
 from litex.gen import *
 
 from litex.soc.interconnect.packet import Header, HeaderField
 from litex.soc.interconnect import stream
+
 # Packetizer ---------------------------------------------------------------------------------------
 
-class Packetizer(Module):
+class Packetizer(LiteXModule):
     def __init__(self, sink_description, source_description, header):
         self.sink   = sink   = stream.Endpoint(sink_description)
         self.source = source = stream.Endpoint(source_description)
         self.header = Signal(header.length*8)
 
         # # #
 
@@ -44,15 +46,15 @@
             self.sync += If(sr_shift, sr.eq(sr[data_width:]))
 
         source_last_a = Signal()
         source_last_b = Signal()
         source_last_s = Signal()
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm_from_idle = Signal()
         fsm.act("IDLE",
             sink.ready.eq(1),
             NextValue(count, 1),
             If(sink.valid,
                 sink.ready.eq(0),
                 source.valid.eq(1),
@@ -144,15 +146,15 @@
 
             # Conditionally delay the calculated last_be for one clock cycle, if
             # it now applies to the next bus word OR if the source is not ready.
             delayed_last_be = Signal.like(sink_last_be)
 
             # FSM used to conveniently assign combinational and synchronous
             # signals in the same context.
-            self.submodules.last_be_fsm = last_be_fsm = FSM(reset_state="DEFAULT")
+            self.last_be_fsm = last_be_fsm = FSM(reset_state="DEFAULT")
 
             # Whether the main FSM is in one of the DATA-COPY states. This is
             # important as we overwrite sink.ready below and need to have
             # different behavior depending on the Packetizer's state
             in_data_copy = Signal()
             self.comb += [
                 in_data_copy.eq(self.fsm.ongoing("ALIGNED-DATA-COPY") | self.fsm.ongoing("UNALIGNED-DATA-COPY"))
@@ -207,15 +209,15 @@
 
         # Error.
         if hasattr(sink, "error") and hasattr(source, "error"):
             self.comb += source.error.eq(sink.error)
 
 # Depacketizer -------------------------------------------------------------------------------------
 
-class Depacketizer(Module):
+class Depacketizer(LiteXModule):
     def __init__(self, sink_description, source_description, header):
         self.sink   = sink   = stream.Endpoint(sink_description)
         self.source = source = stream.Endpoint(source_description)
         self.header = Signal(header.length*8)
 
         # # #
 
@@ -245,15 +247,15 @@
         self.comb += header.decode(self.header, source)
 
         source_last_a = Signal()
         source_last_b = Signal()
         source_last_s = Signal()
 
         # FSM.
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm_from_idle = Signal()
         fsm.act("IDLE",
             sink.ready.eq(1),
             NextValue(count, 1),
             If(sink.valid,
                 sr_shift.eq(1),
                 NextValue(fsm_from_idle, 1),
@@ -342,15 +344,15 @@
 
             # Conditionally delay the calculated last_be for one clock cycle, if
             # it now applies to the next bus word.
             delayed_last_be = Signal.like(sink_last_be)
 
             # FSM used to conveniently assign combinational and synchronous
             # signals in the same context.
-            self.submodules.last_be_fsm = last_be_fsm = FSM(reset_state="DEFAULT")
+            self.last_be_fsm = last_be_fsm = FSM(reset_state="DEFAULT")
 
             # Whether the main FSM is / was in one of the DATA-COPY states. This
             # is important as we must handle a special case when last is
             # asserted while the Depacketizer has just transitioned out of
             # writing the header, which we can then detect by checking
             # (~was_in_copy & is_in_copy).
             is_in_copy = Signal()
```

### Comparing `liteeth-2023.4/liteeth/phy/__init__.py` & `liteeth-2023.8/liteeth/phy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,21 +18,23 @@
     elif len(pads.tx_data) == 4:
         # This is a MII PHY
         from liteeth.phy.mii import LiteEthPHYMII
         return LiteEthPHYMII(clock_pads, pads, **kwargs)
     else:
         raise ValueError("Unable to autodetect PHY from platform file, use direct instantiation")
 
-from liteeth.phy.mii  import LiteEthPHYMII
-from liteeth.phy.rmii import LiteEthPHYRMII
-from liteeth.phy.gmii import LiteEthPHYGMII
+from liteeth.phy.mii      import LiteEthPHYMII
+from liteeth.phy.rmii     import LiteEthPHYRMII
+from liteeth.phy.gmii     import LiteEthPHYGMII
 from liteeth.phy.gmii_mii import LiteEthPHYGMIIMII
-from liteeth.phy.xgmii import LiteEthPHYXGMII
+from liteeth.phy.xgmii    import LiteEthPHYXGMII
 
-from liteeth.phy.s6rgmii import LiteEthPHYRGMII as LiteEthS6PHYRGMII
+from liteeth.phy.s6rgmii   import LiteEthPHYRGMII as LiteEthS6PHYRGMII
 from liteeth.phy.s7rgmii   import LiteEthPHYRGMII as LiteEthS7PHYRGMII
 from liteeth.phy.usrgmii   import LiteEthPHYRGMII as LiteEthUSPHYRGMII
 from liteeth.phy.ecp5rgmii import LiteEthPHYRGMII as LiteEthECP5PHYRGMII
 
-from liteeth.phy.a7_1000basex import A7_1000BASEX
-from liteeth.phy.k7_1000basex import K7_1000BASEX
-from liteeth.phy.ku_1000basex import KU_1000BASEX
+from liteeth.phy.a7_1000basex      import A7_1000BASEX
+from liteeth.phy.k7_1000basex      import K7_1000BASEX
+from liteeth.phy.ku_1000basex      import KU_1000BASEX
+from liteeth.phy.usp_gth_1000basex import USP_GTH_1000BASEX
+from liteeth.phy.usp_gty_1000basex import USP_GTY_1000BASEX
```

### Comparing `liteeth-2023.4/liteeth/phy/a7_1000basex.py` & `liteeth-2023.8/liteeth/phy/a7_2500basex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,66 @@
 #
 # This file is part of MiSoC and has been adapted/modified for LiteEth.
 #
 # Copyright (c) 2018 Sebastien Bourdeauducq <sb@m-labs.hk>
 # Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2023 Sergey Razumov <cyntem@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+
+from litex.soc.cores.clock import S7MMCM
+
 from liteeth.common import *
 from liteeth.phy.a7_gtp import *
 from liteeth.phy.pcs_1000basex import *
 
+# A7_2500BASEX PHY ---------------------------------------------------------------------------------
 
-class Open(Signal):
-    pass
-
-
-class Gearbox(Module):
-    def __init__(self):
-        self.tx_data      = Signal(10)
-        self.tx_data_half = Signal(20)
-        self.rx_data_half = Signal(20)
-        self.rx_data      = Signal(10)
-
-        # TX
-        buf = Signal(20)
-        self.sync.eth_tx += buf.eq(Cat(buf[10:], self.tx_data))
-        self.sync.eth_tx_half += self.tx_data_half.eq(buf)
-
-        # RX
-        phase_half = Signal()
-        phase_half_rereg = Signal()
-        self.sync.eth_rx_half += phase_half_rereg.eq(phase_half)
-        self.sync.eth_rx += [
-            If(phase_half == phase_half_rereg,
-                self.rx_data.eq(self.rx_data_half[10:])
-            ).Else(
-                self.rx_data.eq(self.rx_data_half[:10])
-            ),
-            phase_half.eq(~phase_half),
-        ]
-
-
-class A7_1000BASEX(Module, AutoCSR):
+class A7_2500BASEX(LiteXModule):
     dw          = 8
-    tx_clk_freq = 125e6
-    rx_clk_freq = 125e6
-    def __init__(self, qpll_channel, data_pads, sys_clk_freq, rx_polarity=0, tx_polarity=0):
+    tx_clk_freq = 312.5e6
+    rx_clk_freq = 312.5e6
+    def __init__(self, qpll_channel, data_pads, sys_clk_freq, with_csr=True, rx_polarity=0, tx_polarity=0):
         pcs = PCS(lsb_first=True)
         self.submodules += pcs
 
         self.sink    = pcs.sink
         self.source  = pcs.source
         self.link_up = pcs.link_up
 
-        self.clock_domains.cd_eth_tx      = ClockDomain()
-        self.clock_domains.cd_eth_rx      = ClockDomain()
-        self.clock_domains.cd_eth_tx_half = ClockDomain(reset_less=True)
-        self.clock_domains.cd_eth_rx_half = ClockDomain(reset_less=True)
+        self.cd_eth_tx      = ClockDomain()
+        self.cd_eth_rx      = ClockDomain()
+        self.cd_eth_tx_half = ClockDomain(reset_less=True)
+        self.cd_eth_rx_half = ClockDomain(reset_less=True)
 
         # for specifying clock constraints. 62.5MHz clocks.
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
-        self.crg_reset = CSRStorage()
+        self.reset = Signal()
+        if with_csr:
+            self.add_csr()
 
         # # #
 
         # GTP transceiver
         tx_reset       = Signal()
         tx_mmcm_locked = Signal()
+        tx_mmcm_reset  = Signal(reset=1)
         tx_data        = Signal(20)
         tx_reset_done  = Signal()
 
         rx_reset          = Signal()
         rx_mmcm_locked    = Signal()
+        rx_mmcm_reset     = Signal(reset=1)
         rx_data           = Signal(20)
         rx_reset_done     = Signal()
         rx_pma_reset_done = Signal()
 
         drpaddr = Signal(9)
         drpen   = Signal()
         drpdi   = Signal(16)
@@ -94,596 +74,596 @@
             # Simulation-Only Attributes
             p_SIM_RECEIVER_DETECT_PASS   = "TRUE",
             p_SIM_TX_EIDLE_DRIVE_LEVEL   = "X",
             p_SIM_RESET_SPEEDUP          = "FALSE",
             p_SIM_VERSION                = "2.0",
 
             # RX Byte and Word Alignment Attributes
-            p_ALIGN_COMMA_DOUBLE                     = "FALSE",
-            p_ALIGN_COMMA_ENABLE                     = 0b1111111111,
-            p_ALIGN_COMMA_WORD                       = 1,
-            p_ALIGN_MCOMMA_DET                       = "TRUE",
-            p_ALIGN_MCOMMA_VALUE                     = 0b1010000011,
-            p_ALIGN_PCOMMA_DET                       = "TRUE",
-            p_ALIGN_PCOMMA_VALUE                     = 0b0101111100,
-            p_SHOW_REALIGN_COMMA                     = "TRUE",
-            p_RXSLIDE_AUTO_WAIT                      = 7,
-            p_RXSLIDE_MODE                           = "OFF",
-            p_RX_SIG_VALID_DLY                       = 10,
+            p_ALIGN_COMMA_DOUBLE         = "FALSE",
+            p_ALIGN_COMMA_ENABLE         = 0b1111111111,
+            p_ALIGN_COMMA_WORD           = 1,
+            p_ALIGN_MCOMMA_DET           = "TRUE",
+            p_ALIGN_MCOMMA_VALUE         = 0b1010000011,
+            p_ALIGN_PCOMMA_DET           = "TRUE",
+            p_ALIGN_PCOMMA_VALUE         = 0b0101111100,
+            p_SHOW_REALIGN_COMMA         = "TRUE",
+            p_RXSLIDE_AUTO_WAIT          = 7,
+            p_RXSLIDE_MODE               = "OFF",
+            p_RX_SIG_VALID_DLY           = 10,
 
             # RX 8B/10B Decoder Attributes
-            p_RX_DISPERR_SEQ_MATCH                   = "FALSE",
-            p_DEC_MCOMMA_DETECT                      = "FALSE",
-            p_DEC_PCOMMA_DETECT                      = "FALSE",
-            p_DEC_VALID_COMMA_ONLY                   = "FALSE",
+            p_RX_DISPERR_SEQ_MATCH       = "FALSE",
+            p_DEC_MCOMMA_DETECT          = "FALSE",
+            p_DEC_PCOMMA_DETECT          = "FALSE",
+            p_DEC_VALID_COMMA_ONLY       = "FALSE",
 
             # RX Clock Correction Attributes
-            p_CBCC_DATA_SOURCE_SEL                   = "ENCODED",
-            p_CLK_COR_SEQ_2_USE                      = "FALSE",
-            p_CLK_COR_KEEP_IDLE                      = "FALSE",
-            p_CLK_COR_MAX_LAT                        = 9,
-            p_CLK_COR_MIN_LAT                        = 7,
-            p_CLK_COR_PRECEDENCE                     = "TRUE",
-            p_CLK_COR_REPEAT_WAIT                    = 0,
-            p_CLK_COR_SEQ_LEN                        = 1,
-            p_CLK_COR_SEQ_1_ENABLE                   = 0b1111,
-            p_CLK_COR_SEQ_1_1                        = 0b0100000000,
-            p_CLK_COR_SEQ_1_2                        = 0b0000000000,
-            p_CLK_COR_SEQ_1_3                        = 0b0000000000,
-            p_CLK_COR_SEQ_1_4                        = 0b0000000000,
-            p_CLK_CORRECT_USE                        = "FALSE",
-            p_CLK_COR_SEQ_2_ENABLE                   = 0b1111,
-            p_CLK_COR_SEQ_2_1                        = 0b0100000000,
-            p_CLK_COR_SEQ_2_2                        = 0b0000000000,
-            p_CLK_COR_SEQ_2_3                        = 0b0000000000,
-            p_CLK_COR_SEQ_2_4                        = 0b0000000000,
+            p_CBCC_DATA_SOURCE_SEL       = "ENCODED",
+            p_CLK_COR_SEQ_2_USE          = "FALSE",
+            p_CLK_COR_KEEP_IDLE          = "FALSE",
+            p_CLK_COR_MAX_LAT            = 9,
+            p_CLK_COR_MIN_LAT            = 7,
+            p_CLK_COR_PRECEDENCE         = "TRUE",
+            p_CLK_COR_REPEAT_WAIT        = 0,
+            p_CLK_COR_SEQ_LEN            = 1,
+            p_CLK_COR_SEQ_1_ENABLE       = 0b1111,
+            p_CLK_COR_SEQ_1_1            = 0b0100000000,
+            p_CLK_COR_SEQ_1_2            = 0b0000000000,
+            p_CLK_COR_SEQ_1_3            = 0b0000000000,
+            p_CLK_COR_SEQ_1_4            = 0b0000000000,
+            p_CLK_CORRECT_USE            = "FALSE",
+            p_CLK_COR_SEQ_2_ENABLE       = 0b1111,
+            p_CLK_COR_SEQ_2_1            = 0b0100000000,
+            p_CLK_COR_SEQ_2_2            = 0b0000000000,
+            p_CLK_COR_SEQ_2_3            = 0b0000000000,
+            p_CLK_COR_SEQ_2_4            = 0b0000000000,
 
             # RX Channel Bonding Attributes
-            p_CHAN_BOND_KEEP_ALIGN                   = "FALSE",
-            p_CHAN_BOND_MAX_SKEW                     = 1,
-            p_CHAN_BOND_SEQ_LEN                      = 1,
-            p_CHAN_BOND_SEQ_1_1                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_2                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_3                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_4                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_ENABLE                 = 0b1111,
-            p_CHAN_BOND_SEQ_2_1                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_2                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_3                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_4                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_ENABLE                 = 0b1111,
-            p_CHAN_BOND_SEQ_2_USE                    = "FALSE",
-            p_FTS_DESKEW_SEQ_ENABLE                  = 0b1111,
-            p_FTS_LANE_DESKEW_CFG                    = 0b1111,
-            p_FTS_LANE_DESKEW_EN                     = "FALSE",
+            p_CHAN_BOND_KEEP_ALIGN       = "FALSE",
+            p_CHAN_BOND_MAX_SKEW         = 1,
+            p_CHAN_BOND_SEQ_LEN          = 1,
+            p_CHAN_BOND_SEQ_1_1          = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_2          = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_3          = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_4          = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_ENABLE     = 0b1111,
+            p_CHAN_BOND_SEQ_2_1          = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_2          = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_3          = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_4          = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_ENABLE     = 0b1111,
+            p_CHAN_BOND_SEQ_2_USE        = "FALSE",
+            p_FTS_DESKEW_SEQ_ENABLE      = 0b1111,
+            p_FTS_LANE_DESKEW_CFG        = 0b1111,
+            p_FTS_LANE_DESKEW_EN         = "FALSE",
 
             # RX Margin Analysis Attributes
-            p_ES_CONTROL                             = 0b000000,
-            p_ES_ERRDET_EN                           = "FALSE",
-            p_ES_EYE_SCAN_EN                         = "FALSE",
-            p_ES_HORZ_OFFSET                         = 0x010,
-            p_ES_PMA_CFG                             = 0b0000000000,
-            p_ES_PRESCALE                            = 0b00000,
-            p_ES_QUALIFIER                           = 0x00000000000000000000,
-            p_ES_QUAL_MASK                           = 0x00000000000000000000,
-            p_ES_SDATA_MASK                          = 0x00000000000000000000,
-            p_ES_VERT_OFFSET                         = 0b000000000,
+            p_ES_CONTROL                 = 0b000000,
+            p_ES_ERRDET_EN               = "FALSE",
+            p_ES_EYE_SCAN_EN             = "FALSE",
+            p_ES_HORZ_OFFSET             = 0x010,
+            p_ES_PMA_CFG                 = 0b0000000000,
+            p_ES_PRESCALE                = 0b00000,
+            p_ES_QUALIFIER               = 0x00000000000000000000,
+            p_ES_QUAL_MASK               = 0x00000000000000000000,
+            p_ES_SDATA_MASK              = 0x00000000000000000000,
+            p_ES_VERT_OFFSET             = 0b000000000,
 
             # FPGA RX Interface Attributes
-            p_RX_DATA_WIDTH                          = 20,
+            p_RX_DATA_WIDTH              = 20,
 
             # PMA Attributes
-            p_OUTREFCLK_SEL_INV                      = 0b11,
-            p_PMA_RSV                                = 0x00000333,
-            p_PMA_RSV2                               = 0x00002040,
-            p_PMA_RSV3                               = 0b00,
-            p_PMA_RSV4                               = 0b0000,
-            p_RX_BIAS_CFG                            = 0b0000111100110011,
-            p_DMONITOR_CFG                           = 0x000A00,
-            p_RX_CM_SEL                              = 0b01,
-            p_RX_CM_TRIM                             = 0b0000,
-            p_RX_DEBUG_CFG                           = 0b00000000000000,
-            p_RX_OS_CFG                              = 0b0000010000000,
-            p_TERM_RCAL_CFG                          = 0b100001000010000,
-            p_TERM_RCAL_OVRD                         = 0b000,
-            p_TST_RSV                                = 0x00000000,
-            p_RX_CLK25_DIV                           = 5,
-            p_TX_CLK25_DIV                           = 5,
-            p_UCODEER_CLR                            = 0b0,
+            p_OUTREFCLK_SEL_INV          = 0b11,
+            p_PMA_RSV                    = 0x00000333,
+            p_PMA_RSV2                   = 0x00002040,
+            p_PMA_RSV3                   = 0b00,
+            p_PMA_RSV4                   = 0b0000,
+            p_RX_BIAS_CFG                = 0b0000111100110011,
+            p_DMONITOR_CFG               = 0x000A00,
+            p_RX_CM_SEL                  = 0b01,
+            p_RX_CM_TRIM                 = 0b0000,
+            p_RX_DEBUG_CFG               = 0b00000000000000,
+            p_RX_OS_CFG                  = 0b0000010000000,
+            p_TERM_RCAL_CFG              = 0b100001000010000,
+            p_TERM_RCAL_OVRD             = 0b000,
+            p_TST_RSV                    = 0x00000000,
+            p_RX_CLK25_DIV               = 5,
+            p_TX_CLK25_DIV               = 5,
+            p_UCODEER_CLR                = 0b0,
 
             # PCI Express Attributes
-            p_PCS_PCIE_EN                            = "FALSE",
+            p_PCS_PCIE_EN                = "FALSE",
 
             # PCS Attributes
-            p_PCS_RSVD_ATTR                          = 0x000000000000,
+            p_PCS_RSVD_ATTR              = 0x000000000000,
 
             # RX Buffer Attributes
-            p_RXBUF_ADDR_MODE                        = "FAST",
-            p_RXBUF_EIDLE_HI_CNT                     = 0b1000,
-            p_RXBUF_EIDLE_LO_CNT                     = 0b0000,
-            p_RXBUF_EN                               = "TRUE",
-            p_RX_BUFFER_CFG                          = 0b000000,
-            p_RXBUF_RESET_ON_CB_CHANGE               = "TRUE",
-            p_RXBUF_RESET_ON_COMMAALIGN              = "FALSE",
-            p_RXBUF_RESET_ON_EIDLE                   = "FALSE",
-            p_RXBUF_RESET_ON_RATE_CHANGE             = "TRUE",
-            p_RXBUFRESET_TIME                        = 0b00001,
-            p_RXBUF_THRESH_OVFLW                     = 61,
-            p_RXBUF_THRESH_OVRD                      = "FALSE",
-            p_RXBUF_THRESH_UNDFLW                    = 4,
-            p_RXDLY_CFG                              = 0x001F,
-            p_RXDLY_LCFG                             = 0x030,
-            p_RXDLY_TAP_CFG                          = 0x0000,
-            p_RXPH_CFG                               = 0xC00002,
-            p_RXPHDLY_CFG                            = 0x084020,
-            p_RXPH_MONITOR_SEL                       = 0b00000,
-            p_RX_XCLK_SEL                            = "RXREC",
-            p_RX_DDI_SEL                             = 0b000000,
-            p_RX_DEFER_RESET_BUF_EN                  = "TRUE",
+            p_RXBUF_ADDR_MODE            = "FAST",
+            p_RXBUF_EIDLE_HI_CNT         = 0b1000,
+            p_RXBUF_EIDLE_LO_CNT         = 0b0000,
+            p_RXBUF_EN                   = "TRUE",
+            p_RX_BUFFER_CFG              = 0b000000,
+            p_RXBUF_RESET_ON_CB_CHANGE   = "TRUE",
+            p_RXBUF_RESET_ON_COMMAALIGN  = "FALSE",
+            p_RXBUF_RESET_ON_EIDLE       = "FALSE",
+            p_RXBUF_RESET_ON_RATE_CHANGE = "TRUE",
+            p_RXBUFRESET_TIME            = 0b00001,
+            p_RXBUF_THRESH_OVFLW         = 61,
+            p_RXBUF_THRESH_OVRD          = "FALSE",
+            p_RXBUF_THRESH_UNDFLW        = 4,
+            p_RXDLY_CFG                  = 0x001F,
+            p_RXDLY_LCFG                 = 0x030,
+            p_RXDLY_TAP_CFG              = 0x0000,
+            p_RXPH_CFG                   = 0xC00002,
+            p_RXPHDLY_CFG                = 0x084020,
+            p_RXPH_MONITOR_SEL           = 0b00000,
+            p_RX_XCLK_SEL                = "RXREC",
+            p_RX_DDI_SEL                 = 0b000000,
+            p_RX_DEFER_RESET_BUF_EN      = "TRUE",
 
             # CDR Attributes
-            p_RXCDR_CFG                              = 0x0001107FE086021101010,
-            p_RXCDR_FR_RESET_ON_EIDLE                = 0b0,
-            p_RXCDR_HOLD_DURING_EIDLE                = 0b0,
-            p_RXCDR_PH_RESET_ON_EIDLE                = 0b0,
-            p_RXCDR_LOCK_CFG                         = 0b001001,
+            p_RXCDR_CFG                  = 0x0000107FE206001041010,
+            p_RXCDR_FR_RESET_ON_EIDLE    = 0b0,
+            p_RXCDR_HOLD_DURING_EIDLE    = 0b0,
+            p_RXCDR_PH_RESET_ON_EIDLE    = 0b0,
+            p_RXCDR_LOCK_CFG             = 0b001001,
 
             # RX Initialization and Reset Attributes
-            p_RXCDRFREQRESET_TIME                    = 0b00001,
-            p_RXCDRPHRESET_TIME                      = 0b00001,
-            p_RXISCANRESET_TIME                      = 0b00001,
-            p_RXPCSRESET_TIME                        = 0b00001,
-            p_RXPMARESET_TIME                        = 0b00011,
+            p_RXCDRFREQRESET_TIME        = 0b00001,
+            p_RXCDRPHRESET_TIME          = 0b00001,
+            p_RXISCANRESET_TIME          = 0b00001,
+            p_RXPCSRESET_TIME            = 0b00001,
+            p_RXPMARESET_TIME            = 0b00011,
 
             # RX OOB Signaling Attributes
-            p_RXOOB_CFG                              = 0b0000110,
+            p_RXOOB_CFG                  = 0b0000110,
 
             # RX Gearbox Attributes
-            p_RXGEARBOX_EN                           = "FALSE",
-            p_GEARBOX_MODE                           = 0b000,
+            p_RXGEARBOX_EN               = "FALSE",
+            p_GEARBOX_MODE               = 0b000,
 
             # PRBS Detection Attribute
-            p_RXPRBS_ERR_LOOPBACK                    = 0b0,
+            p_RXPRBS_ERR_LOOPBACK        = 0b0,
 
             # Power-Down Attributes
-            p_PD_TRANS_TIME_FROM_P2                  = 0x03c,
-            p_PD_TRANS_TIME_NONE_P2                  = 0x3c,
-            p_PD_TRANS_TIME_TO_P2                    = 0x64,
+            p_PD_TRANS_TIME_FROM_P2      = 0x03c,
+            p_PD_TRANS_TIME_NONE_P2      = 0x3c,
+            p_PD_TRANS_TIME_TO_P2        = 0x64,
 
             # RX OOB Signaling Attributes
-            p_SAS_MAX_COM                            = 64,
-            p_SAS_MIN_COM                            = 36,
-            p_SATA_BURST_SEQ_LEN                     = 0b0101,
-            p_SATA_BURST_VAL                         = 0b100,
-            p_SATA_EIDLE_VAL                         = 0b100,
-            p_SATA_MAX_BURST                         = 8,
-            p_SATA_MAX_INIT                          = 21,
-            p_SATA_MAX_WAKE                          = 7,
-            p_SATA_MIN_BURST                         = 4,
-            p_SATA_MIN_INIT                          = 12,
-            p_SATA_MIN_WAKE                          = 4,
+            p_SAS_MAX_COM                = 64,
+            p_SAS_MIN_COM                = 36,
+            p_SATA_BURST_SEQ_LEN         = 0b0101,
+            p_SATA_BURST_VAL             = 0b100,
+            p_SATA_EIDLE_VAL             = 0b100,
+            p_SATA_MAX_BURST             = 8,
+            p_SATA_MAX_INIT              = 21,
+            p_SATA_MAX_WAKE              = 7,
+            p_SATA_MIN_BURST             = 4,
+            p_SATA_MIN_INIT              = 12,
+            p_SATA_MIN_WAKE              = 4,
 
             # RX Fabric Clock Output Control Attributes
-            p_TRANS_TIME_RATE                        = 0x0E,
+            p_TRANS_TIME_RATE            = 0x0E,
 
             # TX Buffer Attributes
-            p_TXBUF_EN                               = "TRUE",
-            p_TXBUF_RESET_ON_RATE_CHANGE             = "TRUE",
-            p_TXDLY_CFG                              = 0x001F,
-            p_TXDLY_LCFG                             = 0x030,
-            p_TXDLY_TAP_CFG                          = 0x0000,
-            p_TXPH_CFG                               = 0x0780,
-            p_TXPHDLY_CFG                            = 0x084020,
-            p_TXPH_MONITOR_SEL                       = 0b00000,
-            p_TX_XCLK_SEL                            = "TXOUT",
+            p_TXBUF_EN                   = "TRUE",
+            p_TXBUF_RESET_ON_RATE_CHANGE = "TRUE",
+            p_TXDLY_CFG                  = 0x001F,
+            p_TXDLY_LCFG                 = 0x030,
+            p_TXDLY_TAP_CFG              = 0x0000,
+            p_TXPH_CFG                   = 0x0780,
+            p_TXPHDLY_CFG                = 0x084020,
+            p_TXPH_MONITOR_SEL           = 0b00000,
+            p_TX_XCLK_SEL                = "TXOUT",
 
             # FPGA TX Interface Attributes
-            p_TX_DATA_WIDTH                          = 20,
+            p_TX_DATA_WIDTH              = 20,
 
             # TX Configurable Driver Attributes
-            p_TX_DEEMPH0                             = 0b000000,
-            p_TX_DEEMPH1                             = 0b000000,
-            p_TX_EIDLE_ASSERT_DELAY                  = 0b110,
-            p_TX_EIDLE_DEASSERT_DELAY                = 0b100,
-            p_TX_LOOPBACK_DRIVE_HIZ                  = "FALSE",
-            p_TX_MAINCURSOR_SEL                      = 0b0,
-            p_TX_DRIVE_MODE                          = "DIRECT",
-            p_TX_MARGIN_FULL_0                       = 0b1001110,
-            p_TX_MARGIN_FULL_1                       = 0b1001001,
-            p_TX_MARGIN_FULL_2                       = 0b1000101,
-            p_TX_MARGIN_FULL_3                       = 0b1000010,
-            p_TX_MARGIN_FULL_4                       = 0b1000000,
-            p_TX_MARGIN_LOW_0                        = 0b1000110,
-            p_TX_MARGIN_LOW_1                        = 0b1000100,
-            p_TX_MARGIN_LOW_2                        = 0b1000010,
-            p_TX_MARGIN_LOW_3                        = 0b1000000,
-            p_TX_MARGIN_LOW_4                        = 0b1000000,
+            p_TX_DEEMPH0                 = 0b000000,
+            p_TX_DEEMPH1                 = 0b000000,
+            p_TX_EIDLE_ASSERT_DELAY      = 0b110,
+            p_TX_EIDLE_DEASSERT_DELAY    = 0b100,
+            p_TX_LOOPBACK_DRIVE_HIZ      = "FALSE",
+            p_TX_MAINCURSOR_SEL          = 0b0,
+            p_TX_DRIVE_MODE              = "DIRECT",
+            p_TX_MARGIN_FULL_0           = 0b1001110,
+            p_TX_MARGIN_FULL_1           = 0b1001001,
+            p_TX_MARGIN_FULL_2           = 0b1000101,
+            p_TX_MARGIN_FULL_3           = 0b1000010,
+            p_TX_MARGIN_FULL_4           = 0b1000000,
+            p_TX_MARGIN_LOW_0            = 0b1000110,
+            p_TX_MARGIN_LOW_1            = 0b1000100,
+            p_TX_MARGIN_LOW_2            = 0b1000010,
+            p_TX_MARGIN_LOW_3            = 0b1000000,
+            p_TX_MARGIN_LOW_4            = 0b1000000,
 
             # TX Gearbox Attributes
-            p_TXGEARBOX_EN                           = "FALSE",
+            p_TXGEARBOX_EN               = "FALSE",
 
             # TX Initialization and Reset Attributes
-            p_TXPCSRESET_TIME                        = 0b00001,
-            p_TXPMARESET_TIME                        = 0b00001,
+            p_TXPCSRESET_TIME            = 0b00001,
+            p_TXPMARESET_TIME            = 0b00001,
 
             # TX Receiver Detection Attributes
-            p_TX_RXDETECT_CFG                        = 0x1832,
-            p_TX_RXDETECT_REF                        = 0b100,
+            p_TX_RXDETECT_CFG            = 0x1832,
+            p_TX_RXDETECT_REF            = 0b100,
 
             # JTAG Attributes
-            p_ACJTAG_DEBUG_MODE                      = 0b0,
-            p_ACJTAG_MODE                            = 0b0,
-            p_ACJTAG_RESET                           = 0b0,
+            p_ACJTAG_DEBUG_MODE          = 0b0,
+            p_ACJTAG_MODE                = 0b0,
+            p_ACJTAG_RESET               = 0b0,
 
             # CDR Attributes
-            p_CFOK_CFG                               = 0x49000040E80,
-            p_CFOK_CFG2                              = 0b0100000,
-            p_CFOK_CFG3                              = 0b0100000,
-            p_CFOK_CFG4                              = 0b0,
-            p_CFOK_CFG5                              = 0x0,
-            p_CFOK_CFG6                              = 0b0000,
-            p_RXOSCALRESET_TIME                      = 0b00011,
-            p_RXOSCALRESET_TIMEOUT                   = 0b00000,
+            p_CFOK_CFG                   = 0x49000040E80,
+            p_CFOK_CFG2                  = 0b0100000,
+            p_CFOK_CFG3                  = 0b0100000,
+            p_CFOK_CFG4                  = 0b0,
+            p_CFOK_CFG5                  = 0x0,
+            p_CFOK_CFG6                  = 0b0000,
+            p_RXOSCALRESET_TIME          = 0b00011,
+            p_RXOSCALRESET_TIMEOUT       = 0b00000,
 
             # PMA Attributes
-            p_CLK_COMMON_SWING                       = 0b0,
-            p_RX_CLKMUX_EN                           = 0b1,
-            p_TX_CLKMUX_EN                           = 0b1,
-            p_ES_CLK_PHASE_SEL                       = 0b0,
-            p_USE_PCS_CLK_PHASE_SEL                  = 0b0,
-            p_PMA_RSV6                               = 0b0,
-            p_PMA_RSV7                               = 0b0,
+            p_CLK_COMMON_SWING           = 0b0,
+            p_RX_CLKMUX_EN               = 0b1,
+            p_TX_CLKMUX_EN               = 0b1,
+            p_ES_CLK_PHASE_SEL           = 0b0,
+            p_USE_PCS_CLK_PHASE_SEL      = 0b0,
+            p_PMA_RSV6                   = 0b0,
+            p_PMA_RSV7                   = 0b0,
 
             # TX Configuration Driver Attributes
-            p_TX_PREDRIVER_MODE                      = 0b0,
-            p_PMA_RSV5                               = 0b0,
-            p_SATA_PLL_CFG                           = "VCO_3000MHZ",
+            p_TX_PREDRIVER_MODE          = 0b0,
+            p_PMA_RSV5                   = 0b0,
+            p_SATA_PLL_CFG               = "VCO_3000MHZ",
 
             # RX Fabric Clock Output Control Attributes
-            p_RXOUT_DIV                              = 4,
+            p_RXOUT_DIV                  = 2,
 
             # TX Fabric Clock Output Control Attributes
-            p_TXOUT_DIV                              = 4,
+            p_TXOUT_DIV                  = 2,
 
             # RX Phase Interpolator Attributes
-            p_RXPI_CFG0                              = 0b000,
-            p_RXPI_CFG1                              = 0b1,
-            p_RXPI_CFG2                              = 0b1,
+            p_RXPI_CFG0                  = 0b000,
+            p_RXPI_CFG1                  = 0b1,
+            p_RXPI_CFG2                  = 0b1,
 
             # RX Equalizer Attributes
-            p_ADAPT_CFG0                             = 0x00000,
-            p_RXLPMRESET_TIME                        = 0b0001111,
-            p_RXLPM_BIAS_STARTUP_DISABLE             = 0b0,
-            p_RXLPM_CFG                              = 0b0110,
-            p_RXLPM_CFG1                             = 0b0,
-            p_RXLPM_CM_CFG                           = 0b0,
-            p_RXLPM_GC_CFG                           = 0b111100010,
-            p_RXLPM_GC_CFG2                          = 0b001,
-            p_RXLPM_HF_CFG                           = 0b00001111110000,
-            p_RXLPM_HF_CFG2                          = 0b01010,
-            p_RXLPM_HF_CFG3                          = 0b0000,
-            p_RXLPM_HOLD_DURING_EIDLE                = 0b0,
-            p_RXLPM_INCM_CFG                         = 0b0,
-            p_RXLPM_IPCM_CFG                         = 0b1,
-            p_RXLPM_LF_CFG                           = 0b000000001111110000,
-            p_RXLPM_LF_CFG2                          = 0b01010,
-            p_RXLPM_OSINT_CFG                        = 0b100,
+            p_ADAPT_CFG0                 = 0x00000,
+            p_RXLPMRESET_TIME            = 0b0001111,
+            p_RXLPM_BIAS_STARTUP_DISABLE = 0b0,
+            p_RXLPM_CFG                  = 0b0110,
+            p_RXLPM_CFG1                 = 0b0,
+            p_RXLPM_CM_CFG               = 0b0,
+            p_RXLPM_GC_CFG               = 0b111100010,
+            p_RXLPM_GC_CFG2              = 0b001,
+            p_RXLPM_HF_CFG               = 0b00001111110000,
+            p_RXLPM_HF_CFG2              = 0b01010,
+            p_RXLPM_HF_CFG3              = 0b0000,
+            p_RXLPM_HOLD_DURING_EIDLE    = 0b0,
+            p_RXLPM_INCM_CFG             = 0b0,
+            p_RXLPM_IPCM_CFG             = 0b1,
+            p_RXLPM_LF_CFG               = 0b000000001111110000,
+            p_RXLPM_LF_CFG2              = 0b01010,
+            p_RXLPM_OSINT_CFG            = 0b100,
 
             # TX Phase Interpolator PPM Controller Attributes
-            p_TXPI_CFG0                              = 0b00,
-            p_TXPI_CFG1                              = 0b00,
-            p_TXPI_CFG2                              = 0b00,
-            p_TXPI_CFG3                              = 0b0,
-            p_TXPI_CFG4                              = 0b0,
-            p_TXPI_CFG5                              = 0b000,
-            p_TXPI_GREY_SEL                          = 0b0,
-            p_TXPI_INVSTROBE_SEL                     = 0b0,
-            p_TXPI_PPMCLK_SEL                        = "TXUSRCLK2",
-            p_TXPI_PPM_CFG                           = 0x00,
-            p_TXPI_SYNFREQ_PPM                       = 0b001,
+            p_TXPI_CFG0                  = 0b00,
+            p_TXPI_CFG1                  = 0b00,
+            p_TXPI_CFG2                  = 0b00,
+            p_TXPI_CFG3                  = 0b0,
+            p_TXPI_CFG4                  = 0b0,
+            p_TXPI_CFG5                  = 0b000,
+            p_TXPI_GREY_SEL              = 0b0,
+            p_TXPI_INVSTROBE_SEL         = 0b0,
+            p_TXPI_PPMCLK_SEL            = "TXUSRCLK2",
+            p_TXPI_PPM_CFG               = 0x00,
+            p_TXPI_SYNFREQ_PPM           = 0b001,
 
             # LOOPBACK Attributes
-            p_LOOPBACK_CFG                           = 0b0,
-            p_PMA_LOOPBACK_CFG                       = 0b0,
+            p_LOOPBACK_CFG               = 0b0,
+            p_PMA_LOOPBACK_CFG           = 0b0,
 
             # RX OOB Signalling Attributes
-            p_RXOOB_CLK_CFG                          = "PMA",
+            p_RXOOB_CLK_CFG              = "PMA",
 
             # TX OOB Signalling Attributes
-            p_TXOOB_CFG                              = 0b0,
+            p_TXOOB_CFG                  = 0b0,
 
             # RX Buffer Attributes
-            p_RXSYNC_MULTILANE                       = 0b0,
-            p_RXSYNC_OVRD                            = 0b0,
-            p_RXSYNC_SKIP_DA                         = 0b0,
+            p_RXSYNC_MULTILANE           = 0b0,
+            p_RXSYNC_OVRD                = 0b0,
+            p_RXSYNC_SKIP_DA             = 0b0,
 
             # TX Buffer Attributes
-            p_TXSYNC_MULTILANE                       = 0b0,
-            p_TXSYNC_OVRD                            = 0b0,
-            p_TXSYNC_SKIP_DA                         = 0b0
+            p_TXSYNC_MULTILANE           = 0b0,
+            p_TXSYNC_OVRD                = 0b0,
+            p_TXSYNC_SKIP_DA             = 0b0
         )
         gtp_params.update(
             # CPLL Ports
-            i_GTRSVD                         = 0b0000000000000000,
-            i_PCSRSVDIN                      = 0b0000000000000000,
-            i_TSTIN                          = 0b11111111111111111111,
+            i_GTRSVD               = 0b0000000000000000,
+            i_PCSRSVDIN            = 0b0000000000000000,
+            i_TSTIN                = 0b11111111111111111111,
             # Channel - DRP Ports
-            i_DRPADDR                        = drpaddr,
-            i_DRPCLK                         = ClockSignal(),
-            i_DRPDI                          = drpdi,
-            o_DRPDO                          = drpdo,
-            i_DRPEN                          = drpen,
-            o_DRPRDY                         = drprdy,
-            i_DRPWE                          = drpwe,
+            i_DRPADDR              = drpaddr,
+            i_DRPCLK               = ClockSignal(),
+            i_DRPDI                = drpdi,
+            o_DRPDO                = drpdo,
+            i_DRPEN                = drpen,
+            o_DRPRDY               = drprdy,
+            i_DRPWE                = drpwe,
             # FPGA TX Interface Datapath Configuration
-            i_TX8B10BEN                      = 0,
+            i_TX8B10BEN            = 0,
             # Loopback Ports
-            i_LOOPBACK                       = 0,
+            i_LOOPBACK             = 0,
             # PCI Express Ports
-            o_PHYSTATUS                      = Open(),
-            i_RXRATE                         = 0,
-            o_RXVALID                        = Open(),
+            o_PHYSTATUS            = Open(),
+            i_RXRATE               = 0,
+            o_RXVALID              = Open(),
             # PMA Reserved Ports
-            i_PMARSVDIN3                     = 0b0,
-            i_PMARSVDIN4                     = 0b0,
+            i_PMARSVDIN3           = 0b0,
+            i_PMARSVDIN4           = 0b0,
             # Power-Down Ports
-            i_RXPD                           = 0b00,
-            i_TXPD                           = 0b00,
+            i_RXPD                 = 0b00,
+            i_TXPD                 = 0b00,
             # RX 8B/10B Decoder Ports
-            i_SETERRSTATUS                   = 0,
+            i_SETERRSTATUS         = 0,
             # RX Initialization and Reset Ports
-            i_EYESCANRESET                   = 0,
-            i_RXUSERRDY                      = rx_mmcm_locked,
+            i_EYESCANRESET         = 0,
+            i_RXUSERRDY            = rx_mmcm_locked,
             # RX Margin Analysis Ports
-            o_EYESCANDATAERROR               = Open(),
-            i_EYESCANMODE                    = 0,
-            i_EYESCANTRIGGER                 = 0,
+            o_EYESCANDATAERROR     = Open(),
+            i_EYESCANMODE          = 0,
+            i_EYESCANTRIGGER       = 0,
             # Receive Ports
-            i_CLKRSVD0                       = 0,
-            i_CLKRSVD1                       = 0,
-            i_DMONFIFORESET                  = 0,
-            i_DMONITORCLK                    = 0,
-            o_RXPMARESETDONE                 = rx_pma_reset_done,
-            i_SIGVALIDCLK                    = 0,
+            i_CLKRSVD0             = 0,
+            i_CLKRSVD1             = 0,
+            i_DMONFIFORESET        = 0,
+            i_DMONITORCLK          = 0,
+            o_RXPMARESETDONE       = rx_pma_reset_done,
+            i_SIGVALIDCLK          = 0,
             # Receive Ports - CDR Ports
-            i_RXCDRFREQRESET                 = 0,
-            i_RXCDRHOLD                      = 0,
-            o_RXCDRLOCK                      = Open(),
-            i_RXCDROVRDEN                    = 0,
-            i_RXCDRRESET                     = 0,
-            i_RXCDRRESETRSV                  = 0,
-            i_RXOSCALRESET                   = 0,
-            i_RXOSINTCFG                     = 0b0010,
-            o_RXOSINTDONE                    = Open(),
-            i_RXOSINTHOLD                    = 0,
-            i_RXOSINTOVRDEN                  = 0,
-            i_RXOSINTPD                      = 0,
-            o_RXOSINTSTARTED                 = Open(),
-            i_RXOSINTSTROBE                  = 0,
-            o_RXOSINTSTROBESTARTED           = Open(),
-            i_RXOSINTTESTOVRDEN              = 0,
+            i_RXCDRFREQRESET       = 0,
+            i_RXCDRHOLD            = 0,
+            o_RXCDRLOCK            = Open(),
+            i_RXCDROVRDEN          = 0,
+            i_RXCDRRESET           = 0,
+            i_RXCDRRESETRSV        = 0,
+            i_RXOSCALRESET         = 0,
+            i_RXOSINTCFG           = 0b0010,
+            o_RXOSINTDONE          = Open(),
+            i_RXOSINTHOLD          = 0,
+            i_RXOSINTOVRDEN        = 0,
+            i_RXOSINTPD            = 0,
+            o_RXOSINTSTARTED       = Open(),
+            i_RXOSINTSTROBE        = 0,
+            o_RXOSINTSTROBESTARTED = Open(),
+            i_RXOSINTTESTOVRDEN    = 0,
             # Receive Ports - Clock Correction Ports
-            o_RXCLKCORCNT                    = Open(),
+            o_RXCLKCORCNT          = Open(),
             # Receive Ports - FPGA RX Interface Datapath Configuration
-            i_RX8B10BEN                      = 0,
+            i_RX8B10BEN            = 0,
             # Receive Ports - FPGA RX Interface Ports
-            o_RXDATA                         = Cat(rx_data[:8], rx_data[10:18]),
-            i_RXUSRCLK                       = ClockSignal("eth_rx_half"),
-            i_RXUSRCLK2                      = ClockSignal("eth_rx_half"),
+            o_RXDATA               = Cat(rx_data[:8], rx_data[10:18]),
+            i_RXUSRCLK             = ClockSignal("eth_rx_half"),
+            i_RXUSRCLK2            = ClockSignal("eth_rx_half"),
             # Receive Ports - Pattern Checker Ports
-            o_RXPRBSERR                      = Open(),
-            i_RXPRBSSEL                      = 0,
+            o_RXPRBSERR            = Open(),
+            i_RXPRBSSEL            = 0,
             # Receive Ports - Pattern Checker ports
-            i_RXPRBSCNTRESET                 = 0,
+            i_RXPRBSCNTRESET       = 0,
             # Receive Ports - RX 8B/10B Decoder Ports
-            o_RXCHARISCOMMA                  = Open(),
-            o_RXCHARISK                      = Cat(rx_data[8], rx_data[18]),
-            o_RXDISPERR                      = Cat(rx_data[9], rx_data[19]),
-            o_RXNOTINTABLE                   = Open(),
+            o_RXCHARISCOMMA        = Open(),
+            o_RXCHARISK            = Cat(rx_data[8], rx_data[18]),
+            o_RXDISPERR            = Cat(rx_data[9], rx_data[19]),
+            o_RXNOTINTABLE         = Open(),
             # Receive Ports - RX AFE Ports
-            i_GTPRXN                         = data_pads.rxn,
-            i_GTPRXP                         = data_pads.rxp,
-            i_PMARSVDIN2                     = 0b0,
-            o_PMARSVDOUT0                    = Open(),
-            o_PMARSVDOUT1                    = Open(),
+            i_GTPRXN               = data_pads.rxn,
+            i_GTPRXP               = data_pads.rxp,
+            i_PMARSVDIN2           = 0b0,
+            o_PMARSVDOUT0          = Open(),
+            o_PMARSVDOUT1          = Open(),
             # Receive Ports - RX Buffer Bypass Ports
-            i_RXBUFRESET                     = 0,
-            o_RXBUFSTATUS                    = Open(),
-            i_RXDDIEN                        = 0,
-            i_RXDLYBYPASS                    = 1,
-            i_RXDLYEN                        = 0,
-            i_RXDLYOVRDEN                    = 0,
-            i_RXDLYSRESET                    = 0,
-            o_RXDLYSRESETDONE                = Open(),
-            i_RXPHALIGN                      = 0,
-            o_RXPHALIGNDONE                  = Open(),
-            i_RXPHALIGNEN                    = 0,
-            i_RXPHDLYPD                      = 0,
-            i_RXPHDLYRESET                   = 0,
-            o_RXPHMONITOR                    = Open(),
-            i_RXPHOVRDEN                     = 0,
-            o_RXPHSLIPMONITOR                = Open(),
-            o_RXSTATUS                       = Open(),
-            i_RXSYNCALLIN                    = 0,
-            o_RXSYNCDONE                     = Open(),
-            i_RXSYNCIN                       = 0,
-            i_RXSYNCMODE                     = 0,
-            o_RXSYNCOUT                      = Open(),
+            i_RXBUFRESET           = 0,
+            o_RXBUFSTATUS          = Open(),
+            i_RXDDIEN              = 0,
+            i_RXDLYBYPASS          = 1,
+            i_RXDLYEN              = 0,
+            i_RXDLYOVRDEN          = 0,
+            i_RXDLYSRESET          = 0,
+            o_RXDLYSRESETDONE      = Open(),
+            i_RXPHALIGN            = 0,
+            o_RXPHALIGNDONE        = Open(),
+            i_RXPHALIGNEN          = 0,
+            i_RXPHDLYPD            = 0,
+            i_RXPHDLYRESET         = 0,
+            o_RXPHMONITOR          = Open(),
+            i_RXPHOVRDEN           = 0,
+            o_RXPHSLIPMONITOR      = Open(),
+            o_RXSTATUS             = Open(),
+            i_RXSYNCALLIN          = 0,
+            o_RXSYNCDONE           = Open(),
+            i_RXSYNCIN             = 0,
+            i_RXSYNCMODE           = 0,
+            o_RXSYNCOUT            = Open(),
             # Receive Ports - RX Byte and Word Alignment Ports
-            o_RXBYTEISALIGNED                = Open(),
-            o_RXBYTEREALIGN                  = Open(),
-            o_RXCOMMADET                     = Open(),
-            i_RXCOMMADETEN                   = 0,
-            i_RXMCOMMAALIGNEN                = 0,
-            i_RXPCOMMAALIGNEN                = 0,
-            i_RXSLIDE                        = 0,
+            o_RXBYTEISALIGNED      = Open(),
+            o_RXBYTEREALIGN        = Open(),
+            o_RXCOMMADET           = Open(),
+            i_RXCOMMADETEN         = 0,
+            i_RXMCOMMAALIGNEN      = 0,
+            i_RXPCOMMAALIGNEN      = 0,
+            i_RXSLIDE              = 0,
             # Receive Ports - RX Channel Bonding Ports
-            o_RXCHANBONDSEQ                  = Open(),
-            i_RXCHBONDEN                     = 0,
-            i_RXCHBONDI                      = 0b0000,
-            i_RXCHBONDLEVEL                  = 0,
-            i_RXCHBONDMASTER                 = 0,
-            o_RXCHBONDO                      = Open(),
-            i_RXCHBONDSLAVE                  = 0,
+            o_RXCHANBONDSEQ        = Open(),
+            i_RXCHBONDEN           = 0,
+            i_RXCHBONDI            = 0b0000,
+            i_RXCHBONDLEVEL        = 0,
+            i_RXCHBONDMASTER       = 0,
+            o_RXCHBONDO            = Open(),
+            i_RXCHBONDSLAVE        = 0,
             # Receive Ports - RX Channel Bonding Ports
-            o_RXCHANISALIGNED                = Open(),
-            o_RXCHANREALIGN                  = Open(),
+            o_RXCHANISALIGNED      = Open(),
+            o_RXCHANREALIGN        = Open(),
             # Receive Ports - RX Decision Feedback Equalizer
-            o_DMONITOROUT                    = Open(),
-            i_RXADAPTSELTEST                 = 0,
-            i_RXDFEXYDEN                     = 0,
-            i_RXOSINTEN                      = 0b1,
-            i_RXOSINTID0                     = 0,
-            i_RXOSINTNTRLEN                  = 0,
-            o_RXOSINTSTROBEDONE              = Open(),
+            o_DMONITOROUT          = Open(),
+            i_RXADAPTSELTEST       = 0,
+            i_RXDFEXYDEN           = 0,
+            i_RXOSINTEN            = 0b1,
+            i_RXOSINTID0           = 0,
+            i_RXOSINTNTRLEN        = 0,
+            o_RXOSINTSTROBEDONE    = Open(),
             # Receive Ports - RX Driver,OOB signalling,Coupling and Eq.,CDR
-            i_RXLPMLFOVRDEN                  = 0,
-            i_RXLPMOSINTNTRLEN               = 0,
+            i_RXLPMLFOVRDEN        = 0,
+            i_RXLPMOSINTNTRLEN     = 0,
             # Receive Ports - RX Equalizer Ports
-            i_RXLPMHFHOLD                    = 0,
-            i_RXLPMHFOVRDEN                  = 0,
-            i_RXLPMLFHOLD                    = 0,
-            i_RXOSHOLD                       = 0,
-            i_RXOSOVRDEN                     = 0,
+            i_RXLPMHFHOLD          = 0,
+            i_RXLPMHFOVRDEN        = 0,
+            i_RXLPMLFHOLD          = 0,
+            i_RXOSHOLD             = 0,
+            i_RXOSOVRDEN           = 0,
             # Receive Ports - RX Fabric ClocK Output Control Ports
-            o_RXRATEDONE                     = Open(),
+            o_RXRATEDONE           = Open(),
             # Receive Ports - RX Fabric Clock Output Control Ports
-            i_RXRATEMODE                     = 0b0,
+            i_RXRATEMODE           = 0b0,
             # Receive Ports - RX Fabric Output Control Ports
-            o_RXOUTCLK                       = self.rxoutclk,
-            o_RXOUTCLKFABRIC                 = Open(),
-            o_RXOUTCLKPCS                    = Open(),
-            i_RXOUTCLKSEL                    = 0b010,
+            o_RXOUTCLK             = self.rxoutclk,
+            o_RXOUTCLKFABRIC       = Open(),
+            o_RXOUTCLKPCS          = Open(),
+            i_RXOUTCLKSEL          = 0b010,
             # Receive Ports - RX Gearbox Ports
-            o_RXDATAVALID                    = Open(),
-            o_RXHEADER                       = Open(),
-            o_RXHEADERVALID                  = Open(),
-            o_RXSTARTOFSEQ                   = Open(),
-            i_RXGEARBOXSLIP                  = 0,
+            o_RXDATAVALID          = Open(),
+            o_RXHEADER             = Open(),
+            o_RXHEADERVALID        = Open(),
+            o_RXSTARTOFSEQ         = Open(),
+            i_RXGEARBOXSLIP        = 0,
             # Receive Ports - RX Initialization and Reset Ports
-            i_GTRXRESET                      = rx_reset,
-            i_RXLPMRESET                     = 0,
-            i_RXOOBRESET                     = 0,
-            i_RXPCSRESET                     = 0,
-            i_RXPMARESET                     = 0,
+            i_GTRXRESET            = rx_reset,
+            i_RXLPMRESET           = 0,
+            i_RXOOBRESET           = 0,
+            i_RXPCSRESET           = 0,
+            i_RXPMARESET           = 0,
             # Receive Ports - RX OOB Signaling ports
-            o_RXCOMSASDET                    = Open(),
-            o_RXCOMWAKEDET                   = Open(),
-            o_RXCOMINITDET                   = Open(),
-            o_RXELECIDLE                     = Open(),
-            i_RXELECIDLEMODE                 = 0b11,
+            o_RXCOMSASDET          = Open(),
+            o_RXCOMWAKEDET         = Open(),
+            o_RXCOMINITDET         = Open(),
+            o_RXELECIDLE           = Open(),
+            i_RXELECIDLEMODE       = 0b11,
             # Receive Ports - RX Polarity Control Ports
-            i_RXPOLARITY                     = rx_polarity,
+            i_RXPOLARITY           = rx_polarity,
             # Receive Ports -RX Initialization and Reset Ports
-            o_RXRESETDONE                    = rx_reset_done,
+            o_RXRESETDONE          = rx_reset_done,
             # TX Buffer Bypass Ports
-            i_TXPHDLYTSTCLK                  = 0,
+            i_TXPHDLYTSTCLK        = 0,
             # TX Configurable Driver Ports
-            i_TXPOSTCURSOR                   = 0b00000,
-            i_TXPOSTCURSORINV                = 0,
-            i_TXPRECURSOR                    = 0,
-            i_TXPRECURSORINV                 = 0,
+            i_TXPOSTCURSOR         = 0b00000,
+            i_TXPOSTCURSORINV      = 0,
+            i_TXPRECURSOR          = 0,
+            i_TXPRECURSORINV       = 0,
             # TX Fabric Clock Output Control Ports
-            i_TXRATEMODE                     = 0,
+            i_TXRATEMODE           = 0,
             # TX Initialization and Reset Ports
-            i_CFGRESET                       = 0,
-            i_GTTXRESET                      = tx_reset,
-            o_PCSRSVDOUT                     = Open(),
-            i_TXUSERRDY                      = tx_mmcm_locked,
+            i_CFGRESET             = 0,
+            i_GTTXRESET            = tx_reset,
+            o_PCSRSVDOUT           = Open(),
+            i_TXUSERRDY            = tx_mmcm_locked,
             # TX Phase Interpolator PPM Controller Ports
-            i_TXPIPPMEN                      = 0,
-            i_TXPIPPMOVRDEN                  = 0,
-            i_TXPIPPMPD                      = 0,
-            i_TXPIPPMSEL                     = 1,
-            i_TXPIPPMSTEPSIZE                = 0,
+            i_TXPIPPMEN            = 0,
+            i_TXPIPPMOVRDEN        = 0,
+            i_TXPIPPMPD            = 0,
+            i_TXPIPPMSEL           = 1,
+            i_TXPIPPMSTEPSIZE      = 0,
             # Transceiver Reset Mode Operation
-            i_GTRESETSEL                     = 0,
-            i_RESETOVRD                      = 0,
+            i_GTRESETSEL           = 0,
+            i_RESETOVRD            = 0,
             # Transmit Ports
-            o_TXPMARESETDONE                 = Open(),
+            o_TXPMARESETDONE       = Open(),
             # Transmit Ports - Configurable Driver Ports
-            i_PMARSVDIN0                     = 0b0,
-            i_PMARSVDIN1                     = 0b0,
+            i_PMARSVDIN0           = 0b0,
+            i_PMARSVDIN1           = 0b0,
             # Transmit Ports - FPGA TX Interface Ports
-            i_TXDATA                         = Cat(tx_data[:8], tx_data[10:18]),
-            i_TXUSRCLK                       = ClockSignal("eth_tx_half"),
-            i_TXUSRCLK2                      = ClockSignal("eth_tx_half"),
+            i_TXDATA               = Cat(tx_data[:8], tx_data[10:18]),
+            i_TXUSRCLK             = ClockSignal("eth_tx_half"),
+            i_TXUSRCLK2            = ClockSignal("eth_tx_half"),
             # Transmit Ports - PCI Express Ports
-            i_TXELECIDLE                     = 0,
-            i_TXMARGIN                       = 0,
-            i_TXRATE                         = 0,
-            i_TXSWING                        = 0,
+            i_TXELECIDLE           = 0,
+            i_TXMARGIN             = 0,
+            i_TXRATE               = 0,
+            i_TXSWING              = 0,
             # Transmit Ports - Pattern Generator Ports
-            i_TXPRBSFORCEERR                 = 0,
+            i_TXPRBSFORCEERR       = 0,
             # Transmit Ports - TX 8B/10B Encoder Ports
-            i_TX8B10BBYPASS                  = 0,
-            i_TXCHARDISPMODE                 = Cat(tx_data[9], tx_data[19]),
-            i_TXCHARDISPVAL                  = Cat(tx_data[8], tx_data[18]),
-            i_TXCHARISK                      = 0,
+            i_TX8B10BBYPASS        = 0,
+            i_TXCHARDISPMODE       = Cat(tx_data[9], tx_data[19]),
+            i_TXCHARDISPVAL        = Cat(tx_data[8], tx_data[18]),
+            i_TXCHARISK            = 0,
             # Transmit Ports - TX Buffer Bypass Ports
-            i_TXDLYBYPASS                    = 1,
-            i_TXDLYEN                        = 0,
-            i_TXDLYHOLD                      = 0,
-            i_TXDLYOVRDEN                    = 0,
-            i_TXDLYSRESET                    = 0,
-            o_TXDLYSRESETDONE                = Open(),
-            i_TXDLYUPDOWN                    = 0,
-            i_TXPHALIGN                      = 0,
-            o_TXPHALIGNDONE                  = Open(),
-            i_TXPHALIGNEN                    = 0,
-            i_TXPHDLYPD                      = 0,
-            i_TXPHDLYRESET                   = 0,
-            i_TXPHINIT                       = 0,
-            o_TXPHINITDONE                   = Open(),
-            i_TXPHOVRDEN                     = 0,
+            i_TXDLYBYPASS          = 1,
+            i_TXDLYEN              = 0,
+            i_TXDLYHOLD            = 0,
+            i_TXDLYOVRDEN          = 0,
+            i_TXDLYSRESET          = 0,
+            o_TXDLYSRESETDONE      = Open(),
+            i_TXDLYUPDOWN          = 0,
+            i_TXPHALIGN            = 0,
+            o_TXPHALIGNDONE        = Open(),
+            i_TXPHALIGNEN          = 0,
+            i_TXPHDLYPD            = 0,
+            i_TXPHDLYRESET         = 0,
+            i_TXPHINIT             = 0,
+            o_TXPHINITDONE         = Open(),
+            i_TXPHOVRDEN           = 0,
             # Transmit Ports - TX Buffer Ports
-            o_TXBUFSTATUS                    = Open(),
+            o_TXBUFSTATUS          = Open(),
             # Transmit Ports - TX Buffer and Phase Alignment Ports
-            i_TXSYNCALLIN                    = 0,
-            o_TXSYNCDONE                     = Open(),
-            i_TXSYNCIN                       = 0,
-            i_TXSYNCMODE                     = 0,
-            o_TXSYNCOUT                      = Open(),
+            i_TXSYNCALLIN          = 0,
+            o_TXSYNCDONE           = Open(),
+            i_TXSYNCIN             = 0,
+            i_TXSYNCMODE           = 0,
+            o_TXSYNCOUT            = Open(),
             # Transmit Ports - TX Configurable Driver Ports
-            o_GTPTXN                         = data_pads.txn,
-            o_GTPTXP                         = data_pads.txp,
-            i_TXBUFDIFFCTRL                  = 0b100,
-            i_TXDEEMPH                       = 0,
-            i_TXDIFFCTRL                     = 0b1000,
-            i_TXDIFFPD                       = 0,
-            i_TXINHIBIT                      = 0,
-            i_TXMAINCURSOR                   = 0b0000000,
-            i_TXPISOPD                       = 0,
+            o_GTPTXN               = data_pads.txn,
+            o_GTPTXP               = data_pads.txp,
+            i_TXBUFDIFFCTRL        = 0b100,
+            i_TXDEEMPH             = 0,
+            i_TXDIFFCTRL           = 0b1000,
+            i_TXDIFFPD             = 0,
+            i_TXINHIBIT            = 0,
+            i_TXMAINCURSOR         = 0b0000000,
+            i_TXPISOPD             = 0,
             # Transmit Ports - TX Fabric Clock Output Control Ports
-            o_TXOUTCLK                       = self.txoutclk,
-            o_TXOUTCLKFABRIC                 = Open(),
-            o_TXOUTCLKPCS                    = Open(),
-            i_TXOUTCLKSEL                    = 0b010,
-            o_TXRATEDONE                     = Open(),
+            o_TXOUTCLK             = self.txoutclk,
+            o_TXOUTCLKFABRIC       = Open(),
+            o_TXOUTCLKPCS          = Open(),
+            i_TXOUTCLKSEL          = 0b010,
+            o_TXRATEDONE           = Open(),
             # Transmit Ports - TX Gearbox Ports
-            o_TXGEARBOXREADY                 = Open(),
-            i_TXHEADER                       = 0,
-            i_TXSEQUENCE                     = 0,
-            i_TXSTARTSEQ                     = 0,
+            o_TXGEARBOXREADY       = Open(),
+            i_TXHEADER             = 0,
+            i_TXSEQUENCE           = 0,
+            i_TXSTARTSEQ           = 0,
             # Transmit Ports - TX Initialization and Reset Ports
-            i_TXPCSRESET                     = 0,
-            i_TXPMARESET                     = 0,
-            o_TXRESETDONE                    = tx_reset_done,
+            i_TXPCSRESET           = 0,
+            i_TXPMARESET           = 0,
+            o_TXRESETDONE          = tx_reset_done,
             # Transmit Ports - TX OOB signalling Ports
-            o_TXCOMFINISH                    = Open(),
-            i_TXCOMINIT                      = 0,
-            i_TXCOMSAS                       = 0,
-            i_TXCOMWAKE                      = 0,
-            i_TXPDELECIDLEMODE               = 0,
+            o_TXCOMFINISH          = Open(),
+            i_TXCOMINIT            = 0,
+            i_TXCOMSAS             = 0,
+            i_TXCOMWAKE            = 0,
+            i_TXPDELECIDLEMODE     = 0,
             # Transmit Ports - TX Polarity Control Ports
-            i_TXPOLARITY                     = tx_polarity,
+            i_TXPOLARITY           = tx_polarity,
             # Transmit Ports - TX Receiver Detection Ports
-            i_TXDETECTRX                     = 0,
+            i_TXDETECTRX           = 0,
             # Transmit Ports - pattern Generator Ports
-            i_TXPRBSSEL                      = 0
+            i_TXPRBSSEL            = 0
         )
         if qpll_channel.index == 0:
             gtp_params.update(
                 # Clocking Ports
                 i_RXSYSCLKSEL = 0b00,
                 i_TXSYSCLKSEL = 0b00,
                 # GTPE2_CHANNEL Clocking Ports
@@ -703,102 +683,58 @@
                 i_PLL1CLK     = qpll_channel.clk,
                 i_PLL1REFCLK  = qpll_channel.refclk,
             )
         else:
             raise ValueError
         self.specials += Instance("GTPE2_CHANNEL", **gtp_params)
 
-        # Get 125MHz clocks back - the GTP junk insists on outputting 62.5MHz.
+        # Get 125MHz clocks back - the GTP is outputting 62.5MHz.
         txoutclk_rebuffer = Signal()
-        self.specials += Instance("BUFH", i_I=self.txoutclk, o_O=txoutclk_rebuffer)
+        self.specials += Instance("BUFH",
+            i_I = self.txoutclk,
+            o_O = txoutclk_rebuffer
+        )
         rxoutclk_rebuffer = Signal()
-        self.specials += Instance("BUFG", i_I=self.rxoutclk, o_O=rxoutclk_rebuffer)
-
-        tx_mmcm_fb        = Signal()
-        tx_mmcm_reset     = Signal(reset=1)
-        clk_tx_unbuf      = Signal()
-        clk_tx_half_unbuf = Signal()
-        self.specials += [
-            Instance("MMCME2_BASE",
-                p_CLKIN1_PERIOD    = 16.0,
-                i_CLKIN1           = txoutclk_rebuffer,
-                i_RST              = tx_mmcm_reset,
-
-                o_CLKFBOUT         = tx_mmcm_fb,
-                i_CLKFBIN          = tx_mmcm_fb,
-
-                p_CLKFBOUT_MULT_F  = 16,
-                o_LOCKED           = tx_mmcm_locked,
-                p_DIVCLK_DIVIDE    = 1,
-
-                p_CLKOUT0_DIVIDE_F = 16,
-                o_CLKOUT0          = clk_tx_half_unbuf,
-                p_CLKOUT1_DIVIDE   = 8,
-                o_CLKOUT1          = clk_tx_unbuf,
-            ),
-            Instance("BUFH",
-                i_I = clk_tx_half_unbuf,
-                o_O = self.cd_eth_tx_half.clk,
-            ),
-            Instance("BUFH",
-                i_I = clk_tx_unbuf,
-                o_O = self.cd_eth_tx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_eth_tx, ~tx_mmcm_locked)
-        ]
+        self.specials += Instance("BUFG",
+            i_I = self.rxoutclk,
+            o_O = rxoutclk_rebuffer
+        )
 
-        rx_mmcm_fb        = Signal()
-        rx_mmcm_reset     = Signal(reset=1)
-        clk_rx_unbuf      = Signal()
-        clk_rx_half_unbuf = Signal()
-        self.specials += [
-            Instance("MMCME2_BASE",
-                p_CLKIN1_PERIOD    = 16.0,
-                i_CLKIN1           = rxoutclk_rebuffer,
-                i_RST              = rx_mmcm_reset,
-
-                o_CLKFBOUT         = rx_mmcm_fb,
-                i_CLKFBIN          = rx_mmcm_fb,
-
-                p_CLKFBOUT_MULT_F  = 16,
-                o_LOCKED           = rx_mmcm_locked,
-                p_DIVCLK_DIVIDE    = 1,
-
-                p_CLKOUT0_DIVIDE_F = 16,
-                o_CLKOUT0          = clk_rx_half_unbuf,
-                p_CLKOUT1_DIVIDE   = 8,
-                o_CLKOUT1          = clk_rx_unbuf,
-            ),
-            Instance("BUFG",
-                i_I = clk_rx_half_unbuf,
-                o_O = self.cd_eth_rx_half.clk,
-            ),
-            Instance("BUFG",
-                i_I = clk_rx_unbuf,
-                o_O = self.cd_eth_rx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_eth_rx, ~rx_mmcm_locked)
-        ]
+        # TX MMCM.
+        self.tx_mmcm = tx_mmcm = S7MMCM()
+        tx_mmcm.register_clkin(txoutclk_rebuffer,   156.25e6)
+        tx_mmcm.create_clkout(self.cd_eth_tx_half,  156.25e6, buf="bufh", with_reset=False)
+        tx_mmcm.create_clkout(self.cd_eth_tx,      312.5e6, buf="bufh", with_reset=True)
+        self.comb += tx_mmcm.reset.eq(tx_mmcm_reset)
+        self.comb += tx_mmcm_locked.eq(tx_mmcm.locked)
+
+        # RX MMCM.
+        self.rx_mmcm = rx_mmcm = S7MMCM()
+        rx_mmcm.register_clkin(rxoutclk_rebuffer,   156.25e6)
+        rx_mmcm.create_clkout(self.cd_eth_rx_half,  156.25e6, buf="bufg", with_reset=False)
+        rx_mmcm.create_clkout(self.cd_eth_rx,      312.5e6, buf="bufg", with_reset=True)
+        self.comb += rx_mmcm.reset.eq(rx_mmcm_reset)
+        self.comb += rx_mmcm_locked.eq(rx_mmcm.locked)
 
         # Transceiver init
         tx_init = GTPTxInit(sys_clk_freq)
         self.submodules += tx_init
         self.comb += [
             qpll_channel.reset.eq(tx_init.qpll_reset),
             tx_init.qpll_lock.eq(qpll_channel.lock),
-            tx_reset.eq(tx_init.tx_reset | self.crg_reset.storage)
+            tx_reset.eq(tx_init.tx_reset | self.reset)
         ]
         self.sync += tx_mmcm_reset.eq(~qpll_channel.lock)
         tx_mmcm_reset.attr.add("no_retiming")
 
         rx_init = GTPRxInit(sys_clk_freq)
         self.submodules += rx_init
         self.comb += [
             rx_init.enable.eq(tx_init.done),
-            rx_reset.eq(rx_init.rx_reset | self.crg_reset.storage),
+            rx_reset.eq(rx_init.rx_reset | self.reset),
 
             rx_init.rx_pma_reset_done.eq(rx_pma_reset_done),
             drpaddr.eq(rx_init.drpaddr),
             drpen.eq(rx_init.drpen),
             drpdi.eq(rx_init.drpdi),
             rx_init.drprdy.eq(drprdy),
             rx_init.drpdo.eq(drpdo),
@@ -808,15 +744,15 @@
         self.submodules += ps_restart
         self.comb += [
             ps_restart.i.eq(pcs.restart),
             rx_init.restart.eq(ps_restart.o)
         ]
 
         # Assume CDR lock time is 50,000 UI as per DS183 and similar to what the Xilinx wizards does.
-        cdr_lock_time = round(sys_clk_freq*50e3/1.25e9)
+        cdr_lock_time = round(sys_clk_freq*50e3/(312.5e6))
         cdr_lock_counter = Signal(max=cdr_lock_time+1)
         cdr_locked = Signal()
         self.sync += [
             If(rx_reset,
                 cdr_locked.eq(0),
                 cdr_lock_counter.eq(0)
             ).Elif(cdr_lock_counter != cdr_lock_time,
@@ -825,17 +761,19 @@
                 cdr_locked.eq(1)
             ),
             rx_mmcm_reset.eq(~cdr_locked)
         ]
         rx_mmcm_reset.attr.add("no_retiming")
 
         # Gearbox and PCS connection
-        gearbox = Gearbox()
-        self.submodules += gearbox
-
+        self.gearbox = gearbox = PCSGearbox()
         self.comb += [
             tx_data.eq(gearbox.tx_data_half),
             gearbox.rx_data_half.eq(rx_data),
 
             gearbox.tx_data.eq(pcs.tbi_tx),
             pcs.tbi_rx.eq(gearbox.rx_data)
         ]
+
+    def add_csr(self):
+        self._reset = CSRStorage()
+        self.comb += self.reset.eq(self._reset.storage)
```

### Comparing `liteeth-2023.4/liteeth/phy/a7_gtp.py` & `liteeth-2023.8/liteeth/phy/a7_gtp.py`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth/phy/common.py` & `liteeth-2023.8/liteeth/phy/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
+from litex.gen import *
+
 from liteeth.common import *
 
 from migen.genlib.cdc import MultiReg
 from migen.fhdl.specials import Tristate
 
+# LiteEth PHY HWReset ------------------------------------------------------------------------------
 
 class LiteEthPHYHWReset(Module):
     def __init__(self, cycles=256):
         self.reset = Signal()
 
         # # #
 
@@ -22,34 +25,34 @@
         self.sync += If(counter_ce, counter.eq(counter + 1))
         self.comb += [
             counter_done.eq(counter == cycles),
             counter_ce.eq(~counter_done),
             self.reset.eq(~counter_done)
         ]
 
+# LiteEth PHY MDIO ---------------------------------------------------------------------------------
 
-class LiteEthPHYMDIO(Module, AutoCSR):
+class LiteEthPHYMDIO(LiteXModule):
     def __init__(self, pads):
         self._w = CSRStorage(fields=[
             CSRField("mdc", size=1),
             CSRField("oe",  size=1),
             CSRField("w",   size=1)],
-            name="w")
+            name="w"
+        )
         self._r = CSRStatus(fields=[
             CSRField("r", size=1)],
-            name="r")
-
+            name="r"
+        )
 
         # # #
 
         data_w  = Signal()
         data_oe = Signal()
         data_r  = Signal()
-        self.comb +=[
+        self.comb += [
             pads.mdc.eq(self._w.storage[0]),
-            data_oe.eq(self._w.storage[1]),
-            data_w.eq(self._w.storage[2])
-        ]
-        self.specials += [
-            MultiReg(data_r, self._r.status[0]),
-            Tristate(pads.mdio, data_w, data_oe, data_r)
+            data_oe.eq( self._w.storage[1]),
+            data_w.eq(  self._w.storage[2]),
         ]
+        self.specials += MultiReg(data_r, self._r.status[0])
+        self.specials += Tristate(pads.mdio, data_w, data_oe, data_r)
```

### Comparing `liteeth-2023.4/liteeth/phy/ecp5rgmii.py` & `liteeth-2023.8/liteeth/phy/ecp5rgmii.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2019-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2019-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2020 Shawn Hoffman <godisgovernment@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # RGMII PHY for ECP5 Lattice FPGA
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from litex.build.io import DDROutput, DDRInput
 
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY RGMII TX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIITX(Module):
+class LiteEthPHYRGMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         tx_ctl_oddrx1f  = Signal()
         tx_data_oddrx1f = Signal(4)
 
         self.specials += [
             DDROutput(
                 clk = ClockSignal("eth_tx"),
                 i1  = sink.valid,
                 i2  = sink.valid,
-                o   = tx_ctl_oddrx1f),
+                o   = tx_ctl_oddrx1f,
+            ),
             Instance("DELAYG",
                 p_DEL_MODE  = "SCLK_ALIGNED",
                 p_DEL_VALUE = 0,
                 i_A         = tx_ctl_oddrx1f,
-                o_Z         = pads.tx_ctl)
+                o_Z         = pads.tx_ctl,
+            )
         ]
         for i in range(4):
             self.specials += [
                 DDROutput(
                     clk = ClockSignal("eth_tx"),
                     i1  = sink.data[i],
                     i2  = sink.data[4+i],
-                    o   = tx_data_oddrx1f[i]),
+                    o   = tx_data_oddrx1f[i],
+                ),
                 Instance("DELAYG",
                     p_DEL_MODE  = "SCLK_ALIGNED",
                     p_DEL_VALUE = 0,
                     i_A         = tx_data_oddrx1f[i],
-                    o_Z         = pads.tx_data[i]
+                    o_Z         = pads.tx_data[i],
                 )
             ]
         self.comb += sink.ready.eq(1)
 
+# LiteEth PHY RGMII RX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIIRX(Module, AutoCSR):
+class LiteEthPHYRGMIIRX(LiteXModule):
     def __init__(self, pads, rx_delay=2e-9, with_inband_status=True):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         if with_inband_status:
             self.inband_status = CSRStatus(fields=[
                 CSRField("link_status", size=1, values=[
                     ("``0b0``", "Link down."),
@@ -88,35 +95,36 @@
         rx_data_reg    = Signal(8)
 
         self.specials += [
             Instance("DELAYG",
                 p_DEL_MODE  = "SCLK_ALIGNED",
                 p_DEL_VALUE = rx_delay_taps,
                 i_A         = pads.rx_ctl,
-                o_Z         = rx_ctl_delayf),
+                o_Z         = rx_ctl_delayf,
+            ),
             DDRInput(
                 clk = ClockSignal("eth_rx"),
                 i   = rx_ctl_delayf,
                 o1  = rx_ctl[0],
-                o2  = rx_ctl[1]
+                o2  = rx_ctl[1],
             )
         ]
         self.sync += rx_ctl_reg.eq(rx_ctl)
         for i in range(4):
             self.specials += [
                 Instance("DELAYG",
                     p_DEL_MODE  = "SCLK_ALIGNED",
                     p_DEL_VALUE = rx_delay_taps,
                     i_A         = pads.rx_data[i],
                     o_Z         = rx_data_delayf[i]),
                 DDRInput(
                     clk = ClockSignal("eth_rx"),
                     i   = rx_data_delayf[i],
                     o1  = rx_data[i],
-                    o2  = rx_data[i+4]
+                    o2  = rx_data[i+4],
                 )
             ]
         self.sync += rx_data_reg.eq(rx_data)
 
         rx_ctl_reg_d = Signal(2)
         self.sync += rx_ctl_reg_d.eq(rx_ctl_reg)
 
@@ -127,74 +135,83 @@
             source.data.eq(rx_data_reg)
         ]
         self.comb += source.last.eq(last)
 
         if with_inband_status:
             self.sync += [
                 If(rx_ctl == 0b00,
-                    self.inband_status.fields.link_status.eq(rx_data[0]),
-                    self.inband_status.fields.clock_speed.eq(rx_data[1:3]),
+                    self.inband_status.fields.link_status.eq(  rx_data[0]),
+                    self.inband_status.fields.clock_speed.eq(  rx_data[1:3]),
                     self.inband_status.fields.duplex_status.eq(rx_data[3]),
                 )
             ]
 
+# LiteEth PHY RGMII CRG ----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIICRG(Module, AutoCSR):
-    def __init__(self, clock_pads, pads, with_hw_init_reset, tx_delay=2e-9):
+class LiteEthPHYRGMIICRG(LiteXModule):
+    def __init__(self, clock_pads, pads, with_hw_init_reset, tx_delay=2e-9, tx_clk=None):
         self._reset = CSRStorage()
 
         # # #
 
         # RX Clock
-        self.clock_domains.cd_eth_rx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
         self.comb += self.cd_eth_rx.clk.eq(clock_pads.rx)
 
         # TX Clock
-        self.clock_domains.cd_eth_tx = ClockDomain()
-        self.comb += self.cd_eth_tx.clk.eq(self.cd_eth_rx.clk)
+        self.cd_eth_tx = ClockDomain()
+        if isinstance(tx_clk, Signal):
+            self.comb += self.cd_eth_tx.clk.eq(tx_clk)
+        else:
+            self.comb += self.cd_eth_tx.clk.eq(self.cd_eth_rx.clk)
+
         tx_delay_taps = int(tx_delay/25e-12) # 25ps per tap
         assert tx_delay_taps < 128
 
         eth_tx_clk_o = Signal()
         self.specials += [
             DDROutput(
                 clk = ClockSignal("eth_tx"),
                 i1  = 1,
                 i2  = 0,
-                o   = eth_tx_clk_o),
+                o   = eth_tx_clk_o,
+            ),
             Instance("DELAYG",
                 p_DEL_MODE  = "SCLK_ALIGNED",
                 p_DEL_VALUE = tx_delay_taps,
                 i_A         = eth_tx_clk_o,
-                o_Z         = clock_pads.tx)
+                o_Z         = clock_pads.tx,
+            )
         ]
 
         # Reset
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset()
+            self.hw_reset = LiteEthPHYHWReset()
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
 
-class LiteEthPHYRGMII(Module, AutoCSR):
+class LiteEthPHYRGMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
     def __init__(self, clock_pads, pads, with_hw_init_reset=True,
         tx_delay           = 2e-9,
         rx_delay           = 2e-9,
-        with_inband_status = True):
-        self.submodules.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay)
-        self.submodules.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
-        self.submodules.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay, with_inband_status))
+        with_inband_status = True,
+        tx_clk             = None,
+        ):
+        self.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay, tx_clk)
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay, with_inband_status))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/gmii.py` & `liteeth-2023.8/liteeth/phy/gmii.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from litex.build.io import DDROutput
 
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY GMII TX ------------------------------------------------------------------------------
 
-class LiteEthPHYGMIITX(Module):
+class LiteEthPHYGMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         if hasattr(pads, "tx_er"):
             pads.tx_er.reset_less = True
             self.sync += pads.tx_er.eq(0)
-        pads.tx_en.reset_less = True
+        pads.tx_en.reset_less   = True
         pads.tx_data.reset_less = True
         self.sync += [
             pads.tx_en.eq(sink.valid),
             pads.tx_data.eq(sink.data),
             sink.ready.eq(1)
         ]
 
+# LiteEth PHY GMII RX ------------------------------------------------------------------------------
 
-class LiteEthPHYGMIIRX(Module):
+class LiteEthPHYGMIIRX(LiteXModule):
     def __init__(self, pads):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         dv_d = Signal()
         self.sync += [
             dv_d.eq(pads.rx_dv),
             source.valid.eq(pads.rx_dv),
-            source.data.eq(pads.rx_data)
+            source.data.eq(pads.rx_data),
         ]
         self.comb += source.last.eq(~pads.rx_dv & dv_d)
 
+# LiteEth PHY GMII RX ------------------------------------------------------------------------------
 
-class LiteEthPHYGMIICRG(Module, AutoCSR):
+class LiteEthPHYGMIICRG(LiteXModule):
     def __init__(self, clock_pads, pads, with_hw_init_reset, mii_mode=0, model=False):
         self._reset = CSRStorage()
 
         # # #
 
-        self.clock_domains.cd_eth_rx = ClockDomain()
-        self.clock_domains.cd_eth_tx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
+        self.cd_eth_tx = ClockDomain()
 
         if not model:
             # RX clock: GMII, MII Use PHY clock_pads.rx as eth_rx_clk.
             self.specials += Instance("BUFG",
                 i_I = clock_pads.rx,
                 o_O = ClockSignal("eth_rx"),
             )
@@ -77,15 +82,15 @@
                 i_I = eth_tx_clk,
                 o_O = ClockSignal("eth_tx"),
             )
 
             # Reset
             self.reset = reset = Signal()
             if with_hw_init_reset:
-                self.submodules.hw_reset = LiteEthPHYHWReset()
+                self.hw_reset = LiteEthPHYHWReset()
                 self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
             else:
                 self.comb += reset.eq(self._reset.storage)
             if hasattr(pads, "rst_n"):
                 self.comb += pads.rst_n.eq(~reset)
             self.specials += [
                 AsyncResetSynchronizer(self.cd_eth_tx, reset),
@@ -93,21 +98,22 @@
             ]
         else:
             self.comb += [
                 self.cd_eth_rx.clk.eq(ClockSignal()),
                 self.cd_eth_tx.clk.eq(ClockSignal()),
             ]
 
+# LiteEth PHY GMII ---------------------------------------------------------------------------------
 
-class LiteEthPHYGMII(Module, AutoCSR):
+class LiteEthPHYGMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
     def __init__(self, clock_pads, pads, with_hw_init_reset=True, model=False):
         self.model = model
-        self.submodules.crg = LiteEthPHYGMIICRG(clock_pads, pads, with_hw_init_reset, model=model)
-        self.submodules.tx = ClockDomainsRenamer("eth_tx")(LiteEthPHYGMIITX(pads))
-        self.submodules.rx = ClockDomainsRenamer("eth_rx")(LiteEthPHYGMIIRX(pads))
+        self.crg   = LiteEthPHYGMIICRG(clock_pads, pads, with_hw_init_reset, model=model)
+        self.tx    = ClockDomainsRenamer("eth_tx")(LiteEthPHYGMIITX(pads))
+        self.rx    = ClockDomainsRenamer("eth_rx")(LiteEthPHYGMIIRX(pads))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/gmii_mii.py` & `liteeth-2023.8/liteeth/phy/gmii_mii.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+
 from litex.build.io import DDROutput
 
 from litex.soc.interconnect.stream import Multiplexer, Demultiplexer
 
 from liteeth.common import *
 from liteeth.phy.gmii import LiteEthPHYGMIICRG
 from liteeth.phy.mii import LiteEthPHYMIITX, LiteEthPHYMIIRX
 from liteeth.phy.gmii import LiteEthPHYGMIITX, LiteEthPHYGMIIRX
 from liteeth.phy.common import LiteEthPHYMDIO
 
 
+# Constants / Layouts ------------------------------------------------------------------------------
+
 modes = {
-    "GMII": 0,
-    "MII": 1
+    "GMII" : 0,
+    "MII"  : 1,
 }
 
 tx_pads_layout = [("tx_er", 1), ("tx_en", 1), ("tx_data", 8)]
 rx_pads_layout = [("rx_er", 1), ("rx_dv", 1), ("rx_data", 8)]
 
+# LiteEth PHY GMII-MII TX --------------------------------------------------------------------------
 
-class LiteEthPHYGMIIMIITX(Module):
+class LiteEthPHYGMIIMIITX(LiteXModule):
     def __init__(self, pads, mode):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         gmii_tx_pads = Record(tx_pads_layout)
-        gmii_tx = LiteEthPHYGMIITX(gmii_tx_pads)
+        gmii_tx      = LiteEthPHYGMIITX(gmii_tx_pads)
         self.submodules += gmii_tx
 
         mii_tx_pads = Record(tx_pads_layout)
-        mii_tx = LiteEthPHYMIITX(mii_tx_pads)
+        mii_tx      = LiteEthPHYMIITX(mii_tx_pads)
         self.submodules += mii_tx
 
         demux = Demultiplexer(eth_phy_description(8), 2)
         self.submodules += demux
         self.comb += [
             demux.sel.eq(mode == modes["MII"]),
             sink.connect(demux.sink),
@@ -50,108 +55,99 @@
             demux.source1.connect(mii_tx.sink),
         ]
 
 
         if hasattr(pads, "tx_er"):
             pads.tx_er.reset_less = True
             self.comb += pads.tx_er.eq(0)
-        pads.tx_en.reset_less = True
+        pads.tx_en.reset_less   = True
         pads.tx_data.reset_less = True
         self.sync += [
             If(mode == modes["MII"],
                 pads.tx_en.eq(mii_tx_pads.tx_en),
                 pads.tx_data.eq(mii_tx_pads.tx_data),
             ).Else(
                 pads.tx_en.eq(gmii_tx_pads.tx_en),
                 pads.tx_data.eq(gmii_tx_pads.tx_data),
             )
         ]
 
+# LiteEth PHY GMII-MII RX --------------------------------------------------------------------------
 
-class LiteEthPHYGMIIMIIRX(Module):
+class LiteEthPHYGMIIMIIRX(LiteXModule):
     def __init__(self, pads, mode):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         pads_d = Record(rx_pads_layout)
-        pads_d.rx_dv.reset_less = True
+        pads_d.rx_dv.reset_less   = True
         pads_d.rx_data.reset_less = True
         self.sync += [
             pads_d.rx_dv.eq(pads.rx_dv),
-            pads_d.rx_data.eq(pads.rx_data)
+            pads_d.rx_data.eq(pads.rx_data),
         ]
 
-        gmii_rx = LiteEthPHYGMIIRX(pads_d)
-        self.submodules += gmii_rx
-
-        mii_rx = LiteEthPHYMIIRX(pads_d)
-        self.submodules += mii_rx
-
-        mux = Multiplexer(eth_phy_description(8), 2)
-        self.submodules += mux
+        self.gmii_rx = gmii_rx = LiteEthPHYGMIIRX(pads_d)
+        self.mii_rx  = mii_rx  = LiteEthPHYMIIRX(pads_d)
+        self.mux     = mux     = Multiplexer(eth_phy_description(8), 2)
         self.comb += [
             mux.sel.eq(mode == modes["MII"]),
             gmii_rx.source.connect(mux.sink0),
             mii_rx.source.connect(mux.sink1),
             mux.source.connect(source)
         ]
 
+# LiteEth PHY GMII-MII Mode Detection --------------------------------------------------------------
 
-class LiteEthGMIIMIIModeDetection(Module, AutoCSR):
+class LiteEthGMIIMIIModeDetection(LiteXModule):
     def __init__(self, clk_freq):
-        self.mode = Signal()
+        self.mode  = Signal()
         self._mode = CSRStatus()
 
         # # #
 
-        mode = Signal()
+        mode        = Signal()
         update_mode = Signal()
-        self.sync += \
-            If(update_mode,
-                self.mode.eq(mode)
-            )
+        self.sync += If(update_mode, self.mode.eq(mode))
         self.comb += self._mode.status.eq(self.mode)
 
         # Principle:
-        #  sys_clk >= 125MHz
-        #  eth_rx <= 125Mhz
+        #  sys_clk >= 125MHz.
+        #  eth_rx  <= 125Mhz.
         # We generate ticks every 1024 clock cycles in eth_rx domain
         # and measure ticks period in sys_clk domain.
 
-        # Generate a tick every 1024 clock cycles (eth_rx clock domain)
-        eth_tick = Signal()
+        # Generate a tick every 1024 clock cycles (eth_rx clock domain).
+        eth_tick    = Signal()
         eth_counter = Signal(10, reset_less=True)
         self.sync.eth_rx += eth_counter.eq(eth_counter + 1)
         self.comb += eth_tick.eq(eth_counter == 0)
 
-        # Synchronize tick (sys clock domain)
+        # Synchronize tick (sys clock domain).
         sys_tick = Signal()
-        eth_ps = PulseSynchronizer("eth_rx", "sys")
+        self.eth_ps = eth_ps = PulseSynchronizer("eth_rx", "sys")
         self.comb += [
             eth_ps.i.eq(eth_tick),
             sys_tick.eq(eth_ps.o)
         ]
-        self.submodules += eth_ps
 
-        # sys_clk domain counter
-        sys_counter = Signal(24, reset_less=True)
+        # sys_clk domain counter.
+        sys_counter       = Signal(24, reset_less=True)
         sys_counter_reset = Signal()
-        sys_counter_ce = Signal()
+        sys_counter_ce    = Signal()
         self.sync += [
             If(sys_counter_reset,
                sys_counter.eq(0)
             ).Elif(sys_counter_ce,
                 sys_counter.eq(sys_counter + 1)
             )
         ]
 
-        fsm = FSM(reset_state="IDLE")
-        self.submodules += fsm
-
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             sys_counter_reset.eq(1),
             If(sys_tick,
                 NextState("COUNT")
             )
         )
         fsm.act("COUNT",
@@ -168,23 +164,24 @@
             # if freq >= 125MHz-5% use GMII mode
             ).Else(
                 mode.eq(0)
             ),
             NextState("IDLE")
         )
 
+# LiteEth PHY GMII-MII -----------------------------------------------------------------------------
 
-class LiteEthPHYGMIIMII(Module, AutoCSR):
+class LiteEthPHYGMIIMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
     def __init__(self, clock_pads, pads, clk_freq, with_hw_init_reset=True):
         # Note: we can use GMII CRG since it also handles tx clock pad used for MII
-        self.submodules.mode_detection = LiteEthGMIIMIIModeDetection(clk_freq)
+        self.mode_detection = LiteEthGMIIMIIModeDetection(clk_freq)
         mode = self.mode_detection.mode
-        self.submodules.crg = LiteEthPHYGMIICRG(clock_pads, pads, with_hw_init_reset, mode == modes["MII"])
-        self.submodules.tx = ClockDomainsRenamer("eth_tx")(LiteEthPHYGMIIMIITX(pads, mode))
-        self.submodules.rx = ClockDomainsRenamer("eth_rx")(LiteEthPHYGMIIMIIRX(pads, mode))
+        self.crg = LiteEthPHYGMIICRG(clock_pads, pads, with_hw_init_reset, mode == modes["MII"])
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYGMIIMIITX(pads, mode))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYGMIIMIIRX(pads, mode))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/k7_1000basex.py` & `liteeth-2023.8/liteeth/phy/k7_1000basex.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,73 +4,48 @@
 # Copyright (c) 2018-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+
+from litex.soc.cores.clock import S7MMCM
+
 from liteiclink.transceiver.gtx_7series import GTXChannelPLL, GTXTXInit, GTXRXInit
 
 from liteeth.common import *
 from liteeth.phy.pcs_1000basex import *
 
+# K7_1000BASEX PHY ---------------------------------------------------------------------------------
 
-class Open(Signal):
-    pass
-
-
-class Gearbox(Module):
-    def __init__(self):
-        self.tx_data      = Signal(10)
-        self.tx_data_half = Signal(20)
-        self.rx_data_half = Signal(20)
-        self.rx_data      = Signal(10)
-
-        # TX
-        buf = Signal(20)
-        self.sync.eth_tx += buf.eq(Cat(buf[10:], self.tx_data))
-        self.sync.eth_tx_half += self.tx_data_half.eq(buf)
-
-        # RX
-        phase_half       = Signal()
-        phase_half_rereg = Signal()
-        self.sync.eth_rx_half += phase_half_rereg.eq(phase_half)
-        self.sync.eth_rx += [
-            If(phase_half == phase_half_rereg,
-                self.rx_data.eq(self.rx_data_half[10:])
-            ).Else(
-                self.rx_data.eq(self.rx_data_half[:10])
-            ),
-            phase_half.eq(~phase_half),
-        ]
-
-
-# Configured for 200MHz transceiver reference clock
-class K7_1000BASEX(Module, AutoCSR):
+class K7_1000BASEX(LiteXModule):
+    # Configured for 200MHz transceiver reference clock.
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
-    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq, with_csr=True):
+    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq, with_csr=True, rx_polarity=0, tx_polarity=0):
         pcs = PCS(lsb_first=True)
         self.submodules += pcs
 
         self.sink    = pcs.sink
         self.source  = pcs.source
         self.link_up = pcs.link_up
 
-        self.clock_domains.cd_eth_tx      = ClockDomain()
-        self.clock_domains.cd_eth_rx      = ClockDomain()
-        self.clock_domains.cd_eth_tx_half = ClockDomain(reset_less=True)
-        self.clock_domains.cd_eth_rx_half = ClockDomain(reset_less=True)
+        self.cd_eth_tx      = ClockDomain()
+        self.cd_eth_rx      = ClockDomain()
+        self.cd_eth_tx_half = ClockDomain(reset_less=True)
+        self.cd_eth_rx_half = ClockDomain(reset_less=True)
 
         # for specifying clock constraints. 62.5MHz clocks.
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
-        self.crg_reset = Signal()
+        self.reset = Signal()
         if with_csr:
             self.add_csr()
 
         # # #
 
         if isinstance(refclk_or_clk_pads, Signal):
             refclk = refclk_or_clk_pads
@@ -82,657 +57,659 @@
                 i_CEB = 0,
                 o_O   = refclk
             )
 
         # GTX transceiver
         tx_reset       = Signal()
         tx_mmcm_locked = Signal()
+        tx_mmcm_reset  = Signal(reset=1)
         tx_data        = Signal(20)
         tx_reset_done  = Signal()
 
-        rx_reset       = Signal()
-        rx_mmcm_locked = Signal()
-        rx_data        = Signal(20)
-        rx_reset_done  = Signal()
+        rx_reset          = Signal()
+        rx_mmcm_locked    = Signal()
+        rx_mmcm_reset     = Signal(reset=1)
+        rx_data           = Signal(20)
+        rx_reset_done     = Signal()
 
         pll = GTXChannelPLL(refclk, 200e6, 1.25e9)
         self.submodules.pll = pll
 
         # Work around Python's 255 argument limitation.
         gtx_params = dict(
             # Simulation-Only Attributes
-            p_SIM_RECEIVER_DETECT_PASS   ="TRUE",
-            p_SIM_TX_EIDLE_DRIVE_LEVEL   ="X",
-            p_SIM_RESET_SPEEDUP          ="FALSE",
-            p_SIM_CPLLREFCLK_SEL         ="FALSE",
-            p_SIM_VERSION                ="4.0",
+            p_SIM_RECEIVER_DETECT_PASS     = "TRUE",
+            p_SIM_TX_EIDLE_DRIVE_LEVEL     = "X",
+            p_SIM_RESET_SPEEDUP            = "FALSE",
+            p_SIM_CPLLREFCLK_SEL           = "FALSE",
+            p_SIM_VERSION                  = "4.0",
 
             # RX Byte and Word Alignment Attributes
-            p_ALIGN_COMMA_DOUBLE                     = "FALSE",
-            p_ALIGN_COMMA_ENABLE                     = 0b1111111111,
-            p_ALIGN_COMMA_WORD                       = 2,
-            p_ALIGN_MCOMMA_DET                       = "TRUE",
-            p_ALIGN_MCOMMA_VALUE                     = 0b1010000011,
-            p_ALIGN_PCOMMA_DET                       = "TRUE",
-            p_ALIGN_PCOMMA_VALUE                     = 0b0101111100,
-            p_SHOW_REALIGN_COMMA                     = "TRUE",
-            p_RXSLIDE_AUTO_WAIT                      = 7,
-            p_RXSLIDE_MODE                           = "OFF",
-            p_RX_SIG_VALID_DLY                       = 10,
+            p_ALIGN_COMMA_DOUBLE           = "FALSE",
+            p_ALIGN_COMMA_ENABLE           = 0b1111111111,
+            p_ALIGN_COMMA_WORD             = 2,
+            p_ALIGN_MCOMMA_DET             = "TRUE",
+            p_ALIGN_MCOMMA_VALUE           = 0b1010000011,
+            p_ALIGN_PCOMMA_DET             = "TRUE",
+            p_ALIGN_PCOMMA_VALUE           = 0b0101111100,
+            p_SHOW_REALIGN_COMMA           = "TRUE",
+            p_RXSLIDE_AUTO_WAIT            = 7,
+            p_RXSLIDE_MODE                 = "OFF",
+            p_RX_SIG_VALID_DLY             = 10,
 
             # RX 8B/10B Decoder Attributes
-            p_RX_DISPERR_SEQ_MATCH                   = "TRUE",
-            p_DEC_MCOMMA_DETECT                      = "TRUE",
-            p_DEC_PCOMMA_DETECT                      = "TRUE",
-            p_DEC_VALID_COMMA_ONLY                   = "TRUE",
+            p_RX_DISPERR_SEQ_MATCH         = "TRUE",
+            p_DEC_MCOMMA_DETECT            = "TRUE",
+            p_DEC_PCOMMA_DETECT            = "TRUE",
+            p_DEC_VALID_COMMA_ONLY         = "TRUE",
 
             # RX Clock Correction Attributes
-            p_CBCC_DATA_SOURCE_SEL                   = "DECODED",
-            p_CLK_COR_SEQ_2_USE                      = "FALSE",
-            p_CLK_COR_KEEP_IDLE                      = "FALSE",
-            p_CLK_COR_MAX_LAT                        = 9,
-            p_CLK_COR_MIN_LAT                        = 7,
-            p_CLK_COR_PRECEDENCE                     = "TRUE",
-            p_CLK_COR_REPEAT_WAIT                    = 0,
-            p_CLK_COR_SEQ_LEN                        = 1,
-            p_CLK_COR_SEQ_1_ENABLE                   = 0b1111,
-            p_CLK_COR_SEQ_1_1                        = 0b0100000000,
-            p_CLK_COR_SEQ_1_2                        = 0b0000000000,
-            p_CLK_COR_SEQ_1_3                        = 0b0000000000,
-            p_CLK_COR_SEQ_1_4                        = 0b0000000000,
-            p_CLK_CORRECT_USE                        = "FALSE",
-            p_CLK_COR_SEQ_2_ENABLE                   = 0b1111,
-            p_CLK_COR_SEQ_2_1                        = 0b0100000000,
-            p_CLK_COR_SEQ_2_2                        = 0b0000000000,
-            p_CLK_COR_SEQ_2_3                        = 0b0000000000,
-            p_CLK_COR_SEQ_2_4                        = 0b0000000000,
+            p_CBCC_DATA_SOURCE_SEL         = "DECODED",
+            p_CLK_COR_SEQ_2_USE            = "FALSE",
+            p_CLK_COR_KEEP_IDLE            = "FALSE",
+            p_CLK_COR_MAX_LAT              = 9,
+            p_CLK_COR_MIN_LAT              = 7,
+            p_CLK_COR_PRECEDENCE           = "TRUE",
+            p_CLK_COR_REPEAT_WAIT          = 0,
+            p_CLK_COR_SEQ_LEN              = 1,
+            p_CLK_COR_SEQ_1_ENABLE         = 0b1111,
+            p_CLK_COR_SEQ_1_1              = 0b0100000000,
+            p_CLK_COR_SEQ_1_2              = 0b0000000000,
+            p_CLK_COR_SEQ_1_3              = 0b0000000000,
+            p_CLK_COR_SEQ_1_4              = 0b0000000000,
+            p_CLK_CORRECT_USE              = "FALSE",
+            p_CLK_COR_SEQ_2_ENABLE         = 0b1111,
+            p_CLK_COR_SEQ_2_1              = 0b0100000000,
+            p_CLK_COR_SEQ_2_2              = 0b0000000000,
+            p_CLK_COR_SEQ_2_3              = 0b0000000000,
+            p_CLK_COR_SEQ_2_4              = 0b0000000000,
 
             # RX Channel Bonding Attributes
-            p_CHAN_BOND_KEEP_ALIGN                   = "FALSE",
-            p_CHAN_BOND_MAX_SKEW                     = 1,
-            p_CHAN_BOND_SEQ_LEN                      = 1,
-            p_CHAN_BOND_SEQ_1_1                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_2                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_3                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_4                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_1_ENABLE                 = 0b1111,
-            p_CHAN_BOND_SEQ_2_1                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_2                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_3                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_4                      = 0b0000000000,
-            p_CHAN_BOND_SEQ_2_ENABLE                 = 0b1111,
-            p_CHAN_BOND_SEQ_2_USE                    = "FALSE",
-            p_FTS_DESKEW_SEQ_ENABLE                  = 0b1111,
-            p_FTS_LANE_DESKEW_CFG                    = 0b1111,
-            p_FTS_LANE_DESKEW_EN                     = "FALSE",
+            p_CHAN_BOND_KEEP_ALIGN         = "FALSE",
+            p_CHAN_BOND_MAX_SKEW           = 1,
+            p_CHAN_BOND_SEQ_LEN            = 1,
+            p_CHAN_BOND_SEQ_1_1            = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_2            = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_3            = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_4            = 0b0000000000,
+            p_CHAN_BOND_SEQ_1_ENABLE       = 0b1111,
+            p_CHAN_BOND_SEQ_2_1            = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_2            = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_3            = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_4            = 0b0000000000,
+            p_CHAN_BOND_SEQ_2_ENABLE       = 0b1111,
+            p_CHAN_BOND_SEQ_2_USE          = "FALSE",
+            p_FTS_DESKEW_SEQ_ENABLE        = 0b1111,
+            p_FTS_LANE_DESKEW_CFG          = 0b1111,
+            p_FTS_LANE_DESKEW_EN           = "FALSE",
 
             # RX Margin Analysis Attributes
-            p_ES_CONTROL                             = 0b000000,
-            p_ES_ERRDET_EN                           = "FALSE",
-            p_ES_EYE_SCAN_EN                         = "TRUE",
-            p_ES_HORZ_OFFSET                         = 0x000,
-            p_ES_PMA_CFG                             = 0b0000000000,
-            p_ES_PRESCALE                            = 0b00000,
-            p_ES_QUALIFIER                           = 0x00000000000000000000,
-            p_ES_QUAL_MASK                           = 0x00000000000000000000,
-            p_ES_SDATA_MASK                          = 0x00000000000000000000,
-            p_ES_VERT_OFFSET                         = 0b000000000,
+            p_ES_CONTROL                   = 0b000000,
+            p_ES_ERRDET_EN                 = "FALSE",
+            p_ES_EYE_SCAN_EN               = "TRUE",
+            p_ES_HORZ_OFFSET               = 0x000,
+            p_ES_PMA_CFG                   = 0b0000000000,
+            p_ES_PRESCALE                  = 0b00000,
+            p_ES_QUALIFIER                 = 0x00000000000000000000,
+            p_ES_QUAL_MASK                 = 0x00000000000000000000,
+            p_ES_SDATA_MASK                = 0x00000000000000000000,
+            p_ES_VERT_OFFSET               = 0b000000000,
 
             # FPGA RX Interface Attributes
-            p_RX_DATA_WIDTH                          = 20,
+            p_RX_DATA_WIDTH                = 20,
 
             # PMA Attributes
-            p_OUTREFCLK_SEL_INV                      = 0b11,
-            p_PMA_RSV                                = 0x001e7080,
-            p_PMA_RSV2                               = 0x2050,
-            p_PMA_RSV3                               = 0b00,
-            p_PMA_RSV4                               = 0x00000000,
-            p_RX_BIAS_CFG                            = 0b000000000100,
-            p_DMONITOR_CFG                           = 0x000A00,
-            p_RX_CM_SEL                              = 0b11,
-            p_RX_CM_TRIM                             = 0b010,
-            p_RX_DEBUG_CFG                           = 0b000000000000,
-            p_RX_OS_CFG                              = 0b0000010000000,
-            p_TERM_RCAL_CFG                          = 0b10000,
-            p_TERM_RCAL_OVRD                         = 0b0,
-            p_TST_RSV                                = 0x00000000,
-            p_RX_CLK25_DIV                           = 5,
-            p_TX_CLK25_DIV                           = 5,
-            p_UCODEER_CLR                            = 0b0,
+            p_OUTREFCLK_SEL_INV            = 0b11,
+            p_PMA_RSV                      = 0x001e7080,
+            p_PMA_RSV2                     = 0x2050,
+            p_PMA_RSV3                     = 0b00,
+            p_PMA_RSV4                     = 0x00000000,
+            p_RX_BIAS_CFG                  = 0b000000000100,
+            p_DMONITOR_CFG                 = 0x000A00,
+            p_RX_CM_SEL                    = 0b11,
+            p_RX_CM_TRIM                   = 0b010,
+            p_RX_DEBUG_CFG                 = 0b000000000000,
+            p_RX_OS_CFG                    = 0b0000010000000,
+            p_TERM_RCAL_CFG                = 0b10000,
+            p_TERM_RCAL_OVRD               = 0b0,
+            p_TST_RSV                      = 0x00000000,
+            p_RX_CLK25_DIV                 = 5,
+            p_TX_CLK25_DIV                 = 5,
+            p_UCODEER_CLR                  = 0b0,
 
             # PCI Express Attributes
-            p_PCS_PCIE_EN                            = "FALSE",
+            p_PCS_PCIE_EN                  = "FALSE",
 
             # PCS Attributes
-            p_PCS_RSVD_ATTR                          = 0x000000000000,
+            p_PCS_RSVD_ATTR                = 0x000000000000,
 
             # RX Buffer Attributes
-            p_RXBUF_ADDR_MODE                        = "FAST",
-            p_RXBUF_EIDLE_HI_CNT                     = 0b1000,
-            p_RXBUF_EIDLE_LO_CNT                     = 0b0000,
-            p_RXBUF_EN                               = "TRUE",
-            p_RX_BUFFER_CFG                          = 0b000000,
-            p_RXBUF_RESET_ON_CB_CHANGE               = "TRUE",
-            p_RXBUF_RESET_ON_COMMAALIGN              = "FALSE",
-            p_RXBUF_RESET_ON_EIDLE                   = "FALSE",
-            p_RXBUF_RESET_ON_RATE_CHANGE             = "TRUE",
-            p_RXBUFRESET_TIME                        = 0b00001,
-            p_RXBUF_THRESH_OVFLW                     = 61,
-            p_RXBUF_THRESH_OVRD                      = "FALSE",
-            p_RXBUF_THRESH_UNDFLW                    = 4,
-            p_RXDLY_CFG                              = 0x001F,
-            p_RXDLY_LCFG                             = 0x030,
-            p_RXDLY_TAP_CFG                          = 0x0000,
-            p_RXPH_CFG                               = 0x000000,
-            p_RXPHDLY_CFG                            = 0x084020,
-            p_RXPH_MONITOR_SEL                       = 0b00000,
-            p_RX_XCLK_SEL                            = "RXREC",
-            p_RX_DDI_SEL                             = 0b000000,
-            p_RX_DEFER_RESET_BUF_EN                  = "TRUE",
+            p_RXBUF_ADDR_MODE              = "FAST",
+            p_RXBUF_EIDLE_HI_CNT           = 0b1000,
+            p_RXBUF_EIDLE_LO_CNT           = 0b0000,
+            p_RXBUF_EN                     = "TRUE",
+            p_RX_BUFFER_CFG                = 0b000000,
+            p_RXBUF_RESET_ON_CB_CHANGE     = "TRUE",
+            p_RXBUF_RESET_ON_COMMAALIGN    = "FALSE",
+            p_RXBUF_RESET_ON_EIDLE         = "FALSE",
+            p_RXBUF_RESET_ON_RATE_CHANGE   = "TRUE",
+            p_RXBUFRESET_TIME              = 0b00001,
+            p_RXBUF_THRESH_OVFLW           = 61,
+            p_RXBUF_THRESH_OVRD            = "FALSE",
+            p_RXBUF_THRESH_UNDFLW          = 4,
+            p_RXDLY_CFG                    = 0x001F,
+            p_RXDLY_LCFG                   = 0x030,
+            p_RXDLY_TAP_CFG                = 0x0000,
+            p_RXPH_CFG                     = 0x000000,
+            p_RXPHDLY_CFG                  = 0x084020,
+            p_RXPH_MONITOR_SEL             = 0b00000,
+            p_RX_XCLK_SEL                  = "RXREC",
+            p_RX_DDI_SEL                   = 0b000000,
+            p_RX_DEFER_RESET_BUF_EN        = "TRUE",
 
             # CDR Attributes
-            p_RXCDR_CFG                              = 0x03000023ff10100020,
-            p_RXCDR_FR_RESET_ON_EIDLE                = 0b0,
-            p_RXCDR_HOLD_DURING_EIDLE                = 0b0,
-            p_RXCDR_PH_RESET_ON_EIDLE                = 0b0,
-            p_RXCDR_LOCK_CFG                         = 0b010101,
+            p_RXCDR_CFG                    = 0x03000023ff10100020,
+            p_RXCDR_FR_RESET_ON_EIDLE      = 0b0,
+            p_RXCDR_HOLD_DURING_EIDLE      = 0b0,
+            p_RXCDR_PH_RESET_ON_EIDLE      = 0b0,
+            p_RXCDR_LOCK_CFG               = 0b010101,
 
             # RX Initialization and Reset Attributes
-            p_RXCDRFREQRESET_TIME                    = 0b00001,
-            p_RXCDRPHRESET_TIME                      = 0b00001,
-            p_RXISCANRESET_TIME                      = 0b00001,
-            p_RXPCSRESET_TIME                        = 0b00001,
-            p_RXPMARESET_TIME                        = 0b00011,
+            p_RXCDRFREQRESET_TIME          = 0b00001,
+            p_RXCDRPHRESET_TIME            = 0b00001,
+            p_RXISCANRESET_TIME            = 0b00001,
+            p_RXPCSRESET_TIME              = 0b00001,
+            p_RXPMARESET_TIME              = 0b00011,
 
             # RX OOB Signaling Attributes
-            p_RXOOB_CFG                              = 0b0000110,
+            p_RXOOB_CFG                    = 0b0000110,
 
             # RX Gearbox Attributes
-            p_RXGEARBOX_EN                           = "FALSE",
-            p_GEARBOX_MODE                           = 0b000,
+            p_RXGEARBOX_EN                 = "FALSE",
+            p_GEARBOX_MODE                 = 0b000,
 
             # PRBS Detection Attribute
-            p_RXPRBS_ERR_LOOPBACK                    = 0b0,
+            p_RXPRBS_ERR_LOOPBACK          = 0b0,
 
             # Power-Down Attributes
-            p_PD_TRANS_TIME_FROM_P2                  = 0x03c,
-            p_PD_TRANS_TIME_NONE_P2                  = 0x3c,
-            p_PD_TRANS_TIME_TO_P2                    = 0x64,
+            p_PD_TRANS_TIME_FROM_P2        = 0x03c,
+            p_PD_TRANS_TIME_NONE_P2        = 0x3c,
+            p_PD_TRANS_TIME_TO_P2          = 0x64,
 
             # RX OOB Signaling Attributes
-            p_SAS_MAX_COM                            = 64,
-            p_SAS_MIN_COM                            = 36,
-            p_SATA_BURST_SEQ_LEN                     = 0b0101,
-            p_SATA_BURST_VAL                         = 0b100,
-            p_SATA_EIDLE_VAL                         = 0b100,
-            p_SATA_MAX_BURST                         = 8,
-            p_SATA_MAX_INIT                          = 21,
-            p_SATA_MAX_WAKE                          = 7,
-            p_SATA_MIN_BURST                         = 4,
-            p_SATA_MIN_INIT                          = 12,
-            p_SATA_MIN_WAKE                          = 4,
+            p_SAS_MAX_COM                  = 64,
+            p_SAS_MIN_COM                  = 36,
+            p_SATA_BURST_SEQ_LEN           = 0b0101,
+            p_SATA_BURST_VAL               = 0b100,
+            p_SATA_EIDLE_VAL               = 0b100,
+            p_SATA_MAX_BURST               = 8,
+            p_SATA_MAX_INIT                = 21,
+            p_SATA_MAX_WAKE                = 7,
+            p_SATA_MIN_BURST               = 4,
+            p_SATA_MIN_INIT                = 12,
+            p_SATA_MIN_WAKE                = 4,
 
             # RX Fabric Clock Output Control Attributes
-            p_TRANS_TIME_RATE                        = 0x0E,
+            p_TRANS_TIME_RATE              = 0x0E,
 
             # TX Buffer Attributes
-            p_TXBUF_EN                               = "TRUE",
-            p_TXBUF_RESET_ON_RATE_CHANGE             = "TRUE",
-            p_TXDLY_CFG                              = 0x001F,
-            p_TXDLY_LCFG                             = 0x030,
-            p_TXDLY_TAP_CFG                          = 0x0000,
-            p_TXPH_CFG                               = 0x0780,
-            p_TXPHDLY_CFG                            = 0x084020,
-            p_TXPH_MONITOR_SEL                       = 0b00000,
-            p_TX_XCLK_SEL                            = "TXOUT",
+            p_TXBUF_EN                     = "TRUE",
+            p_TXBUF_RESET_ON_RATE_CHANGE   = "TRUE",
+            p_TXDLY_CFG                    = 0x001F,
+            p_TXDLY_LCFG                   = 0x030,
+            p_TXDLY_TAP_CFG                = 0x0000,
+            p_TXPH_CFG                     = 0x0780,
+            p_TXPHDLY_CFG                  = 0x084020,
+            p_TXPH_MONITOR_SEL             = 0b00000,
+            p_TX_XCLK_SEL                  = "TXOUT",
 
             # FPGA TX Interface Attributes
-            p_TX_DATA_WIDTH                          = 20,
+            p_TX_DATA_WIDTH                = 20,
 
             # TX Configurable Driver Attributes
-            p_TX_DEEMPH0                             = 0b00000,
-            p_TX_DEEMPH1                             = 0b00000,
-            p_TX_EIDLE_ASSERT_DELAY                  = 0b110,
-            p_TX_EIDLE_DEASSERT_DELAY                = 0b100,
-            p_TX_LOOPBACK_DRIVE_HIZ                  = "FALSE",
-            p_TX_MAINCURSOR_SEL                      = 0b0,
-            p_TX_DRIVE_MODE                          = "DIRECT",
-            p_TX_MARGIN_FULL_0                       = 0b1001110,
-            p_TX_MARGIN_FULL_1                       = 0b1001001,
-            p_TX_MARGIN_FULL_2                       = 0b1000101,
-            p_TX_MARGIN_FULL_3                       = 0b1000010,
-            p_TX_MARGIN_FULL_4                       = 0b1000000,
-            p_TX_MARGIN_LOW_0                        = 0b1000110,
-            p_TX_MARGIN_LOW_1                        = 0b1000100,
-            p_TX_MARGIN_LOW_2                        = 0b1000010,
-            p_TX_MARGIN_LOW_3                        = 0b1000000,
-            p_TX_MARGIN_LOW_4                        = 0b1000000,
+            p_TX_DEEMPH0                   = 0b00000,
+            p_TX_DEEMPH1                   = 0b00000,
+            p_TX_EIDLE_ASSERT_DELAY        = 0b110,
+            p_TX_EIDLE_DEASSERT_DELAY      = 0b100,
+            p_TX_LOOPBACK_DRIVE_HIZ        = "FALSE",
+            p_TX_MAINCURSOR_SEL            = 0b0,
+            p_TX_DRIVE_MODE                = "DIRECT",
+            p_TX_MARGIN_FULL_0             = 0b1001110,
+            p_TX_MARGIN_FULL_1             = 0b1001001,
+            p_TX_MARGIN_FULL_2             = 0b1000101,
+            p_TX_MARGIN_FULL_3             = 0b1000010,
+            p_TX_MARGIN_FULL_4             = 0b1000000,
+            p_TX_MARGIN_LOW_0              = 0b1000110,
+            p_TX_MARGIN_LOW_1              = 0b1000100,
+            p_TX_MARGIN_LOW_2              = 0b1000010,
+            p_TX_MARGIN_LOW_3              = 0b1000000,
+            p_TX_MARGIN_LOW_4              = 0b1000000,
 
             # TX Gearbox Attributes
-            p_TXGEARBOX_EN                           = "FALSE",
+            p_TXGEARBOX_EN                 = "FALSE",
 
             # TX Initialization and Reset Attributes
-            p_TXPCSRESET_TIME                        = 0b00001,
-            p_TXPMARESET_TIME                        = 0b00001,
+            p_TXPCSRESET_TIME              = 0b00001,
+            p_TXPMARESET_TIME              = 0b00001,
 
             # TX Receiver Detection Attributes
-            p_TX_RXDETECT_CFG                        = 0x1832,
-            p_TX_RXDETECT_REF                        = 0b100,
+            p_TX_RXDETECT_CFG              = 0x1832,
+            p_TX_RXDETECT_REF              = 0b100,
 
             # CPLL Attributes
-            p_CPLL_CFG                               = 0xBC07DC,
-            p_CPLL_FBDIV                             = pll.config["n2"],
-            p_CPLL_FBDIV_45                          = pll.config["n1"],
-            p_CPLL_INIT_CFG                          = 0x00001E,
-            p_CPLL_LOCK_CFG                          = 0x01E8,
-            p_CPLL_REFCLK_DIV                        = pll.config["m"],
-            p_RXOUT_DIV                              = pll.config["d"],
-            p_TXOUT_DIV                              = pll.config["d"],
-            p_SATA_CPLL_CFG                          = "VCO_3000MHZ",
+            p_CPLL_CFG                     = 0xBC07DC,
+            p_CPLL_FBDIV                   = pll.config["n2"],
+            p_CPLL_FBDIV_45                = pll.config["n1"],
+            p_CPLL_INIT_CFG                = 0x00001E,
+            p_CPLL_LOCK_CFG                = 0x01E8,
+            p_CPLL_REFCLK_DIV              = pll.config["m"],
+            p_RXOUT_DIV                    = pll.config["d"],
+            p_TXOUT_DIV                    = pll.config["d"],
+            p_SATA_CPLL_CFG                = "VCO_3000MHZ",
 
             # RX Initialization and Reset Attributes
-            p_RXDFELPMRESET_TIME                     = 0b0001111,
+            p_RXDFELPMRESET_TIME           = 0b0001111,
 
             # RX Equalizer Attributes
-            p_RXLPM_HF_CFG                           = 0b00000011110000,
-            p_RXLPM_LF_CFG                           = 0b00000011110000,
-            p_RX_DFE_GAIN_CFG                        = 0x020FEA,
-            p_RX_DFE_H2_CFG                          = 0b000000000000,
-            p_RX_DFE_H3_CFG                          = 0b000001000000,
-            p_RX_DFE_H4_CFG                          = 0b00011110000,
-            p_RX_DFE_H5_CFG                          = 0b00011100000,
-            p_RX_DFE_KL_CFG                          = 0b0000011111110,
-            p_RX_DFE_LPM_CFG                         = 0x0954,
-            p_RX_DFE_LPM_HOLD_DURING_EIDLE           = 0b0,
-            p_RX_DFE_UT_CFG                          = 0b10001111000000000,
-            p_RX_DFE_VP_CFG                          = 0b00011111100000011,
+            p_RXLPM_HF_CFG                 = 0b00000011110000,
+            p_RXLPM_LF_CFG                 = 0b00000011110000,
+            p_RX_DFE_GAIN_CFG              = 0x020FEA,
+            p_RX_DFE_H2_CFG                = 0b000000000000,
+            p_RX_DFE_H3_CFG                = 0b000001000000,
+            p_RX_DFE_H4_CFG                = 0b00011110000,
+            p_RX_DFE_H5_CFG                = 0b00011100000,
+            p_RX_DFE_KL_CFG                = 0b0000011111110,
+            p_RX_DFE_LPM_CFG               = 0x0954,
+            p_RX_DFE_LPM_HOLD_DURING_EIDLE = 0b0,
+            p_RX_DFE_UT_CFG                = 0b10001111000000000,
+            p_RX_DFE_VP_CFG                = 0b00011111100000011,
 
             # Power-Down Attributes
-            p_RX_CLKMUX_PD                           = 0b1,
-            p_TX_CLKMUX_PD                           = 0b1,
+            p_RX_CLKMUX_PD                 = 0b1,
+            p_TX_CLKMUX_PD                 = 0b1,
 
             # FPGA RX Interface Attribute
-            p_RX_INT_DATAWIDTH                       = 0,
+            p_RX_INT_DATAWIDTH             = 0,
 
             # FPGA TX Interface Attribute
-            p_TX_INT_DATAWIDTH                       = 0,
+            p_TX_INT_DATAWIDTH             = 0,
 
             # TX Configurable Driver Attributes
-            p_TX_QPI_STATUS_EN                       = 0b0,
+            p_TX_QPI_STATUS_EN             = 0b0,
 
             # RX Equalizer Attributes
-            p_RX_DFE_KL_CFG2                         = 0x301148AC,
-            p_RX_DFE_XYD_CFG                         = 0b0000000000000,
+            p_RX_DFE_KL_CFG2               = 0x301148AC,
+            p_RX_DFE_XYD_CFG               = 0b0000000000000,
 
             # TX Configurable Driver Attributes
-            p_TX_PREDRIVER_MODE                      = 0b0
+            p_TX_PREDRIVER_MODE            = 0b0
         )
         gtx_params.update(
             # CPLL Ports
-            o_CPLLFBCLKLOST                  = Open(),
-            o_CPLLLOCK                       = pll.lock,
-            i_CPLLLOCKDETCLK                 = ClockSignal(),
-            i_CPLLLOCKEN                     = 1,
-            i_CPLLPD                         = 0,
-            o_CPLLREFCLKLOST                 = Open(),
-            i_CPLLREFCLKSEL                  = 0b001,
-            i_CPLLRESET                      = pll.reset,
-            i_GTRSVD                         = 0b0000000000000000,
-            i_PCSRSVDIN                      = 0b0000000000000000,
-            i_PCSRSVDIN2                     = 0b00000,
-            i_PMARSVDIN                      = 0b00000,
-            i_PMARSVDIN2                     = 0b00000,
-            i_TSTIN                          = 0b11111111111111111111,
-            o_TSTOUT                         = Open(),
+            o_CPLLFBCLKLOST    = Open(),
+            o_CPLLLOCK         = pll.lock,
+            i_CPLLLOCKDETCLK   = ClockSignal(),
+            i_CPLLLOCKEN       = 1,
+            i_CPLLPD           = 0,
+            o_CPLLREFCLKLOST   = Open(),
+            i_CPLLREFCLKSEL    = 0b001,
+            i_CPLLRESET        = pll.reset,
+            i_GTRSVD           = 0b0000000000000000,
+            i_PCSRSVDIN        = 0b0000000000000000,
+            i_PCSRSVDIN2       = 0b00000,
+            i_PMARSVDIN        = 0b00000,
+            i_PMARSVDIN2       = 0b00000,
+            i_TSTIN            = 0b11111111111111111111,
+            o_TSTOUT           = Open(),
 
             # Channel
-            i_CLKRSVD                        = 0b0000,
+            i_CLKRSVD          = 0b0000,
 
             # Channel - Clocking Ports
-            i_GTGREFCLK                      = 0,
-            i_GTNORTHREFCLK0                 = 0,
-            i_GTNORTHREFCLK1                 = 0,
-            i_GTREFCLK0                      = pll.refclk,
-            i_GTREFCLK1                      = 0,
-            i_GTSOUTHREFCLK0                 = 0,
-            i_GTSOUTHREFCLK1                 = 0,
+            i_GTGREFCLK        = 0,
+            i_GTNORTHREFCLK0   = 0,
+            i_GTNORTHREFCLK1   = 0,
+            i_GTREFCLK0        = pll.refclk,
+            i_GTREFCLK1        = 0,
+            i_GTSOUTHREFCLK0   = 0,
+            i_GTSOUTHREFCLK1   = 0,
 
             # Channel - DRP Ports
-            i_DRPADDR                        = 0,
-            i_DRPCLK                         = 0,
-            i_DRPDI                          = 0,
-            o_DRPDO                          = Open(),
-            i_DRPEN                          = 0,
-            o_DRPRDY                         = Open(),
-            i_DRPWE                          = 0,
+            i_DRPADDR          = 0,
+            i_DRPCLK           = 0,
+            i_DRPDI            = 0,
+            o_DRPDO            = Open(),
+            i_DRPEN            = 0,
+            o_DRPRDY           = Open(),
+            i_DRPWE            = 0,
 
             # Clocking Ports
-            o_GTREFCLKMONITOR                = Open(),
-            i_QPLLCLK                        = 0,
-            i_QPLLREFCLK                     = 0,
-            i_RXSYSCLKSEL                    = 0b00,
-            i_TXSYSCLKSEL                    = 0b00,
+            o_GTREFCLKMONITOR  = Open(),
+            i_QPLLCLK          = 0,
+            i_QPLLREFCLK       = 0,
+            i_RXSYSCLKSEL      = 0b00,
+            i_TXSYSCLKSEL      = 0b00,
 
             # Digital Monitor Ports
-            o_DMONITOROUT                    = Open(),
+            o_DMONITOROUT      = Open(),
 
             # FPGA TX Interface Datapath Configuration
-            i_TX8B10BEN                      = 0,
+            i_TX8B10BEN        = 0,
 
             # Loopback Ports
-            i_LOOPBACK                       = 0b000,
+            i_LOOPBACK         = 0b000,
 
             # PCI Express Ports
-            o_PHYSTATUS                      = Open(),
-            i_RXRATE                         = 0b000,
-            o_RXVALID                        = Open(),
+            o_PHYSTATUS        = Open(),
+            i_RXRATE           = 0b000,
+            o_RXVALID          = Open(),
 
             # Power-Down Ports
-            i_RXPD                           = 0b00,
-            i_TXPD                           = 0b00,
+            i_RXPD             = 0b00,
+            i_TXPD             = 0b00,
 
             # RX 8B/10B Decoder Ports
-            i_SETERRSTATUS                   = 0,
+            i_SETERRSTATUS     = 0,
 
             # RX Initialization and Reset Ports
-            i_EYESCANRESET                   = 0,
-            i_RXUSERRDY                      = rx_mmcm_locked,
+            i_EYESCANRESET     = 0,
+            i_RXUSERRDY        = rx_mmcm_locked,
 
             # RX Margin Analysis Ports
-            o_EYESCANDATAERROR               = Open(),
-            i_EYESCANMODE                    = 0,
-            i_EYESCANTRIGGER                 = 0,
+            o_EYESCANDATAERROR = Open(),
+            i_EYESCANMODE      = 0,
+            i_EYESCANTRIGGER   = 0,
 
             # Receive Ports - CDR Ports
-            i_RXCDRFREQRESET                 = 0,
-            i_RXCDRHOLD                      = 0,
-            o_RXCDRLOCK                      = Open(),
-            i_RXCDROVRDEN                    = 0,
-            i_RXCDRRESET                     = 0,
-            i_RXCDRRESETRSV                  = 0,
+            i_RXCDRFREQRESET   = 0,
+            i_RXCDRHOLD        = 0,
+            o_RXCDRLOCK        = Open(),
+            i_RXCDROVRDEN      = 0,
+            i_RXCDRRESET       = 0,
+            i_RXCDRRESETRSV    = 0,
 
             # Receive Ports - Clock Correction Ports
-            o_RXCLKCORCNT                    = Open(),
+            o_RXCLKCORCNT      = Open(),
 
             # Receive Ports - FPGA RX Interface Datapath Configuration
-            i_RX8B10BEN                      = 0,
+            i_RX8B10BEN        = 0,
 
             # Receive Ports - FPGA RX Interface Ports
-            i_RXUSRCLK                       = ClockSignal("eth_rx_half"),
-            i_RXUSRCLK2                      = ClockSignal("eth_rx_half"),
+            i_RXUSRCLK         = ClockSignal("eth_rx_half"),
+            i_RXUSRCLK2        = ClockSignal("eth_rx_half"),
 
             # Receive Ports - FPGA RX interface Ports
-            o_RXDATA                         = Cat(*[rx_data[10*i:10*i+8] for i in range(2)]),
+            o_RXDATA           = Cat(*[rx_data[10*i:10*i+8] for i in range(2)]),
 
             # Receive Ports - Pattern Checker Ports
-            o_RXPRBSERR                      = Open(),
-            i_RXPRBSSEL                      = 0b000,
+            o_RXPRBSERR        = Open(),
+            i_RXPRBSSEL        = 0b000,
 
             # Receive Ports - Pattern Checker ports
-            i_RXPRBSCNTRESET                 = 0,
+            i_RXPRBSCNTRESET   = 0,
 
             # Receive Ports - RX  Equalizer Ports
-            i_RXDFEXYDEN                     = 1,
-            i_RXDFEXYDHOLD                   = 0,
-            i_RXDFEXYDOVRDEN                 = 0,
+            i_RXDFEXYDEN       = 1,
+            i_RXDFEXYDHOLD     = 0,
+            i_RXDFEXYDOVRDEN   = 0,
 
             # Receive Ports - RX 8B/10B Decoder Ports
-            i_RXDISPERR                      = Cat(*[rx_data[10*i+9] for i in range(2)]),
-            o_RXNOTINTABLE                   = Open(),
+            i_RXDISPERR        = Cat(*[rx_data[10*i+9] for i in range(2)]),
+            o_RXNOTINTABLE     = Open(),
 
             # Receive Ports - RX AFE
-            i_GTXRXP                         = data_pads.rxp,
+            i_GTXRXP           = data_pads.rxp,
             # Receive Ports - RX AFE Ports
-            i_GTXRXN                         = data_pads.rxn,
+            i_GTXRXN           = data_pads.rxn,
 
             # Receive Ports - RX Buffer Bypass Ports
-            i_RXBUFRESET                     = 0,
-            o_RXBUFSTATUS                    = Open(),
-            i_RXDDIEN                        = 0,
-            i_RXDLYBYPASS                    = 1,
-            i_RXDLYEN                        = 0,
-            i_RXDLYOVRDEN                    = 0,
-            i_RXDLYSRESET                    = 0,
-            o_RXDLYSRESETDONE                = Open(),
-            i_RXPHALIGN                      = 0,
-            o_RXPHALIGNDONE                  = Open(),
-            i_RXPHALIGNEN                    = 0,
-            i_RXPHDLYPD                      = 0,
-            i_RXPHDLYRESET                   = 0,
-            o_RXPHMONITOR                    = Open(),
-            i_RXPHOVRDEN                     = 0,
-            o_RXPHSLIPMONITOR                = Open(),
-            o_RXSTATUS                       = Open(),
+            i_RXBUFRESET       = 0,
+            o_RXBUFSTATUS      = Open(),
+            i_RXDDIEN          = 0,
+            i_RXDLYBYPASS      = 1,
+            i_RXDLYEN          = 0,
+            i_RXDLYOVRDEN      = 0,
+            i_RXDLYSRESET      = 0,
+            o_RXDLYSRESETDONE  = Open(),
+            i_RXPHALIGN        = 0,
+            o_RXPHALIGNDONE    = Open(),
+            i_RXPHALIGNEN      = 0,
+            i_RXPHDLYPD        = 0,
+            i_RXPHDLYRESET     = 0,
+            o_RXPHMONITOR      = Open(),
+            i_RXPHOVRDEN       = 0,
+            o_RXPHSLIPMONITOR  = Open(),
+            o_RXSTATUS         = Open(),
 
             # Receive Ports - RX Byte and Word Alignment Ports
-            o_RXBYTEISALIGNED                = Open(),
-            o_RXBYTEREALIGN                  = Open(),
-            o_RXCOMMADET                     = Open(),
-            i_RXCOMMADETEN                   = 1,
-            i_RXMCOMMAALIGNEN                = 1,
-            i_RXPCOMMAALIGNEN                = 1,
+            o_RXBYTEISALIGNED  = Open(),
+            o_RXBYTEREALIGN    = Open(),
+            o_RXCOMMADET       = Open(),
+            i_RXCOMMADETEN     = 1,
+            i_RXMCOMMAALIGNEN  = 1,
+            i_RXPCOMMAALIGNEN  = 1,
 
             # Receive Ports - RX Channel Bonding Ports
-            o_RXCHANBONDSEQ                  = Open(),
-            i_RXCHBONDEN                     = 0,
-            i_RXCHBONDLEVEL                  = 0b000,
-            i_RXCHBONDMASTER                 = 0,
-            o_RXCHBONDO                      = Open(),
-            i_RXCHBONDSLAVE                  = 0,
+            o_RXCHANBONDSEQ    = Open(),
+            i_RXCHBONDEN       = 0,
+            i_RXCHBONDLEVEL    = 0b000,
+            i_RXCHBONDMASTER   = 0,
+            o_RXCHBONDO        = Open(),
+            i_RXCHBONDSLAVE    = 0,
 
             # Receive Ports - RX Channel Bonding Ports
-            o_RXCHANISALIGNED                = Open(),
-            o_RXCHANREALIGN                  = Open(),
+            o_RXCHANISALIGNED  = Open(),
+            o_RXCHANREALIGN    = Open(),
 
             # Receive Ports - RX Equailizer Ports
-            i_RXLPMHFHOLD                    = 0,
-            i_RXLPMHFOVRDEN                  = 0,
-            i_RXLPMLFHOLD                    = 0,
+            i_RXLPMHFHOLD      = 0,
+            i_RXLPMHFOVRDEN    = 0,
+            i_RXLPMLFHOLD      = 0,
 
             # Receive Ports - RX Equalizer Ports
-            i_RXDFEAGCHOLD                   = 0,
-            i_RXDFEAGCOVRDEN                 = 0,
-            i_RXDFECM1EN                     = 0,
-            i_RXDFELFHOLD                    = 0,
-            i_RXDFELFOVRDEN                  = 1,
-            i_RXDFELPMRESET                  = 0,
-            i_RXDFETAP2HOLD                  = 0,
-            i_RXDFETAP2OVRDEN                = 0,
-            i_RXDFETAP3HOLD                  = 0,
-            i_RXDFETAP3OVRDEN                = 0,
-            i_RXDFETAP4HOLD                  = 0,
-            i_RXDFETAP4OVRDEN                = 0,
-            i_RXDFETAP5HOLD                  = 0,
-            i_RXDFETAP5OVRDEN                = 0,
-            i_RXDFEUTHOLD                    = 0,
-            i_RXDFEUTOVRDEN                  = 0,
-            i_RXDFEVPHOLD                    = 0,
-            i_RXDFEVPOVRDEN                  = 0,
-            i_RXDFEVSEN                      = 0,
-            i_RXLPMLFKLOVRDEN                = 0,
-            o_RXMONITOROUT                   = Open(),
-            i_RXMONITORSEL                   = 0,
-            i_RXOSHOLD                       = 0,
-            i_RXOSOVRDEN                     = 0,
+            i_RXDFEAGCHOLD     = 0,
+            i_RXDFEAGCOVRDEN   = 0,
+            i_RXDFECM1EN       = 0,
+            i_RXDFELFHOLD      = 0,
+            i_RXDFELFOVRDEN    = 1,
+            i_RXDFELPMRESET    = 0,
+            i_RXDFETAP2HOLD    = 0,
+            i_RXDFETAP2OVRDEN  = 0,
+            i_RXDFETAP3HOLD    = 0,
+            i_RXDFETAP3OVRDEN  = 0,
+            i_RXDFETAP4HOLD    = 0,
+            i_RXDFETAP4OVRDEN  = 0,
+            i_RXDFETAP5HOLD    = 0,
+            i_RXDFETAP5OVRDEN  = 0,
+            i_RXDFEUTHOLD      = 0,
+            i_RXDFEUTOVRDEN    = 0,
+            i_RXDFEVPHOLD      = 0,
+            i_RXDFEVPOVRDEN    = 0,
+            i_RXDFEVSEN        = 0,
+            i_RXLPMLFKLOVRDEN  = 0,
+            o_RXMONITOROUT     = Open(),
+            i_RXMONITORSEL     = 0,
+            i_RXOSHOLD         = 0,
+            i_RXOSOVRDEN       = 0,
 
             # Receive Ports - RX Fabric ClocK Output Control Ports
-            o_RXRATEDONE                     = Open(),
+            o_RXRATEDONE       = Open(),
 
             # Receive Ports - RX Fabric Output Control Ports
-            o_RXOUTCLK                       = self.rxoutclk,
-            o_RXOUTCLKFABRIC                 = Open(),
-            o_RXOUTCLKPCS                    = Open(),
-            i_RXOUTCLKSEL                    = 0b010,
+            o_RXOUTCLK         = self.rxoutclk,
+            o_RXOUTCLKFABRIC   = Open(),
+            o_RXOUTCLKPCS      = Open(),
+            i_RXOUTCLKSEL      = 0b010,
 
             # Receive Ports - RX Gearbox Ports
-            o_RXDATAVALID                    = Open(),
-            o_RXHEADER                       = Open(),
-            o_RXHEADERVALID                  = Open(),
-            o_RXSTARTOFSEQ                   = Open(),
+            o_RXDATAVALID      = Open(),
+            o_RXHEADER         = Open(),
+            o_RXHEADERVALID    = Open(),
+            o_RXSTARTOFSEQ     = Open(),
 
             # Receive Ports - RX Gearbox Ports
-            i_RXGEARBOXSLIP                  = 0,
+            i_RXGEARBOXSLIP    = 0,
 
             # Receive Ports - RX Initialization and Reset Ports
-            i_GTRXRESET                      = rx_reset,
-            i_RXOOBRESET                     = 0,
-            i_RXPCSRESET                     = 0,
-            i_RXPMARESET                     = 0,
+            i_GTRXRESET        = rx_reset,
+            i_RXOOBRESET       = 0,
+            i_RXPCSRESET       = 0,
+            i_RXPMARESET       = 0,
 
             # Receive Ports - RX Margin Analysis ports
-            i_RXLPMEN                        = 0,
+            i_RXLPMEN          = 0,
 
             # Receive Ports - RX OOB Signaling ports
-            o_RXCOMSASDET                    = Open(),
-            o_RXCOMWAKEDET                   = Open(),
+            o_RXCOMSASDET      = Open(),
+            o_RXCOMWAKEDET     = Open(),
 
             # Receive Ports - RX OOB Signaling ports
-            o_RXCOMINITDET                   = Open(),
+            o_RXCOMINITDET     = Open(),
 
             # Receive Ports - RX OOB signalling Ports
-            o_RXELECIDLE                     = Open(),
-            i_RXELECIDLEMODE                 = 0b11,
+            o_RXELECIDLE       = Open(),
+            i_RXELECIDLEMODE   = 0b11,
 
             # Receive Ports - RX Polarity Control Ports
-            i_RXPOLARITY                     = 0,
+            i_RXPOLARITY       = rx_polarity,
 
             # Receive Ports - RX gearbox ports
-            i_RXSLIDE                        = 0,
+            i_RXSLIDE          = 0,
 
             # Receive Ports - RX8B/10B Decoder Ports
-            o_RXCHARISCOMMA                  = Open(),
-            o_RXCHARISK                      = Cat(*[rx_data[10*i+8] for i in range(2)]),
+            o_RXCHARISCOMMA    = Open(),
+            o_RXCHARISK        = Cat(*[rx_data[10*i+8] for i in range(2)]),
 
             # Receive Ports - Rx Channel Bonding Ports
-            i_RXCHBONDI                      = 0b00000,
+            i_RXCHBONDI        = 0b00000,
 
             # Receive Ports -RX Initialization and Reset Ports
-            o_RXRESETDONE                    = rx_reset_done,
+            o_RXRESETDONE      = rx_reset_done,
 
             # Rx AFE Ports
-            i_RXQPIEN                        = 0,
-            o_RXQPISENN                      = Open(),
-            o_RXQPISENP                      = Open(),
+            i_RXQPIEN          = 0,
+            o_RXQPISENN        = Open(),
+            o_RXQPISENP        = Open(),
 
             # TX Buffer Bypass Ports
-            i_TXPHDLYTSTCLK                  = 0,
+            i_TXPHDLYTSTCLK    = 0,
 
             # TX Configurable Driver Ports
-            i_TXPOSTCURSOR                   = 0b00000,
-            i_TXPOSTCURSORINV                = 0,
-            i_TXPRECURSOR                    = 0b00000,
-            i_TXPRECURSORINV                 = 0,
-            i_TXQPIBIASEN                    = 0,
-            i_TXQPISTRONGPDOWN               = 0,
-            i_TXQPIWEAKPUP                   = 0,
+            i_TXPOSTCURSOR     = 0b00000,
+            i_TXPOSTCURSORINV  = 0,
+            i_TXPRECURSOR      = 0b00000,
+            i_TXPRECURSORINV   = 0,
+            i_TXQPIBIASEN      = 0,
+            i_TXQPISTRONGPDOWN = 0,
+            i_TXQPIWEAKPUP     = 0,
 
             # TX Initialization and Reset Ports
-            i_CFGRESET                       = 0,
-            i_GTTXRESET                      = tx_reset,
-            o_PCSRSVDOUT                     = Open(),
-            i_TXUSERRDY                      = tx_mmcm_locked,
+            i_CFGRESET         = 0,
+            i_GTTXRESET        = tx_reset,
+            o_PCSRSVDOUT       = Open(),
+            i_TXUSERRDY        = tx_mmcm_locked,
 
             # Transceiver Reset Mode Operation
-            i_GTRESETSEL                     = 0,
-            i_RESETOVRD                      = 0,
+            i_GTRESETSEL       = 0,
+            i_RESETOVRD        = 0,
 
             # Transmit Ports - 8b10b Encoder Control Ports
-            i_TXCHARDISPMODE                 = Cat(*[tx_data[10*i+9] for i in range(2)]),
-            i_TXCHARDISPVAL                  = Cat(*[tx_data[10*i+8] for i in range(2)]),
+            i_TXCHARDISPMODE   = Cat(*[tx_data[10*i+9] for i in range(2)]),
+            i_TXCHARDISPVAL    = Cat(*[tx_data[10*i+8] for i in range(2)]),
 
             # Transmit Ports - FPGA TX Interface Ports
-            i_TXUSRCLK                       = ClockSignal("eth_tx_half"),
-            i_TXUSRCLK2                      = ClockSignal("eth_tx_half"),
+            i_TXUSRCLK         = ClockSignal("eth_tx_half"),
+            i_TXUSRCLK2        = ClockSignal("eth_tx_half"),
 
             # Transmit Ports - PCI Express Ports
-            i_TXELECIDLE                     = 0,
-            i_TXMARGIN                       = 0b000,
-            i_TXRATE                         = 0b000,
-            i_TXSWING                        = 0,
+            i_TXELECIDLE       = 0,
+            i_TXMARGIN         = 0b000,
+            i_TXRATE           = 0b000,
+            i_TXSWING          = 0,
 
             # Transmit Ports - Pattern Generator Ports
-            i_TXPRBSFORCEERR                 = 0,
+            i_TXPRBSFORCEERR   = 0,
 
             # Transmit Ports - TX Buffer Bypass Ports
-            i_TXDLYBYPASS                    = 1,
-            i_TXDLYEN                        = 0,
-            i_TXDLYHOLD                      = 0,
-            i_TXDLYOVRDEN                    = 0,
-            i_TXDLYSRESET                    = 0,
-            o_TXDLYSRESETDONE                = Open(),
-            i_TXDLYUPDOWN                    = 0,
-            i_TXPHALIGN                      = 0,
-            o_TXPHALIGNDONE                  = Open(),
-            i_TXPHALIGNEN                    = 0,
-            i_TXPHDLYPD                      = 0,
-            i_TXPHDLYRESET                   = 0,
-            i_TXPHINIT                       = 0,
-            o_TXPHINITDONE                   = Open(),
-            i_TXPHOVRDEN                     = 0,
+            i_TXDLYBYPASS      = 1,
+            i_TXDLYEN          = 0,
+            i_TXDLYHOLD        = 0,
+            i_TXDLYOVRDEN      = 0,
+            i_TXDLYSRESET      = 0,
+            o_TXDLYSRESETDONE  = Open(),
+            i_TXDLYUPDOWN      = 0,
+            i_TXPHALIGN        = 0,
+            o_TXPHALIGNDONE    = Open(),
+            i_TXPHALIGNEN      = 0,
+            i_TXPHDLYPD        = 0,
+            i_TXPHDLYRESET     = 0,
+            i_TXPHINIT         = 0,
+            o_TXPHINITDONE     = Open(),
+            i_TXPHOVRDEN       = 0,
 
             # Transmit Ports - TX Buffer Ports
-            o_TXBUFSTATUS                    = Open(),
+            o_TXBUFSTATUS      = Open(),
 
             # Transmit Ports - TX Configurable Driver Ports
-            i_TXBUFDIFFCTRL                  = 0b100,
-            i_TXDEEMPH                       = 0,
-            i_TXDIFFCTRL                     = 0b1000,
-            i_TXDIFFPD                       = 0,
-            i_TXINHIBIT                      = 0,
-            i_TXMAINCURSOR                   = 0b0000000,
-            i_TXPISOPD                       = 0,
+            i_TXBUFDIFFCTRL    = 0b100,
+            i_TXDEEMPH         = 0,
+            i_TXDIFFCTRL       = 0b1000,
+            i_TXDIFFPD         = 0,
+            i_TXINHIBIT        = 0,
+            i_TXMAINCURSOR     = 0b0000000,
+            i_TXPISOPD         = 0,
 
             # Transmit Ports - TX Data Path interface
-            i_TXDATA                         = Cat(*[tx_data[10*i:10*i+8] for i in range(2)]),
+            i_TXDATA           = Cat(*[tx_data[10*i:10*i+8] for i in range(2)]),
 
             # Transmit Ports - TX Driver and OOB signaling
-            o_GTXTXN                         = data_pads.txn,
-            o_GTXTXP                         = data_pads.txp,
+            o_GTXTXN           = data_pads.txn,
+            o_GTXTXP           = data_pads.txp,
 
             # Transmit Ports - TX Fabric Clock Output Control Ports
-            o_TXOUTCLK                       = self.txoutclk,
-            o_TXOUTCLKFABRIC                 = Open(),
-            o_TXOUTCLKPCS                    = Open(),
-            i_TXOUTCLKSEL                    = 0b010,
-            o_TXRATEDONE                     = Open(),
+            o_TXOUTCLK         = self.txoutclk,
+            o_TXOUTCLKFABRIC   = Open(),
+            o_TXOUTCLKPCS      = Open(),
+            i_TXOUTCLKSEL      = 0b010,
+            o_TXRATEDONE       = Open(),
 
             # Transmit Ports - TX Gearbox Ports
-            i_TXCHARISK                      = 0b00000000,
-            o_TXGEARBOXREADY                 = Open(),
-            i_TXHEADER                       = 0b000,
-            i_TXSEQUENCE                     = 0b0000000,
-            i_TXSTARTSEQ                     = 0,
+            i_TXCHARISK        = 0b00000000,
+            o_TXGEARBOXREADY   = Open(),
+            i_TXHEADER         = 0b000,
+            i_TXSEQUENCE       = 0b0000000,
+            i_TXSTARTSEQ       = 0,
 
             # Transmit Ports - TX Initialization and Reset Ports
-            i_TXPCSRESET                     = 0,
-            i_TXPMARESET                     = 0,
-            o_TXRESETDONE                    = tx_reset_done,
+            i_TXPCSRESET       = 0,
+            i_TXPMARESET       = 0,
+            o_TXRESETDONE      = tx_reset_done,
 
             # Transmit Ports - TX OOB signaling Ports
-            o_TXCOMFINISH                    = Open(),
-            i_TXCOMINIT                      = 0,
-            i_TXCOMSAS                       = 0,
-            i_TXCOMWAKE                      = 0,
-            i_TXPDELECIDLEMODE               = 0,
+            o_TXCOMFINISH      = Open(),
+            i_TXCOMINIT        = 0,
+            i_TXCOMSAS         = 0,
+            i_TXCOMWAKE        = 0,
+            i_TXPDELECIDLEMODE = 0,
 
             # Transmit Ports - TX Polarity Control Ports
-            i_TXPOLARITY                     = 0,
+            i_TXPOLARITY       = tx_polarity,
 
             # Transmit Ports - TX Receiver Detection Ports
-            i_TXDETECTRX                     = 0,
+            i_TXDETECTRX       = 0,
 
             # Transmit Ports - TX8b/10b Encoder Ports
-            i_TX8B10BBYPASS                  = 0b00000000,
+            i_TX8B10BBYPASS    = 0b00000000,
 
             # Transmit Ports - pattern Generator Ports
-            i_TXPRBSSEL                      = 0b000,
+            i_TXPRBSSEL        = 0b000,
 
             # Tx Configurable Driver  Ports
-            o_TXQPISENN                      = Open(),
-            o_TXQPISENP                      = Open(),
+            o_TXQPISENN        = Open(),
+            o_TXQPISENP        = Open(),
         )
         self.specials += Instance("GTXE2_CHANNEL", **gtx_params)
 
         # Get 125MHz clocks back - the GTX is outputting 62.5MHz.
         txoutclk_rebuffer = Signal()
         self.specials += Instance("BUFH",
             i_I = self.txoutclk,
@@ -740,96 +717,51 @@
         )
         rxoutclk_rebuffer = Signal()
         self.specials += Instance("BUFG",
             i_I = self.rxoutclk,
             o_O = rxoutclk_rebuffer
         )
 
-        tx_mmcm_fb        = Signal()
-        tx_mmcm_reset     = Signal(reset=1)
-        clk_tx_unbuf      = Signal()
-        clk_tx_half_unbuf = Signal()
-        self.specials += [
-            Instance("MMCME2_BASE",
-                p_CLKIN1_PERIOD    = 16.0,
-                i_CLKIN1           = txoutclk_rebuffer,
-                i_RST              = tx_mmcm_reset,
-
-                o_CLKFBOUT         = tx_mmcm_fb,
-                i_CLKFBIN          = tx_mmcm_fb,
-
-                p_CLKFBOUT_MULT_F  = 16,
-                o_LOCKED           = tx_mmcm_locked,
-                p_DIVCLK_DIVIDE    = 1,
-
-                p_CLKOUT0_DIVIDE_F = 16,
-                o_CLKOUT0          = clk_tx_half_unbuf,
-                p_CLKOUT1_DIVIDE   = 8,
-                o_CLKOUT1          = clk_tx_unbuf,
-            ),
-            Instance("BUFH",
-                i_I = clk_tx_half_unbuf,
-                o_O = self.cd_eth_tx_half.clk,
-            ),
-            Instance("BUFH",
-                i_I = clk_tx_unbuf,
-                o_O = self.cd_eth_tx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_eth_tx, ~tx_mmcm_locked)
-        ]
-
-        rx_mmcm_fb        = Signal()
-        rx_mmcm_reset     = Signal(reset=1)
-        clk_rx_unbuf      = Signal()
-        clk_rx_half_unbuf = Signal()
-        self.specials += [
-            Instance("MMCME2_BASE",
-                p_CLKIN1_PERIOD    = 16.0,
-                i_CLKIN1           = rxoutclk_rebuffer,
-                i_RST              = rx_mmcm_reset,
-
-                o_CLKFBOUT         = rx_mmcm_fb,
-                i_CLKFBIN          = rx_mmcm_fb,
-
-                p_CLKFBOUT_MULT_F  = 16,
-                o_LOCKED           = rx_mmcm_locked,
-                p_DIVCLK_DIVIDE    = 1,
-
-                p_CLKOUT0_DIVIDE_F = 16,
-                o_CLKOUT0          = clk_rx_half_unbuf,
-                p_CLKOUT1_DIVIDE   = 8,
-                o_CLKOUT1          = clk_rx_unbuf,
-            ),
-            Instance("BUFG",
-                i_I = clk_rx_half_unbuf,
-                o_O = self.cd_eth_rx_half.clk,
-            ),
-            Instance("BUFG",
-                i_I = clk_rx_unbuf,
-                o_O = self.cd_eth_rx.clk,
-            ),
-            AsyncResetSynchronizer(self.cd_eth_rx, ~rx_mmcm_locked)
-        ]
+        # TX MMCM.
+        self.tx_mmcm = tx_mmcm = S7MMCM()
+        tx_mmcm.register_clkin(txoutclk_rebuffer,   62.5e6)
+        tx_mmcm.create_clkout(self.cd_eth_tx_half,  62.5e6, buf="bufh", with_reset=False)
+        tx_mmcm.create_clkout(self.cd_eth_tx,      125.0e6, buf="bufh", with_reset=True)
+        self.comb += tx_mmcm.reset.eq(tx_mmcm_reset)
+        self.comb += tx_mmcm_locked.eq(tx_mmcm.locked)
+
+        # RX MMCM.
+        self.rx_mmcm = rx_mmcm = S7MMCM()
+        rx_mmcm.register_clkin(rxoutclk_rebuffer,   62.5e6)
+        rx_mmcm.create_clkout(self.cd_eth_rx_half,  62.5e6, buf="bufg", with_reset=False)
+        rx_mmcm.create_clkout(self.cd_eth_rx,      125.0e6, buf="bufg", with_reset=True)
+        self.comb += rx_mmcm.reset.eq(rx_mmcm_reset)
+        self.comb += rx_mmcm_locked.eq(rx_mmcm.locked)
 
         # Transceiver init
-        tx_init = GTXTXInit(sys_clk_freq, buffer_enable=True)
+        tx_init = ResetInserter()(GTXTXInit(sys_clk_freq, buffer_enable=True))
+        self.submodules += tx_init
         self.comb += [
+            tx_init.reset.eq(self.reset),
             pll.reset.eq(tx_init.pllreset),
             tx_init.plllock.eq(pll.lock),
-            tx_reset.eq(tx_init.gtXxreset | self.crg_reset)
+            tx_reset.eq(tx_init.gtXxreset),
+            tx_init.Xxresetdone.eq(tx_reset_done),
         ]
         self.sync += tx_mmcm_reset.eq(~pll.lock)
         tx_mmcm_reset.attr.add("no_retiming")
 
 
         rx_init = ResetInserter()(GTXRXInit(sys_clk_freq, buffer_enable=True))
         self.submodules += rx_init
         self.comb += [
-            rx_init.reset.eq(~tx_init.done),
-            rx_reset.eq(rx_init.gtXxreset | self.crg_reset)
+            rx_init.reset.eq(~tx_init.done | self.reset),
+            rx_init.plllock.eq(pll.lock),
+            rx_reset.eq(rx_init.gtXxreset),
+            rx_init.Xxresetdone.eq(rx_reset_done),
         ]
         ps_restart = PulseSynchronizer("eth_tx", "sys")
         self.submodules += ps_restart
         self.comb += [
             ps_restart.i.eq(pcs.restart),
             rx_init.restart.eq(ps_restart.o)
         ]
@@ -848,21 +780,19 @@
                 cdr_locked.eq(1)
             ),
             rx_mmcm_reset.eq(~cdr_locked)
         ]
         rx_mmcm_reset.attr.add("no_retiming")
 
         # Gearbox and PCS connection
-        gearbox = Gearbox()
-        self.submodules += gearbox
-
+        self.gearbox = gearbox = PCSGearbox()
         self.comb += [
             tx_data.eq(gearbox.tx_data_half),
             gearbox.rx_data_half.eq(rx_data),
 
             gearbox.tx_data.eq(pcs.tbi_tx),
             pcs.tbi_rx.eq(gearbox.rx_data)
         ]
 
     def add_csr(self):
-        self._crg_reset = CSRStorage()
-        self.comb += self.crg_reset.eq(self._crg_reset.storage)
+        self._reset = CSRStorage()
+        self.comb += self.reset.eq(self._reset.storage)
```

### Comparing `liteeth-2023.4/liteeth/phy/ku_1000basex.py` & `liteeth-2023.8/liteeth/phy/ku_1000basex.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,88 +5,63 @@
 # Copyright (c) 2019-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.phy.pcs_1000basex import *
 
+# KU_1000BASEX PHY ---------------------------------------------------------------------------------
 
-class Open(Signal):
-    pass
-
-
-class Gearbox(Module):
-    def __init__(self):
-        self.tx_data      = Signal(10)
-        self.tx_data_half = Signal(20)
-        self.rx_data_half = Signal(20)
-        self.rx_data      = Signal(10)
-
-        # TX
-        buf = Signal(20)
-        self.sync.eth_tx += buf.eq(Cat(buf[10:], self.tx_data))
-        self.sync.eth_tx_half += self.tx_data_half.eq(buf)
-
-        # RX
-        phase_half       = Signal()
-        phase_half_rereg = Signal()
-        self.sync.eth_rx_half += phase_half_rereg.eq(phase_half)
-        self.sync.eth_rx += [
-            If(phase_half == phase_half_rereg,
-                self.rx_data.eq(self.rx_data_half[10:])
-            ).Else(
-                self.rx_data.eq(self.rx_data_half[:10])
-            ),
-            phase_half.eq(~phase_half),
-        ]
-
-
-# Configured for 200MHz transceiver reference clock
-class KU_1000BASEX(Module, AutoCSR):
+class KU_1000BASEX(LiteXModule):
+	# Configured for 200MHz transceiver reference clock
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
-    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq):
+    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq, with_csr=True, rx_polarity=0, tx_polarity=0):
         pcs = PCS(lsb_first=True)
         self.submodules += pcs
 
         self.sink    = pcs.sink
         self.source  = pcs.source
         self.link_up = pcs.link_up
 
-        self.clock_domains.cd_eth_tx      = ClockDomain()
-        self.clock_domains.cd_eth_rx      = ClockDomain()
-        self.clock_domains.cd_eth_tx_half = ClockDomain(reset_less=True)
-        self.clock_domains.cd_eth_rx_half = ClockDomain(reset_less=True)
+        self.cd_eth_tx      = ClockDomain()
+        self.cd_eth_rx      = ClockDomain()
+        self.cd_eth_tx_half = ClockDomain(reset_less=True)
+        self.cd_eth_rx_half = ClockDomain(reset_less=True)
 
         # for specifying clock constraints. 125MHz clocks.
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
-        self.crg_reset = CSRStorage()
+        self.reset = Signal()
+        if with_csr:
+            self.add_csr()
 
         # # #
 
         if isinstance(refclk_or_clk_pads, Signal):
             refclk = refclk_or_clk_pads
         else:
             refclk = Signal()
             self.specials += Instance("IBUFDS_GTE3",
                 i_I   = refclk_or_clk_pads.p,
                 i_IB  = refclk_or_clk_pads.n,
                 i_CEB = 0,
                 o_O   = refclk,
             )
 
-        gtpowergood = Signal()
-        pll_reset   = Signal(reset=1)
-        pll_locked  = Signal()
+        gtpowergood   = Signal()
+        pll_reset     = Signal(reset=1)
+        pll_locked    = Signal()
 
         tx_reset      = Signal()
         tx_data       = Signal(20)
         tx_reset_done = Signal()
 
         rx_reset      = Signal()
         rx_data       = Signal(20)
@@ -625,15 +600,15 @@
             i_RXPHALIGNEN         = 0b0,
             i_RXPHALIGN           = 0b0,
             i_RXPHDLYPD           = 0b1,
             i_RXPHDLYRESET        = 0b0,
             i_RXPHOVRDEN          = 0b0,
             i_RXPLLCLKSEL         = 0b00,
             i_RXPMARESET          = 0b0,
-            i_RXPOLARITY          = 0b0,
+            i_RXPOLARITY          = rx_polarity,
             i_RXPRBSCNTRESET      = 0b0,
             i_RXPRBSSEL           = 0b0000,
             i_RXPROGDIVRESET      = 0b0,
             i_RXQPIEN             = 0b0,
             i_RXRATEMODE          = 0b0,
             i_RXRATE              = 0b000,
             i_RXSLIDE             = 0b0,
@@ -642,16 +617,14 @@
             i_RXSYNCALLIN         = 0b0,
             i_RXSYNCIN            = 0b0,
             i_RXSYNCMODE          = 0b0,
             i_RXSYSCLKSEL         = 0b00,
             i_RXUSERRDY           = 0b1,
             i_RXUSRCLK2           = ClockSignal("eth_rx_half"),
             i_RXUSRCLK            = ClockSignal("eth_rx_half"),
-            #i_SATA_BURST         = 0b100,
-            #i_SATA_EIDLE         = 0b100,
             i_SIGVALIDCLK         = 0b0,
             i_TSTIN               = 0b00000000000000000000,
             i_TX8B10BBYPASS       = 0b00000000,
             i_TX8B10BEN           = 0b0,
             i_TXBUFDIFFCTRL       = 0b000,
             i_TXCOMINIT           = 0b0,
             i_TXCOMSAS            = 0b0,
@@ -692,15 +665,15 @@
             i_TXPIPPMOVRDEN       = 0b0,
             i_TXPIPPMPD           = 0b0,
             i_TXPIPPMSEL          = 0b0,
             i_TXPIPPMSTEPSIZE     = 0b00000,
             i_TXPISOPD            = 0b0,
             i_TXPLLCLKSEL         = 0b00,
             i_TXPMARESET          = 0b0,
-            i_TXPOLARITY          = 0b0,
+            i_TXPOLARITY          = tx_polarity,
             i_TXPOSTCURSORINV     = 0b0,
             i_TXPOSTCURSOR        = 0b00000,
             i_TXPRBSFORCEERR      = 0b0,
             i_TXPRBSSEL           = 0b0000,
             i_TXPRECURSORINV      = 0b0,
             i_TXPRECURSOR         = 0b00000,
             i_TXPROGDIVRESET      = 0b0,
@@ -814,17 +787,17 @@
             o_TXQPISENN            = Open(),
             o_TXQPISENP            = Open(),
             o_TXRATEDONE           = Open(),
             o_TXRESETDONE          = tx_reset_done,
             o_TXSYNCDONE           = Open(),
             o_TXSYNCOUT            = Open(),
         )
-        tx_bufg_gt_ce = Signal()
+        tx_bufg_gt_ce  = Signal()
         tx_bufg_gt_clr = Signal()
-        rx_bufg_gt_ce = Signal()
+        rx_bufg_gt_ce  = Signal()
         rx_bufg_gt_clr = Signal()
         self.specials += [
             Instance("GTHE3_CHANNEL", **gth_params),
             Instance("BUFG_GT",
                 i_DIV = 0,
                 i_I   = self.txoutclk,
                 o_O   = self.cd_eth_tx.clk,
@@ -860,22 +833,24 @@
                     pll_reset.eq(0)
                 ).Else(
                     reset_counter.eq(reset_counter + 1)
                 )
             )
         ]
         self.comb += [
-            tx_reset.eq(pll_reset | ~pll_locked | self.crg_reset.storage),
-            rx_reset.eq(pll_reset | ~pll_locked | pcs.restart | self.crg_reset.storage)
+            tx_reset.eq(pll_reset | ~pll_locked | self.reset),
+            rx_reset.eq(pll_reset | ~pll_locked | pcs.restart | self.reset)
         ]
 
         # Gearbox and PCS connection
-        gearbox = Gearbox()
-        self.submodules += gearbox
-
+        self.gearbox = gearbox = PCSGearbox()
         self.comb += [
             tx_data.eq(gearbox.tx_data_half),
             gearbox.rx_data_half.eq(rx_data),
 
             gearbox.tx_data.eq(pcs.tbi_tx),
             pcs.tbi_rx.eq(gearbox.rx_data)
         ]
+
+    def add_csr(self):
+        self._reset = CSRStorage()
+        self.comb += self.reset.eq(self._reset.storage)
```

### Comparing `liteeth-2023.4/liteeth/phy/mii.py` & `liteeth-2023.8/liteeth/phy/mii.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY MII TX -------------------------------------------------------------------------------
 
-def converter_description(dw):
-    payload_layout = [("data", dw)]
-    return EndpointDescription(payload_layout)
-
-
-class LiteEthPHYMIITX(Module):
+class LiteEthPHYMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         if hasattr(pads, "tx_er"):
             pads.tx_er.reset_less = True
             self.sync += pads.tx_er.eq(0)
-        converter = stream.StrideConverter(converter_description(8),
-                                           converter_description(4))
-        self.submodules += converter
+        self.converter = converter = stream.Converter(8, 4)
         self.comb += [
             converter.sink.valid.eq(sink.valid),
             converter.sink.data.eq(sink.data),
             sink.ready.eq(converter.sink.ready),
-            converter.source.ready.eq(1)
+            converter.source.ready.eq(1),
         ]
-        pads.tx_en.reset_less = True
+        pads.tx_en.reset_less   = True
         pads.tx_data.reset_less = True
         self.sync += [
             pads.tx_en.eq(converter.source.valid),
-            pads.tx_data.eq(converter.source.data)
+            pads.tx_data.eq(converter.source.data),
         ]
 
+# LiteEth PHY MII RX -------------------------------------------------------------------------------
 
-class LiteEthPHYMIIRX(Module):
+class LiteEthPHYMIIRX(LiteXModule):
     def __init__(self, pads):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
-        converter = stream.StrideConverter(converter_description(4),
-                                           converter_description(8))
+        converter = stream.Converter(4, 8)
         converter = ResetInserter()(converter)
         self.submodules += converter
 
         self.sync += [
             converter.reset.eq(~pads.rx_dv),
             converter.sink.valid.eq(1),
-            converter.sink.data.eq(pads.rx_data)
+            converter.sink.data.eq(pads.rx_data),
         ]
         self.comb += [
             converter.sink.last.eq(~pads.rx_dv),
-            converter.source.connect(source)
+            converter.source.connect(source),
         ]
 
+# LiteEth PHY MII RX -------------------------------------------------------------------------------
 
-class LiteEthPHYMIICRG(Module, AutoCSR):
+class LiteEthPHYMIICRG(LiteXModule):
     def __init__(self, clock_pads, pads, with_hw_init_reset):
         self._reset = CSRStorage()
 
         # # #
 
         if hasattr(clock_pads, "phy"):
             self.sync.base50 += clock_pads.phy.eq(~clock_pads.phy)
 
         # RX/TX clocks
-        self.clock_domains.cd_eth_rx = ClockDomain()
-        self.clock_domains.cd_eth_tx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
+        self.cd_eth_tx = ClockDomain()
         self.comb += self.cd_eth_rx.clk.eq(clock_pads.rx)
         self.comb += self.cd_eth_tx.clk.eq(clock_pads.tx)
 
         # Reset
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset()
+            self.hw_reset = LiteEthPHYHWReset()
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
+# LiteEth PHY MII ----------------------------------------------------------------------------------
 
-class LiteEthPHYMII(Module, AutoCSR):
+class LiteEthPHYMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 25e6
     rx_clk_freq = 25e6
     def __init__(self, clock_pads, pads, with_hw_init_reset=True):
-        self.submodules.crg = LiteEthPHYMIICRG(clock_pads, pads, with_hw_init_reset)
-        self.submodules.tx =  ClockDomainsRenamer("eth_tx")(LiteEthPHYMIITX(pads))
-        self.submodules.rx = ClockDomainsRenamer("eth_rx")(LiteEthPHYMIIRX(pads))
+        self.crg = LiteEthPHYMIICRG(clock_pads, pads, with_hw_init_reset)
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYMIITX(pads))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYMIIRX(pads))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/model.py` & `liteeth-2023.8/liteeth/phy/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
+from litex.gen import *
+
 from liteeth.common import *
 
+# LiteEth PHY Model CRG ----------------------------------------------------------------------------
 
-class LiteEthPHYModelCRG(Module, AutoCSR):
+class LiteEthPHYModelCRG(LiteXModule):
     def __init__(self):
         self._reset = CSRStorage()
 
         # # #
 
-        self.clock_domains.cd_eth_rx = ClockDomain()
-        self.clock_domains.cd_eth_tx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
+        self.cd_eth_tx = ClockDomain()
         self.comb += [
-            self.cd_eth_rx.clk.eq(ClockSignal()),
-            self.cd_eth_tx.clk.eq(ClockSignal())
+            self.cd_eth_rx.clk.eq(ClockSignal("sys")),
+            self.cd_eth_tx.clk.eq(ClockSignal("sys")),
         ]
 
         reset = self._reset.storage
         self.comb += [
             self.cd_eth_rx.rst.eq(reset),
             self.cd_eth_tx.rst.eq(reset)
         ]
 
+# LiteEth PHY Model --------------------------------------------------------------------------------
 
-class LiteEthPHYModel(Module, AutoCSR):
+class LiteEthPHYModel(LiteXModule):
     dw = 8
     def __init__(self, pads):
-        self.submodules.crg = LiteEthPHYModelCRG()
-        self.sink = sink = stream.Endpoint(eth_phy_description(8))
+        self.crg    = LiteEthPHYModelCRG()
+        self.sink   = sink   = stream.Endpoint(eth_phy_description(8))
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         self.comb += [
             pads.source_valid.eq(self.sink.valid),
             pads.source_data.eq(self.sink.data),
-            self.sink.ready.eq(1)
+            self.sink.ready.eq(1),
         ]
 
         self.sync += [
             self.source.valid.eq(pads.sink_valid),
             self.source.data.eq(pads.sink_data),
         ]
-        self.comb += [
-            self.source.last.eq(~pads.sink_valid & self.source.valid),
-        ]
+        self.comb += self.source.last.eq(~pads.sink_valid & self.source.valid)
```

### Comparing `liteeth-2023.4/liteeth/phy/pcs_1000basex.py` & `liteeth-2023.8/liteeth/phy/pcs_1000basex.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,59 +4,52 @@
 # Copyright (c) 2018-2020 Sebastien Bourdeauducq <sb@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from math import ceil
 
 from migen import *
 from migen.genlib.fsm import *
-from migen.genlib.misc import WaitTimer
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+from litex.gen.genlib.misc import WaitTimer
+from litex.gen.genlib.cdc import BusSynchronizer
+
 from litex.soc.interconnect import stream
-from litex.soc.cores import code_8b10b
+from litex.soc.cores.code_8b10b import K, D, Encoder, Decoder
 
 from liteeth.common import *
 
+# PCS TX -------------------------------------------------------------------------------------------
 
-__all__ = ["TransmitPath", "ReceivePath", "PCS"]
-
-
-def K(x, y):
-    return (y << 5) | x
-
-
-def D(x, y):
-    return (y << 5) | x
-
-
-class TransmitPath(Module):
+class PCSTX(LiteXModule):
     def __init__(self, lsb_first=False):
-        self.config_stb = Signal()
-        self.config_reg = Signal(16)
-        self.tx_stb = Signal()
-        self.tx_ack = Signal()
-        self.tx_data = Signal(8)
+        self.config_valid = Signal()
+        self.config_reg   = Signal(16)
+        self.tx_valid     = Signal()
+        self.tx_ready     = Signal()
+        self.tx_data      = Signal(8)
 
-        self.submodules.encoder = code_8b10b.Encoder(lsb_first=lsb_first)
+        self.encoder = Encoder(lsb_first=lsb_first)
 
         # SGMII Speed Adaptation
         self.sgmii_speed = Signal(2)
 
         # # #
 
         parity = Signal()
         c_type = Signal()
         self.sync += parity.eq(~parity)
 
-        config_reg_buffer = Signal(16)
+        config_reg_buffer      = Signal(16)
         load_config_reg_buffer = Signal()
         self.sync += If(load_config_reg_buffer, config_reg_buffer.eq(self.config_reg))
 
-        # Timer for SGMII data rates
-        timer = Signal(max=1000)
+        # Timer for SGMII data rates.
+        timer    = Signal(max=1000)
         timer_en = Signal()
         self.sync += [
             If(~timer_en | (timer == 0),
                 If(self.sgmii_speed == 0b00,
                     timer.eq(99)
                 ).Elif(self.sgmii_speed == 0b01,
                     timer.eq(9)
@@ -64,34 +57,32 @@
                     timer.eq(0)
                 )
             ).Elif(timer_en,
                 timer.eq(timer - 1)
             )
         ]
 
-        fsm = FSM()
-        self.submodules += fsm
-
+        self.fsm = fsm = FSM()
         fsm.act("START",
-            If(self.config_stb,
-                self.tx_ack.eq(1),  # discard TX data if we are in config_reg phase
+            If(self.config_valid,
+                self.tx_ready.eq(1),  # Discard TX data if we are in config_reg phase.
                 load_config_reg_buffer.eq(1),
                 self.encoder.k[0].eq(1),
                 self.encoder.d[0].eq(K(28, 5)),
                 NextState("CONFIG_D")
             ).Else(
-                If(self.tx_stb,
-                    # the first byte sent is replaced by /S/
-                    self.tx_ack.eq((timer == 0)),
+                If(self.tx_valid,
+                    # The first byte sent is replaced by /S/.
+                    self.tx_ready.eq((timer == 0)),
                     timer_en.eq(1),
                     self.encoder.k[0].eq(1),
                     self.encoder.d[0].eq(K(27, 7)),
                     NextState("DATA")
                 ).Else(
-                    self.tx_ack.eq(1),  # discard TX data
+                    self.tx_ready.eq(1),  # Discard TX data.
                     self.encoder.k[0].eq(1),
                     self.encoder.d[0].eq(K(28, 5)),
                     NextState("IDLE")
                 )
             )
         )
         fsm.act("CONFIG_D",
@@ -108,32 +99,32 @@
             NextState("CONFIG_REG_MSB")
         )
         fsm.act("CONFIG_REG_MSB",
             self.encoder.d[0].eq(config_reg_buffer[8:]),
             NextState("START")
         )
         fsm.act("IDLE",
-            # due to latency in the encoder, we read here the disparity
+            # Due to latency in the encoder, we read here the disparity
             # just before the K28.5 was sent. K28.5 flips the disparity.
             If(self.encoder.disparity[0],
-                # correcting /I1/ (D5.6 preserves the disparity)
+                # Correcting /I1/ (D5.6 preserves the disparity).
                 self.encoder.d[0].eq(D(5, 6))
             ).Else(
-                # preserving /I2/ (D16.2 flips the disparity)
+                # Preserving /I2/ (D16.2 flips the disparity).
                 self.encoder.d[0].eq(D(16, 2))
             ),
             NextState("START")
         )
         fsm.act("DATA",
-            If(self.tx_stb,
-                self.tx_ack.eq((timer == 0)),
+            If(self.tx_valid,
+                self.tx_ready.eq((timer == 0)),
                 timer_en.eq(1),
                 self.encoder.d[0].eq(self.tx_data)
             ).Else(
-                self.tx_ack.eq(1),
+                self.tx_ready.eq(1),
                 # /T/
                 self.encoder.k[0].eq(1),
                 self.encoder.d[0].eq(K(29, 7)),
                 NextState("CARRIER_EXTEND_1")
             )
         )
         fsm.act("CARRIER_EXTEND_1",
@@ -149,51 +140,52 @@
         fsm.act("CARRIER_EXTEND_2",
             # /R/
             self.encoder.k[0].eq(1),
             self.encoder.d[0].eq(K(23, 7)),
             NextState("START")
         )
 
+# PCS RX -------------------------------------------------------------------------------------------
 
-class ReceivePath(Module):
+class PCSRX(LiteXModule):
     def __init__(self, lsb_first=False):
-        self.rx_en = Signal()
+        self.rx_en   = Signal()
         self.rx_data = Signal(8)
 
-        self.seen_valid_ci = Signal()
+        self.seen_valid_ci   = Signal()
         self.seen_config_reg = Signal()
-        self.config_reg = Signal(16)
+        self.config_reg      = Signal(16)
 
-        self.submodules.decoder = code_8b10b.Decoder(lsb_first=lsb_first)
+        self.decoder = Decoder(lsb_first=lsb_first)
 
-        # SGMII Speed Adaptation
+        # SGMII Speed Adaptation.
         self.sgmii_speed = Signal(2)
-        self.sample_en = Signal()
+        self.sample_en   = Signal()
 
         # # #
 
-        config_reg_lsb = Signal(8)
+        config_reg_lsb      = Signal(8)
         load_config_reg_lsb = Signal()
         load_config_reg_msb = Signal()
         self.sync += [
             self.seen_config_reg.eq(0),
-            If(load_config_reg_lsb,
+            If(load_config_reg_lsb, 
                 config_reg_lsb.eq(self.decoder.d)
             ),
             If(load_config_reg_msb,
                 self.config_reg.eq(Cat(config_reg_lsb, self.decoder.d)),
                 self.seen_config_reg.eq(1)
             )
         ]
 
         first_preamble_byte = Signal()
         self.comb += self.rx_data.eq(Mux(first_preamble_byte, 0x55, self.decoder.d))
 
-        # Timer for SGMII data rates
-        timer = Signal(max=1000)
+        # Timer for SGMII data rates.
+        timer    = Signal(max=1000)
         timer_en = Signal()
         self.sync += [
             If(~timer_en | (timer == 0),
                 If(self.sgmii_speed == 0b00,
                     timer.eq(99)
                 ).Elif(self.sgmii_speed == 0b01,
                     timer.eq(9)
@@ -204,17 +196,15 @@
                 timer.eq(timer - 1)
             )
         ]
 
         # Speed adaptation
         self.comb += self.sample_en.eq(self.rx_en & (timer == 0))
 
-        fsm = FSM()
-        self.submodules += fsm
-
+        self.fsm = fsm = FSM()
         fsm.act("START",
             If(self.decoder.k,
                 If(self.decoder.d == K(28, 5),
                     NextState("K28_5")
                 ),
                 If(self.decoder.d == K(27, 7),
                     self.rx_en.eq(1),
@@ -264,52 +254,78 @@
                 NextState("START")
             ).Else(
                 self.rx_en.eq(1),
                 timer_en.eq(1)
             )
         )
 
+# PCS Gearbox --------------------------------------------------------------------------------------
+
+class PCSGearbox(LiteXModule):
+    def __init__(self):
+        self.tx_data      = Signal(10)
+        self.tx_data_half = Signal(20)
+        self.rx_data_half = Signal(20)
+        self.rx_data      = Signal(10)
+
+        # # #
+
+        # TX
+        buf = Signal(20)
+        self.sync.eth_tx += buf.eq(Cat(buf[10:], self.tx_data))
+        self.sync.eth_tx_half += self.tx_data_half.eq(buf)
+
+        # RX
+        phase_half       = Signal()
+        phase_half_rereg = Signal()
+        self.sync.eth_rx_half += phase_half_rereg.eq(phase_half)
+        self.sync.eth_rx += [
+            If(phase_half == phase_half_rereg,
+                self.rx_data.eq(self.rx_data_half[10:])
+            ).Else(
+                self.rx_data.eq(self.rx_data_half[:10])
+            ),
+            phase_half.eq(~phase_half),
+        ]
+
+# PCS ----------------------------------------------------------------------------------------------
 
-class PCS(Module):
+class PCS(LiteXModule):
     def __init__(self, lsb_first=False, check_period=6e-3, more_ack_time=10e-3):
-        self.submodules.tx = ClockDomainsRenamer("eth_tx")(
-            TransmitPath(lsb_first=lsb_first))
-        self.submodules.rx = ClockDomainsRenamer("eth_rx")(
-            ReceivePath(lsb_first=lsb_first))
+        self.tx = ClockDomainsRenamer("eth_tx")(PCSTX(lsb_first=lsb_first))
+        self.rx = ClockDomainsRenamer("eth_rx")(PCSRX(lsb_first=lsb_first))
 
         self.tbi_tx = self.tx.encoder.output[0]
         self.tbi_rx = self.rx.decoder.input
-        self.sink = stream.Endpoint(eth_phy_description(8))
+        self.sink   = stream.Endpoint(eth_phy_description(8))
         self.source = stream.Endpoint(eth_phy_description(8))
 
         self.link_up = Signal()
         self.restart = Signal()
 
-        # SGMII Speed Adaptation
-        is_sgmii = Signal()
-        self.link_partner_adv_ability = Signal(16)
+        self.lp_abi = BusSynchronizer(16, "eth_rx", "eth_tx")
 
         # # #
-
-        # endpoint interface
+        
+        # Endpoint interface.
         self.comb += [
-            self.tx.tx_stb.eq(self.sink.valid),
-            self.sink.ready.eq(self.tx.tx_ack),
+            self.tx.tx_valid.eq(self.sink.valid),
+            self.sink.ready.eq(self.tx.tx_ready),
             self.tx.tx_data.eq(self.sink.data),
         ]
 
         rx_en_d = Signal()
         self.sync.eth_rx += [
             rx_en_d.eq(self.rx.rx_en),
             self.source.valid.eq(self.rx.sample_en),
-            self.source.data.eq(self.rx.rx_data)
+            self.source.data.eq(self.rx.rx_data),
         ]
         self.comb += self.source.last.eq(~self.rx.rx_en & rx_en_d)
 
-        # main module
+        # Main module.
         seen_valid_ci = PulseSynchronizer("eth_rx", "eth_tx")
         self.submodules += seen_valid_ci
         self.comb += seen_valid_ci.i.eq(self.rx.seen_valid_ci)
 
         checker_max_val = ceil(check_period*125e6)
         checker_counter = Signal(max=checker_max_val+1)
         checker_tick = Signal()
@@ -322,119 +338,132 @@
             ).Else(
                 checker_counter.eq(checker_counter-1)
             ),
             If(seen_valid_ci.o, checker_ok.eq(1)),
             If(checker_tick, checker_ok.eq(0))
         ]
 
+        # Control if tx_config_reg should be empty.
+        tx_config_empty = Signal()
+        # Detections in SGMII mode.
+        is_sgmii = Signal()
+        linkdown = Signal()
+        self.comb += [
+            is_sgmii.eq(self.lp_abi.o[0]),
+            # Detect that link is down:
+            # - 1000BASE-X : linkup can be inferred by non-empty reg.
+            # - SGMII      : linkup is indicated with bit 15.
+            linkdown.eq((self.lp_abi.o[0] & ~self.lp_abi.o[15]) | (self.lp_abi.o == 0)),
+            self.tx.sgmii_speed.eq(Mux(self.lp_abi.o[0],
+                self.lp_abi.o[10:12], 0b10)),
+            self.rx.sgmii_speed.eq(Mux(self.lp_abi.i[0],
+                self.lp_abi.i[10:12], 0b10))
+        ]
         autoneg_ack = Signal()
-        self.comb += self.tx.config_reg.eq(
-            (is_sgmii) |            # SGMII-specific
-            (~is_sgmii << 5) |      # Full-duplex
-            (autoneg_ack << 14)     # ACK
-        )
+        self.comb += [
+            self.tx.config_reg.eq(Mux(tx_config_empty, 0,
+                (is_sgmii)                          | # SGMII: SGMII in-use
+                (~is_sgmii << 5)                    | # 1000BASE-X: Full-duplex
+                (Mux(self.lp_abi.o[0],                # SGMII: Speed
+                    self.lp_abi.o[10:12], 0) << 10) |
+                (is_sgmii << 12)                    | # SGMII: Full-duplex
+                (autoneg_ack << 14)                 | # SGMII/1000BASE-X: Acknowledge Bit
+                (is_sgmii & self.link_up)             # SGMII: Link-up
+            ))
+        ]
 
         rx_config_reg_abi = PulseSynchronizer("eth_rx", "eth_tx")
         rx_config_reg_ack = PulseSynchronizer("eth_rx", "eth_tx")
-        self.submodules += [
-            rx_config_reg_abi, rx_config_reg_ack
-        ]
-
-        more_ack_timer = ClockDomainsRenamer("eth_tx")(
-            WaitTimer(ceil(more_ack_time*125e6)))
-        self.submodules += more_ack_timer
-
-        fsm_inited = Signal()
-        config_reg_empty = Signal()
-
-        fsm = ClockDomainsRenamer("eth_tx")(FSM())
-        self.submodules += fsm
+        self.submodules += rx_config_reg_abi, rx_config_reg_ack
 
+        more_ack_timer = ClockDomainsRenamer("eth_tx")(WaitTimer(ceil(more_ack_time*125e6)))
+        # SGMII: use 1.6ms link_timer
+        sgmii_ack_timer = ClockDomainsRenamer("eth_tx")(WaitTimer(ceil(1.6e-3*125e6)))
+        self.submodules += more_ack_timer, sgmii_ack_timer
+
+        self.fsm = fsm = ClockDomainsRenamer("eth_tx")(FSM())
+        # AN_ENABLE
+        fsm.act("AUTONEG_BREAKLINK",
+            self.tx.config_valid.eq(1),
+            tx_config_empty.eq(1),
+            more_ack_timer.wait.eq(1),
+            If(more_ack_timer.done,
+                NextState("AUTONEG_WAIT_ABI")
+            )
+        )
+        # ABILITY_DETECT
         fsm.act("AUTONEG_WAIT_ABI",
-            self.tx.config_stb.eq(fsm_inited),
+            self.tx.config_valid.eq(1),
             If(rx_config_reg_abi.o,
-                NextValue(fsm_inited, 1),
                 NextState("AUTONEG_WAIT_ACK")
             ),
             If(checker_tick & ~checker_ok,
                 self.restart.eq(1),
-                NextState("AUTONEG_WAIT_ABI")
+                NextState("AUTONEG_BREAKLINK")
             )
         )
+        # ACKNOWLEDGE_DETECT
         fsm.act("AUTONEG_WAIT_ACK",
-            self.tx.config_stb.eq(1),
+            self.tx.config_valid.eq(1),
             autoneg_ack.eq(1),
             If(rx_config_reg_ack.o,
                 NextState("AUTONEG_SEND_MORE_ACK")
             ),
             If(checker_tick & ~checker_ok,
                 self.restart.eq(1),
-                NextState("AUTONEG_WAIT_ABI")
+                NextState("AUTONEG_BREAKLINK")
             )
         )
         # COMPLETE_ACKNOWLEDGE
         fsm.act("AUTONEG_SEND_MORE_ACK",
-            self.tx.config_stb.eq(1),
+            self.tx.config_valid.eq(1),
             autoneg_ack.eq(1),
-            more_ack_timer.wait.eq(1),
-            If(more_ack_timer.done,
+            more_ack_timer.wait.eq(~is_sgmii),
+            sgmii_ack_timer.wait.eq(is_sgmii),
+            If((is_sgmii & sgmii_ack_timer.done) |
+                (~is_sgmii & more_ack_timer.done),
                 NextState("RUNNING")
             ),
             If(checker_tick & ~checker_ok,
                 self.restart.eq(1),
-                NextState("AUTONEG_WAIT_ABI")
+                NextState("AUTONEG_BREAKLINK")
             )
         )
         # LINK_OK
         fsm.act("RUNNING",
             self.link_up.eq(1),
-            If((checker_tick & ~checker_ok) | config_reg_empty,
+            If((checker_tick & ~checker_ok) | linkdown,
                 self.restart.eq(1),
-                NextState("AUTONEG_WAIT_ABI")
+                NextState("AUTONEG_BREAKLINK")
             )
         )
 
-        c_counter = Signal(max=5)
-        previous_config_reg = Signal(16)
-        preack_config_reg = Signal(16)
+        c_counter       = Signal(max=5)
+        prev_config_reg = Signal(16)
         self.sync.eth_rx += [
             # Restart consistency counter
             If(self.rx.seen_config_reg,
                 c_counter.eq(4)
             ).Elif(c_counter != 0,
                 c_counter.eq(c_counter - 1)
             ),
 
             rx_config_reg_abi.i.eq(0),
             rx_config_reg_ack.i.eq(0),
             If(self.rx.seen_config_reg,
-                previous_config_reg.eq(self.rx.config_reg),
-                If((c_counter == 1) &
-                    ((previous_config_reg|0x4000) == (self.rx.config_reg|0x4000)) &
-                    ((self.rx.config_reg | 1) != 1),
-                    # Ability match
-                    rx_config_reg_abi.i.eq(1),
-                    preack_config_reg.eq(previous_config_reg),
+                # Record current config_reg for comparison in the next clock cycle
+                prev_config_reg.eq(self.rx.config_reg),
+                # Compare consecutive values of config_reg
+                If((c_counter == 1) & (prev_config_reg&0xbfff == self.rx.config_reg&0xbfff),
                     # Acknowledgement/Consistency match
-                    If((previous_config_reg[14] & self.rx.config_reg[14]) &
-                        ((preack_config_reg|0x4000) == (self.rx.config_reg|0x4000)),
-                        rx_config_reg_ack.i.eq(1)
+                    If(prev_config_reg[14] & self.rx.config_reg[14],
+                        rx_config_reg_ack.i.eq(1),
+                    )
+                    # Ability match
+                    .Else(
+                        rx_config_reg_abi.i.eq(1),
                     )
                 ),
                 # Record advertised ability of link partner
-                self.link_partner_adv_ability.eq(self.rx.config_reg)
+                self.lp_abi.i.eq(self.rx.config_reg)
             )
         ]
-
-        # Speed detection via SGMII
-        sgmii_speed = Mux(is_sgmii,
-            self.link_partner_adv_ability[10:12], 0b10)
-        self.comb += [
-            is_sgmii.eq(self.link_partner_adv_ability[0]),
-            self.tx.sgmii_speed.eq(sgmii_speed),
-            self.rx.sgmii_speed.eq(sgmii_speed)
-        ]
-
-        # Detect that config_reg is empty
-        self.comb += [
-            config_reg_empty.eq((self.link_partner_adv_ability | 1) == 1)
-        ]
```

### Comparing `liteeth-2023.4/liteeth/phy/rmii.py` & `liteeth-2023.8/liteeth/phy/rmii.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,154 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2018 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.cdc import MultiReg
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from litex.build.io import DDROutput
 
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY RMII TX ------------------------------------------------------------------------------
 
-def converter_description(dw):
-    payload_layout = [("data", dw)]
-    return EndpointDescription(payload_layout)
-
-
-class LiteEthPHYRMIITX(Module):
+class LiteEthPHYRMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
-        converter = stream.StrideConverter(converter_description(8),
-                                           converter_description(2))
-        self.submodules += converter
+        self.converter = converter = stream.Converter(8, 2)
         self.comb += [
             converter.sink.valid.eq(sink.valid),
             converter.sink.data.eq(sink.data),
             sink.ready.eq(converter.sink.ready),
-            converter.source.ready.eq(1)
+            converter.source.ready.eq(1),
         ]
-        pads.tx_en.reset_less = True
+        pads.tx_en.reset_less   = True
         pads.tx_data.reset_less = True
         self.sync += [
             pads.tx_en.eq(converter.source.valid),
             pads.tx_data.eq(converter.source.data)
         ]
 
+# LiteEth PHY RMII RX ------------------------------------------------------------------------------
 
-class LiteEthPHYRMIIRX(Module):
+class LiteEthPHYRMIIRX(LiteXModule):
     def __init__(self, pads):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
-        converter = stream.StrideConverter(converter_description(2),
-                                           converter_description(8))
+        converter = stream.Converter(2, 8)
         converter = ResetInserter()(converter)
-        self.submodules += converter
+        self.converter = converter
 
         converter_sink_valid = Signal()
-        converter_sink_data = Signal(2)
+        converter_sink_data  = Signal(2)
 
         self.specials += [
             MultiReg(converter_sink_valid, converter.sink.valid, n=2),
-            MultiReg(converter_sink_data, converter.sink.data, n=2)
+            MultiReg(converter_sink_data,  converter.sink.data,  n=2)
         ]
 
-        crs_dv = Signal()
+        crs_dv   = Signal()
         crs_dv_d = Signal()
-        rx_data = Signal(2)
+        rx_data  = Signal(2)
         self.sync += [
             crs_dv.eq(pads.crs_dv),
             crs_dv_d.eq(crs_dv),
             rx_data.eq(pads.rx_data)
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(crs_dv & (rx_data != 0b00),
                 converter_sink_valid.eq(1),
                 converter_sink_data.eq(rx_data),
                 NextState("RECEIVE")
             ).Else(
                converter.reset.eq(1)
             )
         )
         fsm.act("RECEIVE",
             converter_sink_valid.eq(1),
             converter_sink_data.eq(rx_data),
-            # end of frame when 2 consecutives 0 on crs_dv
+            # End of frame when 2 consecutives 0 on crs_dv.
             If(~(crs_dv | crs_dv_d),
               converter.sink.last.eq(1),
               NextState("IDLE")
             )
         )
         self.comb += converter.source.connect(source)
 
+# LiteEth PHY RMII CRG -----------------------------------------------------------------------------
 
-class LiteEthPHYRMIICRG(Module, AutoCSR):
-    def __init__(self, clock_pads, pads, refclk_cd, with_hw_init_reset):
+class LiteEthPHYRMIICRG(LiteXModule):
+    def __init__(self, clock_pads, pads, refclk_cd,
+        with_hw_init_reset     = True,
+        with_refclk_ddr_output = True):
         self._reset = CSRStorage()
 
         # # #
 
         # RX/TX clocks
 
-        self.clock_domains.cd_eth_rx = ClockDomain()
-        self.clock_domains.cd_eth_tx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
+        self.cd_eth_tx = ClockDomain()
 
         # When no refclk_cd, use clock_pads.ref_clk as RMII reference clock.
         if refclk_cd is None:
-            self.comb += self.cd_eth_rx.clk.eq(clock_pads.ref_clk)
-            self.comb += self.cd_eth_tx.clk.eq(clock_pads.ref_clk)
+            self.cd_eth_rx.clk = clock_pads.ref_clk
+            self.cd_eth_tx.clk = self.cd_eth_rx.clk
 
         # Else use refclk_cd as RMII reference clock (provided by user design).
         else:
             self.comb += self.cd_eth_rx.clk.eq(ClockSignal(refclk_cd))
             self.comb += self.cd_eth_tx.clk.eq(ClockSignal(refclk_cd))
             # Drive clock_pads if provided.
             if clock_pads is not None:
-                self.specials += DDROutput(0, 1, clock_pads.ref_clk, ClockSignal("eth_tx"))
+                if with_refclk_ddr_output:
+                    self.specials += DDROutput(i1=0, i2=1, o=clock_pads.ref_clk, clk=ClockSignal("eth_tx"))
+                else:
+                    self.comb += clock_pads.ref_clk.eq(~ClockSignal("eth_tx")) # CHEKCME: Keep Invert?
 
         # Reset
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset()
+            self.hw_reset = LiteEthPHYHWReset()
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
 
-class LiteEthPHYRMII(Module, AutoCSR):
+# LiteEth PHY RMII ---------------------------------------------------------------------------------
+
+class LiteEthPHYRMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 50e6
     rx_clk_freq = 50e6
-    def __init__(self, clock_pads, pads, refclk_cd="eth", with_hw_init_reset=True):
-        self.submodules.crg = LiteEthPHYRMIICRG(clock_pads, pads, refclk_cd, with_hw_init_reset)
-        self.submodules.tx = ClockDomainsRenamer("eth_tx")(LiteEthPHYRMIITX(pads))
-        self.submodules.rx = ClockDomainsRenamer("eth_rx")(LiteEthPHYRMIIRX(pads))
+    def __init__(self, clock_pads, pads, refclk_cd="eth",
+        with_hw_init_reset     = True,
+        with_refclk_ddr_output = True):
+        self.crg = LiteEthPHYRMIICRG(clock_pads, pads, refclk_cd,
+            with_hw_init_reset     = with_hw_init_reset,
+            with_refclk_ddr_output = with_refclk_ddr_output,
+        )
+        self.tx = ClockDomainsRenamer("eth_tx")(LiteEthPHYRMIITX(pads))
+        self.rx = ClockDomainsRenamer("eth_rx")(LiteEthPHYRMIIRX(pads))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/s6rgmii.py` & `liteeth-2023.8/liteeth/phy/s6rgmii.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2019-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2019-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # RGMII PHY for Spartan6 Xilinx FPGA
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY RGMII TX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIITX(Module):
+class LiteEthPHYRGMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         tx_ctl_obuf  = Signal()
         tx_data_obuf = Signal(4)
 
         self.specials += [
             Instance("ODDR2",
                 p_DDR_ALIGNMENT = "C0",
                 p_SRTYPE        = "ASYNC",
                 o_Q  = tx_ctl_obuf,
-                i_C0 = ClockSignal("eth_tx"),
+                i_C0 =  ClockSignal("eth_tx"),
                 i_C1 = ~ClockSignal("eth_tx"),
                 i_CE = 1,
                 i_D0 = sink.valid,
                 i_D1 = sink.valid,
                 i_R  = ResetSignal("eth_tx"),
                 i_S  = 0
             ),
@@ -54,15 +57,15 @@
         ]
         for i in range(4):
             self.specials += [
                 Instance("ODDR2",
                     p_DDR_ALIGNMENT = "C0",
                     p_SRTYPE        = "ASYNC",
                     o_Q  = tx_data_obuf[i],
-                    i_C0 = ClockSignal("eth_tx"),
+                    i_C0 =  ClockSignal("eth_tx"),
                     i_C1 = ~ClockSignal("eth_tx"),
                     i_CE = 1,
                     i_D0 = sink.data[i],
                     i_D1 = sink.data[4+i],
                     i_R  = ResetSignal("eth_tx"),
                     i_S  = 0,
                 ),
@@ -81,22 +84,23 @@
                     i_ODATAIN = tx_data_obuf[i],
                     i_RST     = 0,
                     i_T       = 0,
                 )
             ]
         self.comb += sink.ready.eq(1)
 
+# LiteEth PHY RGMII RX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIIRX(Module):
+class LiteEthPHYRGMIIRX(LiteXModule):
     def __init__(self, pads, rx_delay=2e-9):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
-        rx_delay_taps = int(rx_delay/50e-12) # 50ps per tap
+        rx_delay_taps = int(rx_delay/50e-12) # 50ps per tap.
         assert rx_delay_taps < 256
 
         rx_ctl_ibuf    = Signal()
         rx_ctl_idelay  = Signal()
         rx_ctl         = Signal()
         rx_ctl_reg     = Signal()
         rx_data_ibuf   = Signal(4)
@@ -124,15 +128,15 @@
                 i_ODATAIN = 0,
                 i_RST     = 0,
                 i_T       = 1,
             ),
             Instance("IDDR2",
                 p_DDR_ALIGNMENT = "C0",
                 o_Q0 = rx_ctl,
-                i_C0 = ClockSignal("eth_rx"),
+                i_C0 =  ClockSignal("eth_rx"),
                 i_C1 = ~ClockSignal("eth_rx"),
                 i_CE = 1,
                 i_D  = rx_ctl_idelay,
                 i_R  = 0,
                 i_S  = 0,
             )
         ]
@@ -159,15 +163,15 @@
                     i_RST     = 0,
                     i_T       = 1,
                 ),
                 Instance("IDDR2",
                     p_DDR_ALIGNMENT = "C0",
                     o_Q0 = rx_data[i],
                     o_Q1 = rx_data[i+4],
-                    i_C0 = ClockSignal("eth_rx"),
+                    i_C0 =  ClockSignal("eth_rx"),
                     i_C1 = ~ClockSignal("eth_rx"),
                     i_CE = 1,
                     i_D  = rx_data_idelay[i],
                     i_R  = 0,
                     i_S  = 0,
                 )
             ]
@@ -176,48 +180,48 @@
         rx_ctl_reg_d = Signal()
         self.sync += rx_ctl_reg_d.eq(rx_ctl_reg)
 
         last = Signal()
         self.comb += last.eq(~rx_ctl_reg & rx_ctl_reg_d)
         self.sync += [
             source.valid.eq(rx_ctl_reg),
-            source.data.eq(Cat(rx_data_reg[:4], rx_data[4:]))
+            source.data.eq(Cat(rx_data_reg[:4], rx_data[4:])),
         ]
         self.comb += source.last.eq(last)
 
+# LiteEth PHY RGMII CRG ----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIICRG(Module, AutoCSR):
+class LiteEthPHYRGMIICRG(LiteXModule):
     def __init__(self, clock_pads, pads, with_hw_init_reset, tx_delay=2e-9):
         self._reset = CSRStorage()
 
         # # #
 
-        # RX clock
-        self.clock_domains.cd_eth_rx = ClockDomain()
-        eth_rx_clk_ibuf = Signal()
+        # RX clock.
+        self.cd_eth_rx = ClockDomain()
         self.specials += [
             Instance("BUFG",
                 i_I = clock_pads.rx,
                 o_O = self.cd_eth_rx.clk,
             ),
         ]
 
-        # TX clock
-        self.clock_domains.cd_eth_tx = ClockDomain()
+        # TX clock.
+        self.cd_eth_tx = ClockDomain()
         self.comb += self.cd_eth_tx.clk.eq(self.cd_eth_rx.clk)
-        tx_delay_taps = int(tx_delay/50e-12) # 50ps per tap
+        tx_delay_taps = int(tx_delay/50e-12) # 50ps per tap.
         assert tx_delay_taps < 256
 
         eth_tx_clk_o = Signal()
         self.specials += [
             Instance("ODDR2",
                 p_DDR_ALIGNMENT = "C0",
                 p_SRTYPE        = "ASYNC",
                 o_Q  = eth_tx_clk_o,
-                i_C0 = ClockSignal("eth_tx"),
+                i_C0 =  ClockSignal("eth_tx"),
                 i_C1 = ~ClockSignal("eth_tx"),
                 i_CE = 1,
                 i_D0 = 1,
                 i_D1 = 0,
                 i_R  = ResetSignal("eth_tx"),
                 i_S  = 0,
             ),
@@ -235,34 +239,35 @@
                 i_IOCLK1  = 0,
                 i_ODATAIN = eth_tx_clk_o,
                 i_RST     = 0,
                 i_T       = 0,
             )
         ]
 
-        # Reset
+        # Reset.
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset()
+            self.hw_reset = LiteEthPHYHWReset()
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
+# LiteEth PHY RGMII --------------------------------------------------------------------------------
 
-class LiteEthPHYRGMII(Module, AutoCSR):
+class LiteEthPHYRGMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
     def __init__(self, clock_pads, pads, with_hw_init_reset=True, tx_delay=2e-9, rx_delay=2e-9):
-        self.submodules.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay)
-        self.submodules.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
-        self.submodules.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay))
+        self.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay)
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/s7rgmii.py` & `liteeth-2023.8/liteeth/phy/s7rgmii.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # RGMII PHY for 7-Series Xilinx FPGA
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
+from litex.soc.cores.clock import S7PLL
+
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY RGMII TX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIITX(Module):
+class LiteEthPHYRGMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         tx_ctl_obuf  = Signal()
         tx_data_obuf = Signal(4)
@@ -53,16 +58,17 @@
                 Instance("OBUF",
                     i_I = tx_data_obuf[i],
                     o_O = pads.tx_data[i],
                 )
             ]
         self.comb += sink.ready.eq(1)
 
+# LiteEth PHY RGMII RX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIIRX(Module):
+class LiteEthPHYRGMIIRX(LiteXModule):
     def __init__(self, pads, rx_delay=2e-9, iodelay_clk_freq=200e6):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         assert iodelay_clk_freq in [200e6, 300e6, 400e6]
         iodelay_tap_average = 1 / (2*32 * iodelay_clk_freq)
@@ -75,16 +81,16 @@
         rx_data_ibuf   = Signal(4)
         rx_data_idelay = Signal(4)
         rx_data        = Signal(8)
 
         self.specials += [
             Instance("IBUF", i_I=pads.rx_ctl, o_O=rx_ctl_ibuf),
             Instance("IDELAYE2",
-                p_IDELAY_TYPE  = "FIXED",
-                p_IDELAY_VALUE = rx_delay_taps,
+                p_IDELAY_TYPE      = "FIXED",
+                p_IDELAY_VALUE     = rx_delay_taps,
                 p_REFCLK_FREQUENCY = iodelay_clk_freq/1e6,
                 i_C        = 0,
                 i_LD       = 0,
                 i_CE       = 0,
                 i_LDPIPEEN = 0,
                 i_INC      = 0,
                 i_IDATAIN  = rx_ctl_ibuf,
@@ -104,16 +110,16 @@
         for i in range(4):
             self.specials += [
                 Instance("IBUF",
                     i_I = pads.rx_data[i],
                     o_O = rx_data_ibuf[i],
                 ),
                 Instance("IDELAYE2",
-                    p_IDELAY_TYPE  = "FIXED",
-                    p_IDELAY_VALUE = rx_delay_taps,
+                    p_IDELAY_TYPE      = "FIXED",
+                    p_IDELAY_VALUE     = rx_delay_taps,
                     p_REFCLK_FREQUENCY = iodelay_clk_freq/1e6,
                     i_C        = 0,
                     i_LD       = 0,
                     i_CE       = 0,
                     i_LDPIPEEN = 0,
                     i_INC      = 0,
                     i_IDATAIN  = rx_data_ibuf[i],
@@ -138,44 +144,44 @@
         self.comb += last.eq(~rx_ctl & rx_ctl_d)
         self.sync += [
             source.valid.eq(rx_ctl),
             source.data.eq(rx_data)
         ]
         self.comb += source.last.eq(last)
 
+# LiteEth PHY RGMII CRG ----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIICRG(Module, AutoCSR):
+class LiteEthPHYRGMIICRG(LiteXModule):
     def __init__(self, clock_pads, pads, with_hw_init_reset, tx_delay=2e-9, hw_reset_cycles=256):
         self._reset = CSRStorage()
 
         # # #
 
-        # RX clock
-        self.clock_domains.cd_eth_rx = ClockDomain()
+        # RX clock.
+        self.cd_eth_rx = ClockDomain()
         eth_rx_clk_ibuf = Signal()
         self.specials += [
             Instance("IBUF",
                 i_I = clock_pads.rx,
                 o_O = eth_rx_clk_ibuf,
             ),
             Instance("BUFG",
                 i_I = eth_rx_clk_ibuf,
                 o_O = self.cd_eth_rx.clk,
             ),
         ]
 
-        # TX clock
-        self.clock_domains.cd_eth_tx         = ClockDomain()
-        self.clock_domains.cd_eth_tx_delayed = ClockDomain(reset_less=True)
+        # TX clock.
+        self.cd_eth_tx         = ClockDomain()
+        self.cd_eth_tx_delayed = ClockDomain(reset_less=True)
         tx_phase = 125e6*tx_delay*360
         assert tx_phase < 360
-        from litex.soc.cores.clock import S7PLL
-        self.submodules.pll = pll = S7PLL()
+        self.pll = pll = S7PLL()
         pll.register_clkin(ClockSignal("eth_rx"), 125e6)
-        pll.create_clkout(self.cd_eth_tx, 125e6, with_reset=False)
+        pll.create_clkout(self.cd_eth_tx,         125e6, with_reset=False)
         pll.create_clkout(self.cd_eth_tx_delayed, 125e6, phase=tx_phase)
 
         eth_tx_clk_obuf = Signal()
         self.specials += [
             Instance("ODDR",
                 p_DDR_CLK_EDGE = "SAME_EDGE",
                 i_C  = ClockSignal("eth_tx_delayed"),
@@ -191,32 +197,33 @@
                 o_O = clock_pads.tx,
             )
         ]
 
         # Reset
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset(cycles=hw_reset_cycles)
+            self.hw_reset = LiteEthPHYHWReset(cycles=hw_reset_cycles)
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
+# LiteEth PHY RGMII --------------------------------------------------------------------------------
 
-class LiteEthPHYRGMII(Module, AutoCSR):
+class LiteEthPHYRGMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
     def __init__(self, clock_pads, pads, with_hw_init_reset=True, tx_delay=2e-9, rx_delay=2e-9,
             iodelay_clk_freq=200e6, hw_reset_cycles=256):
-        self.submodules.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay, hw_reset_cycles)
-        self.submodules.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
-        self.submodules.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay, iodelay_clk_freq))
+        self.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay, hw_reset_cycles)
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay, iodelay_clk_freq))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/usp_1000basex.py` & `liteeth-2023.8/liteeth/phy/usp_gty_1000basex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,77 +1,51 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2019-2021 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2019-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2018 Sebastien Bourdeauducq <sb@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# Work-In-Progress...
-
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 from migen.genlib.cdc import PulseSynchronizer
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.phy.pcs_1000basex import *
 
+# USP_GTY_1000BASEX PHY ----------------------------------------------------------------------------
 
-class Open(Signal):
-    pass
-
-
-class Gearbox(Module):
-    def __init__(self):
-        self.tx_data      = Signal(10)
-        self.tx_data_half = Signal(20)
-        self.rx_data_half = Signal(20)
-        self.rx_data      = Signal(10)
-
-        # TX
-        buf = Signal(20)
-        self.sync.eth_tx += buf.eq(Cat(buf[10:], self.tx_data))
-        self.sync.eth_tx_half += self.tx_data_half.eq(buf)
-
-        # RX
-        phase_half       = Signal()
-        phase_half_rereg = Signal()
-        self.sync.eth_rx_half += phase_half_rereg.eq(phase_half)
-        self.sync.eth_rx += [
-            If(phase_half == phase_half_rereg,
-                self.rx_data.eq(self.rx_data_half[10:])
-            ).Else(
-                self.rx_data.eq(self.rx_data_half[:10])
-            ),
-              phase_half.eq(~phase_half),
-        ]
-
-
-# Configured for 200MHz transceiver reference clock
-class USP_1000BASEX(Module, AutoCSR):
+class USP_GTY_1000BASEX(LiteXModule):
+    # Configured for 200MHz or 156.25MHz transceiver reference clock
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
-    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq):
+    def __init__(self, refclk_or_clk_pads, data_pads, sys_clk_freq, refclk_freq=200e6, with_csr=True, rx_polarity=0, tx_polarity=0):
+        assert refclk_freq in [200e6, 156.25e6]
         pcs = PCS(lsb_first=True)
         self.submodules += pcs
 
         self.sink    = pcs.sink
         self.source  = pcs.source
         self.link_up = pcs.link_up
 
-        self.clock_domains.cd_eth_tx      = ClockDomain()
-        self.clock_domains.cd_eth_rx      = ClockDomain()
-        self.clock_domains.cd_eth_tx_half = ClockDomain(reset_less=True)
-        self.clock_domains.cd_eth_rx_half = ClockDomain(reset_less=True)
+        self.cd_eth_tx      = ClockDomain()
+        self.cd_eth_rx      = ClockDomain()
+        self.cd_eth_tx_half = ClockDomain(reset_less=True)
+        self.cd_eth_rx_half = ClockDomain(reset_less=True)
 
         # for specifying clock constraints. 125MHz clocks.
         self.txoutclk = Signal()
         self.rxoutclk = Signal()
 
-        self.crg_reset = CSRStorage()
+        self.reset = Signal()
+        if with_csr:
+            self.add_csr()
 
         # # #
 
         if isinstance(refclk_or_clk_pads, Signal):
             refclk = refclk_or_clk_pads
         else:
             refclk = Signal()
@@ -109,15 +83,15 @@
             p_ALIGN_PCOMMA_DET             = "TRUE",
             p_ALIGN_PCOMMA_VALUE           = 0b0101111100,
             p_A_RXOSCALRESET               = 0b0,
             p_A_RXPROGDIVRESET             = 0b0,
             p_A_RXTERMINATION              = 0b1,
             p_A_TXDIFFCTRL                 = 0b01100,
             p_A_TXPROGDIVRESET             = 0b0,
-            p_CBCC_DATA_SOURCE_SEL         = "ENCODED",
+            p_CBCC_DATA_SOURCE_SEL         = "DECODED",
             p_CDR_SWAP_MODE_EN             = 0b0,
             p_CFOK_PWRSVE_EN               = 0b1,
             p_CHAN_BOND_KEEP_ALIGN         = "FALSE",
             p_CHAN_BOND_MAX_SKEW           = 1,
             p_CHAN_BOND_SEQ_1_1            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_2            = 0b0000000000,
             p_CHAN_BOND_SEQ_1_3            = 0b0000000000,
@@ -136,41 +110,41 @@
             p_CKCAL1_CFG_2                 = 0b0010000000001000,
             p_CKCAL1_CFG_3                 = 0b0000000000000000,
             p_CKCAL2_CFG_0                 = 0b1100000011000000,
             p_CKCAL2_CFG_1                 = 0b1000000011000000,
             p_CKCAL2_CFG_2                 = 0b0001000000000000,
             p_CKCAL2_CFG_3                 = 0b0000000000000000,
             p_CKCAL2_CFG_4                 = 0b0000000000000000,
-            p_CLK_CORRECT_USE              = "TRUE",
+            p_CLK_CORRECT_USE              = "FALSE",
             p_CLK_COR_KEEP_IDLE            = "FALSE",
-            p_CLK_COR_MAX_LAT              = 15,
-            p_CLK_COR_MIN_LAT              = 12,
+            p_CLK_COR_MAX_LAT              = 20,
+            p_CLK_COR_MIN_LAT              = 18,
             p_CLK_COR_PRECEDENCE           = "TRUE",
             p_CLK_COR_REPEAT_WAIT          = 0,
-            p_CLK_COR_SEQ_1_1              = 0b0010111100,
-            p_CLK_COR_SEQ_1_2              = 0b0001010000,
-            p_CLK_COR_SEQ_1_3              = 0b0000000000,
-            p_CLK_COR_SEQ_1_4              = 0b0000000000,
+            p_CLK_COR_SEQ_1_1              = 0b0100000000,
+            p_CLK_COR_SEQ_1_2              = 0b0100000000,
+            p_CLK_COR_SEQ_1_3              = 0b0100000000,
+            p_CLK_COR_SEQ_1_4              = 0b0100000000,
             p_CLK_COR_SEQ_1_ENABLE         = 0b1111,
-            p_CLK_COR_SEQ_2_1              = 0b0010111100,
-            p_CLK_COR_SEQ_2_2              = 0b0010110101,
-            p_CLK_COR_SEQ_2_3              = 0b0000000000,
-            p_CLK_COR_SEQ_2_4              = 0b0000000000,
+            p_CLK_COR_SEQ_2_1              = 0b0100000000,
+            p_CLK_COR_SEQ_2_2              = 0b0100000000,
+            p_CLK_COR_SEQ_2_3              = 0b0100000000,
+            p_CLK_COR_SEQ_2_4              = 0b0100000000,
             p_CLK_COR_SEQ_2_ENABLE         = 0b1111,
-            p_CLK_COR_SEQ_2_USE            = "TRUE",
-            p_CLK_COR_SEQ_LEN              = 2,
+            p_CLK_COR_SEQ_2_USE            = "FALSE",
+            p_CLK_COR_SEQ_LEN              = 1,
             p_CPLL_CFG0                    = 0b0000000111111010,
             p_CPLL_CFG1                    = 0b0000000000101011,
             p_CPLL_CFG2                    = 0b0000000000000010,
             p_CPLL_CFG3                    = 0b0000000000000000,
-            p_CPLL_FBDIV                   = 5,
-            p_CPLL_FBDIV_45                = 5,
+            p_CPLL_FBDIV                   = {200e6: 5, 156.25e6: 4}[refclk_freq],
+            p_CPLL_FBDIV_45                = {200e6: 5, 156.25e6: 4}[refclk_freq],
             p_CPLL_INIT_CFG0               = 0b0000001010110010,
             p_CPLL_LOCK_CFG                = 0b0000000111101000,
-            p_CPLL_REFCLK_DIV              = 2,
+            p_CPLL_REFCLK_DIV              = {200e6: 2, 156.25e6: 1}[refclk_freq],
             p_CTLE3_OCAP_EXT_CTRL          = 0b000,
             p_CTLE3_OCAP_EXT_EN            = 0b0,
             p_DDI_CTRL                     = 0b00,
             p_DDI_REALIGN_WAIT             = 15,
             p_DEC_MCOMMA_DETECT            = "TRUE",
             p_DEC_PCOMMA_DETECT            = "TRUE",
             p_DEC_VALID_COMMA_ONLY         = "FALSE",
@@ -209,15 +183,15 @@
             p_ES_SDATA_MASK3               = 0b0000000000000000,
             p_ES_SDATA_MASK4               = 0b0000000000000000,
             p_ES_SDATA_MASK5               = 0b0000000000000000,
             p_ES_SDATA_MASK6               = 0b0000000000000000,
             p_ES_SDATA_MASK7               = 0b0000000000000000,
             p_ES_SDATA_MASK8               = 0b0000000000000000,
             p_ES_SDATA_MASK9               = 0b0000000000000000,
-            p_EYESCAN_VP_RANGE             = 0,
+            p_EYESCAN_VP_RANGE             = 0b0,
             p_EYE_SCAN_SWAP_EN             = 0b0,
             p_FTS_DESKEW_SEQ_ENABLE        = 0b1111,
             p_FTS_LANE_DESKEW_CFG          = 0b1111,
             p_FTS_LANE_DESKEW_EN           = "FALSE",
             p_GEARBOX_MODE                 = 0b00000,
             p_ISCAN_CK_PH_SEL2             = 0b0,
             p_LOCAL_MASTER                 = 0b1,
@@ -264,15 +238,15 @@
             p_PREIQ_FREQ_BST               = 0,
             p_RATE_SW_USE_DRP              = 0b1,
             p_RCLK_SIPO_DLY_ENB            = 0b0,
             p_RCLK_SIPO_INV_EN             = 0b0,
             p_RTX_BUF_CML_CTRL             = 0b011,
             p_RTX_BUF_TERM_CTRL            = 0b00,
             p_RXBUFRESET_TIME              = 0b00011,
-            p_RXBUF_ADDR_MODE              = "FULL",
+            p_RXBUF_ADDR_MODE              = "FAST",
             p_RXBUF_EIDLE_HI_CNT           = 0b1000,
             p_RXBUF_EIDLE_LO_CNT           = 0b0000,
             p_RXBUF_EN                     = "TRUE",
             p_RXBUF_RESET_ON_CB_CHANGE     = "TRUE",
             p_RXBUF_RESET_ON_COMMAALIGN    = "FALSE",
             p_RXBUF_RESET_ON_EIDLE         = "FALSE",
             p_RXBUF_RESET_ON_RATE_CHANGE   = "TRUE",
@@ -394,15 +368,15 @@
             p_RXPRBS_ERR_LOOPBACK          = 0b0,
             p_RXPRBS_LINKACQ_CNT           = 15,
             p_RXREFCLKDIV2_SEL             = 0b0,
             p_RXSLIDE_AUTO_WAIT            = 7,
             p_RXSLIDE_MODE                 = "OFF",
             p_RXSYNC_MULTILANE             = 0b0,
             p_RXSYNC_OVRD                  = 0b0,
-            p_RXSYNC_SKIP_DA               = 0b0,
+            p_RXSYNC_SKIP_DA               = 0b1,
             p_RX_AFE_CM_EN                 = 0b0,
             p_RX_BIAS_CFG0                 = 0b0001001010110000,
             p_RX_BUFFER_CFG                = 0b000000,
             p_RX_CAPFF_SARC_ENB            = 0b0,
             p_RX_CLK25_DIV                 = 8,
             p_RX_CLKMUX_EN                 = 0b1,
             p_RX_CLK_SLIP_OVRD             = 0b00000,
@@ -434,15 +408,15 @@
             p_RX_EYESCAN_VS_RANGE          = 0b10,
             p_RX_EYESCAN_VS_UT_SIGN        = 0b0,
             p_RX_FABINT_USRCLK_FLOP        = 0b0,
             p_RX_I2V_FILTER_EN             = 0b1,
             p_RX_INT_DATAWIDTH             = 0,
             p_RX_PMA_POWER_SAVE            = 0b0,
             p_RX_PMA_RSV0                  = 0b0000000000101111,
-            p_RX_PROGDIV_CFG               = 0.0,
+            p_RX_PROGDIV_CFG               = 20.0,
             p_RX_PROGDIV_RATE              = 0b0000000000000001,
             p_RX_RESLOAD_CTRL              = 0b0000,
             p_RX_RESLOAD_OVRD              = 0b0,
             p_RX_SAMPLE_PERIOD             = 0b111,
             p_RX_SIG_VALID_DLY             = 11,
             p_RX_SUM_DEGEN_AVTT_OVERITE    = 0,
             p_RX_SUM_DFETAPREP_EN          = 0b0,
@@ -460,15 +434,17 @@
             p_RX_WIDEMODE_CDR_GEN3         = 0b00,
             p_RX_WIDEMODE_CDR_GEN4         = 0b01,
             p_RX_XCLK_SEL                  = "RXDES",
             p_RX_XMODE_SEL                 = 0b1,
             p_SAMPLE_CLK_PHASE             = 0b0,
             p_SAS_12G_MODE                 = 0b0,
             p_SATA_BURST_SEQ_LEN           = 0b1111,
+            p_SATA_BURST_VAL               = 0b100,
             p_SATA_CPLL_CFG                = "VCO_3000MHZ",
+            p_SATA_EIDLE_VAL               = 0b100,
             p_SHOW_REALIGN_COMMA           = "TRUE",
             p_SIM_DEVICE                   = "ULTRASCALE_PLUS",
             p_SIM_MODE                     = "FAST",
             p_SIM_RECEIVER_DETECT_PASS     = "TRUE",
             p_SIM_RESET_SPEEDUP            = "TRUE",
             p_SIM_TX_EIDLE_DRIVE_LEVEL     = "Z",
             p_SRSTMODE                     = 0b0,
@@ -500,22 +476,23 @@
             p_TXPI_CFG0                    = 0b0000001100000000,
             p_TXPI_CFG1                    = 0b0111010101010101,
             p_TXPI_GRAY_SEL                = 0b0,
             p_TXPI_INVSTROBE_SEL           = 0b0,
             p_TXPI_PPM                     = 0b0,
             p_TXPI_PPM_CFG                 = 0b00000000,
             p_TXPI_SYNFREQ_PPM             = 0b001,
+            p_TXPMARESET_TIME              = 0b00011,
             p_TXREFCLKDIV2_SEL             = 0b0,
             p_TXSWBST_BST                  = 1,
             p_TXSWBST_EN                   = 0,
             p_TXSWBST_MAG                  = 4,
             p_TXSYNC_MULTILANE             = 0b0,
             p_TXSYNC_OVRD                  = 0b0,
             p_TXSYNC_SKIP_DA               = 0b0,
-            p_TX_CLK25_DIV                 = 8,
+            p_TX_CLK25_DIV                 = {200e6: 8, 156.25e6: 7}[refclk_freq],
             p_TX_CLKMUX_EN                 = 0b1,
             p_TX_DATA_WIDTH                = 20,
             p_TX_DCC_LOOP_RST_CFG          = 0b0000000000000100,
             p_TX_DEEMPH0                   = 0b000000,
             p_TX_DEEMPH1                   = 0b000000,
             p_TX_DEEMPH2                   = 0b000000,
             p_TX_DEEMPH3                   = 0b000000,
@@ -542,16 +519,16 @@
             p_TX_PHICAL_CFG0               = 0b0000000000100000,
             p_TX_PHICAL_CFG1               = 0b0000000001000000,
             p_TX_PI_BIASSET                = 0,
             p_TX_PMADATA_OPT               = 0b0,
             p_TX_PMA_POWER_SAVE            = 0b0,
             p_TX_PMA_RSV0                  = 0b0000000000000000,
             p_TX_PMA_RSV1                  = 0b0000000000000000,
-            p_TX_PROGCLK_SEL               = "PREPI",
-            p_TX_PROGDIV_CFG               = 0.0,
+            p_TX_PROGCLK_SEL               = "CPLL",
+            p_TX_PROGDIV_CFG               = 20.0,
             p_TX_PROGDIV_RATE              = 0b0000000000000001,
             p_TX_RXDETECT_CFG              = 0b00000000110010,
             p_TX_RXDETECT_REF              = 5,
             p_TX_SAMPLE_PERIOD             = 0b111,
             p_TX_SW_MEAS                   = 0b00,
             p_TX_VREG_CTRL                 = 0b011,
             p_TX_VREG_PDB                  = 0b1,
@@ -728,15 +705,15 @@
             i_RXPD                = 0b00,
             i_RXPHALIGN           = 0b0,
             i_RXPHALIGNEN         = 0b0,
             i_RXPHDLYPD           = 0b1,
             i_RXPHDLYRESET        = 0b0,
             i_RXPLLCLKSEL         = 0b00,
             i_RXPMARESET          = 0b0,
-            i_RXPOLARITY          = 0b0,
+            i_RXPOLARITY          = rx_polarity,
             i_RXPRBSCNTRESET      = 0b0,
             i_RXPRBSSEL           = 0b0000,
             i_RXPROGDIVRESET      = 0b0,
             i_RXRATE              = 0b000,
             i_RXRATEMODE          = 0b0,
             i_RXSLIDE             = 0b0,
             i_RXSLIPOUTCLK        = 0b0,
@@ -799,19 +776,19 @@
             i_TXPIPPMOVRDEN       = 0b0,
             i_TXPIPPMPD           = 0b0,
             i_TXPIPPMSEL          = 0b0,
             i_TXPIPPMSTEPSIZE     = 0b00000,
             i_TXPISOPD            = 0b0,
             i_TXPLLCLKSEL         = 0b00,
             i_TXPMARESET          = 0b0,
-            i_TXPOLARITY          = 0b0,
+            i_TXPOLARITY          = tx_polarity,
             i_TXPOSTCURSOR        = 0b00000,
             i_TXPRBSFORCEERR      = 0b0,
             i_TXPRBSSEL           = 0b0000,
-            i_TXPRECURSOR         =0b00000,
+            i_TXPRECURSOR         = 0b00000,
             i_TXPROGDIVRESET      = 0b0,
             i_TXRATE              = 0b000,
             i_TXRATEMODE          = 0b0,
             i_TXSEQUENCE          = 0b0000000,
             i_TXSWING             = 0b0,
             i_TXSYNCALLIN         = 0b0,
             i_TXSYNCIN            = 0b0,
@@ -965,22 +942,24 @@
                       pll_reset.eq(0)
                 ).Else(
                     reset_counter.eq(reset_counter + 1)
                 )
             )
         ]
         self.comb += [
-            tx_reset.eq(pll_reset | ~pll_locked | self.crg_reset.storage),
-            rx_reset.eq(pll_reset | ~pll_locked | pcs.restart | self.crg_reset.storage)
+            tx_reset.eq(pll_reset | ~pll_locked | self.reset),
+            rx_reset.eq(pll_reset | ~pll_locked | pcs.restart | self.reset)
         ]
 
         # Gearbox and PCS connection
-        gearbox = Gearbox()
-        self.submodules += gearbox
-
+        self.gearbox = gearbox = PCSGearbox()
         self.comb += [
             tx_data.eq(gearbox.tx_data_half),
             gearbox.rx_data_half.eq(rx_data),
 
             gearbox.tx_data.eq(pcs.tbi_tx),
-              pcs.tbi_rx.eq(gearbox.rx_data)
+            pcs.tbi_rx.eq(gearbox.rx_data)
         ]
+
+    def add_csr(self):
+        self._reset = CSRStorage()
+        self.comb += self.reset.eq(self._reset.storage)
```

### Comparing `liteeth-2023.4/liteeth/phy/usrgmii.py` & `liteeth-2023.8/liteeth/phy/usrgmii.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 #
 # This file is part of LiteEth.
 #
-# Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # RGMII PHY for Ultrascale Xilinx FPGAs
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
+from litex.gen import *
+
 from liteeth.common import *
 from liteeth.phy.common import *
 
+# LiteEth PHY RGMII TX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIITX(Module):
+class LiteEthPHYRGMIITX(LiteXModule):
     def __init__(self, pads):
         self.sink = sink = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         tx_ctl_obuf  = Signal()
         tx_data_obuf = Signal(4)
 
         self.specials += [
             Instance("ODDRE1",
                 i_C  = ClockSignal("eth_tx"),
                 i_SR = 0,
                 i_D1 = sink.valid,
                 i_D2 = sink.valid,
-                o_Q  = tx_ctl_obuf),
+                o_Q  = tx_ctl_obuf,
+            ),
             Instance("OBUF",
                 i_I = tx_ctl_obuf,
                 o_O = pads.tx_ctl,
             ),
         ]
         for i in range(4):
             self.specials += [
                 Instance("ODDRE1",
-                    i_C=ClockSignal("eth_tx"),
-                    i_SR=0,
-                    i_D1=sink.data[i],
-                    i_D2=sink.data[4 + i],
-                    o_Q=tx_data_obuf[i],
+                    i_C  = ClockSignal("eth_tx"),
+                    i_SR = 0,
+                    i_D1 = sink.data[i],
+                    i_D2 = sink.data[4 + i],
+                    o_Q  = tx_data_obuf[i],
                 ),
                 Instance("OBUF",
-                    i_I=tx_data_obuf[i],
-                    o_O=pads.tx_data[i],
+                    i_I = tx_data_obuf[i],
+                    o_O = pads.tx_data[i],
                 ),
             ]
         self.comb += sink.ready.eq(1)
 
+# LiteEth PHY RGMII RX -----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIIRX(Module):
-    def __init__(self, pads, rx_delay=2e-9):
+class LiteEthPHYRGMIIRX(LiteXModule):
+    def __init__(self, pads, rx_delay=2e-9, usp=False):
         self.source = source = stream.Endpoint(eth_phy_description(8))
 
         # # #
 
         rx_ctl_ibuf    = Signal()
         rx_ctl_idelay  = Signal()
         rx_ctl         = Signal()
         rx_data_ibuf   = Signal(4)
         rx_data_idelay = Signal(4)
         rx_data        = Signal(8)
 
         self.specials += [
             Instance("IBUF",
-                i_I=pads.rx_ctl,
-                o_O=rx_ctl_ibuf
+                i_I = pads.rx_ctl,
+                o_O = rx_ctl_ibuf,
             ),
             Instance("IDELAYE3",
                 p_DELAY_SRC        = "IDATAIN",
                 p_CASCADE          = "NONE",
                 p_DELAY_TYPE       = "FIXED",
                 p_DELAY_VALUE      = int(rx_delay*1e12),
                 p_REFCLK_FREQUENCY = 300.0,
                 p_DELAY_FORMAT     = "TIME",
                 p_UPDATE_MODE      = "ASYNC",
+                p_SIM_DEVICE       = "ULTRASCALE_PLUS" if usp else "ULTRASCALE",
                 i_CASC_IN     = 0,
                 i_CASC_RETURN = 0,
                 i_CE          = 0,
                 i_CLK         = 0,
                 i_INC         = 0,
                 i_LOAD        = 0,
                 i_CNTVALUEIN  = 0,
@@ -111,14 +117,15 @@
                     p_DELAY_SRC        = "IDATAIN",
                     p_CASCADE          = "NONE",
                     p_DELAY_TYPE       = "FIXED",
                     p_DELAY_VALUE      = int(rx_delay*1e12),
                     p_REFCLK_FREQUENCY = 300.0,
                     p_UPDATE_MODE      = "ASYNC",
                     p_DELAY_FORMAT     = "TIME",
+                    p_SIM_DEVICE       = "ULTRASCALE_PLUS" if usp else "ULTRASCALE",
                     i_CASC_IN     = 0,
                     i_CASC_RETURN = 0,
                     i_CE          = 0,
                     i_CLK         = 0,
                     i_INC         = 0,
                     i_LOAD        = 0,
                     i_CNTVALUEIN  = 0,
@@ -143,46 +150,47 @@
         rx_ctl_d = Signal()
         self.sync += rx_ctl_d.eq(rx_ctl)
 
         last = Signal()
         self.comb += last.eq(~rx_ctl & rx_ctl_d)
         self.sync += [
             source.valid.eq(rx_ctl),
-            source.data.eq(rx_data)
+            source.data.eq(rx_data),
         ]
         self.comb += source.last.eq(last)
 
+# LiteEth PHY RGMII CRG ----------------------------------------------------------------------------
 
-class LiteEthPHYRGMIICRG(Module, AutoCSR):
+class LiteEthPHYRGMIICRG(LiteXModule):
     def __init__(self, clock_pads, pads, with_hw_init_reset, tx_delay=2e-9):
         self._reset = CSRStorage()
 
         # # #
 
         # RX
-        self.clock_domains.cd_eth_rx = ClockDomain()
+        self.cd_eth_rx = ClockDomain()
         eth_rx_clk_ibuf = Signal()
         self.specials += [
             Instance("IBUF",
                 i_I = clock_pads.rx,
                 o_O = eth_rx_clk_ibuf,
             ),
             Instance("BUFG",
                i_I = eth_rx_clk_ibuf,
                o_O = self.cd_eth_rx.clk,
             )
         ]
 
         # TX
-        self.clock_domains.cd_eth_tx         = ClockDomain()
-        self.clock_domains.cd_eth_tx_delayed = ClockDomain(reset_less=True)
+        self.cd_eth_tx         = ClockDomain()
+        self.cd_eth_tx_delayed = ClockDomain(reset_less=True)
         tx_phase = 125e6*tx_delay*360
         assert tx_phase < 360
         from litex.soc.cores.clock import USPLL
-        self.submodules.pll = pll = USPLL()
+        self.pll = pll = USPLL()
         pll.register_clkin(ClockSignal("eth_rx"), 125e6)
         pll.create_clkout(self.cd_eth_tx, 125e6, with_reset=False)
         pll.create_clkout(self.cd_eth_tx_delayed, 125e6, phase=tx_phase)
 
         eth_tx_clk_obuf = Signal()
         self.specials += [
             Instance("ODDRE1",
@@ -197,31 +205,32 @@
                 o_O = clock_pads.tx,
             )
         ]
 
         # Reset
         self.reset = reset = Signal()
         if with_hw_init_reset:
-            self.submodules.hw_reset = LiteEthPHYHWReset()
+            self.hw_reset = LiteEthPHYHWReset()
             self.comb += reset.eq(self._reset.storage | self.hw_reset.reset)
         else:
             self.comb += reset.eq(self._reset.storage)
         if hasattr(pads, "rst_n"):
             self.comb += pads.rst_n.eq(~reset)
         self.specials += [
             AsyncResetSynchronizer(self.cd_eth_tx, reset),
             AsyncResetSynchronizer(self.cd_eth_rx, reset),
         ]
 
+# LiteEth PHY RGMII --------------------------------------------------------------------------------
 
-class LiteEthPHYRGMII(Module, AutoCSR):
+class LiteEthPHYRGMII(LiteXModule):
     dw          = 8
     tx_clk_freq = 125e6
     rx_clk_freq = 125e6
-    def __init__(self, clock_pads, pads, with_hw_init_reset=True, tx_delay=2e-9, rx_delay=2e-9):
-        self.submodules.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay)
-        self.submodules.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
-        self.submodules.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay))
+    def __init__(self, clock_pads, pads, with_hw_init_reset=True, tx_delay=2e-9, rx_delay=2e-9, usp=False):
+        self.crg = LiteEthPHYRGMIICRG(clock_pads, pads, with_hw_init_reset, tx_delay)
+        self.tx  = ClockDomainsRenamer("eth_tx")(LiteEthPHYRGMIITX(pads))
+        self.rx  = ClockDomainsRenamer("eth_rx")(LiteEthPHYRGMIIRX(pads, rx_delay, usp))
         self.sink, self.source = self.tx.sink, self.rx.source
 
         if hasattr(pads, "mdc"):
-            self.submodules.mdio = LiteEthPHYMDIO(pads)
+            self.mdio = LiteEthPHYMDIO(pads)
```

### Comparing `liteeth-2023.4/liteeth/phy/xgmii.py` & `liteeth-2023.8/liteeth/phy/xgmii.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 #
 # This file is part of LiteEth.
 #
 # Copyright (c) 2021 Leon Schuermann <leon@is.currently.online>
 #
 # SPDX-License-Identifier: BSD-2-Clause
 
+from functools import reduce
+from operator import or_
 
 from migen import Module
+
+from litex.gen import *
+
 from liteeth.common import *
 
-from functools import reduce
-from operator import or_
+# Constants ----------------------------------------------------------------------------------------
 
-XGMII_IDLE = Constant(0x07, bits_sign=8)
+XGMII_IDLE  = Constant(0x07, bits_sign=8)
 XGMII_START = Constant(0xFB, bits_sign=8)
-XGMII_END = Constant(0xFD, bits_sign=8)
+XGMII_END   = Constant(0xFD, bits_sign=8)
+
+# LiteEth PHY XGMII TX -----------------------------------------------------------------------------
 
 class LiteEthPHYXGMIITX(Module):
     def __init__(self, pads, dw, dic=True):
         # Enforce 64-bit data path
         assert dw == 64
 
         # Sink for data to transmit
@@ -446,14 +452,16 @@
                         NextValue(sink.ready, 0),
                     ),
                     NextState("IDLE"),
                 )
             )
         )
 
+# LiteEth PHY XGMII RX Aligner ---------------------------------------------------------------------
+
 class LiteEthPHYXGMIIRXAligner(Module):
     def __init__(self, unaligned_ctl, unaligned_data):
         # Aligned ctl and data characters
         self.aligned_ctl = Signal.like(unaligned_ctl)
         self.aligned_data = Signal.like(unaligned_data)
 
         # Buffer for low-bytes of the last XGMII bus word
@@ -496,15 +504,17 @@
                 self.aligned_ctl.eq(Cat(low_ctl, unaligned_ctl[0:4])),
                 self.aligned_data.eq(Cat(low_data, unaligned_data[0*8:4*8])),
                 NextValue(low_ctl, unaligned_ctl[4:8]),
                 NextValue(low_data, unaligned_data[4*8:8*8]),
             ),
         )
 
-class LiteEthPHYXGMIIRX(Module):
+# LiteEth PHY XGMII RX -----------------------------------------------------------------------------
+
+class LiteEthPHYXGMIIRX(LiteXModule):
     def __init__(self, pads, dw):
         # Enforce 64-bit data path
         assert dw == 64
 
         # Source we need to feed data into. We assume the sink is always ready,
         # given we can't really pause an incoming XGMII transfer.
         self.source = source = stream.Endpoint(eth_phy_description(dw))
@@ -623,14 +633,15 @@
             If(source.last,
                 NextState("IDLE"),
             ).Else(
                 NextState("RECEIVE"),
             )
         )
 
+# LiteEth PHY XGMII CRG ----------------------------------------------------------------------------
 
 class LiteEthPHYXGMIICRG(Module, AutoCSR):
     def __init__(self, clock_pads, model=False):
         self._reset = CSRStorage()
         self.clock_domains.cd_eth_rx = ClockDomain()
         self.clock_domains.cd_eth_tx = ClockDomain()
         if model:
@@ -640,26 +651,21 @@
             ]
         else:
             self.comb += [
                 self.cd_eth_rx.clk.eq(clock_pads.rx),
                 self.cd_eth_tx.clk.eq(clock_pads.tx)
             ]
 
+# LiteEth PHY XGMII --------------------------------------------------------------------------------
+
 class LiteEthPHYXGMII(Module, AutoCSR):
     dw          = 8
     tx_clk_freq = 156.25e6
     rx_clk_freq = 156.25e6
-    def __init__(self,
-                 clock_pads,
-                 pads,
-                 model=False,
-                 dw=64,
-                 with_hw_init_reset=True,
-                 dic=True,
-                 ):
+    def __init__(self, clock_pads, pads, model=False, dw=64, with_hw_init_reset=True, dic=True):
         self.dw = dw
         self.cd_eth_tx, self.cd_eth_rx = "eth_tx", "eth_rx"
         self.integrated_ifg_inserter = True
         self.submodules.crg = LiteEthPHYXGMIICRG(clock_pads, model)
         self.submodules.tx = ClockDomainsRenamer(self.cd_eth_tx)(
             LiteEthPHYXGMIITX(
                 pads,
```

### Comparing `liteeth-2023.4/liteeth/software/dissector/etherbone.lua` & `liteeth-2023.8/liteeth/software/dissector/etherbone.lua`

 * *Files identical despite different names*

### Comparing `liteeth-2023.4/liteeth.egg-info/PKG-INFO` & `liteeth-2023.8/liteeth.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteeth
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable Ethernet core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/liteeth
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
@@ -26,15 +26,15 @@
 
 ```
                                       __   _ __      ______  __
                                      / /  (_) /____ / __/ /_/ /
                                     / /__/ / __/ -_) _// __/ _ \
                                    /____/_/\__/\__/___/\__/_//_/
 
-                                 Copyright 2012-2022 / EnjoyDigital
+                                 Copyright 2012-2023 / EnjoyDigital
 
                              A small footprint and configurable Ethernet core
                                       powered by Migen & LiteX
 ```
 
 [![](https://github.com/enjoy-digital/liteeth/workflows/ci/badge.svg)](https://github.com/enjoy-digital/liteeth/actions) ![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)
 
@@ -52,22 +52,32 @@
 LiteEth can be used as LiteX library or can be integrated with your standard
 design flow by generating the verilog rtl that you will use as a standard core.
 
 [> Features
 -----------
 PHY:
   - MII, RMII 100Mbps PHYs.
-  - GMII / RGMII /1000BaseX 1Gbps PHYs.
+  - GMII / RGMII / SGMII / 1000BaseX 1Gbps PHYs.
+
+| -     | All | ECP5 | Spartan6 | Trion | Titanium | 7-Series | Ultrascale(+) |
+|-------|-----|------|----------|-------|----------|----------|---------------|
+| MII   |  X  |  X  |      X    |   X   |     X    |     X    |       X       |
+| RMII  |  X  |  X  |      X    |   X   |     X    |     X    |       X       |
+| GMII  |     |     |      X    |       |          |     X    |       X       |
+| RGMII |     |  X  |      X    |   X   |     X    |     X    |       X       |
+| SGMII |     |     |           |       |          |     X    |       X       |
+
 
 Core:
   - Configurable MAC (HW or SW interface)
-  - ARP / ICMP / UDP (HW or SW)
+  - ARP / ICMP / UDP (HW or SW) / DHCP
 
 Frontend:
   - Etherbone (Wishbone over UDP: Slave or Master support)
+  - UDP Streaming.
 
 [> FPGA Proven
 ---------------
 LiteEth is already used in commercial and open-source designs:
 - MiSoC: http://m-labs.hk/gateware.html
 - ARTIQ: http://m-labs.hk/artiq/index.html
 - HDMI2USB: http://hdmi2usb.tv/home/
```

### Comparing `liteeth-2023.4/liteeth.egg-info/SOURCES.txt` & `liteeth-2023.8/liteeth.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 liteeth.egg-info/SOURCES.txt
 liteeth.egg-info/dependency_links.txt
 liteeth.egg-info/entry_points.txt
 liteeth.egg-info/requires.txt
 liteeth.egg-info/top_level.txt
 liteeth/core/__init__.py
 liteeth/core/arp.py
+liteeth/core/dhcp.py
 liteeth/core/icmp.py
 liteeth/core/ip.py
 liteeth/core/udp.py
 liteeth/frontend/__init__.py
 liteeth/frontend/etherbone.py
 liteeth/frontend/stream.py
 liteeth/mac/__init__.py
@@ -35,27 +36,30 @@
 liteeth/mac/last_be.py
 liteeth/mac/padding.py
 liteeth/mac/preamble.py
 liteeth/mac/sram.py
 liteeth/mac/wishbone.py
 liteeth/phy/__init__.py
 liteeth/phy/a7_1000basex.py
+liteeth/phy/a7_2500basex.py
 liteeth/phy/a7_gtp.py
 liteeth/phy/common.py
 liteeth/phy/ecp5rgmii.py
 liteeth/phy/gmii.py
 liteeth/phy/gmii_mii.py
+liteeth/phy/gw5rgmii.py
 liteeth/phy/k7_1000basex.py
 liteeth/phy/ku_1000basex.py
 liteeth/phy/mii.py
 liteeth/phy/model.py
 liteeth/phy/pcs_1000basex.py
 liteeth/phy/rmii.py
 liteeth/phy/s6rgmii.py
 liteeth/phy/s7rgmii.py
 liteeth/phy/titaniumrgmii.py
 liteeth/phy/trionrgmii.py
-liteeth/phy/usp_1000basex.py
+liteeth/phy/usp_gth_1000basex.py
+liteeth/phy/usp_gty_1000basex.py
 liteeth/phy/usrgmii.py
 liteeth/phy/xgmii.py
 liteeth/software/__init__.py
 liteeth/software/dissector/etherbone.lua
```

### Comparing `liteeth-2023.4/setup.py` & `liteeth-2023.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(
     name="liteeth",
-    version="2023.04",
+    version="2023.08",
     description="Small footprint and configurable Ethernet core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/liteeth",
```

