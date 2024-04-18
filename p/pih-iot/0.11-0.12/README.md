# Comparing `tmp/pih-iot-0.11.tar.gz` & `tmp/pih-iot-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-iot-0.11.tar", last modified: Wed Apr 17 13:09:53 2024, max compression
+gzip compressed data, was "pih-iot-0.12.tar", last modified: Wed Apr 17 13:22:32 2024, max compression
```

## Comparing `pih-iot-0.11.tar` & `pih-iot-0.12.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 13:09:53.429665 pih-iot-0.11/
--rw-rw-rw-   0        0        0      296 2024-04-17 13:09:53.398429 pih-iot-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 13:09:53.351541 pih-iot-0.11/pih_iot.egg-info/
--rw-rw-rw-   0        0        0      296 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 13:09:53.429665 pih-iot-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 13:22:32.773229 pih-iot-0.12/
+drwxrwxrwx   0        0        0        0 2024-04-17 13:22:32.050836 pih-iot-0.12/IOTDevicesService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-iot-0.12/IOTDevicesService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-04-17 04:59:58.000000 pih-iot-0.12/IOTDevicesService/__main__.py
+-rw-rw-rw-   0        0        0      599 2024-04-17 13:21:56.000000 pih-iot-0.12/IOTDevicesService/const.py
+-rw-rw-rw-   0        0        0     1374 2024-04-17 06:58:43.000000 pih-iot-0.12/IOTDevicesService/service.py
+-rw-rw-rw-   0        0        0      296 2024-04-17 13:22:32.396535 pih-iot-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 13:22:32.363326 pih-iot-0.12/pih_iot.egg-info/
+-rw-rw-rw-   0        0        0      296 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 13:22:31.000000 pih-iot-0.12/pih_iot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:22:32.773229 pih-iot-0.12/setup.cfg
```

