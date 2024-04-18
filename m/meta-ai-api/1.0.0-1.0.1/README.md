# Comparing `tmp/meta_ai_api-1.0.0.tar.gz` & `tmp/meta_ai_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.0.tar", last modified: Thu Apr 18 21:19:32 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.1.tar", last modified: Thu Apr 18 21:22:47 2024, max compression
```

## Comparing `meta_ai_api-1.0.0.tar` & `meta_ai_api-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:19:32.577049 meta_ai_api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-18 21:19:32.577049 meta_ai_api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 21:19:27.000000 meta_ai_api-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 21:19:27.000000 meta_ai_api-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:19:32.581049 meta_ai_api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-18 21:19:27.000000 meta_ai_api-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:19:32.577049 meta_ai_api-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:19:32.577049 meta_ai_api-1.0.0/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:19:27.000000 meta_ai_api-1.0.0/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-18 21:19:27.000000 meta_ai_api-1.0.0/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:19:32.577049 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-18 21:19:32.000000 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:19:32.000000 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:19:32.000000 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 21:19:32.000000 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:19:32.000000 meta_ai_api-1.0.0/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.585205 meta_ai_api-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.0/PKG-INFO` & `meta_ai_api-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
-Requires-Dist: lxml_html_cleaner
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI
 
 MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
```

### Comparing `meta_ai_api-1.0.0/README.md` & `meta_ai_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.0/setup.py` & `meta_ai_api-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     extras_require={
         "dev": ["check-manifest"],
     },
-    install_requires=["requests", "requests-html", "lxml_html_cleaner"],
+    install_requires=["requests", "requests-html"],
 )
```

### Comparing `meta_ai_api-1.0.0/src/meta_ai_api/main.py` & `meta_ai_api-1.0.1/src/meta_ai_api/main.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.0/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.1/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
-Requires-Dist: lxml_html_cleaner
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI
 
 MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
```

