# Comparing `tmp/noisebase-1.1.tar.gz` & `tmp/noisebase-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisebase-1.1.tar", last modified: Fri Apr 12 10:02:29 2024, max compression
+gzip compressed data, was "noisebase-1.1.1.tar", last modified: Thu Apr 18 10:47:02 2024, max compression
```

## Comparing `noisebase-1.1.tar` & `noisebase-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.174639 noisebase-1.1/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)    11344 2024-04-09 15:43:21.000000 noisebase-1.1/LICENSE
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       39 2024-04-02 13:47:26.000000 noisebase-1.1/MANIFEST.in
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5792 2024-04-12 10:02:29.000000 noisebase-1.1/PKG-INFO
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     4993 2024-04-12 09:55:08.000000 noisebase-1.1/README.md
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.810640 noisebase-1.1/noisebase/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2413 2024-04-12 10:02:10.000000 noisebase-1.1/noisebase/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2239 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/compression.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.690640 noisebase-1.1/noisebase/conf/
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.934640 noisebase-1.1/noisebase/conf/noisebase/
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.962640 noisebase-1.1/noisebase/conf/noisebase/format/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      427 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/conf/noisebase/format/test_sample_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      634 2024-04-04 01:01:46.000000 noisebase-1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      800 2024-04-02 16:37:47.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      879 2024-04-02 15:53:00.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      385 2024-04-02 16:37:54.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     3028 2024-04-03 14:40:25.000000 noisebase-1.1/noisebase/data.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.986640 noisebase-1.1/noisebase/lightning/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       45 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/lightning/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1805 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/lightning/midepoch_ckpt.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.994639 noisebase-1.1/noisebase/loaders/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:20.000000 noisebase-1.1/noisebase/loaders/__init__.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.018639 noisebase-1.1/noisebase/loaders/lightning/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       55 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/loaders/lightning/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      776 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/loaders/lightning/training_sample_v1.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.046639 noisebase-1.1/noisebase/loaders/torch/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      103 2024-04-01 20:01:43.000000 noisebase-1.1/noisebase/loaders/torch/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     9728 2024-04-02 16:02:24.000000 noisebase-1.1/noisebase/loaders/torch/test_sample_v1.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     9202 2024-04-04 01:02:35.000000 noisebase-1.1/noisebase/loaders/torch/training_sample_v1.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.074639 noisebase-1.1/noisebase/metrics/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:31.000000 noisebase-1.1/noisebase/metrics/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)    29927 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/metrics/flip.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     4815 2024-04-04 20:16:47.000000 noisebase-1.1/noisebase/metrics/fvvdp.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     8026 2024-04-01 20:01:41.000000 noisebase-1.1/noisebase/projective.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.118639 noisebase-1.1/noisebase/scripts/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      213 2024-04-02 15:32:45.000000 noisebase-1.1/noisebase/scripts/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5116 2024-04-02 17:19:45.000000 noisebase-1.1/noisebase/scripts/nb_compute_metrics.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      763 2024-04-02 14:22:09.000000 noisebase-1.1/noisebase/scripts/nb_download.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2012 2024-04-05 00:45:54.000000 noisebase-1.1/noisebase/scripts/nb_result_table.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      486 2024-04-02 17:20:49.000000 noisebase-1.1/noisebase/scripts/nb_save_reference.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.158639 noisebase-1.1/noisebase/torch/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       85 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1059 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/misc.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1631 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/projective.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5641 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/video_sampler.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.874640 noisebase-1.1/noisebase.egg-info/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5792 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/PKG-INFO
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1283 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/SOURCES.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        1 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/dependency_links.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      228 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/entry_points.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/requires.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       10 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/top_level.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1061 2024-04-12 09:30:32.000000 noisebase-1.1/pyproject.toml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      133 2024-04-12 10:02:29.000000 noisebase-1.1/setup.cfg
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.901876 noisebase-1.1.1/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    11344 2024-04-15 22:54:27.000000 noisebase-1.1.1/LICENSE
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       39 2024-04-15 22:54:27.000000 noisebase-1.1.1/MANIFEST.in
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5794 2024-04-18 10:47:02.000000 noisebase-1.1.1/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4993 2024-04-15 22:54:38.000000 noisebase-1.1.1/README.md
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.597874 noisebase-1.1.1/noisebase/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2415 2024-04-18 10:45:19.000000 noisebase-1.1.1/noisebase/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2239 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/compression.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.485874 noisebase-1.1.1/noisebase/conf/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.689875 noisebase-1.1.1/noisebase/conf/noisebase/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.713875 noisebase-1.1.1/noisebase/conf/noisebase/format/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      427 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/conf/noisebase/format/test_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      634 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      800 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      879 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      385 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/conf/noisebase/sampleset_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     3397 2024-04-18 10:43:34.000000 noisebase-1.1.1/noisebase/data.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.733875 noisebase-1.1.1/noisebase/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       45 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1805 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/lightning/midepoch_ckpt.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.741875 noisebase-1.1.1/noisebase/loaders/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/loaders/__init__.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.753875 noisebase-1.1.1/noisebase/loaders/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       55 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/loaders/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      776 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/loaders/lightning/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.777876 noisebase-1.1.1/noisebase/loaders/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      103 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/loaders/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9730 2024-04-18 10:36:26.000000 noisebase-1.1.1/noisebase/loaders/torch/test_sample_v1.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9204 2024-04-18 10:36:43.000000 noisebase-1.1.1/noisebase/loaders/torch/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.797876 noisebase-1.1.1/noisebase/metrics/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/metrics/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    29927 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/metrics/flip.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4815 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/metrics/fvvdp.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     8026 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/projective.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.845876 noisebase-1.1.1/noisebase/scripts/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      213 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/scripts/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5116 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/scripts/nb_compute_metrics.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      763 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/scripts/nb_download.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2012 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/scripts/nb_result_table.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      486 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/scripts/nb_save_reference.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.885876 noisebase-1.1.1/noisebase/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       85 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1059 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/torch/misc.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1631 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/torch/projective.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5641 2024-04-15 22:54:27.000000 noisebase-1.1.1/noisebase/torch/video_sampler.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-18 10:47:02.657875 noisebase-1.1.1/noisebase.egg-info/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5794 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1283 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        1 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      228 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/entry_points.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/requires.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       10 2024-04-18 10:47:02.000000 noisebase-1.1.1/noisebase.egg-info/top_level.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1061 2024-04-15 22:54:27.000000 noisebase-1.1.1/pyproject.toml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      133 2024-04-18 10:47:02.000000 noisebase-1.1.1/setup.cfg
```

### Comparing `noisebase-1.1/LICENSE` & `noisebase-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/PKG-INFO` & `noisebase-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisebase
-Version: 1.1
+Version: 1.1.1
 Summary: Datasets and benchmarks for neural Monte Carlo denoising
 Author-email: Martin Bálint <martin@balint.io>
 Project-URL: Documentation, https://balint.io/noisebase
 Project-URL: Repository, https://github.com/balintio/noisebase.git
 Keywords: denoising,Monte Carlo,MC,neural
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noisebase Version: 1.1 Summary: Datasets and
+Metadata-Version: 2.1 Name: noisebase Version: 1.1.1 Summary: Datasets and
 benchmarks for neural Monte Carlo denoising Author-email: Martin BÃ¡lint
 balint.io> Project-URL: Documentation, https://balint.io/noisebase Project-URL:
 Repository, https://github.com/balintio/noisebase.git Keywords: denoising,Monte
 Carlo,MC,neural Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Environment :: GPU
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `noisebase-1.1/README.md` & `noisebase-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/__init__.py` & `noisebase-1.1.1/noisebase/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Datasets and benchmarks for neural Monte Carlo denoising.
 
 This file serves as the main entry point for Noisebase. It registers all 
 Noisebase config files in your Hydra path and, in addition, provides a 
 `Noisebase` function should you wish to keep your use of Hydra to a minimum.
 """
 
-__version__ = '1.1'
+__version__ = '1.1.1'
 
 import os
 
 from hydra.plugins.search_path_plugin import SearchPathPlugin
 from hydra.core.plugins import Plugins
 
 class NoisebaseSearchPathPlugin(SearchPathPlugin):
```

### Comparing `noisebase-1.1/noisebase/compression.py` & `noisebase-1.1.1/noisebase/compression.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml` & `noisebase-1.1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml` & `noisebase-1.1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml` & `noisebase-1.1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/data.py` & `noisebase-1.1.1/noisebase/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,31 @@
 from urllib.parse import unquote_plus, urlparse
 import numpy as np
 import os
 import requests
 from tqdm import tqdm
 
 def resolve_data_path(data_path):
-    if data_path != None:
+    if data_path != None: # Using custom data folder
         return data_path
+    # Otherwise find the default folder
 
-    dist_info = json.loads(metadata.distribution('noisebase').read_text('direct_url.json'))
-    editable = dist_info.get('dir_info', {}).get('editable', False)
+    # Fetch metadata saved by Pip
+    url_file = metadata.distribution('noisebase').read_text('direct_url.json')
 
-    if editable:
+    if url_file == None: # Noisebase installed through PyPI
+        editable = False
+    else: # Noisebase installed from elsewhere (potentially editable)
+        dist_info = json.loads(url_file)
+        editable = dist_info.get('dir_info', {}).get('editable', False)
+
+    if editable: # Default folder is cloned_repo/data
         nb_folder = unquote_plus(urlparse(dist_info['url']).path)
         return os.path.join(nb_folder, 'data')
-    else:
+    else: # Default folder is working_directory/data
         return os.path.join(os.getcwd(), 'data')
 
 def consumer_generator(queue, producer_process):
     try:
         while True:
             if producer_process.exitcode is not None and queue.empty():
                 # Handle producer crash
```

### Comparing `noisebase-1.1/noisebase/lightning/midepoch_ckpt.py` & `noisebase-1.1.1/noisebase/lightning/midepoch_ckpt.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/loaders/lightning/training_sample_v1.py` & `noisebase-1.1.1/noisebase/loaders/lightning/training_sample_v1.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/loaders/torch/test_sample_v1.py` & `noisebase-1.1.1/noisebase/loaders/torch/test_sample_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         return metadata
 
     def download(self):
         data_path = resolve_data_path(self.kwargs['data_path'])
         remote_path = self.kwargs['data_remote']
 
         if remote_path == None:
-            print(f'Download aborted: the remote path for "{self.kwargs['name']}" was not provided.')
+            print(f'Download aborted: the remote path for \"{self.kwargs["name"]}\" was not provided.')
             print('Consult the dataset\'s documentation for instructions on acquiring it.')
             return
 
         files = [
             self.src['files'].format(index=i, sequence_name=sequence['name'])
             for sequence in self.src.sequences
             for i in range(sequence['frames'])
```

### Comparing `noisebase-1.1/noisebase/loaders/torch/training_sample_v1.py` & `noisebase-1.1.1/noisebase/loaders/torch/training_sample_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             self.batch_sampler.start_sequence_idx = state_dict['start_sequence_idx']
     
     def download(self):
         data_path = resolve_data_path(self.__kwargs['data_path'])
         remote_path = self.__kwargs['data_remote']
 
         if remote_path == None:
-            print(f'Download aborted: the remote path for "{self.__kwargs['name']}" was not provided.')
+            print(f'Download aborted: the remote path for \"{self.__kwargs["name"]}\" was not provided.')
             print('Consult the dataset\'s documentation for instructions on acquiring it.')
             return
 
         files = [
             self.__src['files'].format(index=i)
             for i in range(self.__src['sequences'])
         ]
```

### Comparing `noisebase-1.1/noisebase/metrics/flip.py` & `noisebase-1.1.1/noisebase/metrics/flip.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/metrics/fvvdp.py` & `noisebase-1.1.1/noisebase/metrics/fvvdp.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/projective.py` & `noisebase-1.1.1/noisebase/projective.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/scripts/nb_compute_metrics.py` & `noisebase-1.1.1/noisebase/scripts/nb_compute_metrics.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/scripts/nb_download.py` & `noisebase-1.1.1/noisebase/scripts/nb_download.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/scripts/nb_result_table.py` & `noisebase-1.1.1/noisebase/scripts/nb_result_table.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/torch/misc.py` & `noisebase-1.1.1/noisebase/torch/misc.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/torch/projective.py` & `noisebase-1.1.1/noisebase/torch/projective.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase/torch/video_sampler.py` & `noisebase-1.1.1/noisebase/torch/video_sampler.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/noisebase.egg-info/PKG-INFO` & `noisebase-1.1.1/noisebase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisebase
-Version: 1.1
+Version: 1.1.1
 Summary: Datasets and benchmarks for neural Monte Carlo denoising
 Author-email: Martin Bálint <martin@balint.io>
 Project-URL: Documentation, https://balint.io/noisebase
 Project-URL: Repository, https://github.com/balintio/noisebase.git
 Keywords: denoising,Monte Carlo,MC,neural
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noisebase Version: 1.1 Summary: Datasets and
+Metadata-Version: 2.1 Name: noisebase Version: 1.1.1 Summary: Datasets and
 benchmarks for neural Monte Carlo denoising Author-email: Martin BÃ¡lint
 balint.io> Project-URL: Documentation, https://balint.io/noisebase Project-URL:
 Repository, https://github.com/balintio/noisebase.git Keywords: denoising,Monte
 Carlo,MC,neural Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Environment :: GPU
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `noisebase-1.1/noisebase.egg-info/SOURCES.txt` & `noisebase-1.1.1/noisebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noisebase-1.1/pyproject.toml` & `noisebase-1.1.1/pyproject.toml`

 * *Files identical despite different names*

