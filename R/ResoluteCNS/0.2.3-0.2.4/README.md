# Comparing `tmp/resolutecns-0.2.3.tar.gz` & `tmp/resolutecns-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.2.3.tar", last modified: Wed Apr 17 23:15:36 2024, max compression
+gzip compressed data, was "resolutecns-0.2.4.tar", last modified: Wed Apr 17 23:47:23 2024, max compression
```

## Comparing `resolutecns-0.2.3.tar` & `resolutecns-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.101390 resolutecns-0.2.3/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-17 23:15:36.095388 resolutecns-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.041390 resolutecns-0.2.3/ResoluteCNS/
--rw-rw-rw-   0        0        0     7415 2024-04-17 23:15:19.000000 resolutecns-0.2.3/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.3/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.086390 resolutecns-0.2.3/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.3/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.3/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.3/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-17 23:15:36.091389 resolutecns-0.2.3/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 23:15:35.000000 resolutecns-0.2.3/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:15:36.101390 resolutecns-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-17 23:15:28.000000 resolutecns-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.021691 resolutecns-0.2.4/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:47:23.015690 resolutecns-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 23:47:22.964728 resolutecns-0.2.4/ResoluteCNS/
+-rw-rw-rw-   0        0        0     7553 2024-04-17 23:47:09.000000 resolutecns-0.2.4/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.4/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.004691 resolutecns-0.2.4/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.4/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.4/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.4/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.010689 resolutecns-0.2.4/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 23:47:23.021691 resolutecns-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-17 23:30:46.000000 resolutecns-0.2.4/setup.py
```

### Comparing `resolutecns-0.2.3/PKG-INFO` & `resolutecns-0.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.3
+Version: 0.2.4
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.3/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.2.4/ResoluteCNS/ResoluteCNS.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 import urllib
 from datetime import datetime
 from pkg_resources import resource_filename
 
 username = 'jdingman@resolutecommercial.com'
 password = 'ResComm!1'
 
-download_path = r'\\'
+
+download_filename = 'SearchResults.xlsx'
+
+
 
 class CNS:
 
     def __init__(self):
         self._logged_in = False
         self._username = username
         self._password = password
@@ -80,24 +83,28 @@
                 court_check.click()
 
 
     def click_search(self):
         self._driver.find_element(By.ID, 'button_submitbanko').click()
 
     def download_excel(self):
+        try:
+            os.remove(download_folder(download_filename))
+        except OSError:
+            pass
         self._driver.set_page_load_timeout(10)
         try:
             download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")))
             download_excel.click()
         except Exception as e:
             print(e)
 
         
         #Open the file
-        df = pd.read_excel(download_folder('SearchResults.xlsx'))
+        df = pd.read_excel(download_folder(download_filename))
         return df
 
     def get_complaints(self, states=None, counties=None, from_date=None, to_date=None, keywords=None):
         if not self._logged_in:
             self.login()
 
         now = datetime.now()
```

### Comparing `resolutecns-0.2.3/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.2.4/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.3/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.2.4/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.3/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.2.4/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.3
+Version: 0.2.4
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.3/setup.py` & `resolutecns-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.3' 
+VERSION = '0.2.4' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

