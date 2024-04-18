# Comparing `tmp/istr_python-0.0.6.tar.gz` & `tmp/istr_python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.0.6.tar", last modified: Wed Apr 17 15:02:27 2024, max compression
+gzip compressed data, was "istr_python-0.0.7.tar", last modified: Wed Apr 17 16:31:12 2024, max compression
```

## Comparing `istr_python-0.0.6.tar` & `istr_python-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.510317 istr_python-0.0.6/
--rw-rw-rw-   0        0        0     4153 2024-04-17 15:02:27.510317 istr_python-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3724 2024-04-17 07:17:19.000000 istr_python-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.476216 istr_python-0.0.6/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.0.6/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.6/istr/install istr.py
--rw-rw-rw-   0        0        0    12753 2024-04-17 12:29:37.000000 istr_python-0.0.6/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.510317 istr_python-0.0.6/istr_python.egg-info/
--rw-rw-rw-   0        0        0     4153 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2024-04-17 15:02:20.000000 istr_python-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 15:02:27.515329 istr_python-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.508235 istr_python-0.0.6/tests/
--rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.6/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:31:12.957680 istr_python-0.0.7/
+-rw-rw-rw-   0        0        0     6165 2024-04-17 16:31:12.956677 istr_python-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5301 2024-04-17 16:29:06.000000 istr_python-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 16:31:12.941529 istr_python-0.0.7/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.0.7/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.7/istr/install istr.py
+-rw-rw-rw-   0        0        0    12754 2024-04-17 16:29:02.000000 istr_python-0.0.7/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:31:12.956677 istr_python-0.0.7/istr_python.egg-info/
+-rw-rw-rw-   0        0        0     6165 2024-04-17 16:31:12.000000 istr_python-0.0.7/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-17 16:31:12.000000 istr_python-0.0.7/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 16:31:12.000000 istr_python-0.0.7/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 16:31:12.000000 istr_python-0.0.7/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2024-04-17 16:31:07.000000 istr_python-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 16:31:12.958681 istr_python-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 16:31:12.954680 istr_python-0.0.7/tests/
+-rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.7/tests/test_istr.py
```

### Comparing `istr_python-0.0.6/istr/install istr.py` & `istr_python-0.0.7/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.0.6/istr/istr.py` & `istr_python-0.0.7/istr/istr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #   _       _
 #  (_) ___ | |_  _ __
 #  | |/ __|| __|| '__|
 #  | |\__ \| |_ | |
 #  |_||___/ \__||_|    use strings as integers
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 class istr(str):
     """
     istr object
 
     Parameters
     ----------
@@ -34,15 +34,16 @@
             istr(range(3)) ==> istr.range(3)
             list(istr(range(3))) ==> [istr('0'), istr('1'), istr('2')]
             len(istr(range(3))) ==> 3
 
         it is possible to give more than one parameter, in which case a tuple
         of the istrs of the parameters will be returned, which can be handy
         to multiple assign, e.g.
-            a, b, c = istr(5, 6, 7) ==> a=istr("5') , b=istr("6"), c=istr("7")"""
+            a, b, c = istr(5, 6, 7) ==> a=istr("5') , b=istr("6"), c=istr("7")
+"""
 
     _format = ""
 
     @classmethod
     def toint(cls, value):
         try:
             return int(value)
```

### Comparing `istr_python-0.0.6/tests/test_istr.py` & `istr_python-0.0.7/tests/test_istr.py`

 * *Files identical despite different names*

