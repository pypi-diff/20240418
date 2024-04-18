# Comparing `tmp/pyord-0.2.0.tar.gz` & `tmp/pyord-0.3.0.tar.gz`

## Comparing `pyord-0.2.0.tar` & `pyord-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 pyord-0.2.0/Cargo.toml
--rw-r--r--   0      501       20     2146 2024-03-12 09:08:22.000000 pyord-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-03-05 22:52:56.000000 pyord-0.2.0/.gitignore
--rw-r--r--   0      501       20        0 2024-04-02 08:34:30.000000 pyord-0.2.0/.gitmodules
--rw-r--r--   0      501       20      127 2024-03-11 12:27:12.000000 pyord-0.2.0/Dockerfile.build
--rw-r--r--   0      501       20     1487 2024-04-02 22:59:40.000000 pyord-0.2.0/Makefile
--rw-r--r--   0      501       20      632 2024-04-02 11:56:30.000000 pyord-0.2.0/README.md
--rw-r--r--   0      501       20    14777 2024-04-02 22:43:40.000000 pyord-0.2.0/generate_stubs.py
--rw-r--r--   0      501       20      834 2024-03-07 21:49:31.000000 pyord-0.2.0/ord.patch
--rw-r--r--   0      501       20     6121 2024-04-02 22:52:33.000000 pyord-0.2.0/pyord.pyi
--rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.2.0/python_tests/__init__.py
--rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.2.0/python_tests/runes/__init__.py
--rw-r--r--   0      501       20     1122 2024-04-02 18:14:57.000000 pyord-0.2.0/python_tests/runes/test_rune.py
--rw-r--r--   0      501       20      559 2024-04-02 18:18:31.000000 pyord-0.2.0/python_tests/runes/test_rune_id.py
--rw-r--r--   0      501       20     3343 2024-04-02 18:31:46.000000 pyord-0.2.0/python_tests/runes/test_runestone.py
--rw-r--r--   0      501       20     1982 2024-04-02 22:51:16.000000 pyord-0.2.0/src/cenotaph.rs
--rw-r--r--   0      501       20      992 2024-04-02 12:37:18.000000 pyord-0.2.0/src/edict.rs
--rw-r--r--   0      501       20     2353 2024-04-02 21:56:32.000000 pyord-0.2.0/src/etching.rs
--rw-r--r--   0      501       20     1210 2024-04-02 17:53:41.000000 pyord-0.2.0/src/flaw.rs
--rw-r--r--   0      501       20      640 2024-04-02 22:52:22.000000 pyord-0.2.0/src/lib.rs
--rw-r--r--   0      501       20      969 2024-04-02 14:49:08.000000 pyord-0.2.0/src/rune.rs
--rw-r--r--   0      501       20     1622 2024-04-02 22:50:42.000000 pyord-0.2.0/src/rune_id.rs
--rw-r--r--   0      501       20     3378 2024-04-02 21:56:45.000000 pyord-0.2.0/src/runestone.rs
--rw-r--r--   0      501       20     2075 2024-04-02 22:51:11.000000 pyord-0.2.0/src/terms.rs
--rw-r--r--   0      501       20     1633 2024-03-07 23:29:04.000000 pyord-0.2.0/src/utils.rs
--rw-r--r--   0      501       20    23809 2024-04-02 08:33:48.000000 pyord-0.2.0/Cargo.lock
--rw-r--r--   0      501       20      579 2024-03-07 22:24:02.000000 pyord-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pyord-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 pyord-0.3.0/Cargo.toml
+-rw-r--r--   0        0        0     2146 2024-03-12 09:08:22.000000 pyord-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      686 2024-03-05 22:52:56.000000 pyord-0.3.0/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-02 08:34:30.000000 pyord-0.3.0/.gitmodules
+-rw-r--r--   0        0        0      127 2024-03-11 12:27:12.000000 pyord-0.3.0/Dockerfile.build
+-rw-r--r--   0        0        0     1489 2024-04-02 23:20:46.000000 pyord-0.3.0/Makefile
+-rw-r--r--   0        0        0      632 2024-04-02 11:56:30.000000 pyord-0.3.0/README.md
+-rw-r--r--   0        0        0    14777 2024-04-02 22:43:40.000000 pyord-0.3.0/generate_stubs.py
+-rw-r--r--   0        0        0      834 2024-03-07 21:49:31.000000 pyord-0.3.0/ord.patch
+-rw-r--r--   0        0        0     6183 2024-04-18 16:35:22.000000 pyord-0.3.0/pyord.pyi
+-rw-r--r--   0        0        0        0 2024-03-07 19:16:59.000000 pyord-0.3.0/python_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 19:16:59.000000 pyord-0.3.0/python_tests/runes/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-02 18:14:57.000000 pyord-0.3.0/python_tests/runes/test_rune.py
+-rw-r--r--   0        0        0      559 2024-04-02 18:18:31.000000 pyord-0.3.0/python_tests/runes/test_rune_id.py
+-rw-r--r--   0        0        0     3290 2024-04-18 16:35:22.000000 pyord-0.3.0/python_tests/runes/test_runestone.py
+-rw-r--r--   0        0        0     1872 2024-04-18 16:35:22.000000 pyord-0.3.0/src/cenotaph.rs
+-rw-r--r--   0        0        0      992 2024-04-02 12:37:18.000000 pyord-0.3.0/src/edict.rs
+-rw-r--r--   0        0        0     2628 2024-04-18 16:35:22.000000 pyord-0.3.0/src/etching.rs
+-rw-r--r--   0        0        0     1402 2024-04-18 16:35:22.000000 pyord-0.3.0/src/flaw.rs
+-rw-r--r--   0        0        0      640 2024-04-02 22:52:22.000000 pyord-0.3.0/src/lib.rs
+-rw-r--r--   0        0        0      969 2024-04-02 14:49:08.000000 pyord-0.3.0/src/rune.rs
+-rw-r--r--   0        0        0     1622 2024-04-02 22:50:42.000000 pyord-0.3.0/src/rune_id.rs
+-rw-r--r--   0        0        0     3378 2024-04-02 21:56:45.000000 pyord-0.3.0/src/runestone.rs
+-rw-r--r--   0        0        0     2075 2024-04-02 22:51:11.000000 pyord-0.3.0/src/terms.rs
+-rw-r--r--   0        0        0     1633 2024-03-07 23:29:04.000000 pyord-0.3.0/src/utils.rs
+-rw-r--r--   0        0        0    23809 2024-04-18 16:37:59.000000 pyord-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      579 2024-03-07 22:24:02.000000 pyord-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pyord-0.3.0/PKG-INFO
```

### Comparing `pyord-0.2.0/.github/workflows/CI.yml` & `pyord-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/.gitignore` & `pyord-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/Makefile` & `pyord-0.3.0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 
 .PHONY: publish-linux-wheels
 publish-linux-wheels: build-builder-docker-image
 	docker run --rm -it -v $(shell pwd):/io $(shell docker build -q -f Dockerfile.build .) publish
 
 .PHONY: build-builder-docker-image
 build-builder-docker-image:
-	# This is redundant, but building this takes such a long time that it's nice to get some output
-	# from the process, which doesn't happen when it's built with the -q flag
+	@# This is redundant, but building this takes such a long time that it's nice to get some output
+	@# from the process, which doesn't happen when it's built with the -q flag
 	docker build -f Dockerfile.build .
```

### Comparing `pyord-0.2.0/README.md` & `pyord-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/generate_stubs.py` & `pyord-0.3.0/generate_stubs.py`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/ord.patch` & `pyord-0.3.0/ord.patch`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/pyord.pyi` & `pyord-0.3.0/pyord.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing
 
 @typing.final
 class Cenotaph:
     """Cenotaph"""
     etching: typing.Optional[Rune]
-    flaws: list[Flaw]
+    flaw: typing.Optional[Flaw]
     is_cenotaph: bool
     mint: typing.Optional[RuneId]
 
-    def __init__(self, /, flaws: list[Flaw], etching: typing.Optional[Rune]=None, mint: typing.Optional[RuneId]=None) -> None:
+    def __init__(self, /, etching: typing.Optional[Rune]=None, flaw: typing.Optional[Flaw]=None, mint: typing.Optional[RuneId]=None) -> None:
         """Cenotaph"""
 
     def __eq__(self, value: typing.Any, /) -> bool:
         """Return self==value."""
 
     def __ge__(self, value: typing.Any, /) -> bool:
         """Return self>=value."""
@@ -47,25 +47,25 @@
 class Etching:
     divisibility: typing.Optional[int]
     premine: typing.Optional[int]
     rune: typing.Optional[Rune]
     spacers: int
     symbol: typing.Optional[str]
     terms: typing.Optional[Terms]
+    turbo: bool
 
-    def __init__(self, /, divisibility: typing.Optional[int]=None, premine: typing.Optional[int]=None, rune: typing.Optional[Rune]=None, spacers: typing.Optional[int]=None, symbol: typing.Optional[str]=None, terms: typing.Optional[Terms]=None) -> None:...
+    def __init__(self, /, divisibility: typing.Optional[int]=None, premine: typing.Optional[int]=None, rune: typing.Optional[Rune]=None, spacers: typing.Optional[int]=None, symbol: typing.Optional[str]=None, terms: typing.Optional[Terms]=None, turbo: typing.Optional[bool]=None) -> None:...
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
 class Flaw:
     """A Flaw in a Runestone that makes it a Cenotaph
 :param n: Flaw as integer"""
-    flag: int
     reason: str
 
     def __init__(self, /, n: int) -> None:
         """A Flaw in a Runestone that makes it a Cenotaph
 :param n: Flaw as integer"""
 
     @staticmethod
```

### Comparing `pyord-0.2.0/python_tests/runes/test_rune.py` & `pyord-0.3.0/python_tests/runes/test_rune.py`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/python_tests/runes/test_rune_id.py` & `pyord-0.3.0/python_tests/runes/test_rune_id.py`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/python_tests/runes/test_runestone.py` & `pyord-0.3.0/python_tests/runes/test_runestone.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,9 @@
             )
         ],
     )
     tx_hex = tx.serialize().hex()
     runestone_or_cenotaph = Runestone.decipher_hex(tx_hex)
     assert isinstance(runestone_or_cenotaph, Cenotaph)
     assert runestone_or_cenotaph.is_cenotaph
-    assert len(runestone_or_cenotaph.flaws) == 1
-    assert runestone_or_cenotaph.flaws[0].reason == "edict output greater than transaction output count"
+    assert runestone_or_cenotaph.flaw.reason == "edict output greater than transaction output count"
     assert runestone != runestone_or_cenotaph
```

### Comparing `pyord-0.2.0/src/cenotaph.rs` & `pyord-0.3.0/src/cenotaph.rs`

 * *Files 18% similar despite different names*

```diff
@@ -3,65 +3,62 @@
 use ordinals::Cenotaph;
 
 use super::flaw::PyFlaw;
 use super::rune::PyRune;
 use super::rune_id::PyRuneId;
 
 /// Cenotaph
-/// :type flaws: list[Flaw]
 /// :type etching: typing.Optional[Rune]
+/// :type flaw: typing.Optional[Flaw]
 /// :type mint: typing.Optional[RuneId]
 #[pyclass(name="Cenotaph")]
 #[derive(Debug, PartialEq)]
 pub struct PyCenotaph(pub Cenotaph);
 
 
 #[pymethods]
 impl PyCenotaph {
     #[new]
-    #[pyo3(signature = (flaws, etching=None, mint=None))]
+    #[pyo3(signature = (etching=None, flaw=None, mint=None))]
     pub fn new(
-        flaws: Vec<PyFlaw>,
         etching: Option<PyRune>,
+        flaw: Option<PyFlaw>,
         mint: Option<PyRuneId>,
     ) -> Self {
-        let flaw_bitmask = flaws.iter().fold(0, |acc, f| acc | f.0.flag());
         Self(Cenotaph {
             etching: etching.map(|e| e.0),
-            flaws: flaw_bitmask,
+            flaw: flaw.map(|e| e.0),
             mint: mint.map(|m| m.0),
         })
     }
 
     pub fn __eq__(&self, other: &PyCenotaph) -> bool {
         self.0 == other.0
     }
 
     /// :rtype: str
     pub fn __repr__(&self) -> String {
         format!(
             "Cenotaph(flaws={}, etching={}, mint={})",
-            self.flaws()
-                .iter()
+            self.flaw()
                 .map(|f| f.__repr__())
-                .collect::<Vec<String>>()
-                .join(", "),
+                .unwrap_or_else(|| "None".to_string()),
             self.etching()
                 .map(|e| e.__repr__())
                 .unwrap_or_else(|| "None".to_string()),
             self.mint()
                 .map(|m| m.__repr__())
                 .unwrap_or_else(|| "None".to_string())
         )
     }
 
-    /// :rtype: list[Flaw]
+    /// :rtype: typing.Optional[Flaw]
     #[getter]
-    pub fn flaws(&self) -> Vec<PyFlaw> {
-        self.0.flaws().iter().map(|flaw| PyFlaw(*flaw)).collect()
+    pub fn flaw(&self) -> Option<PyFlaw> {
+        self.0.flaw.map(|f| PyFlaw(f))
     }
 
     /// :rtype: typing.Optional[Rune]
     #[getter]
     pub fn etching(&self) -> Option<PyRune> {
         self.0.etching.map(|e| PyRune(e))
     }
```

### Comparing `pyord-0.2.0/src/edict.rs` & `pyord-0.3.0/src/edict.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/etching.rs` & `pyord-0.3.0/src/etching.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,48 +6,52 @@
 
 /// :type divisibility: typing.Optional[int]
 /// :type premine: typing.Optional[int]
 /// :type rune: typing.Optional[Rune]
 /// :type spacers: typing.Optional[int]
 /// :type symbol: typing.Optional[str]
 /// :type terms: typing.Optional[Terms]
+/// :type turbo: typing.Optional[bool]
 #[pyclass(name="Etching")]
 #[derive(Debug, PartialEq, Copy, Clone)]
 pub struct PyEtching(pub Etching);
 
 #[pymethods]
 impl PyEtching {
     #[new]
     pub fn new(
         divisibility: Option<u8>,
         premine: Option<u128>,
         rune: Option<PyRune>,
         spacers: Option<u32>,
         symbol: Option<char>,
         terms: Option<PyTerms>,
+        turbo: Option<bool>,
     ) -> Self {
         Self(Etching {
             divisibility,
             premine,
             rune: rune.map(|r| r.0),
             spacers,
             symbol,
             terms: terms.map(|m| m.0),
+            turbo: turbo.unwrap_or(false),
         })
     }
 
     pub fn __repr__(&self) -> String {
         format!(
-            "Etching(divisibility={}, premine={}, rune={}, spacers={}, symbol={}, terms={})",
+            "Etching(divisibility={}, premine={}, rune={}, spacers={}, symbol={}, terms={}, turbo={})",
             self.divisibility().map(|i| i.to_string()).unwrap_or("None".to_string()),
             self.premine().map(|i| i.to_string()).unwrap_or("None".to_string()),
             self.rune().map(|r| r.__repr__()).unwrap_or("None".to_string()),
             self.spacers().map(|i| i.to_string()).unwrap_or("None".to_string()),
             self.symbol().map(|s| format!("'{}'", s.to_string())).unwrap_or("None".to_string()),
             self.terms().map(|m| m.__repr__()).unwrap_or("None".to_string()),
+            if self.turbo() { "True" } else { "False" },
         )
     }
 
     /// :rtype: typing.Optional[int]
     #[getter]
     pub fn divisibility(&self) -> Option<u8> {
         self.0.divisibility
@@ -78,8 +82,14 @@
     }
 
     /// :rtype: typing.Optional[Terms]
     #[getter]
     pub fn terms(&self) -> Option<PyTerms> {
         self.0.terms.map(|m| PyTerms(m))
     }
+
+    /// :rtype: bool
+    #[getter]
+    pub fn turbo(&self) -> bool {
+        self.0.turbo
+    }
 }
```

### Comparing `pyord-0.2.0/src/flaw.rs` & `pyord-0.3.0/src/flaw.rs`

 * *Files 21% similar despite different names*

```diff
@@ -7,51 +7,59 @@
 /// A Flaw in a Runestone that makes it a Cenotaph
 /// :param n: Flaw as integer
 /// :type n: int
 #[pyclass(name="Flaw")]
 #[derive(Debug, PartialEq, Copy, Clone)]
 pub struct PyFlaw(pub Flaw);
 
+const ALL_FLAWS: [Flaw; 10] = [
+    Flaw::EdictOutput,
+    Flaw::EdictRuneId,
+    Flaw::InvalidScript,
+    Flaw::Opcode,
+    Flaw::SupplyOverflow,
+    Flaw::TrailingIntegers,
+    Flaw::TruncatedField,
+    Flaw::UnrecognizedEvenTag,
+    Flaw::UnrecognizedFlag,
+    Flaw::Varint,
+];
+
+
 #[pymethods]
 impl PyFlaw {
     #[new]
     pub fn new(
         n: u32,
     ) -> PyResult<Self> {
-        for flaw in Flaw::ALL.into_iter() {
+        for flaw in ALL_FLAWS.into_iter() {
             if flaw as u32 == n {
                 return Ok(Self(flaw));
             }
         }
         Err(PyValueError::new_err(format!("Invalid flaw number: {}", n)))
     }
 
     /// :rtype: list[Flaw]
     #[staticmethod]
     pub fn all() -> Vec<Self> {
-        Flaw::ALL.into_iter().map(|flaw| Self(flaw)).collect()
+        ALL_FLAWS.into_iter().map(|flaw| Self(flaw)).collect()
     }
 
     pub fn __eq__(&self, other: &PyFlaw) -> bool {
         self.0 == other.0
     }
 
     pub fn __repr__(&self) -> String {
-        format!("Flaw(n={}, reason='{}')", self.__int__(), self.reason())
+        format!("Flaw(value={}, reason='{}')", self.__int__(), self.reason())
     }
 
     pub fn __int__(&self) -> u32 {
         self.0 as u32
     }
 
-    /// :rtype: int
-    #[getter]
-    pub fn flag(&self) -> u32 {
-        self.0.flag()
-    }
-
     /// :rtype: str
     #[getter]
     pub fn reason(&self) -> String {
         self.0.to_string()
     }
 }
```

### Comparing `pyord-0.2.0/src/lib.rs` & `pyord-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/rune.rs` & `pyord-0.3.0/src/rune.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/rune_id.rs` & `pyord-0.3.0/src/rune_id.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/runestone.rs` & `pyord-0.3.0/src/runestone.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/terms.rs` & `pyord-0.3.0/src/terms.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/src/utils.rs` & `pyord-0.3.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/Cargo.lock` & `pyord-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -334,17 +334,17 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ordinals"
-version = "0.0.6"
+version = "0.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f0677a8fb620f4c7bef9c0cc85c5e9809dccade9ef25bf1b96d9a78ef18472a"
+checksum = "f69dc8f090e996b63e1f96972f0d619f497c9545464c7bddf65e42d38576b3f3"
 dependencies = [
  "bitcoin",
  "derive_more",
  "serde",
  "serde_with",
  "thiserror",
 ]
@@ -454,15 +454,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.52",
 ]
 
 [[package]]
 name = "pyord"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "bitcoin",
  "hex",
  "ordinals",
  "pyo3",
 ]
```

### Comparing `pyord-0.2.0/pyproject.toml` & `pyord-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyord-0.2.0/PKG-INFO` & `pyord-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyord
-Version: 0.2.0
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: python-bitcointx ; extra == 'dev'
 Requires-Dist: ipython ; extra == 'dev'
 Requires-Dist: ipdb ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
```

