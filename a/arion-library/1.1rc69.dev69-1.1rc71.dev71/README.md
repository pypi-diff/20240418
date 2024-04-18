# Comparing `tmp/arion_library-1.1rc69.dev69.tar.gz` & `tmp/arion_library-1.1rc71.dev71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc69.dev69.tar", last modified: Thu Apr 18 13:44:54 2024, max compression
+gzip compressed data, was "arion_library-1.1rc71.dev71.tar", last modified: Thu Apr 18 14:25:58 2024, max compression
```

## Comparing `arion_library-1.1rc69.dev69.tar` & `arion_library-1.1rc71.dev71.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 13:44:54.000000 arion_library-1.1rc69.dev69/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 13:44:54.000000 arion_library-1.1rc69.dev69/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:44:54.000000 arion_library-1.1rc69.dev69/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 13:44:54.000000 arion_library-1.1rc69.dev69/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 13:44:54.000000 arion_library-1.1rc69.dev69/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.346990 arion_library-1.1rc69.dev69/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 13:44:00.000000 arion_library-1.1rc69.dev69/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:44:54.350990 arion_library-1.1rc69.dev69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 13:44:52.000000 arion_library-1.1rc69.dev69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 14:25:58.000000 arion_library-1.1rc71.dev71/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 14:25:58.000000 arion_library-1.1rc71.dev71/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:25:58.000000 arion_library-1.1rc71.dev71/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 14:25:58.000000 arion_library-1.1rc71.dev71/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 14:25:58.000000 arion_library-1.1rc71.dev71/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.310841 arion_library-1.1rc71.dev71/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 14:25:08.000000 arion_library-1.1rc71.dev71/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:25:58.314841 arion_library-1.1rc71.dev71/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 14:25:56.000000 arion_library-1.1rc71.dev71/setup.py
```

### Comparing `arion_library-1.1rc69.dev69/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc71.dev71/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/Convert_xml_json_xml/tests/test_methods.py` & `arion_library-1.1rc71.dev71/processors/Convert_xml_json_xml/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc71.dev71/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc71.dev71/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc71.dev71/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc71.dev71/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc71.dev71/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc71.dev71/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc71.dev71/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc71.dev71/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc71.dev71/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc71.dev71/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc69.dev69/setup.py` & `arion_library-1.1rc71.dev71/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc69.dev69',  # Replace with your package version
+    version='1.1rc71.dev71',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

