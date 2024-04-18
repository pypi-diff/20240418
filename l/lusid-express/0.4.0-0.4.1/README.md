# Comparing `tmp/lusid_express-0.4.0.tar.gz` & `tmp/lusid_express-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.4.0.tar", last modified: Wed Apr 17 21:04:53 2024, max compression
+gzip compressed data, was "lusid_express-0.4.1.tar", last modified: Wed Apr 17 21:16:17 2024, max compression
```

## Comparing `lusid_express-0.4.0.tar` & `lusid_express-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.138337 lusid_express-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-17 21:04:50.000000 lusid_express-0.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-17 21:04:50.000000 lusid_express-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:04:53.138337 lusid_express-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-17 21:04:50.000000 lusid_express-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:04:53.138337 lusid_express-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-17 21:04:50.000000 lusid_express-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.133337 lusid_express-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.136337 lusid_express-0.4.0/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.137337 lusid_express-0.4.0/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.137337 lusid_express-0.4.0/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.137337 lusid_express-0.4.0/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     5831 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-04-17 21:04:50.000000 lusid_express-0.4.0/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:04:53.137337 lusid_express-0.4.0/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:04:53.000000 lusid_express-0.4.0/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-17 21:04:53.000000 lusid_express-0.4.0/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:04:53.000000 lusid_express-0.4.0/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 21:04:53.000000 lusid_express-0.4.0/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 21:04:53.000000 lusid_express-0.4.0/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.890872 lusid_express-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-17 21:16:15.000000 lusid_express-0.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-17 21:16:15.000000 lusid_express-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:16:17.890872 lusid_express-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-17 21:16:15.000000 lusid_express-0.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:16:17.890872 lusid_express-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-17 21:16:15.000000 lusid_express-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.886872 lusid_express-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.888872 lusid_express-0.4.1/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     5995 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.4.0/LICENSE` & `lusid_express-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/PKG-INFO` & `lusid_express-0.4.1/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid_express
-Version: 0.4.0
+Name: lusid-express
+Version: 0.4.1
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.4.0/README.md` & `lusid_express-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/setup.py` & `lusid_express-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.4.0',
+    version='0.4.1',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.4.0/src/lusid_express/__main__.py` & `lusid_express-0.4.1/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/src/lusid_express/apis/__init__.py` & `lusid_express-0.4.1/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-0.4.1/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/src/lusid_express/display/__init__.py` & `lusid_express-0.4.1/src/lusid_express/display/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,7 +196,13 @@
         "<html><head>"
         + STYLES["table"]
         + "</head><body>"
         + html_string
         + "</body></html>"
     )
     return render_html(styled)
+
+def display_preloaded_vars():
+    """
+    Displays the preloaded variables in the current environment.
+    """
+    return render_markdown(PRELOADED_VARS_MARKDOWN)
```

### Comparing `lusid_express-0.4.0/src/lusid_express/load.le` & `lusid_express-0.4.1/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.0/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid-express
-Version: 0.4.0
+Name: lusid_express
+Version: 0.4.1
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

