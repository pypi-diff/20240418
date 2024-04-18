# Comparing `tmp/tokenizernltk-0.0.13.tar.gz` & `tmp/tokenizernltk-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizernltk-0.0.13.tar", last modified: Thu Apr 18 00:19:49 2024, max compression
+gzip compressed data, was "tokenizernltk-0.0.14.tar", last modified: Thu Apr 18 00:44:49 2024, max compression
```

## Comparing `tokenizernltk-0.0.13.tar` & `tokenizernltk-0.0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:19:49.905876 tokenizernltk-0.0.13/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-18 00:19:49.904876 tokenizernltk-0.0.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1678 2024-04-18 00:13:22.000000 tokenizernltk-0.0.13/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 00:19:49.905876 tokenizernltk-0.0.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-18 00:18:47.000000 tokenizernltk-0.0.13/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:19:49.903876 tokenizernltk-0.0.13/tokeninput/
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-18 00:17:47.000000 tokenizernltk-0.0.13/tokeninput/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-04-18 00:17:38.000000 tokenizernltk-0.0.13/tokeninput/tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:19:49.904876 tokenizernltk-0.0.13/tokenizernltk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-18 00:19:49.000000 tokenizernltk-0.0.13/tokenizernltk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-18 00:19:49.000000 tokenizernltk-0.0.13/tokenizernltk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 00:19:49.000000 tokenizernltk-0.0.13/tokenizernltk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 00:19:49.000000 tokenizernltk-0.0.13/tokenizernltk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-18 00:19:49.000000 tokenizernltk-0.0.13/tokenizernltk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:44:49.062947 tokenizernltk-0.0.14/
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-18 00:44:49.062947 tokenizernltk-0.0.14/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-04-18 00:13:22.000000 tokenizernltk-0.0.14/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 00:44:49.062947 tokenizernltk-0.0.14/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-18 00:35:21.000000 tokenizernltk-0.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:44:49.061946 tokenizernltk-0.0.14/tokeninput/
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-18 00:44:02.000000 tokenizernltk-0.0.14/tokeninput/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-04-18 00:27:18.000000 tokenizernltk-0.0.14/tokeninput/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:44:49.062947 tokenizernltk-0.0.14/tokenizernltk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-18 00:44:48.000000 tokenizernltk-0.0.14/tokenizernltk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-18 00:44:49.000000 tokenizernltk-0.0.14/tokenizernltk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 00:44:48.000000 tokenizernltk-0.0.14/tokenizernltk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 00:44:48.000000 tokenizernltk-0.0.14/tokenizernltk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-18 00:44:48.000000 tokenizernltk-0.0.14/tokenizernltk.egg-info/top_level.txt
```

### Comparing `tokenizernltk-0.0.13/README.md` & `tokenizernltk-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `tokenizernltk-0.0.13/tokeninput/tokenizer.py` & `tokenizernltk-0.0.14/tokeninput/tokenizer.py`

 * *Files identical despite different names*

