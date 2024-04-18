# Comparing `tmp/wei_office_simptool-0.0.1.tar.gz` & `tmp/wei_office_simptool-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.1.tar", last modified: Thu Apr 18 08:54:00 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.1.tar", last modified: Wed Mar 20 15:07:28 2024, max compression
```

## Comparing `wei_office_simptool-0.0.1.tar` & `wei_office_simptool-0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 08:54:00.370717 wei_office_simptool-0.0.1/
--rw-rw-rw-   0        0        0     3404 2024-04-18 08:54:00.368725 wei_office_simptool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2746 2024-04-18 08:47:44.000000 wei_office_simptool-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 08:54:00.371714 wei_office_simptool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2544 2024-04-18 08:53:30.000000 wei_office_simptool-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:54:00.346681 wei_office_simptool-0.0.1/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.1/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:54:00.349995 wei_office_simptool-0.0.1/wei_office_simptool/
--rw-rw-rw-   0        0        0     1667 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.1/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    13454 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.1/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:54:00.364514 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     3404 2024-04-18 08:54:00.000000 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-18 08:54:00.000000 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 08:54:00.000000 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-18 08:54:00.000000 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-18 08:54:00.000000 wei_office_simptool-0.0.1/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-20 15:07:28.682153 wei_office_simptool-0.1/
+-rw-rw-rw-   0        0        0      206 2024-03-20 15:07:28.682153 wei_office_simptool-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1644 2024-03-20 15:04:40.000000 wei_office_simptool-0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-20 15:07:28.682153 wei_office_simptool-0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2024-03-20 15:04:40.000000 wei_office_simptool-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:07:28.649952 wei_office_simptool-0.1/tests/
+-rw-rw-rw-   0        0        0     1359 2024-03-20 15:04:41.000000 wei_office_simptool-0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2097 2024-03-20 15:04:41.000000 wei_office_simptool-0.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:07:28.666895 wei_office_simptool-0.1/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1667 2024-03-20 15:04:41.000000 wei_office_simptool-0.1/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    13454 2024-03-20 15:05:57.000000 wei_office_simptool-0.1/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:07:28.682153 wei_office_simptool-0.1/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-03-20 15:07:28.000000 wei_office_simptool-0.1/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-03-20 15:07:28.000000 wei_office_simptool-0.1/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-20 15:07:28.000000 wei_office_simptool-0.1/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-03-20 15:07:28.000000 wei_office_simptool-0.1/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-03-20 15:07:28.000000 wei_office_simptool-0.1/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.1/tests/__init__.py` & `wei_office_simptool-0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.1/tests/test_utils.py` & `wei_office_simptool-0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.1/wei_office_simptool/__init__.py` & `wei_office_simptool-0.1/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.1/wei_office_simptool/utils.py` & `wei_office_simptool-0.1/wei_office_simptool/utils.py`

 * *Files identical despite different names*

