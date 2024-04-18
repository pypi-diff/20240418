# Comparing `tmp/arion_library-1.1rc76.dev76.tar.gz` & `tmp/arion_library-1.1rc77.dev77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc76.dev76.tar", last modified: Thu Apr 18 16:01:18 2024, max compression
+gzip compressed data, was "arion_library-1.1rc77.dev77.tar", last modified: Thu Apr 18 16:03:42 2024, max compression
```

## Comparing `arion_library-1.1rc76.dev76.tar` & `arion_library-1.1rc77.dev77.tar`

### file list

```diff
@@ -1,71 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:01:18.000000 arion_library-1.1rc76.dev76/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 16:01:18.000000 arion_library-1.1rc76.dev76/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:01:18.000000 arion_library-1.1rc76.dev76/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 16:01:18.000000 arion_library-1.1rc76.dev76/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:01:18.000000 arion_library-1.1rc76.dev76/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.890468 arion_library-1.1rc76.dev76/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:00:33.000000 arion_library-1.1rc76.dev76/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:01:18.894468 arion_library-1.1rc76.dev76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 16:01:16.000000 arion_library-1.1rc76.dev76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:03:42.000000 arion_library-1.1rc77.dev77/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-18 16:03:42.000000 arion_library-1.1rc77.dev77/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:03:42.000000 arion_library-1.1rc77.dev77/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 16:03:42.000000 arion_library-1.1rc77.dev77/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:03:42.000000 arion_library-1.1rc77.dev77/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Handle_error_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Handle_error_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Handle_error_response/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Handle_error_response/lib/Handle_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Handle_error_response/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/Handle_error_response/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Handle_error_response/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/Handle_error_response/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.266350 arion_library-1.1rc77.dev77/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:02:55.000000 arion_library-1.1rc77.dev77/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:03:42.270350 arion_library-1.1rc77.dev77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 16:03:40.000000 arion_library-1.1rc77.dev77/setup.py
```

### Comparing `arion_library-1.1rc76.dev76/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc77.dev77/arion_library.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 processors/Convert_xml_json_xml/tests/__init__.py
 processors/Convert_xml_json_xml/tests/test_methods.py
 processors/FTP_connector/__init__.py
 processors/FTP_connector/lib/FTPconnector.py
 processors/FTP_connector/lib/__init__.py
 processors/FTP_connector/tests/__init__.py
 processors/FTP_connector/tests/test_ftp_connector.py
+processors/Handle_error_response/__init__.py
+processors/Handle_error_response/lib/Handle_error_response.py
+processors/Handle_error_response/lib/__init__.py
+processors/Handle_error_response/tests/__init__.py
+processors/Handle_error_response/tests/test_methods.py
 processors/OracleConnector/__init__.py
 processors/OracleConnector/lib/OracleDatabase.py
 processors/OracleConnector/lib/__init__.py
 processors/OracleConnector/tests/__init__.py
 processors/OracleConnector/tests/test_oracle_connector.py
 processors/SFTP/__init__.py
 processors/SFTP/lib/__init__.py
```

### Comparing `arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 import xmltodict
 import json
 import os
 
 class XML_JSON_XML:
     """
-    Classe pour la conversion entre les formats XML et JSON.
+    Class for conversion between XML and JSON formats.
     """
 
     def detect_file_type(self, file_path):
         """
-        Détermine le type de fichier en fonction de son extension.
+        Determine the file type based on its extension.
 
         Args:
-            file_path (str): Chemin du fichier.
+            file_path (str): Path of the file.
 
         Returns:
-            str: Type de fichier ('xml', 'json') ou None si le type n'est pas pris en charge.
+            str: File type ('xml', 'json') or None if the type is not supported.
         """
         file_extension = os.path.splitext(file_path)[1].lower()
         if file_extension == '.xml':
             return 'xml'
         elif file_extension == '.json':
             return 'json'
         else:
             return None
 
     def convert_xml_to_json(self, xml_content):
         """
-        Convertit le contenu XML en JSON.
+        Convert XML content to JSON.
 
         Args:
-            xml_content (str): Contenu XML sous forme de chaîne de caractères.
+            xml_content (str): XML content as a string.
 
         Returns:
-            str: Contenu JSON résultant.
+            str: Resulting JSON content.
         """
         data_dict = xmltodict.parse(xml_content)
         json_data = json.dumps(data_dict, indent=4)
         return json_data
 
     def convert_json_to_xml(self, json_content):
         """
-        Convertit le contenu JSON en XML.
+        Convert JSON content to XML.
 
         Args:
-            json_content (str): Contenu JSON sous forme de chaîne de caractères.
+            json_content (str): JSON content as a string.
 
         Returns:
-            str: Contenu XML résultant.
+            str: Resulting XML content.
         """
-        # Remplacer "None" par "null" dans le contenu JSON
+        # Replace "None" with "null" in the JSON content
         json_content = json_content.replace("None", "null")
 
-        # Analyse du contenu JSON
+        # Parse JSON content
         data_list = json.loads(json_content)
 
-        # Créer une chaîne XML pour chaque élément racine
+        # Create XML string for each root item
         xml_data_list = []
         for item in data_list:
             xml_data_list.append(xmltodict.unparse({"root": item}, pretty=True))
 
-        # Joindre les chaînes XML
+        # Join XML strings
         xml_data = "\n".join(xml_data_list)
         return xml_data
 
     def convert_file(self, file_path):
         """
-        Convertit un fichier du format source (XML ou JSON) au format cible (JSON ou XML).
+        Convert a file from the source format (XML or JSON) to the target format (JSON or XML).
 
         Args:
-            file_path (str): Chemin du fichier source.
+            file_path (str): Path of the source file.
 
         Raises:
-            ValueError: Si le type de fichier n'est pas pris en charge.
+            ValueError: If the file type is not supported.
         """
         file_type = self.detect_file_type(file_path)
         if file_type == 'xml':
             with open(file_path, 'r') as xml_file:
                 xml_content = xml_file.read()
                 json_data = self.convert_xml_to_json(xml_content)
                 with open('Output.json', 'w') as json_file:
                     json_file.write(json_data)
-            print("Conversion XML vers JSON réussie.")
+            print("XML to JSON conversion successful.")
             print(json_data)
         elif file_type == 'json':
             with open(file_path, 'r') as json_file:
                 json_content = json_file.read()
                 xml_data = self.convert_json_to_xml(json_content)
                 with open('Output.xml', 'w') as xml_file:
                     xml_file.write(xml_data)
-            print("Conversion JSON vers XML réussie.")
+            print("JSON to XML conversion successful.")
             print(xml_data)
         else:
-            raise ValueError("Type de fichier non pris en charge.")
+            raise ValueError("Unsupported file type.")
 
-# Exemple d'utilisation de la classe
+# Example of using the class
 xml_json_xml_instance = XML_JSON_XML()
 xml_json_xml_instance.convert_file(r'C:\Repos_Arion\ArionLibrary\processors\Convert_xml_json_xml\tests\Input_File_test\CERT.xml')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `arion_library-1.1rc76.dev76/processors/Convert_xml_json_xml/tests/test_methods.py` & `arion_library-1.1rc77.dev77/processors/Convert_xml_json_xml/tests/test_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import pytest
 from ..lib.Convert_Soap_Rest import XML_JSON_XML
 
 # Fixtures
 @pytest.fixture
 def converter():
     """
-    Fixture pour initialiser une instance de XML_JSON_XML pour les tests.
+    Fixture to initialize an instance of XML_JSON_XML for testing.
     """
     return XML_JSON_XML()
 
-# Chemin du fichier de test XML
-file_path= (r'C:\Repos_Arion\ArionLibrary\processors\Convert_xml_json_xml\tests\Input_File_test\CERT.xml')
+# Path to the XML test file
+file_path = (r'C:\Repos_Arion\ArionLibrary\processors\Convert_xml_json_xml\tests\Input_File_test\CERT.xml')
 
 def test_detect_file_type_json(converter):
     """
-    Test pour vérifier si la méthode detect_file_type détecte correctement le type de fichier JSON.
-    
+    Test to verify if the detect_file_type method correctly detects JSON file type.
+
     Args:
-        converter: Instance de XML_JSON_XML.
+        converter: Instance of XML_JSON_XML.
     """
     assert converter.detect_file_type(file_path) == 'json'
-    
-    
+
+
 def test_convert_file_json(converter):
     """
-    Test pour vérifier si la méthode convert_file convertit correctement un fichier JSON en XML.
-    
+    Test to verify if the convert_file method correctly converts a JSON file to XML.
+
     Args:
-        converter: Instance de XML_JSON_XML.
+        converter: Instance of XML_JSON_XML.
     """
-    # Convertir le fichier JSON en XML en utilisant la méthode convert_file
+    # Convert the JSON file to XML using the convert_file method
     converter.convert_file(file_path)
 
 # Tests
 def test_detect_file_type_xml(converter):
     """
-    Test pour vérifier si la méthode detect_file_type détecte correctement le type de fichier XML.
-    
+    Test to verify if the detect_file_type method correctly detects XML file type.
+
     Args:
-        converter: Instance de XML_JSON_XML.
+        converter: Instance of XML_JSON_XML.
     """
     assert converter.detect_file_type(file_path) == 'xml'
 
+
 def test_convert_file_xml(converter):
     """
-    Test pour vérifier si la méthode convert_file convertit correctement un fichier XML en JSON.
-    
+    Test to verify if the convert_file method correctly converts an XML file to JSON.
+
     Args:
-        converter: Instance de XML_JSON_XML.
+        converter: Instance of XML_JSON_XML.
     """
-    # Convertir le fichier XML en JSON en utilisant la méthode convert_file
+    # Convert the XML file to JSON using the convert_file method
     converter.convert_file(file_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `arion_library-1.1rc76.dev76/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc77.dev77/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc77.dev77/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc77.dev77/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc77.dev77/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc77.dev77/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc77.dev77/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc77.dev77/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc77.dev77/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc77.dev77/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc77.dev77/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc77.dev77/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc76.dev76/setup.py` & `arion_library-1.1rc77.dev77/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc76.dev76',  # Replace with your package version
+    version='1.1rc77.dev77',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
-    install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
+    install_requires=['pyodbc', 'pytest', 'pyodbc', 'pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

