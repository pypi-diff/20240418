# Comparing `tmp/convert-us-to-uk-0.1.1.tar.gz` & `tmp/convert-us-to-uk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.1.tar", last modified: Thu Apr 18 11:11:04 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.2.tar", last modified: Thu Apr 18 11:14:58 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.1.tar` & `convert-us-to-uk-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:11:04.756519 convert-us-to-uk-0.1.1/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1936 2024-04-18 11:11:04.756519 convert-us-to-uk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2024-04-17 15:44:02.000000 convert-us-to-uk-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:11:04.737907 convert-us-to-uk-0.1.1/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.1/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1529 2024-04-18 11:08:31.000000 convert-us-to-uk-0.1.1/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    40123 2024-04-17 12:49:20.000000 convert-us-to-uk-0.1.1/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-04-18 11:11:04.756519 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1936 2024-04-18 11:11:04.000000 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-04-18 11:11:04.000000 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:11:04.000000 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-18 11:11:04.000000 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 11:11:04.000000 convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:11:04.756519 convert-us-to-uk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-04-18 11:10:55.000000 convert-us-to-uk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:58.366129 convert-us-to-uk-0.1.2/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1936 2024-04-18 11:14:58.363854 convert-us-to-uk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2024-04-17 15:44:02.000000 convert-us-to-uk-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:58.346224 convert-us-to-uk-0.1.2/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.2/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1529 2024-04-18 11:14:37.000000 convert-us-to-uk-0.1.2/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    40123 2024-04-17 12:49:20.000000 convert-us-to-uk-0.1.2/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:58.361584 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1936 2024-04-18 11:14:58.000000 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-04-18 11:14:58.000000 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:14:58.000000 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-18 11:14:58.000000 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 11:14:58.000000 convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:14:58.366668 convert-us-to-uk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-04-18 11:14:51.000000 convert-us-to-uk-0.1.2/setup.py
```

### Comparing `convert-us-to-uk-0.1.1/PKG-INFO` & `convert-us-to-uk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.1/README.md` & `convert-us-to-uk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.1/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.2/convert_us_to_uk/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import csv
 import re
 import pkg_resources
 
 # Load the US to UK spelling dictionary
 def load_spelling_dict(filename):
-    file_path = pkg_resources.resource_filename('convert-us-to-uk', filename)
+    file_path = pkg_resources.resource_filename('convert_us_to_uk', filename)
     with open(filename, mode='r', encoding='utf-8') as file:
         reader = csv.DictReader(file)
         return {row['us']: row['uk'] for row in reader}
 
 # Function to replace US spellings with UK spellings
 def convert_to_uk(text):
     spelling_dict = load_spelling_dict("us_to_uk_trans.csv")
```

### Comparing `convert-us-to-uk-0.1.1/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.2/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.1/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.2/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.1/setup.py` & `convert-us-to-uk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='convert-us-to-uk',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     description='A simple utility to convert US spelling to UK spelling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Oliver Blane',
     author_email='oliverblane72@gmail.com',
```

