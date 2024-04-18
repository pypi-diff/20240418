# Comparing `tmp/atmosphericRadiationDoseAndFlux-1.0.3.tar.gz` & `tmp/atmosphericradiationdoseandflux-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmosphericRadiationDoseAndFlux-1.0.3.tar", last modified: Wed Mar  6 14:51:22 2024, max compression
+gzip compressed data, was "atmosphericradiationdoseandflux-1.0.4.tar", last modified: Thu Apr 18 13:19:36 2024, max compression
```

## Comparing `atmosphericRadiationDoseAndFlux-1.0.3.tar` & `atmosphericradiationdoseandflux-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.635441 atmosphericRadiationDoseAndFlux-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-03-06 14:51:22.635441 atmosphericRadiationDoseAndFlux-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/adose.rpf
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/dosee.rpf
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/edose.rpf
--rw-r--r--   0 runner    (1001) docker     (127)   205637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/neutron.rpf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/adose.rpf
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/dosee.rpf
--rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/edose.rpf
--rw-r--r--   0 runner    (1001) docker     (127)   205637 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/neutron.rpf
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/doseAndFluxCalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/particle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/particleResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/responseFileParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-03-06 14:51:22.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-06 14:51:22.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:51:22.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-06 14:51:22.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 14:51:22.000000 atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 14:51:22.635441 atmosphericRadiationDoseAndFlux-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:22.631441 atmosphericRadiationDoseAndFlux-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-06 14:51:15.000000 atmosphericRadiationDoseAndFlux-1.0.3/tests/test_general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.551450 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.551450 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.551450 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/adose.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/dosee.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/edose.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)   205637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/neutron.rpf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/adose.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/dosee.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)    68637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/edose.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)   205637 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/neutron.rpf
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/doseAndFluxCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/particle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/particleResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/responseFileParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-18 13:19:36.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 13:19:36.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:19:36.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 13:19:36.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:19:36.000000 atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:36.555450 atmosphericradiationdoseandflux-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-18 13:19:31.000000 atmosphericradiationdoseandflux-1.0.4/tests/test_general.py
```

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/LICENSE` & `atmosphericradiationdoseandflux-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/PKG-INFO` & `atmosphericradiationdoseandflux-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmosphericRadiationDoseAndFlux
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library for calculating doses and fluxes at a particular altitude given an input spectrum
 Home-page: https://github.com/ssc-maire/DoseAndFluxCalculator
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: atmosphere radiation space weather cosmic rays spectrum alpha particles yield response dose rates ambient effective GLE sun solar aviation neutron monitor
 Description-Content-Type: text/markdown
```

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/README.md` & `atmosphericradiationdoseandflux-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/adose.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/adose.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/dosee.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/dosee.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/edose.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/edose.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/alpha/neutron.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/alpha/neutron.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/adose.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/adose.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/dosee.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/dosee.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/edose.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/edose.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/data/proton/neutron.rpf` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/data/proton/neutron.rpf`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/doseAndFluxCalculator.py` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/doseAndFluxCalculator.py`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/particleResponse.py` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/particleResponse.py`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/responseFileParameters.py` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/responseFileParameters.py`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux/settings.py` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux/settings.py`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/PKG-INFO` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmosphericRadiationDoseAndFlux
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library for calculating doses and fluxes at a particular altitude given an input spectrum
 Home-page: https://github.com/ssc-maire/DoseAndFluxCalculator
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: atmosphere radiation space weather cosmic rays spectrum alpha particles yield response dose rates ambient effective GLE sun solar aviation neutron monitor
 Description-Content-Type: text/markdown
```

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/atmosphericRadiationDoseAndFlux.egg-info/SOURCES.txt` & `atmosphericradiationdoseandflux-1.0.4/atmosphericRadiationDoseAndFlux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/setup.py` & `atmosphericradiationdoseandflux-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='atmosphericRadiationDoseAndFlux',
     packages=find_packages(exclude='tests'),
     package_data={"atmosphericRadiationDoseAndFlux":["atmosphericRadiationDoseAndFlux/data/proton/*.rpf","atmosphericRadiationDoseAndFlux/data/alpha/*.rpf"]},
     include_package_data=True,
-    version='1.0.3',
+    version='1.0.4',
     description='Python library for calculating doses and fluxes at a particular altitude given an input spectrum',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     url='https://github.com/ssc-maire/DoseAndFluxCalculator',
     keywords = 'atmosphere radiation space weather cosmic rays spectrum alpha particles yield response dose rates ambient effective GLE sun solar aviation neutron monitor',
```

### Comparing `atmosphericRadiationDoseAndFlux-1.0.3/tests/test_general.py` & `atmosphericradiationdoseandflux-1.0.4/tests/test_general.py`

 * *Files identical despite different names*

