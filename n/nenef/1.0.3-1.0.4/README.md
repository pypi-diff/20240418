# Comparing `tmp/nenef-1.0.3.tar.gz` & `tmp/nenef-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nenef-1.0.3.tar", last modified: Thu Apr 18 05:33:37 2024, max compression
+gzip compressed data, was "nenef-1.0.4.tar", last modified: Thu Apr 18 05:49:22 2024, max compression
```

## Comparing `nenef-1.0.3.tar` & `nenef-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:33:37.292519 nenef-1.0.3/
--rw-rw-rw-   0        0        0     1061 2024-04-18 04:48:24.000000 nenef-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2396 2024-04-18 05:33:37.292519 nenef-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2024-04-18 04:30:59.000000 nenef-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:33:37.291305 nenef-1.0.3/nenef.egg-info/
--rw-rw-rw-   0        0        0     2396 2024-04-18 05:33:37.000000 nenef-1.0.3/nenef.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-18 05:33:37.000000 nenef-1.0.3/nenef.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:33:37.000000 nenef-1.0.3/nenef.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 05:33:37.000000 nenef-1.0.3/nenef.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:33:37.000000 nenef-1.0.3/nenef.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:33:37.293532 nenef-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-18 05:33:27.000000 nenef-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:49:22.284214 nenef-1.0.4/
+-rw-rw-rw-   0        0        0     1061 2024-04-18 04:48:24.000000 nenef-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2396 2024-04-18 05:49:22.284214 nenef-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2024-04-18 04:30:59.000000 nenef-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:49:22.279424 nenef-1.0.4/nenef/
+-rw-rw-rw-   0        0        0       73 2024-04-18 05:46:06.000000 nenef-1.0.4/nenef/__init__.py
+-rw-rw-rw-   0        0        0    11471 2024-04-18 05:47:38.000000 nenef-1.0.4/nenef/main.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:49:22.283039 nenef-1.0.4/nenef.egg-info/
+-rw-rw-rw-   0        0        0     2396 2024-04-18 05:49:22.000000 nenef-1.0.4/nenef.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-18 05:49:22.000000 nenef-1.0.4/nenef.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:49:22.000000 nenef-1.0.4/nenef.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 05:49:22.000000 nenef-1.0.4/nenef.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 05:49:22.000000 nenef-1.0.4/nenef.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:49:22.285218 nenef-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-04-18 05:49:19.000000 nenef-1.0.4/setup.py
```

### Comparing `nenef-1.0.3/LICENSE` & `nenef-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nenef-1.0.3/PKG-INFO` & `nenef-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nenef
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is module for neuronetworks
 Home-page: https://github.com/ktotozdesest/nenef
 Author: ktotozdesest
 Author-email: kto00210@gmail.com
 Project-URL: Documentation, https://github.com/ktotozdesest/nenef
 Keywords: python neuronetworks neurenet
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `nenef-1.0.3/README.md` & `nenef-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nenef-1.0.3/nenef.egg-info/PKG-INFO` & `nenef-1.0.4/nenef.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nenef
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is module for neuronetworks
 Home-page: https://github.com/ktotozdesest/nenef
 Author: ktotozdesest
 Author-email: kto00210@gmail.com
 Project-URL: Documentation, https://github.com/ktotozdesest/nenef
 Keywords: python neuronetworks neurenet
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `nenef-1.0.3/setup.py` & `nenef-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='nenef',
-    version='1.0.3',
+    version='1.0.4',
     author='ktotozdesest',
     author_email='kto00210@gmail.com',
     description='This is module for neuronetworks',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/ktotozdesest/nenef',
     packages=find_packages(),
```

