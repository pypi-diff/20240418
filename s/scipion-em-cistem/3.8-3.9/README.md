# Comparing `tmp/scipion-em-cistem-3.8.tar.gz` & `tmp/scipion-em-cistem-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cistem-3.8.tar", last modified: Wed Feb 28 09:48:18 2024, max compression
+gzip compressed data, was "scipion-em-cistem-3.9.tar", last modified: Thu Apr 18 12:36:04 2024, max compression
```

## Comparing `scipion-em-cistem-3.8.tar` & `scipion-em-cistem-3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.572272 scipion-em-cistem-3.8/cistem/
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    95934 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/cistem_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.572272 scipion-em-cistem-3.8/cistem/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/convert/dataimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/cistem/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/program_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_refine2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_tomo_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_ts_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_ts_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20788 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols/protocol_unblur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/cistem/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/tests/test_protocols_cistem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/tests/test_protocols_cistem_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/tests/tomo_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/cistem/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/viewers/tomo_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/viewers/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/cistem/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-28 09:48:18.000000 scipion-em-cistem-3.8/scipion_em_cistem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 09:48:18.576272 scipion-em-cistem-3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-02-28 09:47:55.000000 scipion-em-cistem-3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.458840 scipion-em-cistem-3.9/cistem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95934 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/cistem_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/dataimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/program_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_refine2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_tomo_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ts_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ts_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20788 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_unblur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/tomo_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/tomo_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/setup.py
```

### Comparing `scipion-em-cistem-3.8/CHANGES.txt` & `scipion-em-cistem-3.9/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+3.9:
+  Users:
+   - add ctffind5, rename config vars
+  Developers: 
+   - update the acquisition order in the CTFTomo objects (field added to that class in scipion-em-tomo v3.7.0).
 3.8: new protocols to resample tomo and TS
 3.7.1: fix an obsolete import in the viewer.
 3.7:
   Users:
    - Improve import TomoCTF matching.
    - Fix TS Ctffind parallelization.
   Developers:
```

### Comparing `scipion-em-cistem-3.8/LICENSE` & `scipion-em-cistem-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/PKG-INFO` & `scipion-em-cistem-3.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cistem
-Version: 3.8
+Version: 3.9
 Summary: Plugin to use cisTEM programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cistem
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cistem/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cistem/
@@ -55,40 +55,51 @@
         
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-cistem --devel
         
+        **Important:** Starting from plugin v3.9, the config variables have been renamed. See: `scipion3 config -p cistem`
+        
         cisTEM binaries will be installed automatically with the plugin, but you can also link an existing installation.
         
             * Default installation path assumed is ``software/em/cistem-1.0.0-beta``, if you want to change it, set *CISTEM_HOME* in ``scipion.conf`` file pointing to the folder where the cisTEM is installed.
-            * It's possible to use CTFFIND4 installed separately from cisTEM by defining *CTFFIND4_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
+            * It's possible to use CTFFIND installed separately from cisTEM by defining *CTFFIND_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
         
         A complete list of tests can be seen by executing ``scipion test --show --grep cistem``
         
         Supported versions
         ------------------
         
         * 1.0.0-beta (cistem)
         * 4.1.13, 4.1.14 (ctffind4)
+        * 5.0 (ctffind5)
+        
+        Licenses
+        --------
+        
+        * cistem binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
+        * ctffind4 binaries are distributed under `The Janelia Research Campus Software License 1.1 license <https://www.janelia.org/node/47808>`_
+        * ctffind5 binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
         
         Protocols
         ---------
         
-        * ctffind4
+        * ctffind
         * import tomo CTFs
-        * tilt-series ctffind4
+        * tilt-series ctffind
         * unblur
         * find particles
         * classify 2D
         
         References
         ----------
         
-        1. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
+        1. Johannes Elferich, Lingli Kong, Ximena Zottig, Nikolaus Grigorieff. (2024) CTFFIND5 provides improved insight into quality, tilt and thickness of TEM samples. bioRxiv 2024.02.26.582023; doi: https://doi.org/10.1101/2024.02.26.582023
+        2. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-cistem-3.8/README.rst` & `scipion-em-cistem-3.9/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -45,34 +45,45 @@
 
     * install
 
     .. code-block::
 
         scipion installp -p /path/to/scipion-em-cistem --devel
 
+**Important:** Starting from plugin v3.9, the config variables have been renamed. See: `scipion3 config -p cistem`
+
 cisTEM binaries will be installed automatically with the plugin, but you can also link an existing installation.
 
     * Default installation path assumed is ``software/em/cistem-1.0.0-beta``, if you want to change it, set *CISTEM_HOME* in ``scipion.conf`` file pointing to the folder where the cisTEM is installed.
-    * It's possible to use CTFFIND4 installed separately from cisTEM by defining *CTFFIND4_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
+    * It's possible to use CTFFIND installed separately from cisTEM by defining *CTFFIND_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
 
 A complete list of tests can be seen by executing ``scipion test --show --grep cistem``
 
 Supported versions
 ------------------
 
 * 1.0.0-beta (cistem)
 * 4.1.13, 4.1.14 (ctffind4)
+* 5.0 (ctffind5)
+
+Licenses
+--------
+
+* cistem binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
+* ctffind4 binaries are distributed under `The Janelia Research Campus Software License 1.1 license <https://www.janelia.org/node/47808>`_
+* ctffind5 binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
 
 Protocols
 ---------
 
-* ctffind4
+* ctffind
 * import tomo CTFs
-* tilt-series ctffind4
+* tilt-series ctffind
 * unblur
 * find particles
 * classify 2D
 
 References
 ----------
 
-1. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
+1. Johannes Elferich, Lingli Kong, Ximena Zottig, Nikolaus Grigorieff. (2024) CTFFIND5 provides improved insight into quality, tilt and thickness of TEM samples. bioRxiv 2024.02.26.582023; doi: https://doi.org/10.1101/2024.02.26.582023
+2. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
```

### Comparing `scipion-em-cistem-3.8/cistem/__init__.py` & `scipion-em-cistem-3.9/cistem/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,45 +28,45 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.8'
+__version__ = '3.9'
 _logo = "cistem_logo.png"
 _references = ['Grant2018']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = CISTEM_HOME
-    _pathVars = [CISTEM_HOME]
+    _pathVars = [CISTEM_HOME, CTFFIND_HOME]
     _supportedVersions = [V1_0_0]
     _url = "https://github.com/scipion-em/scipion-em-cistem"
 
     @classmethod
     def _defineVariables(cls):
         cls._defineEmVar(CISTEM_HOME, 'cistem-1.0.0-beta')
-        cls._defineEmVar(CTFFIND4_HOME, 'ctffind4-4.1.14')
+        cls._defineEmVar(CTFFIND_HOME, 'ctffind4-4.1.14')
 
     @classmethod
     def getEnviron(cls):
         """ Setup the environment variables needed to launch cisTEM. """
         environ = pwutils.Environ(os.environ)
         environ.update({'PATH': cls.getHome()},
                        position=pwutils.Environ.BEGIN)
 
         return environ
 
     @classmethod
     def getProgram(cls, program):
         """ Return the program binary that will be used. """
-        if program == CTFFIND4_BIN:
-            # if CTFFIND4_HOME is found, use it
-            path = cls.getVar(CTFFIND4_HOME)
+        if program == CTFFIND_BIN:
+            # if CTFFIND_HOME is found, use it
+            path = cls.getVar(CTFFIND_HOME)
             if os.path.exists(path):
                 binary = os.path.join(path, 'bin', program)
             else:
                 binary = os.path.join(cls.getHome(), program)
         else:
             binary = os.path.join(cls.getHome(), program)
 
@@ -76,8 +76,11 @@
     def defineBinaries(cls, env):
         env.addPackage('cistem', version='1.0.0-beta',
                        url="https://grigoriefflab.umassmed.edu/sites/default/files/cistem-1.0.0-beta-intel-linux.tar.gz",
                        default=True)
         env.addPackage('ctffind4', version='4.1.13',
                        tar='ctffind4-4.1.13.tgz')
         env.addPackage('ctffind4', version='4.1.14',
-                       tar='ctffind4-4.1.14.tgz')
+                       tar='ctffind4-4.1.14.tgz',
+                       default=True)
+        env.addPackage('ctffind', version='5.0',
+                       tar='ctffind-5.0.tgz')
```

### Comparing `scipion-em-cistem-3.8/cistem/bibtex.py` & `scipion-em-cistem-3.9/cistem/bibtex.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 
+@article {Elferich2024,
+	author = {Johannes Elferich and Lingli Kong and Ximena Zottig and Nikolaus Grigorieff},
+	title = {CTFFIND5 provides improved insight into quality, tilt and thickness of TEM samples},
+	year = {2024},
+	doi = {10.1101/2024.02.26.582023},
+	publisher = {Cold Spring Harbor Laboratory},
+	URL = {https://www.biorxiv.org/content/early/2024/02/28/2024.02.26.582023},
+	journal = {bioRxiv}
+}
+
 @article{Grant2018,
 title = "cisTEM, user-friendly software for single-particle image processing",
 journal = "eLife",
 volume = "7",
 pages = "e35383",
 year = "2018",
 doi = "https://dx.doi.org/10.7554/eLife.35383.001",
```

### Comparing `scipion-em-cistem-3.8/cistem/cistem_logo.png` & `scipion-em-cistem-3.9/cistem/cistem_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/constants.py` & `scipion-em-cistem-3.9/cistem/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 CISTEM_HOME = 'CISTEM_HOME'
 
 # Supported versions
 V1_0_0 = '1.0.0-beta'
 
 # ------------------ Constants values -----------------------------------------
-
-CTFFIND4_HOME = 'CTFFIND4_HOME'
-CTFFIND4_BIN = 'ctffind'
+CTFFIND_HOME = 'CTFFIND_HOME'
+CTFFIND_BIN = 'ctffind'
 UNBLUR_BIN = 'unblur'
 FIND_PARTICLES_BIN = 'find_particles'
 
 LOW_VARIANCE = 0
 VARIANCE_NEAR_MODE = 1
```

### Comparing `scipion-em-cistem-3.8/cistem/convert/__init__.py` & `scipion-em-cistem-3.9/cistem/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/convert/convert.py` & `scipion-em-cistem-3.9/cistem/convert/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
     """
     defocusU = float(ctfRow.get('DF1'))
     defocusV = float(ctfRow.get('DF2'))
     defocusAngle = float(ctfRow.get('ANGAST'))
     ctfModel.setStandardDefocus(defocusU, defocusV, defocusAngle)
 
 
-def parseCtffind4Output(filename):
+def parseCtffindOutput(filename):
     """ Retrieve defocus U, V and angle from the
-    output file of the ctffind4 execution.
+    output file of the ctffind execution.
     :param filename: input file to parse
     :return: an array with CTF values
     """
     if os.path.exists(filename):
         return np.loadtxt(filename, dtype=float, comments='#')
     else:
         logger.error(f"Warning: Missing file: {filename}")
@@ -139,15 +139,15 @@
 
     if ctfArray is None or np.isnan(values).any(axis=0) or values[1] < 0 or values[2] < 0:
         logger.debug(f"Invalid CTF values: {values}")
         setWrongDefocus(ctfModel)
         ctfFit, ctfResolution, ctfPhaseShift = -999, -999, 0
     else:
         (_, defocusU, defocusV, defocusAngle, ctfPhaseShift,
-         ctfFit, ctfResolution) = values
+         ctfFit, ctfResolution, *_) = values
         ctfModel.setStandardDefocus(defocusU, defocusV, defocusAngle)
     ctfModel.setFitQuality(ctfFit)
     ctfModel.setResolution(ctfResolution)
 
     # Avoid creation of phaseShift
     ctfPhaseShiftDeg = np.rad2deg(ctfPhaseShift)
     if ctfPhaseShiftDeg != 0:
@@ -156,15 +156,15 @@
 
 def readCtfModel(ctfModel, filename):
     """ Shortcut function to read CTFs for non-stacks
     and set ctfModel values.
     :param ctfModel: output CTF model
     :param filename: file to parse
     """
-    result = parseCtffind4Output(filename)
+    result = parseCtffindOutput(filename)
     readCtfModelStack(ctfModel, result, item=0)
 
 
 def readShiftsMovieAlignment(shiftFn):
     """ Parse movie alignment shifts.
     :param shiftFn: input file to parse
     :return: two lists with shift values
```

### Comparing `scipion-em-cistem-3.8/cistem/convert/dataimport.py` & `scipion-em-cistem-3.9/cistem/convert/dataimport.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 import os.path
 
 import pyworkflow.utils as pwutils 
 from pwem.objects import CTFModel, SetOfParticles
 
 from .convert import (readCtfModel, readSetOfParticles,
-                      readCtfModelStack, parseCtffind4Output)
+                      readCtfModelStack, parseCtffindOutput)
 
 with pwutils.weakImport('tomo'):
     from tomo.objects import CTFTomo
 
 
 class GrigorieffLabImportCTF:
-    """ Import CTF estimated with CTFFIND4. """
+    """ Import CTF estimated with CTFFIND. """
     def __init__(self, protocol):
         self.protocol = protocol
         self.copyOrLink = self.protocol.getCopyOrLink()
 
     def importCTF(self, mic, fileName):
         """ Create a CTF model and populate its values.
         :param mic: input micrograph object
@@ -65,29 +65,30 @@
         :param ts: input tilt-series
         :param fileName: input file to be parsed
         :param output: output CTFTomoSeries
         """
         tsId = ts.getTsId()
         fnBase = os.path.join(os.path.dirname(fileName), tsId)
         outputPsd = self._findPsdFile(fnBase)
-        ctfResult = parseCtffind4Output(fileName)
+        ctfResult = parseCtffindOutput(fileName)
         ctf = CTFModel()
         counter = 0
 
         for i, ti in enumerate(ts):
             if ti.isEnabled():
                 self.getCtfTi(ctf, ctfResult, counter, outputPsd)
                 counter += 1
             else:
                 ctf.setWrongDefocus()
 
             newCtfTomo = CTFTomo.ctfModelToCtfTomo(ctf)
             if not ti.isEnabled():
                 newCtfTomo.setEnabled(False)
             newCtfTomo.setIndex(i + 1)
+            newCtfTomo.setAcquisitionOrder(ti.getAcquisitionOrder())
             output.append(newCtfTomo)
 
         output.calculateDefocusUDeviation()
         output.calculateDefocusVDeviation()
 
     @staticmethod
     def getCtfTi(ctf, ctfArray, tiIndex, psdStack=None):
```

### Comparing `scipion-em-cistem-3.8/cistem/protocols/__init__.py` & `scipion-em-cistem-3.9/cistem/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols/program_ctffind.py` & `scipion-em-cistem-3.9/cistem/protocols/program_ctffind.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 
 from numpy import deg2rad
 
 from pwem.objects import CTFModel
 import pyworkflow.protocol.params as params
 
 from cistem import Plugin
-from ..constants import CTFFIND4_BIN
+from ..constants import CTFFIND_BIN
 from ..convert import readCtfModel
 
 
 class ProgramCtffind:
     """
-    Wrapper of Ctffind4 program that will handle parameters definition
+    Wrapper of Ctffind program that will handle parameters definition
     and also execution of the program with the proper arguments.
     This class is not a Protocol, but somewhat related, since it can be used from
     protocols that perform CTF estimation.
     """
     def __init__(self, protocol):
-        self._program = Plugin.getProgram(CTFFIND4_BIN)  # Load program to use
+        self._program = Plugin.getProgram(CTFFIND_BIN)  # Load program to use
         self._findPhaseShift = protocol.findPhaseShift.get()
         self._args, self._params = self._getArgs(protocol)  # Load general arguments
 
     @classmethod
     def defineInputParams(cls, form):
         """ Define input/common parameters. """
         form.addSection(label='Input')
@@ -243,14 +243,16 @@
 %(maxDefocus)f
 %(step_focus)f
 no
 %(slowSearch)s
 %(fixAstig)s
 %(phaseShift)s
 no
+no
+no
 eof\n
 """
 
         if protocol.usePowerSpectra:
             args = args.replace('<< eof > %(ctffindOut)s',
                                 '--amplitude-spectrum-input << eof > %(ctffindOut)s')
             args = args.replace('%(samplingRate)f',
```

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_ctffind.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_ctffind.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,20 @@
 from pwem.objects import CTFModel
 from pwem import emlib
 
 from .program_ctffind import ProgramCtffind
 
 
 class CistemProtCTFFind(ProtCTFMicrographs):
-    """ Estimate CTF for a set of micrographs with ctffind4.
+    """ Estimate CTF for a set of micrographs with ctffind.
     
-    To find more information about ctffind4 visit:
+    To find more information about ctffind visit:
     https://grigoriefflab.umassmed.edu/ctffind4
     """
-    _label = 'ctffind4'
+    _label = 'ctffind'
     _devStatus = PROD
 
     def _defineParams(self, form):
         ProgramCtffind.defineInputParams(form)
         ProgramCtffind.defineProcessParams(form)
         self._defineStreamingParams(form)
 
@@ -157,15 +157,15 @@
                 valueStep <= (valueMax - valueMin) and
                 0. <= valueMax <= 180.):
             errors.append('Wrong values for phase shift search.')
 
         return errors
 
     def _citations(self):
-        return ["Mindell2003", "Rohou2015"]
+        return ["Mindell2003", "Rohou2015", "Elferich2024"]
 
     def _methods(self):
         methods = []
         if self.inputMicrographs.get() is not None:
             methods.append("We calculated the CTF of %s using CTFFind. "
                            % self.getObjectTag('inputMicrographs'))
             methods.append(self.methodsVar.get(''))
```

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_picking.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_refine2d.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_refine2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_tomo_resample.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_tomo_resample.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_ts_ctffind.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_ts_ctffind.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,29 @@
 import pyworkflow.protocol.params as params
 import pyworkflow.utils as pwutils
 from pwem.objects import CTFModel
 from pwem import emlib
 from collections import namedtuple
 from tomo.protocols.protocol_ts_estimate_ctf import createCtfParams
 from .program_ctffind import ProgramCtffind
-from ..convert import readCtfModelStack, parseCtffind4Output
+from ..convert import readCtfModelStack, parseCtffindOutput
 from tomo.objects import CTFTomo, SetOfCTFTomoSeries, CTFTomoSeries
 
 MRCS_EXT = ".mrcs"
 # create simple, lightweight data structures similar to a class, but without the overhead of defining a full class
 CistemTsCtfMd = namedtuple('CistemTsCtfMd', ['ts', 'tsFn', 'outputLog', 'outputPsd'])
 
 
 class TsCtffindOutputs(Enum):
     CTFs = SetOfCTFTomoSeries
 
 
 class CistemProtTsCtffind(EMProtocol):
-    """ CTF estimation on a set of tilt series using CTFFIND4. """
-    _label = 'tilt-series ctffind4'
+    """ CTF estimation on a set of tilt series using CTFFIND. """
+    _label = 'tilt-series ctffind'
     _devStatus = PROD
     _possibleOutputs = TsCtffindOutputs
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.stepsExecutionMode = STEPS_PARALLEL
         self.usePowerSpectra = False
@@ -157,19 +157,20 @@
         newCTFTomoSeries.copyInfo(ts)
         newCTFTomoSeries.setTiltSeries(ts)
         newCTFTomoSeries.setObjId(ts.getObjId())
         newCTFTomoSeries.setTsId(ts.getTsId())
         outCtfSet.append(newCTFTomoSeries)
 
         # Generate the ti CTF and populate the corresponding CTF tomo series
-        ctfResult = parseCtffind4Output(outputLog)
+        ctfResult = parseCtffindOutput(outputLog)
         ctf = CTFModel()
         for i, tiltImage in enumerate(ts.iterItems()):
             ctfTomo = self._getCtfTi(ctf, ctfResult, i, mdObj.outputPsd)
             ctfTomo.setIndex(tiltImage.getIndex())
+            ctfTomo.setAcquisitionOrder(tiltImage.getAcquisitionOrder())
             tiltImage.setCTF(ctfTomo)
             newCTFTomoSeries.append(ctfTomo)
 
         outCtfSet.update(newCTFTomoSeries)
         self._store()
 
     def closeStep(self):
```

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_ts_resample.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_ts_resample.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols/protocol_unblur.py` & `scipion-em-cistem-3.9/cistem/protocols/protocol_unblur.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/protocols.conf` & `scipion-em-cistem-3.9/cistem/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/tests/__init__.py` & `scipion-em-cistem-3.9/cistem/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow.tests import DataSet
 from pyworkflow.utils import weakImport
 
-from .test_protocols_cistem import TestCtffind4
+from .test_protocols_cistem import TestCtffind
 from .test_protocols_cistem_movies import TestMoviesBase, TestUnblur
 with weakImport("tomo"):
-    from .tomo_tests import TestCtffind4Ts
+    from .tomo_tests import TestCtffindTs
 
 DataSet(name='tutorialDataImodCTF',
         folder='tutorialDataImodCTF',
         files={
             'tsCtf1': 'WTI042413_1series4.st'
         })
```

### Comparing `scipion-em-cistem-3.8/cistem/tests/test_protocols_cistem.py` & `scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,23 +89,23 @@
         cls.launchProtocol(cls.protCTF)
         cls.assertIsNotNone(cls.protCTF.outputCTF,
                             "SetOfCTF has not been produced.")
 
         return cls.protCTF
 
 
-class TestCtffind4(TestBase):
+class TestCtffind(TestBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         TestBase.setData()
         print(magentaStr("\n==> Importing data - micrographs:"))
         cls.protImport = cls.runImportMicrographBPV(cls.micFn)
     
-    def testCtffind4V1(self):
+    def testCtffind(self):
         print(magentaStr("\n==> Testing cistem - ctffind:"))
         protCTF = CistemProtCTFFind()
         protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
         self.launchProtocol(protCTF, wait=True)
         self.assertIsNotNone(protCTF.outputCTF, "SetOfCTF has not been produced.")
 
         valuesList = [[24067, 23587], [22373, 22039], [22653, 22480]]
```

### Comparing `scipion-em-cistem-3.8/cistem/tests/test_protocols_cistem_movies.py` & `scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/tests/tomo_tests.py` & `scipion-em-cistem-3.9/cistem/tests/tomo_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                                        tiltAxisAngle=DataSetRe4STATuto.tiltAxisAngle.value)
 
         cls.launchProtocol(protImportTs)
         tsImported = getattr(protImportTs, 'outputTiltSeries', None)
         return tsImported
 
 
-class TestCtffind4Ts(TestBase):
+class TestCtffindTs(TestBase):
     def testCistemCtfFind(self):
         print(magentaStr("\n==> Testing cistem - ctffind:"))
         protCTF = CistemProtTsCtffind(inputTiltSeries=self.inputSoTS,
                                       lowRes=50,
                                       highRes=4,
                                       minDefocus=15000,
                                       maxDefocus=50000,
```

### Comparing `scipion-em-cistem-3.8/cistem/viewers/tomo_viewers.py` & `scipion-em-cistem-3.9/cistem/viewers/tomo_viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/cistem/viewers/viewers.py` & `scipion-em-cistem-3.9/cistem/viewers/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,31 +84,31 @@
 
 
 def _getValuesArray(fn):
     """ Parse input file and return an array with results. """
     return np.loadtxt(fn, dtype=float, comments="#")
 
 
-OBJCMD_CTFFIND4 = "CTFFind plot results"
+OBJCMD_CTFFIND = "CTFFind plot results"
 
-ProjectWindow.registerObjectCommand(OBJCMD_CTFFIND4, createCtfPlot)
+ProjectWindow.registerObjectCommand(OBJCMD_CTFFIND, createCtfPlot)
 
 
 class CtffindViewer(Viewer):
     """ Specific way to visualize SetOfCtf. """
     _environments = [DESKTOP_TKINTER]
     _targets = [CistemProtCTFFind]
 
     def _visualize(self, prot, **kwargs):
         outputCTF = getattr(prot, 'outputCTF', None)
 
         if outputCTF is not None:
             ctfView = CtfView(self._project, outputCTF)
             viewParams = ctfView.getViewParams()
-            viewParams[showj.OBJCMDS] = "'%s'" % OBJCMD_CTFFIND4
+            viewParams[showj.OBJCMDS] = "'%s'" % OBJCMD_CTFFIND
             return [ctfView]
         else:
             return [self.infoMessage("The output SetOfCTFs has not been "
                                      "produced", "Missing output")]
 
 
 class ProtUnblurViewer(EmProtocolViewer):
```

### Comparing `scipion-em-cistem-3.8/cistem/wizards.py` & `scipion-em-cistem-3.9/cistem/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/scipion_em_cistem.egg-info/PKG-INFO` & `scipion-em-cistem-3.9/scipion_em_cistem.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cistem
-Version: 3.8
+Version: 3.9
 Summary: Plugin to use cisTEM programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cistem
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cistem/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cistem/
@@ -55,40 +55,51 @@
         
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-cistem --devel
         
+        **Important:** Starting from plugin v3.9, the config variables have been renamed. See: `scipion3 config -p cistem`
+        
         cisTEM binaries will be installed automatically with the plugin, but you can also link an existing installation.
         
             * Default installation path assumed is ``software/em/cistem-1.0.0-beta``, if you want to change it, set *CISTEM_HOME* in ``scipion.conf`` file pointing to the folder where the cisTEM is installed.
-            * It's possible to use CTFFIND4 installed separately from cisTEM by defining *CTFFIND4_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
+            * It's possible to use CTFFIND installed separately from cisTEM by defining *CTFFIND_HOME* variable in ``scipion.conf``. Setting this value will have the priority over Ctffind inside cisTEM.
         
         A complete list of tests can be seen by executing ``scipion test --show --grep cistem``
         
         Supported versions
         ------------------
         
         * 1.0.0-beta (cistem)
         * 4.1.13, 4.1.14 (ctffind4)
+        * 5.0 (ctffind5)
+        
+        Licenses
+        --------
+        
+        * cistem binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
+        * ctffind4 binaries are distributed under `The Janelia Research Campus Software License 1.1 license <https://www.janelia.org/node/47808>`_
+        * ctffind5 binaries are distributed under `The Janelia Research Campus Software License 1.2 license <http://license.janelia.org/license/janelia_license_1_2.html>`_
         
         Protocols
         ---------
         
-        * ctffind4
+        * ctffind
         * import tomo CTFs
-        * tilt-series ctffind4
+        * tilt-series ctffind
         * unblur
         * find particles
         * classify 2D
         
         References
         ----------
         
-        1. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
+        1. Johannes Elferich, Lingli Kong, Ximena Zottig, Nikolaus Grigorieff. (2024) CTFFIND5 provides improved insight into quality, tilt and thickness of TEM samples. bioRxiv 2024.02.26.582023; doi: https://doi.org/10.1101/2024.02.26.582023
+        2. Timothy Grant and Alexis Rohou and Nikolaus Grigorieff. (2018) cisTEM, user-friendly software for single-particle image processing. eLife 7:e35383.
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-cistem-3.8/scipion_em_cistem.egg-info/SOURCES.txt` & `scipion-em-cistem-3.9/scipion_em_cistem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.8/setup.py` & `scipion-em-cistem-3.9/setup.py`

 * *Files identical despite different names*

