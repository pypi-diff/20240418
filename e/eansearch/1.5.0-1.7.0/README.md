# Comparing `tmp/eansearch-1.5.0.tar.gz` & `tmp/eansearch-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eansearch-1.5.0.tar", last modified: Thu Mar  3 14:14:49 2022, max compression
+gzip compressed data, was "eansearch-1.7.0.tar", last modified: Thu Apr 18 19:11:24 2024, max compression
```

## Comparing `eansearch-1.5.0.tar` & `eansearch-1.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-03-03 14:14:49.812367 eansearch-1.5.0/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1118 2020-03-24 11:35:43.000000 eansearch-1.5.0/LICENSE
--rw-rw-r--   0 jan       (1000) jan       (1000)     2436 2022-03-03 14:14:49.812367 eansearch-1.5.0/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     1147 2021-03-04 22:06:14.000000 eansearch-1.5.0/README.md
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-03-03 14:14:49.808367 eansearch-1.5.0/eansearch.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)     2436 2022-03-03 14:14:49.000000 eansearch-1.5.0/eansearch.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)      171 2022-03-03 14:14:49.000000 eansearch-1.5.0/eansearch.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2022-03-03 14:14:49.000000 eansearch-1.5.0/eansearch.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       10 2022-03-03 14:14:49.000000 eansearch-1.5.0/eansearch.egg-info/top_level.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)     2421 2022-03-03 14:08:32.000000 eansearch-1.5.0/eansearch.py
--rw-rw-r--   0 jan       (1000) jan       (1000)       38 2022-03-03 14:14:49.812367 eansearch-1.5.0/setup.cfg
--rw-rw-r--   0 jan       (1000) jan       (1000)     1546 2022-03-03 14:08:48.000000 eansearch-1.5.0/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 19:11:24.484347 eansearch-1.7.0/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1118 2020-03-24 11:35:43.000000 eansearch-1.7.0/LICENSE
+-rw-r--r--   0 jan       (1000) jan       (1000)     2671 2024-04-18 19:11:24.484347 eansearch-1.7.0/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1419 2023-05-21 08:47:10.000000 eansearch-1.7.0/README.md
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 19:11:24.484347 eansearch-1.7.0/eansearch.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)     2671 2024-04-18 19:11:24.000000 eansearch-1.7.0/eansearch.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      171 2024-04-18 19:11:24.000000 eansearch-1.7.0/eansearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-18 19:11:24.000000 eansearch-1.7.0/eansearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       10 2024-04-18 19:11:24.000000 eansearch-1.7.0/eansearch.egg-info/top_level.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3231 2024-04-18 19:10:01.000000 eansearch-1.7.0/eansearch.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)       38 2024-04-18 19:11:24.484347 eansearch-1.7.0/setup.cfg
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1546 2024-04-18 19:04:25.000000 eansearch-1.7.0/setup.py
```

### Comparing `eansearch-1.5.0/LICENSE` & `eansearch-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eansearch-1.5.0/PKG-INFO` & `eansearch-1.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: eansearch
-Version: 1.5.0
+Version: 1.7.0
 Summary: A Python class for EAN and ISBN name lookup and validation using the API on ean-search.org
 Home-page: https://github.com/eansearch/python-ean-search
 Author: Jan Willamowius
 Author-email: info@relaxedcommunications.com
-License: UNKNOWN
 Keywords: barcode barcodes ean ean13 ean-13 upc gtin isbn13 isbn-13 search lookup find valid validation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -61,9 +59,16 @@
 for product in eanList:
 	print(product["ean"], " is ", product["name"].encode("utf-8"))
 
 eanList = eansearch.barcodePrefixSearch('4007249146');
 for product in eanList:
 	print(product["ean"], " is ", product["name"].encode("utf-8"))
 
+country = eansearch.issuingCountryLookup("5099750442227")
+print(ean + " was issued in " + country)
 
+barcode = eansearch.barcodeImage("5099750442227")
+print("Barcode image for " + ean + " (base64 encoded): " + barcode)
+
+//import base64
+//print (base64.b64decode(barcode))
```

### Comparing `eansearch-1.5.0/eansearch.egg-info/PKG-INFO` & `eansearch-1.7.0/eansearch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: eansearch
-Version: 1.5.0
+Version: 1.7.0
 Summary: A Python class for EAN and ISBN name lookup and validation using the API on ean-search.org
 Home-page: https://github.com/eansearch/python-ean-search
 Author: Jan Willamowius
 Author-email: info@relaxedcommunications.com
-License: UNKNOWN
 Keywords: barcode barcodes ean ean13 ean-13 upc gtin isbn13 isbn-13 search lookup find valid validation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -61,9 +59,16 @@
 for product in eanList:
 	print(product["ean"], " is ", product["name"].encode("utf-8"))
 
 eanList = eansearch.barcodePrefixSearch('4007249146');
 for product in eanList:
 	print(product["ean"], " is ", product["name"].encode("utf-8"))
 
+country = eansearch.issuingCountryLookup("5099750442227")
+print(ean + " was issued in " + country)
 
+barcode = eansearch.barcodeImage("5099750442227")
+print("Barcode image for " + ean + " (base64 encoded): " + barcode)
+
+//import base64
+//print (base64.b64decode(barcode))
```

### Comparing `eansearch-1.5.0/setup.py` & `eansearch-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eansearch',
       description='A Python class for EAN and ISBN name lookup and validation using the API on ean-search.org',
       long_description=long_description,
       long_description_content_type="text/markdown",
-      version='1.5.0',
+      version='1.7.0',
       url='https://github.com/eansearch/python-ean-search',
       author='Jan Willamowius',
       author_email='info@relaxedcommunications.com',
       keywords = 'barcode barcodes ean ean13 ean-13 upc gtin isbn13 isbn-13 search lookup find valid validation',
       packages=setuptools.find_packages(),
       py_modules=['eansearch'],
       classifiers=[
```

