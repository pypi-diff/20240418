# Comparing `tmp/DLMS_SPODES_client-0.7.9.tar.gz` & `tmp/DLMS_SPODES_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.7.9.tar", last modified: Tue Apr 16 08:37:27 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.8.0.tar", last modified: Thu Apr 18 07:34:33 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.7.9.tar` & `DLMS_SPODES_client-0.8.0.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.267256 DLMS_SPODES_client-0.7.9/
--rw-rw-rw-   0        0        0      526 2024-04-16 08:37:27.266258 DLMS_SPODES_client-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.9/README.md
--rw-rw-rw-   0        0        0      836 2024-04-16 08:30:27.000000 DLMS_SPODES_client-0.7.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 08:37:27.268254 DLMS_SPODES_client-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.110255 DLMS_SPODES_client-0.7.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.129256 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   113757 2024-04-16 08:33:37.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.063255 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.148290 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.199293 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.255256 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.258255 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5599 2024-04-11 08:53:09.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    43047 2024-04-12 09:08:36.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.144256 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-16 08:37:26.000000 DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:37:27.264255 DLMS_SPODES_client-0.7.9/test/
--rw-rw-rw-   0        0        0     8082 2024-04-12 09:11:11.000000 DLMS_SPODES_client-0.7.9/test/test_Client.py
--rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.7.9/test/test_services.py
--rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.7.9/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.608812 DLMS_SPODES_client-0.8.0/
+-rw-rw-rw-   0        0        0      526 2024-04-18 07:34:33.607812 DLMS_SPODES_client-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.0/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-18 07:34:22.000000 DLMS_SPODES_client-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 07:34:33.608812 DLMS_SPODES_client-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.451812 DLMS_SPODES_client-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.469820 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   115338 2024-04-18 07:14:59.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.441429 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.490845 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.538813 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.592843 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.594816 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5559 2024-04-17 09:05:51.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    43781 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.485821 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-18 07:34:33.000000 DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:34:33.605813 DLMS_SPODES_client-0.8.0/test/
+-rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.0/test/name2.csv
+-rw-rw-rw-   0        0        0     8289 2024-04-17 14:08:20.000000 DLMS_SPODES_client-0.8.0/test/test_Client.py
+-rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.0/test/test_logger.py
+-rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.8.0/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.0/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.7.9/PKG-INFO` & `DLMS_SPODES_client-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.7.9
+Version: 0.8.0
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.9/pyproject.toml` & `DLMS_SPODES_client-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS-SPODES == 0.69.5",
+    "DLMS-SPODES == 0.69.6",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=['dlms', 'spodes', 'client']
```

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import dataclasses
 import time
+from abc import ABC, abstractmethod
 from functools import cached_property, reduce
 from struct import pack
 from collections import deque
 from itertools import count
 from enum import IntEnum, auto, IntFlag
-from typing import TextIO, Deque, Any
+from typing import TextIO, Deque, Any, Self, Callable
 import threading
 import datetime
 import os
 import hashlib
 from Cryptodome.Cipher import AES
 from DLMS_SPODES_communications import Network, SerialPort, RS485, BLE, AsyncNetwork, AsyncSerial, base
 from DLMS_SPODES.cosem_interface_classes import collection, overview
@@ -32,16 +34,15 @@
 from .gurux_dlms.GXDLMSSNParameters import GXDLMSSNParameters
 from .gurux_dlms.AesGcmParameter import AesGcmParameter
 from .gurux_dlms.GXCiphering import GXCiphering
 from .gurux_dlms.GXDLMSConfirmedServiceError import GXDLMSConfirmedServiceError
 from .gurux_dlms.GXDLMSChippering import GXDLMSChippering
 from .gurux_dlms import CountType
 from .gurux_dlms.internal._GXCommon import _GXCommon
-from .logger import logger
-from .enums import LogLevel as logL
+from .logger import logger, LogLevel as logL
 
 
 def copy_with_align(data: bytes, block_size: int = 16) -> bytes:
     """ fill by zeros to full 16 bytes blocks """
     return data + bytes((block_size - len(data) % block_size) % block_size)
 
 
@@ -103,17 +104,57 @@
     DLMS = auto()
     """DLMS association level."""
 
     def __str__(self):
         return self.name
 
 
+class State(ABC):
+
+    @abstractmethod
+    def __str__(self):
+        """"""
+
+
+@dataclasses.dataclass
+class Text(State):
+    value: str
+
+    def __str__(self):
+        return self.value
+
+
+class ID:
+    def __init__(self, prefix: str):
+        self.count = count()
+        self.value = set()
+        self.prefix = prefix
+
+    def create(self, value: str = None) -> str:
+        id_ = F"{self.prefix}{next(self.count)}" if value is None else value
+        """for identification before LDN reading"""
+        while True:
+            if id_ not in self.value:
+                self.value.add(id_)
+                break
+            elif value:
+                raise ValueError(F"in create ID with {id_}: already exist")
+            else:
+                id_ = F"{self.prefix}{next(self.count)}"
+        return id_
+
+    def remove(self, value: str) -> bool:
+        self.value.remove(value)
+        return True
+
+
 class Client:
-    id_count = count()
-    status: Status
+    id: str | None
+    __del_cb: Callable[[str], None] | None
+    status: Status  # todo all remove to state
     connection_state: ConnectionState
     log_file: TextIO
     media: Network | SerialPort | RS485 | BLE | base.StreamBase | None
     lock: threading.Lock
     errors: Errors
     last_transfer_time: datetime.timedelta | None
     connection_time_release: int
@@ -133,23 +174,28 @@
     DEF_DLMS_VER: int = 6
     """DLMS version by default"""
     m_id: mechanism_id.MechanismIdElement
     """None is the AUTO from current association"""
     device_address: cdt.LongUnsigned | None
     addr_size: frame.AddressLength
     logging_disable: bool
+    state: State
 
     def __init__(self,
                  SAP: int = 0x10,
                  secret: str = "",
                  conformance: str = None,
                  addr_size: int = -1,
-                 media: base.StreamBase = AsyncSerial(port="COM3")):
-        self.__id = next(Client.id_count)
+                 media: base.StreamBase = AsyncSerial(port="COM3"),
+                 id_: str | int = None,
+                 del_cb: Callable[[str], None] = None):
+        self.id = id_
         """for identification before LDN reading"""
+        self.__del_cb = del_cb
+        """callback to unregister id"""
         self.logging_disable = False
         """turn off logging by default"""
         self.objects = None
         self.__sap = enums.ClientSAP(SAP)
         """Service Access Point. Default <Public>"""
         self.server_SAP = long_unsigneds.ServerSAP(1)
         self.secret = bytes.fromhex(secret)
@@ -210,20 +256,28 @@
         self.current_obj = None
         """ current transferring object. For progress bar now """
 
         # from Gurux Client
         self.use_protected_release = False
         """  Gurux Client: If protected release is used release is including a ciphered xDLMS Initiate request. """
 
-    def log(self, level: logL, msg: str):
+        self.state = Text("undefined")
+
+    def __del__(self):
+        if self.__del_cb:
+            self.__del_cb(self.id)
+
+    def log(self, level: logL, msg: str | State):
         """use logger with level and extra=LDN"""
         if not self.logging_disable:
             logger.log(level=level,
-                       msg=msg,
-                       extra={"id": self.objects.LDN.value.to_str() if (self.objects and self.objects.LDN.value) else F"#{self.__id}"})
+                       msg=str(msg),
+                       extra={"id": self.objects.LDN.value.to_str() if (self.objects and self.objects.LDN.value) else F"{self.id}"})
+        if level == logL.STATE and isinstance(msg, State):
+            self.state = msg
 
     @property
     def SAP(self) -> enums.ClientSAP:
         return self.__sap
 
     @SAP.setter
     def SAP(self, value):
@@ -997,34 +1051,37 @@
                     self.media = eval(F"SerialPort({dict_})")
                 case _: raise ValueError(F"unknown type: {value.__class__.__name__} for set communication channel {self}")
             self.log(logL.INFO, F"set2 to {self} communication channel: {self.media}")
         except Exception as e:
             self.log(logL.ERR, F"not set to {self} communication channel by {value}")
 
     async def close(self):
-        """ send DISC to server and after close media """
-        self.log(logL.DEB, "DisconnectRequest")
-        try:
-            # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
-            if self.settings.interfaceType == InterfaceType.WRAPPER or \
-                    (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
-                self.releaseRequest()
-                await self.read_data_block()
-        except Exception:
-            self.log(logL.WARN, "don't support release ReleaseRequest")
-            pass
-            #  All meters don't support release.
-        try:
-            if self.connection_state != ConnectionState.NONE:
+        """close """
+        self.log(logL.DEB, "close")
+        if self.connection_state != ConnectionState.NONE:
+            try:
+                # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
+                if self.settings.interfaceType == InterfaceType.WRAPPER or \
+                        (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
+                    self.releaseRequest()
+                    await self.read_data_block()
+            except Exception:
+                self.log(logL.WARN, "don't support release ReleaseRequest")
+                pass
+                #  All meters don't support release.
+            finally:
+                self.connection_state = ConnectionState.HDLC
+            # hdlc close
+            try:
                 res = await self.disconnect_request()
                 # todo: handle res
-        except Exception as e:
-            self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
-        finally:
-            self.connection_state = ConnectionState.NONE
+            except Exception as e:
+                self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
+            finally:
+                self.connection_state = ConnectionState.NONE
         self.log(logL.DEB, F'Close communication channel: {self.media}')
         if self.status == Status.CONNECTED:
             self.status = Status.READY
 
     async def disconnect_request(self):
         """ Sent to server DISC """
         if self.settings.interfaceType == InterfaceType.HDLC:
@@ -1970,15 +2027,15 @@
                 break
             else:
                 control = frame.Control(self.settings.getNextSend(False))
         self.send_frames.extend(new_frames)
 
     def __str__(self):
         if not self.objects or not self.objects.LDN.value:
-            return str(self.__id)
+            return str(self.id)
         else:
             return self.objects.LDN.value.to_str()
 
     def get_serial_number(self) -> str:
         """ return serial number as text. If serial object is absence return 'недоступен' """
         if self.objects is None:
             return "нет типа"
```

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from threading import Thread, Event
 from functools import cached_property
 import asyncio
 from .client import Client, Errors, cdt
 from . import task
 from DLMS_SPODES.enums import Transmit, Application
 from DLMS_SPODES import exceptions as exc
-from .enums import LogLevel as logL
+from .logger import LogLevel as logL
 
 
 class Result:
     client: Client
     complete: bool
     errors: Errors
     value: cdt.CommonDataType | None
@@ -32,15 +32,15 @@
                  tsk: task.ExTask,
                  name: str = None):
         self.__values = tuple(Result(c) for c in clients)
         self.tsk = tsk
         self.name = name
         """common operation name"""
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Result:
         return self.__values[item]
 
     @cached_property
     def clients(self) -> set[Client]:
         return {res.client for res in self.__values}
 
     @cached_property
@@ -106,16 +106,15 @@
             tg.create_task(
                 coro=check_stop(tg),
                 name="wait abort task")
 
 
 async def session(c: Client,
                   t: task.ExTask,
-                  result: Result = None,
-                  is_public: bool = False):
+                  result: Result):
     if not result:  # if not use TransActionServer
         result = Result(c)
     c.lock.acquire(timeout=10)  # 10 second, todo: keep parameter anywhere
     # try media open
     assert c.media is not None, F"media is absense"
     if not c.media.is_open():
         try:
```

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/services.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from DLMS_SPODES.cosem_interface_classes import collection, overview
 from DLMS_SPODES.types import cdt, ut, cst
 from DLMS_SPODES.hdlc import frame
 from DLMS_SPODES.enums import Transmit, Application
 from DLMS_SPODES.obis import media_id
 from DLMS_SPODES.firmwares import get_firmware
 from DLMS_SPODES.cosem_interface_classes.image_transfer import image_transfer_status as i_t_status
-from .client import Client, pdu, logL, AppVersion, ConnectionState, Status, Security, Data, Conformance, mechanism_id, AcseServiceUser
+from .client import Client, pdu, logL, AppVersion, ConnectionState, Status, Security, Data, Conformance, mechanism_id, AcseServiceUser, State
 
 
 class ExTask(ABC):
     """Exchange task for DLMS client"""
     async def exchange(self, c: Client, is_public: bool = False):
         if c.connection_state == ConnectionState.NONE:
             if await get_HDLC(c, is_public) is False:
@@ -218,16 +218,15 @@
             ret.append(res)
         return ret
 
 
 class InitType(ExTask):
     """nothing params"""
     async def exchange(self, c: Client, is_public: bool = False):
-        await c.disconnect_request()
-        c.connection_state = ConnectionState.NONE
+        await c.close()  # close hdlc before init
         return await super(InitType, self).exchange(c, is_public=True)
 
     async def exchange2(self, c: Client):
         # read LDN
         data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
         ldn = octet_string.LDN(data)
         # find device_id(type for Russia)
@@ -438,14 +437,24 @@
 
 # @dataclass
 # class UpdateResponse:
 #     result:
 
 
 @dataclass
+class Progress(State):
+    position: int
+    max: int
+    message: str
+
+    def __str__(self):
+        return F"{self.message}: {self.position}/{self.max}"
+
+
+@dataclass
 class UpdateFirmware(ExTask):
     """only for KPZ now"""
 
     async def exchange2(self, c: Client) -> bool:
         # check available action todo: not work in 0.0.38
         # if c.current_association.object_list is None:
         #     await ReadAttribute(
@@ -524,15 +533,18 @@
                 c.set_error(Application.VERSION_ERROR, F'Version {c.objects.server_ver} don\'t read update properties')
                 return False
             case _:
                 c.set_error(Transmit.READ_ERROR, 'Wrong AppVersion')
                 return False
         # add optional object if its values absence
         ret = await read_seq.exchange(c)
-        # todo: check exchange result
+        for r, t in zip(ret, read_seq.tasks):
+            if isinstance(r, exc.ResultError):  # todo: rewrite with new ReadResponse
+                c.set_error(Transmit.READ_ERROR, message=F"error in {t}: {r}")
+                return False
         c.objects.firmware_image_transfer.clear_image()  # TODO: check for missing objects !!
         firmwares_description_obj = c.objects.firmwares_description
         boot_version: int = int(firmwares_description_obj.value.decode()[:4])
         firmwares_description = firmwares_description_obj.value.decode()[4:]
         suitable_firmware: AppVersion = AppVersion(0, 0, 1)
         suitable_boot: int = 0
         temp_key: tuple | None = None
@@ -787,18 +799,23 @@
                         case i_t_status.VERIFICATION_FAILED:
                             await ReadAttribute(
                                 ln=obj.logical_name,
                                 index=3
                             ).exchange(c)
                             valid = obj.image_transferred_blocks_status.decode()
                             c.log(logL.INFO, F"Got blocks[{len(obj.image_transferred_blocks_status)}]: {obj.image_transferred_blocks_status}")
+                            log_state = Progress(0, obj.get_n_blocks(), F"update {collection.get_name(obj.logical_name)}")
+                            c.log(logL.STATE, log_state)
                             for index in filter(lambda it: valid[it] == 0, range(len(valid))):
                                 obj.set_block_for_transfer(index)
                                 await c.execute_method(obj.get_meth_descriptor(2))
-                                c.log(logL.INFO, F"start block: {obj.current_block_transfer} transferred")
+                                if isinstance(c.state, Progress):
+                                    log_state.position = index
+                                    c.log(logL.STATE, log_state)
+                                # c.log(logL.INFO, F"start block: {obj.current_block_transfer} transferred")
                             await c.execute_method(obj.get_meth_descriptor(3))
                             c.log(logL.INFO, "Start Verify Transfer")
                         case i_t_status.VERIFICATION_SUCCESSFUL:
                             await ReadAttributes(
                                 ln=obj.logical_name,
                                 indexes=(7, 4, 3)
                             ).exchange(c)
```

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.7.9
+Version: 0.8.0
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.9/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.8.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 README.md
 pyproject.toml
 setup.py
 src/__init__.py
 src/DLMS_SPODES_client/FCS16.py
 src/DLMS_SPODES_client/__init__.py
 src/DLMS_SPODES_client/client.py
-src/DLMS_SPODES_client/enums.py
 src/DLMS_SPODES_client/logger.py
 src/DLMS_SPODES_client/servers.py
 src/DLMS_SPODES_client/services.py
 src/DLMS_SPODES_client/task.py
 src/DLMS_SPODES_client.egg-info/PKG-INFO
 src/DLMS_SPODES_client.egg-info/SOURCES.txt
 src/DLMS_SPODES_client.egg-info/dependency_links.txt
@@ -60,10 +59,12 @@
 src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
 src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
 src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
 src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+test/name2.csv
 test/test_Client.py
+test/test_logger.py
 test/test_services.py
 test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.7.9/test/test_Client.py` & `DLMS_SPODES_client-0.8.0/test/test_Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from DLMS_SPODES.types import cdt
 from src.DLMS_SPODES_client.client import Client, SerialPort, Network, AsyncNetwork, Collection, AppVersion, AsyncSerial
 from src.DLMS_SPODES_client.servers import TransactionServer
 from src.DLMS_SPODES_client import task
 
 
 class TestType(unittest.TestCase):
+    def test_create_Client(self):
+        c1 = Client()
+        c2 = Client(id_="d2")
+        del c2
+        Client()
+        Client()
+        c3 = Client()
+        print(c1.id, c3.id, Client.ids)
+
     def test_connect(self):
         t_server = TransactionServer(
             clients=[c := Client(media=AsyncSerial(
                                 port="COM13",
                                 inactivity_timeout=3))],
             tsk=task.Dummy()
         )
```

