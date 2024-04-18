# Comparing `tmp/openbharatocr-0.1.1.tar.gz` & `tmp/openbharatocr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.1.1.tar", last modified: Fri Mar 29 04:05:20 2024, max compression
+gzip compressed data, was "openbharatocr-0.1.2.tar", last modified: Thu Apr 18 12:48:53 2024, max compression
```

## Comparing `openbharatocr-0.1.1.tar` & `openbharatocr-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:05:20.320231 openbharatocr-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-29 04:05:20.320231 openbharatocr-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:05:20.316231 openbharatocr-0.1.1/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:05:20.320231 openbharatocr-0.1.1/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/openbharatocr/ocr/pan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:05:20.320231 openbharatocr-0.1.1/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 04:05:20.000000 openbharatocr-0.1.1/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 04:05:20.320231 openbharatocr-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 04:05:15.000000 openbharatocr-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.238819 openbharatocr-0.1.2/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/passport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/setup.py
```

### Comparing `openbharatocr-0.1.1/LICENSE` & `openbharatocr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.1/PKG-INFO` & `openbharatocr-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,82 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.1.1
+Version: 0.1.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: opencv-python==4.6.0.66
 
 # openbharatocr
 [![Build status](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml/badge.svg)](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml)
 
-openbharatocr is an opensource python library for ocr Indian government documents 
+openbharatocr is a Python library developed as open-source, designed specifically for optical character recognition (OCR) of Indian government documents.
 
 The features of this package:
-- It will support mostly all the Indian government documents.  
+- It offers comprehensive support for the majority of Indian government documents, covering a wide range of document types. 
 
 
 #### Installation
 
 
 ```
     pip install openbharatocr
 ```
 
 
 **Pan Card**
 
-In this function, Pan card image will pass as path in the function and the output will be in dict.
+This function takes the path of a PAN card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.pan(image_path)
 ```
 
 
 **Aadhaar Card**
 
-In this function, Aadhaar Card front and back image will pass as path in the function and the output will be in dict.
+The two functions accepts the file paths of the front and back images of an Aadhaar card as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.front_aadhaar(image_path)
     dict_output = openbharatocr.back_aadhaar(image_path)
 ```
 
 **Driving Licence**
 
-In this function, Driving Licence image will pass as path in the function and the output will be in dict.
+This function takes the path of a Driving Licence card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.driving_licence(image_path)
 ```
 
+**Passport**
+
+This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
+
+```
+    import openbharatocr 
+    dict_output = openbharatocr.passport(image_path)
+```
+
 ### Contribute & support
-We are so pleased to your help and help you, If you wanna develop openbharatocr, Congrats or if you have problem, don't worry create an issue here:
+We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
 
 ### Pre Commit
-Note: Before commit your changes, run pre-commits 
+Note: Before committing your changes, run pre-commits 
 
 ```
     pre-commit run --all
 ```
```

### Comparing `openbharatocr-0.1.1/README.md` & `openbharatocr-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 # openbharatocr
 [![Build status](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml/badge.svg)](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml)
 
-openbharatocr is an opensource python library for ocr Indian government documents 
+openbharatocr is a Python library developed as open-source, designed specifically for optical character recognition (OCR) of Indian government documents.
 
 The features of this package:
-- It will support mostly all the Indian government documents.  
+- It offers comprehensive support for the majority of Indian government documents, covering a wide range of document types. 
 
 
 #### Installation
 
 
 ```
     pip install openbharatocr
 ```
 
 
 **Pan Card**
 
-In this function, Pan card image will pass as path in the function and the output will be in dict.
+This function takes the path of a PAN card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.pan(image_path)
 ```
 
 
 **Aadhaar Card**
 
-In this function, Aadhaar Card front and back image will pass as path in the function and the output will be in dict.
+The two functions accepts the file paths of the front and back images of an Aadhaar card as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.front_aadhaar(image_path)
     dict_output = openbharatocr.back_aadhaar(image_path)
 ```
 
 **Driving Licence**
 
-In this function, Driving Licence image will pass as path in the function and the output will be in dict.
+This function takes the path of a Driving Licence card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.driving_licence(image_path)
 ```
 
+**Passport**
+
+This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
+
+```
+    import openbharatocr 
+    dict_output = openbharatocr.passport(image_path)
+```
+
 ### Contribute & support
-We are so pleased to your help and help you, If you wanna develop openbharatocr, Congrats or if you have problem, don't worry create an issue here:
+We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
 
 ### Pre Commit
-Note: Before commit your changes, run pre-commits 
+Note: Before committing your changes, run pre-commits 
 
 ```
     pre-commit run --all
 ```
```

### Comparing `openbharatocr-0.1.1/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.1.2/openbharatocr/ocr/aadhaar.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.1/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.1.2/openbharatocr/ocr/driving_licence.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.1/openbharatocr/ocr/pan.py` & `openbharatocr-0.1.2/openbharatocr/ocr/pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.1/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.1.2/openbharatocr.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,82 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.1.1
+Version: 0.1.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: opencv-python==4.6.0.66
 
 # openbharatocr
 [![Build status](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml/badge.svg)](https://github.com/essentiasoftserv/openbharatocr/actions/workflows/main.yml)
 
-openbharatocr is an opensource python library for ocr Indian government documents 
+openbharatocr is a Python library developed as open-source, designed specifically for optical character recognition (OCR) of Indian government documents.
 
 The features of this package:
-- It will support mostly all the Indian government documents.  
+- It offers comprehensive support for the majority of Indian government documents, covering a wide range of document types. 
 
 
 #### Installation
 
 
 ```
     pip install openbharatocr
 ```
 
 
 **Pan Card**
 
-In this function, Pan card image will pass as path in the function and the output will be in dict.
+This function takes the path of a PAN card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.pan(image_path)
 ```
 
 
 **Aadhaar Card**
 
-In this function, Aadhaar Card front and back image will pass as path in the function and the output will be in dict.
+The two functions accepts the file paths of the front and back images of an Aadhaar card as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.front_aadhaar(image_path)
     dict_output = openbharatocr.back_aadhaar(image_path)
 ```
 
 **Driving Licence**
 
-In this function, Driving Licence image will pass as path in the function and the output will be in dict.
+This function takes the path of a Driving Licence card image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.driving_licence(image_path)
 ```
 
+**Passport**
+
+This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
+
+```
+    import openbharatocr 
+    dict_output = openbharatocr.passport(image_path)
+```
+
 ### Contribute & support
-We are so pleased to your help and help you, If you wanna develop openbharatocr, Congrats or if you have problem, don't worry create an issue here:
+We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
 
 ### Pre Commit
-Note: Before commit your changes, run pre-commits 
+Note: Before committing your changes, run pre-commits 
 
 ```
     pre-commit run --all
 ```
```

### Comparing `openbharatocr-0.1.1/setup.py` & `openbharatocr-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.1.1",
+    version="0.1.2",
     description="openbharatocr is an opensource python library for ocr Indian government documents ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

