# Comparing `tmp/pyva-framework-3.1.17.tar.gz` & `tmp/pyva_framework-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva-framework-3.1.17.tar", last modified: Thu Nov 17 19:14:00 2022, max compression
+gzip compressed data, was "pyva_framework-3.3.2.tar", last modified: Thu Apr 18 14:00:47 2024, max compression
```

## Comparing `pyva-framework-3.1.17.tar` & `pyva_framework-3.3.2.tar`

### file list

```diff
@@ -1,58 +1,75 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.433868 pyva-framework-3.1.17/
--rw-rw-rw-   0        0        0     1091 2022-10-07 14:30:16.000000 pyva-framework-3.1.17/LICENSE
--rw-rw-rw-   0        0        0     1921 2022-11-17 19:14:00.433868 pyva-framework-3.1.17/PKG-INFO
--rw-rw-rw-   0        0        0     1328 2022-10-07 14:37:18.000000 pyva-framework-3.1.17/README.md
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.327345 pyva-framework-3.1.17/pyva/
--rw-rw-rw-   0        0        0      897 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/Global.py
--rw-rw-rw-   0        0        0        0 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.329345 pyva-framework-3.1.17/pyva/client/
--rw-rw-rw-   0        0        0       24 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/client/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.339346 pyva-framework-3.1.17/pyva/client/dingtalk/
--rw-rw-rw-   0        0        0     2653 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/client/dingtalk/DingtalkContactClient.py
--rw-rw-rw-   0        0        0     3350 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/client/dingtalk/DingtalkOauth2Client.py
--rw-rw-rw-   0        0        0     5712 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/client/dingtalk/DingtalkYidaClient.py
--rw-rw-rw-   0        0        0       34 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/client/dingtalk/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.362346 pyva-framework-3.1.17/pyva/config/
--rw-rw-rw-   0        0        0      788 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/AppConfig.py
--rw-rw-rw-   0        0        0      934 2022-11-17 15:35:52.000000 pyva-framework-3.1.17/pyva/config/DbConfig.py
--rw-rw-rw-   0        0        0      547 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/DingtalkConfig.py
--rw-rw-rw-   0        0        0      586 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/FastapiConfig.py
--rw-rw-rw-   0        0        0     3645 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/LoggingConfig.py
--rw-rw-rw-   0        0        0      226 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/MongoConfig.py
--rw-rw-rw-   0        0        0      874 2022-11-17 19:06:27.000000 pyva-framework-3.1.17/pyva/config/NacosConfig.py
--rw-rw-rw-   0        0        0      413 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/RedisConfig.py
--rw-rw-rw-   0        0        0       24 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/config/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.369873 pyva-framework-3.1.17/pyva/dao/
--rw-rw-rw-   0        0        0     1331 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/dao/BaseDao.py
--rw-rw-rw-   0        0        0     6114 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/dao/ListDao.py
--rw-rw-rw-   0        0        0       21 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/dao/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.377971 pyva-framework-3.1.17/pyva/dto/
--rw-rw-rw-   0        0        0     1425 2022-11-11 11:13:59.000000 pyva-framework-3.1.17/pyva/dto/BaseDto.py
--rw-rw-rw-   0        0        0     1444 2022-11-11 11:04:05.000000 pyva-framework-3.1.17/pyva/dto/ListDto.py
--rw-rw-rw-   0        0        0       21 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/dto/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.388867 pyva-framework-3.1.17/pyva/entity/
--rw-rw-rw-   0        0        0     1116 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/entity/BaseEntity.py
--rw-rw-rw-   0        0        0     1094 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/entity/GeneralHumpEntity.py
--rw-rw-rw-   0        0        0      460 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/entity/HumpEntity.py
--rw-rw-rw-   0        0        0        0 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.419871 pyva-framework-3.1.17/pyva/util/
--rw-rw-rw-   0        0        0     1586 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/AlipayUtil.py
--rw-rw-rw-   0        0        0     8707 2022-11-07 12:27:14.000000 pyva-framework-3.1.17/pyva/util/DbUtil.py
--rw-rw-rw-   0        0        0     1056 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/EntityUtil.py
--rw-rw-rw-   0        0        0      282 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/IpUtil.py
--rw-rw-rw-   0        0        0      627 2022-11-07 04:43:23.000000 pyva-framework-3.1.17/pyva/util/JsonUtil.py
--rw-rw-rw-   0        0        0      597 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/LockerUtil.py
--rw-rw-rw-   0        0        0     2061 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/MongoUtil.py
--rw-rw-rw-   0        0        0     6196 2022-11-17 19:09:24.000000 pyva-framework-3.1.17/pyva/util/NacosUtil.py
--rw-rw-rw-   0        0        0     4273 2022-11-17 19:12:51.000000 pyva-framework-3.1.17/pyva/util/QrcodeUtil.py
--rw-rw-rw-   0        0        0     2266 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/RedisUtil.py
--rw-rw-rw-   0        0        0      973 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/TimeUtil.py
--rw-rw-rw-   0        0        0       24 2022-11-03 06:18:41.000000 pyva-framework-3.1.17/pyva/util/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:00.431871 pyva-framework-3.1.17/pyva_framework.egg-info/
--rw-rw-rw-   0        0        0     1921 2022-11-17 19:14:00.000000 pyva-framework-3.1.17/pyva_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2022-11-17 19:14:00.000000 pyva-framework-3.1.17/pyva_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 19:14:00.000000 pyva-framework-3.1.17/pyva_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2022-11-17 19:14:00.000000 pyva-framework-3.1.17/pyva_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-11-17 19:14:00.000000 pyva-framework-3.1.17/pyva_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-17 19:14:00.434868 pyva-framework-3.1.17/setup.cfg
--rw-rw-rw-   0        0        0      978 2022-11-17 19:13:07.000000 pyva-framework-3.1.17/setup.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.226403 pyva_framework-3.3.2/
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/LICENSE
+-rw-r--r--   0 szq        (501) staff       (20)     2417 2024-04-18 14:00:47.225611 pyva_framework-3.3.2/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1303 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/README.md
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.177483 pyva_framework-3.3.2/pyva/
+-rw-r--r--   0 szq        (501) staff       (20)     1455 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/Application.py
+-rw-r--r--   0 szq        (501) staff       (20)      708 2023-11-28 12:16:55.000000 pyva_framework-3.3.2/pyva/Global.py
+-rw-r--r--   0 szq        (501) staff       (20)     1010 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/GlobalInit.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.179100 pyva_framework-3.3.2/pyva/cli/
+-rw-r--r--   0 szq        (501) staff       (20)       18 2023-11-26 01:27:02.000000 pyva_framework-3.3.2/pyva/cli/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1464 2023-11-26 11:30:11.000000 pyva_framework-3.3.2/pyva/cli/main.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.180205 pyva_framework-3.3.2/pyva/client/
+-rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.184832 pyva_framework-3.3.2/pyva/client/dingtalk/
+-rw-r--r--   0 szq        (501) staff       (20)     2563 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkContactClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     3239 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkOauth2Client.py
+-rw-r--r--   0 szq        (501) staff       (20)     6758 2023-11-28 14:43:59.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkRobotClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     5526 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkYidaClient.py
+-rw-r--r--   0 szq        (501) staff       (20)       31 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.187862 pyva_framework-3.3.2/pyva/common/
+-rw-r--r--   0 szq        (501) staff       (20)      999 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/FastapiEvents.py
+-rw-r--r--   0 szq        (501) staff       (20)     1911 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/FastapiException.py
+-rw-r--r--   0 szq        (501) staff       (20)     1229 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/LoggerHandler.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/common/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.195212 pyva_framework-3.3.2/pyva/config/
+-rw-r--r--   0 szq        (501) staff       (20)      963 2023-11-26 17:09:44.000000 pyva_framework-3.3.2/pyva/config/AppConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      893 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/config/DbConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      525 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/DingtalkConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      128 2023-11-28 14:45:03.000000 pyva_framework-3.3.2/pyva/config/DingtalkRobotConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      729 2023-11-26 17:08:07.000000 pyva_framework-3.3.2/pyva/config/FastapiConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)     3524 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/LoggingConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       88 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/config/MongoConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      894 2023-11-28 10:52:03.000000 pyva_framework-3.3.2/pyva/config/NacosConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      392 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/RedisConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2023-11-28 08:22:32.000000 pyva_framework-3.3.2/pyva/config/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.198005 pyva_framework-3.3.2/pyva/dao/
+-rw-r--r--   0 szq        (501) staff       (20)     1401 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/dao/BaseDao.py
+-rw-r--r--   0 szq        (501) staff       (20)     5952 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dao/ListDao.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dao/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.200779 pyva_framework-3.3.2/pyva/dto/
+-rw-r--r--   0 szq        (501) staff       (20)     1360 2023-11-26 13:59:29.000000 pyva_framework-3.3.2/pyva/dto/BaseDto.py
+-rw-r--r--   0 szq        (501) staff       (20)     1395 2023-11-22 14:07:26.000000 pyva_framework-3.3.2/pyva/dto/ListDto.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dto/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.204362 pyva_framework-3.3.2/pyva/entity/
+-rw-r--r--   0 szq        (501) staff       (20)     1190 2023-11-26 13:33:29.000000 pyva_framework-3.3.2/pyva/entity/BaseEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2023-11-26 13:27:10.000000 pyva_framework-3.3.2/pyva/entity/GeneralHumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)      441 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/entity/HumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/entity/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1047 2024-04-17 13:46:37.000000 pyva_framework-3.3.2/pyva/startupApp.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.218524 pyva_framework-3.3.2/pyva/util/
+-rw-r--r--   0 szq        (501) staff       (20)     5269 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/util/ConfigUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     9245 2023-11-29 07:09:53.000000 pyva_framework-3.3.2/pyva/util/DbUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)      581 2023-11-27 15:58:15.000000 pyva_framework-3.3.2/pyva/util/DictUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2780 2023-11-21 10:17:20.000000 pyva_framework-3.3.2/pyva/util/EntityUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1081 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/util/FileUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1807 2023-11-22 13:57:36.000000 pyva_framework-3.3.2/pyva/util/IpUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2006 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/JsonUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2034 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/LockerUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1985 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/MongoUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6692 2023-11-28 13:44:28.000000 pyva_framework-3.3.2/pyva/util/NacosUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1608 2023-11-26 15:13:28.000000 pyva_framework-3.3.2/pyva/util/PathUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4136 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/QrcodeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2180 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/RedisUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6613 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/TimeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.224640 pyva_framework-3.3.2/pyva_framework.egg-info/
+-rw-r--r--   0 szq        (501) staff       (20)     2417 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1578 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 szq        (501) staff       (20)        1 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 szq        (501) staff       (20)       43 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/entry_points.txt
+-rw-r--r--   0 szq        (501) staff       (20)      306 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/requires.txt
+-rw-r--r--   0 szq        (501) staff       (20)        5 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/top_level.txt
+-rw-r--r--   0 szq        (501) staff       (20)       38 2024-04-18 14:00:47.226549 pyva_framework-3.3.2/setup.cfg
+-rw-r--r--   0 szq        (501) staff       (20)     1092 2024-04-17 14:40:02.000000 pyva_framework-3.3.2/setup.py
```

### Comparing `pyva-framework-3.1.17/LICENSE` & `pyva_framework-3.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pyva-framework-3.1.17/README.md` & `pyva_framework-3.3.2/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# PyVa
-PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
-
-[Github: PyVa](https://github.com/zhenqiang-sun/pyva)
-
-### 依赖组件：
-
-#### 1、FastAPI
-https://fastapi.tiangolo.com/
-* 快速：可与 NodeJS 和 Go 比肩的极高性能（归功于 Starlette 和 Pydantic）。最快的 Python web 框架之一。
-* 高效编码：提高功能开发速度约 200％ 至 300％。*
-* 更少 bug：减少约 40％ 的人为（开发者）导致错误。*
-* 智能：极佳的编辑器支持。处处皆可自动补全，减少调试时间。
-* 简单：设计的易于使用和学习，阅读文档的时间更短。
-* 简短：使代码重复最小化。通过不同的参数声明实现丰富功能。bug 更少。
-* 健壮：生产可用级别的代码。还有自动生成的交互式文档。
-* 标准化：基于（并完全兼容）API 的相关开放标准：OpenAPI (以前被称为 Swagger) 和 JSON Schema。
-
-#### 2、Uvicorn
-https://www.uvicorn.org/
-基于 Uvicorn 运行的 FastAPI 程序是 最快的 Python web 框架之一。
-
-#### 3、SQLAlchemy
-SQLAlchemy: https://www.sqlalchemy.org/
-采用简单的Python语言，为高效和高性能的数据库访问设计，实现了完整的企业级持久模型”。
+# PyVa
+PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
+
+[Github: PyVa](https://github.com/zhenqiang-sun/pyva)
+
+### 依赖组件：
+
+#### 1、FastAPI
+https://fastapi.tiangolo.com/
+* 快速：可与 NodeJS 和 Go 比肩的极高性能（归功于 Starlette 和 Pydantic）。最快的 Python web 框架之一。
+* 高效编码：提高功能开发速度约 200％ 至 300％。*
+* 更少 bug：减少约 40％ 的人为（开发者）导致错误。*
+* 智能：极佳的编辑器支持。处处皆可自动补全，减少调试时间。
+* 简单：设计的易于使用和学习，阅读文档的时间更短。
+* 简短：使代码重复最小化。通过不同的参数声明实现丰富功能。bug 更少。
+* 健壮：生产可用级别的代码。还有自动生成的交互式文档。
+* 标准化：基于（并完全兼容）API 的相关开放标准：OpenAPI (以前被称为 Swagger) 和 JSON Schema。
+
+#### 2、Uvicorn
+https://www.uvicorn.org/
+基于 Uvicorn 运行的 FastAPI 程序是 最快的 Python web 框架之一。
+
+#### 3、SQLAlchemy
+SQLAlchemy: https://www.sqlalchemy.org/
+采用简单的Python语言，为高效和高性能的数据库访问设计，实现了完整的企业级持久模型”。
```

### Comparing `pyva-framework-3.1.17/pyva/client/dingtalk/DingtalkContactClient.py` & `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkContactClient.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import logging
-
-from pyva.client.dingtalk.DingtalkOauth2Client import DingtalkOauth2Client
-from pyva.config.DingtalkConfig import DingtalkConfig
-
-logger = logging.getLogger('dingtalk')
-
-
-class DingtalkContactClient:
-    """
-    钉钉通讯录Client
-    """
-
-    def __init__(self, dingtalkConfig: DingtalkConfig):
-        self.dingtalkConfig = dingtalkConfig
-        self.oauth = DingtalkOauth2Client(dingtalkConfig)
-
-    def getDepartmentList(self, departmentId: int = None):
-        """
-        获取部门列表
-
-        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.v2.department.listsub
-        """
-
-        url = "https://oapi.dingtalk.com/topapi/v2/department/listsub?access_token={token}"
-        body = {
-            "dept_id": departmentId
-        }
-
-        data = self.oauth.post(url=url, json=body)
-
-        if data.get("errcode", -1) == 0:
-            return data.get("result", [])
-        else:
-            logger.error(url)
-            logger.error(body)
-            logger.error(data)
-            return None
-
-    def getDepartmentUserList(self, departmentId: int = None, cursor: int = 0, size: int = 100):
-        """
-        获取部门用户基础信息
-
-        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.user.listsimple
-        :param departmentId 部门ID
-        :param cursor 分页查询的游标
-        :param size 分页长度
-        """
-
-        url = "https://oapi.dingtalk.com/topapi/user/listsimple?access_token={token}"
-
-        body = {
-            "dept_id": departmentId,
-            "cursor": cursor,
-            "size": size
-        }
-
-        data = self.oauth.post(url=url, json=body)
-
-        if data.get("errcode", -1) == 0:
-            return data.get("result", {}).get("list", [])
-        else:
-            logger.error(url)
-            logger.error(body)
-            logger.error(data)
-            return None
-
-    def getUser(self, userId: int) -> dict:
-        """
-        查询用户详情
-
-        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.v2.user.get
-        :param userId 用户ID
-        """
-
-        url = "https://oapi.dingtalk.com/topapi/v2/user/get?access_token={token}"
-
-        body = {
-            "userid": userId,
-        }
-
-        data = self.oauth.post(url=url, json=body)
-
-        if data.get("errcode", -1) == 0:
-            return data.get("result", {})
-        else:
-            logger.error(url)
-            logger.error(body)
-            logger.error(data)
-            return None
+import logging
+
+from pyva.client.dingtalk.DingtalkOauth2Client import DingtalkOauth2Client
+from pyva.config.DingtalkConfig import DingtalkConfig
+
+logger = logging.getLogger('dingtalk')
+
+
+class DingtalkContactClient:
+    """
+    钉钉通讯录Client
+    """
+
+    def __init__(self, dingtalkConfig: DingtalkConfig):
+        self.dingtalkConfig = dingtalkConfig
+        self.oauth = DingtalkOauth2Client(dingtalkConfig)
+
+    def getDepartmentList(self, departmentId: int = None):
+        """
+        获取部门列表
+
+        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.v2.department.listsub
+        """
+
+        url = "https://oapi.dingtalk.com/topapi/v2/department/listsub?access_token={token}"
+        body = {
+            "dept_id": departmentId
+        }
+
+        data = self.oauth.post(url=url, json=body)
+
+        if data.get("errcode", -1) == 0:
+            return data.get("result", [])
+        else:
+            logger.error(url)
+            logger.error(body)
+            logger.error(data)
+            return None
+
+    def getDepartmentUserList(self, departmentId: int = None, cursor: int = 0, size: int = 100):
+        """
+        获取部门用户基础信息
+
+        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.user.listsimple
+        :param departmentId 部门ID
+        :param cursor 分页查询的游标
+        :param size 分页长度
+        """
+
+        url = "https://oapi.dingtalk.com/topapi/user/listsimple?access_token={token}"
+
+        body = {
+            "dept_id": departmentId,
+            "cursor": cursor,
+            "size": size
+        }
+
+        data = self.oauth.post(url=url, json=body)
+
+        if data.get("errcode", -1) == 0:
+            return data.get("result", {}).get("list", [])
+        else:
+            logger.error(url)
+            logger.error(body)
+            logger.error(data)
+            return None
+
+    def getUser(self, userId: int) -> dict:
+        """
+        查询用户详情
+
+        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=dingtalk.oapi.v2.user.get
+        :param userId 用户ID
+        """
+
+        url = "https://oapi.dingtalk.com/topapi/v2/user/get?access_token={token}"
+
+        body = {
+            "userid": userId,
+        }
+
+        data = self.oauth.post(url=url, json=body)
+
+        if data.get("errcode", -1) == 0:
+            return data.get("result", {})
+        else:
+            logger.error(url)
+            logger.error(body)
+            logger.error(data)
+            return None
```

### Comparing `pyva-framework-3.1.17/pyva/client/dingtalk/DingtalkOauth2Client.py` & `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkOauth2Client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import logging
-import time
-
-import requests
-
-from pyva.config.DingtalkConfig import DingtalkConfig
-
-logger = logging.getLogger('dingtalk')
-
-
-class DingtalkOauth2Client:
-    """
-    钉钉授权Client
-    """
-
-    class Token:
-        """
-        Token对象
-        """
-        expireTime = 0.0
-        accessToken = ""
-
-    # token过期时间
-    expireIn: int = 7200
-    # token池
-    tokenMap: dict = {}
-    # 当前token
-    token: Token = None
-
-    def __init__(self, dingtalkConfig: DingtalkConfig):
-        self.getAccessToken(dingtalkConfig)
-        self.token = DingtalkOauth2Client.tokenMap.get(dingtalkConfig.appKey)
-
-    @staticmethod
-    def getAccessTokenByApi(dingtalkConfig: DingtalkConfig):
-        """
-        获取AccessToken通过Api
-
-        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=oauth2_1.0%23GetAccessToken
-        """
-
-        url = "https://api.dingtalk.com/v1.0/oauth2/accessToken"
-        body = {
-            "appKey": dingtalkConfig.appKey,
-            "appSecret": dingtalkConfig.appSecret
-        }
-        resp = requests.post(url=url, json=body)
-
-        if resp.status_code == 200:
-            return resp.json()
-        else:
-            logger.error(url)
-            logger.error(body)
-            logger.error(resp.text)
-            return resp.json()
-
-    @staticmethod
-    def getAccessToken(dingtalkConfig: DingtalkConfig):
-        """
-        获取AccessToken优先缓存
-        """
-
-        token: DingtalkOauth2Client.Token = DingtalkOauth2Client.tokenMap.get(dingtalkConfig.appKey)
-
-        if token and token.accessToken and token.expireTime > time.time():
-            return token.accessToken
-
-        resp = DingtalkOauth2Client.getAccessTokenByApi(dingtalkConfig)
-
-        token = DingtalkOauth2Client.Token()
-        token.accessToken = resp.get("accessToken", "")
-        token.expireIn = resp.get("expireIn", 0)
-        token.expireTime = time.time() + DingtalkOauth2Client.expireIn
-
-        DingtalkOauth2Client.tokenMap[dingtalkConfig.appKey] = token
-
-        return token.accessToken
-
-    def request(self, method: str, url: str, headers: dict = None, **kwargs):
-        if headers is None:
-            headers = {}
-
-        url = url.format(token=self.token.accessToken)
-        headers["x-acs-dingtalk-access-token"] = self.token.accessToken
-
-        resp = requests.request(method=method, url=url, headers=headers, **kwargs)
-
-        if resp.status_code == 200:
-            return resp.json()
-        else:
-            logger.error(resp.text)
-
-            try:
-                return resp.json()
-            except:
-                return None
-
-    def get(self, url: str, header: dict = None, **kwargs):
-        return self.request("get", url, header, **kwargs)
-
-    def post(self, url: str, header: dict = None, **kwargs):
-        return self.request("post", url, header, **kwargs)
-
-    def put(self, url: str, header: dict = None, **kwargs):
-        return self.request("put", url, header, **kwargs)
-
-    def patch(self, url: str, header: dict = None, **kwargs):
-        return self.request("patch", url, header, **kwargs)
-
-    def delete(self, url: str, header: dict = None, **kwargs):
-        return self.request("delete", url, header, **kwargs)
+import logging
+import time
+
+import requests
+
+from pyva.config.DingtalkConfig import DingtalkConfig
+
+logger = logging.getLogger('dingtalk')
+
+
+class DingtalkOauth2Client:
+    """
+    钉钉授权Client
+    """
+
+    class Token:
+        """
+        Token对象
+        """
+        expireTime = 0.0
+        accessToken = ""
+
+    # token过期时间
+    expireIn: int = 7200
+    # token池
+    tokenMap: dict = {}
+    # 当前token
+    token: Token = None
+
+    def __init__(self, dingtalkConfig: DingtalkConfig):
+        self.getAccessToken(dingtalkConfig)
+        self.token = DingtalkOauth2Client.tokenMap.get(dingtalkConfig.appKey)
+
+    @staticmethod
+    def getAccessTokenByApi(dingtalkConfig: DingtalkConfig):
+        """
+        获取AccessToken通过Api
+
+        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=oauth2_1.0%23GetAccessToken
+        """
+
+        url = "https://api.dingtalk.com/v1.0/oauth2/accessToken"
+        body = {
+            "appKey": dingtalkConfig.appKey,
+            "appSecret": dingtalkConfig.appSecret
+        }
+        resp = requests.post(url=url, json=body)
+
+        if resp.status_code == 200:
+            return resp.json()
+        else:
+            logger.error(url)
+            logger.error(body)
+            logger.error(resp.text)
+            return resp.json()
+
+    @staticmethod
+    def getAccessToken(dingtalkConfig: DingtalkConfig):
+        """
+        获取AccessToken优先缓存
+        """
+
+        token: DingtalkOauth2Client.Token = DingtalkOauth2Client.tokenMap.get(dingtalkConfig.appKey)
+
+        if token and token.accessToken and token.expireTime > time.time():
+            return token.accessToken
+
+        resp = DingtalkOauth2Client.getAccessTokenByApi(dingtalkConfig)
+
+        token = DingtalkOauth2Client.Token()
+        token.accessToken = resp.get("accessToken", "")
+        token.expireIn = resp.get("expireIn", 0)
+        token.expireTime = time.time() + DingtalkOauth2Client.expireIn
+
+        DingtalkOauth2Client.tokenMap[dingtalkConfig.appKey] = token
+
+        return token.accessToken
+
+    def request(self, method: str, url: str, headers: dict = None, **kwargs):
+        if headers is None:
+            headers = {}
+
+        url = url.format(token=self.token.accessToken)
+        headers["x-acs-dingtalk-access-token"] = self.token.accessToken
+
+        resp = requests.request(method=method, url=url, headers=headers, **kwargs)
+
+        if resp.status_code == 200:
+            return resp.json()
+        else:
+            logger.error(resp.text)
+
+            try:
+                return resp.json()
+            except:
+                return None
+
+    def get(self, url: str, header: dict = None, **kwargs):
+        return self.request("get", url, header, **kwargs)
+
+    def post(self, url: str, header: dict = None, **kwargs):
+        return self.request("post", url, header, **kwargs)
+
+    def put(self, url: str, header: dict = None, **kwargs):
+        return self.request("put", url, header, **kwargs)
+
+    def patch(self, url: str, header: dict = None, **kwargs):
+        return self.request("patch", url, header, **kwargs)
+
+    def delete(self, url: str, header: dict = None, **kwargs):
+        return self.request("delete", url, header, **kwargs)
```

### Comparing `pyva-framework-3.1.17/pyva/config/DbConfig.py` & `pyva_framework-3.3.2/pyva/config/DbConfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-class DbConfig:
-    """
-    pyva DbConfig DB配置类
-
-    :version: 1.5
-    :createdDate: 2020-02-11
-    :updatedDate: 2022-10-03
-    """
-
-    # 驱动，默认mysql
-    driver: str = "mysql+pymysql"
-    # 主机
-    host: str = "localhost"
-    # 端口
-    port: int = 3306
-    # 账号
-    username: str = "root"
-    # 密码
-    password: str = ""
-    # 数据库
-    database: str = ""
-    # 字符集
-    charset: str = "utf8mb4"
-    # 表前缀
-    prefix: str = ""
-    # 是否输出
-    echo: bool = False
-    # 最大连接
-    maxOverflow: int = 100
-    # 连接池大小
-    poolSize: int = 100
-    # 回收时间
-    poolRecycle: int = 3600
-    # 回收时间
-    poolPrePing: bool = True
-    # 自动flush
-    autoFlush: bool = False
-    # 自动提交
-    autoCommit: bool = True
-    # 过期提交
-    expireOnCommit: bool = True
-    # 其他配置
-    otherParam: dict = {}
+class DbConfig:
+    """
+    pyva DbConfig DB配置类
+
+    :version: 1.5
+    :createdDate: 2020-02-11
+    :updatedDate: 2022-10-03
+    """
+
+    # 驱动，默认mysql
+    driver: str = "mysql+pymysql"
+    # 主机
+    host: str = "localhost"
+    # 端口
+    port: int = 3306
+    # 账号
+    username: str = "root"
+    # 密码
+    password: str = ""
+    # 数据库
+    database: str = ""
+    # 字符集
+    charset: str = "utf8mb4"
+    # 表前缀
+    prefix: str = ""
+    # 是否输出
+    echo: bool = False
+    # 最大连接
+    maxOverflow: int = 100
+    # 连接池大小
+    poolSize: int = 100
+    # 回收时间
+    poolRecycle: int = 3600
+    # 回收时间
+    poolPrePing: bool = True
+    # 自动flush
+    autoFlush: bool = False
+    # 自动提交
+    autoCommit: bool = False
+    # 过期提交
+    expireOnCommit: bool = False
+    # 其他配置
+    otherParam: dict = {}
```

### Comparing `pyva-framework-3.1.17/pyva/dao/BaseDao.py` & `pyva_framework-3.3.2/pyva/dao/BaseDao.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,68 @@
-from sqlalchemy.orm import Session
-
-from pyva.Global import G
-
-
-class BaseDao:
-    """
-    Base(基础)Dao，用于被继承.
-
-    CRUD基础Dao类，拥有基本方法，可直接继承使用
-    """
-
-    # 数据库连接session
-    db: Session = None
-    # 实体对象
-    Entity = None
-
-    def __init__(self, db: Session = None):
-        if db:
-            self.db = db
-        else:
-            self.db = G.db
-
-    def create(self, entity):
-        """
-        创建一条数据
-        :param entity: 数据模型实例
-        """
-        self.db.add(entity)
-        # self.db.commit()
-        self.db.flush()
-
-        return entity.id
-
-    def read(self, id: int):
-        """
-        读取一条数据
-        :param id: 数据id
-        :return: 数据模型实例
-        """
-
-        return self.db.query(self.Entity).get(id)
-
-    def update(self, entity):
-        """
-        更新一条数据
-        :param entity: 数据模型实例
-        :return:
-        """
-
-        self.db.add(entity)
-        # self.db.commit()
-        self.db.flush()
-
-    def delete(self, entity):
-        """
-        删除一条数据
-        :param entity: 数据模型实体
-        """
-        self.db.delete(entity)
-        # self.db.commit()
-        self.db.flush()
+from sqlalchemy.orm import Session
+
+from pyva.Global import G
+
+
+class BaseDao:
+    """
+    Base(基础)Dao，用于被继承.
+
+    CRUD基础Dao类，拥有基本方法，可直接继承使用
+    """
+
+    # 数据库连接session
+    db: Session = None
+    # 实体对象
+    Entity = None
+
+    def __init__(self, db: Session = None):
+        if db:
+            self.db = db
+        else:
+            self.db = G.db
+
+    def create(self, entity, commit: bool = True):
+        """
+        创建一条数据
+        @param entity: 数据模型实例
+        @param commit:
+        """
+        self.db.add(entity)
+
+        if commit:
+            self.db.commit()
+
+        return entity.id
+
+    def read(self, id: int | str):
+        """
+        读取一条数据
+        :param id: 数据id
+        :return: 数据模型实例
+        """
+
+        return self.db.query(self.Entity).get(id)
+
+    def update(self, entity, commit: bool = True):
+        """
+        更新一条数据
+        @param entity: 数据模型实例
+        @param commit:
+        :return:
+        """
+
+        self.db.add(entity)
+
+        if commit:
+            self.db.commit()
+
+    def delete(self, entity, commit: bool = True):
+        """
+        删除一条数据
+        @param entity: 数据模型实例
+        @param commit:
+        """
+        self.db.delete(entity)
+
+        if commit:
+            self.db.commit()
```

### Comparing `pyva-framework-3.1.17/pyva/dto/BaseDto.py` & `pyva_framework-3.3.2/pyva/dto/BaseDto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from typing import List, Dict, TypeVar
-
-from pydantic import BaseModel, Field
-
-from pyva.util.JsonUtil import JsonUtil
-
-DataT = TypeVar("DataT")
-
-
-class BaseDto(BaseModel):
-    """
-    基础DTO
-    """
-
-    class Config:
-        json_encoders = JsonUtil.jsonEncoders  # 使用自定义json转换
-
-
-class BaseEntityDto(BaseModel):
-    """
-    基础Entity DTO
-    """
-
-    class Config:
-        json_encoders = JsonUtil.jsonEncoders
-        orm_mode = True  # 为模型实例
-
-
-class RespDto(BaseDto):
-    """
-    基础返回DTO
-    """
-    code: int = Field(..., gt=0, description='返回码')
-    message: str = Field(..., description='返回说明')
-
-
-class SuccessRespDto(RespDto):
-    """
-    成功响应DTO
-    """
-    code: int = 10000
-    message: str = "SUCCESS"
-
-
-class FailRespDto(RespDto):
-    """
-    失败响应DTO
-    """
-    code: int = 19999
-    message: str = "FAIL"
-
-
-class RespIdDto(SuccessRespDto):
-    """
-    ID返回DTO
-    """
-    id: int = Field(..., gt=0, description='数据ID')
-
-
-class RespDataDto(SuccessRespDto):
-    """
-    Data返回DTO
-    """
-    data: dict = None  # 返回Data
-
-
-class RespDetailDto(SuccessRespDto):
-    """
-    详情返回DTO
-    """
-    detail: dict = None  # 返回详情
-
-
-class RespListDto(SuccessRespDto):
-    """
-    列表返回DTO
-    """
-    list: List[Dict] = None  # 数据list
+from typing import List, Dict, TypeVar
+
+from pydantic import BaseModel, Field
+
+from pyva.util.JsonUtil import JsonUtil
+
+DataT = TypeVar("DataT")
+
+
+class BaseDto(BaseModel):
+    """
+    基础DTO
+    """
+
+    class Config:
+        json_encoders = JsonUtil.jsonEncoders  # 使用自定义json转换
+
+
+class BaseEntityDto(BaseModel):
+    """
+    基础Entity DTO
+    """
+
+    class Config:
+        json_encoders = JsonUtil.jsonEncoders
+        from_attributes = True  # 为模型实例
+
+
+class RespDto(BaseDto):
+    """
+    基础返回DTO
+    """
+    code: int = Field(..., gt=0, description='返回码')
+    message: str = Field(..., description='返回说明')
+
+
+class SuccessRespDto(RespDto):
+    """
+    成功响应DTO
+    """
+    code: int = 10000
+    message: str = "SUCCESS"
+
+
+class FailRespDto(RespDto):
+    """
+    失败响应DTO
+    """
+    code: int = 19999
+    message: str = "FAIL"
+
+
+class RespIdDto(SuccessRespDto):
+    """
+    ID返回DTO
+    """
+    id: int | str = Field(..., gt=0, description='数据ID')
+
+
+class RespDataDto(SuccessRespDto):
+    """
+    Data返回DTO
+    """
+    data: dict = None  # 返回Data
+
+
+class RespDetailDto(SuccessRespDto):
+    """
+    详情返回DTO
+    """
+    detail: dict = None  # 返回详情
+
+
+class RespListDto(SuccessRespDto):
+    """
+    列表返回DTO
+    """
+    list: List[Dict] = None  # 数据list
```

### Comparing `pyva-framework-3.1.17/pyva/dto/ListDto.py` & `pyva_framework-3.3.2/pyva/dto/ListDto.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import List
-
-from pydantic import BaseModel
-
-from pyva.dto.BaseDto import BaseEntityDto, DataT
-
-
-class ListFilterDto(BaseModel):
-    """
-    列表参数：过滤条件Schema
-    """
-    key: str  # 字段名
-    condition: str  # 条件
-    value: DataT  # 条件值，如condition为in或!in时，value为用“,”分割的多值得字符串
-
-
-class ListOrderDto(BaseModel):
-    """
-    列表参数：排序条件Schema
-    """
-    key: str  # 字段名
-    condition: str  # 排序条件
-
-
-class ListKeyDto(BaseModel):
-    """
-    列表参数：字段条件Schema
-    """
-    key: str  # 字段名
-    rename: str = None  # 字段名重命名, 为空则不进行重命名
-
-
-class ListReqDto(BaseModel):
-    """
-    列表参数Schema
-    """
-    page: int = 1  # 当前页码
-    size: int = 10  # 每页条数
-    keywords: str = None  # 关键字，用于模糊、分词搜索
-    deleted: str = None
-    userId: int = None  # 数据对应用户id
-    filters: List[ListFilterDto] = None  # 过滤条件
-    orders: List[ListOrderDto] = None  # 排序条件
-    keys: List[ListKeyDto] = None  # 字段条件
-
-
-class ListPageDto(BaseModel):
-    """
-    列表返回DTO
-    """
-    page: int = 0  # 当前页码
-    size: int = 0  # 每页大小
-    count: int = 0  # 数据总条数
-    pageCount: int = 0  # 总页数
-    list: List[BaseEntityDto] = None  # 数据list
+from typing import List
+
+from pydantic import BaseModel
+
+from pyva.dto.BaseDto import BaseEntityDto, DataT
+
+
+class ListFilterDto(BaseModel):
+    """
+    列表参数：过滤条件Schema
+    """
+    key: str  # 字段名
+    condition: str  # 条件
+    value: DataT  # 条件值，如condition为in或!in时，value为用“,”分割的多值得字符串
+
+
+class ListOrderDto(BaseModel):
+    """
+    列表参数：排序条件Schema
+    """
+    key: str  # 字段名
+    condition: str  # 排序条件
+
+
+class ListKeyDto(BaseModel):
+    """
+    列表参数：字段条件Schema
+    """
+    key: str  # 字段名
+    rename: str = None  # 字段名重命名, 为空则不进行重命名
+
+
+class ListReqDto(BaseModel):
+    """
+    列表参数Schema
+    """
+    page: int = 1  # 当前页码
+    size: int = 10  # 每页条数
+    keywords: str = None  # 关键字，用于模糊、分词搜索
+    deleted: str = None
+    userId: int | str = None  # 数据对应用户id
+    filters: List[ListFilterDto] = None  # 过滤条件
+    orders: List[ListOrderDto] = None  # 排序条件
+    keys: List[ListKeyDto] = None  # 字段条件
+
+
+class ListPageDto(BaseModel):
+    """
+    列表返回DTO
+    """
+    page: int = 0  # 当前页码
+    size: int = 0  # 每页大小
+    count: int = 0  # 数据总条数
+    pageCount: int = 0  # 总页数
+    list: List[BaseEntityDto] = None  # 数据list
```

### Comparing `pyva-framework-3.1.17/pyva/entity/BaseEntity.py` & `pyva_framework-3.3.2/pyva/entity/BaseEntity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from humps.main import decamelize
-from sqlalchemy import Column, String, TIMESTAMP, text, DECIMAL, Date, DateTime, JSON, VARCHAR, Boolean
-from sqlalchemy.dialects.mysql import BIGINT, INTEGER, LONGTEXT, TINYINT
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import declared_attr
-
-DeclarativeBase = declarative_base()
-
-
-class BaseEntity(DeclarativeBase):
-    """基础Entity模型对象"""
-
-    # 开启继承
-    __abstract__ = True
-
-    # 表名，帕斯卡命名形式的类名转为小写下划线命名形式
-    @declared_attr
-    def __tablename__(cls):
-        return decamelize(cls.__name__)
-
-    # 表参数，将类注释变为表注释
-    @declared_attr
-    def __table_args__(cls):
-        args = {
-            "mysql_charset": "utf8mb4",
-            "mysql_collate": "utf8mb4_general_ci",
-        }
-
-        if cls.__doc__:
-            args["comment"] = cls.__doc__
-
-        return args
-
-
-if __name__ == "__main__":
-    Column, String, TIMESTAMP, text, DECIMAL, Date, DateTime, JSON, VARCHAR, BIGINT, INTEGER, LONGTEXT, TINYINT, Boolean
+from humps.main import decamelize
+from sqlalchemy import Column, BOOLEAN, String, CHAR, VARCHAR, TEXT, TIMESTAMP, Time, DATE, DATETIME, JSON, INT, FLOAT, DECIMAL, text, UniqueConstraint, Index
+from sqlalchemy.dialects.mysql import INTEGER, TINYINT, BIGINT, LONGTEXT
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declared_attr
+
+DeclarativeBase = declarative_base()
+
+
+class BaseEntity(DeclarativeBase):
+    """基础Entity模型对象"""
+
+    # 开启继承
+    __abstract__ = True
+
+    # 表名，帕斯卡命名形式的类名转为小写下划线命名形式
+    @declared_attr
+    def __tablename__(cls):
+        return decamelize(cls.__name__)
+
+    # 表参数，将类注释变为表注释
+    @declared_attr
+    def __table_args__(cls):
+        args = {
+            "mysql_charset": "utf8mb4",
+            "mysql_collate": "utf8mb4_general_ci",
+        }
+
+        if cls.__doc__:
+            args["comment"] = cls.__doc__
+
+        return args
+
+
+if __name__ == "__main__":
+    Column, BOOLEAN, String, CHAR, VARCHAR, TEXT, TIMESTAMP, Time, DATE, DATETIME, JSON, INT, BIGINT, FLOAT, DECIMAL, text, UniqueConstraint, Index, INTEGER, TINYINT, LONGTEXT
```

### Comparing `pyva-framework-3.1.17/pyva/entity/GeneralHumpEntity.py` & `pyva_framework-3.3.2/pyva/entity/GeneralHumpEntity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from pyva.entity.HumpEntity import *
-
-
-class GeneralHumpEntity(HumpEntity):
-    """通用驼峰Entity"""
-
-    # 开启继承
-    __abstract__ = True
-
-    id = Column(BIGINT(20, unsigned=True), nullable=False, primary_key=True, comment="主键")
-    createdTime = Column(TIMESTAMP, nullable=False, server_default=text("current_timestamp()"), comment="创建时间")
-    createdBy = Column(BIGINT(20, unsigned=True), nullable=False, server_default=text("0"), comment="创建人ID")
-    createdByName = Column(VARCHAR(50), nullable=False, server_default=text("''"), comment="创建人名称")
-    updatedTime = Column(TIMESTAMP, nullable=False, server_default=text("current_timestamp() ON UPDATE current_timestamp()"), comment="修改时间")
-    updatedBy = Column(BIGINT(20, unsigned=True), nullable=False, server_default=text("0"), comment="修改人ID")
-    updatedByName = Column(VARCHAR(50), nullable=False, server_default=text("''"), comment="修改人名称")
-    deleted = Column(Boolean(), nullable=False, server_default=text("0"), comment="是否删除：1是、0否")
+from pyva.entity.HumpEntity import *
+
+
+class GeneralHumpEntity(HumpEntity):
+    """通用驼峰Entity"""
+
+    # 开启继承
+    __abstract__ = True
+
+    id = Column(BIGINT(20, unsigned=True), nullable=False, primary_key=True, comment="主键")
+    createdTime = Column(DATETIME, nullable=False, server_default=text("current_timestamp()"), comment="创建时间")
+    createdBy = Column(BIGINT(20, unsigned=True), nullable=False, server_default=text("0"), comment="创建人ID")
+    createdByName = Column(VARCHAR(50), nullable=False, server_default=text("''"), comment="创建人名称")
+    updatedTime = Column(DATETIME, nullable=False, server_default=text("current_timestamp() ON UPDATE current_timestamp()"), comment="修改时间")
+    updatedBy = Column(BIGINT(20, unsigned=True), nullable=False, server_default=text("0"), comment="修改人ID")
+    updatedByName = Column(VARCHAR(50), nullable=False, server_default=text("''"), comment="修改人名称")
+    deleted = Column(BOOLEAN, nullable=False, server_default=text("0"), comment="是否删除：1是、0否")
```

### Comparing `pyva-framework-3.1.17/pyva/util/DbUtil.py` & `pyva_framework-3.3.2/pyva/util/DbUtil.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from datetime import datetime
 from decimal import Decimal
 from urllib.parse import quote_plus
 
 from humps.main import camelize
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, text
 from sqlalchemy.orm import sessionmaker, scoped_session, Session
 
 from pyva.Global import G
 from pyva.config.DbConfig import DbConfig
 
 
 class DbUtil:
@@ -25,14 +25,15 @@
     def __init__(self, dbConfig: DbConfig):
         """
         初始化时创建session
         :param dbConfig:
         """
         self.config = dbConfig
         self.sess = self.getSession(dbConfig)
+        self.sess.autocommit = dbConfig.autoCommit
 
     def __del__(self):
         """
         销毁时关闭sess
         :return:
         """
 
@@ -78,15 +79,15 @@
             pool_recycle=dbConfig.poolRecycle,
             pool_pre_ping=dbConfig.poolPrePing,
             echo=dbConfig.echo,
             **dbConfig.otherParam
         )
 
         session_factory = sessionmaker(
-            autocommit=dbConfig.autoCommit,
+            # autocommit=dbConfig.autoCommit,
             autoflush=dbConfig.autoFlush,
             bind=engine,
             expire_on_commit=dbConfig.expireOnCommit)
 
         return scoped_session(session_factory)
 
     # 根据文件获取SQL文件
@@ -158,15 +159,15 @@
     def getOne(sess: Session, sql: str):
         """
         查找一个结果
         :param sess:
         :param sql:
         :return:
         """
-        row = sess.execute(sql).fetchone()
+        row = DbUtil.executeSql(sess, sql).fetchone()
         return DbUtil.rowToDict(row)
 
     @staticmethod
     def getOneAndCamelize(sess: Session, sql: str):
         """
         查找一个结果并转为驼峰命名
         :param sess:
@@ -184,15 +185,15 @@
     def getAll(sess: Session, sql: str):
         """
         查找全部结果
         :param sess:
         :param sql:
         :return:
         """
-        rows = sess.execute(sql).fetchall()
+        rows = DbUtil.executeSql(sess, sql).fetchall()
         return DbUtil.rowsToList(rows)
 
     @staticmethod
     def getAllAndCamelize(sess: Session, sql: str):
         """
         查找全部结果并转为驼峰命名
         :param sess:
@@ -233,16 +234,15 @@
         :return:
         """
 
         return str(value).replace(
             "\\", "\\\\").replace(
             '\"', '\\\"').replace(
             ":", "\\:").replace(
-            "%", "\\%").replace(
-            "_", "\\_")
+            "%", "\\%")
 
     @staticmethod
     def handleSqlValue(value) -> str:
         """
         处理Sql的值，转义字符串
         :param value:
         :return:
@@ -346,7 +346,29 @@
         if not table or not where:
             return ""
 
         table = DbUtil.handleSqlField(table)
 
         sql = "DELETE FROM {} WHERE {}".format(table, where)
         return sql
+
+    @staticmethod
+    def executeSql(sess: Session, sql: str):
+        """
+        执行SQL语句
+        :param sess:
+        :param sql:
+        :return:
+        """
+        return sess.execute(text(sql))
+
+    @staticmethod
+    def executeFile(sess: Session, filePath, params: dict = {}):
+        """
+        执行SQL文件
+        :param sess:
+        :param sql:
+        :return:
+        """
+        sql = DbUtil.getSql(filePath, params)
+
+        return DbUtil.executeSql(sess, sql)
```

### Comparing `pyva-framework-3.1.17/pyva/util/NacosUtil.py` & `pyva_framework-3.3.2/pyva/util/NacosUtil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,222 @@
-import _thread
-import logging
-import os
-import random
-import time
-
-import nacos
-import requests
-import yaml
-
-from pyva.config.NacosConfig import NacosConfig
-from pyva.util.JsonUtil import JsonUtil
-
-logger = logging.getLogger('nacos')
-
-
-class NacosUtil:
-    """
-    Nacos工具了
-    :version: 3.0
-    :createdDate: 2020-02-28
-    :updatedDate: 2022-10-03
-    """
-
-    nacosConfig: NacosConfig
-    url: str
-    client = None
-    config = None
-
-    def __init__(self, nacosConfig: NacosConfig):
-        """
-        初始化
-        """
-
-        self.nacosConfig = nacosConfig
-
-        if nacosConfig.ssl:
-            protocol = "https"
-        else:
-            protocol = "http"
-
-        self.url = "{}://{}:{}".format(
-            protocol,
-            nacosConfig.host,
-            nacosConfig.port)
-
-        # 获取client
-        self.getClient(self.url, nacosConfig.namespace)
-
-        # 获取配置
-        self.getConfig()
-
-        # 判断配置赋值
-        if self.config and self.config.get("nacos"):
-            # 判断更新配置：注册服开启状态
-            if self.config.get("nacos").get("serviceEnabled") is not None:
-                nacosConfig.serviceEnabled = self.config.get("nacos").get("serviceEnabled")
-
-            # 判断更新配置：注册服务IP
-            if self.config.get("nacos").get("serviceIp"):
-                nacosConfig.serviceIp = self.config.get("nacos").get("serviceIp")
-            elif os.getenv("SERVICE_IP"):
-                nacosConfig.serviceIp = os.getenv("SERVICE_IP")
-
-        if not nacosConfig.serviceEnabled:
-            return
-
-        # 注册实例
-        self.client.add_naming_instance(
-            self.nacosConfig.serviceName,
-            self.nacosConfig.serviceIp,
-            self.nacosConfig.servicePort,
-            self.nacosConfig.clusterName,
-            self.nacosConfig.weight,
-            self.nacosConfig.metadata,
-            self.nacosConfig.enable,
-            self.nacosConfig.healthy,
-            self.nacosConfig.ephemeral,
-            self.nacosConfig.group)
-
-        # 发送心跳
-        _thread.start_new_thread(self.sendHeartbeat, ())
-
-    def __del__(self):
-        """
-        销毁时注销服务
-        :return:
-        """
-
-        if self.client:
-            self.client.unsubscribe(self.nacosConfig.serviceName)
-
-    def sendHeartbeat(self):
-        """
-        发送心跳
-        :return:
-        """
-        while True:
-            # 发送心跳
-            try:
-                self.client.send_heartbeat(
-                    self.nacosConfig.serviceName,
-                    self.nacosConfig.serviceIp,
-                    self.nacosConfig.servicePort,
-                    self.nacosConfig.clusterName,
-                    self.nacosConfig.weight,
-                    self.nacosConfig.metadata,
-                    self.nacosConfig.ephemeral,
-                    self.nacosConfig.group)
-            except:
-                logger.error("Nacos服务器连接失败")
-
-            time.sleep(self.nacosConfig.heartInterval)
-
-    def getClient(self, url, namespace):
-        """
-        获取client
-        :param url:
-        :param namespace:
-        :return:
-        """
-        self.client = nacos.NacosClient(url, namespace=namespace)
-        return self.client
-
-    def getConfig(self):
-        """
-        获取配置
-        :return:
-        """
-        configStr = self.client.get_config(self.nacosConfig.dataId, self.nacosConfig.group)
-
-        if self.nacosConfig.dataId.endswith(".yml"):
-            self.config = yaml.full_load(configStr)
-        elif self.nacosConfig.dataId.endswith(".json"):
-            self.config = JsonUtil.decode(configStr)
-
-        return self.config
-
-    @staticmethod
-    def resetConfig(obj: object, config: dict):
-        for key, value in config.items():
-            if hasattr(obj, key):
-                setattr(obj, key, value)
-
-    def setConfig(self, obj: object, key):
-        if not self.config:
-            self.getConfig()
-
-        if self.config.get(key):
-            self.resetConfig(obj, self.config.get(key))
-
-    def getInstanceUrl(self, service_name):
-        instance_list = self.client.list_naming_instance(service_name)
-
-        if not instance_list.get('hosts'):
-            return None
-
-        # 提取第一个实例
-        # instance = instance_list.get('hosts')[0]
-        # 随机取一个实例
-        instance = random.choice(instance_list.get('hosts'))
-
-        # 判断是否dev环境，是则用nocos服务器的host地址代替实例的ip
-        if self.nacosConfig.env == 'dev':
-            url = '{}:{}'.format(self.client.get_server()[0], instance.get('port'))
-        else:
-            url = 'http://{}:{}'.format(instance.get('ip'), instance.get('port'))
-
-        return url
-
-    def request(self, method: str, serviceName: str, path: str, **kwargs):
-        """
-        请求屏幕系统服务POST方法
-        :param method 请求方式
-        :param serviceName 服务名
-        :param path 请求地址
-        """
-
-        url = self.getInstanceUrl(serviceName) + path
-
-        resp = requests.request(method=method, url=url, **kwargs)
-
-        if resp.status_code == 200:
-            return resp.json()
-        else:
-            logger.error(resp.text)
-
-            try:
-                return resp.json()
-            except:
-                return None
-
-    def get(self, serviceName: str, path: str, **kwargs):
-        return self.request("get", serviceName, path, **kwargs)
-
-    def post(self, serviceName: str, path: str, **kwargs):
-        return self.request("post", serviceName, path, **kwargs)
-
-    def put(self, serviceName: str, path: str, **kwargs):
-        return self.request("put", serviceName, path, **kwargs)
-
-    def patch(self, serviceName: str, path: str, **kwargs):
-        return self.request("patch", serviceName, path, **kwargs)
-
-    def delete(self, serviceName: str, path: str, **kwargs):
-        return self.request("delete", serviceName, path, **kwargs)
+import _thread
+import os
+import random
+import time
+
+import nacos
+import requests
+import yaml
+
+from pyva.Global import G
+from pyva.config.NacosConfig import NacosConfig
+from pyva.util.DictUtil import DictUtil
+from pyva.util.JsonUtil import JsonUtil
+
+
+class NacosUtil:
+    """
+    Nacos工具了
+    :version: 3.0
+    :createdDate: 2020-02-28
+    :updatedDate: 2022-10-03
+    """
+
+    nacosConfig: NacosConfig
+    url: str
+    client = None
+    config = None
+
+    def __init__(self, nacosConfig: NacosConfig, serviceEnabled=True):
+        """
+        初始化
+        """
+
+        self.nacosConfig = nacosConfig
+
+        if nacosConfig.ssl:
+            protocol = "https"
+        else:
+            protocol = "http"
+
+        self.url = "{}://{}:{}".format(
+            protocol,
+            nacosConfig.host,
+            nacosConfig.port)
+
+        # 获取client
+        self.getClient(self.url, nacosConfig.namespace)
+
+        # 获取配置
+        self.getConfig()
+
+        # 判断配置赋值
+        if self.config and self.config.get("nacos"):
+            # 判断更新配置：注册服开启状态
+            if self.config.get("nacos").get("serviceEnabled") is not None:
+                nacosConfig.serviceEnabled = self.config.get("nacos").get("serviceEnabled")
+
+            # 判断更新配置：注册服务IP
+            if self.config.get("nacos").get("serviceIp"):
+                nacosConfig.serviceIp = self.config.get("nacos").get("serviceIp")
+            elif os.getenv("SERVICE_IP"):
+                nacosConfig.serviceIp = os.getenv("SERVICE_IP")
+
+        if not nacosConfig.serviceEnabled or not serviceEnabled:
+            return
+
+        # 注册实例
+        self.client.add_naming_instance(
+            self.nacosConfig.serviceName,
+            self.nacosConfig.serviceIp,
+            self.nacosConfig.servicePort,
+            self.nacosConfig.clusterName,
+            self.nacosConfig.weight,
+            self.nacosConfig.metadata,
+            self.nacosConfig.enable,
+            self.nacosConfig.healthy,
+            self.nacosConfig.ephemeral,
+            self.nacosConfig.group)
+
+        # 发送心跳
+        _thread.start_new_thread(self.sendHeartbeat, ())
+
+    def __del__(self):
+        """
+        销毁时注销服务
+        :return:
+        """
+
+        if self.client:
+            self.client.unsubscribe(self.nacosConfig.serviceName)
+
+    def sendHeartbeat(self):
+        """
+        发送心跳
+        :return:
+        """
+        while True:
+            # 发送心跳
+            try:
+                self.client.send_heartbeat(
+                    self.nacosConfig.serviceName,
+                    self.nacosConfig.serviceIp,
+                    self.nacosConfig.servicePort,
+                    self.nacosConfig.clusterName,
+                    self.nacosConfig.weight,
+                    self.nacosConfig.metadata,
+                    self.nacosConfig.ephemeral,
+                    self.nacosConfig.group)
+            except:
+                G.logger.error("Nacos服务器连接失败")
+
+            time.sleep(self.nacosConfig.heartInterval)
+
+    def getClient(self, url, namespace):
+        """
+        获取client
+        :param url:
+        :param namespace:
+        :return:
+        """
+        self.client = nacos.NacosClient(url, namespace=namespace)
+        return self.client
+
+    def getConfig(self):
+        """
+        获取配置
+        :return:
+        """
+        if not self.nacosConfig.dataIdList:
+            self.nacosConfig.dataIdList = [self.nacosConfig.dataId]
+
+        config = {}
+
+        for dataId in self.nacosConfig.dataIdList:
+            G.logger.info(f"Nacos配置文件读取：{dataId}")
+            try:
+                configStr = self.client.get_config(dataId, self.nacosConfig.group)
+                if configStr:
+                    if dataId.endswith(".yml"):
+                        DictUtil.mergeDict(config, yaml.full_load(configStr))
+                    elif dataId.endswith(".json"):
+                        DictUtil.mergeDict(config, JsonUtil.decode(configStr))
+                    else:
+                        G.logger.error(f"Nacos配置文件后缀不支持：{dataId}")
+            except Exception as e:
+                G.logger.error(f"Nacos配置文件读取失败：{dataId}，错误：{e}")
+
+        self.config = config
+
+        return self.config
+
+    @staticmethod
+    def resetConfig(obj: object, config: dict):
+        if not config:
+            return
+
+        for key, value in config.items():
+            if hasattr(obj, key):
+                setattr(obj, key, value)
+
+    def setConfig(self, obj: object, key):
+        if not self.config:
+            self.getConfig()
+
+        if self.config.get(key):
+            self.resetConfig(obj, self.config.get(key))
+
+    def getInstanceUrl(self, service_name):
+        instance_list = self.client.list_naming_instance(service_name)
+
+        if not instance_list.get('hosts'):
+            return None
+
+        # 提取第一个实例
+        # instance = instance_list.get('hosts')[0]
+        # 随机取一个实例
+        instance = random.choice(instance_list.get('hosts'))
+
+        # 判断是否dev环境，是则用nocos服务器的host地址代替实例的ip
+        if self.nacosConfig.env == 'dev':
+            url = '{}:{}'.format(self.client.get_server()[0], instance.get('port'))
+        else:
+            url = 'http://{}:{}'.format(instance.get('ip'), instance.get('port'))
+
+        return url
+
+    def request(self, method: str, serviceName: str, path: str, **kwargs):
+        """
+        请求屏幕系统服务POST方法
+        :param method 请求方式
+        :param serviceName 服务名
+        :param path 请求地址
+        """
+
+        url = self.getInstanceUrl(serviceName) + path
+
+        resp = requests.request(method=method, url=url, **kwargs)
+
+        if resp.status_code == 200:
+            return resp.json()
+        else:
+            G.logger.error(resp.text)
+
+            try:
+                return resp.json()
+            except:
+                return None
+
+    def get(self, serviceName: str, path: str, **kwargs):
+        return self.request("get", serviceName, path, **kwargs)
+
+    def post(self, serviceName: str, path: str, **kwargs):
+        return self.request("post", serviceName, path, **kwargs)
+
+    def put(self, serviceName: str, path: str, **kwargs):
+        return self.request("put", serviceName, path, **kwargs)
+
+    def patch(self, serviceName: str, path: str, **kwargs):
+        return self.request("patch", serviceName, path, **kwargs)
+
+    def delete(self, serviceName: str, path: str, **kwargs):
+        return self.request("delete", serviceName, path, **kwargs)
```

### Comparing `pyva-framework-3.1.17/pyva/util/QrcodeUtil.py` & `pyva_framework-3.3.2/pyva/util/QrcodeUtil.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import os
-import random
-from shutil import copyfile
-
-import cv2
-import qrcode
-import requests
-from PIL import Image
-
-from pyva.Global import G
-
-
-def decodeQrcode(img_path):
-    dir_path = os.path.abspath(os.curdir)
-    file_path = dir_path + "/tmp_qrcode_" + str(random.randint(1, 9999)) + os.path.splitext(img_path)[-1]
-
-    if os.path.isfile(img_path):
-        copyfile(img_path, file_path)
-    else:
-        with open(file_path, "wb") as f:
-            f.write(requests.get(url=img_path).content)
-
-    # read the QRCODE image
-    img = cv2.imread(file_path)
-    os.remove(file_path)
-
-    # create a qrcode detector
-    detect = cv2.QRCodeDetector()
-
-    try:
-        # get the data and other threshold
-        # put the image that we have read
-        data, bbox, sqrcode = detect.detectAndDecode(img)
-
-        # bbox is the main thing in the qrcode
-        # if it exist it will give us the data
-        if bbox is not None:
-            return data
-        else:
-            data = decodeQrcodeByCaoliaoApi(img_path)
-
-            if data == "解析失败1":
-                return decodeQrcodeByUomgApi(img_path)
-    except:
-        return decodeQrcodeByCaoliaoApi(img_path)
-
-
-def decodeQrcodeByMuxiaoguoApi(img_path):
-    G.logger.info('decode by muxiaoguo api: {}'.format(img_path))
-    api_url = 'https://api.muxiaoguo.cn/api/QrcodeRT?api_key=0d5f8678d522a4b2&url={}'.format(img_path)
-    resp = requests.get(api_url)
-
-    if resp.status_code == 200 and resp.json().get('code') == '200':
-        data = resp.json()
-        return str(data.get('data', {}).get('content', ''))
-    else:
-        G.logger.error('decode error by muxiaoguo api: {}'.format(api_url))
-        return '解析失败'
-
-
-def decodeQrcodeByUomgApi(img_path):
-    G.logger.info('decode by uomg api: {}'.format(img_path))
-    api_url = 'https://api.uomg.com/api/qr.encode?url={}'.format(img_path)
-    resp = requests.get(api_url)
-
-    if resp.status_code == 200 and resp.json().get('code') == 1:
-        data = resp.json()
-        return data.get('qrurl', '')
-    else:
-        G.logger.error('decode error by uomg api: {}'.format(api_url))
-        return '解析失败'
-
-
-def decodeQrcodeByCaoliaoApi(img_path):
-    G.logger.info('decode by caoliao api: {}'.format(img_path))
-    api_url = 'https://cli.im/Api/Browser/deqr'
-    resp = requests.post(api_url, data={'data': img_path})
-
-    if resp.status_code == 200 and resp.json().get('status') == 1:
-        data = resp.json()
-        result = data.get('data', {}).get('RawData', '')
-
-        if result:
-            return result
-        else:
-            return '解析失败2'
-    else:
-        G.logger.error('decode error by caoliao api: {}'.format(api_url))
-        return '解析失败1'
-
-
-def generateQrcode(text, file_path):
-    img = qrcode.make(text)
-    with open(file_path, 'wb') as f:
-        img.save(f)
-
-
-def generateQrcodeWithLogo(text, file_path, logo_path):
-    qr = qrcode.QRCode(
-        version=10,
-        error_correction=qrcode.constants.ERROR_CORRECT_Q,
-        box_size=7,
-        border=3,
-    )
-    qr.add_data(text)
-    qr.make(fit=True)
-    img = qr.make_image(back_color="#FFF")
-
-    # 添加logo，打开logo照片
-    icon = Image.open(logo_path)
-    # 获取图片的宽高
-    img_w, img_h = img.size
-    # 参数设置logo的大小
-    factor = 1
-    size_w = int(img_w / factor)
-    size_h = int(img_h / factor)
-    icon_w, icon_h = icon.size
-    if icon_w > size_w:
-        icon_w = size_w
-    if icon_h > size_h:
-        icon_h = size_h
-    # 重新设置logo的尺寸
-    icon = icon.resize((icon_w, icon_h), Image.ANTIALIAS)
-    # 得到画图的x，y坐标，居中显示
-    w = int((img_w - icon_w) / 2)
-    h = int((img_h - icon_h) / 2)
-    # 黏贴logo照
-    img.paste(icon, (w, h), mask=None)
-
-    with open(file_path, 'wb') as f:
-        img.save(f)
-
-
-if __name__ == '__main__':
-    filePath = "https://dll-screen-prod.oss-cn-beijing.aliyuncs.com/screenQrCode/6aa3218b0c954935a71119534017c589.png"
-    generateQrcodeWithLogo("https://mhimg.clewm.net/cli/images/beautify/new/logo/30.png", "vc.png",
-                           "../templates/logo_zhifubao.png")
+import os
+import random
+from shutil import copyfile
+
+import cv2
+import qrcode
+import requests
+from PIL import Image
+
+from pyva.Global import G
+
+
+def decodeQrcode(img_path):
+    dir_path = os.path.abspath(os.curdir)
+    file_path = dir_path + "/tmp_qrcode_" + str(random.randint(1, 9999)) + os.path.splitext(img_path)[-1]
+
+    if os.path.isfile(img_path):
+        copyfile(img_path, file_path)
+    else:
+        with open(file_path, "wb") as f:
+            f.write(requests.get(url=img_path).content)
+
+    # read the QRCODE image
+    img = cv2.imread(file_path)
+    os.remove(file_path)
+
+    # create a qrcode detector
+    detect = cv2.QRCodeDetector()
+
+    try:
+        # get the data and other threshold
+        # put the image that we have read
+        data, bbox, sqrcode = detect.detectAndDecode(img)
+
+        # bbox is the main thing in the qrcode
+        # if it exist it will give us the data
+        if bbox is not None:
+            return data
+        else:
+            data = decodeQrcodeByCaoliaoApi(img_path)
+
+            if data == "解析失败1":
+                return decodeQrcodeByUomgApi(img_path)
+    except:
+        return decodeQrcodeByCaoliaoApi(img_path)
+
+
+def decodeQrcodeByMuxiaoguoApi(img_path):
+    G.logger.info('decode by muxiaoguo api: {}'.format(img_path))
+    api_url = 'https://api.muxiaoguo.cn/api/QrcodeRT?api_key=0d5f8678d522a4b2&url={}'.format(img_path)
+    resp = requests.get(api_url)
+
+    if resp.status_code == 200 and resp.json().get('code') == '200':
+        data = resp.json()
+        return str(data.get('data', {}).get('content', ''))
+    else:
+        G.logger.error('decode error by muxiaoguo api: {}'.format(api_url))
+        return '解析失败'
+
+
+def decodeQrcodeByUomgApi(img_path):
+    G.logger.info('decode by uomg api: {}'.format(img_path))
+    api_url = 'https://api.uomg.com/api/qr.encode?url={}'.format(img_path)
+    resp = requests.get(api_url)
+
+    if resp.status_code == 200 and resp.json().get('code') == 1:
+        data = resp.json()
+        return data.get('qrurl', '')
+    else:
+        G.logger.error('decode error by uomg api: {}'.format(api_url))
+        return '解析失败'
+
+
+def decodeQrcodeByCaoliaoApi(img_path):
+    G.logger.info('decode by caoliao api: {}'.format(img_path))
+    api_url = 'https://cli.im/Api/Browser/deqr'
+    resp = requests.post(api_url, data={'data': img_path})
+
+    if resp.status_code == 200 and resp.json().get('status') == 1:
+        data = resp.json()
+        result = data.get('data', {}).get('RawData', '')
+
+        if result:
+            return result
+        else:
+            return '解析失败2'
+    else:
+        G.logger.error('decode error by caoliao api: {}'.format(api_url))
+        return '解析失败1'
+
+
+def generateQrcode(text, file_path):
+    img = qrcode.make(text)
+    with open(file_path, 'wb') as f:
+        img.save(f)
+
+
+def generateQrcodeWithLogo(text, file_path, logo_path):
+    qr = qrcode.QRCode(
+        version=10,
+        error_correction=qrcode.constants.ERROR_CORRECT_Q,
+        box_size=7,
+        border=3,
+    )
+    qr.add_data(text)
+    qr.make(fit=True)
+    img = qr.make_image(back_color="#FFF")
+
+    # 添加logo，打开logo照片
+    icon = Image.open(logo_path)
+    # 获取图片的宽高
+    img_w, img_h = img.size
+    # 参数设置logo的大小
+    factor = 1
+    size_w = int(img_w / factor)
+    size_h = int(img_h / factor)
+    icon_w, icon_h = icon.size
+    if icon_w > size_w:
+        icon_w = size_w
+    if icon_h > size_h:
+        icon_h = size_h
+    # 重新设置logo的尺寸
+    icon = icon.resize((icon_w, icon_h), Image.ANTIALIAS)
+    # 得到画图的x，y坐标，居中显示
+    w = int((img_w - icon_w) / 2)
+    h = int((img_h - icon_h) / 2)
+    # 黏贴logo照
+    img.paste(icon, (w, h), mask=None)
+
+    with open(file_path, 'wb') as f:
+        img.save(f)
+
+
+if __name__ == '__main__':
+    filePath = "https://dll-screen-prod.oss-cn-beijing.aliyuncs.com/screenQrCode/6aa3218b0c954935a71119534017c589.png"
+    generateQrcodeWithLogo("https://mhimg.clewm.net/cli/images/beautify/new/logo/30.png", "vc.png",
+                           "../templates/logo_zhifubao.png")
```

### Comparing `pyva-framework-3.1.17/pyva/util/RedisUtil.py` & `pyva_framework-3.3.2/pyva/util/RedisUtil.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from redis import ConnectionPool, Redis
-
-from pyva.config.RedisConfig import RedisConfig
-from pyva.util.JsonUtil import JsonUtil
-
-
-class RedisUtil:
-    """
-    RedisUtils redis工具类
-    :version: 1.2
-    :date: 2020-02-11
-    """
-
-    conn = None
-    conn_pool = None
-    config: RedisConfig = None
-
-    def __init__(self, redisConfig: RedisConfig):
-        self.config = redisConfig
-
-        # self.conn = self.getConn(config)
-
-        self.initConn()
-
-    def initConn(self):
-        if not self.conn:
-            if not self.conn_pool:
-                self.conn_pool = self.createPool(self.config)
-
-            self.conn = Redis(connection_pool=self.conn_pool)
-
-    @staticmethod
-    def createPool(redisConfig: RedisConfig):
-        return ConnectionPool(
-            host=redisConfig.host,
-            port=redisConfig.port,
-            max_connections=redisConfig.maxConnections,
-            username=redisConfig.username,
-            password=redisConfig.password,
-            db=redisConfig.database
-        )
-
-    @staticmethod
-    def getConn(redisConfig: RedisConfig):
-        return Redis(
-            host=redisConfig.host,
-            port=redisConfig.port,
-            max_connections=redisConfig.maxConnections,
-            username=redisConfig.username,
-            password=redisConfig.password,
-            db=redisConfig.database
-        )
-
-    def delete(self, key):
-        self.initConn()
-        return self.conn.delete(key)
-
-    def setString(self, key, value, ex=None):
-        self.initConn()
-        return self.conn.set(key, value, ex)
-
-    def getString(self, key):
-        self.initConn()
-        value = self.conn.get(key)
-
-        if value:
-            return str(value, "utf-8")
-        else:
-            return None
-
-    def set(self, key, value, ex=None):
-        self.initConn()
-        return self.conn.set(key, JsonUtil.encode(value), ex)
-
-    def get(self, key):
-        self.initConn()
-        value = self.conn.get(key)
-
-        if value:
-            return JsonUtil.decode(str(value, "utf-8"))
-        else:
-            return None
-
-    def expire(self, key, ex=int):
-        self.initConn()
-        return self.conn.expire(key, ex)
+from redis import ConnectionPool, Redis
+
+from pyva.config.RedisConfig import RedisConfig
+from pyva.util.JsonUtil import JsonUtil
+
+
+class RedisUtil:
+    """
+    RedisUtils redis工具类
+    :version: 1.2
+    :date: 2020-02-11
+    """
+
+    conn = None
+    conn_pool = None
+    config: RedisConfig = None
+
+    def __init__(self, redisConfig: RedisConfig):
+        self.config = redisConfig
+
+        # self.conn = self.getConn(config)
+
+        self.initConn()
+
+    def initConn(self):
+        if not self.conn:
+            if not self.conn_pool:
+                self.conn_pool = self.createPool(self.config)
+
+            self.conn = Redis(connection_pool=self.conn_pool)
+
+    @staticmethod
+    def createPool(redisConfig: RedisConfig):
+        return ConnectionPool(
+            host=redisConfig.host,
+            port=redisConfig.port,
+            max_connections=redisConfig.maxConnections,
+            username=redisConfig.username,
+            password=redisConfig.password,
+            db=redisConfig.database
+        )
+
+    @staticmethod
+    def getConn(redisConfig: RedisConfig):
+        return Redis(
+            host=redisConfig.host,
+            port=redisConfig.port,
+            max_connections=redisConfig.maxConnections,
+            username=redisConfig.username,
+            password=redisConfig.password,
+            db=redisConfig.database
+        )
+
+    def delete(self, key):
+        self.initConn()
+        return self.conn.delete(key)
+
+    def setString(self, key, value, ex=None):
+        self.initConn()
+        return self.conn.set(key, value, ex)
+
+    def getString(self, key):
+        self.initConn()
+        value = self.conn.get(key)
+
+        if value:
+            return str(value, "utf-8")
+        else:
+            return None
+
+    def set(self, key, value, ex=None):
+        self.initConn()
+        return self.conn.set(key, JsonUtil.encode(value), ex)
+
+    def get(self, key):
+        self.initConn()
+        value = self.conn.get(key)
+
+        if value:
+            return JsonUtil.decode(str(value, "utf-8"))
+        else:
+            return None
+
+    def expire(self, key, ex=int):
+        self.initConn()
+        return self.conn.expire(key, ex)
```

### Comparing `pyva-framework-3.1.17/pyva_framework.egg-info/SOURCES.txt` & `pyva_framework-3.3.2/pyva_framework.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 LICENSE
 README.md
 setup.py
+pyva/Application.py
 pyva/Global.py
+pyva/GlobalInit.py
 pyva/__init__.py
+pyva/startupApp.py
+pyva/cli/__init__.py
+pyva/cli/main.py
 pyva/client/__init__.py
 pyva/client/dingtalk/DingtalkContactClient.py
 pyva/client/dingtalk/DingtalkOauth2Client.py
+pyva/client/dingtalk/DingtalkRobotClient.py
 pyva/client/dingtalk/DingtalkYidaClient.py
 pyva/client/dingtalk/__init__.py
+pyva/common/FastapiEvents.py
+pyva/common/FastapiException.py
+pyva/common/LoggerHandler.py
+pyva/common/__init__.py
 pyva/config/AppConfig.py
 pyva/config/DbConfig.py
 pyva/config/DingtalkConfig.py
+pyva/config/DingtalkRobotConfig.py
 pyva/config/FastapiConfig.py
 pyva/config/LoggingConfig.py
 pyva/config/MongoConfig.py
 pyva/config/NacosConfig.py
 pyva/config/RedisConfig.py
 pyva/config/__init__.py
 pyva/dao/BaseDao.py
@@ -23,24 +34,28 @@
 pyva/dto/BaseDto.py
 pyva/dto/ListDto.py
 pyva/dto/__init__.py
 pyva/entity/BaseEntity.py
 pyva/entity/GeneralHumpEntity.py
 pyva/entity/HumpEntity.py
 pyva/entity/__init__.py
-pyva/util/AlipayUtil.py
+pyva/util/ConfigUtil.py
 pyva/util/DbUtil.py
+pyva/util/DictUtil.py
 pyva/util/EntityUtil.py
+pyva/util/FileUtil.py
 pyva/util/IpUtil.py
 pyva/util/JsonUtil.py
 pyva/util/LockerUtil.py
 pyva/util/MongoUtil.py
 pyva/util/NacosUtil.py
+pyva/util/PathUtil.py
 pyva/util/QrcodeUtil.py
 pyva/util/RedisUtil.py
 pyva/util/TimeUtil.py
 pyva/util/__init__.py
 pyva_framework.egg-info/PKG-INFO
 pyva_framework.egg-info/SOURCES.txt
 pyva_framework.egg-info/dependency_links.txt
+pyva_framework.egg-info/entry_points.txt
 pyva_framework.egg-info/requires.txt
 pyva_framework.egg-info/top_level.txt
```

### Comparing `pyva-framework-3.1.17/setup.py` & `pyva_framework-3.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-"""
-PyVa-Framework
-"""
-
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-with open("requirements.txt", "r", encoding="utf-8") as fh:
-    requirements = fh.read()
-
-setuptools.setup(
-    name="pyva-framework",
-    version="3.1.17",
-    author="Zhenqiang Sun",
-    author_email="zhenqiang.sun@gmail.com",
-    description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/zhenqiang-sun/pyva",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.6",
-    install_requires=requirements.replace("\n", " ").split(),
-)
+"""
+PyVa-Framework
+"""
+import re
+
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+with open("requirements.txt", "r", encoding="utf-8") as fh:
+    requirements = fh.read()
+    requirements = re.sub(r'(?m)#.*$', '', requirements)
+
+setuptools.setup(
+    name="pyva-framework",
+    version="3.3.2",
+    author="Zhenqiang Sun",
+    author_email="zhenqiang.sun@gmail.com",
+    description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/zhenqiang-sun/pyva",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.11",
+    install_requires=requirements,
+    entry_points={
+        'console_scripts': [
+            'pyva=pyva.cli.main:app',
+        ],
+    },
+)
```

