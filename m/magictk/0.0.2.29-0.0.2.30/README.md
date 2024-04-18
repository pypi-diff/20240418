# Comparing `tmp/magictk-0.0.2.29.tar.gz` & `tmp/magictk-0.0.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.29.tar", last modified: Thu Apr 18 13:19:08 2024, max compression
+gzip compressed data, was "magictk-0.0.2.30.tar", last modified: Thu Apr 18 14:03:59 2024, max compression
```

## Comparing `magictk-0.0.2.29.tar` & `magictk-0.0.2.30.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:19:08.074744 magictk-0.0.2.29/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 13:19:08.074744 magictk-0.0.2.29/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-18 13:19:07.000000 magictk-0.0.2.29/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:19:08.074744 magictk-0.0.2.29/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 13:19:08.000000 magictk-0.0.2.29/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 13:19:08.000000 magictk-0.0.2.29/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:19:08.000000 magictk-0.0.2.29/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 13:19:08.000000 magictk-0.0.2.29/magictk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:19:08.000000 magictk-0.0.2.29/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 13:19:08.074744 magictk-0.0.2.29/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-18 13:19:07.000000 magictk-0.0.2.29/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:03:59.605702 magictk-0.0.2.30/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:03:59.605702 magictk-0.0.2.30/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-18 14:03:59.000000 magictk-0.0.2.30/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:03:59.605702 magictk-0.0.2.30/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:03:59.000000 magictk-0.0.2.30/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-18 14:03:59.000000 magictk-0.0.2.30/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:03:59.000000 magictk-0.0.2.30/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:03:59.000000 magictk-0.0.2.30/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 14:03:59.605702 magictk-0.0.2.30/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2024-04-18 14:03:59.000000 magictk-0.0.2.30/setup.py
```

### Comparing `magictk-0.0.2.29/README.md` & `magictk-0.0.2.30/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.29/setup.py` & `magictk-0.0.2.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     version=set_v,
     packages=(
         find_packages(where="./magictk")
     ),
     package_dir={
         "magictk": "./magictk",
     },
-    install_requires=["pywin32"],
+    install_requires=[],
     author='cxykevin|git.hmtsai.cn',
     author_email='cxykevin@yeah.net',
     description='A tkinter weights looks like element-plus',
     url='http://git.hmtsai.cn/cxykevin/magictk.git',
     license='GPLv2',
 )
```

