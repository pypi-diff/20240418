# Comparing `tmp/wkregister-0.0.4.tar.gz` & `tmp/wkregister-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkregister-0.0.4.tar", last modified: Thu Apr 18 18:29:33 2024, max compression
+gzip compressed data, was "wkregister-0.0.5.tar", last modified: Thu Apr 18 18:34:57 2024, max compression
```

## Comparing `wkregister-0.0.4.tar` & `wkregister-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.308839 wkregister-0.0.4/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.4/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:29:33.308557 wkregister-0.0.4/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.4/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 18:29:22.000000 wkregister-0.0.4/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 18:29:33.308893 wkregister-0.0.4/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.306551 wkregister-0.0.4/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.306788 wkregister-0.0.4/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.4/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.4/src/test/test_logs.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.4/src/test.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.307467 wkregister-0.0.4/src/wkregister/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.4/src/wkregister/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1783 2024-04-18 18:29:13.000000 wkregister-0.0.4/src/wkregister/decorator.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.4/src/wkregister/models.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.4/src/wkregister/producer.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.4/src/wkregister/util.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.308320 wkregister-0.0.4/src/wkregister.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/requires.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:34:57.636356 wkregister-0.0.5/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.5/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:34:57.636075 wkregister-0.0.5/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.5/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 18:34:49.000000 wkregister-0.0.5/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 18:34:57.636409 wkregister-0.0.5/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:34:57.633686 wkregister-0.0.5/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:34:57.634056 wkregister-0.0.5/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.5/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.5/src/test/test_logs.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.5/src/test.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:34:57.634770 wkregister-0.0.5/src/wkregister/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.5/src/wkregister/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1686 2024-04-18 18:34:31.000000 wkregister-0.0.5/src/wkregister/decorator.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.5/src/wkregister/models.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.5/src/wkregister/producer.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.5/src/wkregister/util.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:34:57.635776 wkregister-0.0.5/src/wkregister.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:34:57.000000 wkregister-0.0.5/src/wkregister.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 18:34:57.000000 wkregister-0.0.5/src/wkregister.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 18:34:57.000000 wkregister-0.0.5/src/wkregister.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:34:57.000000 wkregister-0.0.5/src/wkregister.egg-info/requires.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:34:57.000000 wkregister-0.0.5/src/wkregister.egg-info/top_level.txt
```

### Comparing `wkregister-0.0.4/LICENSE` & `wkregister-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/PKG-INFO` & `wkregister-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkregister-0.0.4/README.md` & `wkregister-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/pyproject.toml` & `wkregister-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wkregister"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Gustavo", email="gustavo.gordillo.giron@gmail.com" },
 ]
 description = "A wk register library for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wkregister-0.0.4/src/test/test_logs.py` & `wkregister-0.0.5/src/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/src/wkregister/decorator.py` & `wkregister-0.0.5/src/wkregister/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,13 @@
             elapsed_time = end_time - start_time  # Calculate elapsed time
             # print(f"The function took {elapsed_time} seconds to complete.")
 
             output = {}
             for key, value in result.items():
                 if not key == "record" or not key == "log":
                     output[key] = value
-                if key == "record" or key == "log":
-                    output[key] = log.dict()
 
             return output
 
         return wrapper
 
     return decorator_log
```

### Comparing `wkregister-0.0.4/src/wkregister/models.py` & `wkregister-0.0.5/src/wkregister/models.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/src/wkregister/producer.py` & `wkregister-0.0.5/src/wkregister/producer.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/src/wkregister/util.py` & `wkregister-0.0.5/src/wkregister/util.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.4/src/wkregister.egg-info/PKG-INFO` & `wkregister-0.0.5/src/wkregister.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

