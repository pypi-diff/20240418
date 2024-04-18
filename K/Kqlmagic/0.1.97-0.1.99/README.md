# Comparing `tmp/Kqlmagic-0.1.97.tar.gz` & `tmp/Kqlmagic-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Kqlmagic-0.1.97.tar", last modified: Tue May  7 17:56:01 2019, max compression
+gzip compressed data, was "dist\Kqlmagic-0.1.99.tar", last modified: Sun Jun  9 12:30:01 2019, max compression
```

## Comparing `Kqlmagic-0.1.97.tar` & `Kqlmagic-0.1.99.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/
--rw-rw-rw-   0        0        0     7571 2019-05-07 17:35:32.000000 Kqlmagic-0.1.97/HISTORY.rst
--rw-rw-rw-   0        0        0     1129 2018-12-20 19:59:06.000000 Kqlmagic-0.1.97/LICENSE.TXT
--rw-rw-rw-   0        0        0       60 2018-12-20 19:59:06.000000 Kqlmagic-0.1.97/MANIFEST.in
--rw-rw-rw-   0        0        0        0 2018-12-20 19:59:06.000000 Kqlmagic-0.1.97/NEWS.txt
--rw-rw-rw-   0        0        0      156 2018-12-20 19:59:06.000000 Kqlmagic-0.1.97/NOTICE.TXT
--rw-rw-rw-   0        0        0     5021 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2019-01-02 16:16:01.000000 Kqlmagic-0.1.97/README.rst
-drwxrwxrwx   0        0        0        0 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/azure/
-drwxrwxrwx   0        0        0        0 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/azure/Kqlmagic/
--rw-rw-rw-   0        0        0      404 2018-12-20 19:59:06.000000 Kqlmagic-0.1.97/azure/Kqlmagic/__init__.py
--rw-rw-rw-   0        0        0     4699 2019-03-31 18:07:54.000000 Kqlmagic-0.1.97/azure/Kqlmagic/adal_token_cache.py
--rw-rw-rw-   0        0        0     1870 2019-04-07 12:52:55.000000 Kqlmagic-0.1.97/azure/Kqlmagic/ai_engine.py
--rw-rw-rw-   0        0        0     5686 2019-04-08 10:45:10.000000 Kqlmagic-0.1.97/azure/Kqlmagic/cache_client.py
--rw-rw-rw-   0        0        0     5957 2019-04-07 16:56:32.000000 Kqlmagic-0.1.97/azure/Kqlmagic/cache_engine.py
--rw-rw-rw-   0        0        0    10238 2019-03-18 12:43:17.000000 Kqlmagic-0.1.97/azure/Kqlmagic/column_guesser.py
--rw-rw-rw-   0        0        0     6753 2019-04-07 17:05:55.000000 Kqlmagic-0.1.97/azure/Kqlmagic/connection.py
--rw-rw-rw-   0        0        0     7384 2018-12-20 19:59:07.000000 Kqlmagic-0.1.97/azure/Kqlmagic/constants.py
--rw-rw-rw-   0        0        0    10012 2019-04-07 10:10:28.000000 Kqlmagic-0.1.97/azure/Kqlmagic/database_html.py
--rw-rw-rw-   0        0        0    12510 2019-04-08 12:54:17.000000 Kqlmagic-0.1.97/azure/Kqlmagic/display.py
--rw-rw-rw-   0        0        0     5842 2019-03-31 16:00:30.000000 Kqlmagic-0.1.97/azure/Kqlmagic/draft_client.py
--rw-rw-rw-   0        0        0    21011 2019-01-16 20:55:31.000000 Kqlmagic-0.1.97/azure/Kqlmagic/help.py
--rw-rw-rw-   0        0        0     3807 2018-12-20 19:59:07.000000 Kqlmagic-0.1.97/azure/Kqlmagic/help_html.py
--rw-rw-rw-   0        0        0    14402 2019-02-19 10:35:16.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kql_client.py
--rw-rw-rw-   0        0        0    13311 2019-05-07 15:28:37.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kql_engine.py
--rw-rw-rw-   0        0        0    62093 2019-04-08 12:55:20.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kql_magic.py
--rw-rw-rw-   0        0        0     7822 2019-01-23 11:40:55.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kql_proxy.py
--rw-rw-rw-   0        0        0     8039 2019-05-07 17:54:11.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kusto_client.py
--rw-rw-rw-   0        0        0     3541 2019-04-08 09:40:41.000000 Kqlmagic-0.1.97/azure/Kqlmagic/kusto_engine.py
--rw-rw-rw-   0        0        0     1775 2018-12-20 19:59:07.000000 Kqlmagic-0.1.97/azure/Kqlmagic/la_engine.py
--rw-rw-rw-   0        0        0     5863 2019-03-31 14:26:57.000000 Kqlmagic-0.1.97/azure/Kqlmagic/log.py
--rw-rw-rw-   0        0        0     2557 2019-04-08 09:03:31.000000 Kqlmagic-0.1.97/azure/Kqlmagic/magic_extension.py
--rw-rw-rw-   0        0        0    10508 2019-05-07 17:37:56.000000 Kqlmagic-0.1.97/azure/Kqlmagic/my_aad_helper.py
--rw-rw-rw-   0        0        0     2923 2019-05-07 17:54:11.000000 Kqlmagic-0.1.97/azure/Kqlmagic/my_utils.py
--rw-rw-rw-   0        0        0    12156 2018-12-30 01:07:19.000000 Kqlmagic-0.1.97/azure/Kqlmagic/palette.py
--rw-rw-rw-   0        0        0    10957 2019-04-05 22:39:14.000000 Kqlmagic-0.1.97/azure/Kqlmagic/parameterizer.py
--rw-rw-rw-   0        0        0    32004 2019-05-07 17:54:11.000000 Kqlmagic-0.1.97/azure/Kqlmagic/parser.py
--rw-rw-rw-   0        0        0    52811 2019-05-07 15:32:29.000000 Kqlmagic-0.1.97/azure/Kqlmagic/results.py
--rw-rw-rw-   0        0        0     5352 2019-05-07 17:55:00.000000 Kqlmagic-0.1.97/azure/Kqlmagic/version.py
-drwxrwxrwx   0        0        0        0 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/
--rw-rw-rw-   0        0        0     5021 2019-05-07 17:56:00.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-05-07 17:56:00.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-12-20 20:54:20.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      276 2019-05-07 17:56:00.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2019-05-07 17:56:00.000000 Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2377 2018-12-20 19:59:07.000000 Kqlmagic-0.1.97/azure_bdist_wheel.py
--rw-rw-rw-   0        0        0      105 2018-12-20 19:59:07.000000 Kqlmagic-0.1.97/dev_requirements.txt
--rw-rw-rw-   0        0        0       42 2019-05-07 17:56:01.000000 Kqlmagic-0.1.97/setup.cfg
--rw-rw-rw-   0        0        0     3732 2019-03-24 15:42:00.000000 Kqlmagic-0.1.97/setup.py
+drwxrwxrwx   0        0        0        0 2019-06-09 12:30:00.000000 Kqlmagic-0.1.99/
+-rw-rw-rw-   0        0        0     7571 2019-05-07 17:35:32.000000 Kqlmagic-0.1.99/HISTORY.rst
+-rw-rw-rw-   0        0        0     1129 2018-12-20 19:59:06.000000 Kqlmagic-0.1.99/LICENSE.TXT
+-rw-rw-rw-   0        0        0       60 2018-12-20 19:59:06.000000 Kqlmagic-0.1.99/MANIFEST.in
+-rw-rw-rw-   0        0        0        0 2018-12-20 19:59:06.000000 Kqlmagic-0.1.99/NEWS.txt
+-rw-rw-rw-   0        0        0      156 2018-12-20 19:59:06.000000 Kqlmagic-0.1.99/NOTICE.TXT
+-rw-rw-rw-   0        0        0     5042 2019-06-09 12:30:00.000000 Kqlmagic-0.1.99/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2019-01-02 16:16:01.000000 Kqlmagic-0.1.99/README.rst
+-rw-rw-rw-   0        0        0      990 2019-06-09 12:26:18.000000 Kqlmagic-0.1.99/TODO.txt
+drwxrwxrwx   0        0        0        0 2019-06-09 12:30:00.000000 Kqlmagic-0.1.99/azure/
+drwxrwxrwx   0        0        0        0 2019-06-09 12:30:00.000000 Kqlmagic-0.1.99/azure/Kqlmagic/
+-rw-rw-rw-   0        0        0      404 2018-12-20 19:59:06.000000 Kqlmagic-0.1.99/azure/Kqlmagic/__init__.py
+-rw-rw-rw-   0        0        0     4699 2019-03-31 18:07:54.000000 Kqlmagic-0.1.99/azure/Kqlmagic/adal_token_cache.py
+-rw-rw-rw-   0        0        0     1870 2019-04-07 12:52:55.000000 Kqlmagic-0.1.99/azure/Kqlmagic/ai_engine.py
+-rw-rw-rw-   0        0        0     5686 2019-04-08 10:45:10.000000 Kqlmagic-0.1.99/azure/Kqlmagic/cache_client.py
+-rw-rw-rw-   0        0        0     5957 2019-04-07 16:56:32.000000 Kqlmagic-0.1.99/azure/Kqlmagic/cache_engine.py
+-rw-rw-rw-   0        0        0    10238 2019-03-18 12:43:17.000000 Kqlmagic-0.1.99/azure/Kqlmagic/column_guesser.py
+-rw-rw-rw-   0        0        0     6753 2019-04-07 17:05:55.000000 Kqlmagic-0.1.99/azure/Kqlmagic/connection.py
+-rw-rw-rw-   0        0        0     7384 2018-12-20 19:59:07.000000 Kqlmagic-0.1.99/azure/Kqlmagic/constants.py
+-rw-rw-rw-   0        0        0    10012 2019-04-07 10:10:28.000000 Kqlmagic-0.1.99/azure/Kqlmagic/database_html.py
+-rw-rw-rw-   0        0        0    12510 2019-04-08 12:54:17.000000 Kqlmagic-0.1.99/azure/Kqlmagic/display.py
+-rw-rw-rw-   0        0        0     5842 2019-03-31 16:00:30.000000 Kqlmagic-0.1.99/azure/Kqlmagic/draft_client.py
+-rw-rw-rw-   0        0        0    21011 2019-01-16 20:55:31.000000 Kqlmagic-0.1.99/azure/Kqlmagic/help.py
+-rw-rw-rw-   0        0        0     3807 2018-12-20 19:59:07.000000 Kqlmagic-0.1.99/azure/Kqlmagic/help_html.py
+-rw-rw-rw-   0        0        0    14402 2019-02-19 10:35:16.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kql_client.py
+-rw-rw-rw-   0        0        0    13311 2019-05-07 15:28:37.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kql_engine.py
+-rw-rw-rw-   0        0        0    62095 2019-06-03 13:15:04.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kql_magic.py
+-rw-rw-rw-   0        0        0     7822 2019-01-23 11:40:55.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kql_proxy.py
+-rw-rw-rw-   0        0        0     8248 2019-06-03 13:12:09.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kusto_client.py
+-rw-rw-rw-   0        0        0     3541 2019-04-08 09:40:41.000000 Kqlmagic-0.1.99/azure/Kqlmagic/kusto_engine.py
+-rw-rw-rw-   0        0        0     1775 2018-12-20 19:59:07.000000 Kqlmagic-0.1.99/azure/Kqlmagic/la_engine.py
+-rw-rw-rw-   0        0        0     5863 2019-03-31 14:26:57.000000 Kqlmagic-0.1.99/azure/Kqlmagic/log.py
+-rw-rw-rw-   0        0        0     2557 2019-04-08 09:03:31.000000 Kqlmagic-0.1.99/azure/Kqlmagic/magic_extension.py
+-rw-rw-rw-   0        0        0    10508 2019-05-07 17:37:56.000000 Kqlmagic-0.1.99/azure/Kqlmagic/my_aad_helper.py
+-rw-rw-rw-   0        0        0     2923 2019-05-07 17:54:11.000000 Kqlmagic-0.1.99/azure/Kqlmagic/my_utils.py
+-rw-rw-rw-   0        0        0    12156 2018-12-30 01:07:19.000000 Kqlmagic-0.1.99/azure/Kqlmagic/palette.py
+-rw-rw-rw-   0        0        0    10957 2019-04-05 22:39:14.000000 Kqlmagic-0.1.99/azure/Kqlmagic/parameterizer.py
+-rw-rw-rw-   0        0        0    32004 2019-05-07 17:54:11.000000 Kqlmagic-0.1.99/azure/Kqlmagic/parser.py
+-rw-rw-rw-   0        0        0    53413 2019-06-09 12:26:18.000000 Kqlmagic-0.1.99/azure/Kqlmagic/results.py
+-rw-rw-rw-   0        0        0     5352 2019-06-09 12:19:23.000000 Kqlmagic-0.1.99/azure/Kqlmagic/version.py
+drwxrwxrwx   0        0        0        0 2019-06-09 12:30:00.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/
+-rw-rw-rw-   0        0        0     5042 2019-06-09 12:29:58.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2019-06-09 12:29:59.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-06-09 12:29:58.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-12-20 20:54:20.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      343 2019-06-09 12:29:58.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2019-06-09 12:29:58.000000 Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2377 2018-12-20 19:59:07.000000 Kqlmagic-0.1.99/azure_bdist_wheel.py
+-rw-rw-rw-   0        0        0      105 2018-12-20 19:59:07.000000 Kqlmagic-0.1.99/dev_requirements.txt
+-rw-rw-rw-   0        0        0       42 2019-06-09 12:30:01.000000 Kqlmagic-0.1.99/setup.cfg
+-rw-rw-rw-   0        0        0     3940 2019-06-04 08:21:29.000000 Kqlmagic-0.1.99/setup.py
```

### Comparing `Kqlmagic-0.1.97/HISTORY.rst` & `Kqlmagic-0.1.99/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/LICENSE.TXT` & `Kqlmagic-0.1.99/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/PKG-INFO` & `Kqlmagic-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: Kqlmagic
-Version: 0.1.97
+Version: 0.1.99
 Summary: Kqlmagic: Microsoft Azure Monitor magic extension to Jupyter notebook
 Home-page: https://github.com/Microsoft/jupyter-Kqlmagic
 Author: Michael Binshtock
 Author-email: michabin@microsoft.com
 Maintainer: Michael Binshtock
 Maintainer-email: michabin@microsoft.com
 License: MIT License
@@ -111,7 +111,8 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
+Provides-Extra: dev
```

### Comparing `Kqlmagic-0.1.97/README.rst` & `Kqlmagic-0.1.99/README.rst`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/adal_token_cache.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/adal_token_cache.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/ai_engine.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/ai_engine.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/cache_client.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/cache_client.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/cache_engine.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/cache_engine.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/column_guesser.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/column_guesser.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/connection.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/connection.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/constants.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/constants.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/database_html.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/database_html.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/display.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/display.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/draft_client.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/draft_client.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/help.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/help.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/help_html.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/help_html.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kql_client.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kql_client.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kql_engine.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kql_engine.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kql_magic.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kql_magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,18 +316,18 @@
             </head>
             <body>
                 <div class='kql-magic-banner'>
                     <div><img src='"""+logo+"""'></div>
                     <div>
                         <p>Kql Query Language, aka kql, is the query language for advanced analytics on Azure Monitor resources. The current supported data sources are 
                         Azure Data Explorer (Kusto), Log Analytics and Application Insights. To get more information execute '%kql --help "kql"'</p>
-                        <p>   &bull; kql reference: Click on 'Help' tab > and Select 'kql referece' or execute '%kql --help "kql"'<br>
+                        <p>   &bull; kql reference: Click on 'Help' tab > and Select 'kql reference' or execute '%kql --help "kql"'<br>
                           &bull; """
                 + Constants.MAGIC_CLASS_NAME
-                + """ configuarion: execute '%config """
+                + """ configuration: execute '%config """
                 + Constants.MAGIC_CLASS_NAME
                 + """'<br>
                           &bull; """
                 + Constants.MAGIC_CLASS_NAME
                 + """ usage: execute '%kql --usage'<br>
                     </div>
                 </div>
```

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kql_proxy.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kql_proxy.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kusto_client.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kusto_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 
     _DEFAULT_CLIENTID = "db662dc1-0cfe-4e1c-a843-19a68e65be58"  # kusto client app, (didn't find app name ?)
     #    _DEFAULT_CLIENTID = "8430759c-5626-4577-b151-d0755f5355d8" # kusto client app, don't know app name
     _MGMT_ENDPOINT_VERSION = "v1"
     _QUERY_ENDPOINT_VERSION = "v2"
     _MGMT_ENDPOINT_TEMPLATE = "{0}/{1}/rest/mgmt"
     _QUERY_ENDPOINT_TEMPLATE = "{0}/{1}/rest/query"
+    _PUBLIC_CLOUD_DATA_SOURCE = "windows.net"
+    _MOONCAKE_CLOUD_DATA_SOURCE = "chinacloudapi.cn"
+    _BLACKFOREST_CLOUD_DATA_SOURCE = "cloudapi.de"
+    _FAIRFAX_CLOUD_DATA_SOURCE = "usgovcloudapi.net"
+
     _DATA_SOURCE_TEMPLATE = "https://{0}.kusto.windows.net"
 
     _WEB_CLIENT_VERSION = VERSION
 
     def __init__(self, conn_kv:dict):
         """
         Kusto Client constructor.
```

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/kusto_engine.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/kusto_engine.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/la_engine.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/la_engine.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/log.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/log.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/magic_extension.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/magic_extension.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/my_aad_helper.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/my_aad_helper.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/my_utils.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/my_utils.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/palette.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/palette.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/parameterizer.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/parameterizer.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/parser.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/parser.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/results.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 from Kqlmagic.palette import Palette, Palettes
 
 import plotly
 
 import plotly.plotly as py
 import plotly.graph_objs as go
+try:
+    import ipywidgets
+except Exception:
+    ipywidgets_installed = False
+else:
+    ipywidgets_installed = True
 
 
 def _unduplicate_field_names(field_names):
     """Append a number to duplicate field names to make them unique. """
     res = []
     for k in field_names:
         if k in res:
@@ -460,15 +466,15 @@
         if window_mode and not options.get("button_text"):
             options["button_text"] = "popup " + self.visualization + ((" - " + self.title) if self.title else "") + " "
         c = self._getChartHtml(window_mode)
         if c.get("body") or c.get("head"):
             html = Display.toHtml(**c)
             Display.show(html, **options)
         elif c.get("fig"):
-            if Display.notebooks_host or options.get("notebook_app") in ["jupyterlab", "visualstudiocode", "ipython"]:
+            if not ipywidgets_installed or Display.notebooks_host or options.get("notebook_app") in ["jupyterlab", "visualstudiocode", "ipython"]:
                 plotly.offline.init_notebook_mode(connected=True)
                 plotly.offline.iplot(c.get("fig"), filename="plotlychart")
             else:
                 Display.show(c.get("fig"), **options)
         else:
             return self.show_table(**kwargs)
 
@@ -939,14 +945,22 @@
             chart_properties["orientation"] = "v"
         chart_properties["autorange"] = "reversed" if tabs[0].is_descending_sorted else True
         chart_properties["showlegend"] = properties.get(VisualizationKeys.LEGEND) != VisualizationLegends.HIDDEN
         chart_properties["title"] = properties.get(VisualizationKeys.TITLE) or properties.get(VisualizationKeys.VISUALIZATION)
         chart_properties["n_colors"] = len(tabs)
         return chart_properties
 
+    def _figure_or_figurewidget(self, data, layout):
+        if ipywidgets_installed:
+            # print("----------- FigureWidget --------------")
+            fig = go.FigureWidget(data=data, layout=layout)
+        else:
+            # print("----------- Figure --------------")
+            fig = go.Figure(data=data, layout=layout)
+        return fig
 
     def _render_areachart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Area graph. 
         First column is x-axis, and should be a numeric column. Other numeric columns are y-axes.
         """
@@ -979,15 +993,15 @@
                 title=chart_properties["ylabel"],
                 type=chart_properties["yscale"],
                 # range=[0, 3],
                 # dtick=20,
                 ticksuffix="",
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
     def _render_stackedareachart_plotly(self, properties:dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Stacked area graph. 
         First column is x-axis, and should be a numeric column. Other numeric columns are y-axes.
@@ -1029,15 +1043,15 @@
                 title=chart_properties["ylabel"],
                 type=chart_properties["yscale"],
                 # range=[0, 3],
                 # dtick=20,
                 ticksuffix="",
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
     def _render_timechart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Line graph. 
         First column is x-axis, and should be datetime. Other columns are y-axes.
@@ -1081,15 +1095,15 @@
                 title=chart_properties["ylabel"],
                 type=chart_properties["yscale"],
                 # range=[0, 3],
                 # dtick=20,
                 ticksuffix="",
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
     def _render_piechart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Pie chart. 
         First column is color-axis, second column is numeric.
@@ -1144,15 +1158,15 @@
                     showarrow=False,
                     x=(domains[idx].get("x")[0] + domains[idx].get("x")[1]) / 2,
                     y=domains[idx].get("y")[0] - 0.05 * ydelta,
                 )
                 for idx, tab in enumerate(self.chart_sub_tables)
             ],
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
     def _render_barchart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Bar chart. 
         First column is x-axis, and can be text, datetime or numeric. Other columns are numeric, displayed as horizontal strips.
@@ -1185,15 +1199,15 @@
                 ticksuffix="",
             ),
             yaxis=dict(
                 type=chart_properties["yscale"],
                 title=chart_properties["ylabel"],
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
 
     def _render_linechart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Line graph. 
@@ -1227,15 +1241,15 @@
                 title=chart_properties["ylabel"],
                 type=chart_properties["yscale"],
                 # range=[0, 3],
                 # dtick=20,
                 # ticksuffix=''
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
     def _render_scatterchart_plotly(self, properties: dict, key_word_sep=" ", **kwargs):
         """Generates a pylab plot from the result set.
 
         Points graph. 
         First column is x-axis, and should be a numeric column. Other numeric columns are y-axes.
@@ -1268,15 +1282,15 @@
                 title=chart_properties["ylabel"],
                 type=chart_properties["yscale"],
                 # range=[0, 3],
                 # dtick=20,
                 ticksuffix="",
             ),
         )
-        fig = go.FigureWidget(data=data, layout=layout)
+        fig = self._figure_or_figurewidget(data=data, layout=layout)
         return fig
 
 
 class PrettyTable(prettytable.PrettyTable):
 
     # Object constructor
     def __init__(self, *args, **kwargs):
```

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic/version.py` & `Kqlmagic-0.1.99/azure/Kqlmagic/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """A module that manage package version.
 """
 
-VERSION = "0.1.97"
+VERSION = "0.1.99"
 
 import sys
 import requests
 from Kqlmagic.constants import Constants
 from Kqlmagic.help import MarkdownString
```

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/PKG-INFO` & `Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: Kqlmagic
-Version: 0.1.97
+Version: 0.1.99
 Summary: Kqlmagic: Microsoft Azure Monitor magic extension to Jupyter notebook
 Home-page: https://github.com/Microsoft/jupyter-Kqlmagic
 Author: Michael Binshtock
 Author-email: michabin@microsoft.com
 Maintainer: Michael Binshtock
 Maintainer-email: michabin@microsoft.com
 License: MIT License
@@ -111,7 +111,8 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
+Provides-Extra: dev
```

### Comparing `Kqlmagic-0.1.97/azure/Kqlmagic.egg-info/SOURCES.txt` & `Kqlmagic-0.1.99/azure/Kqlmagic.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 HISTORY.rst
 LICENSE.TXT
 MANIFEST.in
 NEWS.txt
 NOTICE.TXT
 README.rst
+TODO.txt
 azure_bdist_wheel.py
 dev_requirements.txt
 setup.py
 azure/Kqlmagic/__init__.py
 azure/Kqlmagic/adal_token_cache.py
 azure/Kqlmagic/ai_engine.py
 azure/Kqlmagic/cache_client.py
```

### Comparing `Kqlmagic-0.1.97/azure_bdist_wheel.py` & `Kqlmagic-0.1.99/azure_bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `Kqlmagic-0.1.97/setup.py` & `Kqlmagic-0.1.99/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,42 @@
 
 LICENSE             = 'MIT License'
 
 KEYWORDS            = 'database ipython jupyter jupyterlab jupyter-notebook query language kql kusto loganalytics applicationinsights'
 
 INSTALL_REQUIRES    = [
                         'ipython>=7.1.1',
-                        'plotly>=3.6.1',
+                        'plotly>=3.8.1',
                         'prettytable>=0.7.2',
                         'matplotlib>=3.0.0',
-                        'pandas>=0.22.0',
+                        'pandas>=0.23.4',
                         'adal>=1.2.1',
                         'Pygments>=2.2.0',
                         'seaborn>=0.9.0',
                         'requests>=2.21.0',
                         'python-dateutil>=2.7.5',
                         'traitlets>=4.3.2',
                         'psutil>=5.4.7',
                         'six>=1.11.0',
-                        'setuptools>=40.8.0',
+                        'setuptools>=41.0.1',
                         'Markdown>=3.0.1',
                         'beautifulsoup4>=4.6.3',
                         'lxml>=4.2.5',
 ]
 
+EXTRAS_REQUIRE      = {
+    'dev':  [
+        'pytest',
+        'pytest-pep8',
+        'pytest-docstyle',
+        'pytest-flakes',
+        'pytest-cov',
+    ]
+}
+
 
 # To use a consistent encoding
 import codecs
 
 import re
 from os import path
 
@@ -103,8 +113,9 @@
     license=LICENSE,
     python_requires='>=3.6',
     packages=find_packages('azure'),
     package_dir = {'': 'azure'},
     include_package_data=True,
     zip_safe=False,
     install_requires=INSTALL_REQUIRES,
+    extras_require=EXTRAS_REQUIRE,
 )
```

