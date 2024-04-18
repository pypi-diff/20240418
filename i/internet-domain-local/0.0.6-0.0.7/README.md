# Comparing `tmp/internet_domain_local-0.0.6.tar.gz` & `tmp/internet_domain_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet_domain_local-0.0.6.tar", last modified: Wed Apr 17 14:43:22 2024, max compression
+gzip compressed data, was "internet_domain_local-0.0.7.tar", last modified: Thu Apr 18 18:57:20 2024, max compression
```

## Comparing `internet_domain_local-0.0.6.tar` & `internet_domain_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:43:22.223003 internet_domain_local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 14:43:22.223003 internet_domain_local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:43:22.219004 internet_domain_local-0.0.6/internet_domain_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:43:22.223003 internet_domain_local-0.0.6/internet_domain_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/internet_domain_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/internet_domain_local/src/internet_domain_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/internet_domain_local/src/internet_domain_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:43:22.223003 internet_domain_local-0.0.6/internet_domain_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 14:43:22.000000 internet_domain_local-0.0.6/internet_domain_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 14:43:22.000000 internet_domain_local-0.0.6/internet_domain_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:43:22.000000 internet_domain_local-0.0.6/internet_domain_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 14:43:22.000000 internet_domain_local-0.0.6/internet_domain_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 14:43:22.000000 internet_domain_local-0.0.6/internet_domain_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:43:22.223003 internet_domain_local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 14:43:01.000000 internet_domain_local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:20.253502 internet_domain_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 18:57:20.253502 internet_domain_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:20.249502 internet_domain_local-0.0.7/internet_domain_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:20.253502 internet_domain_local-0.0.7/internet_domain_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/internet_domain_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/internet_domain_local/src/internet_domain_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/internet_domain_local/src/internet_domain_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:20.253502 internet_domain_local-0.0.7/internet_domain_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 18:57:20.000000 internet_domain_local-0.0.7/internet_domain_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 18:57:20.000000 internet_domain_local-0.0.7/internet_domain_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:57:20.000000 internet_domain_local-0.0.7/internet_domain_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 18:57:20.000000 internet_domain_local-0.0.7/internet_domain_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 18:57:20.000000 internet_domain_local-0.0.7/internet_domain_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:57:20.253502 internet_domain_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 18:57:04.000000 internet_domain_local-0.0.7/setup.py
```

### Comparing `internet_domain_local-0.0.6/PKG-INFO` & `internet_domain_local-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet_domain_local-0.0.6/internet_domain_local/src/internet_domain_local.py` & `internet_domain_local-0.0.7/internet_domain_local/src/internet_domain_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,18 @@
                     ignore_duplicate=True
                 )
             # Add url to url_table
             # TODO: add url type
             parsed_url = urlparse(url)
             normalized_url = parsed_url.netloc + parsed_url.path.rstrip('/')
 
+            # Remove 'www.' prefix if it exists
+            if normalized_url.startswith('www.'):
+                normalized_url = normalized_url[4:]
+
             url_id = self.select_one_value_by_id(
                 schema_name='url',
                 view_table_name='url_view',
                 select_clause_value='url_id',
                 id_column_name='url',
                 id_column_value=normalized_url
             )
```

### Comparing `internet_domain_local-0.0.6/internet_domain_local/src/internet_domain_local_constants.py` & `internet_domain_local-0.0.7/internet_domain_local/src/internet_domain_local_constants.py`

 * *Files identical despite different names*

### Comparing `internet_domain_local-0.0.6/internet_domain_local.egg-info/PKG-INFO` & `internet_domain_local-0.0.7/internet_domain_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet_domain_local-0.0.6/setup.py` & `internet_domain_local-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "internet-domain-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
+    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles internet-domain-local Python",
     long_description="PyPI Package for Circles internet-domain-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/internet-domain-local-python-package",
     packages=[package_dir],
```
