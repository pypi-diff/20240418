# Comparing `tmp/uniswap_v3_liquidity_pool_simulator-0.3.3.tar.gz` & `tmp/uniswap_v3_liquidity_pool_simulator-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswap_v3_liquidity_pool_simulator-0.3.3.tar", last modified: Tue Apr  9 23:56:31 2024, max compression
+gzip compressed data, was "uniswap_v3_liquidity_pool_simulator-0.3.4.tar", last modified: Thu Apr 18 06:57:09 2024, max compression
```

## Comparing `uniswap_v3_liquidity_pool_simulator-0.3.3.tar` & `uniswap_v3_liquidity_pool_simulator-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-09 23:56:31.357959 uniswap_v3_liquidity_pool_simulator-0.3.3/
--rw-r--r--   0 abauer    (1000) abauer    (1000)     2072 2024-04-09 23:56:31.357959 uniswap_v3_liquidity_pool_simulator-0.3.3/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      254 2024-03-12 17:04:53.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/README.md
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-04-09 23:56:31.357959 uniswap_v3_liquidity_pool_simulator-0.3.3/setup.cfg
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      998 2024-04-09 23:55:27.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/setup.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-09 23:56:31.357959 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator/
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator/__init__.py
--rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator/simulator.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-09 23:56:31.357959 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/
--rw-r--r--   0 abauer    (1000) abauer    (1000)     2072 2024-04-09 23:56:31.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      409 2024-04-09 23:56:31.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-04-09 23:56:31.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      506 2024-04-09 23:56:31.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/requires.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       36 2024-04-09 23:56:31.000000 uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-18 06:57:09.987679 uniswap_v3_liquidity_pool_simulator-0.3.4/
+-rw-r--r--   0 abauer    (1000) abauer    (1000)     4381 2024-04-18 06:57:09.987679 uniswap_v3_liquidity_pool_simulator-0.3.4/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      254 2024-03-12 17:04:53.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/README.md
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-04-18 06:57:09.987679 uniswap_v3_liquidity_pool_simulator-0.3.4/setup.cfg
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      998 2024-04-18 06:53:38.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/setup.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-18 06:57:09.983679 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator/
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator/__init__.py
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator/simulator.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-18 06:57:09.987679 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/
+-rw-r--r--   0 abauer    (1000) abauer    (1000)     4381 2024-04-18 06:57:09.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      409 2024-04-18 06:57:09.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-04-18 06:57:09.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)     1510 2024-04-18 06:57:09.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/requires.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       36 2024-04-18 06:57:09.000000 uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator.egg-info/top_level.txt
```

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.3/setup.py` & `uniswap_v3_liquidity_pool_simulator-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="uniswap_v3_liquidity_pool_simulator",
-    version="0.3.3",
+    version="0.3.4",
     author="the_orthanc_tower",
     author_email="andrbaue@gmail.com",
     description="A simple simulator for Uniswap V3 liquidity pools.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator",
     project_urls={
```

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.3/uniswap_v3_liquidity_pool_simulator/simulator.py` & `uniswap_v3_liquidity_pool_simulator-0.3.4/uniswap_v3_liquidity_pool_simulator/simulator.py`

 * *Files identical despite different names*

