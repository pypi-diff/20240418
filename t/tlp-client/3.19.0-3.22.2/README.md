# Comparing `tmp/tlp-client-3.19.0.tar.gz` & `tmp/tlp-client-3.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlp-client-3.19.0.tar", last modified: Wed Jan 18 13:00:59 2023, max compression
+gzip compressed data, was "tlp-client-3.22.2.tar", last modified: Wed Apr 17 22:54:02 2024, max compression
```

## Comparing `tlp-client-3.19.0.tar` & `tlp-client-3.22.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2023-01-18 13:00:59.588474 tlp-client-3.19.0/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     8998 2023-01-18 13:00:59.588474 tlp-client-3.19.0/PKG-INFO
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     6644 2022-03-04 10:01:51.000000 tlp-client-3.19.0/README.md
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2023-01-18 13:00:59.588474 tlp-client-3.19.0/bin/
--rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)    74259 2023-01-18 12:46:03.000000 tlp-client-3.19.0/bin/tlp-api-cli
--rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)     9510 2022-03-04 10:01:51.000000 tlp-client-3.19.0/bin/tlp-player-urlgen
--rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)     8795 2022-03-04 10:01:51.000000 tlp-client-3.19.0/bin/tlp-transedit-urlgen
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       38 2023-01-18 13:00:59.588474 tlp-client-3.19.0/setup.cfg
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1316 2023-01-18 12:46:03.000000 tlp-client-3.19.0/setup.py
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2023-01-18 13:00:59.588474 tlp-client-3.19.0/tlp_client/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    98680 2023-01-18 12:46:03.000000 tlp-client-3.19.0/tlp_client/__init__.py
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2023-01-18 13:00:59.588474 tlp-client-3.19.0/tlp_client.egg-info/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     8998 2023-01-18 13:00:59.000000 tlp-client-3.19.0/tlp_client.egg-info/PKG-INFO
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      273 2023-01-18 13:00:59.000000 tlp-client-3.19.0/tlp_client.egg-info/SOURCES.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)        1 2023-01-18 13:00:59.000000 tlp-client-3.19.0/tlp_client.egg-info/dependency_links.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       35 2023-01-18 13:00:59.000000 tlp-client-3.19.0/tlp_client.egg-info/requires.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       11 2023-01-18 13:00:59.000000 tlp-client-3.19.0/tlp_client.egg-info/top_level.txt
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-04-17 22:54:02.709775 tlp-client-3.22.2/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     8998 2024-04-17 22:54:02.709775 tlp-client-3.22.2/PKG-INFO
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     6644 2022-03-04 10:01:51.000000 tlp-client-3.22.2/README.md
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-04-17 22:54:02.705774 tlp-client-3.22.2/bin/
+-rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)    74259 2023-01-18 13:02:44.000000 tlp-client-3.22.2/bin/tlp-api-cli
+-rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)     9510 2022-03-04 10:01:51.000000 tlp-client-3.22.2/bin/tlp-player-urlgen
+-rwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)     8795 2022-03-04 10:01:51.000000 tlp-client-3.22.2/bin/tlp-transedit-urlgen
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       38 2024-04-17 22:54:02.709775 tlp-client-3.22.2/setup.cfg
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1331 2024-04-17 22:43:02.000000 tlp-client-3.22.2/setup.py
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-04-17 22:54:02.705774 tlp-client-3.22.2/tlp_client/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    98681 2023-08-04 10:01:00.000000 tlp-client-3.22.2/tlp_client/__init__.py
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-04-17 22:54:02.709775 tlp-client-3.22.2/tlp_client.egg-info/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     8998 2024-04-17 22:54:02.000000 tlp-client-3.22.2/tlp_client.egg-info/PKG-INFO
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      273 2024-04-17 22:54:02.000000 tlp-client-3.22.2/tlp_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)        1 2024-04-17 22:54:02.000000 tlp-client-3.22.2/tlp_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       47 2024-04-17 22:54:02.000000 tlp-client-3.22.2/tlp_client.egg-info/requires.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       11 2024-04-17 22:54:02.000000 tlp-client-3.22.2/tlp_client.egg-info/top_level.txt
```

### Comparing `tlp-client-3.19.0/PKG-INFO` & `tlp-client-3.22.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlp-client
-Version: 3.19.0
+Version: 3.22.2
 Summary: The MLLP-VRAIN's transLectures Platform (TLP) Python3 API client library and tools
 Home-page: https://www.mllp.upv.es
 Author: MLLP-VRAIN
 Author-email: mllp-support@upv.es
 License: UNKNOWN
 Project-URL: Documentation (TLP Platform), https://ttp.mllp.upv.es/doc
 Project-URL: Documentation (library), https://ttp.mllp.upv.es/doc/clients/python3
```

### Comparing `tlp-client-3.19.0/README.md` & `tlp-client-3.22.2/README.md`

 * *Files identical despite different names*

### Comparing `tlp-client-3.19.0/bin/tlp-api-cli` & `tlp-client-3.22.2/bin/tlp-api-cli`

 * *Files identical despite different names*

### Comparing `tlp-client-3.19.0/bin/tlp-player-urlgen` & `tlp-client-3.22.2/bin/tlp-player-urlgen`

 * *Files identical despite different names*

### Comparing `tlp-client-3.19.0/bin/tlp-transedit-urlgen` & `tlp-client-3.22.2/bin/tlp-transedit-urlgen`

 * *Files identical despite different names*

### Comparing `tlp-client-3.19.0/setup.py` & `tlp-client-3.22.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.5',
-    install_requires=['requests', 'requests-toolbelt==0.10.1'],
+    install_requires=['requests', 'requests-toolbelt==0.10.1', 'urllib3<2.0'],
     scripts=['bin/tlp-api-cli',
              'bin/tlp-player-urlgen',
              'bin/tlp-transedit-urlgen']
 )
```

### Comparing `tlp-client-3.19.0/tlp_client/__init__.py` & `tlp-client-3.22.2/tlp_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1737,15 +1737,15 @@
 
           Optionally, a media hash value can be provided using the optional **_vhash_** parameter.
 
           The **_format_** optional parameter sets the downloaded subtitles format.
           Possible values are:  *`TLPTextClient.TRANS_FORMAT_ORIGINAL`*, 
           *`TLPTextClient.TRANS_FORMAT_HTML`*,
           *`TLPTextClient.TRANS_FORMAT_DTLX`*,
-          *`TLPTextClient.TRANS_FORMAT_TXT`*.
+          *`TLPTextClient.TRANS_FORMAT_TEXT`*.
 
 	  **_seldata_** defines which subtitle contents are returned. Possible
           values are: *`TLPTextClient.TRANS_SELDATA_ALL`*,
           *`TLPTextClient.TRANS_SELDATA_FORMER`*,
           *`TLPTextClient.TRANS_SELDATA_CURRENT`*.
 
           A **_session_id_** argument can be provided in order to apply subtitle modifications made under the given edit session ID to the subtitles file.
```

### Comparing `tlp-client-3.19.0/tlp_client.egg-info/PKG-INFO` & `tlp-client-3.22.2/tlp_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlp-client
-Version: 3.19.0
+Version: 3.22.2
 Summary: The MLLP-VRAIN's transLectures Platform (TLP) Python3 API client library and tools
 Home-page: https://www.mllp.upv.es
 Author: MLLP-VRAIN
 Author-email: mllp-support@upv.es
 License: UNKNOWN
 Project-URL: Documentation (TLP Platform), https://ttp.mllp.upv.es/doc
 Project-URL: Documentation (library), https://ttp.mllp.upv.es/doc/clients/python3
```

