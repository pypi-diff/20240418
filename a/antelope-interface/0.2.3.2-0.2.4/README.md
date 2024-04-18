# Comparing `tmp/antelope_interface-0.2.3.2.tar.gz` & `tmp/antelope_interface-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_interface-0.2.3.2.tar", last modified: Wed Mar 27 00:35:36 2024, max compression
+gzip compressed data, was "antelope_interface-0.2.4.tar", last modified: Thu Apr 18 05:36:15 2024, max compression
```

## Comparing `antelope_interface-0.2.3.2.tar` & `antelope_interface-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.953101 antelope_interface-0.2.3.2/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.3.2/LICENSE
--rw-r--r--   0 b          (500) b          (506)       48 2024-03-26 23:28:57.000000 antelope_interface-0.2.3.2/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)     1760 2024-03-27 00:35:36.953101 antelope_interface-0.2.3.2/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1013 2020-12-30 20:52:39.000000 antelope_interface-0.2.3.2/README.md
--rw-r--r--   0 b          (500) b          (506)      848 2024-03-27 00:35:34.000000 antelope_interface-0.2.3.2/pyproject.toml
--rw-r--r--   0 b          (500) b          (506)       38 2024-03-27 00:35:36.953101 antelope_interface-0.2.3.2/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     3018 2024-03-27 00:32:45.000000 antelope_interface-0.2.3.2/setup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/
--rw-r--r--   0 b          (500) b          (506)     7363 2024-03-27 00:31:29.000000 antelope_interface-0.2.3.2/src/antelope/__init__.py
--rw-r--r--   0 b          (500) b          (506)     7128 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/exchanges_from_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/flows/
--rw-r--r--   0 b          (500) b          (506)       89 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/flows/__init__.py
--rw-r--r--   0 b          (500) b          (506)    12111 2024-03-20 01:05:41.000000 antelope_interface-0.2.3.2/src/antelope/flows/flow.py
--rw-r--r--   0 b          (500) b          (506)     3751 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/flows/flow_interface.py
--rw-r--r--   0 b          (500) b          (506)    13903 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/flows/openlca_locales.json
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/interfaces/
--rw-r--r--   0 b          (500) b          (506)      111 2020-09-25 19:28:16.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/__init__.py
--rw-r--r--   0 b          (500) b          (506)     5159 2024-03-13 01:45:59.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/abstract_query.py
--rw-r--r--   0 b          (500) b          (506)    10480 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/ibackground.py
--rw-r--r--   0 b          (500) b          (506)     4333 2020-09-24 22:08:18.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/iconfigure.py
--rw-r--r--   0 b          (500) b          (506)     5947 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/iexchange.py
--rw-r--r--   0 b          (500) b          (506)     8787 2023-11-22 06:08:07.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/iforeground.py
--rw-r--r--   0 b          (500) b          (506)     7432 2024-03-13 01:45:20.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/iindex.py
--rw-r--r--   0 b          (500) b          (506)    13916 2024-03-13 01:45:59.000000 antelope_interface-0.2.3.2/src/antelope/interfaces/iquantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/models/
--rw-r--r--   0 b          (500) b          (506)    19881 2024-03-22 20:54:23.000000 antelope_interface-0.2.3.2/src/antelope/models/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4683 2023-11-18 09:46:10.000000 antelope_interface-0.2.3.2/src/antelope/models/auth.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/refs/
--rw-r--r--   0 b          (500) b          (506)      185 2024-03-20 21:43:30.000000 antelope_interface-0.2.3.2/src/antelope/refs/__init__.py
--rw-r--r--   0 b          (500) b          (506)    14403 2024-03-13 02:00:24.000000 antelope_interface-0.2.3.2/src/antelope/refs/base.py
--rw-r--r--   0 b          (500) b          (506)     4702 2024-03-13 01:45:20.000000 antelope_interface-0.2.3.2/src/antelope/refs/catalog_ref.py
--rw-r--r--   0 b          (500) b          (506)     8424 2024-03-13 02:00:24.000000 antelope_interface-0.2.3.2/src/antelope/refs/exchange_ref.py
--rw-r--r--   0 b          (500) b          (506)     5179 2024-03-13 01:44:47.000000 antelope_interface-0.2.3.2/src/antelope/refs/flow_ref.py
--rw-r--r--   0 b          (500) b          (506)    11993 2024-03-15 22:38:06.000000 antelope_interface-0.2.3.2/src/antelope/refs/process_ref.py
--rw-r--r--   0 b          (500) b          (506)     9418 2024-03-13 01:58:16.000000 antelope_interface-0.2.3.2/src/antelope/refs/quantity_ref.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.949767 antelope_interface-0.2.3.2/src/antelope/refs/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/refs/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1150 2023-07-21 21:50:52.000000 antelope_interface-0.2.3.2/src/antelope/refs/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     4717 2023-11-28 23:43:13.000000 antelope_interface-0.2.3.2/src/antelope/xdb_tokens.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-27 00:35:36.953101 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/
--rw-r--r--   0 b          (500) b          (506)     1760 2024-03-27 00:35:36.000000 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1168 2024-03-27 00:35:36.000000 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-03-27 00:35:36.000000 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       22 2024-03-27 00:35:36.000000 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)        9 2024-03-27 00:35:36.000000 antelope_interface-0.2.3.2/src/antelope_interface.egg-info/top_level.txt
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.4/LICENSE
+-rw-r--r--   0 b          (500) b          (506)       48 2024-03-26 23:28:57.000000 antelope_interface-0.2.4/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)     2553 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1871 2024-04-11 07:45:58.000000 antelope_interface-0.2.4/README.md
+-rw-r--r--   0 b          (500) b          (506)      864 2024-04-17 23:03:37.000000 antelope_interface-0.2.4/pyproject.toml
+-rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     2327 2024-04-17 23:12:49.000000 antelope_interface-0.2.4/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/antelope/
+-rw-r--r--   0 b          (500) b          (506)     7294 2024-04-18 05:03:09.000000 antelope_interface-0.2.4/src/antelope/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     7128 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/exchanges_from_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/antelope/flows/
+-rw-r--r--   0 b          (500) b          (506)       89 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/flows/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    12139 2024-04-18 05:19:57.000000 antelope_interface-0.2.4/src/antelope/flows/flow.py
+-rw-r--r--   0 b          (500) b          (506)     3824 2024-04-18 05:10:28.000000 antelope_interface-0.2.4/src/antelope/flows/flow_interface.py
+-rw-r--r--   0 b          (500) b          (506)    13903 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/flows/openlca_locales.json
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/interfaces/
+-rw-r--r--   0 b          (500) b          (506)      169 2024-04-17 23:12:49.000000 antelope_interface-0.2.4/src/antelope/interfaces/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1769 2024-04-18 05:27:57.000000 antelope_interface-0.2.4/src/antelope/interfaces/abstract_query.py
+-rw-r--r--   0 b          (500) b          (506)    10480 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/interfaces/ibackground.py
+-rw-r--r--   0 b          (500) b          (506)     4879 2024-04-18 05:31:46.000000 antelope_interface-0.2.4/src/antelope/interfaces/ibasic.py
+-rw-r--r--   0 b          (500) b          (506)     4333 2024-04-18 05:28:30.000000 antelope_interface-0.2.4/src/antelope/interfaces/iconfigure.py
+-rw-r--r--   0 b          (500) b          (506)     5164 2024-04-18 05:29:58.000000 antelope_interface-0.2.4/src/antelope/interfaces/iexchange.py
+-rw-r--r--   0 b          (500) b          (506)     8785 2024-04-18 05:15:43.000000 antelope_interface-0.2.4/src/antelope/interfaces/iforeground.py
+-rw-r--r--   0 b          (500) b          (506)     7432 2024-03-13 01:45:20.000000 antelope_interface-0.2.4/src/antelope/interfaces/iindex.py
+-rw-r--r--   0 b          (500) b          (506)    13917 2024-04-18 05:17:15.000000 antelope_interface-0.2.4/src/antelope/interfaces/iquantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/models/
+-rw-r--r--   0 b          (500) b          (506)    21308 2024-04-18 05:18:56.000000 antelope_interface-0.2.4/src/antelope/models/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4683 2023-11-18 09:46:10.000000 antelope_interface-0.2.4/src/antelope/models/auth.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/refs/
+-rw-r--r--   0 b          (500) b          (506)      185 2024-03-20 21:43:30.000000 antelope_interface-0.2.4/src/antelope/refs/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    14361 2024-04-18 05:17:38.000000 antelope_interface-0.2.4/src/antelope/refs/base.py
+-rw-r--r--   0 b          (500) b          (506)     4702 2024-03-13 01:45:20.000000 antelope_interface-0.2.4/src/antelope/refs/catalog_ref.py
+-rw-r--r--   0 b          (500) b          (506)     8424 2024-03-13 02:00:24.000000 antelope_interface-0.2.4/src/antelope/refs/exchange_ref.py
+-rw-r--r--   0 b          (500) b          (506)     5179 2024-03-13 01:44:47.000000 antelope_interface-0.2.4/src/antelope/refs/flow_ref.py
+-rw-r--r--   0 b          (500) b          (506)    12182 2024-04-11 07:44:14.000000 antelope_interface-0.2.4/src/antelope/refs/process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     9422 2024-04-18 05:26:09.000000 antelope_interface-0.2.4/src/antelope/refs/quantity_ref.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/refs/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/refs/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1150 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/refs/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     4717 2023-11-28 23:43:13.000000 antelope_interface-0.2.4/src/antelope/xdb_tokens.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope_interface.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     2553 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1202 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       36 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)        9 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/top_level.txt
```

### Comparing `antelope_interface-0.2.3.2/LICENSE` & `antelope_interface-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/pyproject.toml` & `antelope_interface-0.2.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering"
 ]
-dependencies = ["synonym_dict", "pydantic"]
-version = "0.2.3.2"
+dependencies = ["synonym_dict >= 0.2.4", "pydantic >= 2.5.0"]
+version = "0.2.4"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `antelope_interface-0.2.3.2/setup.py` & `antelope_interface-0.2.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
-ANTELOPE_VERSION = '0.2.3.2'
+setup()
 
-requires = [
-    "synonym_dict>=0.2.4",
-    "pydantic>=2.5.0"
-]
 
 """
 Version History:
+0.2.4 2024/04/17 - split out BasicInterface from AbstractQuery. 
+                   abandon setup.py except for this changelog.
+                   Redesign ExteriorFlow to have maybe a little bit more logic
+                   First pass at API documentation
+
 0.2.3.2 2024/03/26 move to src layout
 
 0.2.3.1 2024/03/22 LciaDetail objects now return DirectedFlow instead of FlowSpec (as exchange proxy)
 
 0.2.3 2024/01/05 - 'lcia' index route; exclude LCIA metadata from quantity manager synonyms
                    Versions >= 0.2.3 to support 0.3-branch development code (but this package is not branched)
 
@@ -51,32 +52,7 @@
 0.1.1 2020/11/12 - Bug fixes and boundary setting
                    add synonyms() route and grant a ref access to synonyms from its origin
                    terminate() is now called targets()
                    remove most of the foreground interface spec
                    
 0.1.0 2020/07/31 - Initial release - JIE paper 
 """
-
-setup(
-    name="antelope_interface",
-    version=ANTELOPE_VERSION,
-    author="Brandon Kuczenski",
-    author_email="bkuczenski@ucsb.edu",
-    license="BSD 3-Clause",
-    install_requires=requires,
-    url="https://github.com/AntelopeLCA/antelope",
-    summary="An interface specification for accessing LCA data",
-    long_description_content_type='text/markdown',
-    long_description=open('README.md').read(),
-    include_package_data=True,
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Topic :: Scientific/Engineering"
-    ],
-    python_requires='>=3.6',
-    packages=find_packages('src')
-)
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/__init__.py` & `antelope_interface-0.2.4/src/antelope/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Antelope Interface Definitions
 
 The abstract classes in this sub-package define what information is made available via a stateless query to an Antelope
 resource of some kind.  The interfaces must be instantiated in order to be used.  In the core package
 """
 
-from .interfaces.abstract_query import PrivateArchive, EntityNotFound, NoAccessToEntity
+from .interfaces import ANTELOPE_INTERFACES
 
+from .interfaces.ibasic import BasicInterface, EntityNotFound, NoAccessToEntity
 from .interfaces.iconfigure import ConfigureInterface
 from .interfaces.iexchange import ExchangeInterface, ExchangeRequired
 from .interfaces.iindex import IndexInterface, IndexRequired, directions, comp_dir, num_dir, check_direction, valid_sense, comp_sense
 from .interfaces.ibackground import BackgroundInterface, BackgroundRequired
 from .interfaces.iquantity import QuantityInterface, QuantityRequired, NoFactorsFound, ConversionReferenceMismatch, FlowableMismatch
 from .interfaces.iforeground import ForegroundInterface
 
@@ -24,16 +25,14 @@
 from .refs.exchange_ref import ExchangeRef, RxRef, EXCHANGE_TYPES
 
 
 import re
 
 from os.path import splitext
 
-from collections import namedtuple
-
 
 class ValuesAccessRequired(Exception):
     """
     The requested route requires a grant that has values=True
     """
     pass
 
@@ -46,22 +45,22 @@
 
 
 '''
 Query classes
 '''
 
 
-class BasicQuery(IndexInterface, ExchangeInterface, QuantityInterface):
+class BasicQuery(BasicInterface, IndexInterface, ExchangeInterface, QuantityInterface):
     """
-    A basic query depends on an archive-- which is not yet well-defined, but which has the following API:
-    archive.make_interface(interface): returns an implementation of the designated interface
-    archive.ref: returns the archive's semantic reference
-    archive.source: returns the physical source for the archive's content
+    A basic query depends on an archive-- which has the following API:
+
+     - archive.make_interface(interface): returns an implementation of the designated interface
+     - archive.ref: returns the archive's semantic reference
+     - archive.source: returns the physical source (or URI) for the archive's content
 
-    Note that an alternative abstract query implementation could be imagined
     """
     def __init__(self, archive, debug=False):
         self._archive = archive
         self._dbg = debug
 
     def _perform_query(self, itype, attrname, exc, *args, **kwargs):
         if itype is None:
@@ -149,17 +148,18 @@
     except EntityNotFound:
         fg.new_quantity('Node Activity', ref_unit='activity', external_ref='node activity', comment='MFA metric')
         return fg.get_canonical('node activity')
 
 
 def enum(iterable, filt=None, invert=True):
     """
-    Enumerate an iterable for interactive use. return it as a list. Optional negative filter supplied as regex
+    Enumerate an iterable for interactive use. return it as a list. Optional negative filter supplied as regex.
+
     :param iterable:
-    :param filt:
+    :param filt: regex to filter out entries from return and enumeration.
     :param invert: [True] sense of filter. note default is negative i.e. to screen *out* matches
      (the thinking is that the input is already positive-filtered)
     :return:
     """
     ret = []
     if filt is not None:
         if invert:
@@ -169,18 +169,18 @@
     else:
         _iter = iterable
     for k, v in enumerate(_iter):
         print(' [%02d] %s' % (k, v))
         ret.append(v)
     return ret
 
+
 """
-In most LCA software, including the current operational version of lca-tools, a 'flow' is a composite entity
-that is made up of a 'flowable' (substance, product, intervention, or service) and a 'context', which is 
-synonymous with an environmental compartment.
+In most LCA software, a 'flow' is a composite entity that is made up of a 'flowable' (substance, product, 
+intervention, or service) and a 'context', which is synonymous with an environmental compartment.
 
 The US EPA review of elementary flows recommended managing the names of flowables and contexts separately, and that
 is the approach that is done here.  
 
 The exchange model consists of : parent | flow(able), direction | [exch value] | [terminal node]
 
 If the terminal node is a context, the exchange is elementary. if it's a process, then intermediate. 
@@ -192,16 +192,16 @@
 'new' means use the new data model (exchange terminations are contexts) 
 """
 CONTEXT_STATUS_ = 'new'  # 'compat': context = flow['Compartment']; 'new': context = exch.termination
 
 
 # Exterior exchanges- with contexts outside the db.  Direction is given with respect to the Interior (e.g. "Output" "to air")
 # LciaResults should negate values when an exchange direction and a context are not complementary (i.e. "Input" "to air")
-ExteriorFlow = namedtuple('ExteriorFlow', ('origin', 'flow', 'direction', 'termination'))
+# ExteriorFlow = namedtuple('ExteriorFlow', ('origin', 'flow', 'direction', 'termination'))
 
-EntitySpec = namedtuple('EntitySpec', ('link', 'ref', 'name', 'group'))
+# EntitySpec = namedtuple('EntitySpec', ('link', 'ref', 'name', 'group'))
 
 # packages that contain 'providers'
 antelope_herd = [
     'antelope_background',
     'antelope_foreground'
 ]
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/exchanges_from_spreadsheet.py` & `antelope_interface-0.2.4/src/antelope/exchanges_from_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/flows/flow.py` & `antelope_interface-0.2.4/src/antelope/flows/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .flow_interface import FlowInterface
 from ..interfaces.iquantity import ConversionReferenceMismatch, NoFactorsFound
 
 import os
 import re
 import json
 
+from abc import ABC
+
 from synonym_dict import SynonymSet
 from synonym_dict.flowables.cas_number import CasNumber, InvalidCasNumber
 
 
 # the weak link in our biogenic CO2 accounting: flow name MUST be caught by this regex in order to be quelled
 # our hacky-hack: rename flows when they are CO2 and any term matches the regex. do this in the LciaEngine.
 biogenic = re.compile('(biotic|biogenic|non-fossil|in air)', flags=re.IGNORECASE)
@@ -32,22 +34,24 @@
 openlca_locales.json file created from: antelope_olca package, gen_locales('openlca_locales.json') 
 """
 
 with open(os.path.join(os.path.dirname(__file__), 'openlca_locales.json')) as fp:
     olca_locales = json.load(fp)
 
 
-class Flow(FlowInterface):
+class Flow(FlowInterface, ABC):
     """
     A partly-abstract class that implements the flow specification but not the entity specification.
 
     Included in this specification is a *detection of biogenic CO2 by regex*
     Each flow has a quell_co2 property which is True if:
+
      - the flow is a synonym for CO2 and
      - the flow's name matches the biogenic regex: '(biotic|biogenic|non-fossil|in air)' (case insensitive)
+
     There are 3 ways for a flow to be identified as a synonym for CO2:
      1. pass is_co2=True at instantiation
      2. set flow.is_co2 = True
      3. assign a CasNumber equivalent to '124-38-9'
 
     Item #2 can be used in general by downstream implementations.
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/flows/flow_interface.py` & `antelope_interface-0.2.4/src/antelope/flows/flow_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from abc import ABC
+
+
 class BaseEntity(object):
     """
     The very most basic characteristics of entities and entity refs
     """
     @property
     def entity_type(self):
         return NotImplemented
@@ -77,15 +80,15 @@
     def get(self, item):
         raise KeyError
 
     def make_ref(self, query):
         return NotImplemented
 
 
-class FlowInterface(BaseEntity):
+class FlowInterface(BaseEntity, ABC):
     """
     An abstract class that establishes common functionality for OBSERVATIONS OF FLOWS.  A Flow consists of:
      - a reference quantity with a fixed unit
      - a flowable (a list of synonyms for the flowable substnce being described)
      - a context (a hierarchical list of strings designating the flows 'compartment' or category)
 
     Must be implemented (properties):
@@ -134,16 +137,16 @@
         :param other:
         :return:
         """
         raise NotImplementedError
 
     def lookup_cf(self, quantity, context, locale, refresh=False, **kwargs):
         """
-        Look for cached characterizations, and retrieve if none is found
-        :param quantity:
+        Look for cached characterizations, and retrieve one from the provided quantity if none is found.
+        :param quantity: a QuantityRef
         :param context:
         :param locale:
         :param refresh: [False] if True, discard cached CF
         :param kwargs: passed to quantity relation
         :return:
         """
         raise NotImplementedError
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/flows/openlca_locales.json` & `antelope_interface-0.2.4/src/antelope/flows/openlca_locales.json`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/abstract_query.py` & `antelope_interface-0.2.4/src/antelope/interfaces/ibasic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,69 @@
-"""
-Root-level catalog interface
-"""
+from .abstract_query import AbstractQuery
 
 
-class ValidationError(Exception):
+class BasicRequired(Exception):
+    """
+    Default exception to indicate that the requested method cannot be invoked without an implementation of the
+    basic interface (and none could be found).
+    """
     pass
 
 
-class PrivateArchive(Exception):
+class ValidationError(Exception):
+    """
+    :meta private:
+    """
     pass
 
 
 class EntityNotFound(Exception):
+    """
+    An exception of generic usefulness.
+    """
     pass
 
 
 class NoAccessToEntity(Exception):
     """
     Used when the actual entity is not accessible, i.e. when a ref cannot dereference itself
     """
     pass
 
 
-class AbstractQuery(object):
+class BasicInterface(AbstractQuery):
     """
-    Not-quite-abstract base class for executing queries
+    BasicInterface core methods.
 
-    Query implementation must provide:
-     - origin (property)
-     - _iface (generator: itype)
-     - _tm (property) a TermManager
-    """
-    _validated = None
-
-    '''
-    Overridde these methods
-    '''
-    @property
-    def origin(self):
-        return NotImplemented
-
-    def make_ref(self, entity):
-        raise NotImplementedError
-
-    def _perform_query(self, itype, attrname, exc, *args, **kwargs):
-        """
-
-        :param itype: type of query being performed (which interface is being invoked)
-        :param attrname: query name
-        :param exc: "fallback exception": ignore it if an implementation raises it; then raise it if no implementation
-         succeeds
-        :param args: to pass to the query
-        :param kwargs: to pass to the query or subclass
-        :return:
-        """
-        raise NotImplementedError
+    These are methods for retrieving objects and accessing documentary information about them. The basic interface
+    should provide access to the most authoritative source of information about a data resource.
 
-    '''
-    Internal workings
-    '''
-    '''
-    Can be overridden
-    '''
-    def _grounded_query(self, origin):
-        """
-        Pseudo-abstract method used to construct entity references from a query that is anchored to a metaresource.
-        must be overriden by user-facing subclasses if resources beyond self are required to answer
-        the queries (e.g. a catalog).
-        :param origin:
-        :return:
-        """
-        return self
 
     """
+    """
     Basic "Documentary" interface implementation
     From JIE submitted:
      - get(id)
      - properties(id)
      - get item(id, item)
      - get reference(id)
      - synonyms(id-or-string)
     provided but not spec'd:
      - validate
      - get_uuid
     """
 
     def validate(self):
+        """
+        This method should return `True` whenever the implementation is attached to a valid data source that is
+        capable of answering questions.  The existence of a basic implementation is necessary and sufficient for a
+        query to be valid.
+
+        :return: bool
+        """
         if self._validated is None:
             try:
                 self._perform_query('basic', 'validate', ValidationError)
                 self._validated = True
             except ValidationError:
                 return False
         return self._validated
@@ -111,25 +85,20 @@
         :param kwargs:
         :return:
         """
         return self._perform_query('basic', 'properties', EntityNotFound, external_ref, **kwargs)
 
     def get_item(self, external_ref, item):
         """
-        access an entity's dictionary items
-        :param external_ref:
-        :param item:
+        access an entity's properties.  This requires de-referencing the query to the true entity.  This method
+        is used to access essentially all documentary information about an object.
+        :param external_ref: the entity's identifier
+        :param item: the desired property
         :return:
         """
-        '''
-        if hasattr(external_ref, 'external_ref'):  # debounce
-            err_str = external_ref.external_ref
-        else:
-            err_str = external_ref
-        '''
         return self._perform_query('basic', 'get_item', EntityNotFound,
                                    external_ref, item)
 
     def get_uuid(self, external_ref):
         return self._perform_query('basic', 'get_uuid', EntityNotFound,
                                    external_ref)
 
@@ -144,27 +113,33 @@
         :return: list of strings
         """
         return self._perform_query('basic', 'synonyms', KeyError, item,
                                    **kwargs)
 
     def is_lcia_engine(self, **kwargs):
         """
-        A key question in the quantity interface is the way terms are managed.  There are two main footings:
-         - the terms specified by the source are authentic / canonical and should be reproduced
-         - terms from different data sources refer to the same concept.
+        A key question in the quantity interface is the way terms are managed.
         An archive's Term Manager determines how input terms are interpreted and how characterizations are looked up.
+        There are two main footings:
+
+         - the terms specified by the source are authentic / canonical and should be reproduced
+         - terms from different data sources refer to the same concept, and the *concept* should be returned.
+
+        A *provincial* term manager considers the local archive (to which it is attached) to be the source of all
+        truth. It will return flowables and contexts exactly as they are defined in the native data source.  In
+        this case, `is_lcia_engine()` returns `False`.
 
         if the term manager is an LciaEngine, it uses a standard set of contexts and flowables, and provides routes
         to add new synonyms for flowables/contexts and to report new flowables or contexts.  Ultimately the objective
-        is to manage characterization + knowledge of intermediate flows.
-
-        This routine reports whether an origin implements the LciaEngine [protocol?] for dealing with flows.
+        is to manage characterization + knowledge of both elementary and intermediate flows.
+        In this case, `is_lcia_engine()` returns `True`.
 
         :param kwargs:
-        :return: True/False - could also provide more structured information as needed.
+        :return: bool
         """
 
         try:
             return self._perform_query('basic', 'is_lcia_engine', TypeError, **kwargs)
         except TypeError:
             return False
 
+
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/ibackground.py` & `antelope_interface-0.2.4/src/antelope/interfaces/ibackground.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/iconfigure.py` & `antelope_interface-0.2.4/src/antelope/interfaces/iconfigure.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         """
         return self._perform_query(_interface, 'unset_reference', ConfigRequired,
                                    process_ref, flow_ref, direction, **kwargs)
 
     def characterize_flow(self, flow_ref, quantity_ref, value, location='GLO', **kwargs):
         """
         Add a characterization to the given flow in the given quantity, with respect to the flow's native reference
-         quantity.  Optional location field.
+        quantity.  Optional location field.
+
         :param flow_ref:
         :param quantity_ref:
         :param value:
         :param location: ['GLO']
         :param kwargs:
         :return:
         """
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/iexchange.py` & `antelope_interface-0.2.4/src/antelope/interfaces/iexchange.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,40 +9,32 @@
 _interface = 'exchange'
 
 EXCHANGE_VALUES_REQUIRED = {'ev', 'exchange_values', 'inventory', 'exchange_relation'}
 
 
 class ExchangeInterface(AbstractQuery):
     """
-    InventoryInterface core methods: individual processes, quantitative data.
+    The Exchange Interface implements the Exchange Relation:
+     - given a process, a reference flow, and a query flow, report the quantity of the query flow that is exchanged
+       with respect to a unit of the reference flow.
 
-    Need to do some thinking here-- the list of methods is very short. In particular there is no way to do any of
-    the following:
-     * retrieve reference exchanges
-     * retrieve cutoff exchanges or only terminated exchanges
-     * retrieve only intermediate or only elementary exchanges [[ pending context refactor :(:( ]]
-       = this is frankly not possible to do, even after the context refactor, because there is no bulletproof way to
-         determine whether a termination is a context or a process or some non-elementary compartment, until you
-         introduce the Lcia Engine with its reference set of contexts, UNLESS you include the reference elementary set
-         in ALL context managers.  Which is feasible- since it's a short list- but still, not done as yet.
-    There's also no access to information from the original source that is not part of the data model, e.g. uncertainty
-    information, arbitrary XML queries, etc.
     """
     def exchanges(self, process, **kwargs):
         """
         Retrieve process's full exchange list, without values
         :param process:
         :return: list of exchanges without values
         """
         return self._perform_query(_interface, 'exchanges',
                                    ExchangeRequired, process, **kwargs)
 
     def ev(self, process, flow, direction=None, termination=None, ref_flow=None, **kwargs):
         """
         Return a float.  Symmetric to quantity.cf
+
         :param process:
         :param flow:
         :param direction: [None] if none, if flows exist with both directions, raise an error
         :param termination: [None] if none, return sum of flows across all terminations
         :param ref_flow: [None] if none, return unallocated value. Otherwise, return value allocated to a unit of the
          specified reference
         :return: a float
@@ -53,15 +45,16 @@
 
     def exchange_values(self, process, flow, direction=None, termination=None, reference=None, **kwargs):
         """
         Leftover from earlier implementation; deprecated.
         2022-12-27: is this really deprecated? it's used in computing reference_value and I don't see any other way...
         perhaps we should add reference_value() to the API but for now let's keep this around
 
-        Return a list of exchanges with values matching the specification
+        Return a list of exchanges with values matching the specification.
+
         :param process:
         :param flow:
         :param direction: [None] if none,
         :param termination: [None] if none, return all terminations
         :param reference: [None] if True, only find reference exchanges. If false- maybe omit reference exchanges?
         :return: list of exchanges with values matching the specification
         """
@@ -73,25 +66,26 @@
     def inventory(self, process, ref_flow=None, scenario=None, **kwargs):
         """
         Return a list of exchanges with values. If no reference is supplied, return all unallocated exchanges, including
         reference exchanges.
 
         If a reference flow is supplied, expected behavior depends on a number of factors.
          - If the supplied reference flow is part of the process's reference entity, the inventory should return all
-         non-reference exchanges, appropriately allocated to the specified flow, and normalized to a unit of the
-         specified flow.
+           non-reference exchanges, appropriately allocated to the specified flow, and normalized to a unit of the
+           specified flow.
          - If the supplied reference flow is not part of the reference entity, NO allocation should be performed.
-         Instead, the inventory should return ALL exchanges except for the specified flow, un-allocated, normalized to
-         a unit of the specified flow.  This query is only valid if the specified flow is a cut-off (i.e. un-terminated)
-         exchange (i.e. it could be treated as a "silent reference" or effective co-product)
+           Instead, the inventory should return ALL exchanges except for the specified flow, un-allocated, normalized to
+           a unit of the specified flow.  This query is only valid if the specified flow is a cut-off (i.e. un-terminated)
+           exchange (i.e. it could be treated as a "silent reference" or effective co-product)
          - If the supplied reference flow is a non-reference, non-cutoff flow (i.e. it is a terminated exchange), then
-         the appropriate behavior is undefined. The default implementation raises an ExchangeError.
+           the appropriate behavior is undefined. The default implementation raises an ExchangeError.
 
         Note: if this is called on a fragment, the signature is the same but the 'ref_flow' argument is ignored and
         the alternative 'scenario' kwarg is accepted
+
         :param process:
         :param ref_flow: used only for processes
         :param scenario: used only for fragments (antelope_foreground)
         :return: a list of unallocated or allocated exchange refs
         """
         return self._perform_query(_interface, 'inventory', ExchangeRequired,
                                    process, ref_flow=ref_flow, scenario=scenario, **kwargs)
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/iforeground.py` & `antelope_interface-0.2.4/src/antelope/interfaces/iforeground.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         >>> elec = fg.new_flow('Electricity supply fragment', 'kWh')
         >>> my_frag = fg.new_fragment(elec, 'Output')  # flow is an output from my_frag
         >>> child = fg.new_fragment(elec, 'Input', parent=my_frag, balance=True)  # flow is an input to my_frag
         >>> child.terminate(elec_production_process)
 
         :param flow: a flow entity/ref, or an external_ref known to the foreground
         :param direction:
-        :param kwargs: uuid=None, parent=None, comment=None, value=None, balance=False; **kwargs passed to LcFragment
+        :param kwargs: uuid=None, parent=None, comment=None, value=None, balance=False; kwargs passed to LcFragment
         :return: the fragment? or a fragment ref? <== should only be used in the event of a non-local foreground
         """
         return self._perform_query(_interface, 'new_fragment', ForegroundRequired,
                                    flow, direction, **kwargs)
 
     def child_flows(self, fragment, **kwargs):
         """
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/iindex.py` & `antelope_interface-0.2.4/src/antelope/interfaces/iindex.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/interfaces/iquantity.py` & `antelope_interface-0.2.4/src/antelope/interfaces/iquantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         The way we imagine this working in the days of future XDB/QDB:
          - it's not foreground LCIA at all, it's encapsulated LCIA
          - it's not part of the quantity interface, it's part of the basic interface
          - it requires background data implemented at the server, even if the client is denied background authorization
            (hence the basic interface)
          - either the quantity ref must be known locally or resolvable to a do_lcia operation by the catalog
          - there is also the implied need for sys_lcia which is a POST operation that uses sys_lci
+
         It needs to be rewritten.
 
         :param process:
         :param ref_flow:
         :param quantity_ref:
         :param kwargs:
         :return: an LciaResult whose components are flows
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/models/__init__.py` & `antelope_interface-0.2.4/src/antelope/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,23 @@
             yield k
 
     @property
     def external_ref(self):  # what, was there some taboo against this?
         return self.entity_id
 
     @classmethod
-    def from_entity(cls, entity, **kwargs):
+    def from_search(cls, entity):
+        ent = cls(origin=entity.origin, entity_id=entity.external_ref, entity_type=entity.entity_type,
+                  properties=dict())
+        for k in entity.signature_fields():
+            ent.properties[k] = entity[k]
+        return ent
+
+    @classmethod
+    def from_entity(cls, entity):
         ent = cls(origin=entity.origin, entity_id=entity.external_ref, entity_type=entity.entity_type,
                   properties=dict())
         # ent.properties.update(kwargs)  # I don't know why this was here but I don't think I want it
         for k in entity.signature_fields():
             ent.properties[k] = entity[k]
 
         if entity.uuid is not None and entity.uuid != entity.external_ref:
@@ -158,14 +166,15 @@
                   entity_type=entity.entity_type,
                   context=list(entity.context),
                   locale=entity.locale,
                   properties=dict())
 
         obj.properties['name'] = entity.name
         obj.properties[entity.reference_field] = entity.reference_entity.external_ref
+        obj.properties['unit'] = entity.unit
         obj.properties['Synonyms'] = []
 
         for key, val in kwargs.items():
             obj.properties[key] = entity[key]
         return obj
 
     @classmethod
@@ -241,28 +250,14 @@
             raise TypeError('%s\nUnknown exchange type %s' % (x, x.type))
         loc = locale or x.flow.locale
         return cls(origin=x.flow.origin, external_ref=x.flow.external_ref, flowable=x.flow.name,
                    quantity_ref=x.flow.reference_entity.external_ref,
                    context=cx, locale=loc)
 
 
-class ExteriorFlow(ResponseModel):
-    """
-    Do we really need both an ExteriorFlow model and a FlowSpec model? this one has direction, and origin+flow;
-    that one has flowable+ref entity, and locale (but we added locale)
-
-    This is currently unused, but that's because we haven't implemented the {origin}/exterior route yet
-    """
-    origin: str
-    flow: str
-    direction: str  # antelope_interface specifies the direction as w/r/t/ context, as in "Input" "to air". This SEEMS WRONG.
-    context: List[str]
-    locale: Optional[str] = 'GLO'  # ???
-
-
 class DirectedFlow(ResponseModel):
     flow: FlowSpec
     direction: str
 
     @property
     def origin(self):
         return self.flow.origin
@@ -280,14 +275,46 @@
         return self.flow.flowable
 
     @classmethod
     def from_exchange(cls, obj):
         return cls(flow=FlowSpec.from_exchange(obj), direction=obj.direction)
 
 
+class ExteriorFlow(DirectedFlow):
+    """
+    An ExteriorFlow is essentially a row in the LCI Environment `B` matrix. It consists of a directed flow,
+    enhanced with a context. Now I know a flow already has a context, but (a) context is not required for a flow and
+    (b) flows can be terminated to contexts other than their 'default'
+    """
+    context: List[str]
+
+    @classmethod
+    def from_background(cls, flow, direction, context):
+        if hasattr(context, 'entity_type'):
+            if context.entity_type == 'context':
+                cx = context.as_list()
+            else:
+                raise TypeError('supplied Context %s (type %s)' % (context, context.entity_type))
+        elif context is None:
+            cx = []
+        else:
+            cx = list(context)
+        return cls(flow=FlowSpec.from_flow(flow), direction=direction, context=cx)
+
+    @classmethod
+    def from_exchange(cls, obj):
+        if obj.type == 'context':
+            context = obj.termination.as_list()
+        elif obj.type == 'cutoff':
+            context = []
+        else:
+            raise TypeError('exchange is not exterior (type %s)' % obj.type)
+        return cls(flow=FlowSpec.from_exchange(obj), direction=obj.direction, context=context)
+
+
 class Exchange(ResponseModel):
     """
     Do we need to add locale??
     """
     origin: str
     process: str
     flow: FlowEntity
@@ -309,14 +336,23 @@
                    direction=x.direction, termination=term, context=cx, type=x.type, comment=x.comment, str=str(x), **kwargs)
 
 
 class ReferenceExchange(Exchange):
     is_reference: bool = True
     termination: None
 
+    @classmethod
+    def from_exchange(cls, x):
+        if x.termination is not None:
+            cx = list(x.termination)
+        else:
+            cx = None
+        return cls(origin=x.process.origin, process=x.process.external_ref, flow=FlowEntity.from_flow(x.flow),
+                   direction=x.direction, termination=None, context=cx, type=x.type, comment=x.comment, str=str(x))
+
 
 class ReferenceValue(ReferenceExchange):
     value: float
 
     @classmethod
     def from_rx(cls, x):
         return cls.from_exchange(x, value=x.value)
@@ -579,14 +615,15 @@
                    result=d.result)
 
 
 class DisaggregatedLciaScore(AggregatedLciaScore):
     details: List[LciaDetail] = []
 
     '''
+    :meta exclude:
     @classmethod
     def from_component(cls, obj, c):
         if hasattr(c.entity, 'name'):
             component = c.entity.name
         else:
             component = str(c.entity)
         if hasattr(c.entity, 'external_ref'):
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/models/auth.py` & `antelope_interface-0.2.4/src/antelope/models/auth.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/base.py` & `antelope_interface-0.2.4/src/antelope/refs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 The CatalogRef can instantiate a grounded reference if supplied with a query object that implements the interface.
 
 """
 from synonym_dict import LowerDict
 
 from ..flows import BaseEntity
-from ..interfaces.abstract_query import NoAccessToEntity, EntityNotFound
+from ..interfaces import NoAccessToEntity, EntityNotFound
 
 import re
 
 uuid_regex = re.compile('([0-9a-f]{8}-?([0-9a-f]{4}-?){3}[0-9a-f]{12})', flags=re.IGNORECASE)
 
 
 class NoCatalog(Exception):
@@ -386,16 +386,16 @@
         This keeps generating recursion errors. Let's think it through.
          - first checks locally. If known, great.
          - if not, need to check remotely by running the query.
          - the query retrieves the entity and asks has_property
            -- which causes recursion error if the query actually gets the entity_ref
            --- attempted solution with NoAccessToEntity exception in BasicImplementation
          - fine. So when do we raise a key error?
+
         :param item:
-        :param force_query:
         :return:
         """
         if item == self._ref_field:
             return self.reference_entity
         # check local first.  return Localitem if present.
         loc = self.get(item)
         if loc is _MissingItem:
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/catalog_ref.py` & `antelope_interface-0.2.4/src/antelope/refs/catalog_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/exchange_ref.py` & `antelope_interface-0.2.4/src/antelope/refs/exchange_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/flow_ref.py` & `antelope_interface-0.2.4/src/antelope/refs/flow_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/process_ref.py` & `antelope_interface-0.2.4/src/antelope/refs/process_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .base import EntityRef
+from .base import EntityRef, _MissingItem
 from .exchange_ref import ExchangeRef
 from itertools import chain
 
 
 class MultipleReferences(Exception):
     pass
 
@@ -17,14 +17,19 @@
 class ProcessRef(EntityRef):
     """
     Processes can lookup:
     """
     _etype = 'process'
     _ref_field = 'referenceExchange'
 
+    def signature_fields(self):
+        for k in ('Name', 'Comment', 'SpatialScope', 'TemporalScope'):
+            if self._d[k] is not _MissingItem:
+                yield k
+
     @property
     def _addl(self):
         return self.get('SpatialScope', default='')
 
     def __init__(self, external_ref, query, **kwargs):
         self._default_rx = None
         self._lci = dict()
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/quantity_ref.py` & `antelope_interface-0.2.4/src/antelope/refs/quantity_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,38 +197,46 @@
             return 1.0
         return self._query.cf(flow, self.external_ref, ref_quantity=ref_quantity, **kwargs)
 
     def characterize(self, flowable, ref_quantity, value, **kwargs):
         """
         Enter a characterization factor for the current object (query quantity) w.r.t. the specified reference quantity.
         The characterization value should report the amount of the query quantity (quantity being characterized) that
-         equals a unit of the reference quantity (used to measure the flow). The following is correct,
-         for mass in kg and volume in m3:
+        equals a unit of the reference quantity (used to measure the flow). The following is correct,
+        for mass in kg and volume in m3:
+
         >>> mass.characterize('water', 'volume', 1000.0)
-        "I {characterize} the [mass] of [water] in a unit [volume] to be 1000.0".  The thing being measured is mass.
+        "I {characterize} the [mass] of [water] in a unit [volume] to be 1000.0".
+
+        The thing being measured is mass.
         The flow's reference quantity is volume. a unit reference quantity of water is characterized as 1000.0 kg.
 
         The following is NOT correct, but it may SEEM more semantically natural:
+
         >>> mass.characterize('water', 'volume', 0.001)
         "I {characterize} the unit [mass] of [water] to have a [volume] of 0.001"
+
         The unit of the flow is measured in terms of the query quantity.  But we don't yet know the size of a unit
         of the query quantity because that is what is in fact being characterized.
 
         To see this borne out, imagine using characterize() in its most natural way, for LCIA:
+
         >>> gwp.characterize('methane', 'mass', 25)
         "I characterize the GWP of methane in a unit mass to be 25" <<--- CORRECT
         {I characterize the unit GWP of methane to have a mass of 0.04} <<--- plainly wrong
 
-        REALLY, the MOST natural way to characterize is as follows (see FlowRef.characterize()):
+        REALLY, the MOST natural way to characterize is to use `FlowRef.characterize()`:
+
         >>> m = q.get('methane')
         >>> m.unit
         'kg'
         >>> m.characterize(gwp, 25, context='to air')
 
         generations may determine whether this was a terrible mistake.
+
         :param flowable:
         :param ref_quantity:
         :param value:
         :param kwargs:
         :return:
         """
         return self._query.characterize(flowable, ref_quantity, self, value, **kwargs)
```

### Comparing `antelope_interface-0.2.3.2/src/antelope/refs/tests/test_flows.py` & `antelope_interface-0.2.4/src/antelope/refs/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope/xdb_tokens.py` & `antelope_interface-0.2.4/src/antelope/xdb_tokens.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.3.2/src/antelope_interface.egg-info/SOURCES.txt` & `antelope_interface-0.2.4/src/antelope_interface.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/antelope/flows/__init__.py
 src/antelope/flows/flow.py
 src/antelope/flows/flow_interface.py
 src/antelope/flows/openlca_locales.json
 src/antelope/interfaces/__init__.py
 src/antelope/interfaces/abstract_query.py
 src/antelope/interfaces/ibackground.py
+src/antelope/interfaces/ibasic.py
 src/antelope/interfaces/iconfigure.py
 src/antelope/interfaces/iexchange.py
 src/antelope/interfaces/iforeground.py
 src/antelope/interfaces/iindex.py
 src/antelope/interfaces/iquantity.py
 src/antelope/models/__init__.py
 src/antelope/models/auth.py
```

