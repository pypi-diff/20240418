# Comparing `tmp/resolutecns-0.2.2.tar.gz` & `tmp/resolutecns-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.2.2.tar", last modified: Wed Apr 17 23:03:37 2024, max compression
+gzip compressed data, was "resolutecns-0.2.3.tar", last modified: Wed Apr 17 23:15:36 2024, max compression
```

## Comparing `resolutecns-0.2.2.tar` & `resolutecns-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.306706 resolutecns-0.2.2/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-17 23:03:37.291705 resolutecns-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.109527 resolutecns-0.2.2/ResoluteCNS/
--rw-rw-rw-   0        0        0     7338 2024-04-17 23:02:45.000000 resolutecns-0.2.2/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.2/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.254528 resolutecns-0.2.2/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.2/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.2/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.2/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.278685 resolutecns-0.2.2/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:03:37.307372 resolutecns-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-17 23:00:34.000000 resolutecns-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.101390 resolutecns-0.2.3/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:15:36.095388 resolutecns-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.041390 resolutecns-0.2.3/ResoluteCNS/
+-rw-rw-rw-   0        0        0     7415 2024-04-17 23:15:19.000000 resolutecns-0.2.3/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.3/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.086390 resolutecns-0.2.3/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.3/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.3/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.3/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.091389 resolutecns-0.2.3/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 23:15:36.101390 resolutecns-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-17 23:15:28.000000 resolutecns-0.2.3/setup.py
```

### Comparing `resolutecns-0.2.2/PKG-INFO` & `resolutecns-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.2
+Version: 0.2.3
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.2/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.2.3/ResoluteCNS/ResoluteCNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,16 @@
         
         #Open the file
         df = pd.read_excel(download_folder('SearchResults.xlsx'))
         return df
 
     def set_state_filters(self, in_states):
         try:
-            states = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//input[@name='States']")))
+            WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//input[@name='States']")))
+            states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
         except Exception as e:
             print(e)
 
         for state in states:
             if validate_state(in_states, state):
                 state.click()
```

### Comparing `resolutecns-0.2.2/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.2.3/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.2/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.2.3/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.2/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.2.3/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.2
+Version: 0.2.3
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.2/setup.py` & `resolutecns-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2' 
+VERSION = '0.2.3' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

