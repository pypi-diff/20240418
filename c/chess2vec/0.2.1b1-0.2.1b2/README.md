# Comparing `tmp/chess2vec-0.2.1b1.tar.gz` & `tmp/chess2vec-0.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.2.1b1.tar", max compression
+gzip compressed data, was "chess2vec-0.2.1b2.tar", max compression
```

## Comparing `chess2vec-0.2.1b1.tar` & `chess2vec-0.2.1b2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b1/README.md
--rw-r--r--   0        0        0     4218 2024-04-18 16:03:41.945246 chess2vec-0.2.1b1/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b1/chess2vec/pgn.py
--rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b1/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b1/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b1/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-18 16:03:58.252169 chess2vec-0.2.1b1/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b2/README.md
+-rw-r--r--   0        0        0     4209 2024-04-18 16:05:15.756722 chess2vec-0.2.1b2/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b2/chess2vec/pgn.py
+-rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b2/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b2/chess2vec/utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b2/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-18 16:05:21.870151 chess2vec-0.2.1b2/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b2/PKG-INFO
```

### Comparing `chess2vec-0.2.1b1/chess2vec/__init__.py` & `chess2vec-0.2.1b2/chess2vec/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         while game and num_game < max_games:
             board = game.board()
 
             for move in itertools.chain(game.mainline_moves(), [chess.Move.null()]):
                 entries = list(self._entries_getter(board))
                 builder.add_entry(idx, entries, 1, np.uint8)
-                self.utilspdate_labels([board.fen()])
+                self._update_labels([board.fen()])
 
                 board.push(move)
                 idx += 1
 
             if status:
                 bar.update(1)
 
@@ -83,15 +83,15 @@
                         indices,
                         loaded["mat_indptr"],
                     ),
                     shape=(loaded["size"], self.entry_size),
                 )
 
                 self.entries = sparse.vstack([self.entries, mat])
-                self.utilspdate_labels(list(loaded["labels"]))
+                self._update_labels(list(loaded["labels"]))
 
     def save(self, file: str) -> None:
         """saves the already loaded data to a compressed .npz file."""
 
         _save_dict = {}
         _save_dict.update(
             mat_indices=self.entries.indices,
@@ -110,29 +110,29 @@
 
     def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
             child = self.__new__(type(self))
             child.__init__(self.with_fen)
 
             child.entries = self.entries[idx : idx + batch_size]
-            child.utilspdate_labels(self.labels[idx : idx + batch_size])
+            child._update_labels(self.labels[idx : idx + batch_size])
 
             yield child
 
     def shuffle(self, *, seed: int = 42):
         rng = np.random.default_rng(seed)
         idx = rng.permutation(len(self.entries))
 
         self.entries = self.entries[idx]
 
         if self.with_fen:
             self.labels = list(np.array(self.labels)[idx])
 
     def cov(self) -> np.ndarray:
-        return sparse.scov(self.entries.T).toarray()
+        return sparse.covs(self.entries.T).toarray()
 
     def __add__(self, item):
         assert isinstance(item, type(self))
 
         new = self.__new__(type(self))
         new.__init__(self.with_fen)
```

### Comparing `chess2vec-0.2.1b1/chess2vec/utils/__init__.py` & `chess2vec-0.2.1b2/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b1/chess2vec/utils/sparse.py` & `chess2vec-0.2.1b2/chess2vec/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b1/chess2vec/utils/vector.py` & `chess2vec-0.2.1b2/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b1/PKG-INFO` & `chess2vec-0.2.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.2.1b1
+Version: 0.2.1b2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

