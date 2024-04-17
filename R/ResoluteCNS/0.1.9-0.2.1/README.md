# Comparing `tmp/resolutecns-0.1.9.tar.gz` & `tmp/resolutecns-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.9.tar", last modified: Tue Apr 16 22:24:22 2024, max compression
+gzip compressed data, was "resolutecns-0.2.1.tar", last modified: Wed Apr 17 22:45:54 2024, max compression
```

## Comparing `resolutecns-0.1.9.tar` & `resolutecns-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.038633 resolutecns-0.1.9/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 22:24:22.033634 resolutecns-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 22:24:21.985634 resolutecns-0.1.9/ResoluteCNS/
--rw-rw-rw-   0        0        0     6167 2024-04-16 22:24:10.000000 resolutecns-0.1.9/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.9/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.022635 resolutecns-0.1.9/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.9/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.9/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.9/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 22:24:22.028632 resolutecns-0.1.9/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 22:24:21.000000 resolutecns-0.1.9/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 22:24:22.038633 resolutecns-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 22:24:15.000000 resolutecns-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.453108 resolutecns-0.2.1/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-17 22:45:54.447107 resolutecns-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.396105 resolutecns-0.2.1/ResoluteCNS/
+-rw-rw-rw-   0        0        0     7004 2024-04-17 22:45:03.000000 resolutecns-0.2.1/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.1/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.435113 resolutecns-0.2.1/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.1/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.1/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.1/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.442105 resolutecns-0.2.1/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 22:45:54.453108 resolutecns-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-17 22:45:47.000000 resolutecns-0.2.1/setup.py
```

### Comparing `resolutecns-0.1.9/PKG-INFO` & `resolutecns-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.9
+Version: 0.2.1
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.9/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.2.1/ResoluteCNS/ResoluteCNS.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 #importing webdriver from selenium 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver import FirefoxOptions
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
 import time
 import pandas as pd
 import platform
 from os.path import expanduser
 import os
 import urllib
 from datetime import datetime
 from pkg_resources import resource_filename
 
 username = 'jdingman@resolutecommercial.com'
 password = 'ResComm!1'
 
+download_path = r'\\'
 
 class CNS:
 
     def __init__(self):
         self._logged_in = False
         self._username = username
         self._password = password
         self._opts = FirefoxOptions()
+        # self._opts.set_preference("browser.download.dir", download_path)
+        # self._opts.set_preference("browser.download.folderList", 2)
+        # self._opts.set_preference("browser.download.useDownloadDir", True)
+        
         self._ublock_path = resource_filename('ResoluteCNS', 'uBlock0.xpi')
         self._driver = None
         
 
     def login(self):
         self._driver = webdriver.Firefox(options=self._opts)
         self._driver.install_addon(self._ublock_path, temporary=True)
@@ -75,55 +82,67 @@
 
     def click_search(self):
         self._driver.find_element(By.ID, 'button_submitbanko').click()
 
     def download_excel(self):
         self._driver.set_page_load_timeout(10)
         try:
-            download_excel = self._driver.find_element(By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")
+            download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")))
             download_excel.click()
         except Exception as e:
             print(e)
+
         
         #Open the file
         df = pd.read_excel(download_folder('SearchResults.xlsx'))
         return df
 
-    def get_complaints(self, states=None, counties=None, from_date=None, to_date=None):
+    def get_complaints(self, states=None, counties=None, from_date=None, to_date=None, keywords=None):
         if not self._logged_in:
             self.login()
 
         now = datetime.now()
         
         if not from_date:
             from_date = now.strftime("%m/%d/%Y")
         if not to_date:
-            from_date = now.strftime("%m/%d/%Y")
+            to_date = now.strftime("%m/%d/%Y")
 
         #URL of the website     
         url = self._baseurl + "SearchBeta/Complaints"
         self._driver.get(url)
         time.sleep(1)
         self.setup_date_filters(from_date, to_date)
 
         if states:
+            time.sleep(2)
             self.set_state_filters(states)
         if counties:
+            time.sleep(2)
             self.set_county_filters(counties)
+
+        if keywords:
+            time.sleep(1)
+            self.setup_keyword_filters(keywords)
         
+        time.sleep(1)
         self.click_search_complaints()
-        time.sleep(2)
+        time.sleep(10)
 
         return self.download_excel_complaints()
 
+    def setup_keyword_filters(self, keywords):
+        keyword_field = self._driver.find_element(By.NAME, 'Summary')
+        keyword_field.send_keys(keywords)
+    
 
     def download_excel_complaints(self):
         self._driver.set_page_load_timeout(10)
         try:
-            download_excel = self._driver.find_element(By.XPATH, "//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")
+            download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")))
             download_excel.click()
         except Exception as e:
             print(e)
         
         #Open the file
         df = pd.read_excel(download_folder('SearchResults.xlsx'))
         return df
```

### Comparing `resolutecns-0.1.9/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.2.1/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.9/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.2.1/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.9/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.2.1/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.9
+Version: 0.2.1
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.9/setup.py` & `resolutecns-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.9' 
+VERSION = '0.2.1' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

