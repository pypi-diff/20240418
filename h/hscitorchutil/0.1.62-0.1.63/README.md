# Comparing `tmp/hscitorchutil-0.1.62.tar.gz` & `tmp/hscitorchutil-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscitorchutil-0.1.62.tar", max compression
+gzip compressed data, was "hscitorchutil-0.1.63.tar", max compression
```

## Comparing `hscitorchutil-0.1.62.tar` & `hscitorchutil-0.1.63.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.62/README.md
--rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.62/hscitorchutil/callbacks.py
--rw-r--r--   0        0        0     8694 2024-04-17 14:29:04.250160 hscitorchutil-0.1.62/hscitorchutil/dataset.py
--rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.62/hscitorchutil/fsspec.py
--rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.62/hscitorchutil/processlocal.py
--rw-r--r--   0        0        0     9968 2024-01-12 13:06:49.061793 hscitorchutil-0.1.62/hscitorchutil/sqlite.py
--rw-r--r--   0        0        0      908 2024-04-17 15:22:40.330720 hscitorchutil-0.1.62/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.62/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.63/README.md
+-rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.63/hscitorchutil/callbacks.py
+-rw-r--r--   0        0        0     8694 2024-04-17 14:29:04.250160 hscitorchutil-0.1.63/hscitorchutil/dataset.py
+-rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.63/hscitorchutil/fsspec.py
+-rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.63/hscitorchutil/processlocal.py
+-rw-r--r--   0        0        0     8723 2024-04-18 07:22:14.216785 hscitorchutil-0.1.63/hscitorchutil/sqlite.py
+-rw-r--r--   0        0        0      908 2024-04-18 07:54:41.748398 hscitorchutil-0.1.63/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.63/PKG-INFO
```

### Comparing `hscitorchutil-0.1.62/hscitorchutil/callbacks.py` & `hscitorchutil-0.1.63/hscitorchutil/callbacks.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.62/hscitorchutil/dataset.py` & `hscitorchutil-0.1.63/hscitorchutil/dataset.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.62/hscitorchutil/fsspec.py` & `hscitorchutil-0.1.63/hscitorchutil/fsspec.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.62/hscitorchutil/processlocal.py` & `hscitorchutil-0.1.63/hscitorchutil/processlocal.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.62/hscitorchutil/sqlite.py` & `hscitorchutil-0.1.63/hscitorchutil/sqlite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 import logging
 import os
 import sqlite3
-from typing import Callable, Generic, Optional, Tuple, TypeVar, Sequence
+from typing import Callable, Generic, Iterable, Iterator, Optional, Tuple, TypeVar, Sequence, TypeVarTuple, cast
 from zipfile import ZipFile
 import click
 import fsspec
+import torch.utils.data.dataloader
 from torch.utils.data import Dataset, DataLoader
 import torch
 import lightning.pytorch
 from edzip.sqlite import create_sqlite_directory_from_zip
-from hscitorchutil.dataset import UnionMapDataset
 from hscitorchutil.fsspec import get_s3fs_credentials, cache_locally_if_remote
 
+Ts = TypeVarTuple("Ts")
 T_co = TypeVar('T_co', covariant=True)
 T2_co = TypeVar('T2_co', covariant=True)
 
 
-def _identity(x: Sequence[Tuple]) -> Sequence[Tuple]:
+def _identity(x: T_co) -> T_co:
     return x
 
 
-class SQLiteDataset(Dataset[T2_co], Generic[T_co, T2_co]):
-    # type: ignore
-    def __init__(self, sqlite_filename: str, table_name: str, index_column: str, columns_to_return: str, id_column: str | None = None, transform: Callable[[Sequence[T_co]], Sequence[T2_co]] = _identity):
+class SQLiteDataset(Dataset[T_co], Generic[*Ts, T_co]):
+    def __init__(self, sqlite_filename: str, table_name: str, index_column: str, columns_to_return: str, id_column: str):
         self.sqlite_filename = sqlite_filename
         self.table_name = table_name
         self.index_column = index_column
         self.id_column = id_column
         self.columns_to_return = columns_to_return
-        self.transform = transform
         self.sqlite = sqlite3.connect(sqlite_filename)
         self._len = self.sqlite.execute(
             f"SELECT COUNT(*) FROM {table_name}").fetchone()[0]
 
     def __len__(self):
         return self._len
 
-    def __getitem__(self, idx: int | str) -> T2_co:
+    def __getitem__(self, idx: int | str) -> T_co:
         return self.__getitems__([idx])[0]
 
-    def __getitems__(self, idxs: Sequence[int | str]) -> Sequence[T2_co]:
+    def __getitems__(self, idxs: Sequence[int | str]) -> Sequence[T_co]:
         if isinstance(idxs[0], int):
-            return self.transform(
-                self.sqlite.execute(f"SELECT {self.columns_to_return} FROM {self.table_name} WHERE {self.index_column} IN (%s)" % ','.join(
-                    '?' * len(idxs)), idxs).fetchall(),
-            )
+            return self.sqlite.execute(f"SELECT {self.columns_to_return} FROM {self.table_name} WHERE {self.index_column} IN (%s)" % ','.join(
+                '?' * len(idxs)), idxs).fetchall()
         else:
-            return self.transform(
-                self.sqlite.execute(f"SELECT {self.columns_to_return} FROM {self.table_name} WHERE {self.id_column} IN (%s)" % ','.join(
-                    '?' * len(idxs)), idxs).fetchall(),
-            )
+            return self.sqlite.execute(f"SELECT {self.columns_to_return} FROM {self.table_name} WHERE {self.id_column} IN (%s)" % ','.join(
+                '?' * len(idxs)), idxs).fetchall()
 
     def __setstate__(self, state):
         (
             self.sqlite_filename,
             self.table_name,
             self.index_column,
             self.columns_to_return,
@@ -84,66 +79,56 @@
         except Exception as e:
             logging.exception("Failed to collate batch, returning None")
             return None
     logging.warn("Batch is empty, returning None")
     return None
 
 
-def get_test_dataset(train_dataset: Dataset[T_co], val_dataset: Dataset[T_co], test_dataset: Dataset[T_co]) -> Dataset[T_co]:
-    return test_dataset
+class TypedDataLoader(Iterable[T_co], DataLoader[T_co], Generic[T_co]):
+    pass
 
 
-def combine_datasets(train_dataset: Dataset[T_co], val_dataset: Dataset[T_co], test_dataset: Dataset[T_co]) -> Dataset[T_co]:
-    return UnionMapDataset([train_dataset, val_dataset, test_dataset])
-
-
-class SQLiteDataModule(lightning.pytorch.LightningDataModule, Generic[T_co, T2_co]):
+class SQLiteDataModule(lightning.pytorch.LightningDataModule, Generic[*Ts, T_co, T2_co]):
     def __init__(self,
                  train_sqlite_url: str,
                  val_sqlite_url: str,
                  test_sqlite_url: str,
                  cache_dir: str,
                  table_name: str,
                  index_column: str,
                  columns_to_return: str,
-                 id_column: str | None = None,
+                 id_column: str,
                  storage_options: dict = dict(),
                  batch_size: int = 64,
                  num_workers: int = 0,
                  train_transform: Callable[[
-                     Sequence[T_co]], Sequence[T2_co]] = _identity,
+                     Dataset[tuple[*Ts]]], Dataset[T_co]] = _identity,
                  test_transform: Callable[[
-                     Sequence[T_co]], Sequence[T2_co]] = _identity,
+                     Dataset[tuple[*Ts]]], Dataset[T_co]] = _identity,
                  prepare_data_per_node: bool = True,
-                 collate_fn: Optional[Callable] = _remove_nones_from_batch,
-                 get_predict_dataset: Callable[[Dataset[T2_co], Dataset[T2_co], Dataset[T2_co]], Dataset[T2_co]] = get_test_dataset):
+                 collate_fn: Optional[Callable[[Sequence[T_co]], T2_co]] = _remove_nones_from_batch):
         self.train_sqlite_url = train_sqlite_url
         self.val_sqlite_url = val_sqlite_url
         self.test_sqlite_url = test_sqlite_url
         self.cache_dir = cache_dir
         self.storage_options = storage_options
         self.batch_size = batch_size
         self.num_workers = num_workers
 
         self.table_name = table_name
         self.index_column = index_column
         self.columns_to_return = columns_to_return
         self.id_column = id_column
-
-        self.train_transform: Callable[[
-            Sequence[T_co]], Sequence[T2_co]] = train_transform
-        self.test_transform: Callable[[
-            Sequence[T_co]], Sequence[T2_co]] = test_transform
+        self.train_transform = train_transform
+        self.test_transform = test_transform
         self.prepare_data_per_node = prepare_data_per_node
         self.collate_fn = collate_fn
         self.train_dataset = None
         self.val_dataset = None
         self.test_dataset = None
-        self.predict_dataset = None
-        self.get_predict_dataset = get_predict_dataset
         super().__init__()
 
     def prepare_data(self):
         # download, IO, etc. Useful with shared filesystems
         # only called on 1 GPU/TPU in distributed
 
         # Ensure sqlite databases are downloaded
@@ -151,57 +136,51 @@
             self.train_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
         cache_locally_if_remote(
             self.val_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
         cache_locally_if_remote(
             self.test_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
 
     def setup(self, stage: Optional[str] = None):
-        if (stage is None or stage == "fit" or (self.predict_dataset is None and stage == "predict")) and self.train_dataset is None:
-            self.train_dataset = SQLiteDataset(cache_locally_if_remote(
+        if (stage is None or stage == "fit") and self.train_dataset is None:
+            self.train_dataset = self.train_transform(SQLiteDataset(cache_locally_if_remote(
                 self.train_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
-                self.id_column,
-                self.train_transform)
-        if (stage is None or stage == "fit" or stage == "validate" or (self.predict_dataset is None and stage == "predict")) and self.val_dataset is None:
-            self.val_dataset = SQLiteDataset(cache_locally_if_remote(
+                self.id_column))
+        if (stage is None or stage == "fit" or stage == "validate") and self.val_dataset is None:
+            self.val_dataset = self.test_transform(SQLiteDataset(cache_locally_if_remote(
                 self.val_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
-                self.id_column,
-                self.test_transform)
-        if (stage is None or stage == "test" or (self.predict_dataset is None and stage == "predict")) and self.test_dataset is None:
-            self.test_dataset = SQLiteDataset(cache_locally_if_remote(
+                self.id_column))
+        if (stage is None or stage == "test") and self.test_dataset is None:
+            self.test_dataset = self.test_transform(SQLiteDataset(cache_locally_if_remote(
                 self.test_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
-                self.id_column,
-                self.test_transform)
-        if (stage is None or stage == "predict") and self.predict_dataset is None:
-            self.predict_dataset = self.get_predict_dataset(
-                self.train_dataset, self.val_dataset, self.test_dataset)  # type: ignore
-
-    def train_dataloader(self) -> DataLoader[T2_co]:
-        return DataLoader(self.train_dataset, shuffle=True, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0,  # type: ignore
-                          collate_fn=self.collate_fn, pin_memory=True)
-
-    def val_dataloader(self) -> DataLoader[T2_co] | None:
-        if self.val_dataset is not None:
-            return DataLoader(self.val_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True)
-
-    def test_dataloader(self) -> DataLoader[T2_co] | None:
-        if self.test_dataset is not None:
-            return DataLoader(self.test_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True)
-
-    def predict_dataloader(self) -> DataLoader[T2_co] | None:
-        if self.predict_dataset is not None:
-            return DataLoader(self.predict_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True)
+                self.id_column))
+
+    def train_dataloader(self) -> TypedDataLoader[T2_co]:
+        if self.train_dataset is None:
+            raise ValueError("Training dataset not available")
+        return cast(TypedDataLoader[T2_co], DataLoader(self.train_dataset, shuffle=True, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0,
+                                                       collate_fn=self.collate_fn, pin_memory=True))
+
+    def val_dataloader(self) -> TypedDataLoader[T2_co]:
+        if self.val_dataset is None:
+            raise ValueError("Validation dataset not available")
+        return cast(TypedDataLoader[T2_co], DataLoader(self.val_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True))
+
+    def test_dataloader(self) -> TypedDataLoader[T2_co]:
+        if self.test_dataset is None:
+            raise ValueError("Test dataset not available")
+        return cast(TypedDataLoader[T2_co], DataLoader(self.test_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True))
 
     def teardown(self, stage: str):
         # clean up state after the trainer stops, delete files...
         # called on every process in DDP
         pass
```

### Comparing `hscitorchutil-0.1.62/pyproject.toml` & `hscitorchutil-0.1.63/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hscitorchutil"
-version = "0.1.62"
+version = "0.1.63"
 description = "HSCI research group utilities for pytorch (lightning)"
 authors = ["Eetu Mäkelä <eetu.makela@helsinki.fi>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hsci-r/hscitorchutil"
 keywords = [
     "pytorch",
```

### Comparing `hscitorchutil-0.1.62/PKG-INFO` & `hscitorchutil-0.1.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscitorchutil
-Version: 0.1.62
+Version: 0.1.63
 Summary: HSCI research group utilities for pytorch (lightning)
 Home-page: https://github.com/hsci-r/hscitorchutil
 License: MIT
 Keywords: pytorch,dataset
 Author: Eetu Mäkelä
 Author-email: eetu.makela@helsinki.fi
 Requires-Python: >=3.10,<3.12
```

