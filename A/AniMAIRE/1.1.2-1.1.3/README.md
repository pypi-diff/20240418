# Comparing `tmp/AniMAIRE-1.1.2.tar.gz` & `tmp/animaire-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AniMAIRE-1.1.2.tar", last modified: Sat Mar 30 01:51:57 2024, max compression
+gzip compressed data, was "animaire-1.1.3.tar", last modified: Thu Apr 18 14:46:27 2024, max compression
```

## Comparing `AniMAIRE-1.1.2.tar` & `animaire-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.184473 AniMAIRE-1.1.2/AniMAIRE/
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/AniMAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.184473 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/dose_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/AniMAIRE/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/AniMAIRE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27993 2024-03-30 01:51:57.000000 AniMAIRE-1.1.2/AniMAIRE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-30 01:51:57.000000 AniMAIRE-1.1.2/AniMAIRE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 01:51:57.000000 AniMAIRE-1.1.2/AniMAIRE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-30 01:51:57.000000 AniMAIRE-1.1.2/AniMAIRE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 01:51:57.000000 AniMAIRE-1.1.2/AniMAIRE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27993 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27141 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/pytests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/pytests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/pytests/test_anisotropic_MAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 01:51:57.188473 AniMAIRE-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-30 01:51:49.000000 AniMAIRE-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.314966 animaire-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.310966 animaire-1.1.3/AniMAIRE/
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/AniMAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.310966 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.310966 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.314966 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/dose_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-18 14:46:22.000000 animaire-1.1.3/AniMAIRE/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.314966 animaire-1.1.3/AniMAIRE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27993 2024-04-18 14:46:27.000000 animaire-1.1.3/AniMAIRE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 14:46:27.000000 animaire-1.1.3/AniMAIRE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:46:27.000000 animaire-1.1.3/AniMAIRE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 14:46:27.000000 animaire-1.1.3/AniMAIRE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 14:46:27.000000 animaire-1.1.3/AniMAIRE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 14:46:22.000000 animaire-1.1.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 14:46:22.000000 animaire-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27993 2024-04-18 14:46:27.314966 animaire-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27141 2024-04-18 14:46:22.000000 animaire-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:27.314966 animaire-1.1.3/pytests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:22.000000 animaire-1.1.3/pytests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-18 14:46:22.000000 animaire-1.1.3/pytests/test_anisotropic_MAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:46:27.314966 animaire-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-18 14:46:22.000000 animaire-1.1.3/setup.py
```

### Comparing `AniMAIRE-1.1.2/AniMAIRE/AniMAIRE.py` & `animaire-1.1.3/AniMAIRE/AniMAIRE.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py` & `animaire-1.1.3/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/dose_plotting.py` & `animaire-1.1.3/AniMAIRE/dose_plotting.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE/utils.py` & `animaire-1.1.3/AniMAIRE/utils.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/AniMAIRE.egg-info/PKG-INFO` & `animaire-1.1.3/AniMAIRE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
```

### Comparing `AniMAIRE-1.1.2/AniMAIRE.egg-info/SOURCES.txt` & `animaire-1.1.3/AniMAIRE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/LICENCE` & `animaire-1.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/PKG-INFO` & `animaire-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
```

### Comparing `AniMAIRE-1.1.2/README.md` & `animaire-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/pytests/test_anisotropic_MAIRE.py` & `animaire-1.1.3/pytests/test_anisotropic_MAIRE.py`

 * *Files identical despite different names*

### Comparing `AniMAIRE-1.1.2/setup.py` & `animaire-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='AniMAIRE',
     packages=find_packages(exclude='pytests'),
     package_data={"AniMAIRE":[
                                 "anisotropic_MAIRE_engine/data/*.csv"
                                          ]},
-    version='1.1.2',
+    version='1.1.3',
     description='Python library for running the anisotropic version of MAIRE+',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     license='GNU General Public License v3.0',
     url='https://github.com/ssc-maire/AniMAIRE-public',
```

