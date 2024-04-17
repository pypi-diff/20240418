# Comparing `tmp/synthetix-0.1.7.tar.gz` & `tmp/synthetix-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetix-0.1.7.tar", last modified: Tue Apr 16 21:34:54 2024, max compression
+gzip compressed data, was "synthetix-0.1.8.tar", last modified: Wed Apr 17 22:17:29 2024, max compression
```

## Comparing `synthetix-0.1.7.tar` & `synthetix-0.1.8.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 21:34:41.000000 synthetix-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 21:34:54.297219 synthetix-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-16 21:34:41.000000 synthetix-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:34:54.297219 synthetix-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 21:34:41.000000 synthetix-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/1/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/1/CannonRegistry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/10/
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.289219 synthetix-0.1.7/synthetix/contracts/deployments/420/
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.289219 synthetix-0.1.7/synthetix/contracts/deployments/421614/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/421614/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/contracts/deployments/8453/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/contracts/deployments/84532/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/MintableToken.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/Pyth.json
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/core/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/perps/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/perps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/perps/perps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/pyth/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/spot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/spot/spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/wei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_perps_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_spot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_susd.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 22:17:15.000000 synthetix-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 22:17:29.341613 synthetix-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-17 22:17:15.000000 synthetix-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:17:29.341613 synthetix-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 22:17:15.000000 synthetix-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/contracts/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/1/CannonRegistry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/10/
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/420/
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/421614/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/421614/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.333613 synthetix-0.1.8/synthetix/contracts/deployments/8453/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/contracts/deployments/84532/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/MintableToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/Pyth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/perps/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/perps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37760 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/perps/perps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/pyth/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/spot/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/synthetix/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/wei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/synthetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_perps_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_spot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_susd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_synthetix.py
```

### Comparing `synthetix-0.1.7/PKG-INFO` & `synthetix-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.7
+Version: 0.1.8
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.7/README.md` & `synthetix-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/setup.py` & `synthetix-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="synthetix",
-    version="0.1.7",
+    version="0.1.8",
     description="Synthetix protocol SDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Synthetix DAO",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `synthetix-0.1.7/synthetix/constants.py` & `synthetix-0.1.8/synthetix/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/contracts.py` & `synthetix-0.1.8/synthetix/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/1/CannonRegistry.json` & `synthetix-0.1.8/synthetix/contracts/deployments/1/CannonRegistry.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/10/PerpsV2MarketData.json` & `synthetix-0.1.8/synthetix/contracts/deployments/10/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/10/USDProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/10/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/10/WETH.json` & `synthetix-0.1.8/synthetix/contracts/deployments/10/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/10/sUSD.json` & `synthetix-0.1.8/synthetix/contracts/deployments/10/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/AccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/CoreProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsAccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2Market.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2MarketData.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/SpotMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/USDProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/WETH.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/420/sUSD.json` & `synthetix-0.1.8/synthetix/contracts/deployments/420/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/421614/WETH.json` & `synthetix-0.1.8/synthetix/contracts/deployments/421614/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/AccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/CoreProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsAccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/SpotMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/USDC.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/USDC.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/USDProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/8453/WETH.json` & `synthetix-0.1.8/synthetix/contracts/deployments/8453/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/AccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/CoreProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/MintableToken.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/MintableToken.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsAccountProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/Pyth.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/Pyth.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/SpotMarketProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/USDProxy.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/contracts/deployments/84532/WETH.json` & `synthetix-0.1.8/synthetix/contracts/deployments/84532/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/core/core.py` & `synthetix-0.1.8/synthetix/core/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Module for interacting with Synthetix V3 Core."""
 
 from ..utils import ether_to_wei, wei_to_ether, format_ether
 from ..utils.multicall import call_erc7412, multicall_erc7412, write_erc7412
-import time
-import requests
 
 
 class Core:
     """
     Class for interacting with Synthetix V3 core contracts.
 
     Provides methods for creating accounts, depositing and delegating
@@ -141,18 +139,15 @@
         :rtype: str | dict
         """
         if not account_id:
             tx_args = []
         else:
             tx_args = [account_id]
 
-        tx_params = self.snx._get_tx_params()
-        tx_params = self.core_proxy.functions.createAccount(*tx_args).build_transaction(
-            tx_params
-        )
+        tx_params = write_erc7412(self.snx, self.core_proxy, "createAccount", tx_args)
 
         if submit:
             tx_hash = self.snx.execute_transaction(tx_params)
             self.logger.info(f"Creating account for {self.snx.address}")
             self.logger.info(f"create_account tx: {tx_hash}")
 
             # wait for the transaction, then refetch the ids
@@ -185,18 +180,24 @@
         :rtype: str | dict
         """
         if not account_id:
             account_id = self.default_account_id
 
         amount_wei = format_ether(amount, decimals)
 
-        tx_params = self.snx._get_tx_params()
-        tx_params = self.core_proxy.functions.deposit(
-            account_id, token_address, amount_wei
-        ).build_transaction(tx_params)
+        tx_params = write_erc7412(
+            self.snx,
+            self.core_proxy,
+            "deposit",
+            (
+                account_id,
+                token_address,
+                amount_wei,
+            ),
+        )
 
         if submit:
             tx_hash = self.snx.execute_transaction(tx_params)
             self.logger.info(
                 f"Depositing {amount} {token_address} for account {account_id}"
             )
             self.logger.info(f"deposit tx: {tx_hash}")
```

### Comparing `synthetix-0.1.7/synthetix/perps/perps.py` & `synthetix-0.1.8/synthetix/perps/perps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Module for interacting with Synthetix Perps V3."""
 
 import time
-import requests
 from eth_utils import decode_hex
-from eth_abi import encode
 from ..utils import ether_to_wei, wei_to_ether
 from ..utils.multicall import (
     call_erc7412,
     multicall_erc7412,
     write_erc7412,
     make_fulfillment_request,
 )
```

### Comparing `synthetix-0.1.7/synthetix/pyth/constants.py` & `synthetix-0.1.8/synthetix/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/pyth/pyth.py` & `synthetix-0.1.8/synthetix/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/queries/config.py` & `synthetix-0.1.8/synthetix/queries/config.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/queries/gql.py` & `synthetix-0.1.8/synthetix/queries/gql.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/queries/queries.py` & `synthetix-0.1.8/synthetix/queries/queries.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/spot/spot.py` & `synthetix-0.1.8/synthetix/spot/spot.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/synthetix.py` & `synthetix-0.1.8/synthetix/synthetix.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix/utils/multicall.py` & `synthetix-0.1.8/synthetix/utils/multicall.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import base64
 from web3.exceptions import ContractCustomError
 from web3._utils.abi import get_abi_output_types
 from eth_abi import decode, encode
 from eth_utils import encode_hex, decode_hex
 
+
 # constants
 ORACLE_DATA_REQUIRED = "0xcf2cabdf"
 
 
 def decode_result(contract, function_name, result):
     # get the function abi
     func_abi = contract.get_function_by_name(function_name).abi
@@ -113,16 +114,29 @@
         else:
             snx.logger.error(f"Unknown update type: {update_type}")
             raise error
 
         calls = [(to, True, value, data)] + calls
         return calls
     else:
-        snx.logger.debug(f"Error is not related to oracle data")
-        raise error
+        try:
+            is_nonce_error = (
+                "message" in error.args[0]
+                and "nonce" in error.args[0]["message"].lower()
+            )
+        except:
+            is_nonce_error = False
+
+        if is_nonce_error:
+            snx.logger.debug(f"Error is related to nonce, resetting nonce")
+            snx.nonce = snx.web3.eth.get_transaction_count(snx.address)
+            return calls
+        else:
+            snx.logger.debug(f"Error is not related to oracle data")
+            raise error
 
 
 def write_erc7412(snx, contract, function_name, args, tx_params={}, calls=[]):
     # prepare the initial call
     this_call = [
         (
             contract.address,
```

### Comparing `synthetix-0.1.7/synthetix/utils/wei.py` & `synthetix-0.1.8/synthetix/utils/wei.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/synthetix.egg-info/PKG-INFO` & `synthetix-0.1.8/synthetix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.7
+Version: 0.1.8
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.7/synthetix.egg-info/SOURCES.txt` & `synthetix-0.1.8/synthetix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/tests/test_perps_v3.py` & `synthetix-0.1.8/tests/test_perps_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/tests/test_spot_v3.py` & `synthetix-0.1.8/tests/test_spot_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.7/tests/test_susd.py` & `synthetix-0.1.8/tests/test_susd.py`

 * *Files identical despite different names*

