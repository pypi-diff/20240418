# Comparing `tmp/litepcie-2023.4.tar.gz` & `tmp/litepcie-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litepcie-2023.4.tar", last modified: Thu Apr 18 20:06:37 2024, max compression
+gzip compressed data, was "litepcie-2023.8.tar", last modified: Thu Apr 18 20:06:57 2024, max compression
```

## Comparing `litepcie-2023.4.tar` & `litepcie-2023.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.497178 litepcie-2023.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1054 2024-04-18 20:06:34.000000 litepcie-2023.4/CONTRIBUTORS
--rw-r--r--   0 timkpaine   (501) staff       (20)     1683 2024-04-18 20:06:24.000000 litepcie-2023.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      103 2024-04-18 20:06:24.000000 litepcie-2023.4/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     5194 2024-04-18 20:06:37.496907 litepcie-2023.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4315 2024-04-18 20:06:34.000000 litepcie-2023.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.481389 litepcie-2023.4/doc/
--rw-r--r--   0 timkpaine   (501) staff       (20)    69329 2024-04-18 20:06:24.000000 litepcie-2023.4/doc/architecture.png
--rw-r--r--   0 timkpaine   (501) staff       (20)     4280 2024-04-18 20:06:24.000000 litepcie-2023.4/doc/enjoy_digital.png
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.482233 litepcie-2023.4/litepcie/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2588 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.484352 litepcie-2023.4/litepcie/core/
--rw-r--r--   0 timkpaine   (501) staff       (20)      132 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/core/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1428 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/core/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6864 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/core/crossbar.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3689 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/core/endpoint.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5841 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/core/msi.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.485065 litepcie-2023.4/litepcie/frontend/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/frontend/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5224 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/frontend/axi.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    43539 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/frontend/dma.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5145 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/frontend/wishbone.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    17597 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/gen.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.486129 litepcie-2023.4/litepcie/phy/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/phy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10239 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/c5pciephy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7346 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/phy/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    22563 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/s7pciephy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17552 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/uspciephy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17850 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/usppciephy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.486580 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x4/
--rw-r--r--   0 timkpaine   (501) staff       (20)   114668 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x4/pcie_us.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    66011 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x4/pcie_us_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.487082 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x8/
--rw-r--r--   0 timkpaine   (501) staff       (20)   114790 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x8/pcie_us.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    59879 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x8/pcie_us_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.487552 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x16/
--rw-r--r--   0 timkpaine   (501) staff       (20)   147208 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    58719 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.487995 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x4/
--rw-r--r--   0 timkpaine   (501) staff       (20)   146826 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    59753 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.488429 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x8/
--rw-r--r--   0 timkpaine   (501) staff       (20)   147444 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    58397 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.488881 litepcie-2023.4/litepcie/phy/xilinx_usp_hbm_gen3_x4/
--rw-r--r--   0 timkpaine   (501) staff       (20)   162422 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp.xci
--rw-r--r--   0 timkpaine   (501) staff       (20)    59753 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp_support.v
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.492062 litepcie-2023.4/litepcie/software/
--rw-r--r--   0 timkpaine   (501) staff       (20)      892 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/software/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.493662 litepcie-2023.4/litepcie/software/kernel/
--rw-r--r--   0 timkpaine   (501) staff       (20)      639 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/software/kernel/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)      137 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/software/kernel/README
--rw-r--r--   0 timkpaine   (501) staff       (20)     3208 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/config.h
--rw-r--r--   0 timkpaine   (501) staff       (20)      301 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/flags.h
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     1257 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/software/kernel/init.sh
--rw-r--r--   0 timkpaine   (501) staff       (20)     2404 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/litepcie.h
--rw-r--r--   0 timkpaine   (501) staff       (20)    11101 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/liteuart.c
--rw-r--r--   0 timkpaine   (501) staff       (20)     2107 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/litex.h
--rw-r--r--   0 timkpaine   (501) staff       (20)    34935 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/kernel/main.c
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.494247 litepcie-2023.4/litepcie/software/user/
--rw-r--r--   0 timkpaine   (501) staff       (20)      726 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/software/user/Makefile
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.495339 litepcie-2023.4/litepcie/software/user/liblitepcie/
--rw-r--r--   0 timkpaine   (501) staff       (20)      430 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/liblitepcie.h
--rw-r--r--   0 timkpaine   (501) staff       (20)     7741 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_dma.c
--rw-r--r--   0 timkpaine   (501) staff       (20)     1521 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_dma.h
--rw-r--r--   0 timkpaine   (501) staff       (20)     6333 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_flash.c
--rw-r--r--   0 timkpaine   (501) staff       (20)      941 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_flash.h
--rw-r--r--   0 timkpaine   (501) staff       (20)     1239 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_helpers.c
--rw-r--r--   0 timkpaine   (501) staff       (20)      628 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_helpers.h
--rw-r--r--   0 timkpaine   (501) staff       (20)     7997 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/litepcie_test.c
--rw-r--r--   0 timkpaine   (501) staff       (20)    16335 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/software/user/litepcie_util.c
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.496134 litepcie-2023.4/litepcie/tlp/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.4/litepcie/tlp/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5180 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/tlp/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7824 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/tlp/controller.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    15841 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/tlp/depacketizer.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    36110 2024-04-18 20:06:34.000000 litepcie-2023.4/litepcie/tlp/packetizer.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:37.496428 litepcie-2023.4/litepcie.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5194 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     2243 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       55 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:06:37.000000 litepcie-2023.4/litepcie.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:06:37.497227 litepcie-2023.4/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     1424 2024-04-18 20:06:34.000000 litepcie-2023.4/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.011000 litepcie-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1054 2024-04-18 20:06:34.000000 litepcie-2023.8/CONTRIBUTORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1683 2024-04-18 20:06:24.000000 litepcie-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      103 2024-04-18 20:06:24.000000 litepcie-2023.8/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5194 2024-04-18 20:06:57.010731 litepcie-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4315 2024-04-18 20:06:34.000000 litepcie-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.982964 litepcie-2023.8/doc/
+-rw-r--r--   0 timkpaine   (501) staff       (20)    69329 2024-04-18 20:06:24.000000 litepcie-2023.8/doc/architecture.png
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4280 2024-04-18 20:06:24.000000 litepcie-2023.8/doc/enjoy_digital.png
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.983926 litepcie-2023.8/litepcie/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3950 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.986482 litepcie-2023.8/litepcie/core/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      132 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/core/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1428 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/core/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6864 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/core/crossbar.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4877 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/core/endpoint.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5879 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/core/msi.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.987769 litepcie-2023.8/litepcie/frontend/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/frontend/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5224 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/frontend/axi.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    44153 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/frontend/dma.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5145 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/frontend/wishbone.py
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)    17101 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/gen.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.991344 litepcie-2023.8/litepcie/phy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/phy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10296 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/c5pciephy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7346 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/phy/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    24075 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/s7pciephy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    17626 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/uspciephy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    17923 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/usppciephy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.992414 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x4/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   114668 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x4/pcie_us.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    66064 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x4/pcie_us_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.993707 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   114790 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x8/pcie_us.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    59932 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x8/pcie_us_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.997505 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x16/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   147208 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    58772 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:56.999544 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x4/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   146826 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    59806 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.001047 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   147444 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    58450 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.002024 litepcie-2023.8/litepcie/phy/xilinx_usp_hbm_gen3_x4/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   162422 2024-04-18 20:06:34.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp.xci
+-rw-r--r--   0 timkpaine   (501) staff       (20)    59806 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp_support.v
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.002229 litepcie-2023.8/litepcie/software/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      892 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/software/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.006539 litepcie-2023.8/litepcie/software/kernel/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      639 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/software/kernel/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)      137 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/software/kernel/README
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3343 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/config.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)      436 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/flags.h
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     1257 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/software/kernel/init.sh
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2404 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/litepcie.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11223 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/liteuart.c
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2104 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/litex.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)    35273 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/kernel/main.c
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.007425 litepcie-2023.8/litepcie/software/user/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      726 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/software/user/Makefile
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.008757 litepcie-2023.8/litepcie/software/user/liblitepcie/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      433 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/liblitepcie.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7744 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_dma.c
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1524 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_dma.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6336 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_flash.c
+-rw-r--r--   0 timkpaine   (501) staff       (20)      944 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_flash.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1242 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_helpers.c
+-rw-r--r--   0 timkpaine   (501) staff       (20)      631 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_helpers.h
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7999 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/litepcie_test.c
+-rw-r--r--   0 timkpaine   (501) staff       (20)    16338 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/software/user/litepcie_util.c
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.009900 litepcie-2023.8/litepcie/tlp/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:24.000000 litepcie-2023.8/litepcie/tlp/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    13103 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/tlp/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7810 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/tlp/controller.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    19948 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/tlp/depacketizer.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    39649 2024-04-18 20:06:50.000000 litepcie-2023.8/litepcie/tlp/packetizer.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:06:57.010206 litepcie-2023.8/litepcie.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5194 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2243 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       51 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       55 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        9 2024-04-18 20:06:56.000000 litepcie-2023.8/litepcie.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:06:57.011056 litepcie-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     1424 2024-04-18 20:06:55.000000 litepcie-2023.8/setup.py
```

### Comparing `litepcie-2023.4/CONTRIBUTORS` & `litepcie-2023.8/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/LICENSE` & `litepcie-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/PKG-INFO` & `litepcie-2023.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litepcie
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable PCIe core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litepcie
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `litepcie-2023.4/README.md` & `litepcie-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/doc/architecture.png` & `litepcie-2023.8/doc/architecture.png`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/doc/enjoy_digital.png` & `litepcie-2023.8/doc/enjoy_digital.png`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/common.py` & `litepcie-2023.8/litepcie/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,14 +34,34 @@
 def phy_layout(data_width):
     layout = [
         ("dat", data_width),
         ("be",  data_width//8)
     ]
     return EndpointDescription(layout)
 
+def configuration_layout(data_width, address_width=32):
+    layout = [
+        # Request Parameters.
+        ("req_id",          16), # Requester ID.
+        ("we",               1), # Configuration type; 0 : Read / 1 : Write.
+        ("bus_number",       8), # Configuration Bus number.
+        ("device_no",        5), # Configuration Device number.
+        ("func",             3), # Configuration Function number.
+        ("ext_reg",          3), # Configuration Extended Register.
+        ("register_no",      6), # Configuration Register number.
+        ("tag",              8), # Configuration tag.
+
+        # Data Stream.
+        ("dat", data_width),
+
+        # Internal LitePCIe Routing/Identification.
+        ("channel", 8), # Crossbar's channel (Used for internal routing).
+    ]
+    return EndpointDescription(layout)
+
 def request_layout(data_width, address_width=32):
     layout = [
         # Request Parameters.
         ("req_id",          16), # Requester ID.
         ("we",               1), # Request type; 0 : Read / 1 : Write.
         ("adr",  address_width), # Request address (In Bytes).
         ("len",             10), # Request length (In Dwords).
@@ -72,13 +92,31 @@
 
         # Internal LitePCIe Routing/Identification.
         ("channel", 8), # Crossbar's channel (Used for internal routing).
         ("user_id", 8)  # Packet identification (Used for packet delimitation).
     ]
     return EndpointDescription(layout)
 
+def ptm_layout(data_width):
+    layout = [
+        ("request",       1), # Request.
+        ("response",      1), # Response.
+        ("requester_id", 16), # Requester ID.
+        ("length",       10), # Length.
+        ("message_code",  8), # Message Code.
+        ("master_time",  64), # Master Time.
+
+        # Data Stream.
+        ("dat", data_width),
+
+        # Internal LitePCIe Routing/Identification.
+        ("channel", 8), # Crossbar's channel (Used for internal routing).
+    ]
+    return EndpointDescription(layout)
+
+
 def msi_layout():
     return [("dat", 8)]
 
 def dma_layout(data_width):
     layout = [("data", data_width)]
     return EndpointDescription(layout)
```

### Comparing `litepcie-2023.4/litepcie/core/common.py` & `litepcie-2023.8/litepcie/core/common.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/core/crossbar.py` & `litepcie-2023.8/litepcie/core/crossbar.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/core/msi.py` & `litepcie-2023.8/litepcie/core/msi.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
                     If(msix_ready,
                         clear.eq(1 << i)
                     )
                 )
             ]
 
         # Send MSI-X as TLP-Write ------------------------------------------------------------------
-        port     = endpoint.crossbar.get_master_port()
-        table_port = self.table.get_port(has_re=True)
+        self.port       = port       = endpoint.crossbar.get_master_port()
+        self.table_port = table_port = self.table.get_port(has_re=True)
         self.specials += table_port
 
         self.submodules.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             table_port.adr.eq(msix_num),
             table_port.re.eq(1),
             If(msix_valid,
```

### Comparing `litepcie-2023.4/litepcie/frontend/axi.py` & `litepcie-2023.8/litepcie/frontend/axi.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/frontend/dma.py` & `litepcie-2023.8/litepcie/frontend/dma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #
 # This file is part of LitePCIe.
 #
-# Copyright (c) 2015-2022 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2020 Antmicro <www.antmicro.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
+from litex.gen import *
+
 from litex.soc.interconnect import stream
 from litex.soc.interconnect.csr import *
 
 from litepcie.common import *
 from litepcie.tlp.common import *
 
 # Constants/Layouts --------------------------------------------------------------------------------
@@ -20,15 +22,15 @@
     if with_user_id:
         layout += [("user_id", 8)]
     return EndpointDescription(layout)
 
 
 # LitePCIeDMAScatterGather --------------------------------------------------------------------------
 
-class LitePCIeDMAScatterGather(Module, AutoCSR):
+class LitePCIeDMAScatterGather(LiteXModule):
     """LitePCIe DMA Scatter-Gather
 
     Software programmable table storing a list of DMA descriptors.
 
                                Mode
                                 │
                               ┌─▼─┐  ┌───────────────────┐
@@ -163,15 +165,15 @@
                     )
                 )
             )
         ]
 
 # LitePCIeDMADescriptorSplitter --------------------------------------------------------------------
 
-class LitePCIeDMADescriptorSplitter(Module, AutoCSR):
+class LitePCIeDMADescriptorSplitter(LiteXModule):
     """LitePCIe DMA Descriptor Splitter
 
     Splits descriptors from LitePCIeDMAScatterGather in shorter descriptors of:
     - Maximum Payload Size for Writes.
     - Maximum Request Size for Reads.
 
     Descriptors from LitePCIeDMAScatterGather have a maximum length of 16Mb (24-bits). It is not
@@ -190,15 +192,15 @@
         # # #
 
         desc_length  = Signal(32)
         desc_offset  = Signal(32)
         desc_id      = Signal(32)
 
         # FSM --------------------------------------------------------------------------------------
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             # Set Descriptor Offset/Length.
             NextValue(desc_offset, 0),
             NextValue(desc_length, sink.length),
             # Wait for a Descriptor and go to Run.
             If(sink.valid,
                 NextState("SPLIT")
@@ -240,32 +242,33 @@
                     NextState("IDLE")
                 )
             )
         )
 
 # LitePCIeDMAReader --------------------------------------------------------------------------------
 
-class LitePCIeDMAReader(Module, AutoCSR):
+class LitePCIeDMAReader(LiteXModule):
     """LitePCIe DMA Reader
 
     Generates a data stream from Host's memory.
 
     This module allows Scatter-Gather DMAs from Host's memory to data stream in the FPGA. The DMA
     descriptors, stored in a software programmable table, are split and executed as Read Requests
     on the PCIe bus.
 
     A Read Request is only sent to the Host when enough space is available in the Data FIFO to store
     the requested data.
 
     A MSI IRQ can be generated when a descriptor has been executed.
     """
-    def __init__(self, endpoint, port, with_table=True, table_depth=256, address_width=32, with_splitter_buffer=True):
-        self.port = port
+    def __init__(self, endpoint, port, with_table=True, table_depth=256, address_width=32, data_width=None, with_splitter_buffer=True):
+        self.port       = port
+        self.data_width = data_width or endpoint.phy.data_width
         # Stream Endpoint.
-        self.source = stream.Endpoint(dma_layout(endpoint.phy.data_width))
+        self.source = stream.Endpoint(dma_layout(self.data_width))
 
         # Control.
         self._enable = CSRStorage(size=2, description="DMA Reader Control. Write ``1`` to enable DMA Reader.", reset=0 if with_table else 1)
 
         # IRQ.
         self.irq = Signal()
 
@@ -276,46 +279,51 @@
 
         length_shift          = log2_int(endpoint.phy.data_width//8)
         max_words_per_request = max_request_size//(endpoint.phy.data_width//8)
         max_pending_words     = endpoint.max_pending_requests*max_words_per_request
 
         # Table ------------------------------------------------------------------------------------
         if with_table:
-            self.submodules.table = LitePCIeDMAScatterGather(table_depth, address_width=address_width)
+            self.table = LitePCIeDMAScatterGather(table_depth, address_width=address_width)
         else:
             self.desc_sink = stream.Endpoint(descriptor_layout(address_width=address_width)) # Expose a Descriptor sink.
 
         # Splitter ---------------------------------------------------------------------------------
         # DMA descriptors need to be splitted in descriptors of max_request_size (negotiated at link-up)
         splitter = LitePCIeDMADescriptorSplitter(
             max_size      = endpoint.phy.max_request_size,
             address_width = address_width
         )
         splitter = ResetInserter()(splitter)
         if with_splitter_buffer: # For timings.
             splitter = BufferizeEndpoints({"source": DIR_SOURCE})(splitter)
-        self.submodules.splitter = splitter
+        self.splitter = splitter
         if with_table:
             self.comb += self.table.source.connect(splitter.sink)
         else:
             self.comb += self.desc_sink.connect(splitter.sink)
 
         # User ID ----------------------------------------------------------------------------------
         last_user_id = Signal(8, reset=255)
         self.sync += If(port.sink.valid & port.sink.first & port.sink.ready,
             last_user_id.eq(port.sink.user_id)
         )
 
+        # Data Converter ---------------------------------------------------------------------------
+
+        self.data_conv = stream.Converter(endpoint.phy.data_width, self.data_width)
+        self.comb += self.data_conv.source.connect(self.source)
+
         # Data FIFO --------------------------------------------------------------------------------
         data_fifo_depth = 4*max_pending_words
         data_fifo = SyncFIFO(dma_layout(endpoint.phy.data_width), data_fifo_depth, buffered=True)
-        self.submodules.data_fifo = ResetInserter()(data_fifo)
+        self.data_fifo = ResetInserter()(data_fifo)
         self.comb += [
-            # Connect Data FIFO to Source.
-            data_fifo.source.connect(self.source),
+            # Connect Data FIFO to Data Converter.
+            data_fifo.source.connect(self.data_conv.sink),
             # When Enabled, connect Sink to Data FIFO.
             If(enable,
                 port.sink.connect(data_fifo.sink, keep={"valid", "ready"}),
                 data_fifo.sink.data.eq(port.sink.dat),
                 data_fifo.sink.first.eq(port.sink.first & (port.sink.user_id != last_user_id)),
             # Else accept incoming Port Data.
             ).Else(
@@ -338,15 +346,15 @@
             ),
         ]
         # Update Pending words.
         self.sync += pending_words.eq(pending_words + pending_words_queue - pending_words_dequeue)
         self.sync += If(~enable, pending_words.eq(0))
 
         # FSM --------------------------------------------------------------------------------------
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             # Reset Splitter/FIFO when disabled.
             If(~enable,
                 splitter.reset.eq(1),
                 data_fifo.reset.eq(1),
             # Else wait for a Descriptor and to have enough Space to generate the Request.
             ).Elif(splitter.source.valid & (pending_words < (data_fifo_depth - max_words_per_request)),
@@ -382,32 +390,33 @@
         # IRQ --------------------------------------------------------------------------------------
         self.comb += If(splitter.source.valid & splitter.source.ready & splitter.source.last,
             self.irq.eq(~splitter.source.irq_disable)
         )
 
 # LitePCIeDMAWriter --------------------------------------------------------------------------------
 
-class LitePCIeDMAWriter(Module, AutoCSR):
+class LitePCIeDMAWriter(LiteXModule):
     """LitePCIe DMA Writer
 
     Stores a data stream to Host's memory.
 
     This module allows Scatter-Gather DMAs from a data stream in the FPGA to Host's memory. The DMA
     descriptors, stored in a software programmable table, are split and executed as Write Requests
     on the PCIe bus.
 
     A Write Request is only sent to the Host when enough data are available for the current split
     descriptor.
 
     A MSI IRQ can be generated when a descriptor has been executed.
     """
-    def __init__(self, endpoint, port, with_table=True, table_depth=256, address_width=32, with_splitter_buffer=True):
-        self.port = port
+    def __init__(self, endpoint, port, with_table=True, table_depth=256, address_width=32, data_width=None, with_splitter_buffer=True):
+        self.port       = port
+        self.data_width = data_width or endpoint.phy.data_width
         # Stream Endpoint.
-        self.sink = sink = stream.Endpoint(dma_layout(endpoint.phy.data_width))
+        self.sink = stream.Endpoint(dma_layout(self.data_width))
 
         # Control.
         self._enable = CSRStorage(size=2, description="DMA Writer Control. Write ``1`` to enable DMA Writer.", reset=0 if with_table else 1)
 
         # IRQ.
         self.irq = Signal()
 
@@ -417,46 +426,51 @@
         self.enable = enable = self._enable.storage[0]
 
         length_shift          = log2_int(endpoint.phy.data_width//8)
         max_words_per_request = max_payload_size//(endpoint.phy.data_width//8)
 
         # Table ------------------------------------------------------------------------------------
         if with_table:
-            self.submodules.table = LitePCIeDMAScatterGather(table_depth, address_width)
+            self.table = LitePCIeDMAScatterGather(table_depth, address_width)
         else:
             self.desc_sink = stream.Endpoint(descriptor_layout(address_width=address_width)) # Expose a Descriptor sink.
 
         # Splitter ---------------------------------------------------------------------------------
         # DMA descriptors need to be splitted in descriptors of max_request_size (negotiated at link-up)
         splitter = LitePCIeDMADescriptorSplitter(
             max_size      = endpoint.phy.max_payload_size,
             address_width = address_width
         )
         splitter = ResetInserter()(splitter)
         if with_splitter_buffer: # For timings.
             # FIXME: Prevent early termination, so don't use when early termination is required.
             splitter = BufferizeEndpoints({"source": DIR_SOURCE})(splitter)
-        self.submodules.splitter = splitter
+        self.splitter = splitter
         if with_table:
             self.comb += self.table.source.connect(splitter.sink)
         else:
             self.comb += self.desc_sink.connect(splitter.sink)
 
+        # Data Converter ---------------------------------------------------------------------------
+
+        self.data_conv = stream.Converter(self.data_width, endpoint.phy.data_width)
+        self.comb += self.sink.connect(self.data_conv.sink)
+
         # Data FIFO --------------------------------------------------------------------------------
         data_fifo_depth = 4*max_words_per_request
         data_fifo = stream.SyncFIFO([("data", endpoint.phy.data_width)], data_fifo_depth, buffered=True)
-        self.submodules.data_fifo = ResetInserter()(data_fifo)
+        self.data_fifo = ResetInserter()(data_fifo)
         # By default, accept incoming stream when disabled.
-        self.comb += sink.ready.eq(1)
-        # When Enabled, connect Sink to Data FIFO.
-        self.comb += If(enable, sink.connect(data_fifo.sink))
+        self.comb += self.data_conv.source.ready.eq(1)
+        # When Enabled, connect Data Converter to Data FIFO.
+        self.comb += If(enable, self.data_conv.source.connect(data_fifo.sink))
 
         # FSM --------------------------------------------------------------------------------------
         req_count = Signal.like(splitter.source.length)
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             # Reset Request Count.
             NextValue(req_count, 0),
             # Reset Splitter/FIFO when disabled.
             If(~enable,
                 splitter.reset.eq(1),
                 data_fifo.reset.eq(1),
@@ -507,15 +521,15 @@
         # IRQ --------------------------------------------------------------------------------------
         self.comb += If(splitter.source.valid & splitter.source.ready & splitter.source.last,
             self.irq.eq(~splitter.source.irq_disable)
         )
 
 # LitePCIeDMALoopback ------------------------------------------------------------------------------
 
-class LitePCIeDMALoopback(Module, AutoCSR):
+class LitePCIeDMALoopback(LiteXModule):
     """LitePCIe DMA Loopback
 
     Optional DMA Reader to DMA Writer loopback.
 
     For software development or system bring-up/check, being able to do a DMA loopback in the FPGA
     is very useful. This module allows doing a DMA Reader to DMA Writer loopback that can be enabled
     by a CSR. When enabled, user data stream from the DMA Reader is no longer generated, the same
@@ -540,15 +554,15 @@
                 self.sink.connect(self.next_source),
                 self.next_sink.connect(self.source)
             )
         ]
 
 # LitePCIeDMASynchronizer --------------------------------------------------------------------------
 
-class LitePCIeDMASynchronizer(Module, AutoCSR):
+class LitePCIeDMASynchronizer(LiteXModule):
     """LitePCIe DMA Synchronizer
 
     Optional DMA synchronization.
 
     For some applications (Software Defined Radio, Video, ...), DMA start needs to be precisely
     synchronized to an internal signal of the FPGA (PPS for example for an SDR applications). This
     module allows releasing precisely one or both of the DMA Writer/Reader data streams.
@@ -608,15 +622,15 @@
                 self.source.valid.eq(0),
                 self.next_sink.ready.eq(1),
             )
         ]
 
 # LitePCIeDMABuffering -----------------------------------------------------------------------------
 
-class LitePCIeDMABuffering(Module, AutoCSR):
+class LitePCIeDMABuffering(LiteXModule):
     """LitePCIe DMA Buffering
 
     Optional DMA buffering with dynamically configurable depth.
 
     For some applications (Software Defined Radio, Video, ...), the user module consuming the data
     from the DMA Reader works at fixed rate and does not handle backpressure. (The same also applies
     to the user module generating the data to the DMA Writer). Since the PCIe bus is shared, gaps
@@ -728,15 +742,15 @@
                 ).Else(
                     self.writer_fifo_status.fields.level[depth_shift:].eq(writer_fifo_level_max)
                 )
             ]
 
 # LitePCIeDMAStatus --------------------------------------------------------------------------------
 
-class LitePCIeDMAStatus(Module, AutoCSR):
+class LitePCIeDMAStatus(LiteXModule):
     """LitePCIe DMA Status
 
     Optional DMA Status writer to Host Memory.
 
     LitePCIeDMAStatus writes 16 x 32-bit words to the Host memory. The first 8 words are reserved for
     the internal DMA status and the last 8 words for optional external status. The mapping as follows:
 
@@ -800,15 +814,15 @@
         # Update Logic.
         # -------------
         port   = endpoint.crossbar.get_master_port(write_only=True)
         dwords = len(port.source.dat)//32
         offset = Signal(4)
         assert len(status)%dwords == 0
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             If(self.control.fields.enable,
                 If(update,
                     NextValue(offset, 0),
                     NextState("WORDS-WRITE")
                 )
             )
@@ -845,24 +859,24 @@
             If(port.source.ready,
                 NextState("WORDS-UPDATE")
             )
         )
 
 # LitePCIeDMA --------------------------------------------------------------------------------------
 
-class LitePCIeDMA(Module, AutoCSR):
+class LitePCIeDMA(LiteXModule):
     """LitePCIe DMA
 
     Scatter-Gather bi-directional DMA:
     - Generates a data stream from Host's memory.
     - Stores a data stream to Host's memory.
 
     Optional buffering, loopback, synchronization and monitoring.
     """
-    def __init__(self, phy, endpoint, table_depth=256, address_width=32, with_writer=True, with_reader=True,
+    def __init__(self, phy, endpoint, table_depth=256, address_width=32, data_width=None, with_writer=True, with_reader=True,
         # Loopback.
         with_loopback     = False,
         # Synchronizer.
         with_synchronizer = False,
         # Buffering.
         with_buffering    = False, buffering_depth=256*8, writer_buffering_depth=None, reader_buffering_depth=None,
         # Monitor.
@@ -870,85 +884,85 @@
         # Status.
         with_status       = False,
         # Splitter Buffer.
         with_writer_splitter_buffer = True,
         with_reader_splitter_buffer = True,
     ):
         # Parameters -------------------------------------------------------------------------------
-        self.data_width = data_width = phy.data_width
+        self.data_width = data_width or phy.data_width
 
         # Endoints ---------------------------------------------------------------------------------
-        self.sink   = stream.Endpoint(dma_layout(data_width))
-        self.source = stream.Endpoint(dma_layout(data_width))
+        self.sink   = stream.Endpoint(dma_layout(self.data_width))
+        self.source = stream.Endpoint(dma_layout(self.data_width))
 
         # Writer/Reader ----------------------------------------------------------------------------
         if with_writer:
-            writer = LitePCIeDMAWriter(
+            self.writer = LitePCIeDMAWriter(
                 endpoint             = endpoint,
                 port                 = endpoint.crossbar.get_master_port(write_only=True),
                 table_depth          = table_depth,
                 address_width        = address_width,
+                data_width           = self.data_width,
                 with_splitter_buffer = with_writer_splitter_buffer,
             )
-            self.submodules.writer = writer
             self.comb += self.sink.connect(self.writer.sink)
 
         if with_reader:
-            reader = LitePCIeDMAReader(
+            self.reader = LitePCIeDMAReader(
                 endpoint             = endpoint,
                 port                 = endpoint.crossbar.get_master_port(read_only=True),
                 table_depth          = table_depth,
                 address_width        = address_width,
+                data_width           = self.data_width,
                 with_splitter_buffer = with_reader_splitter_buffer,
             )
-            self.submodules.reader = reader
-            self.comb += reader.source.connect(self.source)
+            self.comb += self.reader.source.connect(self.source)
 
         # Loopback ---------------------------------------------------------------------------------
         if with_loopback:
             if not (with_writer and with_reader):
                 raise ValueError("Loopback capability requires DMAWriter and DMAReader to be enabled.")
-            self.submodules.loopback = LitePCIeDMALoopback(data_width)
+            self.loopback = LitePCIeDMALoopback(self.data_width)
             self.add_plugin_module(self.loopback)
 
         # Synchronizer -----------------------------------------------------------------------------
         if with_synchronizer:
             if not (with_writer and with_reader):
                 raise ValueError("Synchronizer capability requires DMAWriter and DMAReader to be enabled.")
-            self.submodules.synchronizer = LitePCIeDMASynchronizer(data_width)
+            self.synchronizer = LitePCIeDMASynchronizer(self.data_width)
             self.add_plugin_module(self.synchronizer)
 
         # Buffering --------------------------------------------------------------------------------
         if with_buffering:
             writer_depth = writer_buffering_depth if writer_buffering_depth is not None else buffering_depth
             reader_depth = reader_buffering_depth if reader_buffering_depth is not None else buffering_depth
-            self.submodules.buffering = LitePCIeDMABuffering(
-                data_width   = data_width,
+            self.buffering = LitePCIeDMABuffering(
+                data_width   = self.data_width,
                 with_reader  = with_reader,
                 with_writer  = with_writer,
                 reader_depth = reader_depth,
                 writer_depth = writer_depth,
             )
             self.add_plugin_module(self.buffering)
 
         # Monitor ----------------------------------------------------------------------------------
         if with_monitor:
             if with_writer:
-                self.submodules.writer_monitor = stream.Monitor(self.sink,   count_width=16, with_overflows  = True)
+                self.writer_monitor = stream.Monitor(self.sink,   count_width=16, with_overflows  = True)
             if with_reader:
-                self.submodules.reader_monitor = stream.Monitor(self.source, count_width=16, with_underflows = True)
+                self.reader_monitor = stream.Monitor(self.source, count_width=16, with_underflows = True)
 
         # Status -----------------------------------------------------------------------------------
         if with_status:
             if not (with_writer and with_reader):
                 raise ValueError("Status capability requires DMAWriter and DMAReader to be enabled.")
-            self.submodules.status = LitePCIeDMAStatus(
+            self.status = LitePCIeDMAStatus(
                 endpoint      = endpoint,
-                writer        = writer,
-                reader        = reader,
+                writer        = self.writer,
+                reader        = self.reader,
                 address_width = address_width,
             )
 
     def add_plugin_module(self, m):
         self.comb += [
             self.source.connect(m.sink),
             m.source.connect(self.sink)
```

### Comparing `litepcie-2023.4/litepcie/frontend/wishbone.py` & `litepcie-2023.8/litepcie/frontend/wishbone.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/gen.py` & `litepcie-2023.8/litepcie/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 import yaml
 import argparse
 import subprocess
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
-from migen.genlib.misc import WaitTimer
 
 from litex.gen import *
 
 from litex.soc.cores.clock import *
 from litex.soc.interconnect.csr import *
 from litex.soc.interconnect import wishbone
 from litex.soc.interconnect.axi import *
@@ -312,21 +311,15 @@
             self.comb += self.pcie_msi.irqs[32:32+core_config["msi_irqs"]].eq(platform.request("msi_irqs"))
         else:
             assert core_config["msi_irqs"] <= 16
             if core_config.get("msi_multivector", False):
                 self.pcie_msi = LitePCIeMSIMultiVector(width=32)
             else:
                 self.pcie_msi = LitePCIeMSI(width=32)
-            # On Ultrascale/Ultrascale+ limit rate of IRQs to 1MHz (to prevent issue with IRQs stalled).
-            if isinstance(self.pcie_phy, (USPCIEPHY, USPPCIEPHY)):
-                self.pcie_msi_timer = WaitTimer(int(sys_clk_freq/1e6))
-                self.comb += self.pcie_msi_timer.wait.eq(~self.pcie_msi_timer.done)
-                self.comb += If(self.pcie_msi_timer.done, self.pcie_msi.source.connect(self.pcie_phy.msi))
-            else:
-                self.comb += self.pcie_msi.source.connect(self.pcie_phy.msi)
+            self.comb += self.pcie_msi.source.connect(self.pcie_phy.msi)
             self.comb += self.pcie_msi.irqs[16:16+core_config["msi_irqs"]].eq(platform.request("msi_irqs"))
         self.interrupts = {}
         for i in range(core_config["dma_channels"]):
             pcie_dma = getattr(self, f"pcie_dma{i}")
             if hasattr(pcie_dma, "writer"):
                 self.interrupts[f"pcie_dma{i}_writer"] = pcie_dma.writer.irq
             if hasattr(pcie_dma, "reader"):
```

### Comparing `litepcie-2023.4/litepcie/phy/c5pciephy.py` & `litepcie-2023.8/litepcie/phy/c5pciephy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 from litepcie.common import *
 
 # --------------------------------------------------------------------------------------------------
 
 class C5PCIEPHY(LiteXModule):
     endianness    = "little"
     qword_aligned = True
-    def __init__(self, platform, pads, data_width=64, bar0_size=1*MB, cd="sys"):
+    def __init__(self, platform, pads, data_width=64, cd="sys",
+        # PCIe hardblock parameters.
+        bar0_size = 0x100000,
+    ):
         # Streams ---------------------------------------------------------------------------------
         self.sink   = stream.Endpoint(phy_layout(data_width))
         self.source = stream.Endpoint(phy_layout(data_width))
         self.msi    = stream.Endpoint(msi_layout())
 
         # Parameters/Locals ------------------------------------------------------------------------
         self.pads             = pads
```

### Comparing `litepcie-2023.4/litepcie/phy/common.py` & `litepcie-2023.8/litepcie/phy/common.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/s7pciephy.py` & `litepcie-2023.8/litepcie/phy/s7pciephy.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 from litepcie.phy.common import *
 
 # S7PCIEPHY ----------------------------------------------------------------------------------------
 
 class S7PCIEPHY(LiteXModule):
     endianness    = "big"
     qword_aligned = False
-    def __init__(self, platform, pads, data_width=64, bar0_size=1*MB, cd="sys", pcie_data_width=None):
+    def __init__(self, platform, pads, data_width=64,  cd="sys",
+        # PCIe hardblock parameters.
+        pcie_data_width = None,
+        bar0_size       = 0x100000,
+        msi_type        = "msi",
+        with_ptm        = False,
+    ):
         # Streams ----------------------------------------------------------------------------------
         self.sink   = stream.Endpoint(phy_layout(data_width))
         self.source = stream.Endpoint(phy_layout(data_width))
         self.msi    = stream.Endpoint(msi_layout())
 
         # Registers --------------------------------------------------------------------------------
         self._link_status = CSRStatus(fields=[
@@ -53,14 +59,16 @@
         self._max_payload_size  = CSRStatus(16, description="Negiotiated Max Payload Size (in bytes).")
 
         # Parameters/Locals ------------------------------------------------------------------------
         if pcie_data_width is None: pcie_data_width = data_width
         self.platform         = platform
         self.data_width       = data_width
         self.pcie_data_width  = pcie_data_width
+        self.msi_type         = msi_type
+        self.with_ptm         = with_ptm
 
         self.id               = Signal(16, reset_less=True)
         self.bar0_size        = bar0_size
         self.bar0_mask        = get_bar_mask(bar0_size)
         self.max_request_size = Signal(16, reset_less=True)
         self.max_payload_size = Signal(16, reset_less=True)
 
@@ -430,43 +438,76 @@
         self.ltssm_tracer = LTSSMTracer(self._link_status.fields.ltssm)
 
     # Hard IP sources ------------------------------------------------------------------------------
     def add_sources(self, platform, phy_path, phy_filename=None):
         if phy_filename is not None:
             platform.add_ip(os.path.join(phy_path, phy_filename))
         else:
+            # Global parameters.
             config = {
                 "Bar0_Scale"         : "Megabytes",
                 "Bar0_Size"          : 1,
                 "Buf_Opt_BMA"        : True,
                 "Component_Name"     : "pcie",
                 "Device_ID"          : 7020 + self.nlanes,
-                "IntX_Generation"    : False,
                 "Interface_Width"    : f"{self.pcie_data_width}_bit",
-                "Legacy_Interrupt"   : None,
-                "Multiple_Message_Capable"  : '1_vector',
                 "Link_Speed"         : "5.0_GT/s",
-                "MSI_64b"            : False,
                 "Max_Payload_Size"   : "512_bytes" if self.nlanes != 8 else "256_bytes",
                 "Maximum_Link_Width" : f"X{self.nlanes}",
                 "PCIe_Blk_Locn"      : "X0Y0",
                 "Ref_Clk_Freq"       : "100_MHz",
                 "Trans_Buf_Pipeline" : None,
                 "Trgt_Link_Speed"    : "4'h2",
                 "User_Clk_Freq"      : 125 if self.nlanes != 8 else 250,
             }
+
+            # Interrupts parameters.
+            assert self.msi_type in ["msi", "msi-multi-vector", "msi-x"]
+            config.update({
+                    "Legacy_Interrupt" : None,
+                    "IntX_Generation"  : False,
+            })
+            if self.msi_type == "msi":
+                config.update({
+                    "MSI_64b"                  : False,
+                    "Multiple_Message_Capable" : "1_vector",
+                })
+            if self.msi_type == "msi-multi-vector":
+                config.update({
+                    "MSI_64b"                  : False,
+                    "Multiple_Message_Capable" : "1_vector", # FIXME.
+                })
+            if self.msi_type == "msi-x":
+                config.update({
+                    "mode_selection"    : "Advanced",
+                    "MSI_Enabled"       : False,
+                    "MSIx_Enabled"      : True,
+                    "MSIx_Table_Size"   : "20",   # Hexa.
+                    "MSIx_Table_Offset" : "2000", # Hexa, should match CSR_PCIE_MSI_TABLE_BASE.
+                    "MSIx_PBA_Offset"   : "1808", # Hexa, should match CSR_PCIE_MSI_PBA_ADDR.
+                })
+
+            # Extended Capabilities Registers.
+            if self.with_ptm:
+                config.update({
+                    "EXT_PCI_CFG_Space"      : True,
+                    "EXT_PCI_CFG_Space_Addr" : "6B", # 0x1AC.
+                })
+
+            # Tcl generation.
             ip_tcl = []
             ip_tcl.append("create_ip -vendor xilinx.com -name pcie_7x -module_name pcie_s7")
             ip_tcl.append("set obj [get_ips pcie_s7]")
             ip_tcl.append("set_property -dict [list \\")
             for config, value in config.items():
                 ip_tcl.append("CONFIG.{} {} \\".format(config, '{{' + str(value) + '}}'))
             ip_tcl.append(f"] $obj")
             ip_tcl.append("synth_ip $obj")
             platform.toolchain.pre_synthesis_commands += ip_tcl
+
         # Reset LOC constraints on GTPE2_COMMON and BRAM36 from .xci (we only want to keep Timing constraints).
         if platform.device.startswith("xc7a"):
             platform.toolchain.pre_placement_commands.append("reset_property LOC [get_cells -hierarchical -filter {{NAME=~pcie_s7/*gtp_common.gtpe2_common_i}}]")
         else:
             platform.toolchain.pre_placement_commands.append("reset_property LOC [get_cells -hierarchical -filter {{NAME=~pcie_s7/*gtx_common.gtxe2_common_i}}]")
         if self.nlanes != 8:
             platform.toolchain.pre_placement_commands.append("reset_property LOC [get_cells -hierarchical -filter {{NAME=~pcie_s7/*genblk*.bram36_tdp_bl.bram36_tdp_bl}}]")
```

### Comparing `litepcie-2023.4/litepcie/phy/uspciephy.py` & `litepcie-2023.8/litepcie/phy/uspciephy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 from litepcie.phy.common import *
 
 # USPCIEPHY ----------------------------------------------------------------------------------------
 
 class USPCIEPHY(LiteXModule):
     endianness    = "little"
     qword_aligned = False
-    def __init__(self, platform, pads, speed="gen3", data_width=64, bar0_size=1*MB, cd="sys", pcie_data_width=None):
+    def __init__(self, platform, pads, speed="gen3", data_width=64,  cd="sys",
+        # PCIe hardblock parameters.
+        pcie_data_width = None,
+        bar0_size       = 0x100000,
+    ):
         # Streams ----------------------------------------------------------------------------------
         self.req_sink   = stream.Endpoint(phy_layout(data_width))
         self.cmp_sink   = stream.Endpoint(phy_layout(data_width))
         self.req_source = stream.Endpoint(phy_layout(data_width))
         self.cmp_source = stream.Endpoint(phy_layout(data_width))
         self.msi        = stream.Endpoint(msi_layout())
```

### Comparing `litepcie-2023.4/litepcie/phy/usppciephy.py` & `litepcie-2023.8/litepcie/phy/usppciephy.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 from litepcie.phy.common import *
 
 # USPPCIEPHY ----------------------------------------------------------------------------------------
 
 class USPPCIEPHY(LiteXModule):
     endianness    = "little"
     qword_aligned = False
-    def __init__(self, platform, pads, speed="gen3", data_width=64, bar0_size=1*MB, cd="sys", pcie_data_width=None):
+    def __init__(self, platform, pads, speed="gen3", data_width=64, cd="sys",
+        # PCIe hardblock parameters.
+        pcie_data_width = None,
+        bar0_size       = 0x100000,
+    ):
         # Streams ----------------------------------------------------------------------------------
         self.req_sink   = stream.Endpoint(phy_layout(data_width))
         self.cmp_sink   = stream.Endpoint(phy_layout(data_width))
         self.req_source = stream.Endpoint(phy_layout(data_width))
         self.cmp_source = stream.Endpoint(phy_layout(data_width))
         self.msi        = stream.Endpoint(msi_layout())
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x4/pcie_us.xci` & `litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x4/pcie_us.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x4/pcie_us_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x4/pcie_us_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -1060,15 +1060,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x8/pcie_us.xci` & `litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x8/pcie_us.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_us_gen3_x8/pcie_us_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_us_gen3_x8/pcie_us_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp.xci` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x16/pcie_usp_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -857,15 +857,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp.xci` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x4/pcie_usp_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -895,15 +895,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp.xci` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_usp_gen3_x8/pcie_usp_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -854,15 +854,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp.xci` & `litepcie-2023.8/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp.xci`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp_support.v` & `litepcie-2023.8/litepcie/phy/xilinx_usp_hbm_gen3_x4/pcie_usp_support.v`

 * *Files 0% similar despite different names*

```diff
@@ -895,15 +895,15 @@
        endcase
 
   //edge detect valid
   reg [1:0]       cfg_interrupt_msi_int_valid_sh;
   wire            cfg_interrupt_msi_int_valid_edge = cfg_interrupt_msi_int_valid_sh == 2'b01;
   always @(posedge user_clk_out)
       if (user_reset_out) cfg_interrupt_msi_int_valid_sh <= 2'd0;
-      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid};
+      else cfg_interrupt_msi_int_valid_sh <= {cfg_interrupt_msi_int_valid_sh[0], cfg_interrupt_msi_int_valid & ~(cfg_interrupt_msi_sent | cfg_interrupt_msi_fail)};
 
   //latch int_enc
   reg [31:0]      cfg_interrupt_msi_int_enc_lat = 32'b0;
   always @(posedge user_clk_out)
       if (cfg_interrupt_msi_int_valid_edge) cfg_interrupt_msi_int_enc_lat <= cfg_interrupt_msi_int_enc;
       else if (cfg_interrupt_msi_sent) cfg_interrupt_msi_int_enc_lat <= 32'b0;
```

### Comparing `litepcie-2023.4/litepcie/software/__init__.py` & `litepcie-2023.8/litepcie/software/__init__.py`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/software/kernel/Makefile` & `litepcie-2023.8/litepcie/software/kernel/Makefile`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/software/kernel/config.h` & `litepcie-2023.8/litepcie/software/kernel/config.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 /* SPDX-License-Identifier: BSD-2-Clause
+ *
+ * LitePCIe driver
+ *
+ * This file is part of LitePCIe.
+ *
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #ifndef __HW_CONFIG_H
 #define __HW_CONFIG_H
 #include "soc.h"
 
 /* PCIe PHY Vendor/Device IDs */
```

### Comparing `litepcie-2023.4/litepcie/software/kernel/init.sh` & `litepcie-2023.8/litepcie/software/kernel/init.sh`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/software/kernel/litepcie.h` & `litepcie-2023.8/litepcie/software/kernel/litepcie.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /* SPDX-License-Identifier: BSD-2-Clause
  *
  * LitePCIe driver
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
  *
  */
 
 #ifndef _LINUX_LITEPCIE_H
 #define _LINUX_LITEPCIE_H
 
 #include <linux/types.h>
```

### Comparing `litepcie-2023.4/litepcie/software/kernel/liteuart.c` & `litepcie-2023.8/litepcie/software/kernel/liteuart.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-// SPDX-License-Identifier: GPL-2.0
-/*
+/* SPDX-License-Identifier: GPL-2.0
+ *
  * LiteUART serial controller (LiteX) Driver
  *
  * Copyright (C) 2019-2020 Antmicro <www.antmicro.com>
  */
 
 #include <linux/console.h>
 //#include <linux/litex.h> FIXME: Too early to use litex.h directly from kernel, use a local version for now.
@@ -12,14 +12,15 @@
 #include <linux/of_address.h>
 #include <linux/of_platform.h>
 #include <linux/serial.h>
 #include <linux/serial_core.h>
 #include <linux/slab.h>
 #include <linux/timer.h>
 #include <linux/tty_flip.h>
+#include <linux/version.h>
 #include <linux/xarray.h>
 
 #include "litex.h"
 
 // FIXME: Too early to use  platform_get_mem_or_io directly from kernel, use a local version for now.
 
 static struct resource *local_platform_get_mem_or_io(struct platform_device *dev,
@@ -193,15 +194,19 @@
 }
 
 static void liteuart_shutdown(struct uart_port *port)
 {
 }
 
 static void liteuart_set_termios(struct uart_port *port, struct ktermios *new,
+#if LINUX_VERSION_CODE < KERNEL_VERSION(6, 1, 0)
 				 struct ktermios *old)
+#else
+				 const struct ktermios *old)
+#endif
 {
 	unsigned int baud;
 	unsigned long flags;
 
 	spin_lock_irqsave(&port->lock, flags);
 
 	/* update baudrate */
```

### Comparing `litepcie-2023.4/litepcie/software/kernel/litex.h` & `litepcie-2023.8/litepcie/software/kernel/litex.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-/* SPDX-License-Identifier: GPL-2.0 */
-/*
+/* SPDX-License-Identifier: GPL-2.0
+ *
  * Common LiteX header providing
  * helper functions for accessing CSRs.
  *
  * Copyright (C) 2019-2020 Antmicro <www.antmicro.com>
  */
 
 #ifndef _LINUX_LITEX_H
```

### Comparing `litepcie-2023.4/litepcie/software/kernel/main.c` & `litepcie-2023.8/litepcie/software/kernel/main.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-// SPDX-License-Identifier: BSD-2-Clause
-
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe driver
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <linux/kernel.h>
 #include <linux/module.h>
 #include <linux/types.h>
 #include <linux/ioctl.h>
 #include <linux/init.h>
@@ -45,14 +45,18 @@
 //#define DEBUG_POLL
 //#define DEBUG_READ
 //#define DEBUG_WRITE
 
 #define LITEPCIE_NAME "litepcie"
 #define LITEPCIE_MINOR_COUNT 32
 
+#ifndef CSR_BASE
+#define CSR_BASE 0x00000000
+#endif
+
 struct litepcie_dma_chan {
 	uint32_t base;
 	uint32_t writer_interrupt;
 	uint32_t reader_interrupt;
 	dma_addr_t reader_handle[DMA_BUFFER_COUNT];
 	dma_addr_t writer_handle[DMA_BUFFER_COUNT];
 	uint32_t *reader_addr[DMA_BUFFER_COUNT];
@@ -309,15 +313,15 @@
 	uint32_t clear_mask, irq_vector, irq_enable;
 	int i;
 
 /* Single MSI */
 #ifdef CSR_PCIE_MSI_CLEAR_ADDR
 	irq_vector = litepcie_readl(s, CSR_PCIE_MSI_VECTOR_ADDR);
 	irq_enable = litepcie_readl(s, CSR_PCIE_MSI_ENABLE_ADDR);
-/* Multi-Vector MSI */
+/* MSI MultiVector / MSI-X */
 #else
 	irq_vector = 0;
 	for (i = 0; i < s->irqs; i++) {
 		if (irq == pci_irq_vector(s->dev, i)) {
 			irq_vector = (1 << i);
 			break;
 		}
@@ -1043,27 +1047,40 @@
 	ret = dma_set_mask(&dev->dev, DMA_BIT_MASK(DMA_ADDR_WIDTH));
 #endif
 	if (ret) {
 		dev_err(&dev->dev, "Failed to set DMA mask\n");
 		goto fail1;
 	};
 
+
+/* MSI-X */
+#ifdef CSR_PCIE_MSI_PBA_ADDR
+	irqs = pci_alloc_irq_vectors(dev, 1, 32, PCI_IRQ_MSIX);
+/* MSI Single / MultiVector */
+#else
 	irqs = pci_alloc_irq_vectors(dev, 1, 32, PCI_IRQ_MSI);
+#endif
 	if (irqs < 0) {
 		dev_err(&dev->dev, "Failed to enable MSI\n");
 		ret = irqs;
 		goto fail1;
 	}
+/* MSI-X */
+#ifdef CSR_PCIE_MSI_PBA_ADDR
+	dev_info(&dev->dev, "%d MSI-X IRQs allocated.\n", irqs);
+/* MSI Single / MultiVector */
+#else
 	dev_info(&dev->dev, "%d MSI IRQs allocated.\n", irqs);
+#endif
 
 	litepcie_dev->irqs = 0;
 	for (i = 0; i < irqs; i++) {
 		int irq = pci_irq_vector(dev, i);
 
-		ret = request_irq(irq, litepcie_interrupt, IRQF_SHARED, LITEPCIE_NAME, litepcie_dev);
+		ret = request_irq(irq, litepcie_interrupt, 0, LITEPCIE_NAME, litepcie_dev);
 		if (ret < 0) {
 			dev_err(&dev->dev, " Failed to allocate IRQ %d\n", dev->irq);
 			while (--i >= 0) {
 				irq = pci_irq_vector(dev, i);
 				free_irq(irq, dev);
 			}
 			goto fail2;
```

### Comparing `litepcie-2023.4/litepcie/software/user/Makefile` & `litepcie-2023.8/litepcie/software/user/Makefile`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_dma.c` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_dma.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <stdio.h>
 #include <stdlib.h>
 #include <fcntl.h>
 #include <unistd.h>
 #include <sys/mman.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_dma.h` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_dma.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #ifndef LITEPCIE_LIB_DMA_H
 #define LITEPCIE_LIB_DMA_H
 
 #include <stdint.h>
 #include <poll.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_flash.c` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_flash.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <sys/ioctl.h>
 #include <stdio.h>
 #include <unistd.h>
 #include <string.h>
 #include "litepcie_flash.h"
```

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_flash.h` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_flash.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #ifndef LITEPCIE_LIB_FLASH_H
 #define LITEPCIE_LIB_FLASH_H
 
 #include <stdint.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_helpers.c` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_helpers.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <time.h>
 #include <sys/ioctl.h>
 #include <stdio.h>
 #include <errno.h>
 #include <string.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/liblitepcie/litepcie_helpers.h` & `litepcie-2023.8/litepcie/software/user/liblitepcie/litepcie_helpers.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe library
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2020 / EnjoyDigital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #ifndef LITEPCIE_LIB_HELPERS_H
 #define LITEPCIE_LIB_HELPERS_H
 
 #include <stdint.h>
 #include <sys/ioctl.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/litepcie_test.c` & `litepcie-2023.8/litepcie/software/user/litepcie_test.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe test
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2022 / Enjoy-Digital  / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 #include <inttypes.h>
 #include <unistd.h>
```

### Comparing `litepcie-2023.4/litepcie/software/user/litepcie_util.c` & `litepcie-2023.8/litepcie/software/user/litepcie_util.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-/*
+/* SPDX-License-Identifier: BSD-2-Clause
+ *
  * LitePCIe util
  *
  * This file is part of LitePCIe.
  *
- * Copyright (C) 2018-2022 / Enjoy-Digital / florent@enjoy-digital.fr
- * SPDX-License-Identifier: BSD-2-Clause
+ * Copyright (C) 2018-2023 / EnjoyDigital  / florent@enjoy-digital.fr
+ *
  */
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 #include <stdarg.h>
 #include <inttypes.h>
```

### Comparing `litepcie-2023.4/litepcie/tlp/controller.py` & `litepcie-2023.8/litepcie/tlp/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # This file is part of LitePCIe.
 #
 # Copyright (c) 2015-2021 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
+from litex.gen import *
+
 from litepcie.common import *
 from litepcie.core.common import *
 from litepcie.tlp.common import *
 
 
-class LitePCIeTLPController(Module):
+class LitePCIeTLPController(LiteXModule):
     """LitePCIe TLP requests/completions controller.
 
     Arbitrate/throttle TLP requests and reorder/assemble/redirect completions.
     """
     def __init__(self, data_width, address_width, max_pending_requests, cmp_bufs_buffered=True):
         self.master_in  = LitePCIeMasterInternalPort(data_width, address_width)
         self.master_out = LitePCIeMasterInternalPort(data_width, address_width)
@@ -29,27 +31,27 @@
         tag_bits = log2_int(max_pending_requests)
 
         # Tag queue --------------------------------------------------------------------------------
         # The tag queue is filled initially with the tags that will be used to issue read requests
         # to the host. A tag is dequeued when a read requests is issued to the host and queued when
         # a readcomplementation is received from the host.
         tag_queue = SyncFIFO([("tag", tag_bits)], max_pending_requests, buffered=True)
-        self.submodules.tag_queue = tag_queue
+        self.tag_queue = tag_queue
 
         # Requests queue ---------------------------------------------------------------------------
         # Store the read requests tags as emitted to the host, datas will be dequeued in this order
         req_queue_layout = [("tag", tag_bits), ("channel", 8), ("user_id", 8)]
         req_queue        = SyncFIFO(req_queue_layout, max_pending_requests, buffered=True)
-        self.submodules.req_queue = req_queue
+        self.req_queue = req_queue
 
         # Requests Management ----------------------------------------------------------------------
 
         # Connect Data-Path.
         self.comb += req_sink.connect(req_source, omit={"valid", "ready", "tag"})
-        self.submodules.req_fsm = req_fsm = FSM(reset_state="WAIT-REQ")
+        self.req_fsm = req_fsm = FSM(reset_state="WAIT-REQ")
 
         # FSM.
         req_fsm.act("WAIT-REQ",
             # Wait for a TLP Request...
             If(req_sink.valid & req_sink.first,
                 # TLP Write: We can send the request directly.
                 If(req_sink.we,
@@ -135,15 +137,15 @@
 
         fill_tag = Signal(tag_bits)
 
         # Connect Data-Path.
         self.comb += cmp_sink.connect(cmp_reorder, omit={"valid", "ready"})
 
         # FSM
-        self.submodules.cmp_fsm = cmp_fsm = FSM(reset_state="FILL-TAG-QUEUE")
+        self.cmp_fsm = cmp_fsm = FSM(reset_state="FILL-TAG-QUEUE")
         cmp_fsm.act("FILL-TAG-QUEUE",
             # Pre-fill Tags.
             tag_queue.sink.valid.eq(1),
             tag_queue.sink.tag.eq(fill_tag),
             NextValue(fill_tag, fill_tag + 1),
             If(fill_tag == (max_pending_requests - 1),
                 NextState("WAIT")
```

### Comparing `litepcie-2023.4/litepcie/tlp/depacketizer.py` & `litepcie-2023.8/litepcie/tlp/depacketizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # This file is part of LitePCIe.
 #
 # Copyright (c) 2015-2022 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
+from litex.gen import *
+
 from litepcie.tlp.common import *
 
 # LitePCIeTLPHeaderExtracter64b --------------------------------------------------------------------
 
-class LitePCIeTLPHeaderExtracter64b(Module):
+class LitePCIeTLPHeaderExtracter64b(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(phy_layout(64))
         self.source = source = stream.Endpoint(tlp_raw_layout(64))
 
         # # #
 
         first = Signal()
@@ -24,15 +26,15 @@
         be    = Signal(64//8, reset_less=True)
         self.sync += \
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be)
             )
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(first, 1),
             NextValue(last,  0),
             NextValue(count, 0),
             If(sink.valid, NextState("HEADER"))
         )
         fsm.act("HEADER",
@@ -64,15 +66,15 @@
             source.dat[32*1:32*2].eq(sink.dat[32*0:32*1]),
             source.be[  4*0: 4*1].eq(     be[4*1:4*2]),
             source.be[  4*1: 4*2].eq(sink.be[4*0:4*1])
         ]
 
 # LitePCIeTLPHeaderExtracter128b -------------------------------------------------------------------
 
-class LitePCIeTLPHeaderExtracter128b(Module):
+class LitePCIeTLPHeaderExtracter128b(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(phy_layout(128))
         self.source = source = stream.Endpoint(tlp_raw_layout(128))
 
         # # #
 
         first = Signal()
@@ -81,15 +83,15 @@
         be    = Signal(128//8, reset_less=True)
         self.sync += \
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be)
             )
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(first, 1),
             NextValue(last,  0),
             If(sink.valid,
                 NextState("HEADER")
             )
         )
@@ -127,15 +129,15 @@
             source.be[  4*1: 4*2].eq(   sink.be[4*0:4*1]),
             source.be[  4*2: 4*3].eq(   sink.be[4*1:4*2]),
             source.be[  4*1: 4*2].eq(   sink.be[4*2:4*3]),
         ]
 
 # LitePCIeTLPHeaderExtracter256b -------------------------------------------------------------------
 
-class LitePCIeTLPHeaderExtracter256b(Module):
+class LitePCIeTLPHeaderExtracter256b(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(phy_layout(256))
         self.source = source = stream.Endpoint(tlp_raw_layout(256))
 
         # # #
 
         first = Signal()
@@ -144,15 +146,15 @@
         be    = Signal(256//8, reset_less=True)
         self.sync += \
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be)
             )
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(first, 1),
             NextValue(last,  0),
             If(sink.valid,
                 NextState("HEADER")
             )
         )
@@ -199,15 +201,15 @@
             source.be[4*5:4*6].eq(sink.be[4*0:4*1]),
             source.be[4*6:4*7].eq(sink.be[4*1:4*2]),
             source.be[4*7:4*8].eq(sink.be[4*2:4*3])
         ]
 
 # LitePCIeTLPHeaderExtracter512b -------------------------------------------------------------------
 
-class LitePCIeTLPHeaderExtracter512b(Module):
+class LitePCIeTLPHeaderExtracter512b(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(phy_layout(512))
         self.source = source = stream.Endpoint(tlp_raw_layout(512))
 
         # # #
 
         first = Signal()
@@ -216,15 +218,15 @@
         be    = Signal(512//8, reset_less=True)
         self.sync += \
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be)
             )
 
-        self.submodules.fsm = fsm = FSM(reset_state="IDLE")
+        self.fsm = fsm = FSM(reset_state="IDLE")
         fsm.act("IDLE",
             NextValue(first, 1),
             NextValue(last,  0),
             If(sink.valid,
                 NextState("HEADER")
             )
         )
@@ -288,108 +290,207 @@
             source.be[4*13:4*14].eq(sink.be[ 4*0: 4*1]),
             source.be[4*14:4*15].eq(sink.be[ 4*1: 4*2]),
             source.be[4*15:4*16].eq(sink.be[ 4*2: 4*3]),
         ]
 
 # LitePCIeTLPDepacketizer --------------------------------------------------------------------------
 
-class LitePCIeTLPDepacketizer(Module):
-    def __init__(self, data_width, endianness, address_mask=0):
-        self.sink       = stream.Endpoint(phy_layout(data_width))
-        self.req_source = stream.Endpoint(request_layout(data_width))
-        self.cmp_source = stream.Endpoint(completion_layout(data_width))
+class LitePCIeTLPDepacketizer(LiteXModule):
+    def __init__(self, data_width, endianness, address_mask=0, capabilities=["REQUEST", "COMPLETION"]):
+        # Sink Endpoint.
+        self.sink = stream.Endpoint(phy_layout(data_width))
+
+        # Source Endpoints.
+        for c in capabilities:
+            assert c in ["REQUEST", "COMPLETION", "CONFIGURATION", "PTM"]
+        if "REQUEST" in capabilities:
+            self.req_source  = req_source  = stream.Endpoint(request_layout(data_width))
+        if "COMPLETION" in capabilities:
+            self.cmp_source  = cmp_source  = stream.Endpoint(completion_layout(data_width))
+        if "CONFIGURATION" in capabilities:
+            self.conf_source = conf_source = stream.Endpoint(configuration_layout(data_width))
+        if "PTM" in capabilities:
+            self.ptm_source = ptm_source = stream.Endpoint(ptm_layout(data_width))
 
         # # #
 
-        # Extract raw header -----------------------------------------------------------------------
+        # Extract RAW Header from Sink -------------------------------------------------------------
+
         header_extracter_cls = {
              64 : LitePCIeTLPHeaderExtracter64b,
             128 : LitePCIeTLPHeaderExtracter128b,
             256 : LitePCIeTLPHeaderExtracter256b,
             512 : LitePCIeTLPHeaderExtracter512b,
         }
-        header_extracter = header_extracter_cls[data_width]()
-        self.submodules += header_extracter
+        self.header_extracter = header_extracter = header_extracter_cls[data_width]()
         self.comb += self.sink.connect(header_extracter.sink)
         header = header_extracter.source.header
 
-        # Dispatch data according to fmt/type ------------------------------------------------------
-        dispatch_source = stream.Endpoint(tlp_common_layout(data_width))
-        dispatch_sinks  = [stream.Endpoint(tlp_common_layout(data_width)) for i in range(3)]
-        self.comb += dispatch_sinks[0b00].ready.eq(1) # Always ready when unknown.
+        # Create Dispatcher ------------------------------------------------------------------------
+
+        # Dispatch Sources
+        self.dispatch_sources = dispatch_sources = {"DISCARD" : stream.Endpoint(tlp_common_layout(data_width))}
+        for source in capabilities:
+            dispatch_sources[source] = stream.Endpoint(tlp_common_layout(data_width))
+
+        def dispatch_source_sel(name):
+            for n, k in enumerate(dispatch_sources.keys()):
+                if k == name:
+                    return n
+            return None
+
+        # Dispatch Sink.
+        self.dispatch_sink = dispatch_sink = stream.Endpoint(tlp_common_layout(data_width))
+
+        # Dispatcher
+        self.dispatcher = Dispatcher(
+            master = dispatch_sink,
+            slaves = dispatch_sources.values()
+        )
+
+        # Ensure DISCARD source is always ready.
+        self.comb += dispatch_sources["DISCARD"].ready.eq(1)
 
+        # Connect Header Extracter to Dispatch Sink.
         self.comb += [
-            dispatch_source.valid.eq(header_extracter.source.valid),
-            header_extracter.source.ready.eq(dispatch_source.ready),
-            dispatch_source.first.eq(header_extracter.source.first),
-            dispatch_source.last.eq(header_extracter.source.last),
-            tlp_common_header.decode(header, dispatch_source)
+            header_extracter.source.connect(dispatch_sink, keep={"valid", "ready", "first", "last"}),
+            tlp_common_header.decode(header, dispatch_sink)
         ]
         self.comb += dword_endianness_swap(
             src        = header_extracter.source.dat,
-            dst        = dispatch_source.dat,
+            dst        = dispatch_sink.dat,
             data_width = data_width,
             endianness = endianness,
             mode       = "dat",
         )
         self.comb += dword_endianness_swap(
             src        = header_extracter.source.be,
-            dst        = dispatch_source.be,
+            dst        = dispatch_sink.be,
             data_width = data_width,
             endianness = endianness,
             mode       = "be",
         )
-        self.submodules.dispatcher = Dispatcher(dispatch_source, dispatch_sinks)
 
-        fmt_type = Cat(dispatch_source.type, dispatch_source.fmt)
-        self.comb += [
-            self.dispatcher.sel.eq(0b00),
-            If((fmt_type == fmt_type_dict["mem_rd32"]) |
-               (fmt_type == fmt_type_dict["mem_wr32"]),
-                self.dispatcher.sel.eq(0b01),
-            ),
-            If((fmt_type == fmt_type_dict["cpld"]) |
-               (fmt_type == fmt_type_dict["cpl"]),
-               self.dispatcher.sel.eq(0b10),
-            ),
-        ]
+        # Create fmt_type for destination decoding.
+        fmt_type = Cat(dispatch_sink.type, dispatch_sink.fmt)
 
-        # Decode TLP request and format local request ----------------------------------------------
-        self.tlp_req = tlp_req = stream.Endpoint(tlp_request_layout(data_width))
-        self.comb += dispatch_sinks[0b01].connect(tlp_req)
-        self.comb += tlp_request_header.decode(header, tlp_req)
+        # Set default Dispatcher select to DISCARD Sink.
+        self.comb += self.dispatcher.sel.eq(dispatch_source_sel("DISCARD"))
 
-        req_type   = Cat(tlp_req.type, tlp_req.fmt)
-        req_source = self.req_source
-        self.comb += [
-            req_source.valid.eq(tlp_req.valid),
-            req_source.we.eq(tlp_req.valid & (req_type == fmt_type_dict["mem_wr32"])),
-            tlp_req.ready.eq(req_source.ready),
-            req_source.first.eq(tlp_req.first),
-            req_source.last.eq(tlp_req.last),
-            req_source.adr.eq(tlp_req.address & (~address_mask)),
-            req_source.len.eq(tlp_req.length),
-            req_source.req_id.eq(tlp_req.requester_id),
-            req_source.tag.eq(tlp_req.tag),
-            req_source.dat.eq(tlp_req.dat)
-        ]
+        # Decode/Dispatch TLP Requests -------------------------------------------------------------
 
-        # Decode TLP completion and format local completion ----------------------------------------
-        self.tlp_cmp = tlp_cmp = stream.Endpoint(tlp_completion_layout(data_width))
-        self.comb += dispatch_sinks[0b10].connect(tlp_cmp)
-        self.comb += tlp_completion_header.decode(header, tlp_cmp)
+        if "REQUEST" in capabilities:
+            self.comb += [
+                If((fmt_type == fmt_type_dict["mem_rd32"]) |
+                   (fmt_type == fmt_type_dict["mem_wr32"]),
+                    self.dispatcher.sel.eq(dispatch_source_sel("REQUEST")),
+                )
+            ]
 
-        cmp_source = self.cmp_source
-        self.comb += [
-            cmp_source.valid.eq(tlp_cmp.valid),
-            tlp_cmp.ready.eq(cmp_source.ready),
-            cmp_source.first.eq(tlp_cmp.first),
-            cmp_source.last.eq(tlp_cmp.last),
-            cmp_source.len.eq(tlp_cmp.length),
-            cmp_source.end.eq(tlp_cmp.length == (tlp_cmp.byte_count[2:])),
-            cmp_source.adr.eq(tlp_cmp.lower_address),
-            cmp_source.req_id.eq(tlp_cmp.requester_id),
-            cmp_source.cmp_id.eq(tlp_cmp.completer_id),
-            cmp_source.err.eq(tlp_cmp.status != 0),
-            cmp_source.tag.eq(tlp_cmp.tag),
-            cmp_source.dat.eq(tlp_cmp.dat)
-        ]
+            self.tlp_req = tlp_req = stream.Endpoint(tlp_request_layout(data_width))
+            self.comb += dispatch_sources["REQUEST"].connect(tlp_req)
+            self.comb += tlp_request_header.decode(header, tlp_req)
+
+            req_type = Cat(tlp_req.type, tlp_req.fmt)
+            self.comb += [
+                req_source.valid.eq(tlp_req.valid),
+                req_source.we.eq(tlp_req.valid & (req_type == fmt_type_dict["mem_wr32"])),
+                tlp_req.ready.eq(req_source.ready),
+                req_source.first.eq(tlp_req.first),
+                req_source.last.eq(tlp_req.last),
+                req_source.adr.eq(tlp_req.address & (~address_mask)),
+                req_source.len.eq(tlp_req.length),
+                req_source.req_id.eq(tlp_req.requester_id),
+                req_source.tag.eq(tlp_req.tag),
+                req_source.dat.eq(tlp_req.dat)
+            ]
+
+        # Decode/Dispatch TLP Completions ----------------------------------------------------------
+
+        if "COMPLETION" in capabilities:
+            self.comb += [
+                If((fmt_type == fmt_type_dict["cpld"]) |
+                   (fmt_type == fmt_type_dict["cpl"]),
+                    self.dispatcher.sel.eq(dispatch_source_sel("COMPLETION")),
+                )
+            ]
+
+            self.tlp_cmp = tlp_cmp = stream.Endpoint(tlp_completion_layout(data_width))
+            self.comb += dispatch_sources["COMPLETION"].connect(tlp_cmp)
+            self.comb += tlp_completion_header.decode(header, tlp_cmp)
+
+            self.comb += [
+                cmp_source.valid.eq(tlp_cmp.valid),
+                tlp_cmp.ready.eq(cmp_source.ready),
+                cmp_source.first.eq(tlp_cmp.first),
+                cmp_source.last.eq(tlp_cmp.last),
+                cmp_source.len.eq(tlp_cmp.length),
+                cmp_source.end.eq(tlp_cmp.length == (tlp_cmp.byte_count[2:])),
+                cmp_source.adr.eq(tlp_cmp.lower_address),
+                cmp_source.req_id.eq(tlp_cmp.requester_id),
+                cmp_source.cmp_id.eq(tlp_cmp.completer_id),
+                cmp_source.err.eq(tlp_cmp.status != 0),
+                cmp_source.tag.eq(tlp_cmp.tag),
+                cmp_source.dat.eq(tlp_cmp.dat)
+            ]
+
+
+        # Decode/Dispatch TLP Configurations -------------------------------------------------------
+
+        if "CONFIGURATION" in capabilities:
+            self.comb += [
+                If((fmt_type == fmt_type_dict["cfg_rd0"]) |
+                   (fmt_type == fmt_type_dict["cfg_wr0"]),
+                    self.dispatcher.sel.eq(dispatch_source_sel("CONFIGURATION")),
+                )
+            ]
+
+            self.tlp_conf = tlp_conf = stream.Endpoint(tlp_configuration_layout(data_width))
+            self.comb += dispatch_sources["CONFIGURATION"].connect(tlp_conf)
+            self.comb += tlp_configuration_header.decode(header, tlp_conf)
+
+            self.comb += [
+                conf_source.valid.eq(tlp_conf.valid),
+                tlp_conf.ready.eq(conf_source.ready),
+                conf_source.first.eq(tlp_conf.first),
+                conf_source.last.eq(tlp_conf.last),
+                If(fmt_type == fmt_type_dict["cfg_rd0"],
+                    conf_source.we.eq(0)
+                ),
+                If(fmt_type == fmt_type_dict["cfg_wr0"],
+                    conf_source.we.eq(1)
+                ),
+                conf_source.req_id.eq(tlp_conf.requester_id),
+                conf_source.bus_number.eq(tlp_conf.bus_number),
+                conf_source.device_no.eq(tlp_conf.device_no),
+                conf_source.func.eq(tlp_conf.func),
+                conf_source.ext_reg.eq(tlp_conf.ext_reg),
+                conf_source.register_no.eq(tlp_conf.register_no),
+                conf_source.tag.eq(tlp_conf.tag),
+                conf_source.dat.eq(tlp_conf.dat)
+            ]
+
+        # Decode/Dispatch TLP PTM Requests/Responses -----------------------------------------------
+
+        if "PTM" in capabilities:
+            self.comb += [
+                If((fmt_type == fmt_type_dict["ptm_req"]) |
+                   (fmt_type == fmt_type_dict["ptm_res"]),
+                    self.dispatcher.sel.eq(dispatch_source_sel("PTM")),
+                )
+            ]
+
+            self.tlp_ptm = tlp_ptm = stream.Endpoint(tlp_ptm_layout(data_width))
+            self.comb += dispatch_sources["PTM"].connect(tlp_ptm)
+            self.comb += tlp_ptm_header.decode(header, tlp_ptm)
+
+            self.comb += [
+                ptm_source.valid.eq(tlp_ptm.valid),
+                tlp_ptm.ready.eq(ptm_source.ready),
+                ptm_source.first.eq(tlp_ptm.first),
+                ptm_source.last.eq(tlp_ptm.last),
+                ptm_source.requester_id.eq(tlp_ptm.requester_id),
+                ptm_source.length.eq(tlp_ptm.length),
+                ptm_source.message_code.eq(tlp_ptm.message_code),
+                ptm_source.master_time.eq(tlp_ptm.master_time),
+                ptm_source.dat.eq(tlp_ptm.dat)
+            ]
```

### Comparing `litepcie-2023.4/litepcie/tlp/packetizer.py` & `litepcie-2023.8/litepcie/tlp/packetizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #
 # This file is part of LitePCIe.
 #
-# Copyright (c) 2015-2022 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015-2023 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import chooser
+
+from litex.gen import *
+from litex.gen.genlib.misc import chooser
 
 from litepcie.tlp.common import *
 
 # LitePCIeTLPHeaderInserter ------------------------------------------------------------------------
 
-class LitePCIeTLPHeaderInserter3DWs4DWs(Module):
+class LitePCIeTLPHeaderInserter3DWs4DWs(LiteXModule):
     def __init__(self, data_width, header_inserter_3dws_cls, header_inserter_4dws_cls, fmt):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(data_width))
         self.source = source = stream.Endpoint(phy_layout(data_width))
 
         # # #
 
         # Header Inserters Modules.
@@ -30,14 +32,16 @@
         self.comb += Case(fmt, {
             fmt_dict["mem_rd32"] : header_sel.eq(_3DWS_SEL),
             fmt_dict["mem_rd64"] : header_sel.eq(_4DWS_SEL),
             fmt_dict["mem_wr32"] : header_sel.eq(_3DWS_SEL),
             fmt_dict["mem_wr64"] : header_sel.eq(_4DWS_SEL),
             fmt_dict[    "cpld"] : header_sel.eq(_3DWS_SEL),
             fmt_dict[     "cpl"] : header_sel.eq(_3DWS_SEL),
+            fmt_dict[ "ptm_req"] : header_sel.eq(_4DWS_SEL),
+            fmt_dict[ "ptm_res"] : header_sel.eq(_4DWS_SEL),
         })
 
         # Header Inserters Mux.
         self.comb += Case(header_sel, {
             _3DWS_SEL : [
                 sink.connect(header_inserter_3dws.sink),
                 header_inserter_3dws.source.connect(source),
@@ -46,15 +50,15 @@
                 sink.connect(header_inserter_4dws.sink),
                 header_inserter_4dws.source.connect(source),
             ],
         })
 
 # LitePCIeTLPHeaderInserter64b ---------------------------------------------------------------------
 
-class LitePCIeTLPHeaderInserter64b3DWs(Module):
+class LitePCIeTLPHeaderInserter64b3DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(64))
         self.source = source = stream.Endpoint(phy_layout(64))
 
         # # #
 
         count = Signal()
@@ -65,15 +69,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq((count == 0) & sink.first),
                 source.last.eq( (count == 1) & sink.last & (sink.be[4*1:] == 0)),
@@ -118,23 +122,23 @@
                 sink.ready.eq(~last),
                 If(source.last,
                     NextState("HEADER")
                 )
             )
         )
 
-class LitePCIeTLPHeaderInserter64b4DWs(Module):
+class LitePCIeTLPHeaderInserter64b4DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(64))
         self.source = source = stream.Endpoint(phy_layout(64))
 
         # # #
 
         count = Signal()
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq((count == 0) & sink.first),
                 source.last.eq( (count == 1) & sink.last & (sink.be == 0)),
@@ -186,15 +190,15 @@
             header_inserter_3dws_cls = LitePCIeTLPHeaderInserter64b3DWs,
             header_inserter_4dws_cls = LitePCIeTLPHeaderInserter64b4DWs,
             fmt                      = fmt,
         )
 
 # LitePCIeTLPHeaderInserter128b --------------------------------------------------------------------
 
-class LitePCIeTLPHeaderInserter128b3DWs(Module):
+class LitePCIeTLPHeaderInserter128b3DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(128))
         self.source = source = stream.Endpoint(phy_layout(128))
 
         # # #
 
         dat  = Signal(128,    reset_less=True)
@@ -204,15 +208,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be[4*1:] == 0)),
@@ -257,22 +261,22 @@
                 sink.ready.eq(~last),
                 If(source.last,
                     NextState("HEADER")
                 )
             )
         )
 
-class LitePCIeTLPHeaderInserter128b4DWs(Module):
+class LitePCIeTLPHeaderInserter128b4DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(128))
         self.source = source = stream.Endpoint(phy_layout(128))
 
         # # #
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be == 0)),
@@ -325,15 +329,15 @@
             header_inserter_3dws_cls = LitePCIeTLPHeaderInserter128b3DWs,
             header_inserter_4dws_cls = LitePCIeTLPHeaderInserter128b4DWs,
             fmt                      = fmt,
         )
 
 # LitePCIeTLPHeaderInserter256b --------------------------------------------------------------------
 
-class LitePCIeTLPHeaderInserter256b3DWs(Module):
+class LitePCIeTLPHeaderInserter256b3DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(256))
         self.source = source = stream.Endpoint(phy_layout(256))
 
         # # #
 
         dat  = Signal(256,    reset_less=True)
@@ -343,15 +347,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be[4*5:] == 0)),
@@ -411,15 +415,15 @@
                 sink.ready.eq(~last),
                 If(source.last,
                     NextState("HEADER")
                 )
             )
         )
 
-class LitePCIeTLPHeaderInserter256b4DWs(Module):
+class LitePCIeTLPHeaderInserter256b4DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(256))
         self.source = source = stream.Endpoint(phy_layout(256))
 
         # # #
 
         dat  = Signal(256,    reset_less=True)
@@ -429,15 +433,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be[4*4:] == 0)),
@@ -508,15 +512,15 @@
             header_inserter_3dws_cls = LitePCIeTLPHeaderInserter256b3DWs,
             header_inserter_4dws_cls = LitePCIeTLPHeaderInserter256b4DWs,
             fmt                      = fmt,
         )
 
 # LitePCIeTLPHeaderInserter512b --------------------------------------------------------------------
 
-class LitePCIeTLPHeaderInserter512b3DWs(Module):
+class LitePCIeTLPHeaderInserter512b3DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(512))
         self.source = source = stream.Endpoint(phy_layout(512))
 
         # # #
 
         dat  = Signal(512,    reset_less=True)
@@ -526,15 +530,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be[4*13:] == 0)),
@@ -626,15 +630,15 @@
                 sink.ready.eq(~last),
                 If(source.last,
                     NextState("HEADER")
                 )
             )
         )
 
-class LitePCIeTLPHeaderInserter512b4DWs(Module):
+class LitePCIeTLPHeaderInserter512b4DWs(LiteXModule):
     def __init__(self):
         self.sink   = sink   = stream.Endpoint(tlp_raw_layout(512))
         self.source = source = stream.Endpoint(phy_layout(512))
 
         # # #
 
         dat  = Signal(512,    reset_less=True)
@@ -644,15 +648,15 @@
             If(sink.valid & sink.ready,
                 dat.eq(sink.dat),
                 be.eq(sink.be),
                 last.eq(sink.last)
             )
         ]
 
-        self.submodules.fsm = fsm = FSM(reset_state="HEADER")
+        self.fsm = fsm = FSM(reset_state="HEADER")
         fsm.act("HEADER",
             sink.ready.eq(1),
             If(sink.valid & sink.first,
                 sink.ready.eq(0),
                 source.valid.eq(1),
                 source.first.eq(1),
                 source.last.eq(sink.last & (sink.be[4*12:] == 0)),
@@ -756,157 +760,230 @@
             header_inserter_3dws_cls = LitePCIeTLPHeaderInserter512b3DWs,
             header_inserter_4dws_cls = LitePCIeTLPHeaderInserter512b4DWs,
             fmt                      = fmt,
         )
 
 # LitePCIeTLPPacketizer ----------------------------------------------------------------------------
 
-class LitePCIeTLPPacketizer(Module):
-    def __init__(self, data_width, endianness, address_width=32):
+class LitePCIeTLPPacketizer(LiteXModule):
+    def __init__(self, data_width, endianness, address_width=32, capabilities=["REQUEST", "COMPLETION"]):
         assert data_width%32 == 0
         assert address_width in [32, 64]
         if address_width == 64:
             assert data_width in [64, 128, 256, 512]
-        self.req_sink = req_sink = stream.Endpoint(request_layout(data_width, address_width))
-        self.cmp_sink = cmp_sink = stream.Endpoint(completion_layout(data_width))
+        for c in capabilities:
+            assert c in ["REQUEST", "COMPLETION", "PTM"]
+        # Sink Endpoints.
+        if "REQUEST" in capabilities:
+            self.req_sink = req_sink = stream.Endpoint(request_layout(data_width, address_width))
+        if "COMPLETION" in capabilities:
+            self.cmp_sink = cmp_sink = stream.Endpoint(completion_layout(data_width))
+        if "PTM" in capabilities:
+            self.ptm_sink = ptm_sink = stream.Endpoint(ptm_layout(data_width))
+        # Source Endpoints.
         self.source   = stream.Endpoint(phy_layout(data_width))
 
         # # #
 
-        # Format TLP request and encode it ---------------------------------------------------------
-        self.tlp_req = tlp_req = stream.Endpoint(tlp_request_layout(data_width))
-        self.comb += [
-            tlp_req.valid.eq(req_sink.valid),
-            req_sink.ready.eq(tlp_req.ready),
-            tlp_req.first.eq(req_sink.first),
-            tlp_req.last.eq(req_sink.last),
-
-            tlp_req.type.eq(0b00000),
-            If(req_sink.we,
-                tlp_req.fmt.eq( fmt_dict[ f"mem_wr32"]),
-            ).Else(
-                tlp_req.fmt.eq( fmt_dict[ f"mem_rd32"]),
-            ),
-            tlp_req.address.eq(req_sink.adr),
-        ]
-        if address_width == 64:
+        # Format and Encode TLP Requests -----------------------------------------------------------
+
+        if "REQUEST" in capabilities:
+            self.tlp_req = tlp_req = stream.Endpoint(tlp_request_layout(data_width))
             self.comb += [
-                # Use WR64/RD64 only when 64-bit Address's MSB != 0, else use WR32/RD32.
-                If(req_sink.adr[32:] != 0,
-                    # Address's MSB on DW2, LSB on DW3 with 64-bit addressing: Requires swap due to
-                    # Packetizer's behavior.
-                    tlp_req.address[:32].eq(req_sink.adr[32:]),
-                    tlp_req.address[32:].eq(req_sink.adr[:32]),
-                    If(req_sink.we,
-                        tlp_req.fmt.eq( fmt_dict[ f"mem_wr64"]),
+                tlp_req.valid.eq(req_sink.valid),
+                req_sink.ready.eq(tlp_req.ready),
+                tlp_req.first.eq(req_sink.first),
+                tlp_req.last.eq(req_sink.last),
+
+                tlp_req.type.eq(0b00000),
+                If(req_sink.we,
+                    tlp_req.fmt.eq( fmt_dict[ f"mem_wr32"]),
+                ).Else(
+                    tlp_req.fmt.eq( fmt_dict[ f"mem_rd32"]),
+                ),
+                tlp_req.address.eq(req_sink.adr),
+            ]
+            if address_width == 64:
+                self.comb += [
+                    # Use WR64/RD64 only when 64-bit Address's MSB != 0, else use WR32/RD32.
+                    If(req_sink.adr[32:] != 0,
+                        # Address's MSB on DW2, LSB on DW3 with 64-bit addressing: Requires swap due to
+                        # Packetizer's behavior.
+                        tlp_req.address[:32].eq(req_sink.adr[32:]),
+                        tlp_req.address[32:].eq(req_sink.adr[:32]),
+                        If(req_sink.we,
+                            tlp_req.fmt.eq( fmt_dict[ f"mem_wr64"]),
+                        ).Else(
+                            tlp_req.fmt.eq( fmt_dict[ f"mem_rd64"]),
+                        ),
+                    )
+                ]
+
+            self.comb += [
+                tlp_req.tc.eq(0),
+                tlp_req.td.eq(0),
+                tlp_req.ep.eq(0),
+                tlp_req.attr.eq(0),
+                tlp_req.length.eq(req_sink.len),
+
+                tlp_req.requester_id.eq(req_sink.req_id),
+                tlp_req.tag.eq(req_sink.tag),
+                If(req_sink.len > 1,
+                    tlp_req.last_be.eq(0xf)
+                ).Else(
+                    tlp_req.last_be.eq(0x0)
+                ),
+                tlp_req.first_be.eq(0xf),
+                tlp_req.dat.eq(req_sink.dat),
+                If(req_sink.we,
+                    If(req_sink.len == 1,
+                        tlp_req.be.eq(0xf)
                     ).Else(
-                        tlp_req.fmt.eq( fmt_dict[ f"mem_rd64"]),
-                    ),
+                        tlp_req.be.eq(2**(data_width//8)-1)
+                    )
+                ).Else(
+                    tlp_req.be.eq(0x00)
                 )
             ]
 
-        self.comb += [
-            tlp_req.tc.eq(0),
-            tlp_req.td.eq(0),
-            tlp_req.ep.eq(0),
-            tlp_req.attr.eq(0),
-            tlp_req.length.eq(req_sink.len),
-
-            tlp_req.requester_id.eq(req_sink.req_id),
-            tlp_req.tag.eq(req_sink.tag),
-            If(req_sink.len > 1,
-                tlp_req.last_be.eq(0xf)
-            ).Else(
-                tlp_req.last_be.eq(0x0)
-            ),
-            tlp_req.first_be.eq(0xf),
-            tlp_req.dat.eq(req_sink.dat),
-            If(req_sink.we,
-                tlp_req.be.eq(2**(data_width//8)-1)
-            ).Else(
-                tlp_req.be.eq(0x00)
+            tlp_raw_req        = stream.Endpoint(tlp_raw_layout(data_width))
+            tlp_raw_req_header = Signal(len(tlp_raw_req.header))
+            self.comb += [
+                tlp_req.connect(tlp_raw_req, omit={*tlp_request_header_fields.keys()}),
+                tlp_raw_req.fmt.eq(tlp_req.fmt),
+                tlp_request_header.encode(tlp_req, tlp_raw_req_header),
+            ]
+            self.comb += dword_endianness_swap(
+                src        = tlp_raw_req_header,
+                dst        = tlp_raw_req.header,
+                data_width = data_width,
+                endianness = endianness,
+                mode       = "dat",
+                ndwords    = 4
             )
-        ]
 
-        tlp_raw_req        = stream.Endpoint(tlp_raw_layout(data_width))
-        tlp_raw_req_header = Signal(len(tlp_raw_req.header))
-        self.comb += [
-            tlp_req.connect(tlp_raw_req, omit={*tlp_request_header_fields.keys()}),
-            tlp_raw_req.fmt.eq(tlp_req.fmt),
-            tlp_request_header.encode(tlp_req, tlp_raw_req_header),
-        ]
-        self.comb += dword_endianness_swap(
-            src        = tlp_raw_req_header,
-            dst        = tlp_raw_req.header,
-            data_width = data_width,
-            endianness = endianness,
-            mode       = "dat",
-            ndwords    = 4
-        )
-
-        # Format TLP completion and encode it ------------------------------------------------------
-        self.tlp_cmp = tlp_cmp = stream.Endpoint(tlp_completion_layout(data_width))
-        self.comb += [
-            tlp_cmp.valid.eq(cmp_sink.valid),
-            cmp_sink.ready.eq(tlp_cmp.ready),
-            tlp_cmp.first.eq(cmp_sink.first),
-            tlp_cmp.last.eq(cmp_sink.last),
-
-            tlp_cmp.tc.eq(0),
-            tlp_cmp.td.eq(0),
-            tlp_cmp.ep.eq(0),
-            tlp_cmp.attr.eq(0),
-            tlp_cmp.length.eq(cmp_sink.len),
-
-            tlp_cmp.completer_id.eq(cmp_sink.cmp_id),
-            If(cmp_sink.err,
-                tlp_cmp.type.eq(type_dict["cpl"]),
-                tlp_cmp.fmt.eq( fmt_dict["cpl"]),
-                tlp_cmp.status.eq(cpl_dict["ur"])
-            ).Else(
-                tlp_cmp.type.eq(type_dict["cpld"]),
-                tlp_cmp.fmt.eq( fmt_dict["cpld"]),
-                tlp_cmp.status.eq(cpl_dict["sc"])
-            ),
-            tlp_cmp.bcm.eq(0),
-            tlp_cmp.byte_count.eq(cmp_sink.len*4),
+        # Format and Encode TLP Completions --------------------------------------------------------
 
-            tlp_cmp.requester_id.eq(cmp_sink.req_id),
-            tlp_cmp.tag.eq(cmp_sink.tag),
-            tlp_cmp.lower_address.eq(cmp_sink.adr),
-
-            tlp_cmp.dat.eq(cmp_sink.dat),
-            If(cmp_sink.last & cmp_sink.first,
-                tlp_cmp.be.eq(0xf)
-            ).Else(
-                tlp_cmp.be.eq(2**(data_width//8)-1)
-            ),
-        ]
+        if "COMPLETION" in capabilities:
+            self.tlp_cmp = tlp_cmp = stream.Endpoint(tlp_completion_layout(data_width))
+            self.comb += [
+                tlp_cmp.valid.eq(cmp_sink.valid),
+                cmp_sink.ready.eq(tlp_cmp.ready),
+                tlp_cmp.first.eq(cmp_sink.first),
+                tlp_cmp.last.eq(cmp_sink.last),
+
+                tlp_cmp.tc.eq(0),
+                tlp_cmp.td.eq(0),
+                tlp_cmp.ep.eq(0),
+                tlp_cmp.attr.eq(0),
+                tlp_cmp.length.eq(cmp_sink.len),
+
+                tlp_cmp.completer_id.eq(cmp_sink.cmp_id),
+                If(cmp_sink.err,
+                    tlp_cmp.type.eq(type_dict["cpl"]),
+                    tlp_cmp.fmt.eq( fmt_dict["cpl"]),
+                    tlp_cmp.status.eq(cpl_dict["ur"])
+                ).Else(
+                    tlp_cmp.type.eq(type_dict["cpld"]),
+                    tlp_cmp.fmt.eq( fmt_dict["cpld"]),
+                    tlp_cmp.status.eq(cpl_dict["sc"])
+                ),
+                tlp_cmp.bcm.eq(0),
+                tlp_cmp.byte_count.eq(cmp_sink.len*4),
 
-        tlp_raw_cmp        = stream.Endpoint(tlp_raw_layout(data_width))
-        tlp_raw_cmp_header = Signal(len(tlp_raw_cmp.header))
-        self.comb += [
-            tlp_cmp.connect(tlp_raw_cmp, omit={*tlp_completion_header_fields.keys()}),
-            tlp_raw_cmp.fmt.eq(tlp_cmp.fmt),
-            tlp_completion_header.encode(tlp_cmp, tlp_raw_cmp_header),
-        ]
-        self.comb += dword_endianness_swap(
-            src        = tlp_raw_cmp_header,
-            dst        = tlp_raw_cmp.header,
-            data_width = data_width,
-            endianness = endianness,
-            mode       = "dat",
-            ndwords    = 4
-        )
+                tlp_cmp.requester_id.eq(cmp_sink.req_id),
+                tlp_cmp.tag.eq(cmp_sink.tag),
+                tlp_cmp.lower_address.eq(cmp_sink.adr),
+
+                tlp_cmp.dat.eq(cmp_sink.dat),
+                If(cmp_sink.last & cmp_sink.first,
+                    tlp_cmp.be.eq(0xf)
+                ).Else(
+                    tlp_cmp.be.eq(2**(data_width//8)-1)
+                ),
+            ]
+
+            tlp_raw_cmp        = stream.Endpoint(tlp_raw_layout(data_width))
+            tlp_raw_cmp_header = Signal(len(tlp_raw_cmp.header))
+            self.comb += [
+                tlp_cmp.connect(tlp_raw_cmp, omit={*tlp_completion_header_fields.keys()}),
+                tlp_raw_cmp.fmt.eq(tlp_cmp.fmt),
+                tlp_completion_header.encode(tlp_cmp, tlp_raw_cmp_header),
+            ]
+            self.comb += dword_endianness_swap(
+                src        = tlp_raw_cmp_header,
+                dst        = tlp_raw_cmp.header,
+                data_width = data_width,
+                endianness = endianness,
+                mode       = "dat",
+                ndwords    = 4
+            )
+
+        # Format and Encode TLP Completions --------------------------------------------------------
+
+        if "PTM" in capabilities:
+            self.tlp_ptm = tlp_ptm = stream.Endpoint(tlp_ptm_layout(data_width))
+            self.comb += [
+                tlp_ptm.valid.eq(ptm_sink.valid),
+                ptm_sink.ready.eq(tlp_ptm.ready),
+                tlp_ptm.first.eq(ptm_sink.first),
+                tlp_ptm.last.eq(ptm_sink.last),
+
+                tlp_ptm.tc.eq(0),   # CHECKME.
+                tlp_ptm.ln.eq(0),   # CHECKME.
+                tlp_ptm.th.eq(0),   # CHECKME.
+                tlp_ptm.td.eq(0),   # CHECKME.
+                tlp_ptm.ep.eq(0),   # CHECKME.
+                tlp_ptm.attr.eq(0), # CHECKME.
+                tlp_ptm.length.eq(ptm_sink.length),
+
+                tlp_ptm.requester_id.eq(ptm_sink.requester_id),
+                tlp_ptm.message_code.eq(ptm_sink.message_code),
+                tlp_ptm.master_time.eq(ptm_sink.master_time),
+
+                If(ptm_sink.request,
+                    tlp_ptm.type.eq(type_dict["ptm_req"]),
+                    tlp_ptm.fmt.eq( fmt_dict["ptm_req"]),
+                ),
+                If(ptm_sink.response,
+                    tlp_ptm.type.eq(type_dict["ptm_res"]),
+                    tlp_ptm.fmt.eq( fmt_dict["ptm_res"]),
+                    tlp_ptm.dat.eq(ptm_sink.dat),
+                    tlp_ptm.be.eq(2**(data_width//8)-1), # CHECKME.
+                ),
+            ]
+
+            tlp_raw_ptm        = stream.Endpoint(tlp_raw_layout(data_width))
+            tlp_raw_ptm_header = Signal(len(tlp_raw_ptm.header))
+            self.comb += [
+                tlp_ptm.connect(tlp_raw_ptm, omit={*tlp_ptm_header_fields.keys()}),
+                tlp_raw_ptm.fmt.eq(tlp_ptm.fmt),
+                tlp_ptm_header.encode(tlp_ptm, tlp_raw_ptm_header),
+            ]
+            self.comb += dword_endianness_swap(
+                src        = tlp_raw_ptm_header,
+                dst        = tlp_raw_ptm.header,
+                data_width = data_width,
+                endianness = endianness,
+                mode       = "dat",
+                ndwords    = 4
+            )
 
         # Arbitrate --------------------------------------------------------------------------------
 
+        tlp_raws = []
+        if "REQUEST" in capabilities:
+            tlp_raws.append(tlp_raw_req)
+        if "COMPLETION" in capabilities:
+            tlp_raws.append(tlp_raw_cmp)
+        if "PTM" in capabilities:
+            tlp_raws.append(tlp_raw_ptm)
         tlp_raw = stream.Endpoint(tlp_raw_layout(data_width))
-        self.submodules.arbitrer = Arbiter(
-            masters = [tlp_raw_req, tlp_raw_cmp],
+        self.arbitrer = Arbiter(
+            masters = tlp_raws,
             slave   = tlp_raw
         )
 
         # Insert header ----------------------------------------------------------------------------
         header_inserter_cls = {
             64 : LitePCIeTLPHeaderInserter64b,
            128 : LitePCIeTLPHeaderInserter128b,
```

### Comparing `litepcie-2023.4/litepcie.egg-info/PKG-INFO` & `litepcie-2023.8/litepcie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litepcie
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable PCIe core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litepcie
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Keywords: HDL ASIC FPGA hardware design
```

### Comparing `litepcie-2023.4/litepcie.egg-info/SOURCES.txt` & `litepcie-2023.8/litepcie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litepcie-2023.4/setup.py` & `litepcie-2023.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(
     name="litepcie",
-    version="2023.04",
+    version="2023.08",
     description="Small footprint and configurable PCIe core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/litepcie",
```

