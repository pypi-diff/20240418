# Comparing `tmp/chess2vec-0.2.1b7.tar.gz` & `tmp/chess2vec-0.2.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.2.1b7.tar", max compression
+gzip compressed data, was "chess2vec-0.2.1b8.tar", max compression
```

## Comparing `chess2vec-0.2.1b7.tar` & `chess2vec-0.2.1b8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b7/README.md
--rw-r--r--   0        0        0     4809 2024-04-18 18:16:32.898139 chess2vec-0.2.1b7/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b7/chess2vec/pgn.py
--rw-r--r--   0        0        0      571 2024-04-18 18:14:08.796474 chess2vec-0.2.1b7/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b7/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b7/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-18 18:16:37.114855 chess2vec-0.2.1b7/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b8/README.md
+-rw-r--r--   0        0        0     4734 2024-04-18 18:37:59.491461 chess2vec-0.2.1b8/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b8/chess2vec/pgn.py
+-rw-r--r--   0        0        0      571 2024-04-18 18:14:08.796474 chess2vec-0.2.1b8/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b8/chess2vec/utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b8/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-18 18:38:08.808253 chess2vec-0.2.1b8/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b8/PKG-INFO
```

### Comparing `chess2vec-0.2.1b7/chess2vec/__init__.py` & `chess2vec-0.2.1b8/chess2vec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,16 +107,15 @@
 
     @property
     def size(self) -> int:
         return self.entries.shape[0]
 
     def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
-            child = self.__new__(type(self))
-            child.__init__(self.rep, self.with_fen)
+            child = self.__class__(self.rep, with_fen=self.with_fen)
 
             child.entries = self.entries[idx : idx + batch_size]
             child._update_labels(self.labels[idx : idx + batch_size])
 
             yield child
 
     def shuffle(self, *, seed: int = 42):
@@ -129,16 +128,15 @@
             self.labels = list(np.array(self.labels)[idx])
             
     def sample(self, sample_size: int | float, *, seed: int = 42):
         if isinstance(sample_size, float):
             assert 0.0 <= sample_size <= 1.0
             sample_size = self.size * sample_size
         
-        sample = self.__new__(type(self))
-        sample.__init__(self.rep, self.with_fen)
+        sample = self.__class__(self.rep, with_fen=self.with_fen)
         
         rng = np.random.default_rng(seed)
         idx = rng.permutation(sample_size)
         
         sample.entries = self.entries[idx]
         sample._update_labels(list(np.array(self.labels)[idx]))
         
@@ -146,16 +144,15 @@
 
     def cov(self) -> np.ndarray:
         return sparse.covs(self.entries.T).toarray()
 
     def __add__(self, item):
         assert isinstance(item, type(self))
 
-        new = self.__new__(type(self))
-        new.__init__(self.rep, self.with_fen)
+        new = self.__class__(self.rep, with_fen=self.with_fen)
 
         new.entries = sparse.vstack([self.entries, item.entries])
 
         if self.with_fen:
             new.labels = self.labels + item.labels
 
         return new
```

### Comparing `chess2vec-0.2.1b7/chess2vec/utils/__init__.py` & `chess2vec-0.2.1b8/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b7/chess2vec/utils/sparse.py` & `chess2vec-0.2.1b8/chess2vec/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b7/chess2vec/utils/vector.py` & `chess2vec-0.2.1b8/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b7/PKG-INFO` & `chess2vec-0.2.1b8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.2.1b7
+Version: 0.2.1b8
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

