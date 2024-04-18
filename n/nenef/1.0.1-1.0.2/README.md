# Comparing `tmp/nenef-1.0.1.tar.gz` & `tmp/nenef-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nenef-1.0.1.tar", last modified: Thu Apr 18 05:18:41 2024, max compression
+gzip compressed data, was "nenef-1.0.2.tar", last modified: Thu Apr 18 05:24:11 2024, max compression
```

## Comparing `nenef-1.0.1.tar` & `nenef-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:18:41.089284 nenef-1.0.1/
--rw-rw-rw-   0        0        0     1061 2024-04-18 04:48:24.000000 nenef-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2396 2024-04-18 05:18:41.089284 nenef-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2024-04-18 04:30:59.000000 nenef-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:18:41.087848 nenef-1.0.1/nenef.egg-info/
--rw-rw-rw-   0        0        0     2396 2024-04-18 05:18:41.000000 nenef-1.0.1/nenef.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-18 05:18:41.000000 nenef-1.0.1/nenef.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:18:41.000000 nenef-1.0.1/nenef.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 05:18:41.000000 nenef-1.0.1/nenef.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:18:41.000000 nenef-1.0.1/nenef.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:18:41.090288 nenef-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-18 05:18:37.000000 nenef-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:24:11.239893 nenef-1.0.2/
+-rw-rw-rw-   0        0        0     1061 2024-04-18 04:48:24.000000 nenef-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2396 2024-04-18 05:24:11.239893 nenef-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2024-04-18 04:30:59.000000 nenef-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:24:11.239893 nenef-1.0.2/nenef.egg-info/
+-rw-rw-rw-   0        0        0     2396 2024-04-18 05:24:11.000000 nenef-1.0.2/nenef.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-18 05:24:11.000000 nenef-1.0.2/nenef.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:24:11.000000 nenef-1.0.2/nenef.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 05:24:11.000000 nenef-1.0.2/nenef.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:24:11.000000 nenef-1.0.2/nenef.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:24:11.240897 nenef-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-04-18 05:24:06.000000 nenef-1.0.2/setup.py
```

### Comparing `nenef-1.0.1/LICENSE` & `nenef-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nenef-1.0.1/PKG-INFO` & `nenef-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nenef
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is module for neuronetworks
 Home-page: https://github.com/ktotozdesest/nenef
 Author: ktotozdesest
 Author-email: kto00210@gmail.com
 Project-URL: Documentation, https://github.com/ktotozdesest/nenef
 Keywords: python neuronetworks neurenet
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `nenef-1.0.1/README.md` & `nenef-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nenef-1.0.1/nenef.egg-info/PKG-INFO` & `nenef-1.0.2/nenef.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nenef
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is module for neuronetworks
 Home-page: https://github.com/ktotozdesest/nenef
 Author: ktotozdesest
 Author-email: kto00210@gmail.com
 Project-URL: Documentation, https://github.com/ktotozdesest/nenef
 Keywords: python neuronetworks neurenet
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `nenef-1.0.1/setup.py` & `nenef-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='nenef',
-    version='1.0.1',
+    version='1.0.2',
     author='ktotozdesest',
     author_email='kto00210@gmail.com',
     description='This is module for neuronetworks',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/ktotozdesest/nenef',
     packages=find_packages(),
```

