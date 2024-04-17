# Comparing `tmp/resolutecns-0.1.8.tar.gz` & `tmp/resolutecns-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.8.tar", last modified: Tue Apr 16 22:14:07 2024, max compression
+gzip compressed data, was "resolutecns-0.1.9.tar", last modified: Tue Apr 16 22:24:22 2024, max compression
```

## Comparing `resolutecns-0.1.8.tar` & `resolutecns-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 22:14:07.905913 resolutecns-0.1.8/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 22:14:07.900916 resolutecns-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 22:14:07.854869 resolutecns-0.1.8/ResoluteCNS/
--rw-rw-rw-   0        0        0     6144 2024-04-16 22:13:56.000000 resolutecns-0.1.8/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.8/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:14:07.888914 resolutecns-0.1.8/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.8/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.8/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.8/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 22:14:07.895916 resolutecns-0.1.8/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 22:14:07.000000 resolutecns-0.1.8/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 22:14:07.000000 resolutecns-0.1.8/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 22:14:07.000000 resolutecns-0.1.8/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 22:14:07.000000 resolutecns-0.1.8/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 22:14:07.000000 resolutecns-0.1.8/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 22:14:07.905913 resolutecns-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 22:14:04.000000 resolutecns-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.038633 resolutecns-0.1.9/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-16 22:24:22.033634 resolutecns-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 22:24:21.985634 resolutecns-0.1.9/ResoluteCNS/
+-rw-rw-rw-   0        0        0     6167 2024-04-16 22:24:10.000000 resolutecns-0.1.9/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.9/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.022635 resolutecns-0.1.9/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.9/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.9/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.9/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.028632 resolutecns-0.1.9/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 22:24:22.038633 resolutecns-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-16 22:24:15.000000 resolutecns-0.1.9/setup.py
```

### Comparing `resolutecns-0.1.8/PKG-INFO` & `resolutecns-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.8
+Version: 0.1.9
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.8/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.1.9/ResoluteCNS/ResoluteCNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
         if states:
             self.set_state_filters(states)
         if counties:
             self.set_county_filters(counties)
         
         self.click_search_complaints()
+        time.sleep(2)
 
         return self.download_excel_complaints()
 
 
     def download_excel_complaints(self):
         self._driver.set_page_load_timeout(10)
         try:
```

### Comparing `resolutecns-0.1.8/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.1.9/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.8/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.1.9/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.8/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.9/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.8
+Version: 0.1.9
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.8/setup.py` & `resolutecns-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.8' 
+VERSION = '0.1.9' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

