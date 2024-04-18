# Comparing `tmp/nb_libs-0.9.tar.gz` & `tmp/nb_libs-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_libs-0.9.tar", last modified: Thu Apr 18 02:56:35 2024, max compression
+gzip compressed data, was "dist\nb_libs-1.0.tar", last modified: Thu Apr 18 03:00:52 2024, max compression
```

## Comparing `nb_libs-0.9.tar` & `nb_libs-1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:56:35.000000 nb_libs-0.9/
--rw-rw-rw-   0        0        0       41 2024-04-18 02:51:35.000000 nb_libs-0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2253 2024-04-18 02:56:35.000000 nb_libs-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1536 2023-11-17 02:24:36.000000 nb_libs-0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:56:35.000000 nb_libs-0.9/nb_libs/
--rw-rw-rw-   0        0        0        0 2024-04-18 02:55:05.000000 nb_libs-0.9/nb_libs/__init__.py
--rw-rw-rw-   0        0        0     3106 2023-11-17 02:18:55.000000 nb_libs-0.9/nb_libs/auto_git.py
--rw-rw-rw-   0        0        0     2041 2024-01-02 03:07:27.000000 nb_libs-0.9/nb_libs/code_line_statistics.py
--rw-rw-rw-   0        0        0      362 2023-10-23 03:14:12.000000 nb_libs-0.9/nb_libs/dict2json.py
--rw-rw-rw-   0        0        0      490 2023-10-23 03:14:12.000000 nb_libs-0.9/nb_libs/global_dict.py
--rw-rw-rw-   0        0        0      487 2024-04-16 03:39:38.000000 nb_libs-0.9/nb_libs/lazy_importer.py
--rw-rw-rw-   0        0        0       21 2024-03-20 10:00:54.000000 nb_libs-0.9/nb_libs/nb_time.py
--rw-rw-rw-   0        0        0     2841 2024-04-03 08:52:42.000000 nb_libs-0.9/nb_libs/path_helper.py
--rw-rw-rw-   0        0        0     1418 2023-03-15 02:37:59.000000 nb_libs-0.9/nb_libs/restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      229 2023-11-24 10:39:15.000000 nb_libs-0.9/nb_libs/sys_frame_uitils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:56:35.000000 nb_libs-0.9/nb_libs.egg-info/
--rw-rw-rw-   0        0        0     2253 2024-04-18 02:56:34.000000 nb_libs-0.9/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-04-18 02:56:34.000000 nb_libs-0.9/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:56:34.000000 nb_libs-0.9/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 02:56:34.000000 nb_libs-0.9/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 02:56:34.000000 nb_libs-0.9/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 02:56:35.000000 nb_libs-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1712 2024-04-18 02:56:32.000000 nb_libs-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:56:35.000000 nb_libs-0.9/tests/
--rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-0.9/tests/test_restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-0.9/tests/tests_time.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/
+-rw-rw-rw-   0        0        0       41 2024-04-18 02:51:35.000000 nb_libs-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      995 2024-04-18 03:00:52.000000 nb_libs-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-18 03:00:48.000000 nb_libs-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/nb_libs/
+-rw-rw-rw-   0        0        0        0 2024-04-18 02:55:05.000000 nb_libs-1.0/nb_libs/__init__.py
+-rw-rw-rw-   0        0        0     3106 2023-11-17 02:18:55.000000 nb_libs-1.0/nb_libs/auto_git.py
+-rw-rw-rw-   0        0        0     2041 2024-01-02 03:07:27.000000 nb_libs-1.0/nb_libs/code_line_statistics.py
+-rw-rw-rw-   0        0        0      362 2023-10-23 03:14:12.000000 nb_libs-1.0/nb_libs/dict2json.py
+-rw-rw-rw-   0        0        0      490 2023-10-23 03:14:12.000000 nb_libs-1.0/nb_libs/global_dict.py
+-rw-rw-rw-   0        0        0      487 2024-04-16 03:39:38.000000 nb_libs-1.0/nb_libs/lazy_importer.py
+-rw-rw-rw-   0        0        0       21 2024-03-20 10:00:54.000000 nb_libs-1.0/nb_libs/nb_time.py
+-rw-rw-rw-   0        0        0     2841 2024-04-03 08:52:42.000000 nb_libs-1.0/nb_libs/path_helper.py
+-rw-rw-rw-   0        0        0     1418 2023-03-15 02:37:59.000000 nb_libs-1.0/nb_libs/restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      229 2023-11-24 10:39:15.000000 nb_libs-1.0/nb_libs/sys_frame_uitils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0      995 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 03:00:52.000000 nb_libs-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-04-18 03:00:48.000000 nb_libs-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/tests/
+-rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-1.0/tests/test_restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-1.0/tests/tests_time.py
```

### Comparing `nb_libs-0.9/nb_libs/auto_git.py` & `nb_libs-1.0/nb_libs/auto_git.py`

 * *Files identical despite different names*

### Comparing `nb_libs-0.9/nb_libs/code_line_statistics.py` & `nb_libs-1.0/nb_libs/code_line_statistics.py`

 * *Files identical despite different names*

### Comparing `nb_libs-0.9/nb_libs/path_helper.py` & `nb_libs-1.0/nb_libs/path_helper.py`

 * *Files identical despite different names*

### Comparing `nb_libs-0.9/nb_libs/restart_programe_by_interval.py` & `nb_libs-1.0/nb_libs/restart_programe_by_interval.py`

 * *Files identical despite different names*

### Comparing `nb_libs-0.9/setup.py` & `nb_libs-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="0.9",
-    description=('nb_libs'),
+    version="1.0",
+    description=('nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
     author_email='ydf0509@sohu.com',
```

### Comparing `nb_libs-0.9/tests/tests_time.py` & `nb_libs-1.0/tests/tests_time.py`

 * *Files identical despite different names*

