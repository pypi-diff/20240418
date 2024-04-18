# Comparing `tmp/BoschRpaMagicBox-0.0.8.tar.gz` & `tmp/BoschRpaMagicBox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BoschRpaMagicBox-0.0.8.tar", last modified: Wed Dec 20 06:33:36 2023, max compression
+gzip compressed data, was "BoschRpaMagicBox-0.0.9.tar", last modified: Wed Dec 20 06:49:11 2023, max compression
```

## Comparing `BoschRpaMagicBox-0.0.8.tar` & `BoschRpaMagicBox-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-12-20 06:33:36.134188 BoschRpaMagicBox-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-12-14 01:12:36.000000 BoschRpaMagicBox-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      728 2023-12-20 06:33:36.131189 BoschRpaMagicBox-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-02-17 15:45:03.000000 BoschRpaMagicBox-0.0.8/README.md
--rw-rw-rw-   0        0        0      724 2023-12-20 06:32:29.000000 BoschRpaMagicBox-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-20 06:33:36.135189 BoschRpaMagicBox-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-20 06:33:36.050191 BoschRpaMagicBox-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-12-20 06:33:36.097191 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/
--rw-rw-rw-   0        0        0        0 2022-12-14 00:49:26.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/__init__.py
--rw-rw-rw-   0        0        0     3592 2023-12-20 06:19:46.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/common_config.py
--rw-rw-rw-   0        0        0    51043 2023-12-20 06:32:02.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/common_functions.py
--rw-rw-rw-   0        0        0    16681 2023-12-20 05:41:56.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/data_process_functions.py
--rw-rw-rw-   0        0        0    27278 2023-12-20 05:45:03.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/helper_functions.py
-drwxrwxrwx   0        0        0        0 2023-12-20 06:33:36.127190 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/
--rw-rw-rw-   0        0        0      728 2023-12-20 06:33:35.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-12-20 06:33:36.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-20 06:33:35.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-12-20 06:33:35.000000 BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-20 06:49:11.156746 BoschRpaMagicBox-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-12-14 01:12:36.000000 BoschRpaMagicBox-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      728 2023-12-20 06:49:11.151744 BoschRpaMagicBox-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-02-17 15:45:03.000000 BoschRpaMagicBox-0.0.9/README.md
+-rw-rw-rw-   0        0        0      724 2023-12-20 06:48:01.000000 BoschRpaMagicBox-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-12-20 06:49:11.156746 BoschRpaMagicBox-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-20 06:49:10.912747 BoschRpaMagicBox-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-12-20 06:49:11.113745 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/
+-rw-rw-rw-   0        0        0        0 2022-12-14 00:49:26.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/__init__.py
+-rw-rw-rw-   0        0        0     3592 2023-12-20 06:19:46.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/common_config.py
+-rw-rw-rw-   0        0        0    51322 2023-12-20 06:48:01.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/common_functions.py
+-rw-rw-rw-   0        0        0    16681 2023-12-20 05:41:56.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/data_process_functions.py
+-rw-rw-rw-   0        0        0    27278 2023-12-20 05:45:03.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/helper_functions.py
+drwxrwxrwx   0        0        0        0 2023-12-20 06:49:11.147744 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/
+-rw-rw-rw-   0        0        0      728 2023-12-20 06:49:10.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-12-20 06:49:10.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-20 06:49:10.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-12-20 06:49:10.000000 BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/top_level.txt
```

### Comparing `BoschRpaMagicBox-0.0.8/LICENSE` & `BoschRpaMagicBox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BoschRpaMagicBox-0.0.8/PKG-INFO` & `BoschRpaMagicBox-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BoschRpaMagicBox
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package is used for building automation functions for rpa within Bosch
 Author-email: LV Zhichao <zhichao.lv@cn.bosch.com>
 Project-URL: Homepage, https://github.boschdevcloud.com/LZV2SZH/BoschRpaMagicBox
 Project-URL: Bug Tracker, https://github.boschdevcloud.com/LZV2SZH/BoschRpaMagicBox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `BoschRpaMagicBox-0.0.8/pyproject.toml` & `BoschRpaMagicBox-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","pyperclip","selenium==4.8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BoschRpaMagicBox"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="LV Zhichao", email="zhichao.lv@cn.bosch.com" },
 ]
 description = "This package is used for building automation functions for rpa within Bosch"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/common_config.py` & `BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/common_config.py`

 * *Files identical despite different names*

### Comparing `BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/common_functions.py` & `BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.firefox.service import Service
 
 from .common_config import *
 
 
 # from selenium.webdriver.firefox.firefox_profile import FirefoxProfile
 
 
@@ -76,15 +77,15 @@
                         pass
                     else:
                         is_loop = False
                         break
             sleep(4)
 
     def initial_browser(self, has_save_folder: bool = False, save_folder_path: str = '', has_proxy: bool = True, proxy_area: str = 'hk',
-                        is_private: bool = False, is_headless=False, firefox_binary_location: str = ''):
+                        is_private: bool = False, is_headless=False, firefox_binary_location: str = '', geckodriver_binary_location: str = ''):
         """This function is used to initial FireFox browser
 
         Args:
             is_private(bool): Whether to open a private window
             has_save_folder(bool):This is the flag whether to set save folder path
             save_folder_path(str): This is the folder path of save folder
             has_proxy(bool): This is whether to use proxy when open browser
@@ -116,16 +117,19 @@
             # default download folder setting
             if has_save_folder:
                 opts.set_preference("browser.download.folderList", 2)
                 opts.set_preference("browser.download.manager.showWhenStarting", False)
                 opts.set_preference("browser.download.dir", f'{save_folder_path}')
                 opts.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/x-gzip")
                 self.save_folder_path = save_folder_path
-
-        self.browser = webdriver.Firefox(options=opts)
+        if geckodriver_binary_location:
+            service = Service(geckodriver_path)
+            self.browser = webdriver.Firefox(options=opts, service=service)
+        else:
+            self.browser = webdriver.Firefox(options=opts)
         self.wait = WebDriverWait(self.browser, 1800)
         return self.browser, self.wait
 
     def wait_page_loaded(self):
         """This function is used to wait page loaded
 
         """
```

### Comparing `BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/data_process_functions.py` & `BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/data_process_functions.py`

 * *Files identical despite different names*

### Comparing `BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox/helper_functions.py` & `BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox/helper_functions.py`

 * *Files identical despite different names*

### Comparing `BoschRpaMagicBox-0.0.8/src/BoschRpaMagicBox.egg-info/PKG-INFO` & `BoschRpaMagicBox-0.0.9/src/BoschRpaMagicBox.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BoschRpaMagicBox
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package is used for building automation functions for rpa within Bosch
 Author-email: LV Zhichao <zhichao.lv@cn.bosch.com>
 Project-URL: Homepage, https://github.boschdevcloud.com/LZV2SZH/BoschRpaMagicBox
 Project-URL: Bug Tracker, https://github.boschdevcloud.com/LZV2SZH/BoschRpaMagicBox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

