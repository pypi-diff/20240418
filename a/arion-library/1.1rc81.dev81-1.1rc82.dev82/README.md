# Comparing `tmp/arion_library-1.1rc81.dev81.tar.gz` & `tmp/arion_library-1.1rc82.dev82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc81.dev81.tar", last modified: Thu Apr 18 16:44:09 2024, max compression
+gzip compressed data, was "arion_library-1.1rc82.dev82.tar", last modified: Thu Apr 18 16:44:43 2024, max compression
```

## Comparing `arion_library-1.1rc81.dev81.tar` & `arion_library-1.1rc82.dev82.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:44:09.000000 arion_library-1.1rc81.dev81/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-18 16:44:09.000000 arion_library-1.1rc81.dev81/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:09.000000 arion_library-1.1rc81.dev81/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 16:44:09.000000 arion_library-1.1rc81.dev81/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:44:09.000000 arion_library-1.1rc81.dev81/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Handle_error_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Handle_error_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Handle_error_response/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Handle_error_response/lib/Handle_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Handle_error_response/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/Handle_error_response/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Handle_error_response/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/Handle_error_response/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.296280 arion_library-1.1rc81.dev81/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3077 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:43:14.000000 arion_library-1.1rc81.dev81/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:44:09.300280 arion_library-1.1rc81.dev81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 16:44:07.000000 arion_library-1.1rc81.dev81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.677797 arion_library-1.1rc82.dev82/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.665797 arion_library-1.1rc82.dev82/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:44:43.000000 arion_library-1.1rc82.dev82/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-18 16:44:43.000000 arion_library-1.1rc82.dev82/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:43.000000 arion_library-1.1rc82.dev82/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 16:44:43.000000 arion_library-1.1rc82.dev82/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:44:43.000000 arion_library-1.1rc82.dev82/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.665797 arion_library-1.1rc82.dev82/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.665797 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/Handle_error_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Handle_error_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/Handle_error_response/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Handle_error_response/lib/Handle_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Handle_error_response/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/Handle_error_response/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Handle_error_response/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/Handle_error_response/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.669797 arion_library-1.1rc82.dev82/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3077 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:43.673797 arion_library-1.1rc82.dev82/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:43:50.000000 arion_library-1.1rc82.dev82/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:44:43.677797 arion_library-1.1rc82.dev82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 16:44:42.000000 arion_library-1.1rc82.dev82/setup.py
```

### Comparing `arion_library-1.1rc81.dev81/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc82.dev82/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/Convert_xml_json_xml/tests/test_methods.py` & `arion_library-1.1rc82.dev82/processors/Convert_xml_json_xml/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc82.dev82/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/Handle_error_response/lib/Handle_error_response.py` & `arion_library-1.1rc82.dev82/processors/Handle_error_response/lib/Handle_error_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 import logging
 import xml.etree.ElementTree as ET
 
 class ErrorAPI:
+    """A class for handling error responses.
+
+    This class provides a method for handling error responses in XML format.
+
+    Attributes:
+        None
+
+    Methods:
+        _handle_error_response(response):
+            Handles the error response and extracts the error message.
+
+    """
+
     def _handle_error_response(self, response):
-        """
-        Handle error response from the API and extract desired error messages.
+        """Handle the error response and extract the error message.
+
+        Args:
+            response (str): The XML response containing error information.
+
+        Returns:
+            str: Extracted error message or original response if no error message found.
 
-        :param response: The response from the API.
-        :type response: str
-        :param id: The identifier associated with the request.
-        :type id: str
-        :return: Extracted error message or response text.
-        :rtype: str
         """
         try:
             root = ET.fromstring(response)
 
             # Modified this line to directly access the root of the XML tree
             error_message_element = root.find(".//{http://www.cegid.fr/fault}Message")
```

### Comparing `arion_library-1.1rc81.dev81/processors/Handle_error_response/tests/test_methods.py` & `arion_library-1.1rc82.dev82/processors/Handle_error_response/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc82.dev82/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc82.dev82/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc82.dev82/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc82.dev82/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc82.dev82/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc82.dev82/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc82.dev82/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc82.dev82/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc82.dev82/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc82.dev82/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc81.dev81/setup.py` & `arion_library-1.1rc82.dev82/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc81.dev81',  # Replace with your package version
+    version='1.1rc82.dev82',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pyodbc', 'pytest', 'pyodbc', 'pysftp==0.2.9', 'ShopifyAPI==12.5.0', 'requests==2.31.0', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

