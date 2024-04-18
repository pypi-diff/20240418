# Comparing `tmp/AsympDirsCalculator-1.0.8.tar.gz` & `tmp/asympdirscalculator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsympDirsCalculator-1.0.8.tar", last modified: Wed Mar  6 14:48:25 2024, max compression
+gzip compressed data, was "asympdirscalculator-1.0.9.tar", last modified: Thu Apr 18 13:31:59 2024, max compression
```

## Comparing `AsympDirsCalculator-1.0.8.tar` & `asympdirscalculator-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:25.418446 AsympDirsCalculator-1.0.8/AsympDirsCalculator/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/AsympDirsTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGCOSmacroFileGenerator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7449 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSimportingTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSrun.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2791 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSrunManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/AsympDirsCalculator/magcos_running_scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2622 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/magcos_running_scripts/AsymptoticDirection.g4mac
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator/magcos_running_scripts/runNoRewriteMAGCOSsimulation.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15552 2024-03-06 14:48:25.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-06 14:48:25.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:48:25.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-06 14:48:25.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-06 14:48:25.000000 AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15552 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:25.422446 AsympDirsCalculator-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-06 14:48:19.000000 AsympDirsCalculator-1.0.8/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/AsympDirsCalculator/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/AsympDirsTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/MAGCOSmacroFileGenerator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7449 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSimportingTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSrun.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2791 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSrunManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/AsympDirsCalculator/magcos_running_scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2622 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/magcos_running_scripts/AsymptoticDirection.g4mac
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/AsympDirsCalculator/magcos_running_scripts/runNoRewriteMAGCOSsimulation.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15552 2024-04-18 13:31:59.000000 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-18 13:31:59.000000 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:31:59.000000 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 13:31:59.000000 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 13:31:59.000000 asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15552 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:59.170689 asympdirscalculator-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-18 13:31:53.000000 asympdirscalculator-1.0.9/tests/test_basic.py
```

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/AsympDirsTools.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/AsympDirsTools.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGCOSmacroFileGenerator.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/MAGCOSmacroFileGenerator.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSimportingTools.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSimportingTools.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSrun.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSrun.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/MAGNETOCOSMICSrunManager.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/MAGNETOCOSMICSrunManager.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/globals.py` & `asympdirscalculator-1.0.9/AsympDirsCalculator/globals.py`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator/magcos_running_scripts/AsymptoticDirection.g4mac` & `asympdirscalculator-1.0.9/AsympDirsCalculator/magcos_running_scripts/AsymptoticDirection.g4mac`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/PKG-INFO` & `asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsympDirsCalculator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library containing tools for calculating asymptotic directions and vertical cut-off rigidities.
 Home-page: https://github.com/ssc-maire/AsymptoticDirectionsCalculator-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: space physics earth asymptotic trajectory geomagnetic rigidity magnetocosmics
 Description-Content-Type: text/markdown
```

### Comparing `AsympDirsCalculator-1.0.8/AsympDirsCalculator.egg-info/SOURCES.txt` & `asympdirscalculator-1.0.9/AsympDirsCalculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/LICENSE` & `asympdirscalculator-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/PKG-INFO` & `asympdirscalculator-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsympDirsCalculator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library containing tools for calculating asymptotic directions and vertical cut-off rigidities.
 Home-page: https://github.com/ssc-maire/AsymptoticDirectionsCalculator-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: space physics earth asymptotic trajectory geomagnetic rigidity magnetocosmics
 Description-Content-Type: text/markdown
```

### Comparing `AsympDirsCalculator-1.0.8/README.md` & `asympdirscalculator-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AsympDirsCalculator-1.0.8/setup.py` & `asympdirscalculator-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 setup(
     name='AsympDirsCalculator',
     packages=find_packages(exclude='tests'),
     package_data={"AsympDirsCalculator":["magcos_running_scripts/runNoRewriteMAGCOSsimulation.sh",
                                          "magcos_running_scripts/AsymptoticDirection.g4mac",
                                          ]},
-    version='1.0.8',
+    version='1.0.9',
     description='Python library containing tools for calculating asymptotic directions and vertical cut-off rigidities.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     url='https://github.com/ssc-maire/AsymptoticDirectionsCalculator-public',
     keywords = 'space physics earth asymptotic trajectory geomagnetic rigidity magnetocosmics',
```

### Comparing `AsympDirsCalculator-1.0.8/tests/test_basic.py` & `asympdirscalculator-1.0.9/tests/test_basic.py`

 * *Files identical despite different names*

