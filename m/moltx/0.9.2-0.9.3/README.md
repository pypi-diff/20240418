# Comparing `tmp/moltx-0.9.2.tar.gz` & `tmp/moltx-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-0.9.2.tar", last modified: Wed Apr 17 01:28:00 2024, max compression
+gzip compressed data, was "moltx-0.9.3.tar", last modified: Thu Apr 18 01:48:15 2024, max compression
```

## Comparing `moltx-0.9.2.tar` & `moltx-0.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:28:00.831320 moltx-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 01:27:55.000000 moltx-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-17 01:28:00.831320 moltx-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-17 01:27:55.000000 moltx-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:28:00.827320 moltx-0.9.2/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:28:00.831320 moltx-0.9.2/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-17 01:27:55.000000 moltx-0.9.2/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:28:00.831320 moltx-0.9.2/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-17 01:28:00.000000 moltx-0.9.2/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-17 01:28:00.000000 moltx-0.9.2/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:28:00.000000 moltx-0.9.2/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 01:28:00.000000 moltx-0.9.2/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 01:28:00.000000 moltx-0.9.2/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 01:27:55.000000 moltx-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-17 01:28:00.831320 moltx-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:27:55.000000 moltx-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:28:00.831320 moltx-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-17 01:27:55.000000 moltx-0.9.2/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-17 01:27:55.000000 moltx-0.9.2/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 01:27:55.000000 moltx-0.9.2/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-17 01:27:55.000000 moltx-0.9.2/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:15.233039 moltx-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 01:48:10.000000 moltx-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-18 01:48:15.233039 moltx-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-18 01:48:10.000000 moltx-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:15.229039 moltx-0.9.3/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:15.233039 moltx-0.9.3/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-18 01:48:10.000000 moltx-0.9.3/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:15.233039 moltx-0.9.3/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-18 01:48:15.000000 moltx-0.9.3/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-18 01:48:15.000000 moltx-0.9.3/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:48:15.000000 moltx-0.9.3/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 01:48:15.000000 moltx-0.9.3/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 01:48:15.000000 moltx-0.9.3/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 01:48:10.000000 moltx-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 01:48:15.233039 moltx-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:48:10.000000 moltx-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:48:15.233039 moltx-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 01:48:10.000000 moltx-0.9.3/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-18 01:48:10.000000 moltx-0.9.3/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 01:48:10.000000 moltx-0.9.3/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-18 01:48:10.000000 moltx-0.9.3/tests/test_tokenizer.py
```

### Comparing `moltx-0.9.2/LICENSE` & `moltx-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/PKG-INFO` & `moltx-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.2
+Version: 0.9.3
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.2/README.md` & `moltx-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/data/spe_safe.txt` & `moltx-0.9.3/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/data/spe_smiles.txt` & `moltx-0.9.3/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/data/tks_safe.json` & `moltx-0.9.3/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/data/tks_smiles.json` & `moltx-0.9.3/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/datasets.py` & `moltx-0.9.3/moltx/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,22 @@
         return out.to(self.device)
 
 
 class AdaMR(Base):
     def __call__(self, s1: typing.Sequence[str], s2: typing.Sequence[str]) -> typing.Tuple[torch.Tensor]:
         if len(s1) != len(s2):
             raise RuntimeError("the length of s1 and s2 must be the same!")
+        bos = self.tokenizer[self.tokenizer.BOS]
+        eos = self.tokenizer[self.tokenizer.EOS]
         src = self._tokenize(s1)
-        tgt = self._tokenize([f"{self.tokenizer.BOS}{smi}" for smi in s2])
-        out = self._tokenize([f"{smi}{self.tokenizer.EOS}" for smi in s2])
-        return src, tgt, out
+        s2tokens = [self.tokenizer(smi) for smi in s2]
+        size = max(map(len, s2tokens)) + 1
+        tgt = [self._tokens2tensor([bos] + tks, size).unsqueeze(0) for tks in s2tokens]
+        out = [self._tokens2tensor(tks + [eos], size).unsqueeze(0) for tks in s2tokens]
+        return src, torch.concat(tgt), torch.concat(out)
 
 
 class AdaMRClassifier(AdaMR):
     def __call__(self, smiles: typing.Sequence[str], labels: typing.Sequence[int]) -> typing.Tuple[torch.Tensor]:
         if len(smiles) != len(labels):
             raise RuntimeError(
                 "the length of smiles and labels must be the same!")
```

### Comparing `moltx-0.9.2/moltx/models.py` & `moltx-0.9.3/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/nets.py` & `moltx-0.9.3/moltx/nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/pipelines.py` & `moltx-0.9.3/moltx/pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/moltx/tokenizers.py` & `moltx-0.9.3/moltx/tokenizers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -197,20 +197,20 @@
             if start > pos:
                 tokens.extend(self._smi_tkz(smiles[pos:start]))
             tokens.append(m[0])
             pos = end
             m = self.REGEX.search(smiles, pos=pos)
         if len(smiles) > pos:
             tokens.extend(self._smi_tkz(smiles[pos:]))
+        self._update_tokens(tokens)
         return tokens
 
     def decode(self, token_idxs: typing.Sequence[int]) -> str:
         tokens = [self[idx] for idx in token_idxs]
         return ''.join(tokens)
 
     def encode(self, smiles: str) -> typing.Sequence[int]:
         tokens = self.smi2tokens(smiles)
-        self._update_tokens(tokens)
         return [self[t] for t in tokens]
 
     def __call__(self, smiles: str) -> typing.Sequence[int]:
         return self.encode(smiles)
```

### Comparing `moltx-0.9.2/moltx.egg-info/PKG-INFO` & `moltx-0.9.3/moltx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.2
+Version: 0.9.3
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.2/moltx.egg-info/SOURCES.txt` & `moltx-0.9.3/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/setup.cfg` & `moltx-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/tests/test_datasets.py` & `moltx-0.9.3/tests/test_datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pytest
-from moltx import datasets
+from moltx import datasets, tokenizers as tkz
 
 
 def test_Base(tokenizer):
     ds = datasets.Base(tokenizer)
     smiles = ["<bos>CC[N+](C)(C)Br", "<bos>c1ccccc1"]
     out = ds._tokenize(smiles)
     assert out.shape == (2, 11)
     assert out[0, 0].item() == out[1, 0].item() == ds.tokenizer[ds.tokenizer.BOS]
     assert out[1, -1].item() == 0
 
 
-def test_AdaMR(tokenizer):
+def test_AdaMR():
+    tokenizer = tkz.MoltxTokenizer.from_jsonfile(spe_codes=True, token_size=128, dropout=0.5, spe_merges=256)
     ds = datasets.AdaMR(tokenizer)
-    s1 = ["<bos>CC[N+]CCBr", "<bos>c1ccc1"]
-    s2 = ["<bos>CC[N+]CCBr"]
+    s1 = ["CC[N+]CCBr", "c1ccccc1"]
+    s2 = ["CC[N+]CCBr"]
     with pytest.raises(RuntimeError):
         ds(s1, s2)
-    s2 = ["<bos>CC[N+](C)(C)Br", "<bos>c1ccccc1"]
+    s2 = ["CC[N+](C)(C)Br", ""]
     src, tgt, out = ds(s1, s2)
-    assert src.shape == (2, 7)
-    assert tgt.shape == out.shape == (2, 12)
+    assert src.size(0) == 2 and src.size(1) <= 8
+    assert tgt.shape == out.shape
     assert tgt[0, 1:].eq(out[0, :-1]).all()
 
 def test_AdaMRClassifier(tokenizer):
     ds = datasets.AdaMRClassifier(tokenizer)
     smiles = ["CC[N+]CCBr", "Cc1ccc1"]
     labels = [1, 2]
     with pytest.raises(RuntimeError):
```

### Comparing `moltx-0.9.2/tests/test_nets.py` & `moltx-0.9.3/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/tests/test_pipelines.py` & `moltx-0.9.3/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.2/tests/test_tokenizer.py` & `moltx-0.9.3/tests/test_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,10 +70,8 @@
     assert tok._tokens == tok2._tokens
     assert tok._token_idx == tok2._token_idx
 
     stok = tkz.MoltxTokenizer(token_size=2)
     assert stok._token_size == 2
     assert len(stok._tokens) == 2
     tokens = stok('BrCl')
-    assert tokens[0] == 1
-
-    #TODO add test for from_jsonfile
+    assert tokens[0] == 1 # <unk>
```

