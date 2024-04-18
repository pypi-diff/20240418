# Comparing `tmp/CQE-2.0.2.tar.gz` & `tmp/CQE-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-2.0.2.tar", last modified: Thu Nov  9 10:28:02 2023, max compression
+gzip compressed data, was "CQE-2.0.3.tar", last modified: Thu Apr 18 12:34:10 2024, max compression
```

## Comparing `CQE-2.0.2.tar` & `CQE-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-11-09 10:28:02.061492 CQE-2.0.2/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-11-09 10:28:02.058941 CQE-2.0.2/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   132994 2023-11-09 10:02:24.000000 CQE-2.0.2/CQE/CQE.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    21336 2023-11-09 09:59:09.000000 CQE-2.0.2/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-2.0.2/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    22155 2023-11-09 10:01:09.000000 CQE-2.0.2/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     9429 2023-11-09 09:55:00.000000 CQE-2.0.2/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    46736 2023-11-09 10:00:52.000000 CQE-2.0.2/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-2.0.2/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-11-09 10:28:02.061022 CQE-2.0.2/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-2.0.2/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-2.0.2/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7063 2023-05-16 19:21:43.000000 CQE-2.0.2/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1705 2023-05-17 12:02:10.000000 CQE-2.0.2/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     3505 2023-10-08 16:23:04.000000 CQE-2.0.2/CQE/unit_conversion.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1482733 2023-05-17 11:57:02.000000 CQE-2.0.2/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-11-09 10:28:02.060494 CQE-2.0.2/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10359 2023-11-09 10:28:02.000000 CQE-2.0.2/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      475 2023-11-09 10:28:02.000000 CQE-2.0.2/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-11-09 10:28:02.000000 CQE-2.0.2/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      240 2023-11-09 10:28:02.000000 CQE-2.0.2/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-11-09 10:28:02.000000 CQE-2.0.2/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-2.0.2/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10359 2023-11-09 10:28:02.061257 CQE-2.0.2/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10096 2023-11-09 10:23:14.000000 CQE-2.0.2/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-11-09 10:28:02.061540 CQE-2.0.2/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      978 2023-11-09 10:28:01.000000 CQE-2.0.2/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2024-04-18 12:34:10.602982 CQE-2.0.3/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2024-04-18 12:34:10.597618 CQE-2.0.3/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   133018 2024-04-18 12:22:20.000000 CQE-2.0.3/CQE/CQE.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    21336 2023-11-09 09:59:09.000000 CQE-2.0.3/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-2.0.3/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    22155 2023-11-09 10:01:09.000000 CQE-2.0.3/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     9429 2023-11-09 09:55:00.000000 CQE-2.0.3/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    46736 2023-11-09 10:00:52.000000 CQE-2.0.3/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-2.0.3/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2024-04-18 12:34:10.601759 CQE-2.0.3/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-2.0.3/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-2.0.3/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7063 2023-05-16 19:21:43.000000 CQE-2.0.3/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1705 2023-05-17 12:02:10.000000 CQE-2.0.3/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     3505 2023-10-08 16:23:04.000000 CQE-2.0.3/CQE/unit_conversion.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1482733 2023-05-17 11:57:02.000000 CQE-2.0.3/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2024-04-18 12:34:10.600657 CQE-2.0.3/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10359 2024-04-18 12:34:10.000000 CQE-2.0.3/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      475 2024-04-18 12:34:10.000000 CQE-2.0.3/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2024-04-18 12:34:10.000000 CQE-2.0.3/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      219 2024-04-18 12:34:10.000000 CQE-2.0.3/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2024-04-18 12:34:10.000000 CQE-2.0.3/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34976 2024-04-18 12:24:23.000000 CQE-2.0.3/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10359 2024-04-18 12:34:10.602076 CQE-2.0.3/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10096 2023-11-09 10:23:14.000000 CQE-2.0.3/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2024-04-18 12:34:10.603034 CQE-2.0.3/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1335 2024-04-18 12:33:16.000000 CQE-2.0.3/setup.py
```

### Comparing `CQE-2.0.2/CQE/CQE.py` & `CQE-2.0.3/CQE/CQE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 import json
 import re
-import argparse
+# import argparse
 import logging
 import spacy
 import os
 import numpy
 import copy
 from spacy.matcher import DependencyMatcher, Matcher
 from spacy.tokens import Token
@@ -25,26 +25,26 @@
 from .classes import Change, Value, Range, Unit, Quantity
 from .unit_conversion import unit_conversion
 
 def get_project_root() -> Path:
     return Path(__file__).parent
 
 # Add a debug option to the numparser, so that we can disable the warnings
-parser = argparse.ArgumentParser()
-parser.add_argument('--loglevel',
-                    default='',
-                    choices=logging._nameToLevel.keys(),
-                    help='Provide logging level parameter in order to set what level of log messages you want to record.' )
-
-args = parser.parse_args()
-
-if not args.loglevel: # default is to disable warnings
-    logging.getLogger().disabled = True
-else:
-    logging.basicConfig(format='%(levelname)s:%(message)s', level=args.loglevel) # change default level
+# parser = argparse.ArgumentParser()
+# parser.add_argument('--loglevel',
+#                     default='',
+#                     choices=logging._nameToLevel.keys(),
+#                     help='Provide logging level parameter in order to set what level of log messages you want to record.' )
+#
+# args = parser.parse_args()
+#
+# if not args.loglevel: # default is to disable warnings
+#     logging.getLogger().disabled = True
+# else:
+#     logging.basicConfig(format='%(levelname)s:%(message)s', level=args.loglevel) # change default level
 
 
 #SUBJECTS = ["nsubj", "nsubjpass", "csubj", "csubjpass", "agent", "expl"]
 #OBJECTS = ["dobj", "dative", "attr", "oprd"]
 MONTHS = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December", "Jan.", "Feb.", "Aug.", "Sept.", "Oct", "Nov.", "Dec."]
 BLACK_LIST_UNITS = {"low", "high", "am"} # black list of units that should not be a unit
 MONEY_SYMBOL = {"¥", "$", "₿", "¢", "₡", "₫", "₾", "₵", "₹", "円", "圓", "₭", "₥", "ரூ", "₩"}
```

### Comparing `CQE-2.0.2/CQE/NumberNormalizer.py` & `CQE-2.0.3/CQE/NumberNormalizer.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/classes.py` & `CQE-2.0.3/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/number_lookup.py` & `CQE-2.0.3/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/rules.py` & `CQE-2.0.3/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit.json` & `CQE-2.0.3/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit_classifier/sample_usage.py` & `CQE-2.0.3/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit_classifier/train_classifier_bert.py` & `CQE-2.0.3/CQE/unit_classifier/train_classifier_bert.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit_classifier/unit_disambiguator.py` & `CQE-2.0.3/CQE/unit_classifier/unit_disambiguator.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit_conversion.py` & `CQE-2.0.3/CQE/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE/unit_models.zip` & `CQE-2.0.3/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-2.0.2/CQE.egg-info/PKG-INFO` & `CQE-2.0.3/CQE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 2.0.2
+Version: 2.0.3
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-2.0.2/LICENSE.md` & `CQE-2.0.3/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-                    GNU GENERAL PUBLIC LICENSE
+python3 -m pip install --upgrade twine
+GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
 Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.
 
                             Preamble
```

### Comparing `CQE-2.0.2/PKG-INFO` & `CQE-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 2.0.2
+Version: 2.0.3
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-2.0.2/README.md` & `CQE-2.0.3/README.md`

 * *Files identical despite different names*

