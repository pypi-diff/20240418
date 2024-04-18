# Comparing `tmp/arion_library-1.1rc78.dev78.tar.gz` & `tmp/arion_library-1.1rc79.dev79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc78.dev78.tar", last modified: Thu Apr 18 16:11:21 2024, max compression
+gzip compressed data, was "arion_library-1.1rc79.dev79.tar", last modified: Thu Apr 18 16:23:48 2024, max compression
```

## Comparing `arion_library-1.1rc78.dev78.tar` & `arion_library-1.1rc79.dev79.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:11:21.000000 arion_library-1.1rc78.dev78/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-18 16:11:21.000000 arion_library-1.1rc78.dev78/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:11:21.000000 arion_library-1.1rc78.dev78/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 16:11:21.000000 arion_library-1.1rc78.dev78/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:11:21.000000 arion_library-1.1rc78.dev78/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Handle_error_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Handle_error_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Handle_error_response/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Handle_error_response/lib/Handle_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Handle_error_response/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/Handle_error_response/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Handle_error_response/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/Handle_error_response/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.063238 arion_library-1.1rc78.dev78/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3077 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:10:37.000000 arion_library-1.1rc78.dev78/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:11:21.067237 arion_library-1.1rc78.dev78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 16:11:20.000000 arion_library-1.1rc78.dev78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:23:48.000000 arion_library-1.1rc79.dev79/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-18 16:23:48.000000 arion_library-1.1rc79.dev79/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:23:48.000000 arion_library-1.1rc79.dev79/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 16:23:48.000000 arion_library-1.1rc79.dev79/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:23:48.000000 arion_library-1.1rc79.dev79/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.483926 arion_library-1.1rc79.dev79/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/Handle_error_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Handle_error_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/Handle_error_response/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Handle_error_response/lib/Handle_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Handle_error_response/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/Handle_error_response/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Handle_error_response/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/Handle_error_response/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3077 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.487926 arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 16:23:01.000000 arion_library-1.1rc79.dev79/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:23:48.491926 arion_library-1.1rc79.dev79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 16:23:46.000000 arion_library-1.1rc79.dev79/setup.py
```

### Comparing `arion_library-1.1rc78.dev78/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc79.dev79/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/Convert_xml_json_xml/tests/test_methods.py` & `arion_library-1.1rc79.dev79/processors/Convert_xml_json_xml/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc79.dev79/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/Handle_error_response/lib/Handle_error_response.py` & `arion_library-1.1rc79.dev79/processors/Handle_error_response/lib/Handle_error_response.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/Handle_error_response/tests/test_methods.py` & `arion_library-1.1rc79.dev79/processors/Handle_error_response/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc79.dev79/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc79.dev79/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc79.dev79/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc79.dev79/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc79.dev79/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc79.dev79/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc79.dev79/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc79.dev79/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc79.dev79/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc79.dev79/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc78.dev78/setup.py` & `arion_library-1.1rc79.dev79/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc78.dev78',  # Replace with your package version
+    version='1.1rc79.dev79',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pyodbc', 'pytest', 'pyodbc', 'pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

