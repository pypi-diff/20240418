# Comparing `tmp/py_ios_device-2.4.11.tar.gz` & `tmp/py_ios_device-2.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ios_device-2.4.11.tar", last modified: Thu Feb 29 09:54:53 2024, max compression
+gzip compressed data, was "py_ios_device-2.4.12.tar", last modified: Thu Apr 18 09:38:35 2024, max compression
```

## Comparing `py_ios_device-2.4.11.tar` & `py_ios_device-2.4.12.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.668548 py_ios_device-2.4.11/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    12156 2024-02-29 09:54:53.668367 py_ios_device-2.4.11/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    11691 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.644250 py_ios_device-2.4.11/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.648446 py_ios_device-2.4.11/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2024-01-09 02:12:45.000000 py_ios_device-2.4.11/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.4.11/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4442 2024-02-29 09:51:40.000000 py_ios_device-2.4.11/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-06-16 01:58:11.000000 py_ios_device-2.4.11/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2385 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.4.11/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2241 2023-09-08 10:58:15.000000 py_ios_device-2.4.11/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.4.11/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-07-11 11:46:22.000000 py_ios_device-2.4.11/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.4.11/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.4.11/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-07-11 11:46:22.000000 py_ios_device-2.4.11/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2662 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2024-02-29 09:50:41.000000 py_ios_device-2.4.11/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.649403 py_ios_device-2.4.11/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       23 2024-02-29 09:47:44.000000 py_ios_device-2.4.11/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.651292 py_ios_device-2.4.11/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    31701 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-06-28 10:07:29.000000 py_ios_device-2.4.11/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    21967 2024-01-10 02:23:37.000000 py_ios_device-2.4.11/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11238 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2023-07-11 11:50:46.000000 py_ios_device-2.4.11/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.4.11/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.653063 py_ios_device-2.4.11/ios_device/remote/
--rw-r--r--   0 rongcloud   (501) staff       (20)       91 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/remote/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3751 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/remote/remote_lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6078 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/remote/remotexpc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9393 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/remote/xpc_message.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.658422 py_ios_device-2.4.11/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     7533 2024-02-29 09:53:39.000000 py_ios_device-2.4.11/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1389 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19384 2024-02-29 09:47:03.000000 py_ios_device-2.4.11/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1277 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-06-16 01:58:11.000000 py_ios_device-2.4.11/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1532 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3618 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1926 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31576 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3204 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3456 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/pcapd.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3319 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/plist_service.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2024-01-24 09:24:29.000000 py_ios_device-2.4.11/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2024-01-24 09:23:14.000000 py_ios_device-2.4.11/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3630 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1042 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.667180 py_ios_device-2.4.11/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     2682 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11811 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    25263 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2024-01-25 01:58:12.000000 py_ios_device-2.4.11/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2024-01-24 09:20:47.000000 py_ios_device-2.4.11/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2243 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.4.11/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-09-08 10:55:38.000000 py_ios_device-2.4.11/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.4.11/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    42160 2024-01-10 02:08:29.000000 py_ios_device-2.4.11/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16643 2024-01-08 10:35:48.000000 py_ios_device-2.4.11/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    15702 2024-01-25 10:25:01.000000 py_ios_device-2.4.11/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27369 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12642 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12077 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4330 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-02-29 09:54:53.668047 py_ios_device-2.4.11/py_ios_device.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    12156 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2530 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      207 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       16 2024-02-29 09:54:53.000000 py_ios_device-2.4.11/py_ios_device.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      207 2024-01-25 11:32:17.000000 py_ios_device-2.4.11/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2024-02-29 09:54:53.668604 py_ios_device-2.4.11/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      982 2024-01-25 07:51:52.000000 py_ios_device-2.4.11/setup.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.955853 py_ios_device-2.4.12/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12156 2024-04-18 09:38:35.955721 py_ios_device-2.4.12/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11691 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.926189 py_ios_device-2.4.12/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.930532 py_ios_device-2.4.12/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2024-01-09 02:12:45.000000 py_ios_device-2.4.12/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.4.12/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4442 2024-02-29 09:51:40.000000 py_ios_device-2.4.12/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-06-16 01:58:11.000000 py_ios_device-2.4.12/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2385 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.4.12/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2241 2023-09-08 10:58:15.000000 py_ios_device-2.4.12/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.4.12/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1131 2024-04-18 01:49:22.000000 py_ios_device-2.4.12/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.4.12/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.4.12/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-07-11 11:46:22.000000 py_ios_device-2.4.12/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2662 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2024-02-29 09:50:41.000000 py_ios_device-2.4.12/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.931408 py_ios_device-2.4.12/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       23 2024-04-18 09:38:34.000000 py_ios_device-2.4.12/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.934039 py_ios_device-2.4.12/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    31701 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-06-28 10:07:29.000000 py_ios_device-2.4.12/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    21967 2024-01-10 02:23:37.000000 py_ios_device-2.4.12/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11238 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2023-07-11 11:50:46.000000 py_ios_device-2.4.12/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.4.12/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.936017 py_ios_device-2.4.12/ios_device/remote/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       91 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/remote/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3751 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/remote/remote_lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6078 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/remote/remotexpc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9393 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/remote/xpc_message.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.941680 py_ios_device-2.4.12/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7533 2024-02-29 09:53:39.000000 py_ios_device-2.4.12/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1389 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19384 2024-02-29 09:47:03.000000 py_ios_device-2.4.12/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1277 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-06-16 01:58:11.000000 py_ios_device-2.4.12/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1532 2024-04-18 09:37:37.000000 py_ios_device-2.4.12/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3618 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1926 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31576 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3204 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3456 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/pcapd.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3319 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/plist_service.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2024-01-24 09:24:29.000000 py_ios_device-2.4.12/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2024-01-24 09:23:14.000000 py_ios_device-2.4.12/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3630 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1042 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.954832 py_ios_device-2.4.12/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2682 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11811 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    25263 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2024-01-25 01:58:12.000000 py_ios_device-2.4.12/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2024-01-24 09:20:47.000000 py_ios_device-2.4.12/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2243 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.4.12/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-09-08 10:55:38.000000 py_ios_device-2.4.12/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.4.12/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    42160 2024-01-10 02:08:29.000000 py_ios_device-2.4.12/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16643 2024-01-08 10:35:48.000000 py_ios_device-2.4.12/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    15702 2024-01-25 10:25:01.000000 py_ios_device-2.4.12/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27369 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12642 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12077 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4330 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2024-04-18 09:38:35.955525 py_ios_device-2.4.12/py_ios_device.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12156 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2530 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      194 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       16 2024-04-18 09:38:35.000000 py_ios_device-2.4.12/py_ios_device.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      194 2024-04-18 09:37:14.000000 py_ios_device-2.4.12/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2024-04-18 09:38:35.955894 py_ios_device-2.4.12/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      982 2024-01-25 07:51:52.000000 py_ios_device-2.4.12/setup.py
```

### Comparing `py_ios_device-2.4.11/LICENSE` & `py_ios_device-2.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/PKG-INFO` & `py_ios_device-2.4.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ios_device
-Version: 2.4.11
+Version: 2.4.12
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.4.11/README.md` & `py_ios_device-2.4.12/README.md`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/afc.py` & `py_ios_device-2.4.12/demo/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/crash_log.py` & `py_ios_device-2.4.12/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/installation_proxy.py` & `py_ios_device-2.4.12/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/activity.py` & `py_ios_device-2.4.12/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/app_lifecycle.py` & `py_ios_device-2.4.12/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/applictionListing.py` & `py_ios_device-2.4.12/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/coreprofilesessiontap.py` & `py_ios_device-2.4.12/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/coreprofilesessiontap_parse.py` & `py_ios_device-2.4.12/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/deviceinfo.py` & `py_ios_device-2.4.12/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/gpu.py` & `py_ios_device-2.4.12/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/graphics.py` & `py_ios_device-2.4.12/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/mobileNotifications.py` & `py_ios_device-2.4.12/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/netstatPID.py` & `py_ios_device-2.4.12/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/networking.py` & `py_ios_device-2.4.12/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/sysmontap.py` & `py_ios_device-2.4.12/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/instrument_demo/xcuitest.py` & `py_ios_device-2.4.12/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/mobile_config.py` & `py_ios_device-2.4.12/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/pcapd.py` & `py_ios_device-2.4.12/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/screenshotr.py` & `py_ios_device-2.4.12/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/demo/syslog.py` & `py_ios_device-2.4.12/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/cli/base.py` & `py_ios_device-2.4.12/ios_device/cli/base.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/cli/cli.py` & `py_ios_device-2.4.12/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/cli/instruments.py` & `py_ios_device-2.4.12/ios_device/cli/instruments.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/cli/mobile.py` & `py_ios_device-2.4.12/ios_device/cli/mobile.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/py_ios_device.py` & `py_ios_device-2.4.12/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/remote/remote_lockdown.py` & `py_ios_device-2.4.12/ios_device/remote/remote_lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/remote/remotexpc.py` & `py_ios_device-2.4.12/ios_device/remote/remotexpc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/remote/xpc_message.py` & `py_ios_device-2.4.12/ios_device/remote/xpc_message.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/Installation.py` & `py_ios_device-2.4.12/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/Instrument.py` & `py_ios_device-2.4.12/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/afc.py` & `py_ios_device-2.4.12/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/amfi.py` & `py_ios_device-2.4.12/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/crash_log.py` & `py_ios_device-2.4.12/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/diagnostics_relay.py` & `py_ios_device-2.4.12/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/dvt.py` & `py_ios_device-2.4.12/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/house_arrest.py` & `py_ios_device-2.4.12/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/image_mounter.py` & `py_ios_device-2.4.12/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/mc_install.py` & `py_ios_device-2.4.12/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/notification_proxy.py` & `py_ios_device-2.4.12/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/os_trace.py` & `py_ios_device-2.4.12/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/pcapd.py` & `py_ios_device-2.4.12/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/plist_service.py` & `py_ios_device-2.4.12/ios_device/servers/plist_service.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/screenshotr.py` & `py_ios_device-2.4.12/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/simulate_location.py` & `py_ios_device-2.4.12/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/spring_board.py` & `py_ios_device-2.4.12/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/syslog.py` & `py_ios_device-2.4.12/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/servers/testmanagerd.py` & `py_ios_device-2.4.12/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/__init__.py` & `py_ios_device-2.4.12/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/api_util.py` & `py_ios_device-2.4.12/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/bpylist2.py` & `py_ios_device-2.4.12/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/ca.py` & `py_ios_device-2.4.12/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/constants.py` & `py_ios_device-2.4.12/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/dtx_msg.py` & `py_ios_device-2.4.12/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/exceptions.py` & `py_ios_device-2.4.12/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/forward.py` & `py_ios_device-2.4.12/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/gpu_decode.py` & `py_ios_device-2.4.12/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/kc_data.py` & `py_ios_device-2.4.12/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/kperf_data.py` & `py_ios_device-2.4.12/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/lifecycle.py` & `py_ios_device-2.4.12/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/lockdown.py` & `py_ios_device-2.4.12/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/plistlib.py` & `py_ios_device-2.4.12/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/usbmux.py` & `py_ios_device-2.4.12/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/utils.py` & `py_ios_device-2.4.12/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/ios_device/util/variables.py` & `py_ios_device-2.4.12/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/py_ios_device.egg-info/PKG-INFO` & `py_ios_device-2.4.12/py_ios_device.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ios-device
-Version: 2.4.11
+Version: 2.4.12
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.4.11/py_ios_device.egg-info/SOURCES.txt` & `py_ios_device-2.4.12/py_ios_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.4.11/setup.py` & `py_ios_device-2.4.12/setup.py`

 * *Files identical despite different names*

