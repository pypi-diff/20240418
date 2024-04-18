# Comparing `tmp/compare-locales-9.0.2.tar.gz` & `tmp/compare_locales-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare-locales-9.0.2.tar", last modified: Mon Sep 18 16:48:41 2023, max compression
+gzip compressed data, was "compare_locales-9.0.3.tar", last modified: Thu Apr 18 11:52:03 2024, max compression
```

## Comparing `compare-locales-9.0.2.tar` & `compare_locales-9.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.364117 compare-locales-9.0.2/
--rw-r--r--   0 mathjazz   (502) staff       (20)    16725 2023-09-18 15:34:15.000000 compare-locales-9.0.2/LICENSE.md
--rw-r--r--   0 mathjazz   (502) staff       (20)     2707 2023-09-18 16:48:41.363884 compare-locales-9.0.2/PKG-INFO
--rw-r--r--   0 mathjazz   (502) staff       (20)     1539 2023-09-18 15:34:15.000000 compare-locales-9.0.2/README.md
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.357498 compare-locales-9.0.2/compare_locales/
--rw-r--r--   0 mathjazz   (502) staff       (20)       18 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/__init__.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.359557 compare-locales-9.0.2/compare_locales/checks/
--rw-r--r--   0 mathjazz   (502) staff       (20)      985 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/checks/__init__.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     7957 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/checks/android.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4316 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/checks/base.py
--rw-r--r--   0 mathjazz   (502) staff       (20)    10270 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/checks/dtd.py
--rw-r--r--   0 mathjazz   (502) staff       (20)    12840 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/checks/fluent.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     6486 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/checks/properties.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     8666 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/commands.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.360330 compare-locales-9.0.2/compare_locales/compare/
--rw-r--r--   0 mathjazz   (502) staff       (20)     3181 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/compare/__init__.py
--rw-r--r--   0 mathjazz   (502) staff       (20)    11426 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/compare/content.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     7263 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/compare/observer.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4207 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/compare/utils.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     1506 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/keyedtuple.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.360986 compare-locales-9.0.2/compare_locales/lint/
--rw-r--r--   0 mathjazz   (502) staff       (20)        0 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/lint/__init__.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     2951 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/lint/cli.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4116 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/lint/linter.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     1284 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/lint/util.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4650 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/merge.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4234 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/mozpath.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.362584 compare-locales-9.0.2/compare_locales/parser/
--rw-r--r--   0 mathjazz   (502) staff       (20)     2122 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/__init__.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     9115 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/android.py
--rw-r--r--   0 mathjazz   (502) staff       (20)    12779 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/base.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     3402 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/defines.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4254 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/dtd.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     6875 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/fluent.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     1529 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/ini.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     3145 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/po.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     3676 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/parser/properties.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.363573 compare-locales-9.0.2/compare_locales/paths/
--rw-r--r--   0 mathjazz   (502) staff       (20)     1442 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/__init__.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4202 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/configparser.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     8961 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/files.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     8230 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/ini.py
--rw-r--r--   0 mathjazz   (502) staff       (20)    14926 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/matcher.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     8475 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/paths/project.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4014 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/plurals.py
--rw-r--r--   0 mathjazz   (502) staff       (20)     4295 2023-09-18 15:34:35.000000 compare-locales-9.0.2/compare_locales/serializer.py
--rw-r--r--   0 mathjazz   (502) staff       (20)      448 2023-09-18 15:34:15.000000 compare-locales-9.0.2/compare_locales/util.py
-drwxr-xr-x   0 mathjazz   (502) staff       (20)        0 2023-09-18 16:48:41.358399 compare-locales-9.0.2/compare_locales.egg-info/
--rw-r--r--   0 mathjazz   (502) staff       (20)     2707 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/PKG-INFO
--rw-r--r--   0 mathjazz   (502) staff       (20)     1442 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/SOURCES.txt
--rw-r--r--   0 mathjazz   (502) staff       (20)        1 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/dependency_links.txt
--rw-r--r--   0 mathjazz   (502) staff       (20)      127 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/entry_points.txt
--rw-r--r--   0 mathjazz   (502) staff       (20)       37 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/requires.txt
--rw-r--r--   0 mathjazz   (502) staff       (20)       16 2023-09-18 16:48:41.000000 compare-locales-9.0.2/compare_locales.egg-info/top_level.txt
--rw-r--r--   0 mathjazz   (502) staff       (20)     1694 2023-09-18 15:34:35.000000 compare-locales-9.0.2/pyproject.toml
--rw-r--r--   0 mathjazz   (502) staff       (20)       38 2023-09-18 16:48:41.364169 compare-locales-9.0.2/setup.cfg
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.371358 compare_locales-9.0.3/
+-rw-r--r--   0 eemeli     (501) staff       (20)    16725 2023-11-08 00:26:12.000000 compare_locales-9.0.3/LICENSE.md
+-rw-r--r--   0 eemeli     (501) staff       (20)     2707 2024-04-18 11:52:03.371145 compare_locales-9.0.3/PKG-INFO
+-rw-r--r--   0 eemeli     (501) staff       (20)     1539 2023-11-08 00:26:12.000000 compare_locales-9.0.3/README.md
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.362436 compare_locales-9.0.3/compare_locales/
+-rw-r--r--   0 eemeli     (501) staff       (20)       18 2024-04-18 11:48:59.000000 compare_locales-9.0.3/compare_locales/__init__.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.364941 compare_locales-9.0.3/compare_locales/checks/
+-rw-r--r--   0 eemeli     (501) staff       (20)      985 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/checks/__init__.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     7994 2024-04-18 11:33:34.000000 compare_locales-9.0.3/compare_locales/checks/android.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4316 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/checks/base.py
+-rw-r--r--   0 eemeli     (501) staff       (20)    10270 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/checks/dtd.py
+-rw-r--r--   0 eemeli     (501) staff       (20)    12840 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/checks/fluent.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     6486 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/checks/properties.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     8666 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/commands.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.365954 compare_locales-9.0.3/compare_locales/compare/
+-rw-r--r--   0 eemeli     (501) staff       (20)     3181 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/compare/__init__.py
+-rw-r--r--   0 eemeli     (501) staff       (20)    11426 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/compare/content.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     7263 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/compare/observer.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4207 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/compare/utils.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     1506 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/keyedtuple.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.366765 compare_locales-9.0.3/compare_locales/lint/
+-rw-r--r--   0 eemeli     (501) staff       (20)        0 2021-10-22 09:06:34.000000 compare_locales-9.0.3/compare_locales/lint/__init__.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     2951 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/lint/cli.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4116 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/lint/linter.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     1284 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/lint/util.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4650 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/merge.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4234 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/mozpath.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.368991 compare_locales-9.0.3/compare_locales/parser/
+-rw-r--r--   0 eemeli     (501) staff       (20)     2122 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/__init__.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     9115 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/android.py
+-rw-r--r--   0 eemeli     (501) staff       (20)    12779 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/base.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     3402 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/defines.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4254 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/dtd.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     6875 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/fluent.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     1529 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/ini.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     3145 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/po.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     3676 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/parser/properties.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.370666 compare_locales-9.0.3/compare_locales/paths/
+-rw-r--r--   0 eemeli     (501) staff       (20)     1442 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/__init__.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4202 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/configparser.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     8961 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/files.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     8230 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/ini.py
+-rw-r--r--   0 eemeli     (501) staff       (20)    14926 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/matcher.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     8475 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/paths/project.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4014 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/plurals.py
+-rw-r--r--   0 eemeli     (501) staff       (20)     4295 2024-04-18 11:31:52.000000 compare_locales-9.0.3/compare_locales/serializer.py
+-rw-r--r--   0 eemeli     (501) staff       (20)      448 2023-11-08 00:26:12.000000 compare_locales-9.0.3/compare_locales/util.py
+drwxr-xr-x   0 eemeli     (501) staff       (20)        0 2024-04-18 11:52:03.370893 compare_locales-9.0.3/compare_locales.egg-info/
+-rw-r--r--   0 eemeli     (501) staff       (20)     2707 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/PKG-INFO
+-rw-r--r--   0 eemeli     (501) staff       (20)     1442 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/SOURCES.txt
+-rw-r--r--   0 eemeli     (501) staff       (20)        1 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/dependency_links.txt
+-rw-r--r--   0 eemeli     (501) staff       (20)      127 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/entry_points.txt
+-rw-r--r--   0 eemeli     (501) staff       (20)       37 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/requires.txt
+-rw-r--r--   0 eemeli     (501) staff       (20)       16 2024-04-18 11:52:03.000000 compare_locales-9.0.3/compare_locales.egg-info/top_level.txt
+-rw-r--r--   0 eemeli     (501) staff       (20)     1694 2024-04-18 11:31:52.000000 compare_locales-9.0.3/pyproject.toml
+-rw-r--r--   0 eemeli     (501) staff       (20)       38 2024-04-18 11:52:03.371399 compare_locales-9.0.3/setup.cfg
```

### Comparing `compare-locales-9.0.2/LICENSE.md` & `compare_locales-9.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/PKG-INFO` & `compare_locales-9.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compare-locales
-Version: 9.0.2
+Version: 9.0.3
 Summary: Lint Mozilla localizations
 Author: Axel Hecht
 Author-email: Mozilla <l10n-drivers@mozilla.org>, Eemeli Aro <eemeli@mozilla.com>
 License: MPL-2.0
 Project-URL: repository, https://github.com/mozilla/compare-locales
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `compare-locales-9.0.2/README.md` & `compare_locales-9.0.3/README.md`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/checks/__init__.py` & `compare_locales-9.0.3/compare_locales/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/checks/android.py` & `compare_locales-9.0.3/compare_locales/checks/android.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,17 @@
     params = {}
     errors = []
     count = 0
     next_implicit = 1
     for ref in refs:
         if isinstance(ref, minidom.Node):
             ref = textContent(ref)
-        for m in re.finditer(r"%(?P<order>[1-9]\$)?(?P<format>[sSd])", ref):
+        for m in re.finditer(
+            r"%(?P<order>[1-9]\$)?(?P<format>(?:\.[0-9]+)?f|[dsS])", ref
+        ):
             count += 1
             order = m.group("order")
             if order:
                 order = int(order[0])
             else:
                 order = next_implicit
                 next_implicit += 1
```

### Comparing `compare-locales-9.0.2/compare_locales/checks/base.py` & `compare_locales-9.0.3/compare_locales/checks/base.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/checks/dtd.py` & `compare_locales-9.0.3/compare_locales/checks/dtd.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/checks/fluent.py` & `compare_locales-9.0.3/compare_locales/checks/fluent.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/checks/properties.py` & `compare_locales-9.0.3/compare_locales/checks/properties.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/commands.py` & `compare_locales-9.0.3/compare_locales/commands.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/compare/__init__.py` & `compare_locales-9.0.3/compare_locales/compare/__init__.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/compare/content.py` & `compare_locales-9.0.3/compare_locales/compare/content.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/compare/observer.py` & `compare_locales-9.0.3/compare_locales/compare/observer.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/compare/utils.py` & `compare_locales-9.0.3/compare_locales/compare/utils.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/keyedtuple.py` & `compare_locales-9.0.3/compare_locales/keyedtuple.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/lint/cli.py` & `compare_locales-9.0.3/compare_locales/lint/cli.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/lint/linter.py` & `compare_locales-9.0.3/compare_locales/lint/linter.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/lint/util.py` & `compare_locales-9.0.3/compare_locales/lint/util.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/merge.py` & `compare_locales-9.0.3/compare_locales/merge.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/mozpath.py` & `compare_locales-9.0.3/compare_locales/mozpath.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/__init__.py` & `compare_locales-9.0.3/compare_locales/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/android.py` & `compare_locales-9.0.3/compare_locales/parser/android.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/base.py` & `compare_locales-9.0.3/compare_locales/parser/base.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/defines.py` & `compare_locales-9.0.3/compare_locales/parser/defines.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/dtd.py` & `compare_locales-9.0.3/compare_locales/parser/dtd.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/fluent.py` & `compare_locales-9.0.3/compare_locales/parser/fluent.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/ini.py` & `compare_locales-9.0.3/compare_locales/parser/ini.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/po.py` & `compare_locales-9.0.3/compare_locales/parser/po.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/parser/properties.py` & `compare_locales-9.0.3/compare_locales/parser/properties.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/__init__.py` & `compare_locales-9.0.3/compare_locales/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/configparser.py` & `compare_locales-9.0.3/compare_locales/paths/configparser.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/files.py` & `compare_locales-9.0.3/compare_locales/paths/files.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/ini.py` & `compare_locales-9.0.3/compare_locales/paths/ini.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/matcher.py` & `compare_locales-9.0.3/compare_locales/paths/matcher.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/paths/project.py` & `compare_locales-9.0.3/compare_locales/paths/project.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/plurals.py` & `compare_locales-9.0.3/compare_locales/plurals.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales/serializer.py` & `compare_locales-9.0.3/compare_locales/serializer.py`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/compare_locales.egg-info/PKG-INFO` & `compare_locales-9.0.3/compare_locales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compare-locales
-Version: 9.0.2
+Version: 9.0.3
 Summary: Lint Mozilla localizations
 Author: Axel Hecht
 Author-email: Mozilla <l10n-drivers@mozilla.org>, Eemeli Aro <eemeli@mozilla.com>
 License: MPL-2.0
 Project-URL: repository, https://github.com/mozilla/compare-locales
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `compare-locales-9.0.2/compare_locales.egg-info/SOURCES.txt` & `compare_locales-9.0.3/compare_locales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compare-locales-9.0.2/pyproject.toml` & `compare_locales-9.0.3/pyproject.toml`

 * *Files identical despite different names*

