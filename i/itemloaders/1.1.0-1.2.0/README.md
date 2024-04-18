# Comparing `tmp/itemloaders-1.1.0.tar.gz` & `tmp/itemloaders-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemloaders-1.1.0.tar", last modified: Fri Apr 21 09:00:08 2023, max compression
+gzip compressed data, was "itemloaders-1.2.0.tar", last modified: Thu Apr 18 09:56:24 2024, max compression
```

## Comparing `itemloaders-1.1.0.tar` & `itemloaders-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-21 08:59:57.000000 itemloaders-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 08:59:57.000000 itemloaders-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 09:00:08.439595 itemloaders-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 08:59:57.000000 itemloaders-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.435594 itemloaders-1.1.0/itemloaders/
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/itemloaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 09:00:08.439595 itemloaders-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-21 08:59:57.000000 itemloaders-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_base_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_loader_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_nested_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_nested_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_output_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_select_jmes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_selector_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_utils_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-18 09:56:14.000000 itemloaders-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:56:14.000000 itemloaders-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-18 09:56:23.996741 itemloaders-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-18 09:56:14.000000 itemloaders-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/itemloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/itemloaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 09:56:23.996741 itemloaders-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-18 09:56:14.000000 itemloaders-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_loader_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_nested_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_nested_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_output_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_select_jmes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_selector_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_utils_python.py
```

### Comparing `itemloaders-1.1.0/LICENSE` & `itemloaders-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/PKG-INFO` & `itemloaders-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.1.0
+Version: 1.2.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: w3lib>=1.17.0
+Requires-Dist: parsel>=1.5.0
+Requires-Dist: jmespath>=0.9.5
+Requires-Dist: itemadapter>=0.1.0
 
 ===========
 itemloaders
 ===========
 
 .. image:: https://img.shields.io/pypi/v/itemloaders.svg
    :target: https://pypi.python.org/pypi/itemloaders
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.1.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.2.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
-Description-Content-Type: text/x-rst License-File: LICENSE ===========
-itemloaders =========== .. image:: https://img.shields.io/pypi/v/
-itemloaders.svg :target: https://pypi.python.org/pypi/itemloaders :alt: PyPI
-Version .. image:: https://img.shields.io/pypi/pyversions/itemloaders.svg :
-target: https://pypi.python.org/pypi/itemloaders :alt: Supported Python
-Versions .. image:: https://github.com/scrapy/itemloaders/workflows/CI/
-badge.svg?branch=master :target: https://github.com/scrapy/itemloaders/
-actions?workflow=CI :alt: CI Status .. image:: https://codecov.io/github/
-scrapy/itemloaders/coverage.svg?branch=master :target: https://codecov.io/gh/
-scrapy/itemloaders :alt: Coverage report .. image:: https://readthedocs.org/
-projects/itemloaders/badge/?version=latest :target: https://
-itemloaders.readthedocs.io/en/latest/?badge=latest :alt: Documentation Status
-``itemloaders`` is a library that helps you collect data from HTML and XML
-sources. It comes in handy to extract data from web pages, as it supports data
-extraction using CSS and XPath Selectors. It's specially useful when you need
-to standardize the data from many sources. For example, it allows you to have
-all your casting and parsing rules in a single place. Here is an example to get
-you started:: from itemloaders import ItemLoader from parsel import Selector
-html_data = '''
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8
+Description-Content-Type: text/x-rst License-File: LICENSE Requires-Dist:
+w3lib>=1.17.0 Requires-Dist: parsel>=1.5.0 Requires-Dist: jmespath>=0.9.5
+Requires-Dist: itemadapter>=0.1.0 =========== itemloaders =========== ..
+image:: https://img.shields.io/pypi/v/itemloaders.svg :target: https://
+pypi.python.org/pypi/itemloaders :alt: PyPI Version .. image:: https://
+img.shields.io/pypi/pyversions/itemloaders.svg :target: https://
+pypi.python.org/pypi/itemloaders :alt: Supported Python Versions .. image::
+https://github.com/scrapy/itemloaders/workflows/CI/badge.svg?branch=master :
+target: https://github.com/scrapy/itemloaders/actions?workflow=CI :alt: CI
+Status .. image:: https://codecov.io/github/scrapy/itemloaders/
+coverage.svg?branch=master :target: https://codecov.io/gh/scrapy/itemloaders :
+alt: Coverage report .. image:: https://readthedocs.org/projects/itemloaders/
+badge/?version=latest :target: https://itemloaders.readthedocs.io/en/latest/
+?badge=latest :alt: Documentation Status ``itemloaders`` is a library that
+helps you collect data from HTML and XML sources. It comes in handy to extract
+data from web pages, as it supports data extraction using CSS and XPath
+Selectors. It's specially useful when you need to standardize the data from
+many sources. For example, it allows you to have all your casting and parsing
+rules in a single place. Here is an example to get you started:: from
+itemloaders import ItemLoader from parsel import Selector html_data = '''
 Some random product page
 $ 100.12
 ''' loader = ItemLoader(selector=Selector(html_data)) loader.add_xpath('name',
 '//div[@class="product_name"]/text()') loader.add_xpath('name', '//div
 [@class="product_title"]/text()') loader.add_css('price', '#price::text')
 loader.add_value('last_updated', 'today') # you can also use literal values
 item = loader.load_item() item # {'name': ['Some random product page'],
```

### Comparing `itemloaders-1.1.0/README.rst` & `itemloaders-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/itemloaders/__init__.py` & `itemloaders-1.2.0/itemloaders/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Item Loader
 
 See documentation in docs/topics/loaders.rst
 """
+
 from contextlib import suppress
 
 from itemadapter import ItemAdapter
 from parsel.utils import extract_regex, flatten
 
 from itemloaders.common import wrap_loader_context
 from itemloaders.processors import Identity
```

### Comparing `itemloaders-1.1.0/itemloaders/processors.py` & `itemloaders-1.2.0/itemloaders/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module provides some commonly used processors for Item Loaders.
 
 See documentation in docs/topics/loaders.rst
 """
+
 from collections import ChainMap
 
 from itemloaders.common import wrap_loader_context
 from itemloaders.utils import arg_to_iter
 
 
 class MapCompose:
```

### Comparing `itemloaders-1.1.0/itemloaders/utils.py` & `itemloaders-1.2.0/itemloaders/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 """
 Copy/paste from scrapy source at the moment, to ensure tests are working.
 Refactoring to come later
 """
+
 import inspect
 from functools import partial
+from typing import Generator
 
-from itemadapter import is_item
 
-_ITERABLE_SINGLE_VALUES = str, bytes
+def arg_to_iter(arg):
+    """Return an iterable based on *arg*.
 
+    If *arg* is a list, a tuple or a generator, it will be returned as is.
 
-def arg_to_iter(arg):
-    """Convert an argument to an iterable. The argument can be a None, single
-    value, or an iterable.
+    If *arg* is ``None``, an empty list will be returned.
 
-    Exception: if arg is a dict, [arg] will be returned
+    If *arg* is anything else, a list will be returned with *arg* as its only
+    item, i.e. ``[arg]``.
     """
     if arg is None:
         return []
-    elif (
-        hasattr(arg, "__iter__")
-        and not isinstance(arg, _ITERABLE_SINGLE_VALUES)
-        and not is_item(arg)
-    ):
+    if isinstance(arg, (list, tuple, Generator)):
         return arg
-    else:
-        return [arg]
+    return [arg]
 
 
 def get_func_args(func, stripself=False):
     """Return the argument name list of a callable object"""
     if not callable(func):
         raise TypeError(f"func must be callable, got {type(func).__name__!r}")
```

### Comparing `itemloaders-1.1.0/itemloaders.egg-info/PKG-INFO` & `itemloaders-1.2.0/itemloaders.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.1.0
+Version: 1.2.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: w3lib>=1.17.0
+Requires-Dist: parsel>=1.5.0
+Requires-Dist: jmespath>=0.9.5
+Requires-Dist: itemadapter>=0.1.0
 
 ===========
 itemloaders
 ===========
 
 .. image:: https://img.shields.io/pypi/v/itemloaders.svg
    :target: https://pypi.python.org/pypi/itemloaders
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.1.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.2.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
-Description-Content-Type: text/x-rst License-File: LICENSE ===========
-itemloaders =========== .. image:: https://img.shields.io/pypi/v/
-itemloaders.svg :target: https://pypi.python.org/pypi/itemloaders :alt: PyPI
-Version .. image:: https://img.shields.io/pypi/pyversions/itemloaders.svg :
-target: https://pypi.python.org/pypi/itemloaders :alt: Supported Python
-Versions .. image:: https://github.com/scrapy/itemloaders/workflows/CI/
-badge.svg?branch=master :target: https://github.com/scrapy/itemloaders/
-actions?workflow=CI :alt: CI Status .. image:: https://codecov.io/github/
-scrapy/itemloaders/coverage.svg?branch=master :target: https://codecov.io/gh/
-scrapy/itemloaders :alt: Coverage report .. image:: https://readthedocs.org/
-projects/itemloaders/badge/?version=latest :target: https://
-itemloaders.readthedocs.io/en/latest/?badge=latest :alt: Documentation Status
-``itemloaders`` is a library that helps you collect data from HTML and XML
-sources. It comes in handy to extract data from web pages, as it supports data
-extraction using CSS and XPath Selectors. It's specially useful when you need
-to standardize the data from many sources. For example, it allows you to have
-all your casting and parsing rules in a single place. Here is an example to get
-you started:: from itemloaders import ItemLoader from parsel import Selector
-html_data = '''
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8
+Description-Content-Type: text/x-rst License-File: LICENSE Requires-Dist:
+w3lib>=1.17.0 Requires-Dist: parsel>=1.5.0 Requires-Dist: jmespath>=0.9.5
+Requires-Dist: itemadapter>=0.1.0 =========== itemloaders =========== ..
+image:: https://img.shields.io/pypi/v/itemloaders.svg :target: https://
+pypi.python.org/pypi/itemloaders :alt: PyPI Version .. image:: https://
+img.shields.io/pypi/pyversions/itemloaders.svg :target: https://
+pypi.python.org/pypi/itemloaders :alt: Supported Python Versions .. image::
+https://github.com/scrapy/itemloaders/workflows/CI/badge.svg?branch=master :
+target: https://github.com/scrapy/itemloaders/actions?workflow=CI :alt: CI
+Status .. image:: https://codecov.io/github/scrapy/itemloaders/
+coverage.svg?branch=master :target: https://codecov.io/gh/scrapy/itemloaders :
+alt: Coverage report .. image:: https://readthedocs.org/projects/itemloaders/
+badge/?version=latest :target: https://itemloaders.readthedocs.io/en/latest/
+?badge=latest :alt: Documentation Status ``itemloaders`` is a library that
+helps you collect data from HTML and XML sources. It comes in handy to extract
+data from web pages, as it supports data extraction using CSS and XPath
+Selectors. It's specially useful when you need to standardize the data from
+many sources. For example, it allows you to have all your casting and parsing
+rules in a single place. Here is an example to get you started:: from
+itemloaders import ItemLoader from parsel import Selector html_data = '''
 Some random product page
 $ 100.12
 ''' loader = ItemLoader(selector=Selector(html_data)) loader.add_xpath('name',
 '//div[@class="product_name"]/text()') loader.add_xpath('name', '//div
 [@class="product_title"]/text()') loader.add_css('price', '#price::text')
 loader.add_value('last_updated', 'today') # you can also use literal values
 item = loader.load_item() item # {'name': ['Some random product page'],
```

### Comparing `itemloaders-1.1.0/itemloaders.egg-info/SOURCES.txt` & `itemloaders-1.2.0/itemloaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/setup.py` & `itemloaders-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="itemloaders",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/scrapy/itemloaders",
     project_urls={
         "Documentation": "https://itemloaders.readthedocs.io/",
         "Source": "https://github.com/scrapy/itemloaders",
     },
     description="Base library for scrapy's ItemLoader",
     long_description=long_description,
@@ -23,23 +23,23 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         # before updating these versions, be sure they are not higher than
         # scrapy's requirements
         "w3lib>=1.17.0",
         "parsel>=1.5.0",
         "jmespath>=0.9.5",
         "itemadapter>=0.1.0",
```

### Comparing `itemloaders-1.1.0/tests/test_base_loader.py` & `itemloaders-1.2.0/tests/test_base_loader.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_loader_initialization.py` & `itemloaders-1.2.0/tests/test_loader_initialization.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_nested_items.py` & `itemloaders-1.2.0/tests/test_nested_items.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_nested_loader.py` & `itemloaders-1.2.0/tests/test_nested_loader.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_output_processor.py` & `itemloaders-1.2.0/tests/test_output_processor.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_processors.py` & `itemloaders-1.2.0/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_select_jmes.py` & `itemloaders-1.2.0/tests/test_select_jmes.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_selector_loader.py` & `itemloaders-1.2.0/tests/test_selector_loader.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_utils_misc.py` & `itemloaders-1.2.0/tests/test_utils_misc.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.1.0/tests/test_utils_python.py` & `itemloaders-1.2.0/tests/test_utils_python.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,19 @@
         self.assertEqual(get_func_args(partial_f3), ["c"])
         self.assertEqual(get_func_args(cal), ["a", "b", "c"])
         self.assertEqual(get_func_args(object), [])
         self.assertEqual(get_func_args(str.split, stripself=True), ["sep", "maxsplit"])
         self.assertEqual(get_func_args(" ".join, stripself=True), ["iterable"])
 
         if platform.python_implementation() == "CPython":
-            # doesn't work on CPython: https://bugs.python.org/issue42785
-            self.assertEqual(get_func_args(operator.itemgetter(2)), [])
+            # This didn't work on older versions of CPython: https://github.com/python/cpython/issues/86951
+            self.assertIn(
+                get_func_args(operator.itemgetter(2), stripself=True),
+                [[], ["args", "kwargs"]],
+            )
         elif platform.python_implementation() == "PyPy":
             self.assertEqual(
                 get_func_args(operator.itemgetter(2), stripself=True), ["obj"]
             )
 
 
 if __name__ == "__main__":
```

