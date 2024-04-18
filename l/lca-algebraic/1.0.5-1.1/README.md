# Comparing `tmp/lca_algebraic-1.0.5.tar.gz` & `tmp/lca_algebraic-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lca_algebraic-1.0.5.tar", last modified: Tue Sep 13 16:15:07 2022, max compression
+gzip compressed data, was "lca_algebraic-1.1.tar", last modified: Thu Apr 18 15:58:22 2024, max compression
```

## Comparing `lca_algebraic-1.0.5.tar` & `lca_algebraic-1.1.tar`

### file list

```diff
@@ -1,48 +1,36 @@
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      170 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/.gitignore
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic-1.0.5/LICENSE
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      927 2021-06-23 08:53:38.000000 lca_algebraic-1.0.5/Makefile
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4387 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3904 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/README.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4487 2022-09-13 16:14:05.000000 lca_algebraic-1.0.5/RELEASE_NOTES.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        5 2022-09-13 16:12:30.000000 lca_algebraic-1.0.5/VERSION
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.100245 lca_algebraic-1.0.5/conda-recipe/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      795 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/conda-recipe/meta.yaml
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      460 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/construct.yaml
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/doc/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    17897 2021-06-23 09:18:46.000000 lca_algebraic-1.0.5/doc/base_utils.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   156146 2020-03-24 15:08:44.000000 lca_algebraic-1.0.5/doc/doc.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    88740 2021-06-23 09:18:46.000000 lca_algebraic-1.0.5/doc/helpers.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    12016 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/doc/index.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    10282 2021-06-23 09:18:46.000000 lca_algebraic-1.0.5/doc/io.html
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)    29363 2020-03-24 15:08:44.000000 lca_algebraic-1.0.5/doc/lca-algebraic.odp
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)   206268 2020-03-24 15:08:44.000000 lca_algebraic-1.0.5/doc/lca-algebraic.png
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    49312 2021-06-23 09:18:46.000000 lca_algebraic-1.0.5/doc/lca.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   100461 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/doc/params.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    76217 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/doc/stats.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    21081 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/example-notebook.Rmd
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  1257599 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/example-notebook.ipynb
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    21067 2022-08-03 18:27:03.000000 lca_algebraic-1.0.5/example-notebook.md
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/lca_algebraic/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1292 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/lca_algebraic/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3815 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/lca_algebraic/base_utils.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26505 2022-09-13 16:09:14.000000 lca_algebraic-1.0.5/lca_algebraic/helpers.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1928 2022-08-03 18:31:45.000000 lca_algebraic-1.0.5/lca_algebraic/io.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    20729 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/lca_algebraic/lca.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    31641 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/lca_algebraic/params.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    36432 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/lca_algebraic/stats.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/lca_algebraic.egg-info/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4387 2022-09-13 16:15:06.000000 lca_algebraic-1.0.5/lca_algebraic.egg-info/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      787 2022-09-13 16:15:07.000000 lca_algebraic-1.0.5/lca_algebraic.egg-info/SOURCES.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2022-09-13 16:15:06.000000 lca_algebraic-1.0.5/lca_algebraic.egg-info/dependency_links.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       86 2022-09-13 16:15:06.000000 lca_algebraic-1.0.5/lca_algebraic.egg-info/requires.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2022-09-13 16:15:06.000000 lca_algebraic-1.0.5/lca_algebraic.egg-info/top_level.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      127 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/requirements.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       38 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/setup.cfg
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1861 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/setup.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/test/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic-1.0.5/test/__init__.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2022-09-13 16:15:07.104245 lca_algebraic-1.0.5/test/fixtures/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1508 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/test/fixtures/__init__.py
--rwxr-xr-x   0 rjolivet  (1000) rjolivet  (1000)     1015 2020-03-24 15:08:44.000000 lca_algebraic-1.0.5/test/notebook_runner.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    10436 2022-09-13 15:51:20.000000 lca_algebraic-1.0.5/test/tests.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-18 15:58:22.035438 lca_algebraic-1.1/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-18 15:56:46.000000 lca_algebraic-1.1/.gitignore
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic-1.1/LICENSE
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-18 15:56:46.000000 lca_algebraic-1.1/Makefile
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2595 2024-04-18 15:58:22.035438 lca_algebraic-1.1/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1867 2024-04-18 15:56:46.000000 lca_algebraic-1.1/README.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5451 2024-04-18 15:57:55.000000 lca_algebraic-1.1/RELEASE_NOTES.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-04-18 15:58:00.000000 lca_algebraic-1.1/VERSION
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-18 15:58:22.035438 lca_algebraic-1.1/lca_algebraic/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1095 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    22533 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/activity.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4385 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/base_utils.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3023 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/cache.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/database.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3010 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/interpolation.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/io.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    27718 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/lca.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/log.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1640 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/methods.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    40757 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/params.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39543 2024-04-18 15:56:46.000000 lca_algebraic-1.1/lca_algebraic/stats.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-18 15:58:22.035438 lca_algebraic-1.1/lca_algebraic.egg-info/
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2595 2024-04-18 15:58:21.000000 lca_algebraic-1.1/lca_algebraic.egg-info/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      669 2024-04-18 15:58:21.000000 lca_algebraic-1.1/lca_algebraic.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-04-18 15:58:21.000000 lca_algebraic-1.1/lca_algebraic.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       99 2024-04-18 15:58:21.000000 lca_algebraic-1.1/lca_algebraic.egg-info/requires.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-04-18 15:58:21.000000 lca_algebraic-1.1/lca_algebraic.egg-info/top_level.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      144 2024-04-18 15:56:46.000000 lca_algebraic-1.1/requirements.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-04-18 15:58:22.035438 lca_algebraic-1.1/setup.cfg
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2017 2024-04-18 15:56:46.000000 lca_algebraic-1.1/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-18 15:58:22.035438 lca_algebraic-1.1/test/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic-1.1/test/__init__.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-18 15:58:22.035438 lca_algebraic-1.1/test/fixtures/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1543 2024-04-18 15:56:46.000000 lca_algebraic-1.1/test/fixtures/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-18 15:56:46.000000 lca_algebraic-1.1/test/test_axis_dict.py
```

### Comparing `lca_algebraic-1.0.5/LICENSE` & `lca_algebraic-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lca_algebraic-1.0.5/RELEASE_NOTES.md` & `lca_algebraic-1.1/RELEASE_NOTES.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,22 @@
-# 1.0.5 
+# 1.1
 
-Fix bug in ActivityExtended#getExchanges introduced by merge #14
+* Fixed bug in ActivityExtended#getExchanges introduced by merge #14
+* Added linear interpolation between activities with function `interpolate_activities`
+* Rename multiLCaAlgebraic => compute_impacts
+* Added breakdown of impacts by arbitrary attribute with the parameter `axis` of `compute_impacts`
+* Added `functional_unit` in compute_impacts : You are not obliged to define a custom activity anymore 
+* findActivities() is now case insensitive by default
+* Fixed bug #38 : getOutputAmount was wrong with activities having circular input exchanges with themselves
+* Fixed bug #37 : Increased number of results in findActivities
+* Added disk cache of LCIA results and act Expressions
+* Fixed bug when loading params with undefined uncertainty
+* Added "formula" in params, to have parameters automatically computed from others
+* Added option *return_params* in compute_impacts that returns "Tabbed Dataframe" to display / save as excel both results and all parameters   
+* Remove support for conda : Only pip install supported now
 
 # 1.0.4 
 
 Fix typo in helpers
 
 # 1.0.3
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/base_utils.py` & `lca_algebraic-1.1/lca_algebraic/base_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,147 +1,169 @@
 from contextlib import AbstractContextManager
-from sys import stderr
-from typing import Union
+from inspect import isfunction
+from typing import Dict, Iterable, Union
 
 import brightway2 as bw
-from bw2data.backends.peewee import Activity, ExchangeDataset
-from six import raise_from
-from sympy import Basic
-from sympy.parsing.sympy_parser import parse_expr
 import ipywidgets as widgets
-from IPython.core.display import display
 import numpy as np
+import pandas as pd
+from bw2data.backends.peewee import Activity
+from IPython.display import display
+from six import raise_from
+from sympy import Expr
 
-DEBUG=False
-LANG="fr"
-UNIT_OVERRIDE = dict()
-
-
-def set_debug(value=True) :
-    """ Activate debug logs """
-    global DEBUG
-    DEBUG=value
-
-def set_lang(lang):
-    """Set language """
-    global LANG
-    LANG=lang
-
-def debug(*args, **kwargs) :
-    if DEBUG :
-        print(*args, **kwargs)
-
-def error(*args, **kwargs):
-    """Print message on stderr """
-    print(*args, **kwargs, file=stderr)
+_user_functions = dict()
 
 
-def _isOutputExch(exc) :
-    return exc.get('input') == exc.get('output') or exc.get("type") == "production"
+def _isOutputExch(exc):
+    return exc.get("type") == "production"
 
 
 def _isnumber(value):
     return isinstance(value, int) or isinstance(value, float)
 
+
 dbs = dict()
+
+
 def _getDb(dbname) -> bw.Database:
     """Pool of Database instances"""
-    if not dbname in dbs:
+    if dbname not in dbs:
         dbs[dbname] = bw.Database(dbname)
     return dbs[dbname]
 
 
-def interpolate(x, x1, x2, y1, y2):
-    """Build an expression for linear interpolation between two points.
-    If x is not within [x1, x2] the corresponding bound Y values are returned"""
-    x = Min(Max(x, x1), x2)
-    return y1 + (y2 - y1) * (x - x1) / (x2 - x1)
-
-
-def Max(a, b) :
-    """Max define as algrebraic forumal with 'abs' for proper computation on vectors """
+def Max(a, b):
+    """Max define as algrebraic forumal with 'abs' for proper computation on vectors"""
     return (a + b + abs(a - b)) / 2
 
 
-def Min(a, b) :
-    """Max define as algrebraic forumal with 'abs' for proper computation on vectors """
+def Min(a, b):
+    """Max define as algrebraic forumal with 'abs' for proper computation on vectors"""
     return (a + b - abs(b - a)) / 2
 
 
-def _actDesc(act: Activity):
-    """Generate pretty name for activity + basic information """
-    name = _actName(act)
-    amount = 1
-    for ex in act.exchanges() :
-        if _isOutputExch(ex):
-            amount = ex['amount']
-
-    return "%s (%f %s)" % (name, amount, act['unit'])
-
-
-def _method_unit(method) :
-    if method in UNIT_OVERRIDE :
-        return UNIT_OVERRIDE[method]
-    return bw.Method(method).metadata['unit']
-
-
 def _actName(act: Activity):
-    
-    """Generate pretty name for activity, appending location if not 'GLO' """
-    res = act['name']
-    if 'location' in act and act['location'] != 'GLO':
+    """Generate pretty name for activity, appending location if not 'GLO'"""
+    res = act["name"]
+    if "location" in act and act["location"] != "GLO":
         res += "[%s]" % act["location"]
     return res
 
 
-def _getAmountOrFormula(ex: ExchangeDataset) -> Union[Basic, float]:
-    """ Return either a fixed float value or an expression for the amount of this exchange"""
-    if 'formula' in ex:
-        try:
-            return parse_expr(ex['formula'])
-        except:
-            error("Error while parsing formula '%s' : backing to amount" % ex['formula'])
-
-    return ex['amount']
-
-
 def displayWithExportButton(df):
-    '''Display dataframe with option to export'''
+    """Display dataframe with option to export"""
 
     button = widgets.Button(description="Export data")
     button.style.button_color = "lightgray"
-    def click(e) :
+
+    def click(e):
         df.to_csv("out.csv")
         button.description = "exported as 'out.csv'"
+
     dfout = widgets.Output()
-    with dfout :
+    with dfout:
         display(df)
 
     button.on_click(click)
 
     display(widgets.VBox([button, dfout]))
 
 
-def as_np_array(a) :
-    if type(a) == list :
+def as_np_array(a):
+    if isinstance(a, list):
         return np.asarray(a)
-    else :
+    else:
         return a
 
+
 def r_squared(y, y_hat):
     y_bar = y.mean()
     ss_tot = ((y - y_bar) ** 2).sum()
     ss_res = ((y - y_hat) ** 2).sum()
     return 1 - (ss_res / ss_tot)
 
 
-class  ExceptionContext(AbstractContextManager) :
+class ExceptionContext(AbstractContextManager):
     def __init__(self, context):
         self.context = context
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        if exc_val != None :
+        if exc_val is not None:
             raise_from(Exception("Context : %s" % str(self.context)), exc_val)
         return True
 
+
 def _snake2camel(val):
-    return ''.join(word.title() for word in val.split('_'))
+    return "".join(word.title() for word in val.split("_"))
+
+
+class TabbedDataframe:
+    """This class holds a dictionnary of dataframes and can display and saved them awith 'tabs'/'sheets'"""
+
+    def __init__(self, metadata=dict(), **dataframes):
+        self.dataframes = dataframes
+        self.metadata = metadata
+
+    def __str__(self):
+        res = ""
+        for name, df in self.dataframes.items():
+            res += f"\n{name} : \n"
+            res += df.__str__() + "\n"
+        return res
+
+    def _repr_html_(self):
+        display(_mk_tabs(self.dataframes))
+
+    def to_excel(self, filename):
+        assert filename.endswith(".xlsx")
+
+        with pd.ExcelWriter(filename, engine="xlsxwriter") as writer:
+            for itab, (name, df) in enumerate(self.dataframes.items()):
+                if itab == 0:
+                    df.to_excel(writer, sheet_name=name, startrow=len(self.metadata) + 1)
+
+                    # Write metadata in header
+                    worksheet = writer.sheets[name]
+                    for imeta, (key, val) in enumerate(self.metadata.items()):
+                        worksheet.write_string(imeta, 0, str(key))
+                        worksheet.write_string(imeta, 1, str(val))
+
+                else:
+                    df.to_excel(writer, sheet_name=name)
+
+
+def _mk_tabs(titlesAndContent: Dict):
+    """Generate iPywidget tabs"""
+    tabs = []
+    titles = []
+    for title, content in titlesAndContent.items():
+        titles.append(title)
+
+        tab = widgets.Output()
+        with tab:
+            if isfunction(content):
+                content()
+            else:
+                display(content)
+        tabs.append(tab)
+
+    res = widgets.Tab(children=tabs)
+    for i, title in enumerate(titles):
+        res.set_title(i, title)
+    return res
+
+
+def _display_tabs(titlesAndContent: Dict):
+    display(_mk_tabs(titlesAndContent))
+
+
+def one(it: Iterable):
+    """Expect a list with single value a returns it"""
+    it = list(it)
+    if len(it) != 1:
+        raise Exception(f"Expected a single value but got {len(it)}")
+    return it[0]
+
+
+# Custom types
+ValueOrExpression = Union[float, Expr]
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/helpers.py` & `lca_algebraic-1.1/lca_algebraic/activity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,338 +1,228 @@
-import functools
-import inspect
 import re
-import types
-
+from collections import defaultdict
 from copy import deepcopy
-from itertools import chain
+from types import FunctionType
+from typing import Dict, Tuple, Union
 
+import brightway2 as bw
 import pandas as pd
+from bw2data.backends.peewee import Activity, ExchangeDataset
 from bw2data.backends.peewee.utils import dict_as_exchangedataset
-from bw2data.meta import databases as dbmeta
-from sympy import symbols
-
-from .base_utils import *
-from .base_utils import _getDb, _actDesc, _getAmountOrFormula, _actName, _isOutputExch
-from .params import *
-from .params import _param_registry, _completeParamValues
-from typing import Tuple, Dict
-import inspect
-
-
-BIOSPHERE3_DB_NAME="biosphere3"
-
-_metaCache = defaultdict(lambda : {})
-
-def _setMeta(dbname, key, value) :
-    """Set meta param on DB"""
-    _metaCache[dbname][key] = value
-
-    data = dbmeta[dbname]
-    data[key] = value
-    dbmeta[dbname] = data
-    dbmeta.flush()
-
-
-def _getMeta(db_name, key) :
+from sympy import Basic, symbols
 
-    if key in _metaCache[db_name] :
-        return _metaCache[db_name][key]
+from lca_algebraic.base_utils import _actName, _getDb, _isOutputExch
+from lca_algebraic.database import (
+    _find_biosphere_db,
+    _isForeground,
+    _listTechBackgroundDbs,
+    with_db_context,
+)
+from lca_algebraic.params import (
+    DbContext,
+    ParamDef,
+    _complete_and_expand_params,
+    _getAmountOrFormula,
+    _param_registry,
+)
 
-    val = dbmeta[db_name].get(key)
-    _metaCache[db_name][key] = val
-    return val
+from .log import warn
 
-FOREGROUND_KEY = "fg"
+# Can be used in expression of amount for updateExchanges, in order to reference the previous value
+old_amount = symbols("old_amount")
 
-def _isForeground(db_name) :
-    """ Check is db is marked as foreground DB : which means activities may be parametrized / should be developped. """
-    return _getMeta(db_name, FOREGROUND_KEY)
-
-def setForeground(db_name) :
-    """ Set a db as being a foreground database, meaning it is parametrized and lca_algebraic should develop its activities"""
-    return _setMeta(db_name, FOREGROUND_KEY, True)
-
-def setBackground(db_name) :
-    """ Set a db as being a foreground database, meaning it should be considred as static"""
-    return _setMeta(db_name, FOREGROUND_KEY, False)
-
-def SET_USER_DB(db_name) :
-    """Deprecated, use #setForeground() / setBackground() instead"""
-    error("Deprecated, use #setForeground() / setBackground() instead")
-    setForeground(db_name)
-
-def _listTechBackgroundDbs() :
-    """List all background databases technosphere (non biosphere) batabases"""
-    return list(name for name in bw.databases if not _isForeground(name) and not name == BIOSPHERE3_DB_NAME)
-
-old_amount = symbols("old_amount")  # Can be used in expression of amount for updateExchanges, in order to reference the previous value
 NumOrExpression = Union[float, Basic]
 
 
-def list_databases() :
-    """List of databases and their status"""
-    data = list(
-        dict(
-            name=name,
-            backend=_getMeta(name, "backend"),
-            type="foreground" if _isForeground(name) else "background") for name in bw.databases)
-    res = pd.DataFrame(data)
-    return res.set_index("name")
-
-
-def with_db_context(func=None, arg="self"):
-    """ Internal decorator wrapping function into DbContext, using its first parameters (either Activity, Db or Db name)"""
-
-    if func is None:
-        return functools.partial(with_db_context, arg=arg)
-
-    param_specs = inspect.signature(func).parameters
-
-    if not arg in param_specs :
-        raise Exception("No param %s in signature of %s" % (arg, func))
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-
-        # Transform all parameters (positionnal and named) to named ones
-        all_param = {
-            k: args[n] if n < len(args) else v.default
-            for n, (k, v) in enumerate(param_specs.items()) if k != 'kwargs'
-        }
-        all_param.update(kwargs)
-
-        val = all_param[arg]
-        if hasattr(val, "key") :
-            # value is an activity
-            dbname = val.key[0]
-        elif isinstance(val, str) :
-            # Value is directly a  db_name
-            dbname = val
-        else:
-            raise Exception("Param %s is neither an Activity or a db_name : %s" % (arg, val))
-
-        with DbContext(dbname) :
-            return func(*args, **kwargs)
-
-    return wrapper
-
-
 def _exch_name(exch):
-    return exch['name'] if 'name' in exch else str(exch.input)
+    return exch["name"] if "name" in exch else str(exch.input)
+
 
 class ActivityExtended(Activity):
     """Improved API for activity : adding a few useful methods.
     Those methods are backported to #Activity in order to be directly available on all existing instances
     """
 
     @with_db_context
-    def listExchanges(self) :
-        """ Iterates on all exchanges (except "production") and return a list of (exch-name, target-act, amount) """
+    def listExchanges(self):
+        """Iterates on all exchanges (except "production") and return a list of (exch-name, target-act, amount)"""
         res = []
         for exc in self.exchanges():
-
             # Don't show production
-            if _isOutputExch(exc) :
+            if _isOutputExch(exc):
                 continue
 
             input = bw.get_activity(exc.input.key)
             amount = _getAmountOrFormula(exc)
             res.append((exc["name"], input, amount))
         return res
 
     @with_db_context
-    def getExchange(self, name=None, input=None, single=True):
+    def getExchange(self, name: str = None, input: Activity = None, single=True):
         """Get exchange by name or input
 
         Parameters
         ----------
-        name : name of the exchange. Name can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
+        name :
+            name of the exchange. Name can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
             It can also be suffised by '*' to match an exchange starting with this name. Location can be a negative match '!'
-            Exampple : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+            Example  "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+
+        input :
+            input activity
 
-        single :True if a single match is expected. Otherwize, a list of result is returned
+        single :
+            True if a single match is expected. Otherwize, a list of result is returned
 
         Returns
         -------
-            Single exchange or list of exchanges (if _single is False or "name" contains a '*')
-            raise Exception if not matching exchange found
+        Single exchange or list of exchanges (if _single is False or "name" contains a '*')
+        raise Exception if not matching exchange found
+
         """
 
         def single_match(name, exch):
-
             # Name can be "Elecricity#RER"
             if "#" in name:
                 name, loc = name.split("#")
                 negative = False
                 if loc.startswith("!"):
                     negative = True
                     loc = loc[1:]
-                act = getActByCode(*exch['input'])
+                act = getActByCode(*exch["input"])
 
-                if not 'location' in act or (negative and act['location'] == loc) or (
-                        not negative and act['location'] != loc):
+                if "location" not in act or (negative and act["location"] == loc) or (not negative and act["location"] != loc):
                     return False
 
-            if '*' in name:
-                name = name.replace('*', '')
-                return name in  _exch_name(exch)
+            if "*" in name:
+                name = name.replace("*", "")
+                return name in _exch_name(exch)
             else:
                 return name == _exch_name(exch)
 
-
         def match(exch):
             if name:
                 if isinstance(name, list):
                     return any(single_match(iname, exch) for iname in name)
                 else:
                     return single_match(name, exch)
 
             if input:
-                return input == exch['input']
+                return input == exch["input"]
 
-        exchs = list(exch for exch in self.exchangesNp() if match(exch))
+        exchs = list(exch for exch in self.non_production_exchanges() if match(exch))
         if len(exchs) == 0:
             raise Exception("Found no exchange matching name : %s" % name)
 
         if single and len(exchs) != 1:
             raise Exception("Expected 1 exchange with name '%s' found %d" % (name, len(exchs)))
         if single:
             return exchs[0]
         else:
             return exchs
 
     def setOutputAmount(self, amount):
-        '''Set the amount for the single output exchange (1 by default)'''
+        """Set the amount for the single output exchange (1 by default)"""
         self.addExchanges({self: amount})
 
     @with_db_context
     def updateExchanges(self, updates: Dict[str, any] = dict()):
-
         """Update existing exchanges, by name.
 
         Parameters
         ----------
         updates : Dict of "<exchange name>" => <new value>
 
             <exchange name> can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
             It can also be suffixed by '*' to match an exchange starting with this name. Location can be a negative match '!'
-            Exampple : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+            Example : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
 
-            <New Value>  : either single value (float or SympPy expression) for updating only amount, or activity for updating only input,
+            <New Value>  : either single value (float or SympPy expression) for updating only amount, \
+                or activity for updating only input,
             or dict of attributes, for updating both at once, or any other attribute.
             The amount can reference the symbol 'old_amount' that will be replaced with the current amount of the exchange.
         """
 
-        parametrized = False
-
         # Update exchanges
         for name, attrs in updates.items():
-
-            exchs = self.getExchange(name, single=not '*' in name)
+            exchs = self.getExchange(name, single="*" not in name)
             if not isinstance(exchs, list):
                 exchs = [exchs]
 
-
             for exch in exchs:
-
                 if attrs is None:
                     exch.delete()
                     exch.save()
                     continue
 
                 # Single value ? => amount
                 if not isinstance(attrs, dict):
                     if isinstance(attrs, Activity):
                         attrs = dict(input=attrs)
                     else:
                         attrs = dict(amount=attrs)
 
-                if 'amount' in attrs:
-                    attrs.update(_amountToFormula(attrs['amount'], exch['amount']))
+                if "amount" in attrs:
+                    attrs.update(_amountToFormula(attrs["amount"], exch["amount"]))
 
                 exch.update(attrs)
                 exch.save()
 
-                # We have a formula now ? => register it to parametrized exchange
-                if 'formula' in attrs:
-                    parametrized = True
+    def deleteExchanges(self, name, single=True):
+        """Remove matching exchanges
 
+        Parameters
+        ----------
+        name:
+            Name of the exchange to delete. Can contain wildcards. See #getExchange for more details.
 
-    def deleteExchanges(self, name, single=True):
-        ''' Remove matching exchanges '''
+        single:
+            If true (default) expect to only delete a single exchange
+        """
         exchs = self.getExchange(name, single=single)
         if not isinstance(exchs, list):
             exchs = [exchs]
         if len(exchs) == 0:
             raise Exception("No exchange found for '%s'" % name)
         for ex in exchs:
             ex.delete()
             ex.save()
         self.save()
 
     @with_db_context
-    def substituteWithDefault(self, exchange_name: str, switch_act: Activity, paramSwitch: EnumParam, amount=None):
-
-        """Substitutes one exchange with a switch on other activities, or fallback to the current one as default (parameter set to None)
-        For this purpose, we create a new exchange referencing the activity switch, and we multiply current activity by '<param_name>_default',
-        making it null as soon as one enum value is set.
-
-        This is useful for changing electricty mix, leaving the default one if needed
-
-        Parameters
-        ----------
-        act : Activity to update
-        exchange_name : Name of the exchange to update
-        switch_act : Activity to substitue as input
-        amount : Amount of the input (uses previous amount by default)
-        """
-
-        current_exch = self.getExchange(exchange_name)
-
-        prev_amount = amount if amount else _getAmountOrFormula(current_exch)
-
-        self.addExchanges({switch_act: prev_amount})
-        self.updateExchanges({exchange_name: paramSwitch.symbol(None) * prev_amount})
-
-    @with_db_context
     def addExchanges(self, exchanges: Dict[Activity, Union[NumOrExpression, dict]] = dict()):
         """Add exchanges to an existing activity, with a compact syntax :
 
         Parameters
         ----------
-        exchanges : Dict of activity => amount or activity => attributes_dict. \
+        exchanges :
+            Dict of activity => amount or activity => attributes_dict. \
             Amount being either a fixed value or Sympy expression (arithmetic expression of Sympy symbols)
         """
 
-        with DbContext(self.key[0]) :
-
+        with DbContext(self.key[0]):
             for sub_act, attrs in exchanges.items():
-
                 if isinstance(attrs, dict):
-                    amount = attrs.pop('amount')
+                    amount = attrs.pop("amount")
                 else:
                     amount = attrs
                     attrs = dict()
 
                 exch = self.new_exchange(
                     input=sub_act.key,
-                    name=sub_act['name'],
-                    unit=sub_act['unit'] if 'unit' in sub_act else None,
-                    type='production' if self == sub_act else 'technosphere' if sub_act.get('type') == 'process' else 'biosphere')
+                    name=sub_act["name"],
+                    unit=sub_act["unit"] if "unit" in sub_act else None,
+                    type="production" if self == sub_act else "technosphere" if sub_act.get("type") == "process" else "biosphere",
+                )
 
                 exch.update(attrs)
                 exch.update(_amountToFormula(amount))
-                if 'formula' in exch:
-                    parametrized = True
-
                 exch.save()
             self.save()
 
-
     @with_db_context
     def getAmount(self, *args, sum=False, **kargs):
         """
         Get the amount of one or several exchanges, selected by name or input. See #getExchange()
         """
         exchs = self.getExchange(*args, single=not sum, **kargs)
         if sum:
@@ -342,332 +232,400 @@
             for exch in exchs:
                 res += _getAmountOrFormula(exch)
             return res
         else:
             return _getAmountOrFormula(exchs)
 
     def getOutputAmount(self):
+        """Return the amount of the production : 1 if none is found"""
+        res = 1.0
 
-        """ Return the amount of the production : 1 if none is found """
-        res = 1
-        for exch in self.exchanges() :
-            if exch['input'] == exch['output']:
-                # Not 1 ?
-                if exch['amount'] != 1:
-                    res = exch['amount']
+        for exch in self.exchanges():
+            if (exch["input"] == exch["output"]) and (exch["type"] == "production"):
+                res = exch["amount"]
                 break
         return res
 
-
-    def exchangesNp(self):
-        """ List of exchange, except production (output) one."""
+    def non_production_exchanges(self):
+        """List of exchange, except production (output) one."""
         for exch in self.exchanges():
-            if exch['input'] != exch['output']:
+            if exch["input"] != exch["output"]:
                 yield exch
 
-
-# Backport new methods to vanilla Activity class in order to benefit from it for all existing instances
-for name, item in ActivityExtended.__dict__.items():
-    if isinstance(item, types.FunctionType):
-        setattr(Activity, name, item)
-
-
-def _split_words(name):
-    clean = re.sub('[^0-9a-zA-Z]+', ' ', name)
-    clean = re.sub(' +', ' ', clean)
-    clean = clean.lower()
-
-    return clean.split(' ')
-
-
-def _build_index(db):
-    res = defaultdict(set)
-    for act in db:
-        words = _split_words(act['name'])
-        for word in words:
-            res[word].add(act)
-    return res
-
-
-# Index of activities per name, for fast search dict[db_name][activity_word] => list of activitites
-db_index = dict()
-
-
-def _get_indexed_db(db_name):
-    if not db_name in db_index:
-        db_index[db_name] = _build_index(_getDb(db_name))
-    return db_index[db_name]
-
-
-def _find_candidates(db_name, name):
-    res = []
-    index = _get_indexed_db(db_name)
-    words = _split_words(name)
-    for word in words:
-        candidates = index[word]
-        if len(res) == 0 or (0 < len(candidates) < len(res)):
-            res = list(candidates)
-    return res
+    def updateMeta(self, **kwargs):
+        """Update any property. Useful to update axes"""
+        for key, val in kwargs.items():
+            self._data[key] = val
+        self.save()
 
 
 def getActByCode(db_name, code):
-    """ Get activity by code """
+    """Get activity by code"""
     return _getDb(db_name).get(code)
 
 
-def findActivity(name=None, loc=None, in_name=None, code=None, categories=None, category=None, db_name=None,
-                 single=True, unit=None) -> ActivityExtended :
+def findActivity(
+    name=None,
+    loc=None,
+    code=None,
+    categories=None,
+    category=None,
+    db_name=None,
+    single=True,
+    case_sensitive=False,
+    unit=None,
+    limit=1500,
+) -> ActivityExtended:
     """
-        Find single activity by name & location
+        Find activity by name & location
         Uses index for fast fetching
+
+    :param name: Name of the activity. Can contain '*' for searching partial chain
+    :param loc: optional location
+    :param code: Unique code. If provided alone, returns the activity for this code
+    :param categories: Optional : exact list of catagories
+    :param category: Optional : single category that should be part of the list of categories of the selected activities
+    :param db_name: Name of the database
+    :param single: If False, returns a list of matching activities. If True (default) fails if more than one activity fits.
+    :param case_sensitive: If True (default) ignore the case
+    :param unit: If provided, only match activities with provided unit
+    :return: Either a single activity (if single is True) or a list of activities, possibly empty.
     """
 
-    if name and '*' in name:
+    in_name = None
+
+    if name and "*" in name:
         in_name = name.replace("*", "")
         name = None
 
+    if not case_sensitive:
+        if name:
+            name = name.lower()
+        if in_name:
+            in_name = in_name.lower()
+
     def act_filter(act):
-        if name and not name == act['name']:
+        act_name = act["name"]
+        if not case_sensitive:
+            act_name = act_name.lower()
+
+        if name and not name == act_name:
             return False
-        if in_name and not in_name in act['name']:
+        if in_name and in_name not in act_name:
             return False
-        if loc and not loc == act['location']:
+        if loc and not loc == act["location"]:
             return False
-        if unit and not unit == act['unit']:
+        if unit and not unit == act["unit"]:
             return False
-        if category and not category in act['categories']:
+        if category and category not in act["categories"]:
             return False
-        if categories and not tuple(categories) == act['categories']:
+        if categories and not tuple(categories) == tuple(act["categories"]):
             return False
         return True
 
     if code:
         acts = [getActByCode(db_name, code)]
     else:
         search = name if name is not None else in_name
 
         search = search.lower()
-        search = search.replace(',', ' ')
+        search = search.replace(",", " ")
 
         # Find candidates via index
         # candidates = _find_candidates(db_name, name_key)
-        candidates = _getDb(db_name).search(search, limit=200)
+        candidates = _getDb(db_name).search(search, limit=limit)
 
-        if len(candidates) == 0 :
+        if len(candidates) == 0:
             # Try again removing strange caracters
-            search = re.sub(r'\w*[^a-zA-Z ]+\w*', ' ', search)
-            candidates = _getDb(db_name).search(search, limit=200)
-
-        # print(search, candidates)
+            search = re.sub(r"\w*[^a-zA-Z ]+\w*", " ", search)
+            candidates = _getDb(db_name).search(search, limit=limit)
 
         # Exact match
         acts = list(filter(act_filter, candidates))
 
     if single and len(acts) == 0:
-        raise Exception("No activity found in '%s' with name '%s' and location '%s'" % (db_name, name, loc))
+        any_name = name if name else in_name
+        raise Exception("No activity found in '%s' with name '%s' and location '%s'" % (db_name, any_name, loc))
     if single and len(acts) > 1:
-        raise Exception("Several activity found in '%s' with name '%s' and location '%s':\n%s" % (
-            db_name, name, loc, str(acts)))
+        raise Exception(
+            "Several activity found in '%s' with name '%s' and location '%s':\n%s"
+            % (db_name, name, loc, "\n".join(str(act) for act in acts))
+        )
     if len(acts) == 1:
         return acts[0]
     else:
         return acts
 
 
 def findBioAct(name=None, loc=None, **kwargs):
-    """Alias for findActivity(name, ... db_name=BIOSPHERE3_DB_NAME). See doc for #findActivity """
-    return findActivity(name=name, loc=loc, db_name=BIOSPHERE3_DB_NAME, **kwargs)
+    """Alias for findActivity(name, ... db_name=BIOSPHERE3_DB_NAME). See doc for #findActivity"""
+    return findActivity(name=name, loc=loc, db_name=_find_biosphere_db(), **kwargs)
 
 
 def findTechAct(name=None, loc=None, single=True, **kwargs):
     """
-        Search activities in technosphere. This function try to guess which database is your background database.
-        See also doc for #findActivity """
+    Search activities in technosphere. This function tries to guess which database is your background database.
+    If you have more than one background technosphere, you should use findActivity() and specify the **db_name** directly.
+    See also doc for #findActivity"""
     dbs = _listTechBackgroundDbs()
-    if len(dbs) > 1 :
-        raise Exception("There is more than one technosphere background DB (%s) please use findActivity(..., db_name=YOUR_DB)" % str(dbs))
+    if len(dbs) > 1:
+        raise Exception(
+            "There is more than one technosphere background DB (%s) please use findActivity(..., db_name=YOUR_DB)" % str(dbs)
+        )
 
     return findActivity(name=name, loc=loc, db_name=dbs[0], single=single, **kwargs)
 
 
-
 def _amountToFormula(amount: Union[float, str, Basic], currentAmount=None):
     """Transform amount in exchange to either simple amount or formula"""
     res = dict()
     if isinstance(amount, Basic):
-
-        if currentAmount != None:
+        if currentAmount is not None:
             amount = amount.subs(old_amount, currentAmount)
 
         # Check the expression does not reference undefined params
         all_symbols = list([key for param in _param_registry().values() for key, val in param.expandParams().items()])
         for symbol in amount.free_symbols:
             if not str(symbol) in all_symbols:
                 raise Exception("Symbol '%s' not found in params : %s" % (symbol, all_symbols))
 
-        res['formula'] = str(amount)
-        res['amount'] = 0
+        res["formula"] = str(amount)
+        res["amount"] = 0
     elif isinstance(amount, float) or isinstance(amount, int):
-        res['amount'] = amount
+        res["amount"] = amount
     else:
         raise Exception(
-            "Amount should be either a constant number or a Sympy expression (expression of ParamDef). Was : %s" % type(
-                amount))
+            "Amount should be either a constant number or a Sympy expression (expression of ParamDef). Was : %s" % type(amount)
+        )
     return res
 
 
 def _newAct(db_name, code):
-
-    if not _isForeground(db_name) :
-        error("WARNING: You are creating activity in background DB. You should only do it in your foreground / user DB : ", db_name)
+    if not _isForeground(db_name):
+        warn(
+            "WARNING: You are creating activity in background DB. You should only do it in your foreground / user DB : ",
+            db_name,
+        )
 
     db = _getDb(db_name)
     # Already present : delete it ?
     for act in db:
-        if act['code'] == code:
-            error("Activity '%s' was already in '%s'. Overwriting it" % (code, db_name))
+        if act["code"] == code:
+            warn("Activity '%s' was already in '%s'. Overwriting it" % (code, db_name))
             act.delete()
 
     return db.new_activity(code)
 
 
-def newActivity(db_name, name, unit,
-                exchanges: Dict[Activity, Union[float, str]] = dict(),
-                code=None,
-                **argv):
+def newActivity(
+    db_name,
+    name,
+    unit,
+    exchanges: Dict[Activity, Union[float, str]] = dict(),
+    amount=1,
+    code=None,
+    type="process",
+    **argv,
+):
     """Creates a new activity
 
     Parameters
     ----------
-    name : Name ofthe new activity
-    db_name : Destination DB : ACV DB by default
-    exchanges : Dict of activity => amount. If amount is a string, is it considered as a formula with parameters
-    argv : extra params passed as properties of the new activity
+    name :
+        Name of the new activity
+    db_name :
+        Destination DB : ACV DB by default
+    unit:
+        Unit of the process
+
+    code:
+        Unique code in the Db. Optional. If not provided, the name is used
+
+    exchanges :
+        Dict of activity => amount. See the doc for @addExchanges()
+
+    argv :
+        Any extra params passed as properties of the new activity
+
+    amount:
+        Production amount. 1 by default
     """
-    act = _newAct(db_name, code if code else name)
-    act['name'] = name
-    act['type'] = 'process'
-    act['unit'] = unit
+
+    code = code if code else name
+
+    act = _newAct(db_name, code)
+    act["name"] = name
+    act["type"] = type
+    act["unit"] = unit
     act.update(argv)
 
+    # Add single production exchange
+    if type == "process":
+        ex = act.new_exchange(
+            input=act.key,
+            name=act["name"],
+            unit=act["unit"],
+            type="production",
+            amount=amount,
+        )
+        ex.save()
+
+        act["reference product"] = act["name"]
+        act.save()
+
     # Add exchanges
     act.addExchanges(exchanges)
 
     return act
 
 
-def copyActivity(db_name, activity: ActivityExtended, code=None, withExchanges=True, **kwargs) -> ActivityExtended:
-    """Copy activity into a new DB"""
+def copyActivity(db_name, activity: ActivityExtended, code, withExchanges=True, **kwargs) -> ActivityExtended:
+    """Copy an activity and its exchanges into another database. You usually want to copy activities from your background to
+    your foreground DB to update them, keeping your background DB clean.
+
+    Parameters
+    ----------
+    db_name:
+        Name of the target database
+    activity:
+        Source activity
+    code:
+        Code of the target activity. Also used as its name
+
+
+    Returns
+    -------
+        The new activity. note that is is flagged with the custom property **inherited_from**, providing the full key of the
+        initial activity.
+    """
 
     res = _newAct(db_name, code)
 
     for key, value in activity.items():
-        if key not in ['database', 'code']:
+        if key not in ["database", "code"]:
             res[key] = value
     for k, v in kwargs.items():
         res._data[k] = v
-    res._data[u'code'] = code
-    res['name'] = code
-    res['type'] = 'process'
-    res['inherited_from'] = activity.key
+    res._data["code"] = code
+    res["name"] = code
+    res["type"] = "process"
+    res["inherited_from"] = activity.key
     res.save()
 
     if withExchanges:
         for exc in activity.exchanges():
             data = deepcopy(exc._data)
-            data['output'] = res.key
+            data["output"] = res.key
             # Change `input` for production exchanges
-            if exc['input'] == exc['output']:
-                data['input'] = res.key
+            if exc["input"] == exc["output"]:
+                data["input"] = res.key
             ExchangeDataset.create(**dict_as_exchangedataset(data))
 
     return res
 
+
 ActivityOrActivityAmount = Union[Activity, Tuple[Activity, float]]
+
+
 def newSwitchAct(dbname, name, paramDef: ParamDef, acts_dict: Dict[str, ActivityOrActivityAmount]):
-    """Create a new parametrized, virtual activity, made of a map of other activities, controlled by an enum parameter.
+    """Creates a new parametrized, virtual activity, made of a map of other activities, controlled by an enum parameter.
     This enables to implement a "Switch" with brightway parameters
     Internally, this will create a linear sum of other activities controlled by <param_name>_<enum_value> : 0 or 1
 
     By default, all activities have associated amount of 1.
     You can provide other amounts by providing a tuple of (activity, amount).
 
     Parameters
     ----------
-    dbname: name of the target DB
-    name: Name of the new activity
-    paramDef : parameter definition of type enum
-    acts_dict : dict of "enumValue" => activity or "enumValue" => (activity, amount)
+    dbname:
+        name of the target DB
+    name:
+        Name of the new activity
+    paramDef :
+        parameter definition of type enum
+    acts_dict :
+        dict of "enumValue" => activity or "enumValue" => (activity, amount)
 
     Examples
     --------
 
     >>> newSwitchAct(MYDB, "switchAct", switchParam, {
     >>>    "val1" : act1 # Amount is 1
     >>>    "val2" : (act2, 0.4) # Different amount
     >>>    "val3" : (act3, b + 6) # Amount with formula
     >>> }
     """
 
     # Transform map of enum values to corresponding formulas <param_name>_<enum_value>
-    exch = defaultdict(lambda : 0)
+    exch = defaultdict(lambda: 0)
 
     # Forward last unit as unit of the switch
-    unit= None
-    for key, act in acts_dict.items() :
+    unit = None
+    for key, act in acts_dict.items():
         amount = 1
-        if type(act) == list or type(act) == tuple :
+        if isinstance(act, (list, tuple)):
             act, amount = act
         exch[act] += amount * paramDef.symbol(key)
         unit = act["unit"]
 
-    res = newActivity(
-        dbname,
-        name,
-        unit=unit,
-        exchanges=exch)
+    res = newActivity(dbname, name, unit=unit, exchanges=exch)
 
     return res
 
 
-def printAct(*args, impact=None, **params):
+def _actDesc(act: ActivityExtended):
+    """Generate pretty name for activity + basic information"""
+    name = _actName(act)
+    amount = act.getOutputAmount()
+
+    return "%s (%f %s)" % (name, amount, act["unit"])
+
+
+def printAct(*activities, **params):
     """
     Print activities and their exchanges.
     If parameter values are provided, formulas will be evaluated accordingly.
-    If impact is provided it will be computed.
+
+    Parameters
+    ----------
+    activities:
+        One or two activities. If two activities are provided, differences are highlighted.
+
+    params:
+        If provided, the formulas are evaluated accordingly and the result amount is shown instead of formula
+
+    Returns
+    -------
+        A Dataframe is returned, containing all information, exchange by exchange
     """
     tables = []
     names = []
 
-    activities = args
-
-
     for act in activities:
-        with DbContext(act.key[0]) :
+        with DbContext(act.key[0]):
             inputs_by_ex_name = dict()
-            df = pd.DataFrame(index=['input', 'amount', 'unit'])
+            df = pd.DataFrame(index=["input", "amount", "unit"])
             data = dict()
-            for (i, exc) in enumerate(act.exchanges()):
-
+            for i, exc in enumerate(act.exchanges()):
                 # Don't show production
-                if _isOutputExch(exc) :
+                if _isOutputExch(exc):
                     continue
 
                 input = bw.get_activity(exc.input.key)
                 amount = _getAmountOrFormula(exc)
 
                 # Params provided ? Evaluate formulas
                 if len(params) > 0 and isinstance(amount, Basic):
-                    new_params = [(name, value) for name, value in _completeParamValues(params).items()]
+                    new_params = [(name, value) for name, value in _complete_and_expand_params(params).items()]
                     amount = amount.subs(new_params)
 
                 ex_name = _exch_name(exc)
-                #if 'location' in input and input['location'] != "GLO":
+                # if 'location' in input and input['location'] != "GLO":
                 #    name += "#%s" % input['location']
-                #if exc.input.key[0] not in [BIOSPHERE3_DB_NAME, ECOINVENT_DB_NAME()]:
+                # if exc.input.key[0] not in [BIOSPHERE3_DB_NAME, ECOINVENT_DB_NAME()]:
                 #    name += " {user-db}"
 
                 # Unique name : some exchanges may havve same names
                 _name = ex_name
                 i = 1
                 while ex_name in data:
                     ex_name = "%s#%d" % (_name, i)
@@ -679,15 +637,14 @@
                 if _isForeground(input.key[0]):
                     input_name += "{FG}"
 
                 data[ex_name] = [input_name, amount, exc.unit]
 
             # Provide impact calculation if impact provided
 
-
             for key, values in data.items():
                 df[key] = values
 
             tables.append(df.T)
             names.append(_actDesc(act))
 
     full = pd.concat(tables, axis=1, keys=names, sort=True)
@@ -699,85 +656,24 @@
         iamount2 = full.columns.get_loc((names[1], "amount"))
         iact1 = full.columns.get_loc((names[0], "input"))
         iact2 = full.columns.get_loc((names[1], "input"))
 
         def same_amount(row):
             res = [""] * len(row)
 
-            if row[iamount1] != row[iamount2]:
+            if row.iloc[iamount1] != row.iloc[iamount2]:
                 res[iamount1] = yellow
                 res[iamount2] = yellow
-            if row[iact1] != row[iact2]:
+            if row.iloc[iact1] != row.iloc[iact2]:
                 res[iact1] = yellow
                 res[iact2] = yellow
             return res
 
         full = full.style.apply(same_amount, axis=1)
 
-    display(full)
-
-
-def newInterpolatedAct(dbname: str, name: str, act1: ActivityExtended, act2: ActivityExtended, x1, x2, x, alpha1=1,
-                       alpha2=1, **kwargs):
-    """Creates a new activity made of interpolation of two similar activities.
-    For each exchange :
-    amount = alpha1 * a1 + (x - X1) * (alpha2 * a2 - alpha1 * a1) / (x2 - x1)
-
-    Parameters
-    ----------
-    name : Name of new activity
-    act1 : Activity 1
-    act2 : Activity 2
-    x1 : X for act1
-    x2 : X for act 2
-    x : Should be a parameter symbol
-    alpha1 : Ratio for act1 (Default value = 1)
-    alpha2 : Ratio for act2 (Default value = 1)
-    kwargs : Any other param will be added as attributes of new activity
-    """
-    res = copyActivity(dbname, act1, name, withExchanges=False, **kwargs)
-
-    exch1_by_input = dict({exch['input']: exch for exch in act1.exchangesNp()})
-    exch2_by_input = dict({exch['input']: exch for exch in act2.exchangesNp()})
-
-    inputs = set(chain(exch1_by_input.keys(), exch2_by_input.keys()))
-
-    for input in inputs:
+    return full
 
-        exch1 = exch1_by_input.get(input)
-        exch2 = exch2_by_input.get(input)
-        exch = exch1 if exch1 else exch2
 
-        amount1 = exch1['amount'] if exch1 else 0
-        amount2 = exch2['amount'] if exch2 else 0
-
-        if exch1 and exch2 and exch1['name'] != exch2['name']:
-            raise Exception("Input %s refer two different names : %s, %s" % (input, exch1['name'], exch2['name']))
-
-        amount = interpolate(x, x1, x2, amount1 * alpha1, amount2 * alpha2)
-        act = getActByCode(*input)
-        res.addExchanges({act: dict(amount=amount, name=exch['name'])})
-    return res
-
-
-
-def findMethods(search=None, mainCat=None) :
-
-    """
-    Find impact method. Search in all methods against a list of match strings.
-    Each parameter can be either an exact match match, or case insenstive search, if suffixed by '*'
-
-    Parameters
-    ----------
-    search : String to search
-    mainCat : if specified, limits the research for method[0] == mainCat.
-    """
-    res = []
-    search = search.lower()
-    for method in bw.methods:
-        text = str(method).lower()
-        match  = search in text
-        if mainCat :
-            match = match and (mainCat == method[0])
-        if match :
-            res.append(method)
-    return res
+# Backport new methods to vanilla Activity class in order to benefit from it for all existing instances
+for name, item in ActivityExtended.__dict__.items():
+    if isinstance(item, FunctionType):
+        setattr(Activity, name, item)
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/io.py` & `lca_algebraic-1.1/lca_algebraic/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from os.path import basename, dirname
-
-import bw2data
+import brightway2 as bw
 from bw2data.parameters import DatabaseParameter, ProjectParameter
 from bw2io import BW2Package
-import brightway2 as bw
 
-from lca_algebraic import loadParams, error
-from lca_algebraic.params import _listParams
+from lca_algebraic.log import warn
+from lca_algebraic.params import _listParams, loadParams
 
+__all__ = ["export_db", "import_db"]
 
-__all__ = ['export_db', 'import_db']
 
-def param_data(param) :
+def _param_data(param):
     """Return param data except id"""
-    res =  {key:val for key, val in param.__data__.items() if key != "id"}
+    res = {key: val for key, val in param.__data__.items() if key != "id"}
     data = res.pop("data")
     res.update(data)
 
     return res
 
-def export_db(db_name, filename) :
-    """Export Db and linked parameters"""
+
+def export_db(db_name, filename):
+    """This function exports a database to the **BW2Package** format, including the definition of parameters"""
     db = bw.Database(db_name)
     db_params = DatabaseParameter.select().where(DatabaseParameter.database == db_name)
 
     # Export Db params
-    db.metadata["database_parameters"] = [param_data(param) for param in db_params]
+    db.metadata["database_parameters"] = [_param_data(param) for param in db_params]
 
     # List of all project params used in this dataset
     used_project_params = list(param.name for param in _listParams(db_name) if param.dbname is None)
 
-    if len(used_project_params) > 0 :
-        error('Warning : this DB uses project parameters that are exported as well and might override project params at import time : ', used_project_params)
+    if len(used_project_params) > 0:
+        warn(
+            "Warning : this DB uses project parameters that are exported as well "
+            "and might override project params at import time : ",
+            used_project_params,
+        )
 
-        proj_params = list(ProjectParameter.get(ProjectParameter.name==name) for name in used_project_params)
+        proj_params = list(ProjectParameter.get(ProjectParameter.name == name) for name in used_project_params)
 
-        db.metadata["project_parameters"] = [param_data(param) for param in proj_params]
+        db.metadata["project_parameters"] = [_param_data(param) for param in proj_params]
 
     BW2Package._write_file(filename, [BW2Package._prepare_obj(db, False)])
 
 
-
-def import_db(filename) :
-    """Export Db and linked parameters"""
+def import_db(filename):
+    """Import Db from BW2Package with linked parameters (as produced by **export_db**)"""
 
     db = BW2Package.import_file(filename)[0]
-    if "database_parameters" in db.metadata :
+    if "database_parameters" in db.metadata:
         params = db.metadata["database_parameters"]
         bw.parameters.new_database_parameters(params, db.name)
 
     if "project_parameters" in db.metadata:
         params = db.metadata["project_parameters"]
         bw.parameters.new_project_parameters(params)
 
     # Reload the parameters
     loadParams()
 
     return db
-
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/lca.py` & `lca_algebraic-1.1/lca_algebraic/lca.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,589 +1,850 @@
 import concurrent.futures
+import re
 from collections import OrderedDict
-from typing import Dict, List
+from dataclasses import dataclass
+from types import FunctionType
+from typing import Dict, List, Union
+
+import brightway2 as bw
+import numpy as np
+import pandas as pd
+from peewee import DoesNotExist
+from sympy import Basic, Symbol, lambdify, parse_expr, simplify, symbols
+from sympy.printing.numpy import NumPyPrinter
+
+from . import ValueOrExpression
+from .activity import ActivityExtended, DbContext, newActivity, with_db_context
+from .axis_dict import AxisDict
+from .base_utils import TabbedDataframe, _actName, _getDb, _user_functions
+from .cache import ExprCache, LCIACache
+from .database import BIOSPHERE_PREFIX, _isForeground
+from .log import logger, warn
+from .methods import method_name, method_unit
+from .params import (
+    FixedParamMode,
+    _complete_params,
+    _compute_param_length,
+    _expand_param_names,
+    _expand_params,
+    _expanded_names_to_names,
+    _fixed_params,
+    _getAmountOrFormula,
+    _param_registry,
+    _toSymbolDict,
+    all_params,
+    freezeParams,
+)
 
-from sympy import lambdify, simplify
-
-from .base_utils import _actName, error, _getDb, _method_unit
-from .base_utils import _getAmountOrFormula
-from .helpers import *
-from .helpers import _actDesc, _isForeground
-from .params import _param_registry, _completeParamValues, _fixed_params, _expanded_names_to_names, _expand_param_names
 
+def register_user_function(sym, func):
+    """Register a custom function with is python implementation
+    Parameters
+    ----------
+    sym : the sympy function expression
+    func : the implementation of the function
 
-def _impact_labels():
-    """Dictionnary of custom impact names
-        Dict of "method tuple" => string
+    Examples
+    --------
+    >>> def func_add(*args):
+            returm sum(*args)
+    >>>
+    >>> func_add_sym = register_user_function(sympy.Function('func_add', real=True, imaginary=False), func_add)
+    >>> e = sympy.Symbol('a') * func_add_sym(sympy.Symbol('b'), sympy.Symbol('c'))
+    >>> sympy.srepr(e)
+    "Mul(Symbol('a'), Function('func_add')(Symbol('b'), Symbol('c')))"
+    """
+    global _user_functions
+    _user_functions[sym.name] = (sym, func)
+    return sym
+
+
+def user_function(sym):
+    """Function decorator to register user function
+
+    Usage
+    -----
+    >>> @user_function(sympy.Function('func_add', real=True, imaginary=False))
+    >>> def func_add(*args):
+            returm sum(*args)
+    >>>
+    >>> e = sympy.Symbol('a') * func_add(sympy.Symbol('b'), sympy.Symbol('c'))
+    >>> sympy.srepr(e)
+    "Mul(Symbol('a'), Function('func_add')(Symbol('b'), Symbol('c')))"
     """
-    # Prevent reset upon auto reload in jupyter notebook
-    if not '_impact_labels' in builtins.__dict__:
-        builtins._impact_labels = dict()
+    return lambda func: register_user_function(sym, func)
 
-    return builtins._impact_labels
-
-def set_custom_impact_labels(impact_labels:Dict) :
-    """ Global function to override name of impact method in graphs """
-    _impact_labels().update(impact_labels)
 
 def _multiLCA(activities, methods):
     """Simple wrapper around brightway API"""
-    bw.calculation_setups['process'] = {'inv': activities, 'ia': methods}
-    lca = bw.MultiLCA('process')
+    bw.calculation_setups["process"] = {"inv": activities, "ia": methods}
+    lca = bw.MultiLCA("process")
     cols = [_actName(act) for act_amount in activities for act, amount in act_amount.items()]
     return pd.DataFrame(lca.results.T, index=[method_name(method) for method in methods], columns=cols)
 
 
 def multiLCA(models, methods, **params):
-    """Compute LCA for a single activity and a set of methods, after settings the parameters and updating exchange amounts.
+    """Compute LCA for a single activity and a set of methods,
+    after settings the parameters and updating exchange amounts.
     This function does not use algebraic factorization and just calls the Brightway2 vanilla code.
 
     Parameters
     ----------
     model : Single activity (root model) or list of activities
     methods : Impact methods to consider
     params : Other parameters of the model
     """
 
     if not isinstance(models, list):
         models = [models]
 
     # Freeze params
     dbs = set(model[0] for model in models)
-    for db in dbs :
-        if _isForeground(db) :
+    for db in dbs:
+        if _isForeground(db):
             freezeParams(db, **params)
 
     activities = [{act: 1} for act in models]
     return _multiLCA(activities, methods).transpose()
 
 
+""" Compute LCA and return (act, method) => value """
 
-# Cache of (act, method) => values
-_BG_IMPACTS_CACHE = dict()
 
-def _clearLCACache() :
-    _BG_IMPACTS_CACHE.clear()
+def _multiLCAWithCache(acts, methods):
+    with LCIACache() as cache:
+        # List activities with at least one missing value
+        remaining_acts = list(act for act in acts if any(method for method in methods if (act, method) not in cache.data))
 
-""" Compute LCA and return (act, method) => value """
-def _multiLCAWithCache(acts, methods) :
+        if len(remaining_acts) > 0:
+            lca = _multiLCA([{act: 1} for act in remaining_acts], methods)
 
-    # List activities with at least one missing value
-    remaining_acts = list(act for act in acts if any(method for method in methods if (act, method) not in _BG_IMPACTS_CACHE))
+            # Set output from dataframe
+            for imethod, method in enumerate(methods):
+                for iact, act in enumerate(remaining_acts):
+                    cache.data[(act, method)] = lca.iloc[imethod, iact]
 
-    if (len(remaining_acts) > 0) :
-        lca = _multiLCA(
-            [{act: 1} for act in remaining_acts],
-            methods)
+        # Return a copy of the cache for selected impacts and activities
+        return {(act, method): cache.data[(act, method)] for act in acts for method in methods}
 
-        # Set output from dataframe
-        for imethod, method in enumerate(methods) :
-            for iact, act in enumerate(remaining_acts) :
-                _BG_IMPACTS_CACHE[(act, method)] = lca.iloc[imethod, iact]
 
-    return _BG_IMPACTS_CACHE
+def _replace_symbols_with_params_in_exp(expr: Basic):
+    """After unpickling, the Symbols in the expression with same named are not the same object than Parameters.
+    This is problematic for xreplace wich relies on it :
+    Here we replace them.
+    """
+
+    if not isinstance(expr, Basic):
+        return expr
+
+    all_params = _param_registry().as_dict()
+    subs = {symb: all_params[symb.name] for symb in expr.free_symbols if isinstance(symb, Symbol) and symb.name in all_params}
 
+    logger.debug("Replace: %s", subs)
 
-def _modelToExpr(
-        model: ActivityExtended,
-        methods,
-        extract_activities=None) :
-    '''
+    expr = expr.xreplace(subs)
+    return expr
+
+
+def _modelToExpr(model: ActivityExtended, methods, alpha=1, axis=None):
+    """
     Compute expressions corresponding to a model for each impact, replacing activities by the value of its impact
 
     Return
     ------
     <list of expressions (one per impact)>, <list of required param names>
 
-    '''
-    # print("computing model to expression for %s" % model)
-    expr, actBySymbolName = actToExpression(
-        model,
-        extract_activities=extract_activities)
-
-    # Required params
-    free_names = set([str(symb) for symb in expr.free_symbols])
-    act_names = set([str(symb) for symb in actBySymbolName.keys()])
-    expected_names = free_names - act_names
+    """
+
+    # Try to load from cache
+    with ExprCache() as cache:
+        key = (model, axis)
+
+        if key not in cache.data:
+            logger.debug(f"{model} was not in exrepssion cache, computing...")
+
+            expr, actBySymbolName = actToExpression(model, axis=axis)
+
+            cache.data[key] = (expr, actBySymbolName)
+        else:
+            logger.debug(f"{model} found in exrepssion cache")
+
+        expr, actBySymbolName = cache.data[key]
 
-    # If we expect an enum param name, we also expect the other ones : enumparam_val1 => enumparam_val1, enumparam_val2, ...
-    expected_names = _expand_param_names(_expanded_names_to_names(expected_names))
+    logger.debug("Alpha passed %s", alpha)
+
+    # logger.debug("Raw expression for %s/%s : '%s'", model, str(methods), expr)
+    # logger.debug("Act by symbol : %s", actBySymbolName)
+    # if logger.isEnabledFor("DEBUG") :
+    # logger.debug(f"Length of expression : {len(str(expr))}")
+
+    expr = expr * alpha
 
     # Create dummy reference to biosphere
     # We cannot run LCA to biosphere activities
     # We create a technosphere activity mapping exactly to 1 biosphere item
     pureTechActBySymbol = OrderedDict()
-    for name, act in actBySymbolName.items():
-        pureTechActBySymbol[name] = _createTechProxyForBio(act, model.key[0])
+    for act_name, act in actBySymbolName.items():
+        pureTechActBySymbol[act_name] = _createTechProxyForBio(act, model.key[0])
 
     # Compute LCA for background activities
     lcas = _multiLCAWithCache(pureTechActBySymbol.values(), methods)
 
     # For each method, compute an algebric expression with activities replaced by their values
     exprs = []
     for method in methods:
         # Replace activities by their value in expression for this method
         sub = dict({symbol: lcas[(act, method)] for symbol, act in pureTechActBySymbol.items()})
-        exprs.append(expr.xreplace(sub))
 
-    return exprs, expected_names
+        expr_curr = expr.xreplace(sub)
+
+        # Ensure symbols are params
+        expr_curr = _replace_symbols_with_params_in_exp(expr_curr)
+
+        exprs.append(expr_curr)
+
+    return exprs
 
 
-def _filter_param_values(params, expanded_param_names) :
-    return {key : val for key, val in params.items() if key in expanded_param_names}
+def _filter_param_values(params, expanded_param_names):
+    return {key: val for key, val in params.items() if key in expanded_param_names}
 
-class LambdaWithParamNames :
+
+def _free_symbols(expr: Basic):
+    if isinstance(expr, Basic):
+        return set([str(symb) for symb in expr.free_symbols])
+    else:
+        # Static value
+        return set()
+
+
+def _lambdify(expr: Basic, expanded_params):
+    """Lambdify, handling manually the case of SymDict (for impacts by axis)"""
+
+    printer = NumPyPrinter(
+        {"fully_qualified_modules": False, "inline": True, "allow_unknown_functions": True, "user_functions": dict()}
+    )
+
+    modules = [{x[0].name: x[1] for x in _user_functions.values()}, "numpy"]
+
+    if isinstance(expr, Basic):
+        lambd = lambdify(expanded_params, expr, modules, printer=printer, cse=LambdaWithParamNames._use_sympy_cse)
+
+        def func(*arg, **kwargs):
+            res = lambd(*arg, **kwargs)
+            if isinstance(res, dict):
+                # Transform key symbols into Str
+                return {str(k): v for k, v in res.items()}
+            else:
+                return res
+
+        return func
+
+    else:
+        # Not an expression : return static func
+        def static_func(*args, **kargs):
+            return expr
+
+        return static_func
+
+
+def compute_param_formulas(param_values: Dict, required_params: List[str]):
+    # Compute the values params computed from formulas (and not specified in input)
+    pass
+
+
+@dataclass
+class ValueContext:
+    """Represents a result value, with all parameters values used in context"""
+
+    value: float
+    context: Dict[str, float]
+
+
+class LambdaWithParamNames:
     """
-    This class represents a compiled (lambdified) expression together with the list of requirement parameters and the source expression
+    This class represents a compiled (lambdified) expression together
+    with the list of requirement parameters and the source expression
     """
+
+    _use_sympy_cse = False
+
     def __init__(self, exprOrDict, expanded_params=None, params=None, sobols=None):
-        """ Computes a lamdda function from expression and list of expected parameters.
+        """Computes a lamdda function from expression and list of expected parameters.
         you can provide either the list pf expanded parameters (full vars for enums) for the 'user' param names
         """
 
-        if isinstance(exprOrDict, dict) :
+        if isinstance(exprOrDict, dict):
             # Come from JSON serialization
             obj = exprOrDict
-            # Parse
-            self.params = obj["params"]
+            # LIst of required params for this lambda
+            self.params: List[str] = obj["params"]
 
             # Full names
             self.expanded_params = _expand_param_names(self.params)
-            self.expr = parse_expr(obj["expr"])
-            self.lambd = lambdify(self.expanded_params, self.expr, 'numpy')
+            local_dict = {x[0].name: x[0] for x in _user_functions.values()}
+            self.expr = parse_expr(obj["expr"], local_dict=local_dict)
+            self.lambd = _lambdify(self.expr, self.expanded_params)
             self.sobols = obj["sobols"]
 
-        else :
+        else:
             self.expr = exprOrDict
             self.params = params
 
-            if expanded_params is None :
+            if expanded_params is None:
+                if params is None:
+                    expanded_params = _free_symbols(exprOrDict)
+                    params = _expanded_names_to_names(expanded_params)
+                    self.params = params
+
+                # We expand again the parameters
+                # If we expect an enum param name, we also expect the other ones :
+                # enumparam_val1 => enumparam_val1, enumparam_val2, ...
                 expanded_params = _expand_param_names(params)
-            if self.params is None :
+
+            elif self.params is None:
                 self.params = _expanded_names_to_names(expanded_params)
 
-            self.lambd = lambdify(expanded_params, exprOrDict, 'numpy')
+            self.lambd = _lambdify(exprOrDict, expanded_params)
             self.expanded_params = expanded_params
             self.sobols = sobols
 
-    def complete_params(self, params):
+    @property
+    def has_axis(self):
+        return isinstance(self.expr, AxisDict)
 
-        param_length = _compute_param_length(params)
+    @property
+    def axis_keys(self):
+        if self.has_axis:
+            return self.expr.str_keys()
+        else:
+            return None
 
-        # Check and expand enum params, add default values
-        res = _completeParamValues(params, self.params)
+    def compute(self, **params) -> ValueContext:
+        """Compute result value based of input parameters"""
 
-        # Expand single params and transform them to np.array
-        for key in res.keys():
-            val = res[key]
-            if not isinstance(val, list):
-                val = list([val] * param_length)
-            res[key] = np.array(val, float)
-        return res
+        # Add default or computed values
+        completed_params = _complete_params(params, self.params)
+
+        # Expand enums
+        expanded_params = _expand_params(completed_params)
+
+        # Remove parameters that are not required
+        expanded_params = _filter_param_values(expanded_params, self.expanded_params)
+
+        value = self.lambd(**expanded_params)
+
+        return ValueContext(value=value, context=completed_params)
 
-    def compute(self, **params):
-        """Compute result value based of input parameters """
-        # Filter on required parameters
-        params = _filter_param_values(params, self.expanded_params)
-        return self.lambd(**params)
-
-    def serialize(self) :
-        return dict(
-            params=self.params,
-            expr=str(self.expr),
-            sobols=self.sobols)
+    def serialize(self):
+        expr = str(self.expr)
+        return dict(params=self.params, expr=expr, sobols=self.sobols)
+
+    @staticmethod
+    def use_sympy_cse(b=True):
+        LambdaWithParamNames._use_sympy_cse = b
 
     def __repr__(self):
         return repr(self.expr)
 
     def _repr_latex_(self):
         return self.expr._repr_latex_()
 
-def _preMultiLCAAlgebric(model: ActivityExtended, methods, extract_activities:List[Activity]=None):
-    '''
-        This method transforms an activity into a set of functions ready to compute LCA very fast on a set on methods.
-        You may use is and pass the result to postMultiLCAAlgebric for fast computation on a model that does not change.
-
-        This method is used by multiLCAAlgebric
-    '''
-    with DbContext(model) :
-        exprs, expected_names = _modelToExpr(model, methods, extract_activities=extract_activities)
+
+def lambdify_expr(expr):
+    return LambdaWithParamNames(expr, params=[param.name for param in _param_registry().values()])
+
+
+def _preMultiLCAAlgebric(model: ActivityExtended, methods, alpha=1, axis=None):
+    """
+    This method transforms an activity into a set of functions ready to compute LCA very fast on a set on methods.
+    You may use is and pass the result to postMultiLCAAlgebric for fast computation on a model that does not change.
+
+    This method is used by multiLCAAlgebric
+    """
+    with DbContext(model):
+        exprs = _modelToExpr(model, methods, alpha=alpha, axis=axis)
 
         # Lambdify (compile) expressions
-        return [LambdaWithParamNames(expr, expected_names) for expr in exprs]
+        return [LambdaWithParamNames(expr) for expr in exprs]
+
+
+def _slugify(str):
+    return re.sub("[^0-9a-zA-Z]+", "_", str)
+
+
+@dataclass
+class ResultsWithParams:
+    """Holds bith the result with context parameters"""
+
+    dataframe: pd.DataFrame
+    params: Dict
 
 
-def method_name(method):
-    """Return name of method, taking into account custom label set via set_custom_impact_labels(...) """
-    if method in _impact_labels() :
-        return _impact_labels()[method]
-    return method[1] + " - " + method[2]
-
-def _slugify(str) :
-    return re.sub('[^0-9a-zA-Z]+', '_', str)
-
-def _compute_param_length(params) :
-    # Check length of parameter values
-    param_length = 1
-    for key, val in params.items():
-        if isinstance(val, list):
-            if param_length == 1:
-                param_length = len(val)
-            elif param_length != len(val):
-                raise Exception("Parameters should be a single value or a list of same number of values")
-    return param_length
-
-def _postMultiLCAAlgebric(methods, lambdas, alpha=1, **params):
-    '''
-        Compute LCA for a given set of parameters and pre-compiled lambda functions.
-        This function is used by **multiLCAAlgebric**
-
-        Parameters
-        ----------
-        methodAndLambdas : Output of preMultiLCAAlgebric
-        **params : Parameters of the model
-    '''
+def _postMultiLCAAlgebric(methods, lambdas: List[LambdaWithParamNames], with_params=False, **params):
+    """
+    Compute LCA for a given set of parameters and pre-compiled lambda functions.
+    This function is used by **multiLCAAlgebric**
+
+    Parameters
+    ----------
+    methodAndLambdas : Output of preMultiLCAAlgebric
+    **params : Parameters of the model
+    """
 
     param_length = _compute_param_length(params)
 
+    # lambda are SymDict ?
+    # If use them as number of params
+    if lambdas[0].has_axis:
+        if param_length > 1:
+            raise Exception("Multi params cannot be used together with 'axis'")
+        param_length = len(lambdas[0].axis_keys)
+
     # Init output
     res = np.zeros((len(methods), param_length), float)
 
+    # All params
+    context_params = dict()
+
     # Compute result on whole vectors of parameter samples at a time : lambdas use numpy for vector computation
-    def process(args) :
+    def process(args):
+        nonlocal context_params
+
         imethod = args[0]
-        lambd_with_params : LambdaWithParamNames = args[1]
+        lambd: LambdaWithParamNames = args[1]
+
+        value_context = lambd.compute(**params)
+
+        # Update the param values used
+        context_params.update(value_context.context)
+
+        value = value_context.value
 
-        completed_params = lambd_with_params.complete_params(params)
+        # Expand axis values as a list, to fit into the result numpy array
+        if isinstance(value, dict):
+            # Ensure the values are in the same order as the value
+            value = list(float(value[axis]) if axis in value else 0.0 for axis in lambd.axis_keys)
 
-        value = alpha * lambd_with_params.compute(**completed_params)
         return (imethod, value)
 
     # Use multithread for that
     with concurrent.futures.ThreadPoolExecutor() as exec:
         for imethod, value in exec.map(process, enumerate(lambdas)):
             res[imethod, :] = value
 
-    return pd.DataFrame(res, index=[method_name(method) + "[%s]" % _method_unit(method) for method in methods]).transpose()
+    result = pd.DataFrame(
+        res,
+        index=[method_name(method) + "[%s]" % method_unit(method) for method in methods],
+    ).transpose()
+
+    if with_params:
+        return ResultsWithParams(dataframe=result, params=context_params)
+    else:
+        return result
 
 
 # Add default values for issing parameters or warn about extra params
-def _filter_params(params, expected_names, model) :
+def _filter_params(params, expected_names, model):
     res = params.copy()
 
     expected_params_names = _expanded_names_to_names(expected_names)
     for expected_name in expected_params_names:
         if expected_name not in params:
             default = _param_registry()[expected_name].default
             res[expected_name] = default
-            error("Missing parameter %s, replaced by default value %s" % (expected_name, default))
+            warn("Missing parameter %s, replaced by default value %s" % (expected_name, default))
 
     for key, value in params.items():
-        if not key in expected_params_names:
+        if key not in expected_params_names:
             del res[key]
-            if model :
-                error("Param %s not required for model %s" % (key, model))
+            if model:
+                warn("Param %s not required for model %s" % (key, model))
     return res
 
-def multiLCAAlgebric(models, methods, extract_activities:List[Activity]=None, **params):
+
+def compute_value(formula, **params):
+    """Compute actual value for a given formula, with possible parameters (or default ones)"""
+    if isinstance(formula, float) or isinstance(formula, int):
+        return formula
+
+    lambd = LambdaWithParamNames(formula)
+
+    value_context = lambd.compute(**params)
+
+    return value_context.value
+
+
+def multiLCAAlgebric(*args, **kwargs):
+    """deprecated. `compute_impacts()` instead"""
+    logger.warn("multiLCAAlgebric is deprecated, use compute_impacts instead")
+    return compute_impacts(*args, **kwargs)
+
+
+def _params_dataframe(param_values: Dict[str, float]):
+    """Create a DataFrame, ordered by group, showing param values"""
+    params_by_name = all_params()
+
+    records = []
+
+    plen = _compute_param_length(param_values)
+
+    for param_name, value in param_values.items():
+        param = params_by_name[param_name]
+        record = {
+            "group": param.group if param.group is not None else "",
+            "name": param.name,
+            "min": param.min,
+            "max": param.max,
+            "default": param.default,
+        }
+
+        if plen == 1:
+            record["value"] = value
+        else:
+            if isinstance(value, (list, np.ndarray)):
+                record.update({f"value_{i}": value for i, value in enumerate(value, 1)})
+            else:
+                # Repeat single value
+                record.update({f"value_{i}": value for i in range(1, plen + 1)})
+
+        records.append(record)
+
+    df = pd.DataFrame.from_records(records).set_index(["group", "name"]).sort_index()
+
+    return df
+
+
+SingleOrMultipleFloat = Union[float, List[float], np.ndarray]
+
+
+def compute_impacts(
+    models,
+    methods,
+    axis=None,
+    functional_unit: ValueOrExpression = 1,
+    return_params: bool = False,
+    description: str = None,
+    **params: Dict[str, SingleOrMultipleFloat],
+):
     """
-    Main parametric LCIA method : Computes LCA by expressing the foreground model as symbolic expression of background activities and parameters.
+    Main parametric LCIA method :
+    Computes LCA by expressing the foreground model as symbolic expression of background activities and parameters.
     Then, compute 'static' inventory of the referenced background activities.
-    This enables a very fast recomputation of LCA with different parameters, useful for stochastic evaluation of parametrized model
+    This enables a very fast recomputation of LCA with different parameters, \
+    useful for stochastic evaluation of parametrized model
 
     Parameters
     ----------
     models :
         Single model or
         List of model or
         List of (model, alpha)
         or Dict of model:amount
         In case of several models, you cannot use list of parameters
-    methods : List of methods / impacts to consider
-    extract_activities : Optionnal : list of foregound or background activities. If provided, the result only integrate their contribution
-    params : You should provide named values of all the parameters declared in the model. \
-             Values can be single value or list of samples, all of the same size
+
+    methods :
+        List of methods / impacts to consider
+
+    axis:
+        Designates the name of a custom attribute of foreground activities.
+        You may set this attribute using the method `myActivity.updateMeta(your_custom_attr="some_value")`
+
+        The impacts will be ventilated by this attribute.
+        This is useful to get impact by phase or sub-modules.
+
+    params:
+        Any other argument passed to this function is considered as a value of a parameter of the model :
+        Values can be either single float values, list or ndarray of values.
+        In the later case, all parameters should have the same number of values.
+        Paremeters that are not provided will have their default value set.
+
+    functional_unit:
+        Quantity (static or Sympy formula) by which to divide impacts. Optional, 1 by default.
+
+    return_params:
+        If true, also returns the value of all parameters in as tabbed DataFrame
+
+    description:
+        Optional description/metadata to be added in output when using "return params" Dataframe
+
+    Returns
+    -------
+    A dataframe with the results. If *return_params* is true, it returns `TabbedDataframe`,
+    including all parameters values, that can be saved as a multi sheet excel file.
+
+    Examples
+    --------
+    >>> compute_impacts(
+    >>>    mainAct1, # The root activity of the foreground model
+    >>>    [climate_change], # climate_change is the key (tuple) of the impact method
+    >>>    functional_unit=energy_expression, # energy expression is a Sympy expression computing the energy in kWh
+    >>>    axis="phase", # Split results by phase
+    >>>    return_params=True, # Return all parameter values
+    >>>
+    >>>    # Parameter values
+    >>>    p1=2.0,
+    >>>    p2=3.0)
+
+
     """
     dfs = dict()
 
     if isinstance(models, list):
-        def to_tuple(item) :
-            if isinstance(item, tuple) :
+
+        def to_tuple(item):
+            if isinstance(item, tuple):
                 return item
             else:
                 return (item, 1)
+
         models = dict(to_tuple(item) for item in models)
     elif not isinstance(models, dict):
-        models = {models:1}
+        models = {models: 1}
 
-    for model, alpha in models.items():
+    # Gather all param values (even default and computed)
+    params_all = dict()
 
+    for model, alpha in models.items():
         if type(model) is tuple:
             model, alpha = model
 
+        alpha = float(alpha)
+
         dbname = model.key[0]
         with DbContext(dbname):
-
             # Check no params are passed for FixedParams
             for key in params:
-                if key in _fixed_params() :
-                    error("Param '%s' is marked as FIXED, but passed in parameters : ignored" % key)
+                if key in _fixed_params():
+                    warn("Param '%s' is marked as FIXED, but passed in parameters : ignored" % key)
 
+            if functional_unit != 1:
+                alpha = alpha / functional_unit
 
-            lambdas = _preMultiLCAAlgebric(model, methods, extract_activities=extract_activities)
+            lambdas = _preMultiLCAAlgebric(model, methods, alpha=alpha, axis=axis)
 
-            df = _postMultiLCAAlgebric(methods, lambdas, alpha=alpha, **params)
+            res = _postMultiLCAAlgebric(methods, lambdas, with_params=return_params, **params)
+            if return_params:
+                df = res.dataframe
+                params_all.update(res.params)
+            else:
+                df = res
 
             model_name = _actName(model)
-            while model_name in dfs :
+            while model_name in dfs:
                 model_name += "'"
 
-            # Single params ? => give the single row the name of the model activity
-            if df.shape[0] == 1:
+            # param with several values
+            list_params = {k: vals for k, vals in params.items() if isinstance(vals, list)}
+
+            # Shapes the output / index according to the axis or multi param entry
+            if axis:
+                df[axis] = lambdas[0].axis_keys
+                df = df.set_index(axis)
+                df.index.set_names([axis])
+
+                # Filter out line with zero output
+                df = df.loc[
+                    df.apply(
+                        lambda row: not (row.name is None and row.values[0] == 0.0),
+                        axis=1,
+                    )
+                ]
+
+                # Rename "None" to others
+                df = df.rename(index={None: "_other_"})
+
+                # Sort index
+                df.sort_index(inplace=True)
+
+                # Add "total" line
+                df.loc["*sum*"] = df.sum(numeric_only=True)
+
+            elif len(list_params) > 0:
+                for k, vals in list_params.items():
+                    df[k] = vals
+                df = df.set_index(list(list_params.keys()))
+
+            else:
+                # Single output ? => give the single row the name of the model activity
                 df = df.rename(index={0: model_name})
 
             dfs[model_name] = df
 
     if len(dfs) == 1:
         df = list(dfs.values())[0]
-        return df
     else:
         # Concat several dataframes for several models
-        return pd.concat(list(dfs.values()))
+        df = pd.concat(list(dfs.values()))
+
+    if return_params:
+        metadata = {"Models": str(models), "Functional unit": functional_unit}
+        if description:
+            metadata["Description"] = description
+
+        return TabbedDataframe(metadata=metadata, Results=df, Parameters=_params_dataframe(params_all))
+    else:
+        return df
 
 
 def _createTechProxyForBio(act_key, target_db):
     """
-        We cannot reference directly biosphere in the model, since LCA can only be applied to products
-        We create a dummy activity in our DB, with same code, and single exchange of amount '1'
+    We cannot reference directly biosphere in the model, since LCA can only be applied to products
+    We create a dummy activity in our DB, with same code, and single exchange of amount '1'
     """
     dbname, code = act_key
     act = _getDb(dbname).get(code)
 
     # Biosphere ?
-    if (dbname == BIOSPHERE3_DB_NAME) or ("type" in act and act["type"] in ["emission", "natural resource"]) :
-
+    if (BIOSPHERE_PREFIX in dbname) or ("type" in act and act["type"] in ["emission", "natural resource"]):
         code_to_find = code + "#asTech"
 
         try:
             # Already created ?
             return _getDb(target_db).get(code_to_find)
-        except:
-            name = act['name'] + ' # asTech'
+        except DoesNotExist:
+            name = act["name"] + " # asTech"
 
             # Create biosphere proxy in User Db
-            res = newActivity(target_db, name, act['unit'], {act: 1},
-                              code=code_to_find,
-                              isProxy=True) # add a this flag to distinguish this dummy activity from others
+            res = newActivity(
+                target_db, name, act["unit"], {act: 1}, code=code_to_find, isProxy=True
+            )  # add a this flag to distinguish this dummy activity from others
             return res
-    else :
+    else:
         return act
 
 
-def _replace_fixed_params(expr, fixed_params, fixed_mode=FixedParamMode.DEFAULT) :
+def _replace_fixed_params(expr, fixed_params, fixed_mode=FixedParamMode.DEFAULT):
     """Replace fixed params with their value."""
-    sub = {symbols(key): val for param in fixed_params for key, val in param.expandParams(param.stat_value(fixed_mode)).items()}
+
+    sub = {key: val for param in fixed_params for key, val in param.expandParams(param.stat_value(fixed_mode)).items()}
+    sub = _toSymbolDict(sub)
     return expr.xreplace(sub)
 
-@with_db_context(arg="act")
-def actToExpression(act: Activity, extract_activities=None):
 
+def _safe_axis(axis_name: str):
+    if axis_name.isalnum():
+        return axis_name
+    else:
+        return re.sub("[^0-9a-zA-Z]+", "_", axis_name)
+
+
+def _tag_expr(expr, act, axis):
+    """Tag expression for one axe. Check the child expression is not already tagged with different values"""
+    axis_tag = act.get(axis, None)
+
+    if axis_tag is None:
+        return expr
+
+    axis_tag = _safe_axis(axis_tag)
+
+    if isinstance(expr, AxisDict):
+        res = 0
+        for key, val in expr._dict.items():
+            if key is not None and str(key) != axis_tag:
+                raise ValueError(
+                    "Inconsistent axis for one change of  '%s' : attempt to tag as '%s'. "
+                    "Already tagged as '%s'. Value of the exchange : %s" % (act["name"], axis_tag, key, str(val))
+                )
+            res += val
+    else:
+        res = expr
+
+    return AxisDict({axis_tag: res})
+
+
+@with_db_context(arg="act")
+def actToExpression(act: ActivityExtended, axis=None):
     """Computes a symbolic expression of the model, referencing background activities and model parameters as symbols
 
     Returns
     -------
         (sympy_expr, dict of symbol => activity)
     """
 
-    act_symbols : Dict[Symbol]= dict()  # Cache of  act = > symbol
+    act_symbols: Dict[Symbol] = dict()  # Cache of  act = > symbol
 
     def act_to_symbol(sub_act):
-        """ Transform an activity to a named symbol and keep cache of it """
+        """Transform an activity to a named symbol and keep cache of it"""
 
         db_name, code = sub_act.key
 
         # Look in cache
         if not (db_name, code) in act_symbols:
-
             act = _getDb(db_name).get(code)
-            name = act['name']
+            name = act["name"]
             base_slug = _slugify(name)
 
             slug = base_slug
             i = 1
             while symbols(slug) in act_symbols.values():
                 slug = f"{base_slug}{i}"
                 i += 1
 
             act_symbols[(db_name, code)] = symbols(slug)
 
         return act_symbols[(db_name, code)]
 
-    def rec_func(act: Activity, in_extract_path, parents=[]):
+    # Local cache of expressions
 
+    def actToExpressionRec(act: ActivityExtended, parents=[]):
         res = 0
         outputAmount = act.getOutputAmount()
 
-        if not _isForeground(act["database"]) :
+        if not _isForeground(act["database"]):
             # We reached a background DB ? => stop developping and create reference to activity
             return act_to_symbol(act)
 
         for exch in act.exchanges():
-
             formula = _getAmountOrFormula(exch)
 
-            if isinstance(formula, types.FunctionType):
+            if isinstance(formula, FunctionType):
                 # Some amounts in EIDB are functions ... we ignore them
                 continue
 
             #  Production exchange
-            if exch['input'] == exch['output']:
+            if exch["input"] == exch["output"]:
                 continue
 
-            input_db, input_code = exch['input']
+            input_db, input_code = exch["input"]
             sub_act = _getDb(input_db).get(input_code)
 
-
-            # If list of extract activites requested, we only integrate activites below a tracked one
-            exch_in_path = in_extract_path
-            if extract_activities is not None:
-                if sub_act in extract_activities :
-                    exch_in_path = in_extract_path or (sub_act in extract_activities)
-
             # Background DB => reference it as a symbol
-            if not _isForeground(input_db) :
-
-                if exch_in_path :
-                    # Add to dict of background symbols
-                    act_expr = act_to_symbol(sub_act)
-                else:
-                    continue
+            if not _isForeground(input_db):
+                act_expr = act_to_symbol(sub_act)
 
             # Our model : recursively it to a symbolic expression
             else:
-
                 parents = parents + [act]
-                if sub_act in parents :
+                if sub_act in parents:
                     raise Exception("Found recursive activities : " + ", ".join(_actName(act) for act in (parents + [sub_act])))
 
-                act_expr = rec_func(sub_act, exch_in_path, parents)
+                act_expr = actToExpressionRec(sub_act, parents)
 
             avoidedBurden = 1
 
-            if exch.get('type') == 'production' and not exch.get('input') == exch.get('output') :
-                debug("Avoided burden", exch[name])
+            if exch.get("type") == "production" and not exch.get("input") == exch.get("output"):
                 avoidedBurden = -1
 
-            #debug("adding sub act : ", sub_act, formula, act_expr)
-
             res += formula * act_expr * avoidedBurden
 
-        return res / outputAmount
+        res = res / outputAmount
+
+        # Axis ? transforms this to a dict with the correct Tag
+        if axis:
+            res = _tag_expr(res, act, axis)
 
-    expr = rec_func(act, extract_activities is None)
+        return res
+
+    expr = actToExpressionRec(act)
 
-    if isinstance(expr, float) :
+    if isinstance(expr, float):
         expr = simplify(expr)
     else:
         # Replace fixed params with their default value
         expr = _replace_fixed_params(expr, _fixed_params().values())
 
     return (expr, _reverse_dict(act_symbols))
 
 
 def _reverse_dict(dic):
     return {v: k for k, v in dic.items()}
-
-
-def exploreImpacts(impact, *activities : ActivityExtended, **params):
-    """
-    Advanced version of #printAct()
-
-    Displays all exchanges of one or several activities and their impacts.
-    If parameter values are provided, formulas will be evaluated accordingly.
-    If two activities are provided, they will be shown side by side and compared.
-    """
-    tables = []
-    names = []
-
-    diffOnly = params.pop("diffOnly", False)
-    withImpactPerUnit = params.pop("withImpactPerUnit", False)
-
-    for main_act in activities:
-
-        inputs_by_ex_name = dict()
-        data = dict()
-
-        for i, (name, input, amount) in enumerate(main_act.listExchanges()):
-
-            # Params provided ? Evaluate formulas
-            if len(params) > 0 and isinstance(amount, Basic):
-                new_params = [(name, value) for name, value in _completeParamValues(params).items()]
-                amount = amount.subs(new_params)
-
-            i = 1
-            ex_name = name
-            while ex_name in data:
-                ex_name = "%s#%d" % (name, i)
-                i += 1
-
-            inputs_by_ex_name[ex_name] = _createTechProxyForBio(input.key, main_act.key[0])
-
-            input_name = _actName(input)
-
-            if _isForeground(input.key[0]) :
-                input_name += "{user-db}"
-
-            data[ex_name] = dict(input=input_name, amount=amount)
-
-
-        # Provide impact calculation if impact provided
-        all_acts = list(set(inputs_by_ex_name.values()))
-        res = multiLCAAlgebric(all_acts, [impact], **params)
-        impacts = res[res.columns.tolist()[0]].to_list()
-
-        impact_by_act = {act : value for act, value in zip(all_acts, impacts)}
-
-        # Add impacts to data
-        for key, vals in data.items() :
-            amount = vals["amount"]
-            act = inputs_by_ex_name[key]
-            impact = impact_by_act[act]
-
-            if withImpactPerUnit :
-                vals["impact_per_unit"] = impact
-            vals["impact"] = amount * impact
-
-        # To dataframe
-        df = pd.DataFrame(data)
-
-        tables.append(df.T)
-        names.append(_actDesc(main_act))
-
-    full = pd.concat(tables, axis=1, keys=names, sort=True)
-
-    # Highlight differences in case two activites are provided
-    if len(activities) == 2:
-        YELLOW = "background-color:NavajoWhite"
-        diff_cols = ["amount", "input", "impact"]
-        cols1 = dict()
-        cols2 = dict()
-        for col_name in diff_cols :
-            cols1[col_name] = full.columns.get_loc((names[0], col_name))
-            cols2[col_name] = full.columns.get_loc((names[1], col_name))
-
-        if diffOnly:
-            def isDiff(row):
-                return row[cols1['impact']] != row[cols2['impact']]
-
-            full = full.loc[isDiff]
-
-        def same_amount(row):
-            res = [""] * len(row)
-            for col_name in diff_cols :
-                if row[cols1[col_name]] != row[cols2[col_name]] :
-                    res[cols1[col_name]] = YELLOW
-                    res[cols2[col_name]] = YELLOW
-            return res
-        full = full.style.apply(same_amount, axis=1)
-
-    return full
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/params.py` & `lca_algebraic-1.1/lca_algebraic/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,610 +1,617 @@
 import builtins
-import enum
 from collections import defaultdict
 from enum import Enum
-from typing import Dict, List, Union, Tuple
+from typing import Any, Dict, List, Union
 
 import brightway2 as bw
-import ipywidgets as widgets
 import numpy as np
+import pandas as pd
+from bw2data.backends.peewee import ExchangeDataset
+from bw2data.parameters import (
+    ActivityParameter,
+    DatabaseParameter,
+    Group,
+    ProjectParameter,
+)
 from IPython.core.display import HTML
-from bw2data.backends import LCIBackend
-from bw2data.backends.peewee import Activity
-from bw2data.database import Database
-from bw2data.parameters import ActivityParameter, ProjectParameter, DatabaseParameter, Group
-from bw2data.proxies import ActivityProxyBase
-from lca_algebraic.base_utils import ExceptionContext
-from scipy.stats import triang, truncnorm, norm, beta, lognorm
-from sympy import Symbol, Basic
+from scipy.stats import beta, lognorm, norm, triang, truncnorm
+from sympy import Basic, Expr, Symbol, lambdify, parse_expr
 from tabulate import tabulate
 
-from .base_utils import _snake2camel
-from .base_utils import error, as_np_array, _getAmountOrFormula, LANG
+from lca_algebraic.base_utils import ExceptionContext, ValueOrExpression
+from lca_algebraic.log import logger
 
-import lca_algebraic.base_utils
-from .base_utils import as_np_array, _getAmountOrFormula, _actName
+from .base_utils import _snake2camel, _user_functions, as_np_array
+from .database import DbContext
+from .log import warn
 
 DEFAULT_PARAM_GROUP = "acv"
 UNCERTAINTY_TYPE = "uncertainty type"
 
 
-
-
-class DbContext :
-    """
-        Context class specifying the current foreground DB in use. in internal
-        Used internally to distinguish database parameters with same names
-
-        usage :
-        with DbContext("db") :
-            <some code>
-
-    """
-    stack = []
-
-    @staticmethod
-    def current_db() :
-        if len(DbContext.stack) == 0:
-            return None
-        return DbContext.stack[-1]
-
-
-    def __init__(self, db : Union[str, ActivityProxyBase, LCIBackend]) :
-        if isinstance(db, ActivityProxyBase) :
-            self.db = db.key[0]
-        elif isinstance(db, str) :
-            self.db = db
-        else :
-            self.db = db.name
-
-    def __enter__(self):
-        DbContext.stack.append(self.db)
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        DbContext.stack.pop()
-
-
-
-
-
 class ParamType:
     """Type of parameters"""
 
     ENUM = "enum"
     """ Enum Parameter """
 
     BOOL = "bool"
     """ Boolean parameter """
 
     FLOAT = "float"
     """Float parameter """
 
-class DistributionType():
+
+class DistributionType:
     """
-        Type of statistic distribution of a float parameter.
-        Some type of distribution requires extra parameters, in italic, to be provided in the constructor of **ParamDef**()
+    Type of statistic distribution of a float parameter.
+    Some type of distribution requires extra parameters, in italic, to be provided in the constructor of **ParamDef**()
     """
 
     LINEAR = "linear"
     """ Uniform distribution between *min* and *max*"""
 
     NORMAL = "normal"
     """ Normal distribution, centered on *default* value (mean), with deviation of *std* and truncated between *min* and *max*"""
 
     LOGNORMAL = "lognormal"
     """ Lognormal distribution, centered on *default* value (mean), with deviation of *std*, not truncated """
 
-    BETA = "beta" # requires a, b 'default' is used as the mean. 'std' is used as 'scale' factor
-    """ Beta distribution with extra params *a* and *b*, 
+    BETA = "beta"  # requires a, b 'default' is used as the mean. 'std' is used as 'scale' factor
+    """ Beta distribution with extra params *a* and *b*,
     using *default* value as 'loc' (0 of beta distribution) and *std* as 'scale' (1 of beta distribution)
     See [scipy doc](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.beta.html#scipy.stats.beta) """
 
     TRIANGLE = "triangle"
     """ Triangle distribution between *min* and *max* (set to zero probability), with highest probability at *default* value """
 
     FIXED = "fixed"
     """ Fixed value, not considered as a variable input for monte carlo simulation. """
 
 
-class _UncertaintyType :
-    '''Enum of uncertainty types of Brightway.
+class _UncertaintyType:
+    """Enum of uncertainty types of Brightway.
     See https://stats-arrays.readthedocs.io/en/latest/
-    '''
+    """
+
     UNDEFINED = 0
     FIXED = 1
     LOGNORMAL = 2
     NORMAL = 3
     UNIFORM = 4
     TRIANGLE = 5
     DISCRETE = 7
     BETA = 10
 
 
 # Map to Brightay2 / stats-arrays Distribution Type
 _DistributionTypeMap = {
-    DistributionType.LINEAR : _UncertaintyType.UNIFORM,
-    DistributionType.BETA : _UncertaintyType.BETA,
-    DistributionType.NORMAL : _UncertaintyType.NORMAL,
+    DistributionType.LINEAR: _UncertaintyType.UNIFORM,
+    DistributionType.BETA: _UncertaintyType.BETA,
+    DistributionType.NORMAL: _UncertaintyType.NORMAL,
     DistributionType.LOGNORMAL: _UncertaintyType.LOGNORMAL,
-    DistributionType.TRIANGLE : _UncertaintyType.TRIANGLE,
-    DistributionType.FIXED : _UncertaintyType.FIXED, # I made that up
+    DistributionType.TRIANGLE: _UncertaintyType.TRIANGLE,
+    DistributionType.FIXED: _UncertaintyType.FIXED,  # I made that up
 }
 
-_DistributionTypeMapReverse = {val:key for key, val in _DistributionTypeMap.items()}
+_DistributionTypeMapReverse = {val: key for key, val in _DistributionTypeMap.items()}
 
 
 class FixedParamMode:
-    """ Enum describing what value to set for fixed params """
+    """Enum describing what value to set for fixed params"""
+
     DEFAULT = "default"
     """ Use the default value as the parameter """
 
     MEDIAN = "median"
     """ Use the median of the distribution of the parameter """
 
     MEAN = "mean"
     """ Use the mean of the distribution of the parameter """
 
+
 class ParamDef(Symbol):
-    '''Generic definition of a parameter, with name, bound, type, distribution
+    """
+    Generic definition of a parameter, with name, bound, type, distribution
     This definition will serve both to generate brightway2 parameters and to evaluate.
-
     This class inherits sympy Symbol, making it possible to use in standard arithmetic python
     while keeping it as a symbolic expression (delayed evaluation).
-    '''
+
+    Don't instantiate it directly. Use the function **newXXXParam() instead.
+    """
 
     def __new__(cls, name, *karg, **kargs):
         # We use dbname as an "assumption" so that two symbols with same name are not equal if from separate DBs
         assumptions = dict()
-        if 'dbname' in kargs and kargs['dbname'] :
-            assumptions[kargs['dbname']] = True
+        assumptions["real"] = True
 
-        return Symbol.__new__(cls, name, **assumptions)
+        if "dbname" in kargs and kargs["dbname"]:
+            assumptions[kargs["dbname"]] = True
 
-    def __init__(self, name, type: str, default, min=None, max=None, unit="", description="", label=None, label_fr=None,
-                 group=None, distrib:DistributionType=None, dbname=None, **kwargs):
+        return Symbol.__new__(cls, name, **assumptions)
 
+    def __init__(
+        self,
+        name,
+        type: str,
+        default,
+        min=None,
+        max=None,
+        unit="",
+        description="",
+        label=None,
+        group=None,
+        distrib: DistributionType = None,
+        dbname=None,
+        formula=None,
+        **kwargs,
+    ):
         self.name = name
         self.type = type
         self.default = default
         self.description = description
         self.min = min
         self.max = max
         self.unit = unit
         self.label = label
-        self.label_fr = label_fr
         self.group = group
         self.distrib = distrib
         self.dbname = dbname
+        self.formula = formula
 
-        if (self.dbname == None) :
-            error("Warning : param '%s' linked to root project instead of a specific DB" % self.name)
+        # if (self.dbname == None) :
+        #    error("Warning : param '%s' linked to root project instead of a specific DB" % self.name)
 
         # Cleanup distribution in case of overriding already existing param (reused because of inheritance of Symbol)
-        if hasattr(self, "_distrib") :
+        if hasattr(self, "_distrib"):
             del self._distrib
 
-        if not distrib and type == ParamType.FLOAT  :
+        if not distrib and type == ParamType.FLOAT:
             if self.min is None:
-                error("No 'min/max' provided, param %s marked as FIXED" % self.name)
-                self.distrib = DistributionType.FIXED
+                raise Exception(f"No 'min/max' provided for {self.name}, distrib should explicitely set to FIXED")
             else:
                 self.distrib = DistributionType.LINEAR
 
-        elif distrib in [DistributionType.NORMAL, DistributionType.LOGNORMAL] :
-            if not 'std' in kwargs:
+        elif distrib in [DistributionType.NORMAL, DistributionType.LOGNORMAL]:
+            if "std" not in kwargs:
                 raise Exception("Standard deviation is mandatory for normal / lognormal distribution")
-            self.std = kwargs['std']
+            self.std = kwargs["std"]
 
-            if distrib == DistributionType.LOGNORMAL and self.min is not None :
-                error("Warning : LogNormal does not support min/max boundaries for parameter : ", self.name)
+            if distrib == DistributionType.LOGNORMAL and self.min is not None:
+                warn(
+                    "Warning : LogNormal does not support min/max boundaries for parameter : ",
+                    self.name,
+                )
 
-        elif distrib == DistributionType.BETA :
-            if not 'a' in kwargs or not 'b' in kwargs or not 'std' in kwargs :
+        elif distrib == DistributionType.BETA:
+            if "a" not in kwargs or "b" not in kwargs or "std" not in kwargs:
                 raise Exception("Beta distribution requires params 'a' 'b' and 'std' (used as scale)")
-            self.a = kwargs['a']
-            self.b = kwargs['b']
-            self.std = kwargs['std']
-
-    def stat_value(self, mode : FixedParamMode):
-        """ Compute a fixed value for this parameter, according to the requested FixedParamMode """
-        if mode == FixedParamMode.DEFAULT :
+            self.a = kwargs["a"]
+            self.b = kwargs["b"]
+            self.std = kwargs["std"]
+
+    def stat_value(self, mode: FixedParamMode):
+        """Computes a fixed value for this parameter, either median or mean, according to the requested FixedParamMode and its
+        statistical distribution."""
+        if mode == FixedParamMode.DEFAULT:
             return self.default
-        else :
+        else:
             # Compute statistical value for replacement
             rnd = np.random.rand(1000)
             x = self.rand(rnd)
 
-            if mode == FixedParamMode.MEAN :
+            if mode == FixedParamMode.MEAN:
                 return np.mean(x)
-            elif mode == FixedParamMode.MEDIAN :
+            elif mode == FixedParamMode.MEDIAN:
                 return np.median(x)
-            else :
+            else:
                 raise Exception("Unkown mode " + mode)
 
-
     def get_label(self):
-        if LANG == "fr " and self.label_fr is not None :
-            return self.label_fr
-        elif self.label is not None:
+        if self.label is not None:
             return self.label
         else:
             return self.name.replace("_", " ")
 
     def range(self, n):
         """Return N uniform values of this parameter, within its range of definition"""
         step = (self.max - self.min) / (n - 1)
         return list(i * step + self.min for i in range(0, n))
 
     def rand(self, alpha):
-        """Transforms a random number between 0 and 1 to valid value according to the distribution of probability of the parameter"""
+        """Transforms a random number between 0 and 1 to valid value according
+        to the distribution of probability of the parameter
 
-        if self.distrib == DistributionType.FIXED :
+        Parameters
+        ----------
+
+        alpha:
+            Can be a *float* or numpy array of floats, between 0 and 1.
+        """
+
+        if self.distrib == DistributionType.FIXED:
             return self.default
-        
+
         elif self.distrib == DistributionType.LINEAR:
-            if self.min is None or self.max is None :
+            if self.min is None or self.max is None:
                 raise Exception("Missing min/max for : " + self.name)
             return self.min + alpha * (self.max - self.min)
 
-        else :
+        else:
             if not hasattr(self, "_distrib"):
-
                 if self.distrib == DistributionType.TRIANGLE:
                     scale = self.max - self.min
                     c = (self.default - self.min) / scale
                     self._distrib = triang(c, loc=self.min, scale=scale)
 
                 elif self.distrib == DistributionType.NORMAL:
-
-                    if self.min :
+                    if self.min:
                         # Truncated normal
                         self._distrib = truncnorm(
                             (self.min - self.default) / self.std,
                             (self.max - self.min) / self.std,
                             loc=self.default,
-                            scale=self.std)
-                    else :
+                            scale=self.std,
+                        )
+                    else:
                         # Normal
-                        self._distrib = norm(
-                            loc=self.default,
-                            scale=self.std)
+                        self._distrib = norm(loc=self.default, scale=self.std)
 
                 elif self.distrib == DistributionType.LOGNORMAL:
-
                     self._distrib = lognorm(self.default, self.std)
 
                 elif self.distrib == DistributionType.BETA:
-                    self._distrib = beta(
-                        self.a,
-                        self.b,
-                        loc=self.default,
-                        scale=self.std)
+                    self._distrib = beta(self.a, self.b, loc=self.default, scale=self.std)
 
                 else:
                     raise Exception("Unkown distribution type " + self.distrib)
 
-
             return self._distrib.ppf(alpha)
 
     def __hash__(self):
-        return hash((self.dbname, self.name))
+        return hash((getattr(self, "dbname", ""), self.name))
 
     def __eq__(self, other):
-        if isinstance(other, ParamDef) :
-            return self.name == other.name and self.dbname == other.dbname
-        else :
+        if isinstance(other, ParamDef):
+            return self.name == other.name and getattr(self, "dbname", None) == getattr(other, "dbname", None)
+        else:
             return Symbol.__eq__(self, other)
 
-    # Expand parameter (useful for enum param)
     def expandParams(self, value=None) -> Dict[str, float]:
-        if value == None:
+        """Abstract function to represent a parameter as a dict : useful to be consistent with Enum params"""
+        if value is None:
             value = self.default
         return {self.name: value}
 
-    # Useful for enum param, having several names
     def names(self, use_label=False):
-        if use_label :
+        """Generic method usefull to be consistent with Enum parameters"""
+        if use_label:
             return [self.get_label()]
         else:
             return [self.name]
 
     def __repr__(self):
         return self.name
 
 
 class BooleanDef(ParamDef):
-    """Parameter with discrete value 0 or 1"""
+    """Parameter with discrete value 0 or 1. Use **newBoolParam()** to instantiate it."""
 
     def __init__(self, name, **argv):
-        if not "min" in argv:
+        if "min" not in argv:
             argv = dict(argv, min=None, max=None)
         super(BooleanDef, self).__init__(name, ParamType.BOOL, **argv)
 
-
     def range(self, n):
         return [0, 1]
 
     def rand(self, alpha):
         return np.around(alpha)
 
 
 class EnumParam(ParamDef):
-    """Enum param is a facility wrapping a choice / switch as many boolean parameters.
+    """
+    Enum param is a facility wrapping a choice / switch as many boolean parameters.
     It is not itself a Sympy symbol. use #symbol("value") to access it.
     Statistics weight can be attached to values by providing a dict.
     """
 
     def __init__(self, name, values: Union[List[str], Dict[str, float]], **argv):
-
-        if not "min" in argv :
+        if "min" not in argv:
             argv = dict(argv, min=None, max=None)
         super(EnumParam, self).__init__(name, ParamType.ENUM, **argv)
-        if type(values) == list :
+        if isinstance(values, list):
             self.values = values
-            self.weights = {key:1 for key in values}
-        else :
+            self.weights = {key: 1 for key in values}
+        else:
             self.weights = values
             self.values = list(values)
         self.sum = sum(self.weights.values())
 
     def expandParams(self, currValue=None):
         """
         Return a dictionarry of single enum values as sympy symbols, with only a single one set to 1.
         currValue can be either a single enum value (string) of dict of enum value => weight.
         """
 
         # A dict of weights was passed
-        if isinstance(currValue, dict) :
-            res = { "%s_%s" % (self.name, key) : val / self.sum for key, val in currValue.items()}
+        if isinstance(currValue, dict):
+            res = {"%s_%s" % (self.name, key): val / self.sum for key, val in currValue.items()}
             res["%s_default" % self.name] = 0
             return res
 
-
-
         # Normal case
         values = self.values + [None]
 
         # Bad value ?
-        if currValue not in values :
-            raise Exception("Invalid value %s for param %s. Should be in %s" %
-                            (currValue, self.name, str(self.values)))
+        if currValue not in values:
+            raise Exception("Invalid value %s for param %s. Should be in %s" % (currValue, self.name, str(self.values)))
 
         res = dict()
         for enum_val in values:
-            var_name = "%s_%s" % (self.name, enum_val if enum_val is not None else "default")
+            var_name = "%s_%s" % (
+                self.name,
+                enum_val if enum_val is not None else "default",
+            )
             res[var_name] = 1.0 if enum_val == currValue else 0.0
         return res
 
-    def symbol(self, enumValue):
-        """Return the invididual symbol for a given enum value : <paramName>_<paramValue>"""
-        if enumValue is None:
-            return Symbol(self.name + '_default')
-        if not enumValue in self.values:
-            raise Exception("enumValue should be one of %s. Was %s" % (str(self.values), enumValue))
-        return Symbol(self.name + '_' + enumValue)
+    def symbol(self, choice):
+        """Returns the invididual Sympy symbol for a given choice : <paramName>_<choice>"""
+        if choice is None:
+            return Symbol(self.name + "_default")
+        if choice not in self.values:
+            raise Exception("enumValue should be one of %s. Was %s" % (str(self.values), choice))
+        return Symbol(self.name + "_" + choice)
 
     def names(self, use_label=False):
-        if use_label :
+        if use_label:
             base_name = self.get_label()
-        else :
+        else:
             base_name = self.name
         return ["%s_%s" % (base_name, value) for value in (self.values + ["default"])]
 
     def rand(self, alpha):
         alpha = as_np_array(alpha)
         alpha = alpha * self.sum
 
         # Build bins
         if not hasattr(self, "_bins"):
             self._bins = [0]
-            for i in range(len(self.values)) :
+            for i in range(len(self.values)):
                 enumvalue = self.values[i]
                 self._bins.append(self._bins[i] + self.weights[enumvalue])
 
         inds = np.digitize(alpha, self._bins, right=True)
         values = np.asarray(self.values)
 
         return values[inds - 1]
 
     def range(self, n):
         return self.values
 
-    def stat_value(self, mode : FixedParamMode):
-        if mode == FixedParamMode.DEFAULT :
+    def stat_value(self, mode: FixedParamMode):
+        if mode == FixedParamMode.DEFAULT:
             return self.default
-        else :
+        else:
             # For statistical analysis we setup enum as its weights of values,
             # This distrib is then expanded as float parameters, for better fit of the distribution
             return self.weights
 
 
 def newParamDef(name, type, dbname=None, save=True, **kwargs):
     """
-        Creates a parameter and register it into a global registry and as a brightway parameter.
-
-        Parameters
-        ----------
-
-        type : Type of the parameter (From ParamType)
-        save : Boolean, persist this into Brightway2 project (True by default)
-        dbname : Optional name of db. If None, the parameter is a project parameter
-        other arguments : Refer to the documentation of BooleanDef ParamDef and EnumParam
+    Creates a parameter and register it into a global registry and as a brightway parameter.
 
+    Parameters
+    ----------
+    type :
+        Type of the parameter (From ParamType)
+    save :
+        Boolean, persist this into Brightway2 project (True by default)
+    dbname :
+        Optional name of db. If None, the parameter is a project parameter
+    other arguments :
+        Refer to the documentation of BooleanDef ParamDef and EnumParam
     """
     if type == ParamType.ENUM:
         param = EnumParam(name, dbname=dbname, **kwargs)
     elif type == ParamType.BOOL:
         param = BooleanDef(name, dbname=dbname, **kwargs)
     else:
         param = ParamDef(name, dbname=dbname, type=type, **kwargs)
 
     _param_registry()[name] = param
 
     # Save in brightway2 project
-    if save :
+    if save:
         _persistParam(param)
 
     return param
 
+
 _BOOLEAN_UNCERTAINTY_ATTRIBUTES = {
     UNCERTAINTY_TYPE: _UncertaintyType.DISCRETE,
-    "minimum" : 0,
-    "maximum" : 2 # upper bound + 1
+    "minimum": 0,
+    "maximum": 2,  # upper bound + 1
 }
 
-def persistParams() :
-    """ Persist parameters into Brightway project, as per :
-     https://stats-arrays.readthedocs.io/en/latest/
+
+def persistParams():
     """
+    Persist parameters into Brightway project, as per : https://stats-arrays.readthedocs.io/en/latest/.
+
+    This is important only in case you want t o:
+    - Use parameters outside lca_algebraic (Activity Browser for instance)
+    - Use *loadParams()* to init your parameters instead of deleting them and creating them programmaically each time.
 
-    for param in _param_registry().all() :
+    This function is automatically run when creating new parameters. However, it should be called manually after **updating**
+    manually some properties of a parameter.
+    """
+    for param in _param_registry().all():
         _persistParam(param)
 
+
 def _persistParam(param):
-    """ Persist parameter into Brightway project """
+    """Persist parameter into Brightway project"""
     out = []
 
     # Common attributes for all types of params
     bwParam = dict(
         name=param.name,
         group=param.group,
         label=param.label,
         unit=param.unit,
-        description=param.description)
+        formula=str(param.formula) if param.formula else None,
+        description=param.description,
+    )
 
-    if (param.dbname) :
+    if param.dbname:
         bwParam["database"] = param.dbname
 
-    if param.type == ParamType.ENUM :
+    if param.type == ParamType.ENUM:
         # Enum are not real params but a set of parameters
-        for value in param.values :
+        for value in param.values:
             enumValueParam = dict(bwParam)
-            enumValueParam["name"] = param.name + '_' + value
+            enumValueParam["name"] = param.name + "_" + value
             enumValueParam.update(_BOOLEAN_UNCERTAINTY_ATTRIBUTES)
             # Use 'scale' as weight for this enum value
-            enumValueParam['scale'] = param.weights[value]
-            enumValueParam['amount'] = 1 if param.default == value else 0
+            enumValueParam["scale"] = param.weights[value]
+            enumValueParam["amount"] = 1 if param.default == value else 0
             out.append(enumValueParam)
-    else :
-
+    else:
         bwParam["amount"] = param.default
 
-        if param.type == ParamType.BOOL :
+        if param.type == ParamType.BOOL:
             # "Discrete uniform"
             bwParam.update(_BOOLEAN_UNCERTAINTY_ATTRIBUTES)
 
-        elif param.type == ParamType.FLOAT :
-
+        elif param.type == ParamType.FLOAT:
             # Save uncertainty
             bwParam[UNCERTAINTY_TYPE] = _DistributionTypeMap[param.distrib]
             bwParam["minimum"] = param.min
             bwParam["maximum"] = param.max
             bwParam["loc"] = param.default
 
-            if param.distrib in [DistributionType.NORMAL, DistributionType.LOGNORMAL] :
+            if param.distrib in [DistributionType.NORMAL, DistributionType.LOGNORMAL]:
                 bwParam["scale"] = param.std
 
             elif param.distrib == DistributionType.BETA:
-
                 bwParam["scale"] = param.std
                 bwParam["loc"] = param.a
                 bwParam["shape"] = param.b
 
-        else :
-            error("Param type not supported", param.type)
+        else:
+            warn("Param type not supported", param.type)
 
         out.append(bwParam)
 
-    if param.dbname :
+    if param.dbname:
         bw.parameters.new_database_parameters(out, param.dbname)
     else:
         bw.parameters.new_project_parameters(out)
 
-def _loadArgs(data) :
+
+def _loadArgs(data):
     """Load persisted data attributes into ParamDef attributes"""
     return {
         "group": data.get("group"),
-        "dbname" : data.get("database"),
+        "dbname": data.get("database"),
         "default": data.get("amount"),
         "label": data.get("label"),
         "description": data.get("description"),
         "min": data.get("minimum"),
         "max": data.get("maximum"),
-        "unit" : data.get("unit")
+        "unit": data.get("unit"),
+        "formula": data.get("formula", None),
     }
 
+
 def loadParams(global_variable=True, dbname=None):
     """
     Load parameters from Brightway database, as per : https://stats-arrays.readthedocs.io/en/latest/
 
+    The recommended way is to delete parameters at the start of your session and to define them programmically each time.
+
+    However, it can be useful if your parameters come from an import or where defined in **Activity Browser**.
+
     Parameters
     ----------
-    global_variable If true, loaded parameters are made available as global variable.
-    dbname : None. By default load all project and database parameters. If provided, only load DB params
+    global_variable:
+        If true, loaded parameters are made available as global variable.
+    dbname:
+        If provided, load only database parameters for the given db
+
+    Returns
+    -------
+    A dictionary of parameters
     """
 
-    enumParams=defaultdict(lambda : dict())
+    enumParams = defaultdict(lambda: dict())
 
-    def register(param) :
+    def register(param):
         _param_registry()[param.name] = param
 
         # Make it available as global var
         if global_variable:
-            if param.name in builtins.__dict__ :
-                error("Variable '%s' was already defined : overidding it with param." % param.name)
+            if param.name in builtins.__dict__:
+                warn("Variable '%s' was already defined : overidding it with param." % param.name)
             builtins.__dict__[param.name] = param
 
     select = DatabaseParameter.select()
-    if dbname :
+    if dbname:
         select = select.where(DatabaseParameter.database == dbname)
 
     params = list(select)
-    if not dbname :
+    if not dbname:
         params += list(ProjectParameter.select())
 
     for bwParam in params:
         data = bwParam.data
         data["amount"] = bwParam.amount
         name = bwParam.name
 
         type = data.get(UNCERTAINTY_TYPE, None)
 
         # print("Data for ", name, data)
 
         # Common extra args
         args = _loadArgs(data)
 
-        if type == _UncertaintyType.DISCRETE :
+        if type == _UncertaintyType.DISCRETE:
             # Boolean or enum
 
-            if data.get('scale') is not None :
+            if data.get("scale") is not None:
                 # Enum param : group them by common prefix
                 splits = name.split("_")
                 enum_value = splits.pop()
                 enum_name = "_".join(splits)
                 enumParams[enum_name][enum_value] = data
                 continue
 
-            elif data["maximum"] == 2 :
+            elif data["maximum"] == 2:
                 del args["max"], args["min"]
                 param = newBoolParam(name, save=False, **args)
             else:
-                error("Non boolean discrete values (max != 2) are not supported for param :", name)
+                warn(
+                    "Non boolean discrete values (max != 2) are not supported for param :",
+                    name,
+                )
                 continue
-        else :
+        else:
             # Float parameter
-            if type is None:
-                error("'Uncertainty type' of param %s not provided. Assuming UNIFORM")
+            if type is None or type == _UncertaintyType.UNDEFINED:
+                warn("'Uncertainty type' of param %s not provided. Assuming UNIFORM")
                 type = _UncertaintyType.UNIFORM
 
             # Uncertainty type to distribution type
             args["distrib"] = _DistributionTypeMapReverse[type]
 
-            if type == _UncertaintyType.TRIANGLE :
+            if type == _UncertaintyType.TRIANGLE:
                 args["default"] = data["loc"]
 
             elif type in [_UncertaintyType.NORMAL, _UncertaintyType.LOGNORMAL]:
                 args["default"] = data["loc"]
                 args["std"] = data["scale"]
 
             elif type == _UncertaintyType.BETA:
@@ -614,309 +621,640 @@
                 args["b"] = data["shape"]
 
             param = newFloatParam(name, save=False, **args)
 
         # Save it in shared dictionnary
         register(param)
 
-
     # Loop on EnumParams
-    for param_name, param_values in enumParams.items() :
+    for param_name, param_values in enumParams.items():
         first_enum_param = list(param_values.values())[0]
         args = _loadArgs(first_enum_param)
         del args["default"]
 
         # Dictionary of enum values with scale as weight
-        args["values"] = {key : data["scale"] for key, data in param_values.items()}
+        args["values"] = {key: data["scale"] for key, data in param_values.items()}
 
         # Default enum value is the one with amount=1
         defaults = list(key for key, data in param_values.items() if data.get("amount") == 1)
-        if len(defaults) == 1 :
+        if len(defaults) == 1:
             default = defaults[0]
-        else :
-            default= None
-            error("No default enum value found for ", param_name, defaults)
+        else:
+            default = None
+            warn("No default enum value found for ", param_name, defaults)
 
-        param = newEnumParam(param_name, default, save=False, **args)
+        param = newEnumParam(name=param_name, default=default, save=False, **args)
 
         # Save it in shared dict
         register(param)
 
+    # Parse formulas
+    for param in _param_registry().all():
+        with DbContext(param.dbname):
+            if isinstance(param.formula, str):
+                param.formula = _parse_formula(param.formula)
+
+    return _param_registry()
+
+
+def newFloatParam(
+    name,
+    default,
+    min: float = None,
+    max: float = None,
+    unit: str = None,
+    description: str = None,
+    label: str = None,
+    group: str = None,
+    distrib: DistributionType = DistributionType.LINEAR,
+    formula=None,
+    save=True,
+    **kwargs,
+):
+    """
+    Creates a float (decimal) parameter.
+
+    Parameters
+    ----------
+    name:
+        Name of the parameter
+    default:
+        Default value
+    min:
+        Minimum value
+    max:
+        Maximum value
+    unit:
+        Unit of the parameter
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+    distrib:
+        Type of the distribution (optional) Linear (uniform) by default
+    formula:
+        Sympy expression. Optional. If provided the default value of this parameter (if not provided at runtime) will be computed
+        from other parameter values.
+    kwargs:
+        Extra parameters required for advanced distribution types.
+
+
+    Examples
+    --------
+
+    The following code defines a float parameter *p1* of unit *kg*, with a triangle distribution.
+
+    >>> p1 = newFloatParam("p1", min=1.0, max=3.0, default=2.0, distrib=DistributionType.TRIANGLE, unit="kg")
+
+    Returns
+    -------
+    The newly created parameter
+
+    """
+    return newParamDef(
+        name=name,
+        type=ParamType.FLOAT,
+        default=default,
+        min=min,
+        max=max,
+        unit=unit,
+        description=description,
+        label=label,
+        group=group,
+        distrib=distrib,
+        formula=formula,
+        save=save,
+        **kwargs,
+    )
+
+
+def newBoolParam(name, default, description: str = None, label: str = None, group: str = None, formula=None, save=True, **kwargs):
+    """
+    Creates a boolean parameter.
+
+    Parameters
+    ----------
+    name:
+        Name of the parameter
+    default:
+        Default value
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+    formula:
+        Sympy expression. Optional. If provided the default value of this parameter (if not provided at runtime) will be computed
+        from other parameter values.
+
+
+    Examples
+    --------
+
+    >>> p1 = newBoolParam("p1", default=0, group="param group")
+
+    Returns
+    -------
+    The newly created parameter
+
+    """
+    return newParamDef(
+        name,
+        ParamType.BOOL,
+        default=default,
+        description=description,
+        label=label,
+        group=group,
+        formula=formula,
+        save=save,
+        **kwargs,
+    )
+
+
+def newEnumParam(
+    name: str,
+    default: str,
+    values: Union[List[str], Dict[str, float]],
+    description: str = None,
+    label: str = None,
+    group: str = None,
+    save=True,
+    **kwargs,
+):
+    """
+    Creates an enum parameter : a set of mutually exclusive boolean choices.
+    Enum parameters themselves are *not* Sympy symbols. Each of the choice is represented internally
+    as a boolean sympy symbol, that can be accessed via **param.symbol("choice_name")**
+
+    Parameters
+    ----------
+
+    name:
+        Name of the parameter
+    default:
+        Default
+    values:
+        Possible choices. The values can be provided as a list of strings, in which case every choice is equiprobable.
+        They can also be provided as a python dictionnary of "choice" => value. The proability to be picked is then the
+        pro-rata of the value.
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+
+    Examples
+    --------
+
+    *p1* is an enum param with equiprobable choices "choice_a", "choice_b" and "choice_c"
+
+    >>> p1 = newEnumParam("p1", default="choice_a", values=["choice_a", "choice_b", "choice_c"])
+
+    *p2* is an anum param with "choice_a" and "choice_b" of probability 25% and "choice_c" of probability 50%.
+
+    >>> p2 = newEnumParam("p2", default="choice_a", values={"choice_a":1, "choice_b":1, "choice_c":2})
+
+    """
+    return newParamDef(
+        name,
+        ParamType.ENUM,
+        default=default,
+        values=values,
+        description=description,
+        label=label,
+        group=group,
+        save=save,
+        **kwargs,
+    )
 
-def newFloatParam(name, default, dbname=None, **kwargs):
-    """ Create a FLOAT parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.FLOAT, dbname=dbname, default=default, **kwargs)
-
-def newBoolParam(name, default, dbname=None, **kwargs):
-    """ Create a BOOL parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.BOOL, dbname=dbname, default=default, **kwargs)
-
-def newEnumParam(name, default, dbname=None, **kwargs):
-    """ Create a ENUM parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.ENUM, dbname=dbname, default=default, **kwargs)
 
 def _variable_params(param_names=None):
-    if param_names is None :
-        param_names =  _param_registry().keys()
-    params = {key : _param_registry()[key] for key in param_names}
+    if param_names is None:
+        param_names = _param_registry().keys()
+    params = {key: _param_registry()[key] for key in param_names}
     return {key: param for key, param in params.items() if param.distrib != DistributionType.FIXED}
 
 
 def _fixed_params(param_names=None):
-    if param_names is None :
-        param_names =  _param_registry().keys()
-    params = {key : _param_registry()[key] for key in param_names}
+    if param_names is None:
+        param_names = _param_registry().keys()
+    params = {key: _param_registry()[key] for key in param_names}
     return {key: param for key, param in params.items() if param.distrib == DistributionType.FIXED}
 
 
 def _listOfDictToDictOflist(LD):
     return {k: [dic[k] for dic in LD] for k in LD[0]}
 
-class DuplicateParamsAndNoContextException(Exception) :
+
+class DuplicateParamsAndNoContextException(Exception):
     pass
 
-class ParamRegistry :
-    """ In memory registry of parameters, acting like a dict and maintaining parameters with possibly same names on several DBs"""
-    def __init__(self) :
+
+class ParamRegistry:
+
+    """In memory registry of parameters, acting like a dict and maintaining parameters with possibly same names on several DBs"""
+
+    def __init__(self):
         # We store a dict of dict
         # Param Name -> { dbname ->  param}
-        self.params : Dict[Dict[ParamDef]] = defaultdict(dict)
+        self.params: Dict[Dict[ParamDef]] = defaultdict(dict)
 
     def __len__(self):
         return len(self.params)
 
     def __getitem__(self, key):
-        params_per_db = self.params[key]
-        if len(params_per_db) == 1 :
-            return list(params_per_db.values())[0]
-
-        if DbContext.current_db() == None :
-            dbs = [key or '<project>' for key in params_per_db.keys()]
-            raise DuplicateParamsAndNoContextException(
-
-                """
-                Found several params with name '%s', linked to databases (%s) . Yet no context is provided. 
-                Please embed you code in a DbContext :
-                    with DbContext(currentdb) :
-                        <code>
-                """ % (key, ", ".join(dbs)))
-        if DbContext.current_db() in params_per_db :
-            return params_per_db[DbContext.current_db()]
-        else :
-            return params_per_db[None]
+        try:
+            params_per_db = self.params[key]
+            if len(params_per_db) == 1:
+                return list(params_per_db.values())[0]
+
+            if DbContext.current_db() is None:
+                dbs = [key or "<project>" for key in params_per_db.keys()]
+                raise DuplicateParamsAndNoContextException(
+                    """
+                    Found several params with name '%s', linked to databases (%s) . Yet no context is provided.
+                    Please embed you code in a DbContext :
+                        with DbContext(currentdb) :
+                            <code>
+                    """
+                    % (key, ", ".join(dbs))
+                )
+            if DbContext.current_db() in params_per_db:
+                return params_per_db[DbContext.current_db()]
+            else:
+                return params_per_db[None]
 
-    def __setitem__(self, key, param : ParamDef):
+        except KeyError:
+            raise Exception(f"Parameter {key} not found :. Valid parameters : {self.keys()}")
+
+    def as_dict(self):
+        return dict(self.items())
+
+    def __setitem__(self, key, param: ParamDef):
         if param.dbname in self.params[key]:
-            error("[ParamRegistry] Param %s was already defined in '%s' : overriding." %
-                  (param.name, param.dbname or '<project>'))
+            warn("[ParamRegistry] Param %s was already defined in '%s' : overriding." % (param.name, param.dbname or "<project>"))
 
         self.params[key][param.dbname] = param
 
     def __contains__(self, key):
         return key in self.params
 
-    def values(self) :
+    def values(self):
         return [self.__getitem__(key) for key in (self.params)]
 
-    def keys(self) :
+    def keys(self):
         return self.params.keys()
 
-    def items(self) :
+    def items(self):
         return [(key, self.__getitem__(key)) for key in self.params.keys()]
 
     def clear(self, db_name=None):
-        if db_name is None :
+        if db_name is None:
             self.params.clear()
-        else :
-            for param_name, db_params in self.params.items() :
-                if db_name in db_params :
+        else:
+            for param_name, db_params in self.params.items():
+                if db_name in db_params:
                     del db_params[db_name]
 
-    def all(self) :
+    def all(self):
         """Return list of all parameters, including params with same names and different DB"""
         return list(param for params in self.params.values() for param in params.values())
 
+
 # Possible param values : either floator string (enum value)
 ParamValue = Union[float, str]
 
 # Single value or list of values
-ParamValues = Union[List[ParamValue],  ParamValue]
+ParamValues = Union[List[ParamValue], ParamValue]
 
 
-def _param_registry() -> Dict[str, ParamDef] :
+def _param_registry() -> ParamRegistry:
     # Prevent reset upon auto reload in jupyter notebook
-    if not 'param_registry' in builtins.__dict__:
+    if "param_registry" not in builtins.__dict__:
         builtins.param_registry = ParamRegistry()
 
     return builtins.param_registry
 
-def _completeParamValues(params: Dict[str, ParamValues], required_params : List[str]=None, setDefaults=False) :
-    """Check parameters and expand enum params.
 
-    Returns
-    -------
-        Dict of param_name => float value
-    """
+def all_params() -> Dict[str, ParamDef]:
+    """Return the dict of all parameters defined in memory"""
+    return {param.name: param for param in _param_registry().all()}
 
-    # Add default values for required params
-    if required_params :
-        for param_name in required_params :
-            param = _param_registry()[param_name]
-            if not param_name in params :
-                params[param_name] = param.default
-                error("Required param '%s' was missing, replacing by default value : %s" % (param_name, str(param.default)))
 
-    # Set default variables for missing values
-    if setDefaults :
-        for name, param in _param_registry().items() :
-            if not name in params :
-                params[name] = param.default
+def _toSymbolDict(params: Dict[str, Any]):
+    """Replace names with actual params as key when possible"""
+    all_params = _param_registry().as_dict()
+    return {all_params[name] if name in all_params else Symbol(name): val for name, val in params.items()}
 
-    res = dict()
+
+def _compute_param_length(params):
+    # Check length of parameter values
+    param_length = 1
     for key, val in params.items():
-        if key in _param_registry():
-            param = _param_registry()[key]
-        else:
-            raise Exception("Parameter not found : %s. Valid parameters : %s" % (key, list(_param_registry().keys())))
+        if isinstance(val, (list, np.ndarray)):
+            if param_length == 1:
+                param_length = len(val)
+            elif param_length != len(val):
+                raise Exception("Parameters should be a single value or a list of same number of values")
+    return param_length
+
 
-        if isinstance(val, list):
+def _expand_params(param_values: Dict[str, ParamValues]):
+    res = dict()
+
+    # Expand enum values
+    for key, val in list(param_values.items()):
+        param = _param_registry()[key]
+
+        if isinstance(val, (list, np.ndarray)):
             newvals = [param.expandParams(val) for val in val]
             res.update(_listOfDictToDictOflist(newvals))
         else:
             res.update(param.expandParams(val))
+
+    # Expand single values to lists of values of same size
+    param_length = _compute_param_length(res)
+    if param_length > 1:
+        for key, val in list(res.items()):
+            if not isinstance(val, (list, np.ndarray)):
+                val = list([val] * param_length)
+            res[key] = np.array(val, float)
+
     return res
 
 
+def _complete_params(params: Dict[str, ParamValues], required_params):
+    params = params.copy()
+
+    # Add default values for required params
+    for param_name in required_params:
+        param = _param_registry()[param_name]
+
+        if param_name not in params:
+            if param.formula:
+                params[param_name] = compute_expr_value(param.formula, params)
+                logger.info(f"Param {param_name} was not set. Computing its value from formula :  {params[param_name]}")
+            else:
+                params[param_name] = param.default
+                logger.info("Required param '%s' was missing, replacing by default value : %s" % (param_name, str(param.default)))
+
+    return params
+
+
+def _complete_and_expand_params(params: Dict[str, ParamValues], required_params: List[str] = None, asSymbols=True):
+    """
+    Check parameters and expand enum params.
+    Also transform single values to list of param values of same size and compute formulas of missing params.
+
+    Returns
+    -------
+        Dict of param_name => float value or np.arary of float values
+    """
+    if required_params:
+        params = _complete_params(params, required_params)
+
+    # Expand enum values and list of values
+    params = _expand_params(params)
+
+    # Replace param name with full symbols
+    if asSymbols:
+        params = _toSymbolDict(params)
+
+    return params
+
+
 def resetParams(db_name=None):
-    """Clear parameters in live memory (registry) and on disk.
-    Clear either all params (project and all db params) or db params from a single database (if db_name provided)"""
+    """
+    Clear parameters in live memory (registry) and on disk.
+    Clear either all params (project and all db params) or db params from a single database (if db_name provided).
+
+    This is a good practice in your code to start fresh, cleaning your foreground database and parameters and redefine all
+    programmatically at the start. This ensures the state of the projet / database is always in sync your code and your session
+    / in memory.
+
+    """
     _param_registry().clear(db_name)
 
-    if db_name is None :
+    if db_name is None:
         ProjectParameter.delete().execute()
         ActivityParameter.delete().execute()
         DatabaseParameter.delete().execute()
-    else :
+    else:
         ActivityParameter.delete().where(ActivityParameter.database == db_name).execute()
         DatabaseParameter.delete().where(DatabaseParameter.database == db_name).execute()
         Group.delete().execute()
 
-class NameType(Enum) :
-    NAME="name"
-    LABEL="label"
+
+class NameType(Enum):
+    NAME = "name"
+    LABEL = "label"
     CAMEL_NAME = "CAMEL_NAME"
 
-def _param_name(param, name_type:NameType) :
-    if name_type == NameType.NAME :
+
+def _param_name(param, name_type: NameType):
+    if name_type == NameType.NAME:
         return param.name
-    elif name_type == NameType.LABEL :
+    elif name_type == NameType.LABEL:
         return param.get_label()
-    else :
+    else:
         return _snake2camel(param.name)
 
-def list_parameters(name_type=NameType.NAME):
 
-    """ Print a pretty list of all defined parameters """
-    params = [dict(
-        group=param.group or "",
-        name=_param_name(param, name_type),
-        label=param.get_label(),
-        default=param.default,
-        min=param.min,
-        max=param.max,
-        std=getattr(param, "std", None),
-        distrib=param.distrib,
-        unit=param.unit,
-        db=param.dbname or "[project]") for  param in _param_registry().all()]
+def list_parameters(name_type=NameType.NAME, as_dataframe=False):
+    """Prints a pretty list of all defined parameters
+
+    Parameters
+    ----------
+    as_dataframe:
+        If true, a pandas *Dataframe* is returned. Otherwise, an HTML table is generated.
+    """
+    params = [
+        dict(
+            group=param.group or "",
+            name=_param_name(param, name_type),
+            label=param.get_label(),
+            default=param.default,
+            min=param.min,
+            max=param.max,
+            std=getattr(param, "std", None),
+            distrib=param.distrib,
+            unit=param.unit,
+            db=param.dbname or "[project]",
+        )
+        for param in _param_registry().all()
+    ]
 
     groups = list({p["group"] for p in params})
     groups = sorted(groups)
 
     # Sort by Group / name
-    def keyf(param) :
+    def keyf(param):
         return (groups.index(param["group"]), param["name"])
 
     sorted_params = sorted(params, key=keyf)
 
-    return HTML(tabulate(sorted_params, tablefmt="html", headers="keys"))
+    if as_dataframe:
+        return pd.DataFrame(sorted_params)
+    else:
+        return HTML(tabulate(sorted_params, tablefmt="html", headers="keys"))
+
+
+def compute_expr_value(expr: Expr, param_values: Dict):
+    """Compute value of an expression for given set of parameter values"""
+    free_symbols = [str(symbol) for symbol in expr.free_symbols]
+    lambd = lambdify(free_symbols, expr)
 
+    required_params = _expanded_names_to_names(free_symbols)
 
-def freezeParams(db_name, **params) :
+    values = _complete_and_expand_params(param_values, required_params=required_params, asSymbols=False)
+
+    # Filter only required params
+    values = {name: val for name, val in values.items() if name in free_symbols}
+
+    return lambd(**values)
+    # return expr.evalf(subs=_completeParamValues(param_values, required_params=required_params))
+
+
+def freezeParams(db_name, **params: Dict[str, float]):
     """
-    Freeze parameters values in all exchanges amounts of a DB.
+    Freezes amounts in all exchanges for a given set of parameter values.
     The formulas are computed and the 'amount' attributes are set with the result.
-    This enables parametric datasets to be used by standard, non parametric tools of Brightway2.
+
+    This enables parametric datasets to be used by standard, non-parametric tools of Brightway2 (like Activities browser).
+
+    Parameters
+    ----------
+    db_name :
+        Name of the database for freeze (your foreground db usually)
+
+    params:
+        All other parameters of this function are threated as the values of *lca_algebraic* parameters
+
+    Examples
+    --------
+
+    >>> freezeParams("USER_DB", p1=0.1, p2=3.0)
+
     """
 
     db = bw.Database(db_name)
 
-    with DbContext(db) :
-        for act in db :
+    with DbContext(db):
+        for act in db:
             for exc in act.exchanges():
-
                 amount = _getAmountOrFormula(exc)
 
                 # Amount is a formula ?
-                if isinstance(amount, Basic):
-
-                    replace = [(name, value) for name, value in _completeParamValues(params, setDefaults=True).items()]
-                    val = amount.subs(replace).evalf()
+                if isinstance(amount, Expr):
+                    val = compute_expr_value(amount, params)
 
-                    with ExceptionContext(val) :
+                    with ExceptionContext(val):
                         val = float(val)
 
-                    print("Freezing %s // %s : %s => %d" % (act, exc['name'], amount, val))
+                    print("Freezing %s // %s : %s => %0.2f" % (act, exc["name"], amount, val))
 
                     # Update in DB
                     exc["amount"] = val
                     exc.save()
 
 
 def _listParams(db_name) -> List[ParamDef]:
     """
     Return a set of all parameters used in activities
     """
 
     db = bw.Database(db_name)
     res = set()
 
-    with DbContext(db) :
-        for act in db :
+    with DbContext(db):
+        for act in db:
             for exc in act.exchanges():
-
                 amount = _getAmountOrFormula(exc)
 
                 # Amount is a formula ?
                 if isinstance(amount, Basic):
                     expanded_names = list(str(symbol) for symbol in amount.free_symbols)
                     param_names = _expanded_names_to_names(expanded_names)
                     params = list(_param_registry()[param_name] for param_name in param_names)
                     res.update(params)
     return res
 
 
-def _expand_param_names(param_names):
-    '''Expand parameters names (with enum params) '''
+def _expand_param_names(param_names: List[str]) -> List[str]:
+    """Expand parameters names (with enum params)"""
     return [name for key in param_names for name in _param_registry()[key].names()]
 
 
 def _expanded_names_to_names(param_names):
     """Find params corresponding to expanded names, including enums."""
     param_names = set(param_names)
 
     # param name => param
     res = dict()
 
     # Search for param with same name of prefix paramName_enumValue
-    for expended_name in param_names :
+    for expended_name in param_names:
         for param_name in _param_registry().keys():
-            if expended_name.startswith(param_name) :
+            if expended_name.startswith(param_name):
                 param = _param_registry()[param_name]
                 for name in param.names():
                     if name == expended_name:
                         res[expended_name] = param
 
     missing = param_names - set(res.keys())
     if len(missing) > 0:
         raise Exception("Unkown params : %s" % missing)
 
     return {param.name for param in res.values()}
+
+
+def _parse_formula(formula):
+    local_dict = {x[0].name: x[0] for x in _user_functions.values()}
+    return parse_expr(formula, local_dict=local_dict | _param_registry().as_dict())
+
+
+def _getAmountOrFormula(ex: ExchangeDataset) -> Union[Basic, float]:
+    """Return either a fixed float value or an expression for the amount of this exchange"""
+    if "formula" in ex:
+        try:
+            return _parse_formula(ex["formula"])
+        except Exception:
+            warn("Error while parsing formula '%s' : backing to amount" % ex["formula"])
+
+    return ex["amount"]
+
+
+def switchValue(param: EnumParam, **values: Dict[str, ValueOrExpression]):
+    """
+
+    Helper method defining an expression that returns a different value / formula for each possible choice of an anum param.
+
+    Parameters
+    ----------
+    param: EnumParam
+        The enum param
+
+    values: Dict[str, ValueOrExpression]
+        Each param should correspond to a valid choice of the num parameter.
+
+
+    Examples
+    --------
+
+    Given the enum parameter *p1* :
+
+    >>> p1 = newEnumParam("p1", values=["choice1", "choice2", "choice3"])
+
+    The following code defines an expression worth 0.1 for *choice1*, 0.2 for *choice2*  and *4 x p2* for *choice3*
+
+    >>> amount = switchValue(p1, choice1=0.1, choice2=0.2, choice3=4*p2)
+
+    """
+
+    res = 0
+    for key, val in values.items():
+        res += param.symbol(key) * val
+    return res
```

### Comparing `lca_algebraic-1.0.5/lca_algebraic/stats.py` & `lca_algebraic-1.1/lca_algebraic/stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,135 @@
 import math
 import random
 import warnings
+from collections import defaultdict
 from time import time
-from typing import Type, Dict, Tuple, List
+from typing import List, Tuple, Type
 
 import numpy as np
 import seaborn as sns
-from SALib.analyze import sobol
-from SALib.sample import saltelli, sobol_sequence
+from bw2data.backends.peewee import Activity
+from IPython.display import display
 from ipywidgets import interact
-from jinja2.nodes import Add
 from matplotlib import pyplot as plt
 from matplotlib.lines import Line2D
-from numpy import piecewise
-from sympy import Float, Number, Add, AtomicExpr, Mul, Expr, Function, Abs, Sum, Eq, Piecewise
-from sympy.core import symbol
+from SALib.analyze import sobol as analyse_sobol
+from SALib.sample import sobol, sobol_sequence
+from sympy import (
+    Abs,
+    Add,
+    AtomicExpr,
+    Eq,
+    Expr,
+    Float,
+    Mul,
+    Number,
+    Piecewise,
+    Sum,
+    simplify,
+    symbols,
+)
 from sympy.core.operations import AssocOp
 
-from .base_utils import _method_unit
-from .lca import *
-from .lca import _expanded_names_to_names, _filter_param_values, _replace_fixed_params, _modelToExpr, _preMultiLCAAlgebric, _postMultiLCAAlgebric
-from .params import _variable_params, _param_registry, FixedParamMode, _param_name
+from . import ValueOrExpression, method_name
+from .base_utils import _display_tabs, displayWithExportButton, r_squared
+from .database import DbContext, with_db_context
+from .lca import (
+    Dict,
+    LambdaWithParamNames,
+    Symbol,
+    _expanded_names_to_names,
+    _filter_param_values,
+    _modelToExpr,
+    _postMultiLCAAlgebric,
+    _preMultiLCAAlgebric,
+    _replace_fixed_params,
+    compute_impacts,
+    concurrent,
+    lambdify,
+    pd,
+)
+from .log import warn
+from .methods import method_unit
+from .params import (
+    FixedParamMode,
+    NameType,
+    ParamDef,
+    ParamType,
+    _complete_and_expand_params,
+    _param_name,
+    _param_registry,
+    _variable_params,
+)
 
-PARALLEL=False
+PARALLEL = False
+DEFAULT_N = 1024
 
-def _parallel_map(f, items) :
-    if PARALLEL :
+
+def _parallel_map(f, items):
+    if PARALLEL:
         with concurrent.futures.ThreadPoolExecutor() as exec:
             return exec.map(f, items)
-    else :
+    else:
         return map(f, items)
 
 
 def _heatmap(df, title, vmax, ints=False):
-    ''' Produce heatmap of a dataframe'''
+    """Produce heatmap of a dataframe"""
     fig, ax = plt.subplots(figsize=(17, 17))
-    sns.heatmap(df.transpose(), cmap="gist_heat_r", vmax=vmax, annot=True, fmt='.0f' if ints else '.2f', square=True)
+    sns.heatmap(
+        df.transpose(),
+        cmap="gist_heat_r",
+        vmax=vmax,
+        annot=True,
+        fmt=".0f" if ints else ".2f",
+        square=True,
+    )
     plt.title(title, fontsize=20)
     plt.yticks(rotation=0)
     ax.tick_params(axis="x", labelsize=18)
     ax.tick_params(axis="y", labelsize=18)
 
 
 def _extract_var_params(lambdas):
     required_param_names = set()
-    for lamb in lambdas :
+    for lamb in lambdas:
         required_param_names.update(_expanded_names_to_names(lamb.expanded_params))
     var_params = _variable_params(required_param_names)
     return sorted(var_params.values(), key=lambda p: (p.group if p.group else "", p.name))
 
 
 @with_db_context(arg="model")
-def oat_matrix(model, impacts, n=10, title='Impact variability (% of mean)', name_type=NameType.LABEL):
-    '''Generates a heatmap of the incertitude of the model, varying input parameters one a a time.'''
+def oat_matrix(
+    model: Activity,
+    impacts,
+    functional_unit: ValueOrExpression = 1,
+    n=10,
+    title="Impact variability (% of mean)",
+    name_type=NameType.LABEL,
+):
+    """
+
+    This function generates a heat map of relative the variance of impacts
+    for each parameter varying along its min/max values.
+
+    Parameters
+    ----------
+    model:
+        Root activity of the inventory
+
+    impacts:
+        Impact variabilityList of impact methods keys (tuples)
+
+    functional_unit:
+        Float value of expression by which to divide each impact.
+    """
 
     # Compile model into lambda functions for fast LCA
-    lambdas = _preMultiLCAAlgebric(model, impacts)
+    lambdas = _preMultiLCAAlgebric(model, impacts, alpha=1 / functional_unit)
 
     # Sort params by category
     sorted_params = _extract_var_params(lambdas)
 
     change = np.zeros((len(sorted_params), len(impacts)))
 
     for iparam, param in enumerate(sorted_params):
@@ -70,198 +140,207 @@
 
         # Compute LCA
         df = _postMultiLCAAlgebric(impacts, lambdas, **params)
 
         # Compute change
         change[iparam] = (df.max() - df.min()) / df.median() * 100
 
-
-
     # Build final heatmap
-    change = pd.DataFrame(change,
-                index=[_param_name(param, name_type) for param in sorted_params],
-                columns=[method_name(imp) for imp in impacts])
+    change = pd.DataFrame(
+        change,
+        index=[_param_name(param, name_type) for param in sorted_params],
+        columns=[method_name(imp) for imp in impacts],
+    )
     _heatmap(change.transpose(), title, 100, ints=True)
 
 
-def _display_tabs(titlesAndContentF):
-    """Generate tabs"""
-    tabs = []
-    titles = []
-    for title, content_f in titlesAndContentF:
-        titles.append(title)
-
-        tab = widgets.Output()
-        with tab:
-            content_f()
-        tabs.append(tab)
-
-    res = widgets.Tab(children=tabs)
-    for i, title in enumerate(titles):
-        res.set_title(i, title)
-    display(res)
-
-
-def oat_dasboard(modelOrLambdas, impacts, varying_param: ParamDef, n=10, all_param_names=None,
-                 figsize=(15, 15), figspace=(0.5, 0.5), sharex=True, cols=3, func_unit="kWh"):
-    '''
-    Analyse the evolution of impacts for a single parameter. The other parameters are set to their default values.
-    The result heatmap shows percentage of variation relative to median value.
-
-    Parameters
-    ----------
-    model : activity, or lambdas as precomputed by preMultiLCAAlgebric, for faster computation
-    impacts : set of methods
-    param: parameter to analyse
-    n: number of samples of the parameter
-    figsize: Size of figure fro graphs : (15, 15 by default)
-    figspace: Space between figures for graphs : (0.5, 0.5) by default
-    sharex: Shared X axes ? True by default
-    '''
-
-    if all_param_names == None:
+def _oat_dasboard(
+    model,
+    impacts,
+    varying_param: ParamDef = None,
+    n=10,
+    all_param_names=None,
+    figsize=(15, 15),
+    figspace=(0.5, 0.5),
+    sharex=True,
+    cols=3,
+    func_unit_name="kWh",
+):
+    if all_param_names is None:
         all_param_names = _param_registry().keys()
 
     params = {name: _param_registry()[name].default for name in all_param_names}
 
     # Compute range of values for given param
     params[varying_param.name] = varying_param.range(n)
 
     # print("Params: ", params)
 
-    if isinstance(modelOrLambdas, Activity):
-        with DbContext(modelOrLambdas) :
-            df = multiLCAAlgebric(modelOrLambdas, impacts, **params)
+    if isinstance(model, Activity):
+        with DbContext(model):
+            df = compute_impacts(model, impacts, **params)
     else:
-        df = _postMultiLCAAlgebric(impacts, modelOrLambdas, **params)
+        df = _postMultiLCAAlgebric(impacts, model, **params)
 
     # Add X values in the table
     pname = varying_param.name
     if varying_param.unit:
-        pname = '%s [%s]' % (pname, varying_param.unit)
+        pname = "%s [%s]" % (pname, varying_param.unit)
     df.insert(0, pname, varying_param.range(n))
     df = df.set_index(pname)
 
     def table():
         displayWithExportButton(df)
 
     def graph():
-
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
             nb_rows = int(math.ceil(len(impacts) / cols))
 
             fig, axes = plt.subplots(figsize=figsize)
             plt.subplots_adjust(None, None, None, None, figspace[0], figspace[1])
 
             axes = df.plot(
-                ax=axes, sharex=sharex, subplots=True,
+                ax=axes,
+                sharex=sharex,
+                subplots=True,
                 layout=(nb_rows, cols),
                 # legend=None,
-                kind='line' if varying_param.type == ParamType.FLOAT else 'bar')
+                kind="line" if varying_param.type == ParamType.FLOAT else "bar",
+            )
 
             axes = axes.flatten()
 
             for ax, impact in zip(axes, impacts):
                 ax.set_ylim(ymin=0)
-                unit = _method_unit(impact) + " / " + func_unit
+                unit = method_unit(impact) + " / " + func_unit_name
                 ax.set_ylabel(unit, fontsize=15)
                 ax.set_xlabel(pname, fontsize=15)
 
             plt.show(fig)
 
     def change():
-
         ch = (df.max() - df.min()) / df.median() * 100
         fig, ax = plt.subplots(figsize=(9, 6))
-        plt.title('Relative change for %s' % df.index.name)
-        ch.plot(kind='barh', rot=30)
-        ax.set_xlabel('Relative change of the median value (%)')
+        plt.title("Relative change for %s" % df.index.name)
+        ch.plot(kind="barh", rot=30)
+        ax.set_xlabel("Relative change of the median value (%)")
         plt.tight_layout()
         plt.show(fig)
 
-    _display_tabs([
-        ("Graphs", graph),
-        ("Data", table),
-        ("Variation", change)
-    ])
+    _display_tabs({"Graphs": graph, "Data": table, "Variation": change})
+
 
 @with_db_context(arg="model")
-def oat_dashboard_interact(model, methods, **kwparams):
-    '''Interactive dashboard, with a dropdown for selecting parameter
+def oat_dashboard(model, impacts, functional_unit: ValueOrExpression = 1, func_unit_name="kWh", **kwparams):
+    """
+    This function runs a "one at a time" analysis on the selected param.
+
+    It makes each parameter vary on its min:max range, while keeping other parameters at their default values.
+
+    It returns an interactive dashboard.
 
     Parameters
     ----------
-    figsize: Size of figure fro graphs : (15, 15 by default)
-    figspace: Space between figures for graphs : (0.5, 0.5) by default
-    sharex: Shared X axes ? True by default
-    '''
 
-    lambdas = _preMultiLCAAlgebric(model, methods)
+    model :
+        Root activity of the inventory
+
+    methods :
+        List of methods keys (tuple)
+
+    functional_unit:
+        Value of sympy expression by which to divide the impacts
+
+    func_unit_name:
+        Name of the physical unit of the functional unit, for display
+
+    figsize:
+        Size of figure fro graphs : (15, 15 by default)
+    figspace:
+        Space between figures for graphs : (0.5, 0.5) by default
+    sharex:
+        Shared X axes ? True by default
+
+    Returns
+    -------
+
+    An interactive dashboard with selection of a parameter and graphs of impacts.
+
+    """
+
+    lambdas = _preMultiLCAAlgebric(model, impacts, alpha=1 / functional_unit)
 
     def process_func(param):
         with DbContext(model):
-            oat_dasboard(lambdas, methods, _param_registry()[param], **kwparams)
+            _oat_dasboard(
+                model=lambdas, impacts=impacts, varying_param=_param_registry()[param], func_unit_name=func_unit_name, **kwparams
+            )
 
     param_list = _expanded_names_to_names(lambdas[0].expanded_params)
     param_list = list(_variable_params(param_list).keys())
 
     interact(process_func, param=param_list)
 
 
-class StochasticMethod :
+class StochasticMethod:
     SALTELLI = "saltelli"
     RAND = "rand"
-    SOBOL="sobol"
+    SOBOL = "sobol"
 
 
 def _stochastics(
-        modelOrLambdas, methods, n=1000,
-        var_params=None, sample_method=StochasticMethod.SALTELLI,
-        **extra_fixed_params):
-
+    modelOrLambdas,
+    methods,
+    n=DEFAULT_N,
+    var_params=None,
+    sample_method=StochasticMethod.SALTELLI,
+    functional_unit=1,
+    **extra_fixed_params,
+):
     params, problem = _generate_random_params(n, sample_method, var_params)
 
     # Fix other params
-    if extra_fixed_params :
+    if extra_fixed_params:
         params.update(extra_fixed_params)
 
-    Y = _compute_stochastics(modelOrLambdas, methods , params)
+    Y = _compute_stochastics(modelOrLambdas, methods, params=params, functional_unit=functional_unit)
 
     return problem, params, Y
 
 
-def _compute_stochastics(modelOrLambdas, methods, params):
+def _compute_stochastics(modelOrLambdas, methods, functional_unit=1, params=dict()):
     if isinstance(modelOrLambdas, Activity):
-        Y = multiLCAAlgebric(modelOrLambdas, methods, **params)
+        Y = compute_impacts(modelOrLambdas, methods, functional_unit=functional_unit, **params)
     else:
         Y = _postMultiLCAAlgebric(methods, modelOrLambdas, **params)
     return Y
 
-def _generate_random_params(n, sample_method=StochasticMethod.SALTELLI, var_params=None, seed=None):
 
-    ''' Compute stochastic impacts for later analysis of incertitude '''
+def _generate_random_params(n, sample_method=StochasticMethod.SALTELLI, var_params=None, seed=None):
+    """Compute stochastic impacts for later analysis of incertitude"""
     if var_params is None:
         var_params = _variable_params().values()
 
-    if seed is None :
+    if seed is None:
         seed = int(time() * 1000)
 
     random.seed(seed)
 
     # Extract variable names
     var_param_names = list([param if isinstance(param, str) else param.name for param in var_params])
     problem = {
-        'num_vars': len(var_param_names),
-        'names': var_param_names,
-        'bounds': [[0, 1]] * len(var_param_names)}
+        "num_vars": len(var_param_names),
+        "names": var_param_names,
+        "bounds": [[0, 1]] * len(var_param_names),
+    }
     print("Generating samples ...")
     if sample_method == StochasticMethod.SALTELLI:
-        X = saltelli.sample(problem, n, calc_second_order=True)
+        X = sobol.sample(problem, n, calc_second_order=True)
     elif sample_method == StochasticMethod.RAND:
         X = np.random.rand(n, len(var_param_names))
     elif sample_method == StochasticMethod.SOBOL:
         X = sobol_sequence.sample(n * (len(var_param_names) * 2 + 2), len(var_param_names))
     # elif sample_method == StochasticMethod.LATIN :
     #    X = latin.sample(problem, n)
     else:
@@ -277,569 +356,654 @@
     for param in _param_registry().values():
         if param.name not in var_param_names:
             params[param.name] = param.default
 
     return params, problem
 
 
-class SobolResults :
-
+class SobolResults:
     def __init__(self, s1, s2, st, s1_conf=None, s2_conf=None, st_conf=None):
         self.s1 = s1
         self.s2 = s2
         self.st = st
         self.s1_conf = s1_conf
         self.s2_conf = s2_conf
         self.st_conf = st_conf
 
 
-def _sobols(methods, problem, Y) -> SobolResults :
-    ''' Computes sobols indices'''
-    s1 = np.zeros((len(problem['names']), len(methods)))
-    s1_conf = np.zeros((len(problem['names']), len(methods)))
-    s2 = np.zeros((len(problem['names']), len(problem['names']), len(methods)))
-    s2_conf = np.zeros((len(problem['names']), len(problem['names']), len(methods)))
-    st = np.zeros((len(problem['names']), len(methods)))
-    st_conf = np.zeros((len(problem['names']), len(methods)))
+def _sobols(methods, problem, Y) -> SobolResults:
+    """Computes sobols indices"""
+    s1 = np.zeros((len(problem["names"]), len(methods)))
+    s1_conf = np.zeros((len(problem["names"]), len(methods)))
+    s2 = np.zeros((len(problem["names"]), len(problem["names"]), len(methods)))
+    s2_conf = np.zeros((len(problem["names"]), len(problem["names"]), len(methods)))
+    st = np.zeros((len(problem["names"]), len(methods)))
+    st_conf = np.zeros((len(problem["names"]), len(methods)))
 
-    def process(args) :
+    def process(args):
         imethod, method = args
 
         print("Processing sobol for " + str(method))
         y = Y[Y.columns[imethod]]
-        res = sobol.analyze(problem, y.to_numpy(), calc_second_order=True)
+        res = analyse_sobol.analyze(problem, y.to_numpy(), calc_second_order=True)
         return imethod, res
 
     for imethod, res in _parallel_map(process, enumerate(methods)):
         try:
             s1[:, imethod] = res["S1"]
             s1_conf[:, imethod] = res["S1_conf"]
             s2_ = np.nan_to_num(res["S2"])
             s2_conf_ = np.nan_to_num(res["S2_conf"])
             s2[:, :, imethod] = s2_ + np.transpose(s2_)
             s2_conf[:, :, imethod] = s2_conf_ + np.transpose(s2_conf_)
             st[:, imethod] = res["ST"]
             st_conf[:, imethod] = res["ST_conf"]
 
         except Exception as e:
-            error("Sobol failed on %s" % imethod[2], e)
+            warn("Sobol failed on %s" % imethod[2], e)
 
     return SobolResults(s1, s2, st, s1_conf, s2_conf, st_conf)
 
 
-
-
-
 def _incer_stochastic_matrix(methods, param_names, Y, sob, name_type=NameType.LABEL):
-    ''' Internal method computing matrix of parameter importance '''
-
-
+    """Internal method computing matrix of parameter importance"""
 
     def draw(indice, mode):
-        '''
+        """
         Mode comes as ('s1' || 'st', 'raw' || 'percent')
-        '''
+        """
 
         sx = sob.s1 if indice == "s1" else sob.st
-        if mode == 'raw':
+        if mode == "raw":
             data = sx
         else:
             # If percent, express result as percentage of standard deviation / mean
             data = np.zeros((len(param_names), len(methods)))
             for i, method in enumerate(methods):
                 # Total variance
                 var = np.var(Y[Y.columns[i]])
                 mean = np.mean(Y[Y.columns[i]])
                 if mean != 0:
                     data[:, i] = np.sqrt((sx[:, i] * var)) / mean * 100
 
         param_labels = [_param_name(_param_registry()[name], name_type) for name in param_names]
-        df = pd.DataFrame(data, index=param_labels, columns=[method_name(method) for method in methods])
+        df = pd.DataFrame(
+            data,
+            index=param_labels,
+            columns=[method_name(method) for method in methods],
+        )
         _heatmap(
             df.transpose(),
-            title="Relative deviation of impacts (%)" if mode == 'percent' else "Sobol indices (part of variability)",
-            vmax=100 if mode == 'percent' else 1,
-            ints=mode == 'percent')
-
-    interact(draw,
-             indice=['s1', 'st'],
-             mode=[
-                 ('Raw indices', 'raw'),
-                 ('Relative to mean (%)', 'percent')]
-             )
+            title="Relative deviation of impacts (%)" if mode == "percent" else "Sobol indices (part of variability)",
+            vmax=100 if mode == "percent" else 1,
+            ints=mode == "percent",
+        )
+
+    interact(
+        draw,
+        indice=["s1", "st"],
+        mode=[("Raw indices", "raw"), ("Relative to mean (%)", "percent")],
+    )
+
 
 @with_db_context(arg="model")
-def incer_stochastic_matrix(model, methods, n=1000, name_type=NameType.LABEL):
-    '''
+def incer_stochastic_matrix(model, methods, functional_unit=1, n=DEFAULT_N, name_type=NameType.LABEL):
+    """
     Method computing matrix of parameter importance
 
     parameters
     ----------
     var_params: Optional list of parameters to vary.
     By default use all the parameters with distribution not FIXED
-    '''
+    """
 
-    lambdas = _preMultiLCAAlgebric(model, methods)
+    lambdas = _preMultiLCAAlgebric(model, methods, alpha=1 / functional_unit)
     var_params = _extract_var_params(lambdas)
 
     problem, _, Y = _stochastics(lambdas, methods, n, var_params)
 
     print("Processing Sobol indices ...")
     sob = _sobols(methods, problem, Y)
 
-    _incer_stochastic_matrix(methods, problem['names'], Y, sob, name_type=name_type)
+    _incer_stochastic_matrix(methods, problem["names"], Y, sob, name_type=name_type)
 
 
 def _incer_stochastic_violin(methods, Y, figsize=(15, 15), figspace=(0.5, 0.5), sharex=True, nb_cols=3):
-    ''' Internal method for computing violin graph of impacts
+    """Internal method for computing violin graph of impacts
     Parameters
     ----------
     methods: list of impact methods
     Y : output
     figsize: Size of figure for graphs : (15, 15 by default)
     figspace: Space between figures for graphs : (0.5, 0.5) by default
     sharex: Shared X axes ? True by default
     nb_cols: Number of colums. 3 by default
-    '''
+    """
 
     nb_rows = math.ceil(len(methods) / nb_cols)
     fig, axes = plt.subplots(nb_rows, nb_cols, figsize=figsize, sharex=sharex)
     plt.subplots_adjust(None, None, None, None, figspace[0], figspace[1])
 
     for imethod, method, ax in zip(range(len(methods)), methods, axes.flatten()):
-
         data = Y[Y.columns[imethod]]
         median = np.median(data)
         std = np.std(data)
         mean = np.mean(data)
 
         ax.violinplot(data, showmedians=True)
         ax.title.set_text(method_name(method))
         ax.set_ylim(ymin=0)
-        ax.set_ylabel(_method_unit(method))
+        ax.set_ylabel(method_unit(method))
         ax.set_xticklabels([])
 
         # Add text
-        textstr = '\n'.join((
-            r'$\mu=%.3g$' % (mean,),
-            r'$\mathrm{median}=%.3g$' % (median,),
-            r'$\sigma=%.3g$' % (std,)))
-        props = dict(boxstyle='round', facecolor='wheat', alpha=0.5)
-        ax.text(0.05, 0.95, textstr, transform=ax.transAxes, fontsize=10,
-                verticalalignment='top', bbox=props)
-
-
+        textstr = "\n".join(
+            (
+                r"$\mu=%.3g$" % (mean,),
+                r"$\mathrm{median}=%.3g$" % (median,),
+                r"$\sigma=%.3g$" % (std,),
+            )
+        )
+        props = dict(boxstyle="round", facecolor="wheat", alpha=0.5)
+        ax.text(
+            0.05,
+            0.95,
+            textstr,
+            transform=ax.transAxes,
+            fontsize=10,
+            verticalalignment="top",
+            bbox=props,
+        )
 
-    plt.tick_params(axis='x', which='both', bottom=False, top=False, labelbottom=False)
+    plt.tick_params(axis="x", which="both", bottom=False, top=False, labelbottom=False)
     plt.show(fig)
 
 
 @with_db_context(arg="modelOrLambdas")
-def incer_stochastic_violin(modelOrLambdas, methods, n=1000, var_params=None, **kwparams):
-    '''
+def incer_stochastic_violin(modelOrLambdas, methods, functional_unit=1, n=DEFAULT_N, var_params=None, **kwparams):
+    """
     Method for computing violin graph of impacts
 
     parameters
     ----------
     var_params: Optional list of parameters to vary.
     By default use all the parameters with distribution not FIXED
-    '''
-    _, _, Y = _stochastics(modelOrLambdas, methods, n, var_params)
+    """
+    _, _, Y = _stochastics(
+        modelOrLambdas,
+        methods,
+        n=n,
+        var_params=var_params,
+        functional_unit=functional_unit,
+    )
 
     _incer_stochastic_violin(methods, Y, **kwparams)
 
+
 _percentiles = [10, 90, 25, 50, 75]
+
+
 def _incer_stochastic_variations(methods, param_names, Y, sob1):
-    ''' Method for computing violin graph of impacts '''
+    """Method for computing violin graph of impacts"""
     method_names = [method_name(method) for method in methods]
 
     std = np.std(Y)
     mean = np.mean(Y)
 
-    fig = plt.figure(num=None, figsize=(12, 6), dpi=80, facecolor='w', edgecolor='k')
+    fig = plt.figure(figsize=(12, 6), dpi=80, facecolor="w", edgecolor="k")
     ax = plt.gca()
-    tab20b = plt.get_cmap('tab20b')
-    tab20c = plt.get_cmap('tab20c')
-    ax.set_prop_cycle('color', [tab20b(k) if k < 1 else tab20c(k - 1) for k in np.linspace(0, 2, 40)])
+    tab20b = plt.get_cmap("tab20b")
+    tab20c = plt.get_cmap("tab20c")
+    ax.set_prop_cycle("color", [tab20b(k) if k < 1 else tab20c(k - 1) for k in np.linspace(0, 2, 40)])
 
     relative_variance_pct = std * std / (mean * mean) * 100
     totplt = plt.bar(np.arange(len(method_names)), relative_variance_pct, 0.8)
 
     sum = np.zeros(len(methods))
 
     plots = [totplt[0]]
 
     for i_param, param_name in enumerate(param_names):
-
         s1 = sob1[i_param, :]
 
         curr_bar = s1 * relative_variance_pct
         curr_plt = plt.bar(np.arange(len(method_names)), curr_bar, 0.8, bottom=sum)
         sum += curr_bar
         plots.append(curr_plt[0])
 
-    plt.legend(plots, ['Higher order'] + param_names, loc=(1, 0))
+    plt.legend(plots, ["Higher order"] + param_names, loc=(1, 0))
     plt.xticks(np.arange(len(method_names)), method_names, rotation=90)
     plt.title("variance / mean² (%)")
     plt.show(fig)
 
-def _incer_stochastic_data(methods, param_names, Y, sob1, sobt):
 
-    '''Show full stochastic output with sobol indices'''
-    data = np.zeros((len(param_names) * 2 + len(_percentiles) +2, len(methods)))
-    data[0, :] = np.mean(Y)
-    data[1, :] = np.std(Y)
+def _incer_stochastic_data(methods, param_names, Y, sob1, sobt):
+    """Show full stochastic output with sobol indices"""
+    data = np.zeros((len(param_names) * 2 + len(_percentiles) + 2, len(methods)))
+    data[0, :] = np.mean(Y, 0)
+    data[1, :] = np.std(Y, 0)
 
-    for i, percentile in enumerate(_percentiles) :
+    for i, percentile in enumerate(_percentiles):
         data[2 + i, :] = np.percentile(Y, percentile, axis=0)
 
     for i_param, param_name in enumerate(param_names):
         s1 = sob1[i_param, :]
         data[i_param + 2 + len(_percentiles), :] = s1
         data[i_param + 2 + len(_percentiles) + len(param_names), :] = sobt[i_param, :]
 
-    rows = ["mean", "std"] + \
-           ["p%d" % p for p in _percentiles] + \
-           ["Sobol 1(%s)" % param for param in param_names] + \
-           ["Sobol T(%s)" % param for param in param_names]
+    rows = (
+        ["mean", "std"]
+        + ["p%d" % p for p in _percentiles]
+        + ["Sobol 1(%s)" % param for param in param_names]
+        + ["Sobol T(%s)" % param for param in param_names]
+    )
 
     df = pd.DataFrame(data, index=rows, columns=[method_name(method) for method in methods])
     displayWithExportButton(df)
 
+
 @with_db_context(arg="model")
-def incer_stochastic_dashboard(model, methods, n=1000, var_params=None, **kwparams):
-    ''' Generates a dashboard with several statistics : matrix of parameter incertitude, violin diagrams, ...
+def incer_stochastic_dashboard(
+    model: Activity, methods, n=DEFAULT_N, var_params=None, functional_unit=ValueOrExpression, **kwparams
+):
+    """
+    This function runs a monte carlo & Sobol analysis (GSA) on a parametric model and displays a dashboard with results.
 
-    parameters
+    Parameters
     ----------
-    var_params: Optional list of parameters to vary.
-    By default use all the parameters with distribution not FIXED
-    figsize: Size of figure for violin plots : (15, 15) by default
-    figspace: Space between violin graphs (0.5, 0.5) by default
-    sharex: Share X axe for violin graph : True by default
-    '''
+    model:
+        The root activity of your inventory
+
+    methods:
+        List of impact methods keys (tuples)
+
+    var_params:
+        Optional list of parameters to vary.
+        By default, all the parameters that are not marked as *FIXED* will be varyed.
+
+    functional_unit:
+        Float value or Sympy expression by which to divide the impacts
+
+    figsize:
+        Size of figure for violin plots : (15, 15) by default
+
+    figspace:
+        Space between violin graphs (0.5, 0.5) by default
+
+    sharex:
+        Share X axe for violin graph : True by default
 
-    problem, _, Y = _stochastics(model, methods, n, var_params)
-    param_names = problem['names']
+
+    Returns
+    -------
+    An interactive dashboard with 4 tabs :
+
+    * Violin graphs with distributions of impacts
+    * Bar graph with relative variance of impacts
+    * A heatmap amtrix of Sobol indices for each paramter x impact method
+    * A detailed table with all values
+
+    """
+
+    problem, _, Y = _stochastics(model, methods, n, var_params=var_params, functional_unit=functional_unit)
+
+    param_names = problem["names"]
 
     print("Processing Sobol indices ...")
     sob = _sobols(methods, problem, Y)
 
     def violin():
         _incer_stochastic_violin(methods, Y, **kwparams)
 
     def variation():
         _incer_stochastic_variations(methods, param_names, Y, sob.s1)
 
     def matrix():
-        _incer_stochastic_matrix(methods, problem['names'], Y, sob)
+        _incer_stochastic_matrix(methods, problem["names"], Y, sob)
 
     def data():
-        _incer_stochastic_data(methods, problem['names'], Y, sob.s1, sob.st)
+        _incer_stochastic_data(methods, problem["names"], Y, sob.s1, sob.st)
 
-    _display_tabs([
-        ("Violin graphs", violin),
-        ("Impact variations", variation),
-        ("Sobol matrix", matrix),
-        ("Data", data)
-    ])
+    _display_tabs(
+        {
+            "Violin graphs": violin,
+            "Impact variations": variation,
+            "Sobol matrix": matrix,
+            "Data": data,
+        }
+    )
 
 
 def _round_expr(expr, num_digits):
-    ''' Round all number in sympy expression with n digits'''
-    return expr.xreplace({n : Float(n, num_digits) if isinstance(n, Float) else n for n in expr.atoms(Number)})
+    """Round all number in sympy expression with n digits"""
+
+    return expr.xreplace({n: Float(n, num_digits) if isinstance(n, Float) else n for n in expr.atoms(Number)})
 
-def _snake2camel(val) :
-    return ''.join(word.title() for word in val.split('_'))
 
+def _snake2camel(val):
+    return "".join(word.title() for word in val.split("_"))
 
-def _enum_to_piecewize(exp) :
 
-    def checkEnumSymbol(term) :
-        if not isinstance(term, Symbol) :
+def _enum_to_piecewize(exp):
+    def checkEnumSymbol(term):
+        if not isinstance(term, Symbol):
             return (None, None)
-        if not "_" in term.name :
+        if "_" not in term.name:
             return (None, None)
         enum_name, enum_val = term.name.rsplit("_", 1)
 
-        if not enum_name in _param_registry() :
+        if enum_name not in _param_registry():
             return (None, None)
         return enum_name, enum_val
 
-    def checkEnumProduct(term) :
-
+    def checkEnumProduct(term):
         """If term is enumVal * X return (param, value, X) else return null"""
 
-        if not isinstance(term, Mul) :
+        if not isinstance(term, Mul):
             return (None, None, None)
 
-        if len(term.args) != 2 :
+        if len(term.args) != 2:
             return (None, None, None)
 
         a, b = term.args
 
         name, value = checkEnumSymbol(a)
-        if name is not None :
+        if name is not None:
             return (name, value, b)
 
         name, value = checkEnumSymbol(b)
         if name is not None:
             return (name, value, a)
 
         return (None, None, None)
 
-
-    def _replace_enums(expr) :
+    def _replace_enums(expr):
         # Dict of enum_name -> { enum_value -> ratio }
-        enums = defaultdict(lambda : dict())
+        enums = defaultdict(lambda: dict())
         res_terms = []
 
-        for term in expr.args :
-
+        for term in expr.args:
             name, value, ratio = checkEnumProduct(term)
-            if name is not None :
+            if name is not None:
                 # This is a enum value !
                 enums[name][value] = ratio
-            else :
+            else:
                 # Other term
                 res_terms.append(term)
 
-        if len(enums) == 0 :
+        if len(enums) == 0:
             # No change
             return expr
 
-        for enum_name, ratio_dict in enums.items() :
+        for enum_name, ratio_dict in enums.items():
             choices = [(ratio, Eq(symbols(enum_name), symbols(enum_value))) for enum_value, ratio in ratio_dict.items()]
-            if len(choices) < len(_param_registry()[enum_name].values) :
+            if len(choices) < len(_param_registry()[enum_name].values):
                 # Not all choices covered ? => Add default
                 choices.append((0, True))
 
             res_terms.append(Piecewise(*choices))
 
         return Add(*res_terms)
 
-    return exp.replace(
-        lambda x: isinstance(x, Sum) or isinstance(x, Add),
-        _replace_enums)
-
-def prettify(exp) :
-     """
-     Prettify expression for publication :
-     > change snake_symbols to SnakeSymbols (avoiding lowerscript in Latex)"""
-
-     res = _enum_to_piecewize(exp)
-
-     res = res.replace(
-         lambda x: isinstance(x, Symbol),
-         lambda x: Symbol(_snake2camel(str(x))))
-
-     # Replace absolute values for positive parameters
-     res, nb_match = _replace_abs(res)
-     if nb_match > 0:
-         # It changed => simplify again
-         res = simplify(res)
+    return exp.replace(lambda x: isinstance(x, Sum) or isinstance(x, Add), _replace_enums)
+
+
+def prettify(exp):
+    """
+    Prettify expression for publication :
+    > change snake_symbols to SnakeSymbols (avoiding lowerscript in Latex)"""
+
+    res = _enum_to_piecewize(exp)
 
-     return res
+    res = res.replace(lambda x: isinstance(x, Symbol), lambda x: Symbol(_snake2camel(str(x))))
 
-def _replace_abs(exp) :
-    """Replace |X| by X if X is float param """
+    # Replace absolute values for positive parameters
+    res, nb_match = _replace_abs(res)
+    if nb_match > 0:
+        # It changed => simplify again
+        res = simplify(res)
+
+    return res
+
+
+def _replace_abs(exp):
+    """Replace |X| by X if X is float param"""
 
     nb_match = 0
 
-    def replaceAbs(absExp : Abs) :
+    def replaceAbs(absExp: Abs):
         nonlocal nb_match
-        if len(absExp.args) != 1 :
+        if len(absExp.args) != 1:
             return absExp
         arg = absExp.args[0]
 
-        if not isinstance(arg, Symbol) :
+        if not isinstance(arg, Symbol):
             return absExp
 
         params = _param_registry()
-        if not arg.name in params :
+        if arg.name not in params:
             return absExp
 
         param = params[arg.name]
-        if param.type == ParamType.FLOAT and param.min >= 0 :
+        if param.type == ParamType.FLOAT and param.min >= 0:
             nb_match += 1
             return arg
-        else :
+        else:
             return absExp
 
-    res = exp.replace(
-        lambda x: isinstance(x, Abs),
-        lambda x: replaceAbs(x))
+    res = exp.replace(lambda x: isinstance(x, Abs), lambda x: replaceAbs(x))
 
     return res, nb_match
 
+
 @with_db_context(arg="model")
 def sobol_simplify_model(
-    model, methods,
-    min_ratio=0.8, n=2000, var_params=None,
-    fixed_mode = FixedParamMode.MEDIAN,
+    model: Activity,
+    methods,
+    min_ratio=0.8,
+    functional_unit=1,
+    n=DEFAULT_N * 2,
+    var_params=None,
+    fixed_mode=FixedParamMode.MEDIAN,
     num_digits=3,
     simple_sums=True,
-    simple_products=True) -> List[LambdaWithParamNames]:
-
-    '''
+    simple_products=True,
+) -> List[LambdaWithParamNames]:
+    """
     Computes Sobol indices and selects main parameters for explaining sensibility of at least 'min_ratio',
     Then generates simplified models for those parameters.
 
-    parameters
+    The other parameters are replaced by their mean or median values.
+
+    Also the term contributing to less than 1% of variation in sums and products are removed.
+
+    Decimal numbers are rounded to 3 digits.
+
+    Parameters
     ----------
-    min_ratio: [0, 1] minimum amount of first order variation (sum of S1) to explain
-    var_params: Optional list of parameters to vary.
-    fixed_mode : What to replace minor parameters with : MEDIAN by default
-    sob: [optional] Pre-computed sobol indices
-    simplify_sums: If true (default) remove terms in sums that are lower than 1%
-
-    returns
-    _______
-
-    List of LambdaWithParamNames, one per impact : with wraps the simplified expression together with the
-    list of required parameters and a fast complied lambda function for fast evaluation.
-    '''
+    model:
+        Root activity of the inventory
+
+    methods:
+        List of impact methods to consider
+
+    min_ratio:
+        [0, 1] minimum amount of first order variation (sum of S1) to explain; 0.8 (80%) by default.
+
+    var_params:
+        Optional list of parameters to vary. If not provided, all parameters vary.
+
+    fixed_mode :
+        What to replace minor parameters with : MEDIAN by default
+
+    simple_sums:
+        If true (default) remove terms in sums that are lower than 1%
+
+    simple_products:
+        If true (default) remove terms in products that contribute to less than 1% to variation
+
+    num_digits:
+        Number of decimal places to round decimal number to (default 3)
+
+    Returns
+    -------
+    List of *LambdaWithParamNames*, one per impact.
+    The class *LambdaWithParamNames* wraps the simplified expression together with the
+    list of required parameters and compiled lambda functions for fast evaluation.
+
+    The core simplified expresion may be access with **res[i].expr**
+
+
+    Examples
+    --------
+
+    >>> res = sobol_simplify_model(
+    >>>     model=total_inventory,
+    >>>     methods=[climate_change],
+    >>>     functional_unit=total_energy) # Holds a sympy expression computing the total energy
+
+    >>> print(res[0].expr) # Dispalt the simplified expression
+    """
 
     # Default var param names
-    if var_params is None :
+    if var_params is None:
         var_params = _variable_params().values()
 
     var_param_names = list([param.name for param in var_params])
 
-    problem, params, Y = _stochastics(model, methods, n, var_params)
+    problem, params, Y = _stochastics(model, methods, n, var_params=var_params, functional_unit=functional_unit)
+
     sob = _sobols(methods, problem, Y)
 
     s1, s2 = sob.s1, sob.s2
 
     res = []
 
     # Generate simplified model
-    exprs, _ = _modelToExpr(model, methods)
-
-    for imethod, method in enumerate(methods) :
+    exprs = _modelToExpr(model, methods, alpha=1 / functional_unit)
 
+    for imethod, method in enumerate(methods):
         print("> Method : ", method_name(method))
 
         s1_sum = np.sum(s1[:, imethod])
         s2_sum = np.sum(s2[:, :, imethod]) / 2
-        print('S1: ', s1_sum)
-        print('S2: ', s2_sum)
-        print('ST: ', np.sum(sob.st[:, imethod]))
+        print("S1: ", s1_sum)
+        print("S2: ", s2_sum)
+        print("ST: ", np.sum(sob.st[:, imethod]))
 
         sum = 0
 
         sorted_param_indices = list(range(0, len(var_param_names)))
-        sorted_param_indices = sorted(sorted_param_indices, key=lambda i : s1[i, imethod], reverse=True)
+        sorted_param_indices = sorted(sorted_param_indices, key=lambda i: s1[i, imethod], reverse=True)
         selected_params = []
         sobols = dict()
 
-        for iparam, param in enumerate(sorted_param_indices) :
-
-
+        for iparam, param in enumerate(sorted_param_indices):
             # S1
             sum += s1[param, imethod]
 
             param_name = var_param_names[param]
             selected_params.append(param_name)
             sobols[param_name] = s1[param, imethod]
 
             # S2
-            #for iparam2 in range(0, iparam) :
+            # for iparam2 in range(0, iparam) :
             #    param2 = sorted_param_indices[iparam2]
             #    sum += s2[param, param2, imethod]
 
-            if sum > min_ratio :
+            if sum > min_ratio:
                 break
         print("Selected params : ", selected_params, "explains: ", sum)
 
         expr = exprs[imethod]
 
-        # Replace extra fixed params
-        extraFixedParams = [param for param in _param_registry().values() if param.name not in selected_params]
-        expr = _replace_fixed_params(expr, extraFixedParams, fixed_mode=fixed_mode)
+        # Replace non selected params by their value
+        fixed_params = [param for param in _param_registry().values() if param.name not in selected_params]
+        expr = _replace_fixed_params(expr, fixed_params, fixed_mode=fixed_mode)
 
         # Sympy simplification
         expr = simplify(expr)
 
         # Round numerical values to 3 digits
         expr = _round_expr(expr, num_digits)
 
         # Lambdify the expression
         lambd = LambdaWithParamNames(expr, params=selected_params, sobols=sobols)
 
         # Compute list of parameter values (monte carlo)
-        completed_params = lambd.complete_params(params)
-        expanded_params = _filter_param_values(completed_params, lambd.expanded_params)
+        expanded_params = _complete_and_expand_params(params, lambd.params, asSymbols=False)
+        expanded_params = _filter_param_values(expanded_params, lambd.expanded_params)
 
         # Extra step of simplification : simplify sums with neligeable terms
-        if simple_sums :
+        if simple_sums:
             expr = _simplify_sums(expr, expanded_params)
 
         if simple_products:
             expr = _simplify_products(expr, expanded_params)
 
-
         expr = simplify(expr)
 
         display(prettify(expr))
 
         res.append(LambdaWithParamNames(expr, params=selected_params, sobols=sobols))
 
     return res
 
+
 TERM_MIN_LEVEL = 0.01
 
-def _rec_expression(exp, func) :
-    """ Recurse trough an expression, transforming each term with the result of f(term) """
-    def rec(term) :
+
+def _rec_expression(exp, func):
+    """Recurse trough an expression, transforming each term with the result of f(term)"""
+
+    def rec(term):
         if issubclass(exp.func, AtomicExpr):
             return func(term)
-        else :
+        else:
             args = filter(lambda x: x is not None, list(func(arg) for arg in term.args))
             return term.func(*args)
 
-def _simplify_sums(expr, param_values) :
 
+def _simplify_sums(expr, param_values):
     def replace_term(term, minv, maxv, max_max):
         abs_max = max(abs(minv), abs(maxv))
         if abs_max < (TERM_MIN_LEVEL * max_max):
             return None
         else:
             return term
 
     return _simplify_terms(expr, param_values, Add, replace_term)
 
-def _simplify_products(expr, param_values) :
-
-    def replace_term(term, minv, maxv, max_max) :
 
+def _simplify_products(expr, param_values):
+    def replace_term(term, minv, maxv, max_max):
         # Close to 1 or -1 ?
         for factor in [-1, 1]:
             if abs(minv - factor) < TERM_MIN_LEVEL and abs(maxv - factor) < TERM_MIN_LEVEL:
                 if factor == -1:
                     return -1
                 else:
                     # * 1.0 : remove term
                     return None
 
         return term
 
     return _simplify_terms(expr, param_values, Mul, replace_term)
 
-def _simplify_terms(expr, expanded_param_values, op:Type[AssocOp], replace) :
 
+def _simplify_terms(expr, expanded_param_values, op: Type[AssocOp], replace):
     """Generic simplification of sum or product"""
 
     # Determine max normalized value of this term, for all param values (monte carlo)
-    min_max_cache : Dict[str, Tuple[float, float]] = dict()
-    def min_max(term) :
+    min_max_cache: Dict[str, Tuple[float, float]] = dict()
 
+    def min_max(term):
         # In cache ?
         key = str(term)
-        if key in min_max_cache :
+        if key in min_max_cache:
             return min_max_cache[key]
 
         # Non varying ?
         if len(term.free_symbols) == 0:
             values = [term.evalf()]
         else:
             lambd_term = lambdify(expanded_param_values.keys(), term)
@@ -848,23 +1012,21 @@
         minv = np.min(values)
         maxv = np.max(values)
         min_max_cache[key] = (minv, maxv)
         return (minv, maxv)
 
     # Cleanup :keep only most relevant terms
     def cleanup(exp):
-
         if (not isinstance(exp, Expr)) or issubclass(exp.func, AtomicExpr):
             return exp
 
         # For Op, only select terms than are relevant
-        if exp.func == op :
-
+        if exp.func == op:
             # Compute max of max
-            def abs_max(minv, maxv) :
+            def abs_max(minv, maxv):
                 return max(abs(minv), abs(maxv))
 
             max_max = max([abs_max(*min_max(arg)) for arg in exp.args])
 
             # Only keep term above level
             args = [replace(arg, *min_max(arg), max_max) for arg in exp.args]
         else:
@@ -873,201 +1035,251 @@
         args = [cleanup(arg) for arg in args if arg is not None]
 
         return exp.func(*args)
 
     return cleanup(expr)
 
 
-
-def _hline(x1, x2, y, linewidth=1, linestyle='solid'):
+def _hline(x1, x2, y, linewidth=1, linestyle="solid"):
     ymin, ymax = plt.ylim()
     xmin, xmax = plt.xlim()
     minx = (x1 - xmin) / (xmax - xmin)
     maxx = (x2 - xmin) / (xmax - xmin)
-    plt.axhline(ymax * y, color='k', xmin=minx, xmax=maxx, linewidth=linewidth, linestyle=linestyle)
-
-
-def _vline(x, ymin, ymax, linewidth=1, linestyle='solid'):
-    plt.axvline(x, color='k', ymin=ymin, ymax=ymax, linewidth=linewidth, linestyle=linestyle)
-
-
-def _graph(data, unit, title, ax, alpha=1, textboxtop=0.95, textboxright=0.95, color=None,
-           limit_xrange=False, percentiles=[5,95], fontsize=12):
-
-
+    plt.axhline(
+        ymax * y,
+        color="k",
+        xmin=minx,
+        xmax=maxx,
+        linewidth=linewidth,
+        linestyle=linestyle,
+    )
+
+
+def _vline(x, ymin, ymax, linewidth=1, linestyle="solid"):
+    plt.axvline(x, color="k", ymin=ymin, ymax=ymax, linewidth=linewidth, linestyle=linestyle)
+
+
+def _graph(
+    data,
+    unit,
+    title,
+    ax,
+    alpha=1,
+    textboxtop=0.95,
+    textboxright=0.95,
+    color=None,
+    limit_xrange=False,
+    percentiles=[5, 95],
+    fontsize=12,
+):
     if ax is not None:
         plt.sca(ax)
     else:
         ax = plt.gca()
 
     median = np.median(data)
     std = np.std(data)
     mean = np.mean(data)
-    xmin= np.min(data)
+    xmin = np.min(data)
 
     p9995 = np.percentile(data, 99.95)
 
     pvals = [np.percentile(data, perc) for perc in percentiles]
 
     variability = std / mean
 
     args = dict()
     if color:
-        args['color'] = color
+        args["color"] = color
 
-    if limit_xrange :
+    if limit_xrange:
         plt.xlim(xmin, p9995)
     plt.hist(data, 200, alpha=alpha, **args)
 
-    perc_strs = [r'$p%d=%.3g$' % (p,pval) for p, pval in zip(percentiles, pvals)]
+    perc_strs = [r"$p%d=%.3g$" % (p, pval) for p, pval in zip(percentiles, pvals)]
 
-    textstr = '\n'.join([
-        r'$\mu=%.3g$' % (mean,),
-        r'$\mathrm{median}=%.3g$' % (median,),
-        r'$\sigma=%.3g$' % (std,),
-        r'$\sigma/\mu=%.3g$' % (variability,)
-    ] + perc_strs)
-
-    props = dict(boxstyle='round', facecolor='wheat' if not color else color, alpha=0.5)
-    ax.text(textboxright, textboxtop, textstr, transform=ax.transAxes, fontsize=fontsize,
-            verticalalignment='top', ha='right', bbox=props)
+    textstr = "\n".join(
+        [
+            r"$\mu=%.3g$" % (mean,),
+            r"$\mathrm{median}=%.3g$" % (median,),
+            r"$\sigma=%.3g$" % (std,),
+            r"$\sigma/\mu=%.3g$" % (variability,),
+        ]
+        + perc_strs
+    )
+
+    props = dict(boxstyle="round", facecolor="wheat" if not color else color, alpha=0.5)
+    ax.text(
+        textboxright,
+        textboxtop,
+        textstr,
+        transform=ax.transAxes,
+        fontsize=fontsize,
+        verticalalignment="top",
+        ha="right",
+        bbox=props,
+    )
 
     # Axes
     ax.set_xlabel(unit, dict(fontsize=14))
     ax.set_yticks([])
     ax.set_title(title, dict(fontsize=16))
 
-    return dict(
-        median=median,
-        std=std,
-        p=pvals,
-        mean=mean,
-        var=variability)
-
-def distrib(*args, **kwargs) :
-    """
-       Show distributions together with statistical outcomes
-
-       Synonym of #graphs()
-
-       parameters
-       ----------
-       model: normalized model
-       methods: List of impacts
-       Y: output of processing. If None, monte carlo will be processed again
-       nb_cols : number of colons to display graphs on
-       invert : list of methods for which result should be inverted (1/X). None by default
-       scales : Dict of method => scale, for multiplying results. To be used with unit overrides
-       unit_overrides : Dict of method => string for overriding unit, in respect to custom scales
-       height: Height of graph : 10 inches be default
-       width : Width of graphs : 15 inches by default
-       """
-    return graphs(*args, **kwargs)
+    return dict(median=median, std=std, p=pvals, mean=mean, var=variability)
 
 
-@with_db_context(arg="model")
-def graphs(
-        model, methods,
-        Y=None, nb_cols=1, axes=None, title=None,
-        invert=None,
-        scales=None, # Dict of method => scale
-        unit_overrides=None,
-        height=10, width=15,
-        func_unit="kWh",
-        **kwargs):
+def distrib(
+    model,
+    methods,
+    functional_unit=1,
+    func_unit_name="",
+    Y=None,
+    nb_cols=1,
+    axes=None,
+    title=None,
+    invert=None,
+    scales=None,  # Dict of method => scale
+    unit_overrides=None,
+    height=10,
+    width=15,
+    **kwargs,
+):
     """
     Show distributions together with statistical outcomes
 
+    Synonym of #graphs()
+
     parameters
     ----------
-    model: normalized model
-    methods: List of impacts
-    Y: output of processing. If None, monte carlo will be processed again
-    nb_cols : number of colons to display graphs on
-    invert : list of methods for which result should be inverted (1/X). None by default
-    scales : Dict of method => scale, for multiplying results. To be used with unit overrides
-    unit_overrides : Dict of method => string for overriding unit, in respect to custom scales
-    height: Height of graph : 10 inches be default
-    width : Width of graphs : 15 inches by default
-    """
+    model:
+        Root activity of the onventory
+
+    methods:
+        List of impact methods keys (tuples)
+
+    functional_unit:
+        Value of expression by which to divide the impacts
 
+    func_unit_name:
+        Physical unit name of the fonctional unit
+
+    nb_cols :
+        number of colons to display graphs on
+
+    invert :
+        list of methods for which result should be inverted (1/X). None by default
+
+    scales :
+        Dict of method => scale, for multiplying results. To be used with unit overrides
+
+    unit_overrides :
+        Dict of method => string for overriding unit, in respect to custom scales
+
+    height:
+        Height of graph : 10 inches be default
+    width :
+        Width of graphs : 15 inches by default
+    """
 
     if Y is None:
-        _, _, Y = _stochastics(model, methods, n=10000)
+        _, _, Y = _stochastics(model, methods, n=DEFAULT_N * 16, functional_unit=functional_unit)
 
     if axes is None:
         nb_rows = math.ceil(len(methods) / nb_cols)
         fig, axes = plt.subplots(nb_rows, nb_cols, figsize=(width, height * nb_rows))
 
     if isinstance(axes, np.ndarray):
         axes = axes.flatten()
     else:
         axes = [axes]
 
     plt.subplots_adjust(hspace=0.4)
 
-
-    res=dict()
+    res = dict()
     for i, method, ax in zip(range(len(methods)), methods, axes):
-
         data = Y[Y.columns[i]]
 
         if invert and method in invert:
             data = 1 / data
 
         if scales and method in scales:
             data = data * scales[method]
 
         graph_title = title if title else method_name(method)
 
         if unit_overrides and method in unit_overrides:
             unit = unit_overrides[method]
         else:
-            unit = _method_unit(method)
+            unit = method_unit(method)
 
-        unit += " / " + func_unit
+        unit += " / " + func_unit_name
 
-        stats = _graph(
-            data, unit,
-            graph_title,
-            ax=ax,
-            **kwargs)
+        stats = _graph(data, unit, graph_title, ax=ax, **kwargs)
 
-        res[graph_title + (' [%s]' % unit)] = stats
+        res[graph_title + (" [%s]" % unit)] = stats
 
     for i in range(0, -len(methods) % nb_cols):
         ax = axes.flatten()[-(i + 1)]
         ax.axis("off")
 
     return pd.DataFrame(res)
 
 
 @with_db_context(arg="model")
 def compare_simplified(
-        model, methods, simpl_lambdas,
-        scales=None,  # Dict of method => scale
-        unit_overrides=None,
-        nb_cols=2, height=10, width=15, textboxright=0.6, r2_height=0.65, func_unit="kWh",
-        residuals=False,
-        **kwargs):
-    '''
-    Compare distribution of simplified model with full model
+    model: Activity,
+    methods,
+    simpl_lambdas,
+    functional_unit=1,
+    func_unit_name="",
+    scales=None,  # Dict of method => scale
+    unit_overrides=None,
+    nb_cols=2,
+    height=10,
+    width=15,
+    textboxright=0.6,
+    r2_height=0.65,
+    residuals=False,
+    **kwargs,
+):
+    """
+    Compare distribution of simplified model with full model.
+
+    This functions runs the same monte caarlo random sample as input and feed it to oboth simplified models and full
+    model. It displays graphs and metrics comparing the two.
 
     Parameters
     ----------
-    model: Model
-    residuals : If true, draw heat map of residuals, instead of distributions
-    methods : Impact methods
-    simpl_lambdas : Simplified lambdas, as returned by sobol_simplify_model(...)
-    nb_cols: number of columns for displaying graphs
-    percentiles: List of percentiles to compute [5, 95] by default
-    '''
+    model:
+        Root activity of the inventory
+
+    methods :
+        List of impact methods
+
+    functional_unit:
+        Float value or sympy expression by whicxh to devide the impacts
+
+    func_unit_name:
+        Name of the physical functional unit
+
+    simpl_lambdas :
+        Simplified lambdas, as returned by **sobol_simplify_model(...)**
+
+    residuals :
+        If true, draw heat map of residuals, rather than distributions
+
+    nb_cols:
+        number of columns for displaying graphs
+
+    percentiles:
+        List of percentiles to compute [5, 95] by default
+    """
 
     # Raw model
-    lambdas = _preMultiLCAAlgebric(model, methods)
+    lambdas = _preMultiLCAAlgebric(model, methods, alpha=1 / functional_unit)
 
     nb_rows = math.ceil(len(methods) / nb_cols)
     fig, axes = plt.subplots(nb_rows, nb_cols, figsize=(width, height * nb_rows))
 
     if not isinstance(axes, np.ndarray):
         axes = np.array([axes])
 
@@ -1094,37 +1306,53 @@
         if scales and method in scales:
             d1 = d1 * scales[method]
             d2 = d2 * scales[method]
 
         if unit_overrides and method in unit_overrides:
             unit = unit_overrides[method]
         else:
-            unit = _method_unit(method)
+            unit = method_unit(method)
 
-        unit += " / " + func_unit
+        unit += " / " + func_unit_name
 
-        if residuals :
+        if residuals:
             hb = ax.hexbin(d1, d2, gridsize=(200, 200), mincnt=1)
             cb = fig.colorbar(hb, ax=ax)
 
             xmin, xmax = ax.get_xlim()
             ymin, ymax = ax.get_ylim()
-            vmax= max(ymax, xmax)
-            line = Line2D([0, vmax], [0, vmax], color='grey', linestyle='dashed')
+            vmax = max(ymax, xmax)
+            line = Line2D([0, vmax], [0, vmax], color="grey", linestyle="dashed")
             ax.add_line(line)
             ax.set_xlim(0, vmax)
             ax.set_ylim(0, vmax)
             cb.set_label("Counts")
             ax.set_xlabel("Reference model [%s]" % (unit), dict(fontsize=14))
             ax.set_ylabel("Simplified model [%s]" % (unit), dict(fontsize=14))
             ax.set_title(title, dict(fontsize=16))
 
         else:
             _graph(d1, unit, title, ax=ax, alpha=0.6, color=colors[0], **kwargs)
-            _graph(d2, unit, title, ax=ax, alpha=0.6, textboxright=textboxright, color=colors[1], **kwargs)
-
-        ax.text(0.9, r2_height, "R² : %0.3g" % r_value, transform=ax.transAxes, fontsize=14,
-                verticalalignment='top', ha='right')
+            _graph(
+                d2,
+                unit,
+                title,
+                ax=ax,
+                alpha=0.6,
+                textboxright=textboxright,
+                color=colors[1],
+                **kwargs,
+            )
+
+        ax.text(
+            0.9,
+            r2_height,
+            "R² : %0.3g" % r_value,
+            transform=ax.transAxes,
+            fontsize=14,
+            verticalalignment="top",
+            ha="right",
+        )
 
     # Hide missing graphs
     for i in range(0, -len(methods) % nb_cols):
-        ax = axes.flatten()[-(i + 1)]
+        ax = axes.flatten()[-(i + 1)]
```

### Comparing `lca_algebraic-1.0.5/test/fixtures/__init__.py` & `lca_algebraic-1.1/test/fixtures/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # Defines basic activities and methods for test
 from lca_algebraic import *
+from lca_algebraic import getActByCode, newActivity
 
-def init_acts(db) :
-    """Init bg acts (bio and techno) """
+
+def init_acts(db):
+    """Init bg acts (bio and techno)"""
 
     # Clear DB
     resetDb(db, False)
 
     # Biosphere activities
     bio1 = newActivity(db, "bio1", "unit", type="emission")
     bio2 = newActivity(db, "bio2", "unit", type="emission")
     bio3 = newActivity(db, "bio3", "unit", type="emission")
 
     # Process activities
-    bg_act1 = newActivity(db, "bg_act1", "kg", {
-        bio1 : 1,
-        bio2 : 2
-    })
-    bg_act2 = newActivity(db, "bg_act2", "kg", {
-        bio1 : 2,
-        bio2 : 1
-    })
-    bg_act3 = newActivity(db, "bg_act3", "m3" , {
-        bio3: 1,
-    })
+    bg_act1 = newActivity(db, "bg_act1", "kg", {bio1: 1, bio2: 2})
+    bg_act2 = newActivity(db, "bg_act2", "kg", {bio1: 2, bio2: 1})
+    bg_act3 = newActivity(
+        db,
+        "bg_act3",
+        "m3",
+        {
+            bio3: 1,
+        },
+    )
 
     return bio1, bio2, bio3
 
 
-def init_methods(db, prefix) :
+def init_methods(db, prefix):
     "Create impact methods for bio activities"
     res = []
 
     # One for each bio act
-    for nbio in range(1, 4) :
+    for nbio in range(1, 4):
         bioname = "bio" + str(nbio)
 
         act = getActByCode(db, bioname)
 
-        method = bw.Method((prefix, bioname, 'total'))
-        method.register(
-            unit='MJ-Eq',
-            description='quantity of ' + bioname)
+        method = bw.Method((prefix, bioname, "total"))
+        method.register(unit="MJ-Eq", description="quantity of " + bioname)
         method.write([(act.key, 1)])
 
-        res.append((prefix, bioname, 'total'))
+        res.append((prefix, bioname, "total"))
 
     # Digital : one digit per bio activity
     method = bw.Method((prefix, "all", "total"))
-    method.register(
-        unit='1',
-        description='quantity of ' + bioname)
-    method.write([
-        ((db, "bio1"), 1),
-        ((db, "bio2"), 2),
-        ((db, "bio3"), 4),
-    ])
+    method.register(unit="1", description="quantity of " + bioname)
+    method.write(
+        [
+            ((db, "bio1"), 1),
+            ((db, "bio2"), 2),
+            ((db, "bio3"), 4),
+        ]
+    )
     res.append((prefix, "all", "total"))
 
     return res
```

