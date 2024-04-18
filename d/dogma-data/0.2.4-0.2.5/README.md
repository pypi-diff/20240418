# Comparing `tmp/dogma-data-0.2.4.tar.gz` & `tmp/dogma_data-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogma-data-0.2.4.tar", last modified: Wed Apr 10 08:57:15 2024, max compression
+gzip compressed data, was "dogma_data-0.2.5.tar", last modified: Thu Apr 18 18:35:21 2024, max compression
```

## Comparing `dogma-data-0.2.4.tar` & `dogma_data-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/
--rw-r--r--   0 roed     (23269) root         (0)      648 2024-04-10 08:57:15.204752 dogma-data-0.2.4/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma-data-0.2.4/README.md
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/dogma_data/
--rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-10 03:46:52.000000 dogma-data-0.2.4/dogma_data/__init__.py
--rw-r--r--   0 roed     (23269) root         (0)    11007 2024-04-10 05:57:55.000000 dogma-data-0.2.4/dogma_data/_dogma_data.py
--rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma-data-0.2.4/dogma_data/dogma_torch.py
--rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma-data-0.2.4/dogma_data/fasta.py
--rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma-data-0.2.4/dogma_data/utils.py
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/dogma_data.egg-info/
--rw-r--r--   0 roed     (23269) root         (0)      648 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)      308 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/SOURCES.txt
--rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/dependency_links.txt
--rw-r--r--   0 roed     (23269) root         (0)       98 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/requires.txt
--rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/top_level.txt
--rw-r--r--   0 roed     (23269) root         (0)     1078 2024-04-10 08:55:46.000000 dogma-data-0.2.4/pyproject.toml
--rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-10 08:57:15.204752 dogma-data-0.2.4/setup.cfg
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:35:21.593226 dogma_data-0.2.5/
+-rw-r--r--   0 roed     (23269) root         (0)      669 2024-04-18 18:35:21.593226 dogma_data-0.2.5/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma_data-0.2.5/README.md
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:35:21.593226 dogma_data-0.2.5/dogma_data/
+-rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-18 18:31:18.000000 dogma_data-0.2.5/dogma_data/__init__.py
+-rw-r--r--   0 roed     (23269) root         (0)    11589 2024-04-18 18:30:01.000000 dogma_data-0.2.5/dogma_data/_dogma_data.py
+-rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma_data-0.2.5/dogma_data/dogma_torch.py
+-rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma_data-0.2.5/dogma_data/fasta.py
+-rw-r--r--   0 roed     (23269) root         (0)     3287 2024-04-18 18:25:24.000000 dogma_data-0.2.5/dogma_data/sharded_data.py
+-rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma_data-0.2.5/dogma_data/utils.py
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:35:21.593226 dogma_data-0.2.5/dogma_data.egg-info/
+-rw-r--r--   0 roed     (23269) root         (0)      669 2024-04-18 18:35:21.000000 dogma_data-0.2.5/dogma_data.egg-info/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)      335 2024-04-18 18:35:21.000000 dogma_data-0.2.5/dogma_data.egg-info/SOURCES.txt
+-rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-18 18:35:21.000000 dogma_data-0.2.5/dogma_data.egg-info/dependency_links.txt
+-rw-r--r--   0 roed     (23269) root         (0)      104 2024-04-18 18:35:21.000000 dogma_data-0.2.5/dogma_data.egg-info/requires.txt
+-rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-18 18:35:21.000000 dogma_data-0.2.5/dogma_data.egg-info/top_level.txt
+-rw-r--r--   0 roed     (23269) root         (0)     1092 2024-04-18 18:35:15.000000 dogma_data-0.2.5/pyproject.toml
+-rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-18 18:35:21.593226 dogma_data-0.2.5/setup.cfg
```

### Comparing `dogma-data-0.2.4/PKG-INFO` & `dogma_data-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -13,9 +13,10 @@
 Requires-Dist: h5py
 Requires-Dist: awkward
 Requires-Dist: tqdm
 Requires-Dist: cppyy
 Requires-Dist: numba
 Requires-Dist: lightning_cloud
 Requires-Dist: blosc2
-Requires-Dist: dogma-rust>=0.2.0
+Requires-Dist: dogma-rust>=0.2.4
 Requires-Dist: smart-open
+Requires-Dist: click
```

### Comparing `dogma-data-0.2.4/dogma_data/_dogma_data.py` & `dogma_data-0.2.5/dogma_data/_dogma_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import io
 import warnings
 
 import numpy as np
 import blosc2
-from io import BytesIO
+from io import BytesIO, StringIO
 import pickle
 from pathlib import Path
-from typing import Any
+from typing import IO, Any
 import awkward as ak
 
 from numba import njit, prange
 
 from dogma_data.utils import check_equality, timer, ceildiv
 from smart_open import open as smart_open
 
@@ -63,42 +64,51 @@
         return [_decompress_leaves(v) for v in node]
     elif isinstance(node, bytes):
         return blosc2.unpack_array2(node)
     else:
         return node
 
 
-def write_blosc_pickle(node: dict | tuple | list, path: Path):
+def write_blosc_pickle(node: dict | tuple | list, path_or_fileobj: Path | str | IO):
     compressed = _compress_leaves(node)
-    with smart_open(path, 'wb') as f:
-        pickle.dump(compressed, f)
+    if isinstance(path_or_fileobj, (str, Path)):
+        with smart_open(path_or_fileobj, 'wb') as f:
+            pickle.dump(compressed, f)
+    else:
+        pickle.dump(compressed, path_or_fileobj)
 
-def read_blosc_pickle(path: Path) -> dict | tuple | list:
-    with smart_open(path, 'rb') as f, timer('Reading blosc pickle'):
-        compressed = pickle.load(f)
+def read_blosc_pickle(path_or_fileobj: Path | str | IO) -> dict | tuple | list:
+    if isinstance(path_or_fileobj, (str, Path)):
+        with smart_open(path_or_fileobj, 'rb') as f, timer('Reading blosc pickle'):
+            compressed = pickle.load(f)
+    elif isinstance(path_or_fileobj, io.IOBase):
+        with timer('Reading blosc pickle'):
+            compressed = pickle.load(path_or_fileobj)
+    else:
+        raise ValueError(f'path_or_fileobj must be a Path, str, or IO object, not {type(path_or_fileobj)}')
     with timer('Decompressing'):
         return _decompress_leaves(compressed)
 
 
-def write_awkward(arr: ak.Array, path: Path | str):
+def write_awkward(arr: ak.Array, path_or_fileobj: Path | str | IO):
     """
     Write any awkward array to file.
     Compresses the underlying buffers with Blosc2 blosclz for efficient storage and very fast reading/writing with multiple threads.
     """
     blosc2.set_nthreads(64)
     tree = ak.to_buffers(arr)
-    write_blosc_pickle(tree, path)
+    write_blosc_pickle(tree, path_or_fileobj)
 
-def read_awkward(path: Path | str) -> ak.Array:
+def read_awkward(path_or_fileobj: Path | str | IO) -> ak.Array:
     """
     Read any awkward array from file.
     Decompresses using Blosc2 blosclz for very fast reading with multiple threads.
     """
     blosc2.set_nthreads(64)
-    tree = read_blosc_pickle(path)
+    tree = read_blosc_pickle(path_or_fileobj)
     return ak.from_buffers(*tree)
 
 @njit(parallel=True)
 def _fast_pack(seqlens, starts, stops, content):
     """
     Helper function to quickly pack content into a new Awkward array buffer.
     """
```

### Comparing `dogma-data-0.2.4/dogma_data/fasta.py` & `dogma_data-0.2.5/dogma_data/fasta.py`

 * *Files identical despite different names*

### Comparing `dogma-data-0.2.4/dogma_data/utils.py` & `dogma_data-0.2.5/dogma_data/utils.py`

 * *Files identical despite different names*

### Comparing `dogma-data-0.2.4/dogma_data.egg-info/PKG-INFO` & `dogma_data-0.2.5/dogma_data.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -13,9 +13,10 @@
 Requires-Dist: h5py
 Requires-Dist: awkward
 Requires-Dist: tqdm
 Requires-Dist: cppyy
 Requires-Dist: numba
 Requires-Dist: lightning_cloud
 Requires-Dist: blosc2
-Requires-Dist: dogma-rust>=0.2.0
+Requires-Dist: dogma-rust>=0.2.4
 Requires-Dist: smart-open
+Requires-Dist: click
```

### Comparing `dogma-data-0.2.4/pyproject.toml` & `dogma_data-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,32 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dogma-data"
 description = "Data processing for Dogma"
-version = "0.2.4"
+version = "0.2.5"
 requires-python = ">=3.11"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["single-cell", "RNA-seq", "embedding", "pytorch", "uce"]
 dependencies = [
     "lightning",
     "numpy",
     "h5py",
     "awkward",
     "tqdm",
     "cppyy",
     "numba",
     "lightning_cloud",
     "blosc2",
-    "dogma-rust >= 0.2.0",
-    "smart-open"
+    "dogma-rust >= 0.2.4",
+    "smart-open",
+    "click",
 ]
 
 authors = [
     {name = "Marcel Rød", email = "roed@stanford.edu"},
 ]
 
 [tool.setuptools.packages.find]
```

