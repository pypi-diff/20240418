# Comparing `tmp/wkregister-0.0.3.tar.gz` & `tmp/wkregister-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkregister-0.0.3.tar", last modified: Thu Apr 18 17:46:35 2024, max compression
+gzip compressed data, was "wkregister-0.0.4.tar", last modified: Thu Apr 18 18:29:33 2024, max compression
```

## Comparing `wkregister-0.0.3.tar` & `wkregister-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.449318 wkregister-0.0.3/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.3/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:46:35.449054 wkregister-0.0.3/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.3/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 17:46:25.000000 wkregister-0.0.3/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 17:46:35.449372 wkregister-0.0.3/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.446571 wkregister-0.0.3/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.446812 wkregister-0.0.3/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.3/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.3/src/test/test_logs.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.3/src/test.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.447713 wkregister-0.0.3/src/wkregister/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.3/src/wkregister/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1849 2024-04-18 17:43:59.000000 wkregister-0.0.3/src/wkregister/decorator.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.3/src/wkregister/models.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.3/src/wkregister/producer.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.3/src/wkregister/util.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.448795 wkregister-0.0.3/src/wkregister.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/requires.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.308839 wkregister-0.0.4/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.4/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:29:33.308557 wkregister-0.0.4/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.4/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 18:29:22.000000 wkregister-0.0.4/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 18:29:33.308893 wkregister-0.0.4/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.306551 wkregister-0.0.4/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.306788 wkregister-0.0.4/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.4/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.4/src/test/test_logs.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.4/src/test.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.307467 wkregister-0.0.4/src/wkregister/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.4/src/wkregister/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1783 2024-04-18 18:29:13.000000 wkregister-0.0.4/src/wkregister/decorator.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.4/src/wkregister/models.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.4/src/wkregister/producer.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.4/src/wkregister/util.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:29:33.308320 wkregister-0.0.4/src/wkregister.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/requires.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:29:33.000000 wkregister-0.0.4/src/wkregister.egg-info/top_level.txt
```

### Comparing `wkregister-0.0.3/LICENSE` & `wkregister-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/PKG-INFO` & `wkregister-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkregister-0.0.3/README.md` & `wkregister-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/pyproject.toml` & `wkregister-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wkregister"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Gustavo", email="gustavo.gordillo.giron@gmail.com" },
 ]
 description = "A wk register library for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wkregister-0.0.3/src/test/test_logs.py` & `wkregister-0.0.4/src/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/src/wkregister/decorator.py` & `wkregister-0.0.4/src/wkregister/decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
             if inspect.iscoroutine(input):
                 result = await input
             else:
                 result = input
 
             org, key, log = kafkaParams(result)
-            print(f"log={log.dict()}")
 
             start_time = time.time()  # Capture the start time
 
             # Log after function execution, you can adjust what you log as needed
             asyncio.create_task(record2Kafka(org, key, log.dict()))
 
             end_time = time.time()  # Capture the end time
@@ -50,14 +49,12 @@
             output = {}
             for key, value in result.items():
                 if not key == "record" or not key == "log":
                     output[key] = value
                 if key == "record" or key == "log":
                     output[key] = log.dict()
 
-            print(output)
-
             return output
 
         return wrapper
 
     return decorator_log
```

### Comparing `wkregister-0.0.3/src/wkregister/models.py` & `wkregister-0.0.4/src/wkregister/models.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/src/wkregister/producer.py` & `wkregister-0.0.4/src/wkregister/producer.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/src/wkregister/util.py` & `wkregister-0.0.4/src/wkregister/util.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.3/src/wkregister.egg-info/PKG-INFO` & `wkregister-0.0.4/src/wkregister.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

