# Comparing `tmp/pandoraPlugintools-1.0.8.tar.gz` & `tmp/pandoraPlugintools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoraPlugintools-1.0.8.tar", last modified: Tue Mar 12 14:52:14 2024, max compression
+gzip compressed data, was "pandoraPlugintools-1.0.9.tar", last modified: Wed Mar 20 12:32:21 2024, max compression
```

## Comparing `pandoraPlugintools-1.0.8.tar` & `pandoraPlugintools-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-12 14:52:14.716851 pandoraPlugintools-1.0.8/
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)    11357 2023-08-23 10:07:18.000000 pandoraPlugintools-1.0.8/LICENSE
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2889 2024-03-12 14:52:14.716851 pandoraPlugintools-1.0.8/PKG-INFO
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2372 2023-08-23 11:42:24.000000 pandoraPlugintools-1.0.8/README.md
-drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-12 14:52:14.715851 pandoraPlugintools-1.0.8/pandoraPlugintools/
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)      228 2023-09-19 10:39:47.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/__init__.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)    11193 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/agents.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     5353 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/discovery.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     5636 2023-11-07 12:26:55.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/encryption.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)    17012 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/general.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     4097 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/http.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)    15667 2024-03-12 13:58:51.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/modules.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     3724 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/output.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)    12304 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/snmp.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     7086 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/threads.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     8770 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.8/pandoraPlugintools/transfer.py
-drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-12 14:52:14.716851 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2889 2024-03-12 14:52:14.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/PKG-INFO
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)      615 2024-03-12 14:52:14.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/SOURCES.txt
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)        1 2024-03-12 14:52:14.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/dependency_links.txt
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)        1 2023-08-23 10:41:11.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/not-zip-safe
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)       79 2024-03-12 14:52:14.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/requires.txt
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)       19 2024-03-12 14:52:14.000000 pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/top_level.txt
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)      118 2024-03-12 14:52:14.716851 pandoraPlugintools-1.0.8/setup.cfg
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)      924 2024-03-12 14:47:28.000000 pandoraPlugintools-1.0.8/setup.py
+drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-20 12:32:21.121478 pandoraPlugintools-1.0.9/
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)    11357 2023-08-23 10:07:18.000000 pandoraPlugintools-1.0.9/LICENSE
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2889 2024-03-20 12:32:21.121478 pandoraPlugintools-1.0.9/PKG-INFO
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2372 2023-08-23 11:42:24.000000 pandoraPlugintools-1.0.9/README.md
+drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-20 12:32:21.120478 pandoraPlugintools-1.0.9/pandoraPlugintools/
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)      228 2023-09-19 10:39:47.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/__init__.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)    11193 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/agents.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     5353 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/discovery.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     5636 2023-11-07 12:26:55.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/encryption.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)    17012 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/general.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     4097 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/http.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)    15667 2024-03-12 13:58:51.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/modules.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     3724 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/output.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)    12304 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/snmp.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     7086 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/threads.py
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     8770 2023-08-22 08:12:27.000000 pandoraPlugintools-1.0.9/pandoraPlugintools/transfer.py
+drwxr-xr-x   0 alejandro  (1000) alejandro  (1000)        0 2024-03-20 12:32:21.121478 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)     2889 2024-03-20 12:32:21.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/PKG-INFO
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)      615 2024-03-20 12:32:21.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)        1 2024-03-20 12:32:21.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)        1 2023-08-23 10:41:11.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/not-zip-safe
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)       92 2024-03-20 12:32:21.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/requires.txt
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)       19 2024-03-20 12:32:21.000000 pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/top_level.txt
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)      118 2024-03-20 12:32:21.122478 pandoraPlugintools-1.0.9/setup.cfg
+-rw-r--r--   0 alejandro  (1000) alejandro  (1000)      939 2024-03-20 12:31:08.000000 pandoraPlugintools-1.0.9/setup.py
```

### Comparing `pandoraPlugintools-1.0.8/LICENSE` & `pandoraPlugintools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/PKG-INFO` & `pandoraPlugintools-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoraPlugintools
-Version: 1.0.8
+Version: 1.0.9
 Summary: A plugin tool set of functions for pandorafms
 Home-page: https://github.com/projects-pandorafms/pandoraPlugintools
 Author: PandoraFMS projects department
 Author-email: <projects@pandorafms.com>
 Keywords: python,pandora,pandorafms,plugintool,plugintools
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pandoraPlugintools-1.0.8/README.md` & `pandoraPlugintools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/agents.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/agents.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/discovery.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/discovery.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/encryption.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/encryption.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/general.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/general.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/http.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/http.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/modules.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/modules.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/output.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/output.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/snmp.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/snmp.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/threads.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/threads.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools/transfer.py` & `pandoraPlugintools-1.0.9/pandoraPlugintools/transfer.py`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/PKG-INFO` & `pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoraPlugintools
-Version: 1.0.8
+Version: 1.0.9
 Summary: A plugin tool set of functions for pandorafms
 Home-page: https://github.com/projects-pandorafms/pandoraPlugintools
 Author: PandoraFMS projects department
 Author-email: <projects@pandorafms.com>
 Keywords: python,pandora,pandorafms,plugintool,plugintools
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pandoraPlugintools-1.0.8/pandoraPlugintools.egg-info/SOURCES.txt` & `pandoraPlugintools-1.0.9/pandoraPlugintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandoraPlugintools-1.0.8/setup.py` & `pandoraPlugintools-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     readme = f.read()
 
 # Setting up
 setup(
     name="pandoraPlugintools",
-    version="1.0.8",
+    version="1.0.9",
     author="PandoraFMS projects department",
     author_email="<projects@pandorafms.com>",
     description="A plugin tool set of functions for pandorafms",
     long_description=readme,
     long_description_content_type='text/markdown',
     url = 'https://github.com/projects-pandorafms/pandoraPlugintools',
     packages=find_packages(),
     zip_safe=False,
-    install_requires=['datetime', 'cryptography>=3', 'requests', 'requests_ntlm','pycrypto>=2.6.1','pysnmp>=4.4.12'],
+    install_requires=['datetime', 'cryptography>=3', 'requests', 'requests_ntlm','pycrypto>=2.6.1','pysnmp>=4.4.12','pycryptodome'],
     keywords=['python', 'pandora', 'pandorafms', 'plugintool', 'plugintools'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
     ]
 )
```

