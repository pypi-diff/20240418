# Comparing `tmp/torch-distmap-0.1.0.tar.gz` & `tmp/torch-distmap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch-distmap-0.1.0.tar", last modified: Fri Oct 28 18:09:44 2022, max compression
+gzip compressed data, was "dist/torch-distmap-0.2.0.tar", last modified: Thu Apr 18 11:13:52 2024, max compression
```

## Comparing `torch-distmap-0.1.0.tar` & `torch-distmap-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4766 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/torch_distmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (121)      203 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/distmap/
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/_l1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5389 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/distmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/l1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/_l2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10655 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/jit_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/l2.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/distmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    78254 2022-10-28 18:08:51.000000 torch-distmap-0.1.0/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4766 2022-10-28 18:09:44.000000 torch-distmap-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       50 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3186 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/distmap/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/_l1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/distmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10655 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/jit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/jitfields.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2251 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/l1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2449 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/l2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5389 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/distmap/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      911 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 11:13:52.000000 torch-distmap-0.2.0/torch_distmap.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    78254 2024-04-18 11:13:28.000000 torch-distmap-0.2.0/versioneer.py
```

### Comparing `torch-distmap-0.1.0/setup.cfg` & `torch-distmap-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/README.md` & `torch-distmap-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,28 @@
 
 Although it is in PyTorch, our implementation performs loops across 
 voxels and hence quite slow. Moreover, it takes masks as an input 
 and therefore does not allow backpropagation.
 
 ## Installation
 
+### Dependency
+
+- `torch >= 1.3`
+
+### Conda
+
+```shell
+conda install torch-distmap -c balbasty -c pytorch
+```
+
+### Pip
+
 ```shell
-pip install git+https://github.com/balbasty/torch-distmap
+pip install torch-distmap
 ```
 
 ## API
 
 ```python
 euclidean_distance_transform(x, ndim=None, vx=1)
 """Compute the Euclidean distance transform of a binary image
```

### Comparing `torch-distmap-0.1.0/torch_distmap.egg-info/PKG-INFO` & `torch-distmap-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-distmap
-Version: 0.1.0
+Version: 0.2.0
 Summary: Euclidean distance transform in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-distmap
 Description: # torch-distmap
@@ -19,16 +19,28 @@
         
         Although it is in PyTorch, our implementation performs loops across 
         voxels and hence quite slow. Moreover, it takes masks as an input 
         and therefore does not allow backpropagation.
         
         ## Installation
         
+        ### Dependency
+        
+        - `torch >= 1.3`
+        
+        ### Conda
+        
+        ```shell
+        conda install torch-distmap -c balbasty -c pytorch
+        ```
+        
+        ### Pip
+        
         ```shell
-        pip install git+https://github.com/balbasty/torch-distmap
+        pip install torch-distmap
         ```
         
         ## API
         
         ```python
         euclidean_distance_transform(x, ndim=None, vx=1)
         """Compute the Euclidean distance transform of a binary image
@@ -131,9 +143,9 @@
 Platform: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `torch-distmap-0.1.0/distmap/_l1.py` & `torch-distmap-0.2.0/distmap/_l1.py`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/distmap/utils.py` & `torch-distmap-0.2.0/distmap/utils.py`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/distmap/l1.py` & `torch-distmap-0.2.0/distmap/l1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ['l1_distance_transform', 'l1_signed_transform']
 
 from .utils import make_vector
 from ._l1 import l1dt_1d_
+from . import backend, jitfields
 import torch
 
 
 def l1_distance_transform(x, ndim=None, vx=1):
     """Compute the L1 distance transform of a binary image
 
     Parameters
@@ -26,14 +27,17 @@
     References
     ----------
     ..[1] "Distance Transforms of Sampled Functions"
           Pedro F. Felzenszwalb & Daniel P. Huttenlocher
           Theory of Computing (2012)
           https://www.theoryofcomputing.org/articles/v008a019/v008a019.pdf
     """
+    if backend.jitfields and jitfields.available:
+        return jitfields.l1_distance_transform(x, ndim, vx)
+
     dtype = x.dtype if x.dtype.is_floating_point else torch.get_default_dtype()
     x = x.to(dtype, copy=True)
     x.masked_fill_(x > 0, float('inf'))
     ndim = ndim or x.dim()
     vx = make_vector(vx, ndim, dtype=torch.float).tolist()
     for d, w in enumerate(vx):
         x = l1dt_1d_(x, d - ndim, w)
```

### Comparing `torch-distmap-0.1.0/distmap/_l2.py` & `torch-distmap-0.2.0/distmap/_l2.py`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/distmap/jit_utils.py` & `torch-distmap-0.2.0/distmap/jit_utils.py`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/distmap/l2.py` & `torch-distmap-0.2.0/distmap/l2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = ['euclidean_distance_transform', 'euclidean_signed_transform']
 
+from . import backend, jitfields
 from .utils import make_vector
 from ._l1 import l1dt_1d_
 from ._l2 import edt_1d
 import torch
 
 
 def euclidean_distance_transform(x, ndim=None, vx=1):
@@ -27,14 +28,17 @@
     References
     ----------
     ..[1] "Distance Transforms of Sampled Functions"
           Pedro F. Felzenszwalb & Daniel P. Huttenlocher
           Theory of Computing (2012)
           https://www.theoryofcomputing.org/articles/v008a019/v008a019.pdf
     """
+    if backend.jitfields and jitfields.available:
+        return jitfields.euclidean_distance_transform(x, ndim, vx)
+
     dtype = x.dtype if x.dtype.is_floating_point else torch.get_default_dtype()
     x = x.to(dtype, copy=True)
     x.masked_fill_(x > 0, float('inf'))
     ndim = ndim or x.dim()
     vx = make_vector(vx, ndim, dtype=torch.float).tolist()
     x = l1dt_1d_(x, -ndim, vx[0]).square_()
     for d, w in zip(range(1, ndim), vx[1:]):
```

### Comparing `torch-distmap-0.1.0/versioneer.py` & `torch-distmap-0.2.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `torch-distmap-0.1.0/PKG-INFO` & `torch-distmap-0.2.0/torch_distmap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-distmap
-Version: 0.1.0
+Version: 0.2.0
 Summary: Euclidean distance transform in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-distmap
 Description: # torch-distmap
@@ -19,16 +19,28 @@
         
         Although it is in PyTorch, our implementation performs loops across 
         voxels and hence quite slow. Moreover, it takes masks as an input 
         and therefore does not allow backpropagation.
         
         ## Installation
         
+        ### Dependency
+        
+        - `torch >= 1.3`
+        
+        ### Conda
+        
+        ```shell
+        conda install torch-distmap -c balbasty -c pytorch
+        ```
+        
+        ### Pip
+        
         ```shell
-        pip install git+https://github.com/balbasty/torch-distmap
+        pip install torch-distmap
         ```
         
         ## API
         
         ```python
         euclidean_distance_transform(x, ndim=None, vx=1)
         """Compute the Euclidean distance transform of a binary image
@@ -131,9 +143,9 @@
 Platform: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

