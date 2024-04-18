# Comparing `tmp/brainrender-2.1.6.tar.gz` & `tmp/brainrender-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainrender-2.1.6.tar", last modified: Tue Feb 27 11:33:01 2024, max compression
+gzip compressed data, was "brainrender-2.1.7.tar", last modified: Thu Apr 18 11:17:28 2024, max compression
```

## Comparing `brainrender-2.1.6.tar` & `brainrender-2.1.7.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.217123 brainrender-2.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.201124 brainrender-2.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.201124 brainrender-2.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-27 11:32:53.000000 brainrender-2.1.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-27 11:32:53.000000 brainrender-2.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-27 11:32:53.000000 brainrender-2.1.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-27 11:32:53.000000 brainrender-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-27 11:32:53.000000 brainrender-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-02-27 11:33:01.217123 brainrender-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-02-27 11:32:53.000000 brainrender-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.205124 brainrender-2.1.6/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.205124 brainrender-2.1.6/brainrender/actors/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/neurons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/ruler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/actors/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.205124 brainrender-2.1.6/brainrender/atlas_specific/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas_specific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.205124 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.205124 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.217123 brainrender-2.1.6/brainrender/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/CC_134_1_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/CC_134_2_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/neuron1.swc
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/probe_1_striatum.npy
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/probe_2_RSP.npy
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/random_cells.h5
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/random_cells.npy
--rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/resources/volume.npy
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-02-27 11:32:53.000000 brainrender-2.1.6/brainrender/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:33:01.217123 brainrender-2.1.6/brainrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-02-27 11:33:01.000000 brainrender-2.1.6/brainrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-27 11:33:01.000000 brainrender-2.1.6/brainrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 11:33:01.000000 brainrender-2.1.6/brainrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-27 11:33:01.000000 brainrender-2.1.6/brainrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-27 11:33:01.000000 brainrender-2.1.6/brainrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-02-27 11:32:53.000000 brainrender-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 11:33:01.217123 brainrender-2.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.380255 brainrender-2.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.380255 brainrender-2.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 11:17:22.000000 brainrender-2.1.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-18 11:17:22.000000 brainrender-2.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 11:17:22.000000 brainrender-2.1.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-18 11:17:22.000000 brainrender-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 11:17:22.000000 brainrender-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-18 11:17:28.396255 brainrender-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-18 11:17:22.000000 brainrender-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/ruler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/atlas_specific/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.388255 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/brainrender/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/CC_134_1_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/CC_134_2_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/neuron1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/probe_1_striatum.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/probe_2_RSP.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/random_cells.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/random_cells.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/volume.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/brainrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-18 11:17:22.000000 brainrender-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:17:28.396255 brainrender-2.1.7/setup.cfg
```

### Comparing `brainrender-2.1.6/.github/workflows/test_and_deploy.yml` & `brainrender-2.1.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/.gitignore` & `brainrender-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/CITATION.cff` & `brainrender-2.1.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/LICENSE` & `brainrender-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/PKG-INFO` & `brainrender-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainrender
-Version: 2.1.6
+Version: 2.1.7
 Summary: Visualisation and exploration of brain atlases and other anatomical data
 Author-email: "Federico Claudi, Adam Tyson, Luigi Petrucco" <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainrender
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainrender/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainrender/index.html
```

### Comparing `brainrender-2.1.6/README.md` & `brainrender-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/__init__.py` & `brainrender-2.1.7/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/_colors.py` & `brainrender-2.1.7/brainrender/_colors.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/_io.py` & `brainrender-2.1.7/brainrender/_io.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/_jupyter.py` & `brainrender-2.1.7/brainrender/_jupyter.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/_utils.py` & `brainrender-2.1.7/brainrender/_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/_video.py` & `brainrender-2.1.7/brainrender/_video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actor.py` & `brainrender-2.1.7/brainrender/actor.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/cylinder.py` & `brainrender-2.1.7/brainrender/actors/cylinder.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/neurons.py` & `brainrender-2.1.7/brainrender/actors/neurons.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/points.py` & `brainrender-2.1.7/brainrender/actors/points.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/ruler.py` & `brainrender-2.1.7/brainrender/actors/ruler.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/streamlines.py` & `brainrender-2.1.7/brainrender/actors/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/actors/volume.py` & `brainrender-2.1.7/brainrender/actors/volume.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/atlas.py` & `brainrender-2.1.7/brainrender/atlas.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py` & `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py` & `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/atlas_specific/allen_brain_atlas/streamlines.py` & `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/camera.py` & `brainrender-2.1.7/brainrender/camera.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/cameras.py` & `brainrender-2.1.7/brainrender/cameras.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/render.py` & `brainrender-2.1.7/brainrender/render.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/CC_134_1_ch1inj.obj` & `brainrender-2.1.7/brainrender/resources/CC_134_1_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/CC_134_2_ch1inj.obj` & `brainrender-2.1.7/brainrender/resources/CC_134_2_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/neuron1.swc` & `brainrender-2.1.7/brainrender/resources/neuron1.swc`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/probe_1_striatum.npy` & `brainrender-2.1.7/brainrender/resources/probe_1_striatum.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/probe_2_RSP.npy` & `brainrender-2.1.7/brainrender/resources/probe_2_RSP.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/random_cells.h5` & `brainrender-2.1.7/brainrender/resources/random_cells.h5`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/random_cells.npy` & `brainrender-2.1.7/brainrender/resources/random_cells.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/resources/volume.npy` & `brainrender-2.1.7/brainrender/resources/volume.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/scene.py` & `brainrender-2.1.7/brainrender/scene.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/settings.py` & `brainrender-2.1.7/brainrender/settings.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender/video.py` & `brainrender-2.1.7/brainrender/video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.6/brainrender.egg-info/PKG-INFO` & `brainrender-2.1.7/brainrender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainrender
-Version: 2.1.6
+Version: 2.1.7
 Summary: Visualisation and exploration of brain atlases and other anatomical data
 Author-email: "Federico Claudi, Adam Tyson, Luigi Petrucco" <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainrender
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainrender/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainrender/index.html
```

### Comparing `brainrender-2.1.6/brainrender.egg-info/SOURCES.txt` & `brainrender-2.1.7/brainrender.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 brainrender.egg-info/PKG-INFO
 brainrender.egg-info/SOURCES.txt
 brainrender.egg-info/dependency_links.txt
 brainrender.egg-info/requires.txt
 brainrender.egg-info/top_level.txt
 brainrender/actors/__init__.py
 brainrender/actors/cylinder.py
+brainrender/actors/line.py
 brainrender/actors/neurons.py
 brainrender/actors/points.py
 brainrender/actors/ruler.py
 brainrender/actors/streamlines.py
 brainrender/actors/volume.py
 brainrender/atlas_specific/__init__.py
 brainrender/atlas_specific/allen_brain_atlas/streamlines.py
```

### Comparing `brainrender-2.1.6/pyproject.toml` & `brainrender-2.1.7/pyproject.toml`

 * *Files identical despite different names*

