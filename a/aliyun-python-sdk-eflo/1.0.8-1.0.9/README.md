# Comparing `tmp/aliyun-python-sdk-eflo-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-eflo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.8.tar", last modified: Mon Sep  4 02:53:57 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.9.tar", last modified: Mon Sep  4 06:08:48 2023, max compression
```

## Comparing `aliyun-python-sdk-eflo-1.0.8.tar` & `aliyun-python-sdk-eflo-1.0.9.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4086 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/
--rw-r--r--   0 root         (0) root         (0)     2238 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py
--rw-r--r--   0 root         (0) root         (0)     1908 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateElasticNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErRequest.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1316 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteElasticNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetElasticNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListElasticNetworkInterfacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3556 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateElasticNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-09-04 02:53:57.000000 aliyun-python-sdk-eflo-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-09-04 02:53:56.000000 aliyun-python-sdk-eflo-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateElasticNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteElasticNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetElasticNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetNodeInfoForPodRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListElasticNetworkInterfacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListNodeInfosForPodRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateElasticNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-09-04 06:08:48.000000 aliyun-python-sdk-eflo-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-09-04 06:08:47.000000 aliyun-python-sdk-eflo-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.8/LICENSE` & `aliyun-python-sdk-eflo-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.8
+Version: 1.0.9
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.8/README.rst` & `aliyun-python-sdk-eflo-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.8
+Version: 1.0.9
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyun_python_sdk_eflo.egg-info/SOURCES.txt` & `aliyun-python-sdk-eflo-1.0.9/aliyun_python_sdk_eflo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
 aliyunsdkeflo/request/v20220530/GetErRequest.py
 aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py
 aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
 aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
+aliyunsdkeflo/request/v20220530/GetNodeInfoForPodRequest.py
 aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
 aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVccRequest.py
 aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
@@ -52,14 +53,15 @@
 aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
 aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
 aliyunsdkeflo/request/v20220530/ListErsRequest.py
 aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py
 aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
 aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
+aliyunsdkeflo/request/v20220530/ListNodeInfosForPodRequest.py
 aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
 aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
 aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVccsRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateElasticNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateElasticNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteElasticNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteElasticNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetElasticNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetElasticNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListElasticNetworkInterfacesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListElasticNetworkInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListErsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListErsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVccsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVccsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateElasticNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateElasticNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.9/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.8/setup.py` & `aliyun-python-sdk-eflo-1.0.9/setup.py`

 * *Files identical despite different names*

