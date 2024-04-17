# Comparing `tmp/resolutecns-0.2.1.tar.gz` & `tmp/resolutecns-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.2.1.tar", last modified: Wed Apr 17 22:45:54 2024, max compression
+gzip compressed data, was "resolutecns-0.2.2.tar", last modified: Wed Apr 17 23:03:37 2024, max compression
```

## Comparing `resolutecns-0.2.1.tar` & `resolutecns-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.453108 resolutecns-0.2.1/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-17 22:45:54.447107 resolutecns-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.396105 resolutecns-0.2.1/ResoluteCNS/
--rw-rw-rw-   0        0        0     7004 2024-04-17 22:45:03.000000 resolutecns-0.2.1/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.1/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.435113 resolutecns-0.2.1/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.1/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.1/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.1/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-17 22:45:54.442105 resolutecns-0.2.1/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 22:45:54.000000 resolutecns-0.2.1/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 22:45:54.453108 resolutecns-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-17 22:45:47.000000 resolutecns-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.306706 resolutecns-0.2.2/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:03:37.291705 resolutecns-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.109527 resolutecns-0.2.2/ResoluteCNS/
+-rw-rw-rw-   0        0        0     7338 2024-04-17 23:02:45.000000 resolutecns-0.2.2/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.2.2/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.254528 resolutecns-0.2.2/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.2.2/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.2.2/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.2.2/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-17 23:03:37.278685 resolutecns-0.2.2/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 23:03:36.000000 resolutecns-0.2.2/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 23:03:37.307372 resolutecns-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-17 23:00:34.000000 resolutecns-0.2.2/setup.py
```

### Comparing `resolutecns-0.2.1/PKG-INFO` & `resolutecns-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.1
+Version: 0.2.2
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.1/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.2.2/ResoluteCNS/ResoluteCNS.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,32 +144,40 @@
             print(e)
         
         #Open the file
         df = pd.read_excel(download_folder('SearchResults.xlsx'))
         return df
 
     def set_state_filters(self, in_states):
-        states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
+        try:
+            states = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, "//input[@name='States']")))
+        except Exception as e:
+            print(e)
 
         for state in states:
             if validate_state(in_states, state):
                 state.click()
     
     def set_county_filters(self, in_counties):
         states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
         in_states = list(in_counties.keys())
 
         for state in states:
             if validate_state(in_states, state):
                 state_name = state.get_attribute('id')
                 self._driver.find_element(By.XPATH, f"//div[contains(text(), '{state_name}')][@class='statealphabutton']").click()
-                time.sleep(2)
+                time.sleep(1)
                 
                 for county in in_counties[state_name]:
-                    self._driver.find_element(By.XPATH, f"//label[contains(text(), '{county}')]").click()
+                    try:
+                        county = WebDriverWait(self._driver, 15).until(EC.presence_of_element_located((By.XPATH, f"//label[contains(text(), '{county}')]")))
+                        county.click()
+                    except Exception as e:
+                        print(e)
+                    
                 
                 self._driver.find_element(By.XPATH, f"//span[@onclick='ShowStates();']").click()
                 time.sleep(2)
         
     
     def click_search_complaints(self):
         self._driver.find_element(By.ID, 'button_submittop').click()
```

### Comparing `resolutecns-0.2.1/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.2.2/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.1/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.2.2/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.2.1/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.2.2/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.2.1
+Version: 0.2.2
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.2.1/setup.py` & `resolutecns-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1' 
+VERSION = '0.2.2' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

