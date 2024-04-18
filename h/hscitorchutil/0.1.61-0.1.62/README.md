# Comparing `tmp/hscitorchutil-0.1.61.tar.gz` & `tmp/hscitorchutil-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscitorchutil-0.1.61.tar", max compression
+gzip compressed data, was "hscitorchutil-0.1.62.tar", max compression
```

## Comparing `hscitorchutil-0.1.61.tar` & `hscitorchutil-0.1.62.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.61/README.md
--rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.61/hscitorchutil/callbacks.py
--rw-r--r--   0        0        0     8520 2024-03-28 11:52:22.341913 hscitorchutil-0.1.61/hscitorchutil/dataset.py
--rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.61/hscitorchutil/fsspec.py
--rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.61/hscitorchutil/processlocal.py
--rw-r--r--   0        0        0     9968 2024-01-12 13:06:49.061793 hscitorchutil-0.1.61/hscitorchutil/sqlite.py
--rw-r--r--   0        0        0      908 2024-03-28 20:15:26.106818 hscitorchutil-0.1.61/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.61/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.62/README.md
+-rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.62/hscitorchutil/callbacks.py
+-rw-r--r--   0        0        0     8694 2024-04-17 14:29:04.250160 hscitorchutil-0.1.62/hscitorchutil/dataset.py
+-rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.62/hscitorchutil/fsspec.py
+-rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.62/hscitorchutil/processlocal.py
+-rw-r--r--   0        0        0     9968 2024-01-12 13:06:49.061793 hscitorchutil-0.1.62/hscitorchutil/sqlite.py
+-rw-r--r--   0        0        0      908 2024-04-17 15:22:40.330720 hscitorchutil-0.1.62/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.62/PKG-INFO
```

### Comparing `hscitorchutil-0.1.61/hscitorchutil/callbacks.py` & `hscitorchutil-0.1.62/hscitorchutil/callbacks.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.61/hscitorchutil/dataset.py` & `hscitorchutil-0.1.62/hscitorchutil/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import bisect
 import random
-from typing import Any, Callable, Optional, Sequence, TypeVar
+from typing import Any, Callable, Optional, Sequence, TypeVar, Generic
 import torch
 from torch.utils.data import Dataset
+import torch.utils.data
 import logging
 
 T_co = TypeVar('T_co', covariant=True)
 
 
-class LinearMapSubset(Dataset[T_co]):
+class LinearMapSubset(Dataset[T_co], Generic[T_co]):
     r"""
     Slice a map dataset at specified indices.
 
     Args:
         dataset (Dataset[T_co]): The whole map dataset
         indices (sequence): Indices in the whole set selected for subset
     """
@@ -42,15 +43,15 @@
     def __len__(self):
         return self.end - self.start
 
 
 T2_co = TypeVar('T2_co', covariant=True)
 
 
-class TransformedMapDataset(Dataset[T2_co]):
+class TransformedMapDataset(Dataset[T2_co], Generic[T2_co, T_co]):
     r"""Create a transformed map dataset by applying a transform function to all samples.
 
     Args:
         dataset (Dataset[T_co]): The underlying map dataset
         transform (Callable[T:co,T2_co]): The transformation function to be applied to each sample
     """
 
@@ -69,15 +70,15 @@
         else:
             return self.transform([self.dataset[idx] for idx in indices])
 
     def __len__(self):
         return len(self.dataset)  # type: ignore
 
 
-class ShuffledMapDataset(Dataset[T_co]):
+class ShuffledMapDataset(Dataset[T_co], Generic[T_co]):
     r"""
     Shuffle the input map dataset via its indices.
 
     Args:
         dataset (Dataset): Map dataset being shuffled
         seed: (int, optional): The seed to be used for shuffling. If not provided, the current time is used.
         indices (list[Any]): a list of indices for the parent Dataset. If not provided, we assume it uses 0-based indexing
@@ -133,15 +134,15 @@
 
 
 def _log_exception(ds: 'ExceptionHandlingMapDataset', idx: int, e: Exception) -> None:
     logging.exception(
         f"ExceptionHandlingMapDataset encountered exception at index {idx}. Returning None.")
 
 
-class ExceptionHandlingMapDataset(Dataset[T_co]):
+class ExceptionHandlingMapDataset(Dataset[T_co], Generic[T_co]):
     r"""A dataset wrapper that catches exceptions and instead of bailing out, returns None.
 
     Args:
         dataset (Dataset[T_co]): The underlying map dataset
         on_exception (Callable[[int, Exception],Any]): The function to be called when an exception is raised.
     """
 
@@ -166,26 +167,26 @@
         else:
             return [self.__getitem__(idx) for idx in indices]  # type: ignore
 
     def __len__(self):
         return len(self.dataset)  # type: ignore
 
 
-class DatasetToIterableDataset(torch.utils.data.IterableDataset):
-    def __init__(self, dataset: torch.utils.data.Dataset):
+class DatasetToIterableDataset(torch.utils.data.IterableDataset[T_co], Generic[T_co]):
+    def __init__(self, dataset: torch.utils.data.Dataset[T_co]):
         self.dataset = dataset
 
     def __iter__(self):
         if hasattr(self.dataset, "__iter__"):
-            return self.dataset.__iter__()
-        for i in range(len(self.dataset)):
+            return self.dataset.__iter__()  # type: ignore
+        for i in range(len(self.dataset)):  # type: ignore
             yield self.dataset[i]
 
 
-class UnionMapDataset(Dataset[T_co]):
+class UnionMapDataset(Dataset[T_co], Generic[T_co]):
     def __init__(self, datasets: Sequence[Dataset[T_co]]) -> None:
         self.datasets = datasets
         self.supports_getitems = True
         start = 0
         self.start_offsets = []
         for dataset in datasets:
             if not callable(getattr(dataset, "__getitems__", None)):
```

### Comparing `hscitorchutil-0.1.61/hscitorchutil/fsspec.py` & `hscitorchutil-0.1.62/hscitorchutil/fsspec.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.61/hscitorchutil/processlocal.py` & `hscitorchutil-0.1.62/hscitorchutil/processlocal.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.61/hscitorchutil/sqlite.py` & `hscitorchutil-0.1.62/hscitorchutil/sqlite.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.61/pyproject.toml` & `hscitorchutil-0.1.62/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hscitorchutil"
-version = "0.1.61"
+version = "0.1.62"
 description = "HSCI research group utilities for pytorch (lightning)"
 authors = ["Eetu Mäkelä <eetu.makela@helsinki.fi>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hsci-r/hscitorchutil"
 keywords = [
     "pytorch",
```

### Comparing `hscitorchutil-0.1.61/PKG-INFO` & `hscitorchutil-0.1.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscitorchutil
-Version: 0.1.61
+Version: 0.1.62
 Summary: HSCI research group utilities for pytorch (lightning)
 Home-page: https://github.com/hsci-r/hscitorchutil
 License: MIT
 Keywords: pytorch,dataset
 Author: Eetu Mäkelä
 Author-email: eetu.makela@helsinki.fi
 Requires-Python: >=3.10,<3.12
```

