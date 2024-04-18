# Comparing `tmp/resolutecns-0.2.4.tar.gz` & `tmp/resolutecns-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.2.4.tar", last modified: Wed Apr 17 23:47:23 2024, max compression
+gzip compressed data, was "resolutecns-0.2.5.tar", last modified: Thu Apr 18 00:00:34 2024, max compression
```

## Comparing `resolutecns-0.2.4.tar` & `resolutecns-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.021691 resolutecns-0.2.4/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-17 23:47:23.015690 resolutecns-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 23:47:22.964728 resolutecns-0.2.4/ResoluteCNS/
--rw-rw-rw-   0        0        0     7553 2024-04-17 23:47:09.000000 resolutecns-0.2.4/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.4/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.004691 resolutecns-0.2.4/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.4/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.4/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.4/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-17 23:47:23.010689 resolutecns-0.2.4/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 23:47:22.000000 resolutecns-0.2.4/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:47:23.021691 resolutecns-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-17 23:30:46.000000 resolutecns-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:00:34.644936 resolutecns-0.2.5/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-18 00:00:34.637933 resolutecns-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 00:00:34.588721 resolutecns-0.2.5/ResoluteCNS/
+-rw-rw-rw-   0        0        0     7392 2024-04-18 00:00:15.000000 resolutecns-0.2.5/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.5/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:00:34.625720 resolutecns-0.2.5/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.5/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.5/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.5/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-18 00:00:34.632934 resolutecns-0.2.5/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-18 00:00:34.000000 resolutecns-0.2.5/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-18 00:00:34.000000 resolutecns-0.2.5/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 00:00:34.000000 resolutecns-0.2.5/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 00:00:34.000000 resolutecns-0.2.5/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 00:00:34.000000 resolutecns-0.2.5/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 00:00:34.645932 resolutecns-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-18 00:00:27.000000 resolutecns-0.2.5/setup.py
```

### Comparing `resolutecns-0.2.4/PKG-INFO` & `resolutecns-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.4
+Version: 0.2.5
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.4/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.2.5/ResoluteCNS/ResoluteCNS.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,30 +82,17 @@
                 court_check = self._driver.find_element(By.ID, court.get_attribute('for'))
                 court_check.click()
 
 
     def click_search(self):
         self._driver.find_element(By.ID, 'button_submitbanko').click()
 
-    def download_excel(self):
-        try:
-            os.remove(download_folder(download_filename))
-        except OSError:
-            pass
-        self._driver.set_page_load_timeout(10)
-        try:
-            download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")))
-            download_excel.click()
-        except Exception as e:
-            print(e)
-
-        
-        #Open the file
-        df = pd.read_excel(download_folder(download_filename))
-        return df
+    def download_excel_bankruptcies(self):
+        return self.download_excel("//a[@href='/SearchBeta/GetBankoExcel']/child::img")
+                
 
     def get_complaints(self, states=None, counties=None, from_date=None, to_date=None, keywords=None):
         if not self._logged_in:
             self.login()
 
         now = datetime.now()
         
@@ -137,25 +124,28 @@
 
         return self.download_excel_complaints()
 
     def setup_keyword_filters(self, keywords):
         keyword_field = self._driver.find_element(By.NAME, 'Summary')
         keyword_field.send_keys(keywords)
     
-
     def download_excel_complaints(self):
+        return self.download_excel("//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")
+
+    def download_excel(self, download_search):
+        delete_file_if_exists(download_folder(download_filename))
         self._driver.set_page_load_timeout(10)
         try:
-            download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")))
+            download_excel = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, download_search)))
             download_excel.click()
         except Exception as e:
             print(e)
         
         #Open the file
-        df = pd.read_excel(download_folder('SearchResults.xlsx'))
+        df = pd.read_excel(download_folder(download_filename))
         return df
 
     def set_state_filters(self, in_states):
         try:
             WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//input[@name='States']")))
             states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
         except Exception as e:
@@ -206,8 +196,14 @@
     return result
 
 def validate_court(in_courts, court_to_check):
         result = False
         for c in in_courts:
             if c == court_to_check.text:
                 result = True
-        return result
+        return result
+
+def delete_file_if_exists(file):
+    try:
+        os.remove(file)
+    except OSError:
+        pass
```

### Comparing `resolutecns-0.2.4/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.2.5/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.4/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.2.5/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.4/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.2.5/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.4
+Version: 0.2.5
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.4/setup.py` & `resolutecns-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4' 
+VERSION = '0.2.5' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

