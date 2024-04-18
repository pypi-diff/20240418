# Comparing `tmp/liquer-framework-0.9.6.tar.gz` & `tmp/liquer-framework-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquer-framework-0.9.6.tar", last modified: Mon Jan 15 18:30:09 2024, max compression
+gzip compressed data, was "liquer-framework-0.9.7.tar", last modified: Wed Apr 17 20:41:16 2024, max compression
```

## Comparing `liquer-framework-0.9.6.tar` & `liquer-framework-0.9.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:09.086314 liquer-framework-0.9.6/
--rw-rw-rw-   0        0        0     1068 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/LICENSE
--rw-rw-rw-   0        0        0       77 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7467 2024-01-15 18:30:09.086314 liquer-framework-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     6941 2024-01-15 18:25:10.000000 liquer-framework-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:08.749698 liquer-framework-0.9.6/liquer/
--rw-rw-rw-   0        0        0      436 2024-01-15 18:25:49.000000 liquer-framework-0.9.6/liquer/__init__.py
--rw-rw-rw-   0        0        0     2217 2023-12-17 19:54:18.000000 liquer-framework-0.9.6/liquer/app.py
--rw-rw-rw-   0        0        0      332 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/blueprint.py
--rw-rw-rw-   0        0        0    30438 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/cache.py
--rw-rw-rw-   0        0        0    32154 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/commands.py
--rw-rw-rw-   0        0        0    18299 2024-01-08 20:54:44.000000 liquer-framework-0.9.6/liquer/config.py
--rw-rw-rw-   0        0        0     4034 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/constants.py
--rw-rw-rw-   0        0        0    48720 2024-01-15 18:20:50.000000 liquer-framework-0.9.6/liquer/context.py
--rw-rw-rw-   0        0        0     3918 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:08.905923 liquer-framework-0.9.6/liquer/ext/
--rw-rw-rw-   0        0        0       37 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/__init__.py
--rw-rw-rw-   0        0        0     9243 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/basic.py
--rw-rw-rw-   0        0        0    13175 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/dataframe_batches.py
--rw-rw-rw-   0        0        0     7937 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_datafusion.py
--rw-rw-rw-   0        0        0     4381 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_hxl.py
--rw-rw-rw-   0        0        0     3933 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_keras.py
--rw-rw-rw-   0        0        0     3686 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_matplotlib.py
--rw-rw-rw-   0        0        0     3447 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_openpyxl.py
--rw-rw-rw-   0        0        0    16425 2024-01-15 17:37:08.000000 liquer-framework-0.9.6/liquer/ext/lq_pandas.py
--rw-rw-rw-   0        0        0     3432 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_pil.py
--rw-rw-rw-   0        0        0     2304 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_plotly.py
--rw-rw-rw-   0        0        0     8226 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_polars.py
--rw-rw-rw-   0        0        0     2244 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_pptx.py
--rw-rw-rw-   0        0        0      701 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_pygments.py
--rw-rw-rw-   0        0        0      368 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_python.py
--rw-rw-rw-   0        0        0     1729 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_sklearn_regression.py
--rw-rw-rw-   0        0        0      712 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_sweetviz.py
--rw-rw-rw-   0        0        0     4222 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_whoosh.html
--rw-rw-rw-   0        0        0     4300 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/ext/lq_whoosh.py
--rw-rw-rw-   0        0        0    16597 2023-08-29 15:12:47.000000 liquer-framework-0.9.6/liquer/ext/meta.py
--rw-rw-rw-   0        0        0     7326 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/indexer.py
--rw-rw-rw-   0        0        0     7694 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/metadata.py
--rw-rw-rw-   0        0        0    35759 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/parser.py
--rw-rw-rw-   0        0        0    12019 2023-12-25 23:52:40.000000 liquer-framework-0.9.6/liquer/pool.py
--rw-rw-rw-   0        0        0     1251 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/query.py
--rw-rw-rw-   0        0        0    37374 2023-08-29 14:57:49.000000 liquer-framework-0.9.6/liquer/recipes.py
--rw-rw-rw-   0        0        0     4247 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/remote_store.py
--rw-rw-rw-   0        0        0     6160 2023-12-28 14:43:31.000000 liquer-framework-0.9.6/liquer/s3_store.py
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:08.922021 liquer-framework-0.9.6/liquer/server/
--rw-rw-rw-   0        0        0       63 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/server/__init__.py
--rw-rw-rw-   0        0        0    15042 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/server/blueprint.py
--rw-rw-rw-   0        0        0    15299 2024-01-08 20:39:25.000000 liquer-framework-0.9.6/liquer/server/fastapi.py
--rw-rw-rw-   0        0        0    19966 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/server/handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:09.022416 liquer-framework-0.9.6/liquer/server/static/
--rw-rw-rw-   0        0        0    26489 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/server/static/index.html
--rw-rw-rw-   0        0        0    18057 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/server/static/liquer.js
--rw-rw-rw-   0        0        0     7358 2024-01-08 21:04:18.000000 liquer-framework-0.9.6/liquer/server/tornado_handlers.py
--rw-rw-rw-   0        0        0     8335 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/state.py
--rw-rw-rw-   0        0        0    17774 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/state_types.py
--rw-rw-rw-   0        0        0    54232 2023-12-28 14:41:18.000000 liquer-framework-0.9.6/liquer/store.py
--rw-rw-rw-   0        0        0    11327 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/template.py
--rw-rw-rw-   0        0        0      660 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/tools.py
--rw-rw-rw-   0        0        0     1022 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/util.py
--rw-rw-rw-   0        0        0     2835 2023-08-27 14:29:31.000000 liquer-framework-0.9.6/liquer/web.py
-drwxrwxrwx   0        0        0        0 2024-01-15 18:30:09.082310 liquer-framework-0.9.6/liquer_framework.egg-info/
--rw-rw-rw-   0        0        0     7467 2024-01-15 18:30:07.000000 liquer-framework-0.9.6/liquer_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2024-01-15 18:30:08.000000 liquer-framework-0.9.6/liquer_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-15 18:30:07.000000 liquer-framework-0.9.6/liquer_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-17 20:08:37.000000 liquer-framework-0.9.6/liquer_framework.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-01-15 18:30:07.000000 liquer-framework-0.9.6/liquer_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-15 18:30:07.000000 liquer-framework-0.9.6/liquer_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-15 18:30:09.090313 liquer-framework-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      702 2024-01-15 18:25:23.000000 liquer-framework-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.238040 liquer-framework-0.9.7/
+-rw-rw-rw-   0        0        0     1068 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7515 2024-04-17 20:41:16.238040 liquer-framework-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6989 2024-04-17 20:36:56.000000 liquer-framework-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.194800 liquer-framework-0.9.7/liquer/
+-rw-rw-rw-   0        0        0      436 2024-04-17 20:37:36.000000 liquer-framework-0.9.7/liquer/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-12-17 19:54:18.000000 liquer-framework-0.9.7/liquer/app.py
+-rw-rw-rw-   0        0        0      332 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/blueprint.py
+-rw-rw-rw-   0        0        0    30438 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/cache.py
+-rw-rw-rw-   0        0        0    32154 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/commands.py
+-rw-rw-rw-   0        0        0    18299 2024-01-08 20:54:44.000000 liquer-framework-0.9.7/liquer/config.py
+-rw-rw-rw-   0        0        0     4034 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/constants.py
+-rw-rw-rw-   0        0        0    48720 2024-01-15 18:20:50.000000 liquer-framework-0.9.7/liquer/context.py
+-rw-rw-rw-   0        0        0     3918 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.216375 liquer-framework-0.9.7/liquer/ext/
+-rw-rw-rw-   0        0        0       37 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/__init__.py
+-rw-rw-rw-   0        0        0     9243 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/basic.py
+-rw-rw-rw-   0        0        0    13175 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/dataframe_batches.py
+-rw-rw-rw-   0        0        0     7937 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_datafusion.py
+-rw-rw-rw-   0        0        0     4381 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_hxl.py
+-rw-rw-rw-   0        0        0     3933 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_keras.py
+-rw-rw-rw-   0        0        0     3686 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_matplotlib.py
+-rw-rw-rw-   0        0        0     3447 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_openpyxl.py
+-rw-rw-rw-   0        0        0    16425 2024-01-15 17:37:08.000000 liquer-framework-0.9.7/liquer/ext/lq_pandas.py
+-rw-rw-rw-   0        0        0     3432 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_pil.py
+-rw-rw-rw-   0        0        0     2304 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_plotly.py
+-rw-rw-rw-   0        0        0     8226 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_polars.py
+-rw-rw-rw-   0        0        0     2244 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_pptx.py
+-rw-rw-rw-   0        0        0      701 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_pygments.py
+-rw-rw-rw-   0        0        0      368 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_python.py
+-rw-rw-rw-   0        0        0     1729 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_sklearn_regression.py
+-rw-rw-rw-   0        0        0      712 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_sweetviz.py
+-rw-rw-rw-   0        0        0     4222 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_whoosh.html
+-rw-rw-rw-   0        0        0     4300 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/ext/lq_whoosh.py
+-rw-rw-rw-   0        0        0    16597 2023-08-29 15:12:47.000000 liquer-framework-0.9.7/liquer/ext/meta.py
+-rw-rw-rw-   0        0        0     7326 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/indexer.py
+-rw-rw-rw-   0        0        0     7694 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/metadata.py
+-rw-rw-rw-   0        0        0    35759 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/parser.py
+-rw-rw-rw-   0        0        0    12019 2023-12-25 23:52:40.000000 liquer-framework-0.9.7/liquer/pool.py
+-rw-rw-rw-   0        0        0     1251 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/query.py
+-rw-rw-rw-   0        0        0    37374 2023-08-29 14:57:49.000000 liquer-framework-0.9.7/liquer/recipes.py
+-rw-rw-rw-   0        0        0     4247 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/remote_store.py
+-rw-rw-rw-   0        0        0     6160 2023-12-28 14:43:31.000000 liquer-framework-0.9.7/liquer/s3_store.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.222798 liquer-framework-0.9.7/liquer/server/
+-rw-rw-rw-   0        0        0       63 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/server/__init__.py
+-rw-rw-rw-   0        0        0    15042 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/server/blueprint.py
+-rw-rw-rw-   0        0        0    15299 2024-01-08 20:39:25.000000 liquer-framework-0.9.7/liquer/server/fastapi.py
+-rw-rw-rw-   0        0        0    19966 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/server/handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.224808 liquer-framework-0.9.7/liquer/server/static/
+-rw-rw-rw-   0        0        0    26489 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/server/static/index.html
+-rw-rw-rw-   0        0        0    18057 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/server/static/liquer.js
+-rw-rw-rw-   0        0        0     7358 2024-01-08 21:04:18.000000 liquer-framework-0.9.7/liquer/server/tornado_handlers.py
+-rw-rw-rw-   0        0        0     8335 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/state.py
+-rw-rw-rw-   0        0        0    17774 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/state_types.py
+-rw-rw-rw-   0        0        0    56370 2024-04-17 20:35:04.000000 liquer-framework-0.9.7/liquer/store.py
+-rw-rw-rw-   0        0        0    11327 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/template.py
+-rw-rw-rw-   0        0        0      660 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/tools.py
+-rw-rw-rw-   0        0        0     1022 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/util.py
+-rw-rw-rw-   0        0        0     2835 2023-08-27 14:29:31.000000 liquer-framework-0.9.7/liquer/web.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:41:16.237014 liquer-framework-0.9.7/liquer_framework.egg-info/
+-rw-rw-rw-   0        0        0     7515 2024-04-17 20:41:16.000000 liquer-framework-0.9.7/liquer_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2024-04-17 20:41:16.000000 liquer-framework-0.9.7/liquer_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:41:16.000000 liquer-framework-0.9.7/liquer_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-12-17 20:08:37.000000 liquer-framework-0.9.7/liquer_framework.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-04-17 20:41:16.000000 liquer-framework-0.9.7/liquer_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 20:41:16.000000 liquer-framework-0.9.7/liquer_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:41:16.238040 liquer-framework-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      702 2024-04-17 20:37:11.000000 liquer-framework-0.9.7/setup.py
```

### Comparing `liquer-framework-0.9.6/LICENSE` & `liquer-framework-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/PKG-INFO` & `liquer-framework-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.6
+Version: 0.9.7
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -110,8 +110,8 @@
 - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
 - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
 - 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
 - 2023-06-15 - v0.9.3  - fixing bug impacting evaluate_template with relative paths
 - 2023-12-17 - v0.9.4  - simplified quickstart, evaluate_on query
 - 2023-12-20 - v0.9.5  - python logging in context
 - 2024-01-15 - v0.9.6  - FastAPI, Godot webapps enabled, fixing bugs in evaluate_on
-
+- 2024-04-17 - v0.9.7  - fixing issue with rmdir
```

### Comparing `liquer-framework-0.9.6/README.md` & `liquer-framework-0.9.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -97,8 +97,8 @@
 - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
 - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
 - 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
 - 2023-06-15 - v0.9.3  - fixing bug impacting evaluate_template with relative paths
 - 2023-12-17 - v0.9.4  - simplified quickstart, evaluate_on query
 - 2023-12-20 - v0.9.5  - python logging in context
 - 2024-01-15 - v0.9.6  - FastAPI, Godot webapps enabled, fixing bugs in evaluate_on
-
+- 2024-04-17 - v0.9.7  - fixing issue with rmdir
```

### Comparing `liquer-framework-0.9.6/liquer/app.py` & `liquer-framework-0.9.7/liquer/app.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/cache.py` & `liquer-framework-0.9.7/liquer/cache.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/commands.py` & `liquer-framework-0.9.7/liquer/commands.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/config.py` & `liquer-framework-0.9.7/liquer/config.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/constants.py` & `liquer-framework-0.9.7/liquer/constants.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/context.py` & `liquer-framework-0.9.7/liquer/context.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/dependencies.py` & `liquer-framework-0.9.7/liquer/dependencies.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/basic.py` & `liquer-framework-0.9.7/liquer/ext/basic.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/dataframe_batches.py` & `liquer-framework-0.9.7/liquer/ext/dataframe_batches.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_datafusion.py` & `liquer-framework-0.9.7/liquer/ext/lq_datafusion.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_hxl.py` & `liquer-framework-0.9.7/liquer/ext/lq_hxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_keras.py` & `liquer-framework-0.9.7/liquer/ext/lq_keras.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_matplotlib.py` & `liquer-framework-0.9.7/liquer/ext/lq_matplotlib.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_openpyxl.py` & `liquer-framework-0.9.7/liquer/ext/lq_openpyxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_pandas.py` & `liquer-framework-0.9.7/liquer/ext/lq_pandas.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_pil.py` & `liquer-framework-0.9.7/liquer/ext/lq_pil.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_plotly.py` & `liquer-framework-0.9.7/liquer/ext/lq_plotly.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_polars.py` & `liquer-framework-0.9.7/liquer/ext/lq_polars.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_pptx.py` & `liquer-framework-0.9.7/liquer/ext/lq_pptx.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_pygments.py` & `liquer-framework-0.9.7/liquer/ext/lq_pygments.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_sklearn_regression.py` & `liquer-framework-0.9.7/liquer/ext/lq_sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_sweetviz.py` & `liquer-framework-0.9.7/liquer/ext/lq_sweetviz.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_whoosh.html` & `liquer-framework-0.9.7/liquer/ext/lq_whoosh.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/lq_whoosh.py` & `liquer-framework-0.9.7/liquer/ext/lq_whoosh.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/ext/meta.py` & `liquer-framework-0.9.7/liquer/ext/meta.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/indexer.py` & `liquer-framework-0.9.7/liquer/indexer.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/metadata.py` & `liquer-framework-0.9.7/liquer/metadata.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/parser.py` & `liquer-framework-0.9.7/liquer/parser.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/pool.py` & `liquer-framework-0.9.7/liquer/pool.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/query.py` & `liquer-framework-0.9.7/liquer/query.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/recipes.py` & `liquer-framework-0.9.7/liquer/recipes.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/remote_store.py` & `liquer-framework-0.9.7/liquer/remote_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/s3_store.py` & `liquer-framework-0.9.7/liquer/s3_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/blueprint.py` & `liquer-framework-0.9.7/liquer/server/blueprint.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/fastapi.py` & `liquer-framework-0.9.7/liquer/server/fastapi.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/handlers.py` & `liquer-framework-0.9.7/liquer/server/handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/static/index.html` & `liquer-framework-0.9.7/liquer/server/static/index.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/static/liquer.js` & `liquer-framework-0.9.7/liquer/server/static/liquer.js`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/server/tornado_handlers.py` & `liquer-framework-0.9.7/liquer/server/tornado_handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/state.py` & `liquer-framework-0.9.7/liquer/state.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/state_types.py` & `liquer-framework-0.9.7/liquer/state_types.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/store.py` & `liquer-framework-0.9.7/liquer/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,18 +298,19 @@
         """Store metadata only."""
         raise KeyNotSupportedStoreException(key=key, store=self)
 
     def remove(self, key):
         """Remove data and metadata associated with the key."""
         raise KeyNotFoundStoreException(key=key, store=self)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
         """Remove directory.
         The key must be a directory.
         It depends on the underlying store whether the directory must be empty.
+        If recursive is True, the directory is removed recursively.
         """
         raise KeyNotFoundStoreException(key=key, store=self)
 
     def contains(self, key):
         """Returns true if store contains the key."""
         return key == ""
 
@@ -494,16 +495,26 @@
         try:
             self.metadata_path_for_key(key).unlink()
         except FileNotFoundError:
             pass
 
         self.on_removed(key)
 
-    def removedir(self, key):
-        (self.path_for_key(key) / self.METADATA).rmdir()
+    def removedir(self, key, recursive=False):
+        if key in ("", None):
+            return
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
+        self.metadata_path_for_key(key).unlink(missing_ok=True)
+        if (self.path_for_key(key) / self.METADATA).exists():
+            (self.path_for_key(key) / self.METADATA).rmdir()
         self.path_for_key(key).rmdir()
         self.on_removed(key)
 
     def contains(self, key):
         if key in ("", None):
             return True
         return self.path_for_key(key).exists()
@@ -606,15 +617,23 @@
             pass
         try:
             del self.metadata[key]
         except KeyError:
             pass
         self.on_removed(key)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
+        if key in ("", None):
+            return
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
         if len(self.listdir(key)) == 0:
             try:
                 self.directories.remove(key)
             except KeyError:
                 pass
         self.on_removed(key)
 
@@ -697,16 +716,16 @@
         self._store.store_metadata(key, metadata)
         self.on_metadata_changed(key)
 
     def remove(self, key):
         self._store.remove(key)
         self.on_removed(key)
 
-    def removedir(self, key):
-        self._store.remove(key)
+    def removedir(self, key, recursive=False):
+        self._store.removedir(key, recursive=recursive)
         self.on_removed(key)
 
     def contains(self, key):
         return self._store.contains(key)
 
     def is_dir(self, key):
         return self._store.is_dir(key)
@@ -772,15 +791,15 @@
 
     def store_metadata(self, key, metadata):
         raise ReadOnlyStoreException(key=key, store=self)
 
     def remove(self, key):
         raise ReadOnlyStoreException(key=key, store=self)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
         raise ReadOnlyStoreException(key=key, store=self)
 
     def makedir(self, key):
         raise ReadOnlyStoreException(key=key, store=self)
 
     def __str__(self):
         return f"read only proxy of {self._store}"
@@ -841,15 +860,21 @@
         if key not in self.removed:
             if self.overlay.contains(key):
                 self.overlay.remove(key)
             if self.fallback.contains(key):
                 self.removed.add(key)
         self.on_removed(key)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
         if self.contains(key):
             if len(self.listdir(key)) == 0:
                 if self.overlay.contains(key):
                     self.overlay.remove(key)
                 else:
                     self.removed.add(key)
         self.on_removed(key)
@@ -953,16 +978,16 @@
         self.route_to(key).store_metadata(key, metadata)
         self.on_metadata_changed(key)
 
     def remove(self, key):
         self.route_to(key).remove(key)
         self.on_removed(key)
 
-    def removedir(self, key):
-        self.route_to(key).removedir(key)
+    def removedir(self, key, recursive=False):
+        self.route_to(key).removedir(key, recursive=recursive)
         self.on_removed(key)
 
     def contains(self, key):
         return self.route_to(key).contains(key)
 
     def is_dir(self, key):
         return self.route_to(key).is_dir(key)
@@ -1040,16 +1065,16 @@
         self.substore.store_metadata(self.translate_key(key), metadata)
         self.on_metadata_changed(key)
 
     def remove(self, key):
         self.substore.remove(self.translate_key(key))
         self.on_removed(key)
 
-    def removedir(self, key):
-        self.substore.removedir(self.translate_key(key))
+    def removedir(self, key, recursive=False):
+        self.substore.removedir(self.translate_key(key), recursive=recursive)
         self.on_removed(key)
 
     def contains(self, key):
         return self.substore.contains(self.translate_key(key))
 
     def is_dir(self, key):
         return self.substore.is_dir(self.translate_key(key))
@@ -1227,15 +1252,23 @@
             for prefix in self.default_store.keys():
                 if prefix.startswith(key + "/") or key in (None, ""):
                     v = prefix.split("/")
                     d.add(v[key_depth])
 
         return sorted(d)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
+        if key in ("", None):
+            return
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
         for k, store in self.routing_table:
             if k == key:
                 raise StoreException(
                     f"Can't remove {key} because it is a mount point of {repr(store)}",
                     key=key,
                     store=self,
                 )
@@ -1375,15 +1408,24 @@
             pass
         try:
             self.fs.remove(self.metadata_path_for_key(key))
         except:
             pass
         self.on_removed(key)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
+        if key in ("", None):
+            return
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
+        self.fs.remove(self.metadata_dir_path_for_key(key))
         metadir = self.path_for_key(key) + "/" + self.METADATA
         try:
             self.fs.removedir(metadir)
         except:
             pass
         self.fs.removedir(self.path_for_key(key))
         self.on_removed(key)
@@ -1567,15 +1609,29 @@
             pass
         try:
             self.fs.rm(self.metadata_path_for_key(key))
         except:
             pass
         self.on_removed(key)
 
-    def removedir(self, key):
+    def removedir(self, key, recursive=False):
+        if key in ("", None):
+            return
+        if recursive:
+            for k in self.listdir_keys(key):
+                if self.is_dir(k):
+                    self.removedir(k, recursive=True)
+                else:
+                    self.remove(k)
+
+        try:
+            self.fs.rm(self.metadata_path_for_key(key))
+        except:
+            pass
+
         metadir = self.path_for_key(key) + "/" + self.METADATA
         try:
             self.fs.rmdir(metadir)
         except:
             pass
         self.fs.rmdir(self.path_for_key(key))
         self.on_removed(key)
```

### Comparing `liquer-framework-0.9.6/liquer/template.py` & `liquer-framework-0.9.7/liquer/template.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/tools.py` & `liquer-framework-0.9.7/liquer/tools.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/util.py` & `liquer-framework-0.9.7/liquer/util.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer/web.py` & `liquer-framework-0.9.7/liquer/web.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/liquer_framework.egg-info/PKG-INFO` & `liquer-framework-0.9.7/liquer_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.6
+Version: 0.9.7
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -110,8 +110,8 @@
 - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
 - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
 - 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
 - 2023-06-15 - v0.9.3  - fixing bug impacting evaluate_template with relative paths
 - 2023-12-17 - v0.9.4  - simplified quickstart, evaluate_on query
 - 2023-12-20 - v0.9.5  - python logging in context
 - 2024-01-15 - v0.9.6  - FastAPI, Godot webapps enabled, fixing bugs in evaluate_on
-
+- 2024-04-17 - v0.9.7  - fixing issue with rmdir
```

### Comparing `liquer-framework-0.9.6/liquer_framework.egg-info/SOURCES.txt` & `liquer-framework-0.9.7/liquer_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.6/setup.py` & `liquer-framework-0.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liquer-framework",
-    version="0.9.6",
+    version="0.9.7",
     author="Orest Dubay",
     author_email="orest3.dubay@gmail.com",
     description="LiQuer - Query in (URL) link",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/orest-d/liquer",
     packages=setuptools.find_packages(),
```

