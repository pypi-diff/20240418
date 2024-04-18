# Comparing `tmp/googleadsquerytool-0.1.2.tar.gz` & `tmp/googleadsquerytool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleadsquerytool-0.1.2.tar", max compression
+gzip compressed data, was "googleadsquerytool-0.1.3.tar", max compression
```

## Comparing `googleadsquerytool-0.1.2.tar` & `googleadsquerytool-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      157 2024-04-18 19:39:30.627572 googleadsquerytool-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-18 19:08:34.904765 googleadsquerytool-0.1.2/googleadsquerytool/tools/__init__.py
--rw-r--r--   0        0        0     3951 2024-04-18 12:38:43.656115 googleadsquerytool-0.1.2/googleadsquerytool/tools/googleadsquerytool.py
--rw-r--r--   0        0        0      394 2024-04-18 19:43:58.458121 googleadsquerytool-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 googleadsquerytool-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-04-18 19:39:30.627572 googleadsquerytool-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 19:08:34.904765 googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/__init__.py
+-rw-r--r--   0        0        0     3951 2024-04-18 12:38:43.656115 googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/googleadsquerytool.py
+-rw-r--r--   0        0        0      394 2024-04-18 19:49:15.597768 googleadsquerytool-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 googleadsquerytool-0.1.3/PKG-INFO
```

### Comparing `googleadsquerytool-0.1.2/googleadsquerytool/tools/googleadsquerytool.py` & `googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/googleadsquerytool.py`

 * *Files identical despite different names*

### Comparing `googleadsquerytool-0.1.2/PKG-INFO` & `googleadsquerytool-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleadsquerytool
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is a package you can use to query reporting data from the Google Ads API.
 Author: caspercrause
 Author-email: ccrause07@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

