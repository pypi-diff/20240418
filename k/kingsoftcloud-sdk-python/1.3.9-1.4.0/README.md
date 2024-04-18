# Comparing `tmp/kingsoftcloud-sdk-python-1.3.9.tar.gz` & `tmp/kingsoftcloud_sdk_python-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.3.9.tar", last modified: Fri Apr 12 08:48:38 2024, max compression
+gzip compressed data, was "kingsoftcloud_sdk_python-1.4.0.tar", last modified: Thu Apr 18 09:44:41 2024, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.3.9.tar` & `kingsoftcloud_sdk_python-1.4.0.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 08:48:38.000000 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-12 08:48:38.000000 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:48:38.000000 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 08:48:38.000000 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 08:48:38.000000 kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.481093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20160901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20160901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20160901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20160901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49120 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.485092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26444 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52345 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61057 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.489092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54361 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45896 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28316 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.493093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38868 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53844 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64686 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90642 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   135161 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.497093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/v20240501/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/v20240501/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/v20240501/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/v20240501/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40650 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33045 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.501093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63636 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    82562 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37675 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.505092 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69354 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    92352 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.509093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84131 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    84692 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.513093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 08:48:38.517093 kingsoftcloud-sdk-python-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 08:48:33.000000 kingsoftcloud-sdk-python-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.145148 kingsoftcloud_sdk_python-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 09:44:41.145148 kingsoftcloud_sdk_python-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.145148 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 09:44:41.000000 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-18 09:44:41.000000 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:44:41.000000 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 09:44:41.000000 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 09:44:41.000000 kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.101149 kingsoftcloud_sdk_python-1.4.0/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.101149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.101149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.105149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20160901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20160901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20160901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20160901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49120 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26444 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.109149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52345 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61057 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54361 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45896 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.113149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28316 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.117149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38868 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53844 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64686 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90642 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135161 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.121149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/v20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/v20240501/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/v20240501/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/v20240501/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40650 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33045 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.125149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63636 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82562 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37675 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.129149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.133149 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:35.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69354 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92352 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.137148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84131 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84692 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:41.141148 kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 09:44:41.145148 kingsoftcloud_sdk_python-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 09:44:36.000000 kingsoftcloud_sdk_python-1.4.0/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.3.9/LICENSE` & `kingsoftcloud_sdk_python-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/PKG-INFO` & `kingsoftcloud_sdk_python-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.3.9
+Version: 1.4.0
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 Requires-Dist: requests==2.27.1
 Requires-Dist: requests-aws4auth==1.0.1
 Requires-Dist: six
 
 ============================
 Ksyun Cloud SDK for Python
```

### Comparing `kingsoftcloud-sdk-python-1.3.9/README.rst` & `kingsoftcloud_sdk_python-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.3.9
+Version: 1.4.0
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 Requires-Dist: requests==2.27.1
 Requires-Dist: requests-aws4auth==1.0.1
 Requires-Dist: six
 
 ============================
 Ksyun Cloud SDK for Python
```

### Comparing `kingsoftcloud-sdk-python-1.3.9/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud_sdk_python-1.4.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/__init__.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.3.9'
+__version__ = '1.4.0'
```

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill/v20220601/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill/v20220601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bill_union/v20221222/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bill_union/v20221222/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20160901/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20160901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200630/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200630/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cdn/v20200901/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cdn/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/cen/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/cen/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/clickhouse/v20210101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/clickhouse/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/client/kcm/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/client/kcm/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20180314/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20180314/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20190806/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20190806/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20201231/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20201231/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kce/v20230306/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kce/v20230306/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcm/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcm/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcrs/v20211109/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcrs/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20160701/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20160701/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kcs/v20170401/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kcs/v20170401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kec/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/ket/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/ket/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kingpay/v20240501/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kingpay/v20240501/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kkms/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kkms/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/klog/v20200731/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/klog/v20200731/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/kls/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/kls/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20160701/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20160701/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/krds/v20200825/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/krds/v20200825/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/memcached/v20180627/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/memcached/v20180627/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20100525/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20100525/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20181114/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20181114/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20210101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/monitor/v20220101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/monitor/v20220101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/pdns/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/pdns/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/rabbitmq/v20191017/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/rabbitmq/v20191017/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/tidb/v20210520/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/tidb/v20210520/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/client/waf/v20200707/models.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/client/waf/v20200707/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/abstract_client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/abstract_model.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/common_client.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/credential.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/exception/__init__.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/http/request.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/client_profile.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/ksyun/common/profile/http_profile.py` & `kingsoftcloud_sdk_python-1.4.0/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.3.9/setup.py` & `kingsoftcloud_sdk_python-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,10 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

