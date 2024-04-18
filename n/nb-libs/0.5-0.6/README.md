# Comparing `tmp/nb_libs-0.5.tar.gz` & `tmp/nb_libs-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_libs-0.5.tar", last modified: Thu Apr 18 02:41:41 2024, max compression
+gzip compressed data, was "dist\nb_libs-0.6.tar", last modified: Thu Apr 18 02:51:38 2024, max compression
```

## Comparing `nb_libs-0.5.tar` & `nb_libs-0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/
--rw-rw-rw-   0        0        0     2255 2024-04-18 02:41:41.000000 nb_libs-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1536 2023-11-17 02:24:36.000000 nb_libs-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/nb_libs.egg-info/
--rw-rw-rw-   0        0        0     2255 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 02:41:41.000000 nb_libs-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1714 2024-04-18 02:41:38.000000 nb_libs-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/tests/
--rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-0.5/tests/test_restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-0.5/tests/tests_time.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:51:38.000000 nb_libs-0.6/
+-rw-rw-rw-   0        0        0       41 2024-04-18 02:51:35.000000 nb_libs-0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2255 2024-04-18 02:51:38.000000 nb_libs-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1536 2023-11-17 02:24:36.000000 nb_libs-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 02:51:38.000000 nb_libs-0.6/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0     2255 2024-04-18 02:51:37.000000 nb_libs-0.6/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-18 02:51:37.000000 nb_libs-0.6/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:51:37.000000 nb_libs-0.6/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 02:51:37.000000 nb_libs-0.6/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:51:37.000000 nb_libs-0.6/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:51:38.000000 nb_libs-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2024-04-18 02:51:35.000000 nb_libs-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:51:38.000000 nb_libs-0.6/tests/
+-rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-0.6/tests/test_restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-0.6/tests/tests_time.py
```

### Comparing `nb_libs-0.5/PKG-INFO` & `nb_libs-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_libs
-Version: 0.5
+Version: 0.6
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-0.5/README.md` & `nb_libs-0.6/README.md`

 * *Files identical despite different names*

### Comparing `nb_libs-0.5/nb_libs.egg-info/PKG-INFO` & `nb_libs-0.6/nb_libs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-libs
-Version: 0.5
+Version: 0.6
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-0.5/setup.py` & `nb_libs-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="0.5",
+    version="0.6",
     description=('nb_libs'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
```

### Comparing `nb_libs-0.5/tests/tests_time.py` & `nb_libs-0.6/tests/tests_time.py`

 * *Files identical despite different names*

