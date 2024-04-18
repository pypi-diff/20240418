# Comparing `tmp/chess2vec-0.2.1b4.tar.gz` & `tmp/chess2vec-0.2.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.2.1b4.tar", max compression
+gzip compressed data, was "chess2vec-0.2.1b5.tar", max compression
```

## Comparing `chess2vec-0.2.1b4.tar` & `chess2vec-0.2.1b5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b4/README.md
--rw-r--r--   0        0        0     4177 2024-04-18 16:14:55.429151 chess2vec-0.2.1b4/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b4/chess2vec/pgn.py
--rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b4/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b4/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b4/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-18 16:15:19.886201 chess2vec-0.2.1b4/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b5/README.md
+-rw-r--r--   0        0        0     4756 2024-04-18 16:26:26.023301 chess2vec-0.2.1b5/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b5/chess2vec/pgn.py
+-rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b5/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b5/chess2vec/utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b5/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-18 16:26:36.143459 chess2vec-0.2.1b5/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b5/PKG-INFO
```

### Comparing `chess2vec-0.2.1b4/chess2vec/__init__.py` & `chess2vec-0.2.1b5/chess2vec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,38 +106,54 @@
     @property
     def size(self) -> int:
         return self.entries.shape[0]
 
     def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
             child = self.__new__(type(self))
-            child.__init__(self.with_fen)
+            child.__init__(self.rep, self.with_fen)
 
             child.entries = self.entries[idx : idx + batch_size]
             child._update_labels(self.labels[idx : idx + batch_size])
 
             yield child
 
     def shuffle(self, *, seed: int = 42):
         rng = np.random.default_rng(seed)
         idx = rng.permutation(len(self.entries))
 
         self.entries = self.entries[idx]
 
         if self.with_fen:
             self.labels = list(np.array(self.labels)[idx])
+            
+    def sample(self, sample_size: int | float, *, seed: int = 42):
+        if isinstance(sample_size, float):
+            assert 0.0 <= sample_size <= 1.0
+            sample_size = self.size * sample_size
+        
+        sample = self.__new__(type(self))
+        sample.__init__(self.rep, self.with_fen)
+        
+        rng = np.random.default_rng(seed)
+        idx = rng.permutation(sample_size)
+        
+        sample.entries = self.entries[idx]
+        sample._update_labels(list(np.array(self.labels)[idx]))
+        
+        return sample
 
     def cov(self) -> np.ndarray:
         return sparse.covs(self.entries.T).toarray()
 
     def __add__(self, item):
         assert isinstance(item, type(self))
 
         new = self.__new__(type(self))
-        new.__init__(self.with_fen)
+        new.__init__(self.rep, self.with_fen)
 
         new.entries = sparse.vstack([self.entries, item.entries])
 
         if self.with_fen:
             new.labels = self.labels + item.labels
 
         return new
```

### Comparing `chess2vec-0.2.1b4/chess2vec/utils/__init__.py` & `chess2vec-0.2.1b5/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b4/chess2vec/utils/sparse.py` & `chess2vec-0.2.1b5/chess2vec/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b4/chess2vec/utils/vector.py` & `chess2vec-0.2.1b5/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b4/PKG-INFO` & `chess2vec-0.2.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.2.1b4
+Version: 0.2.1b5
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

