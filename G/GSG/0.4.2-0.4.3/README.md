# Comparing `tmp/GSG-0.4.2.tar.gz` & `tmp/GSG-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.4.2.tar", last modified: Thu Apr 18 04:47:45 2024, max compression
+gzip compressed data, was "dist/GSG-0.4.3.tar", last modified: Thu Apr 18 05:15:13 2024, max compression
```

## Comparing `GSG-0.4.2.tar` & `GSG-0.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      165 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    40574 2024-04-18 04:41:51.000000 GSG-0.4.2/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 04:47:45.000000 GSG-0.4.2/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2854 2023-06-08 05:59:08.000000 GSG-0.4.2/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.4.2/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.4.2/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.4.2/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.4.2/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.4.2/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.4.2/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-18 04:47:45.000000 GSG-0.4.2/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      489 2024-04-18 04:47:41.000000 GSG-0.4.2/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.4.2/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.4.2/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.4.2/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.4.2/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.4.2/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.4.2/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 05:15:13.000000 GSG-0.4.3/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      179 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-18 05:15:13.000000 GSG-0.4.3/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40590 2024-04-18 05:14:31.000000 GSG-0.4.3/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 05:15:13.000000 GSG-0.4.3/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2854 2023-06-08 05:59:08.000000 GSG-0.4.3/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 05:15:13.000000 GSG-0.4.3/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.4.3/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.4.3/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 05:15:13.000000 GSG-0.4.3/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.4.3/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.4.3/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.4.3/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.4.3/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.4.3/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.4.3/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.4.3/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-18 05:15:13.000000 GSG-0.4.3/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-18 05:15:11.000000 GSG-0.4.3/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 05:15:13.000000 GSG-0.4.3/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.4.3/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.4.3/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.4.3/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.4.3/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.4.3/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.4.3/tools/utils.py
```

### Comparing `GSG-0.4.2/GSG.py` & `GSG-0.4.3/GSG.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     KMeans_use,
     drawPicture,
     mkdir,
 )
 warnings.filterwarnings("ignore")
 from scipy.spatial.distance import pdist, squareform
 from scipy import sparse
+import argparse
 
 def build_args():
     parser = argparse.ArgumentParser(description="GAT")
     parser.add_argument("--seeds", type=int, nargs="+", default=[0])
     parser.add_argument("--device", type=int, default=-1)
     parser.add_argument("--warmup_steps", type=int, default=-1)
     parser.add_argument("--num_heads", type=int, default=4,
```

### Comparing `GSG-0.4.2/README.md` & `GSG-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/datasets/data_util.py` & `GSG-0.4.3/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/__init__.py` & `GSG-0.4.3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/dot_gat.py` & `GSG-0.4.3/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/edcoder.py` & `GSG-0.4.3/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/gat.py` & `GSG-0.4.3/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/gcn.py` & `GSG-0.4.3/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/gin.py` & `GSG-0.4.3/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/models/loss_func.py` & `GSG-0.4.3/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/tools/batch_remove.py` & `GSG-0.4.3/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/tools/evaluation.py` & `GSG-0.4.3/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/tools/parameters_dict.py` & `GSG-0.4.3/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/tools/test.py` & `GSG-0.4.3/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.4.2/tools/utils.py` & `GSG-0.4.3/tools/utils.py`

 * *Files identical despite different names*

