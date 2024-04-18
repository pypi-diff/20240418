# Comparing `tmp/gw_chirpy-0.0.2.tar.gz` & `tmp/gw_chirpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw_chirpy-0.0.2.tar", last modified: Mon Apr 15 20:09:30 2024, max compression
+gzip compressed data, was "gw_chirpy-0.0.4.tar", last modified: Thu Apr 18 07:17:22 2024, max compression
```

## Comparing `gw_chirpy-0.0.2.tar` & `gw_chirpy-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.123426 gw_chirpy-0.0.2/
--rw-r--r--   0 sebastian.khan   (501) staff       (20)    35073 2024-04-15 07:03:02.000000 gw_chirpy-0.0.2/LICENSE
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      505 2024-04-15 20:09:30.123254 gw_chirpy-0.0.2/PKG-INFO
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      349 2024-04-15 19:58:31.000000 gw_chirpy-0.0.2/README.md
-drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.121762 gw_chirpy-0.0.2/chirpy/
--rw-r--r--   0 sebastian.khan   (501) staff       (20)       16 2024-04-15 07:03:02.000000 gw_chirpy-0.0.2/chirpy/__init__.py
-drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.122344 gw_chirpy-0.0.2/chirpy/prob_phenom_model/
--rw-r--r--   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 07:21:19.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/__init__.py
--rw-r--r--   0 sebastian.khan   (501) staff       (20)     7416 2024-04-15 07:04:59.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/collocation.py
--rw-r--r--   0 sebastian.khan   (501) staff       (20)     4992 2024-04-15 07:04:59.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/pn.py
--rw-r--r--   0 sebastian.khan   (501) staff       (20)    28364 2024-04-15 07:50:02.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/ppm_utils.py
--rw-r--r--   0 sebastian.khan   (501) staff       (20)    10742 2024-04-15 07:24:15.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/workflow_utils.py
-drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.123068 gw_chirpy-0.0.2/gw_chirpy.egg-info/
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      505 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/PKG-INFO
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      398 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian.khan   (501) staff       (20)        1 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      104 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/requires.txt
--rw-r--r--   0 sebastian.khan   (501) staff       (20)        7 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/top_level.txt
--rw-r--r--   0 sebastian.khan   (501) staff       (20)       38 2024-04-15 20:09:30.123461 gw_chirpy-0.0.2/setup.cfg
--rw-r--r--   0 sebastian.khan   (501) staff       (20)      818 2024-04-15 20:09:27.000000 gw_chirpy-0.0.2/setup.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-18 07:17:22.835250 gw_chirpy-0.0.4/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    35073 2024-04-15 07:03:02.000000 gw_chirpy-0.0.4/LICENSE
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      478 2024-04-18 07:17:22.835080 gw_chirpy-0.0.4/PKG-INFO
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      138 2024-04-18 07:07:32.000000 gw_chirpy-0.0.4/README.md
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-18 07:17:22.833372 gw_chirpy-0.0.4/chirpy/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)       16 2024-04-15 07:03:02.000000 gw_chirpy-0.0.4/chirpy/__init__.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-18 07:17:22.834102 gw_chirpy-0.0.4/chirpy/prob_phenom_model/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 07:21:19.000000 gw_chirpy-0.0.4/chirpy/prob_phenom_model/__init__.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)     7416 2024-04-15 07:04:59.000000 gw_chirpy-0.0.4/chirpy/prob_phenom_model/collocation.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)     4992 2024-04-15 07:04:59.000000 gw_chirpy-0.0.4/chirpy/prob_phenom_model/pn.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    28364 2024-04-15 07:50:02.000000 gw_chirpy-0.0.4/chirpy/prob_phenom_model/ppm_utils.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    10742 2024-04-15 07:24:15.000000 gw_chirpy-0.0.4/chirpy/prob_phenom_model/workflow_utils.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-18 07:17:22.834882 gw_chirpy-0.0.4/gw_chirpy.egg-info/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      478 2024-04-18 07:17:22.000000 gw_chirpy-0.0.4/gw_chirpy.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      413 2024-04-18 07:17:22.000000 gw_chirpy-0.0.4/gw_chirpy.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        1 2024-04-18 07:17:22.000000 gw_chirpy-0.0.4/gw_chirpy.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      104 2024-04-18 07:17:22.000000 gw_chirpy-0.0.4/gw_chirpy.egg-info/requires.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        7 2024-04-18 07:17:22.000000 gw_chirpy-0.0.4/gw_chirpy.egg-info/top_level.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      454 2024-04-18 07:17:20.000000 gw_chirpy-0.0.4/pyproject.toml
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)       38 2024-04-18 07:17:22.835295 gw_chirpy-0.0.4/setup.cfg
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      348 2024-04-18 07:14:43.000000 gw_chirpy-0.0.4/setup.py
```

### Comparing `gw_chirpy-0.0.2/LICENSE` & `gw_chirpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gw_chirpy-0.0.2/chirpy/prob_phenom_model/collocation.py` & `gw_chirpy-0.0.4/chirpy/prob_phenom_model/collocation.py`

 * *Files identical despite different names*

### Comparing `gw_chirpy-0.0.2/chirpy/prob_phenom_model/pn.py` & `gw_chirpy-0.0.4/chirpy/prob_phenom_model/pn.py`

 * *Files identical despite different names*

### Comparing `gw_chirpy-0.0.2/chirpy/prob_phenom_model/ppm_utils.py` & `gw_chirpy-0.0.4/chirpy/prob_phenom_model/ppm_utils.py`

 * *Files identical despite different names*

### Comparing `gw_chirpy-0.0.2/chirpy/prob_phenom_model/workflow_utils.py` & `gw_chirpy-0.0.4/chirpy/prob_phenom_model/workflow_utils.py`

 * *Files identical despite different names*

