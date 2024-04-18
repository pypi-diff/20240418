# Comparing `tmp/transformermath-0.1.1.tar.gz` & `tmp/transformermath-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformermath-0.1.1.tar", last modified: Thu Apr 18 12:00:34 2024, max compression
+gzip compressed data, was "transformermath-0.1.2.tar", last modified: Thu Apr 18 12:05:44 2024, max compression
```

## Comparing `transformermath-0.1.1.tar` & `transformermath-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:00:34.766623 transformermath-0.1.1/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:00:34.766359 transformermath-0.1.1/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.1/README.md
--rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:00:34.766744 transformermath-0.1.1/setup.cfg
--rw-r--r--   0 aaronkher   (501) staff       (20)      407 2024-04-18 12:00:25.000000 transformermath-0.1.1/setup.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:00:34.764475 transformermath-0.1.1/transformermath/
--rw-r--r--   0 aaronkher   (501) staff       (20)     1034 2024-04-18 11:33:41.000000 transformermath-0.1.1/transformermath/__init__.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.1/transformermath/attention_analyzer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)    11771 2024-04-18 05:00:26.000000 transformermath-0.1.1/transformermath/data_creator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.1/transformermath/encoded_representations.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.1/transformermath/evaluator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.1/transformermath/general_helper.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     6874 2024-04-18 11:29:41.000000 transformermath-0.1.1/transformermath/main.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.1/transformermath/prober.py
--rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.1/transformermath/run_config.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.1/transformermath/run_device.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.1/transformermath/tokenizer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.1/transformermath/trainer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.1/transformermath/visualiser.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:00:34.765966 transformermath-0.1.1/transformermath.egg-info/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:00:34.000000 transformermath-0.1.1/transformermath.egg-info/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:00:34.000000 transformermath-0.1.1/transformermath.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:00:34.000000 transformermath-0.1.1/transformermath.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)      142 2024-04-18 12:00:34.000000 transformermath-0.1.1/transformermath.egg-info/requires.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:00:34.000000 transformermath-0.1.1/transformermath.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.577506 transformermath-0.1.2/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:05:44.577275 transformermath-0.1.2/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.2/README.md
+-rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:05:44.577607 transformermath-0.1.2/setup.cfg
+-rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:05:18.000000 transformermath-0.1.2/setup.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.575345 transformermath-0.1.2/transformermath/
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1034 2024-04-18 11:33:41.000000 transformermath-0.1.2/transformermath/__init__.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.2/transformermath/attention_analyzer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)    11771 2024-04-18 05:00:26.000000 transformermath-0.1.2/transformermath/data_creator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.2/transformermath/encoded_representations.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.2/transformermath/evaluator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.2/transformermath/general_helper.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     6874 2024-04-18 11:29:41.000000 transformermath-0.1.2/transformermath/main.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.2/transformermath/prober.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.2/transformermath/run_config.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.2/transformermath/run_device.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.2/transformermath/tokenizer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.2/transformermath/trainer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.2/transformermath/visualiser.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.576891 transformermath-0.1.2/transformermath.egg-info/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/requires.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/top_level.txt
```

### Comparing `transformermath-0.1.1/transformermath/__init__.py` & `transformermath-0.1.2/transformermath/__init__.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/attention_analyzer.py` & `transformermath-0.1.2/transformermath/attention_analyzer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/data_creator.py` & `transformermath-0.1.2/transformermath/data_creator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/encoded_representations.py` & `transformermath-0.1.2/transformermath/encoded_representations.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/evaluator.py` & `transformermath-0.1.2/transformermath/evaluator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/general_helper.py` & `transformermath-0.1.2/transformermath/general_helper.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/main.py` & `transformermath-0.1.2/transformermath/main.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/prober.py` & `transformermath-0.1.2/transformermath/prober.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/run_config.py` & `transformermath-0.1.2/transformermath/run_config.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/run_device.py` & `transformermath-0.1.2/transformermath/run_device.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/tokenizer.py` & `transformermath-0.1.2/transformermath/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/trainer.py` & `transformermath-0.1.2/transformermath/trainer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath/visualiser.py` & `transformermath-0.1.2/transformermath/visualiser.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.1/transformermath.egg-info/SOURCES.txt` & `transformermath-0.1.2/transformermath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

