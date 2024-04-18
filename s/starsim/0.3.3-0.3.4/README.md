# Comparing `tmp/starsim-0.3.3.tar.gz` & `tmp/starsim-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsim-0.3.3.tar", last modified: Tue Apr 16 13:12:03 2024, max compression
+gzip compressed data, was "starsim-0.3.4.tar", last modified: Thu Apr 18 08:31:58 2024, max compression
```

## Comparing `starsim-0.3.3.tar` & `starsim-0.3.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.485074 starsim-0.3.3/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.3/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-16 13:12:03.485074 starsim-0.3.3/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2705 2024-03-30 07:25:13.000000 starsim-0.3.3/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-16 13:12:03.485074 starsim-0.3.3/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.3/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/connectors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       37 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/demo.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19926 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/disease.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim/diseases/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-13 20:12:07.000000 starsim-0.3.3/starsim/diseases/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9033 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/cholera.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5839 2024-04-16 13:06:22.000000 starsim-0.3.3/starsim/diseases/ebola.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/gonorrhea.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/measles.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/ncd.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/sir.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/syphilis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28830 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22027 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6688 2024-04-16 13:02:13.000000 starsim-0.3.3/starsim/modules.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42277 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/network.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/products.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/results.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15347 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/run.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7608 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/states.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-16 13:07:40.000000 starsim-0.3.3/starsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim.egg-info/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1030 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/top_level.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3550 2024-04-16 12:35:49.000000 starsim-0.3.3/tests/test_base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_baselines.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dcp.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_diseases.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dist.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dists.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_simple.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_syphilis.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.4/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-04-18 08:31:58.843789 starsim-0.3.4/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2714 2024-04-18 06:06:16.000000 starsim-0.3.4/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-18 08:31:58.843789 starsim-0.3.4/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.4/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.839789 starsim-0.3.4/starsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/connectors.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       37 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/demo.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19988 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/disease.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/starsim/diseases/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-13 20:12:07.000000 starsim-0.3.4/starsim/diseases/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8863 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/diseases/cholera.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5839 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/ebola.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/gonorrhea.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/measles.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/ncd.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/sir.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/syphilis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    29246 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/distributions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22026 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6688 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/modules.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    33433 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/network.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/products.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/results.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15346 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7750 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/states.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-18 06:07:15.000000 starsim-0.3.4/starsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/starsim.egg-info/
+-rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1030 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/top_level.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3358 2024-04-18 05:47:32.000000 starsim-0.3.4/tests/test_base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dcp.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_diseases.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dist.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dists.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_simple.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_syphilis.py
```

### Comparing `starsim-0.3.3/LICENSE` & `starsim-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/PKG-INFO` & `starsim-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.3
+Version: 0.3.4
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
@@ -28,15 +28,17 @@
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
 Installation
 ------------
 
-To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
+Starsim is most easily installed via PyPI: ``pip install starsim``.
+
+Starsim can also be installed locally. To do this, clone first this repository, then run ``pip install -e .`` (don't forget the dot at the end!).
 
 
 Usage and documentation
 -----------------------
 
 Documentation is available at https://docs.starsim.org.
```

### Comparing `starsim-0.3.3/README.rst` & `starsim-0.3.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
 Installation
 ------------
 
-To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
+Starsim is most easily installed via PyPI: ``pip install starsim``.
+
+Starsim can also be installed locally. To do this, clone first this repository, then run ``pip install -e .`` (don't forget the dot at the end!).
 
 
 Usage and documentation
 -----------------------
 
 Documentation is available at https://docs.starsim.org.
```

### Comparing `starsim-0.3.3/setup.py` & `starsim-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/__init__.py` & `starsim-0.3.4/starsim/__init__.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/connectors.py` & `starsim-0.3.4/starsim/connectors.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/demographics.py` & `starsim-0.3.4/starsim/demographics.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     def update_results(self, n_new, sim):
         self.results['new'][sim.ti] = n_new
 
     def finalize(self, sim):
         super().finalize(sim)
         self.results['cumulative'] = np.cumsum(self.results['new'])
-        self.results['cbr'] = 1/self.pars.units*np.divide(self.results['new'], sim.results['n_alive'], where=sim.results['n_alive']>0)
+        self.results['cbr'] = 1/self.pars.units*np.divide(self.results['new'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
 
 
 class Deaths(Demographics):
     def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
         """
         Configure disease-independent "background" deaths.
 
@@ -232,15 +232,15 @@
     def update_results(self, n_deaths, sim):
         self.results['new'][sim.ti] = n_deaths
         return
 
     def finalize(self, sim):
         super().finalize(sim)
         self.results['cumulative'] = np.cumsum(self.results['new'])
-        self.results['cmr'] = 1/self.pars.units*np.divide(self.results['new'], sim.results['n_alive'], where=sim.results['n_alive']>0)
+        self.results['cmr'] = 1/self.pars.units*np.divide(self.results['new'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
         return
 
 
 class Pregnancy(Demographics):
 
     def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
         super().__init__(pars, **kwargs)
@@ -447,25 +447,25 @@
 
         # Change states for the newly pregnant woman
         self.fecund[uids] = False
         self.pregnant[uids] = True
         self.ti_pregnant[uids] = sim.ti
 
         # Outcomes for pregnancies
-        dur = np.full(len(uids), sim.ti + self.pars.dur_pregnancy / sim.dt)
+        dur_preg = np.full(len(uids), self.pars.dur_pregnancy / sim.dt)
+        dur_postpartum = np.full(len(uids), self.pars.dur_postpartum / sim.dt)
         dead = self.pars.maternal_death_rate.rvs(uids)
-        self.ti_delivery[uids] = dur  # Currently assumes maternal deaths still result in a live baby
-        dur_post_partum = np.full(len(uids), dur + self.pars.dur_postpartum / sim.dt)
-        self.ti_postpartum[uids] = dur_post_partum
+        self.ti_delivery[uids] = sim.ti + dur_preg # Currently assumes maternal deaths still result in a live baby
+        self.ti_postpartum[uids] = sim.ti + dur_preg + dur_postpartum
 
         if np.any(dead): # NB: 100x faster than np.sum(), 10x faster than np.count_nonzero()
-            self.ti_dead[uids[dead]] = dur[dead]
+            self.ti_dead[uids[dead]] = sim.ti + dur_preg[dead]
         return
 
     def update_results(self, sim):
         self.results['pregnancies'][sim.ti] = np.count_nonzero(self.ti_pregnant == sim.ti)
         self.results['births'][sim.ti] = np.count_nonzero(self.ti_delivery == sim.ti)
         return
 
     def finalize(self, sim):
         super().finalize(sim)
-        self.results['cbr'] = 1/self.pars.units * np.divide(self.results['births'], sim.results['n_alive'], where=sim.results['n_alive']>0)
+        self.results['cbr'] = 1/self.pars.units * np.divide(self.results['births'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
```

### Comparing `starsim-0.3.3/starsim/disease.py` & `starsim-0.3.4/starsim/disease.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/cholera.py` & `starsim-0.3.4/starsim/diseases/cholera.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,12 +188,10 @@
             self.statesdict[state][uids] = False
         return
 
     def update_results(self, sim):
         super().update_results(sim)
         res = self.results
         ti = sim.ti
-        res.prevalence[ti]     = res.n_infected[ti] / np.count_nonzero(sim.people.alive)
-        res.new_infections[ti] = np.count_nonzero(self.ti_infected == ti)
-        res.cum_infections[ti] = np.sum(res.new_infections[:ti+1])
-        res.cum_deaths[ti]     = np.sum(res.new_deaths[:ti+1])
+        res.new_deaths[ti] = np.count_nonzero(self.ti_dead == ti)
+        res.cum_deaths[ti] = np.sum(res.new_deaths[:ti+1])
         return
```

### Comparing `starsim-0.3.3/starsim/diseases/ebola.py` & `starsim-0.3.4/starsim/diseases/ebola.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/gonorrhea.py` & `starsim-0.3.4/starsim/diseases/gonorrhea.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/hiv.py` & `starsim-0.3.4/starsim/diseases/hiv.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/measles.py` & `starsim-0.3.4/starsim/diseases/measles.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/ncd.py` & `starsim-0.3.4/starsim/diseases/ncd.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/sir.py` & `starsim-0.3.4/starsim/diseases/sir.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/diseases/syphilis.py` & `starsim-0.3.4/starsim/diseases/syphilis.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/distributions.py` & `starsim-0.3.4/starsim/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,19 @@
             else:
                 checked[seed] = dist
         return
 
     def jump(self, to=None, delta=1):
         """ Advance all RNGs, e.g. to timestep "to", by jumping """
         out = sc.autolist()
+
+        # Do not jump if centralized
+        if ss.options._centralized:
+            return out
+
         for dist in self.dists.values():
             out += dist.jump(to=to, delta=delta)
         return out
 
     def reset(self):
         """ Reset each RNG """
         out = sc.autolist()
@@ -214,15 +219,15 @@
         if kwargs:
             self.pars.update(kwargs)
             self.process_pars(call=False)
         return
 
     @property
     def bitgen(self):
-        try:    return self.rng.bit_generator
+        try:    return self.rng._bit_generator
         except: return None
     
     @property
     def state(self):
         """ Get the current state """
         try:    return self.bitgen.state
         except: return None
@@ -261,20 +266,25 @@
             r4 = dist(5)
             assert all(r1 != r2)
             assert all(r2 == r3)
             assert all(r4 == r1)
         """
         if not isinstance(state, dict):
             state = self.history[state]
-        self.rng.bit_generator.state = state.copy()
+        self.rng._bit_generator.state = state.copy()
         self.ready = True
         return self.state
 
     def jump(self, to=None, delta=1):
         """ Advance the RNG, e.g. to timestep "to", by jumping """
+        
+        # Do not jump if centralized
+        if ss.options._centralized:
+            return self.state
+
         jumps = to if (to is not None) else self.ind + delta
         self.ind = jumps
         self.reset() # First reset back to the initial state (used in case of different numbers of calls)
         if jumps: # Seems to randomize state if jumps=0
             self.bitgen.state = self.bitgen.jumped(jumps=jumps).state # Now take "jumps" number of jumps
         return self.state
     
@@ -285,15 +295,18 @@
             msg = f'Distribution {self} is already initialized, use force=True if intentional'
             ss.warn(msg)
         
         # Calculate the offset (starting seed)
         self.process_seed(trace, seed)
         
         # Create the actual RNG
-        self.rng = np.random.default_rng(seed=self.seed)
+        if ss.options._centralized:
+            self.rng = np.random.mtrand._rand # If _centralized, return the centralized numpy random number instance
+        else:
+            self.rng = np.random.default_rng(seed=self.seed)
         self.make_history(reset=True)
         
         # Handle the sim, module, and slots
         self.sim = sim if (sim is not None) else self.sim
         self.module = module if (module is not None) else self.module
         if slots is None and self.sim is not None:
             try:
@@ -446,15 +459,15 @@
         
         Args:
             n (int/tuple/arr): if an int or tuple, return this many random variables; if an array, treat as UIDs
         """
         # Check for readiness
         if not self.initialized:
             raise DistNotInitializedError(self)
-        if not self.ready and self.strict:
+        if not self.ready and self.strict and not ss.options._centralized:
             raise DistNotReadyError(self)
         
         # Figure out size, UIDs, and slots
         size, slots = self.process_size(n)
         
         # Check if size is 0, then we can return
         if size == 0:
```

### Comparing `starsim-0.3.3/starsim/interventions.py` & `starsim-0.3.4/starsim/interventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     """
     Campaign triage - an instance of base triage combined with campaign delivery.
     See base classes for a description of input arguments.
 
     **Examples**:
         # Example: In 2030, triage all positive screens into confirmatory testing
         screened_pos = lambda sim: sim.get_intervention('screening').outcomes['positive']
-        triage1 = hpv.campaign_triage(product=my_triage, eligibility=screen_pos, prob=0.9, years=2030)
+        triage1 = ss.campaign_triage(product=my_triage, eligibility=screen_pos, prob=0.9, years=2030)
     """
 
     def __init__(self, product=None, sex=None, eligibility=None,
                  prob=None, years=None, interpolate=None, annual_prob=None, **kwargs):
         BaseTriage.__init__(self, product=product, sex=sex, eligibility=eligibility, **kwargs)
         CampaignDelivery.__init__(self, prob=prob, years=years, interpolate=interpolate, annual_prob=annual_prob)
         return
```

### Comparing `starsim-0.3.3/starsim/modules.py` & `starsim-0.3.4/starsim/modules.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/network.py` & `starsim-0.3.4/starsim/network.py`

 * *Files 15% similar despite different names*

```diff
@@ -354,15 +354,15 @@
 
     def beta_per_dt(self, disease_beta=None, dt=None, uids=None):
         if uids is None: uids = Ellipsis
         return self.contacts.beta[uids] * (1 - (1 - disease_beta) ** (self.contacts.acts[uids] * dt))
 
 
 # %% Specific instances of networks
-__all__ += ['StaticNet', 'RandomNet', 'MFNet', 'MSMNet', 'EmbeddingNet', 'MaternalNet', 'HPVNet']
+__all__ += ['StaticNet', 'RandomNet', 'MFNet', 'MSMNet', 'EmbeddingNet', 'MaternalNet']
 
 
 class StaticNet(Network):
     """
     A network class of static partnerships converted from a networkx graph. There's no formation of new partnerships
     and initialized partnerships only end when one of the partners dies. The networkx graph can be created outside Starsim
     if population size is known. Or the graph can be created by passing a networkx generator function to Starsim.
@@ -430,15 +430,15 @@
 class RandomNet(DynamicNetwork):
     """ Random connectivity between agents """
 
     def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
         """ Initialize """
         pars = ss.omerge({
             'n_contacts': 10,  # Distribution or int. If int, interpreted as the mean of the dist listed in par_dists
-            'dur': 1,
+            'dur': 0,
         }, pars)
 
         super().__init__(pars=pars, key_dict=key_dict, **kwargs)
         
         # Default RNG
         self.dist = ss.Dist(distname='RandomNet')
 
@@ -787,227 +787,14 @@
         self.contacts.p1 = np.concatenate([self.contacts.p1, mother_inds])
         self.contacts.p2 = np.concatenate([self.contacts.p2, unborn_inds])
         self.contacts.beta = np.concatenate([self.contacts.beta, beta])
         self.contacts.dur = np.concatenate([self.contacts.dur, dur])
         return len(mother_inds)
 
 
-class HPVNet(MFNet):
-    """
-    WARNING: not CRN safe!
-    """
-    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
-        pars = ss.omergeleft(pars,
-            duration = 15,
-            participation = 0.9,
-            debut = 16,
-            acts = 80,
-            rel_part_rates = 1.0,
-            cross_layer = 0.05,
-            concurrency = 0.05,
-            condoms = 0.2,
-            mixing = None,
-        )
-
-        self.par_dists = ss.omergeleft(par_dists,
-            duration      = ss.lognorm,
-            participation = ss.bernoulli,
-            debut         = ss.norm,
-            acts          = ss.lognorm,
-            cross_layer   = ss.bernoulli,
-            concurrency   = ss.bernoulli,
-        )
-
-        key_dict = dict(
-            acts = ss_float_,
-            start = ss_float_,
-        )
-
-        DynamicNetwork.__init__(self, key_dict)
-        SexualNetwork.__init__(self, pars, key_dict)
-
-        super().__init__(pars, key_dict=key_dict, **kwargs)
-
-        self.get_layer_probs()
-
-        return
-
-    def initialize(self, sim):
-        super().initialize(sim)
-        return self.add_pairs(sim.people)
-
-    def update_pars(self, pars):
-        if pars is not None:
-            for k, v in pars.items():
-                self.pars[k] = v
-        return
-
-    @staticmethod
-    def participation(self, sim, uids):
-        p = np.ones_like(uids, dtype=ss_float_)
-        fem = sim.people.female[uids]
-        p[fem] = np.interp(sim.people.age[uids[fem]], self.agebins, self.f_participation)
-        p[~fem] = np.interp(sim.people.age[uids[~fem]], self.agebins, self.m_participation)
-        return p
-
-    def get_layer_probs(self):
-
-        defaults = {}
-        mixing = np.array([
-            # 0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 75+
-            [0 , 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [5 , 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [10, 0,  0, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [15, 0,  0, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [20, 0,  0, .1, .1, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [25, 0,  0, .5, .1, .5, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [30, 0,  0, 1 , .5, .5, .5, .5, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [35, 0,  0, .5, 1 , 1 , .5, 1 , 1 , .5, 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
-            [40, 0,  0, 0 , .5, 1 , 1 , 1 , 1 , 1 , .5, 0 , 0 , 0 , 0 , 0 , 0] ,
-            [45, 0,  0, 0 , 0 , .1, 1 , 1 , 2 , 1 , 1 , .5, 0 , 0 , 0 , 0 , 0] ,
-            [50, 0,  0, 0 , 0 , 0 , .1, 1 , 1 , 1 , 1 , 2 , .5, 0 , 0 , 0 , 0] ,
-            [55, 0,  0, 0 , 0 , 0 , 0 , .1, 1 , 1 , 1 , 1 , 2 , .5, 0 , 0 , 0] ,
-            [60, 0,  0, 0 , 0 , 0 , 0 , 0 , .1, .5, 1 , 1 , 1 , 2 , .5, 0 , 0] ,
-            [65, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 2 , .5, 0] ,
-            [70, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 1 , .5],
-            [75, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 1] ,
-        ])
-
-        defaults['mixing'] = mixing
-
-        for pkey, pval in defaults.items():
-            if self.pars[pkey] is None:
-                self.pars[pkey] = pval
-
-        return
-
-    def set_participation(self, people, upper_age=None):
-        if upper_age is None:
-            uids = people.uid
-        else:
-            uids = people.uid[(people.age < upper_age)]
-
-        # Compute number of partners
-        f_partnered_inds, f_partnered_counts = np.unique(self.contacts.p1, return_counts=True)
-        m_partnered_inds, m_partnered_counts = np.unique(self.contacts.p2, return_counts=True)
-        current_partners = np.zeros((len(people)))
-        current_partners[f_partnered_inds] = f_partnered_counts
-        current_partners[m_partnered_inds] = m_partnered_counts
-        partners = self.pars.partner_dist.rvs(len(people)) + 1
-        underpartnered = current_partners < partners  # Indices of underpartnered people
-
-        # Set people who will participate in the network at some point
-        can_participate = ss.true(self.active(people) * underpartnered)
-        self.participant[uids] = self.pars.participation_dist.rvs(can_participate)
-        return
-
-    def add_pairs(self, people, ti=0):
-        participating = ss.true(
-            self.participant)  # Will be the same people each time, with participation decided once per person
-        f = participating[people.female[participating]]
-        m = participating[~people.female[participating]]
-
-        # Create preference matrix between eligible females and males that combines age and geo mixing
-        age_bins_f = np.digitize(people.age[f],
-                                 bins=self.agebins) - 1  # Age bins of females that are entering new relationships
-        age_bins_m = np.digitize(people.age[m], bins=self.agebins) - 1  # Age bins of active and participating males
-        age_f, age_m = np.meshgrid(age_bins_f, age_bins_m)
-        pair_probs = self.pars.mixing[age_m, age_f + 1]
-
-        f_to_remove = pair_probs.max(axis=0) == 0  # list of female inds to remove if no male partners are found for her
-        # f = [i for i, flag in zip(f, f_to_remove) if ~flag]  # remove the inds who don't get paired on this timestep
-        f = f[~f_to_remove]
-        selected_males = []
-        if len(f):
-            pair_probs = pair_probs[:, np.invert(f_to_remove)]
-            choices = []
-            fems = np.arange(len(f))
-            f_paired_bools = np.full(len(fems), True, dtype=bool)
-            np.random.shuffle(fems)  # TODO: Stream-ify?
-            for fem in fems:
-                m_col = pair_probs[:, fem]
-                if m_col.sum() > 0:
-                    m_col_norm = m_col / m_col.sum()
-                    choice = np.random.choice(len(m_col_norm), p=m_col_norm)  # TODO: Stream-ify?
-                    choices.append(choice)
-                    pair_probs[choice, :] = 0  # Once male partner is assigned, remove from eligible pool
-                else:
-                    f_paired_bools[fem] = False
-            selected_males = m[np.array(choices).flatten()]
-            f = f[f_paired_bools]
-
-        p1 = selected_males
-        p2 = f
-        n_partnerships = len(p2)
-        dur = self.pars.duration.rvs(n_partnerships)
-        acts = self.pars.acts.rvs(n_partnerships)
-        age_p1 = people.age[p1]
-        age_p2 = people.age[p2]
-
-        age_debut_p1 = self.debut[p1] # TODO: Check that this still works - it was previously people.debut
-        age_debut_p2 = self.debut[p2]
-
-        # For each couple, get the average age they are now and the average age of debut
-        avg_age = np.array([age_p1, age_p2]).mean(axis=0)
-        avg_debut = np.array([age_debut_p1, age_debut_p2]).mean(axis=0)
-
-        # Shorten parameter names
-        aap = self.pars.age_act_pars
-        dr = aap['debut_ratio']
-        peak = aap['peak']
-        rr = aap['retirement_ratio']
-        retire = aap['retirement']
-        peak = aap['peak']
-
-        # Get indices of people at different stages
-        below_peak_inds = avg_age <= peak
-        above_peak_inds = (avg_age > peak) & (avg_age < retire)
-        retired_inds = avg_age > retire
-
-        # Set values by linearly scaling the number of acts for each partnership according to
-        # the age of the couple at the commencement of the relationship
-        below_peak_vals = acts[below_peak_inds] * (dr + (1 - dr) / (peak - avg_debut[below_peak_inds]) * (
-                avg_age[below_peak_inds] - avg_debut[below_peak_inds]))
-        above_peak_vals = acts[above_peak_inds] * (
-                rr + (1 - rr) / (peak - retire) * (avg_age[above_peak_inds] - retire))
-        retired_vals = 0
-
-        # Set values and return
-        scaled_acts = np.full(len(acts), np.nan, dtype=ss_float_)
-        scaled_acts[below_peak_inds] = below_peak_vals
-        scaled_acts[above_peak_inds] = above_peak_vals
-        scaled_acts[retired_inds] = retired_vals
-        start = np.array([ti] * n_partnerships, dtype=ss_float_)
-        beta = np.ones(n_partnerships)
-
-        new_contacts = dict(
-            p1=p1,
-            p2=p2,
-            dur=dur,
-            acts=scaled_acts,
-            start=start,
-            beta=beta
-        )
-        self.append(new_contacts)
-        return len(new_contacts)
-
-    def update(self, people, ti=None, dt=None):
-        if ti is None: ti = people.ti
-        if dt is None: dt = people.dt
-        # First remove any relationships due to end
-        self.contacts.dur = self.contacts.dur - dt
-        active = self.contacts.dur > 0
-        for key in self.meta.keys():
-            self.contacts[key] = self.contacts[key][active]
-
-        # Then add new relationships
-        self.add_pairs(people, ti=ti)
-        return
-
-
 # %% Network connectors
 __all__ += ['NetworkConnector', 'MF_MSM']
 
 class NetworkConnector(ss.Module):
     """
     Template for a connector between networks.
     """
```

### Comparing `starsim-0.3.3/starsim/parameters.py` & `starsim-0.3.4/starsim/parameters.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/people.py` & `starsim-0.3.4/starsim/people.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/products.py` & `starsim-0.3.4/starsim/products.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/results.py` & `starsim-0.3.4/starsim/results.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/run.py` & `starsim-0.3.4/starsim/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
             sims.append(sim)
 
     return sims
 
 
 def parallel(*args, **kwargs):
     """
-    A shortcut to ``hpv.MultiSim()``, allowing the quick running of multiple simulations
+    A shortcut to ``ss.MultiSim()``, allowing the quick running of multiple simulations
     at once.
 
     Args:
         args (list): The simulations to run
         kwargs (dict): passed to multi_run()
 
     Returns:
```

### Comparing `starsim-0.3.3/starsim/samples.py` & `starsim-0.3.4/starsim/samples.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/settings.py` & `starsim-0.3.4/starsim/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
 
         optdesc.sep = 'Set thousands seperator for text output'
         options.sep = str(os.getenv('STARSIM_SEP', ','))
 
         optdesc.precision = 'Set arithmetic precision -- 32-bit by default for efficiency'
         options.precision = int(os.getenv('STARSIM_PRECISION', 64))
 
+        optdesc._centralized = 'If True, revert to centralized random number generation (NOT ADVISED).'
+        options._centralized = False
+
         return optdesc, options
 
     def __call__(self, *args, **kwargs):
         """Allow ``ss.options(dpi=150)`` instead of ``ss.options.set(dpi=150)`` """
 
         return self.set(*args, **kwargs)
```

### Comparing `starsim-0.3.3/starsim/sim.py` & `starsim-0.3.4/starsim/sim.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/states.py` & `starsim-0.3.4/starsim/states.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim/utils.py` & `starsim-0.3.4/starsim/utils.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/starsim.egg-info/PKG-INFO` & `starsim-0.3.4/starsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.3
+Version: 0.3.4
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
@@ -28,15 +28,17 @@
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
 Installation
 ------------
 
-To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
+Starsim is most easily installed via PyPI: ``pip install starsim``.
+
+Starsim can also be installed locally. To do this, clone first this repository, then run ``pip install -e .`` (don't forget the dot at the end!).
 
 
 Usage and documentation
 -----------------------
 
 Documentation is available at https://docs.starsim.org.
```

### Comparing `starsim-0.3.3/starsim.egg-info/SOURCES.txt` & `starsim-0.3.4/starsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_base.py` & `starsim-0.3.4/tests/test_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,20 +46,14 @@
     sim = ss.Sim()
     sim.initialize()
     
     nw3 = ss.MaternalNet()
     nw3.initialize(sim)
     nw3.add_pairs(mother_inds=[1, 2, 3], unborn_inds=[100, 101, 102], dur=[1, 1, 1])
 
-    # HPV NETWORK - NOT FUNCTIONAL
-    # nw3 = ss.hpv_network()
-    # nw3.initialize(sim)
-    # sim.people.networks.update(sim.people)  # Update by providing a timestep & current time index
-
-
     return nw1, nw2, nw3
 
 
 def test_microsim(do_plot=False):
     sc.heading('Test making people and providing them to a sim')
 
     # Make HIV module
```

### Comparing `starsim-0.3.3/tests/test_baselines.py` & `starsim-0.3.4/tests/test_baselines.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_dcp.py` & `starsim-0.3.4/tests/test_dcp.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_demographics.py` & `starsim-0.3.4/tests/test_demographics.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_diseases.py` & `starsim-0.3.4/tests/test_diseases.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_dist.py` & `starsim-0.3.4/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_dists.py` & `starsim-0.3.4/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_samples.py` & `starsim-0.3.4/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_simple.py` & `starsim-0.3.4/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.3/tests/test_syphilis.py` & `starsim-0.3.4/tests/test_syphilis.py`

 * *Files identical despite different names*

