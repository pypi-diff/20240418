# Comparing `tmp/arion_library-1.1rc74.dev74.tar.gz` & `tmp/arion_library-1.1rc75.dev75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc74.dev74.tar", last modified: Thu Apr 18 15:39:57 2024, max compression
+gzip compressed data, was "arion_library-1.1rc75.dev75.tar", last modified: Thu Apr 18 15:48:00 2024, max compression
```

## Comparing `arion_library-1.1rc74.dev74.tar` & `arion_library-1.1rc75.dev75.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 15:39:57.000000 arion_library-1.1rc74.dev74/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 15:39:57.000000 arion_library-1.1rc74.dev74/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:39:57.000000 arion_library-1.1rc74.dev74/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 15:39:57.000000 arion_library-1.1rc74.dev74/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 15:39:57.000000 arion_library-1.1rc74.dev74/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.539095 arion_library-1.1rc74.dev74/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3116 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 15:39:09.000000 arion_library-1.1rc74.dev74/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:39:57.543095 arion_library-1.1rc74.dev74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 15:39:55.000000 arion_library-1.1rc74.dev74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 15:47:59.000000 arion_library-1.1rc75.dev75/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 15:47:59.000000 arion_library-1.1rc75.dev75/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:47:59.000000 arion_library-1.1rc75.dev75/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 15:47:59.000000 arion_library-1.1rc75.dev75/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 15:47:59.000000 arion_library-1.1rc75.dev75/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.013197 arion_library-1.1rc75.dev75/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3129 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 15:47:16.000000 arion_library-1.1rc75.dev75/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:48:00.017197 arion_library-1.1rc75.dev75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 15:47:58.000000 arion_library-1.1rc75.dev75/setup.py
```

### Comparing `arion_library-1.1rc74.dev74/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc75.dev75/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/Convert_xml_json_xml/tests/test_methods.py` & `arion_library-1.1rc75.dev75/processors/Convert_xml_json_xml/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc75.dev75/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc75.dev75/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc75.dev75/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc75.dev75/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc75.dev75/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc75.dev75/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc75.dev75/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 import logging
 
 class AzureBlobProcessor:
     """
 
     A class for processing files in Azure Blob Storage_____test update after github pages
-
+        again
 
 
     
     :param account_name: The Azure Storage account name.
     :param account_key: The Azure Storage account key.
     :param container_name: The name of the container in Azure Blob Storage.
     :param flow_name: The name of the flow for organizing files.
```

### Comparing `arion_library-1.1rc74.dev74/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc75.dev75/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc75.dev75/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc75.dev75/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc75.dev75/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc74.dev74/setup.py` & `arion_library-1.1rc75.dev75/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc74.dev74',  # Replace with your package version
+    version='1.1rc75.dev75',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

