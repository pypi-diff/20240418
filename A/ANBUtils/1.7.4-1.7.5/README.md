# Comparing `tmp/ANBUtils-1.7.4.tar.gz` & `tmp/ANBUtils-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.7.4.tar", last modified: Tue Apr 16 09:45:08 2024, max compression
+gzip compressed data, was "dist/ANBUtils-1.7.5.tar", last modified: Thu Apr 18 06:28:34 2024, max compression
```

## Comparing `ANBUtils-1.7.4.tar` & `ANBUtils-1.7.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-16 09:45:08.464955 ANBUtils-1.7.4/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-16 09:45:08.463435 ANBUtils-1.7.4/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)    14032 2024-04-16 09:33:23.000000 ANBUtils-1.7.4/ANBUtils/DBWorker.py
--rw-r--r--   0 redbson    (501) staff       (20)      865 2024-03-28 10:31:28.000000 ANBUtils-1.7.4/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-07-11 07:09:11.000000 ANBUtils-1.7.4/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)     3186 2024-03-28 10:27:52.000000 ANBUtils-1.7.4/ANBUtils/db_tools.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.7.4/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)     1092 2023-07-03 10:30:53.000000 ANBUtils-1.7.4/ANBUtils/environ.py
--rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.7.4/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     2427 2024-03-28 04:40:26.000000 ANBUtils-1.7.4/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4978 2024-03-18 10:37:34.000000 ANBUtils-1.7.4/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-16 09:45:08.464278 ANBUtils-1.7.4/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-04-16 09:45:08.000000 ANBUtils-1.7.4/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      357 2024-04-16 09:45:08.000000 ANBUtils-1.7.4/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2024-04-16 09:45:08.000000 ANBUtils-1.7.4/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)      108 2024-04-16 09:45:08.000000 ANBUtils-1.7.4/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2024-04-16 09:45:08.000000 ANBUtils-1.7.4/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-04-16 09:45:08.464664 ANBUtils-1.7.4/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4893 2024-03-28 07:19:01.000000 ANBUtils-1.7.4/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2024-04-16 09:45:08.465083 ANBUtils-1.7.4/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      886 2024-04-16 09:36:19.000000 ANBUtils-1.7.4/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-18 06:28:34.025874 ANBUtils-1.7.5/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-18 06:28:34.023983 ANBUtils-1.7.5/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)    13984 2024-04-18 06:27:18.000000 ANBUtils-1.7.5/ANBUtils/DBWorker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      865 2024-03-28 10:31:28.000000 ANBUtils-1.7.5/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-07-11 07:09:11.000000 ANBUtils-1.7.5/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3186 2024-03-28 10:27:52.000000 ANBUtils-1.7.5/ANBUtils/db_tools.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.7.5/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1092 2023-07-03 10:30:53.000000 ANBUtils-1.7.5/ANBUtils/environ.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.7.5/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2427 2024-03-28 04:40:26.000000 ANBUtils-1.7.5/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4978 2024-03-18 10:37:34.000000 ANBUtils-1.7.5/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-04-18 06:28:34.025110 ANBUtils-1.7.5/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-04-18 06:28:33.000000 ANBUtils-1.7.5/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      357 2024-04-18 06:28:33.000000 ANBUtils-1.7.5/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2024-04-18 06:28:33.000000 ANBUtils-1.7.5/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      108 2024-04-18 06:28:33.000000 ANBUtils-1.7.5/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2024-04-18 06:28:33.000000 ANBUtils-1.7.5/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-04-18 06:28:34.025548 ANBUtils-1.7.5/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4893 2024-03-28 07:19:01.000000 ANBUtils-1.7.5/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2024-04-18 06:28:34.025952 ANBUtils-1.7.5/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      886 2024-04-18 06:28:25.000000 ANBUtils-1.7.5/setup.py
```

### Comparing `ANBUtils-1.7.4/ANBUtils/DBWorker.py` & `ANBUtils-1.7.5/ANBUtils/DBWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,13 +387,10 @@
             data (dict): The log data to be inserted.
         """
         data['_type_'] = _type
         self.link('__log__').insert_one(data)
 
     def read_logging(self, _type: str) -> pd.DataFrame:
         return self.link('__log__').find_all({"_type_": _type})
-
-    def __del__(self):
-        self.client.close()
-
+    
     def __repr__(self):
         return f"DBWorker({self.db_code})"
```

### Comparing `ANBUtils-1.7.4/ANBUtils/__init__.py` & `ANBUtils-1.7.5/ANBUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/a.py` & `ANBUtils-1.7.5/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/db_tools.py` & `ANBUtils-1.7.5/ANBUtils/db_tools.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/easy_pickle.py` & `ANBUtils-1.7.5/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/environ.py` & `ANBUtils-1.7.5/ANBUtils/environ.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/id_work.py` & `ANBUtils-1.7.5/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/messenger.py` & `ANBUtils-1.7.5/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils/tbox.py` & `ANBUtils-1.7.5/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.7.5/ANBUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.7.4
+Version: 1.7.5
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.0.0
```

### Comparing `ANBUtils-1.7.4/PKG-INFO` & `ANBUtils-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.7.4
+Version: 1.7.5
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.0.0
```

### Comparing `ANBUtils-1.7.4/README.md` & `ANBUtils-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.7.4/setup.py` & `ANBUtils-1.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
     name = "ANBUtils",
-    version = '1.7.4',
+    version = '1.7.5',
     packages = find_packages(),
     author = 'Yafei Hou',
     author_email = 'redbson@gmail.com',
     url = 'https://github.com/redbson/ANBUtils',
     description = 'ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and '
                   'tools for data analysis, database operations, and messaging integration.',
     long_description = long_description,
```

