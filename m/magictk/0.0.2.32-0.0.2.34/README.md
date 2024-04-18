# Comparing `tmp/magictk-0.0.2.32.tar.gz` & `tmp/magictk-0.0.2.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.32.tar", last modified: Thu Apr 18 14:10:53 2024, max compression
+gzip compressed data, was "magictk-0.0.2.34.tar", last modified: Thu Apr 18 14:23:35 2024, max compression
```

## Comparing `magictk-0.0.2.32.tar` & `magictk-0.0.2.34.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:10:53.588007 magictk-0.0.2.32/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:10:53.588007 magictk-0.0.2.32/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-18 14:10:53.000000 magictk-0.0.2.32/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:10:53.588007 magictk-0.0.2.32/magictk/
--rw-r--r--   0 root         (0) root         (0)      323 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9778 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    11910 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10457 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:10:53.588007 magictk-0.0.2.32/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      475 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 14:10:53.000000 magictk-0.0.2.32/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 14:10:53.588007 magictk-0.0.2.32/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-18 14:10:53.000000 magictk-0.0.2.32/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:23:35.276654 magictk-0.0.2.34/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:23:35.276654 magictk-0.0.2.34/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-18 14:23:34.000000 magictk-0.0.2.34/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:23:35.276654 magictk-0.0.2.34/magictk/
+-rw-r--r--   0 root         (0) root         (0)      323 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-18 14:23:34.000000 magictk-0.0.2.34/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:23:35.276654 magictk-0.0.2.34/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 14:23:35.000000 magictk-0.0.2.34/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      475 2024-04-18 14:23:35.000000 magictk-0.0.2.34/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:23:35.000000 magictk-0.0.2.34/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 14:23:35.000000 magictk-0.0.2.34/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 14:23:35.276654 magictk-0.0.2.34/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-18 14:23:34.000000 magictk-0.0.2.34/setup.py
```

### Comparing `magictk-0.0.2.32/README.md` & `magictk-0.0.2.34/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/_window_ctl.py` & `magictk-0.0.2.34/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/_window_size.py` & `magictk-0.0.2.34/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/button.py` & `magictk-0.0.2.34/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/checkbox.py` & `magictk-0.0.2.34/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/color_tmpl.py` & `magictk-0.0.2.34/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/entry.py` & `magictk-0.0.2.34/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/fontconfig.py` & `magictk-0.0.2.34/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/photoload.py` & `magictk-0.0.2.34/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/progressbar.py` & `magictk-0.0.2.34/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/select.py` & `magictk-0.0.2.34/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/submenu.py` & `magictk-0.0.2.34/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/window.py` & `magictk-0.0.2.34/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/magictk/workspace.py` & `magictk-0.0.2.34/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.32/setup.py` & `magictk-0.0.2.34/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 setup(
     name="magictk",
     version=set_v,
     packages=find_packages(),
     package_dir={
         "magictk": "./magictk",
     },
+    package_data={
+        '':['*.py'],
+        'res file':['*.pickle']
+    },
     install_requires=[],
     author='cxykevin|git.hmtsai.cn',
     author_email='cxykevin@yeah.net',
     description='A tkinter weights looks like element-plus',
     url='http://git.hmtsai.cn/cxykevin/magictk.git',
     license='GPLv2',
 )
```

