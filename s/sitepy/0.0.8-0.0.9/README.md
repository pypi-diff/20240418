# Comparing `tmp/sitepy-0.0.8.tar.gz` & `tmp/sitepy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.8.tar", last modified: Thu Apr 18 18:40:48 2024, max compression
+gzip compressed data, was "sitepy-0.0.9.tar", last modified: Thu Apr 18 18:57:05 2024, max compression
```

## Comparing `sitepy-0.0.8.tar` & `sitepy-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.064246 sitepy-0.0.8/
--rw-rw-rw-   0        0        0     1766 2024-04-18 18:40:48.063246 sitepy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      913 2024-04-17 20:28:24.000000 sitepy-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 18:40:48.065248 sitepy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-04-17 20:39:38.000000 sitepy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.046242 sitepy-0.0.8/sitepy/
--rw-rw-rw-   0        0        0      112 2024-04-18 18:39:00.000000 sitepy-0.0.8/sitepy/__init__.py
--rw-rw-rw-   0        0        0     3274 2024-04-18 01:58:35.000000 sitepy-0.0.8/sitepy/sitepy.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.060245 sitepy-0.0.8/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1766 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.166716 sitepy-0.0.9/
+-rw-rw-rw-   0        0        0     1787 2024-04-18 18:57:05.157631 sitepy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2024-04-17 20:28:24.000000 sitepy-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:57:05.167813 sitepy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-04-18 18:56:36.000000 sitepy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.032173 sitepy-0.0.9/sitepy/
+-rw-rw-rw-   0        0        0      130 2024-04-18 18:55:57.000000 sitepy-0.0.9/sitepy/__init__.py
+-rw-rw-rw-   0        0        0     3274 2024-04-18 01:58:35.000000 sitepy-0.0.9/sitepy/sitepy.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.155028 sitepy-0.0.9/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1787 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.8/PKG-INFO` & `sitepy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
+License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sitepy-0.0.8/README.md` & `sitepy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.0.8/setup.py` & `sitepy-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.0.8',
+    version='0.0.9',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
+    license='Apache 2.0',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
     long_description_content_type='text/markdown',  # Add this line
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `sitepy-0.0.8/sitepy/sitepy.py` & `sitepy-0.0.9/sitepy/sitepy.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.0.8/sitepy.egg-info/PKG-INFO` & `sitepy-0.0.9/sitepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
+License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

