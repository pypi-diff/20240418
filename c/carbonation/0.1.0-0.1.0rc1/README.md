# Comparing `tmp/carbonation-0.1.0.tar.gz` & `tmp/carbonation-0.1.0rc1.tar.gz`

## Comparing `carbonation-0.1.0.tar` & `carbonation-0.1.0rc1.tar`

### file list

```diff
@@ -1,38 +1,26 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/__about__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/utils.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/measurand/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/measurand/__main__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/reframe/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/cli/reframe/__main__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/__init__.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/component.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/euc.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/generic.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/interp.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/measurand.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/parameter.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/sampling.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 carbonation-0.1.0/src/carbonation/measurand/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/cli/test_measurand.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/cli/test_reframe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/cases.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/conftest.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/strategies.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_component.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_euc.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_interp.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_measurand.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_parameter.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 carbonation-0.1.0/tests/measurand/test_utils.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 carbonation-0.1.0/.gitignore
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 carbonation-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 carbonation-0.1.0/README.md
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 carbonation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 carbonation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/_version.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/__init__.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/component.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/euc.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/generic.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/interp.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/measurand.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/parameter.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/sampling.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/src/carbonation/measurand/utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/__init__.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/cases.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/conftest.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/strategies.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_component.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_euc.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_interp.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_measurand.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_parameter.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/tests/measurand/test_utils.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 carbonation-0.1.0rc1/PKG-INFO
```

### Comparing `carbonation-0.1.0/src/carbonation/measurand/component.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel, Field
 
 from carbonation.measurand.utils import (
     _bit_range_to_mask_and_shift,
     _range_to_tuple,
     _reverse_bits_ndarray,
     _reverse_bits_paarray,
-    size_to_uint,
+    _size_to_uint,
 )
 
 _RE_COMPONENT = re.compile(
     r"^\[?(?P<W>\d+(?:-\d+)?)(?:\:(?P<B>\d+(?:-\d+)?))?(?P<R>R)?\]?$", re.IGNORECASE
 )
 
 
@@ -78,15 +78,15 @@
     def size(self) -> int:
         if self.mask:
             return f"{self.mask:b}".count("1")
         return self.word_size
 
     @cached_property
     def input_dtype(self) -> np.dtype:
-        return size_to_uint(self.word_size)
+        return _size_to_uint(self.word_size)
 
     def __eq__(self, other: "Component") -> bool:
         return all(
             [
                 self.word == other.word,
                 self.mask == other.mask,
                 self.shift == other.shift,
```

### Comparing `carbonation-0.1.0/src/carbonation/measurand/euc.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/euc.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/src/carbonation/measurand/generic.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/generic.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/src/carbonation/measurand/interp.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/interp.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/src/carbonation/measurand/measurand.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/measurand.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,45 +26,47 @@
         return make_measurand(spec)
 
     def build(self, data: DataArray) -> DataArray:
         if isinstance(data, np.ndarray):
             return self._build_ndarray(data)
         if isinstance(data, pa.Table):
             return self._build_paarray(data)
-        msg = f"data must be np.ndarray or pa.Table, but is {type(data)}"
-        raise TypeError(msg)
+        raise TypeError
 
     def _build_ndarray(self, data: np.ndarray) -> np.ndarray:
         tmp = self.parameter._build_ndarray(data)
 
         if self.interp:
+            print("interp ndarray")
             tmp = self.interp.apply_ndarray(tmp, self.parameter.size)
 
         if self.euc:
             tmp = self.euc.apply_ndarray(tmp, self.parameter.size)
 
         return tmp
 
     def _build_paarray(self, data: pa.Table) -> pa.Array:
         tmp = self.parameter._build_paarray(data)
 
         if self.interp:
+            print("interp paarray")
             tmp = self.interp.apply_paarray(tmp, self.parameter.size)
 
         if self.euc:
             tmp = self.euc.apply_paarray(tmp, self.parameter.size)
 
         return tmp
 
 
 def make_measurand(spec: str, word_size: int = 8, one_based: bool = True) -> Measurand:
     parts = spec.split(";")
     parameter = make_parameter(parts[0], word_size=word_size, one_based=one_based)
     mapping = {"parameter": parameter}
 
+    print(parts)
     if len(parts) >= 2:
         mapping["interp"] = make_interp(parts[1])
 
     if len(parts) >= 3:
         mapping["euc"] = make_euc(parts[2])
 
     return Measurand(**mapping)
```

### Comparing `carbonation-0.1.0/src/carbonation/measurand/parameter.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pyarrow as pa
 import pyarrow.compute as pac
 from pydantic import BaseModel, Field
 
 from carbonation.measurand.component import Component, make_component
-from carbonation.measurand.utils import _expand_component_range, size_to_uint
+from carbonation.measurand.utils import _expand_component_range, _size_to_uint
 
 DataArray = Union[np.ndarray, pa.Table]
 
 
 class Parameter(BaseModel):
     components: Tuple[Component, ...]
     one_based: bool = Field(default=True, frozen=True)
@@ -27,30 +27,30 @@
 
     @cached_property
     def size(self) -> int:
         return sum([c.size for c in self.components])
 
     @cached_property
     def output_dtype(self) -> str:
-        return size_to_uint(self.size)
+        return _size_to_uint(self.size)
 
     @classmethod
     def from_spec(cls, spec: str, word_size=word_size) -> "Parameter":
         return make_parameter(spec, word_size=word_size)
 
     def build(self, data: DataArray) -> DataArray:
         if isinstance(data, np.ndarray):
             return self._build_ndarray(data)
         if isinstance(data, pa.Table):
             return self._build_paarray(data)
         raise TypeError
 
     def _build_ndarray(self, data: np.ndarray) -> np.ndarray:
         tmp = np.atleast_2d(data)
-        dtype = size_to_uint(self.size)
+        dtype = _size_to_uint(self.size)
         result = np.zeros(tmp.shape[0], dtype=dtype)
         size = 0
         for comp in reversed(self.components):
             result += comp._build_ndarray(tmp).astype(dtype) << size
             size += comp.size
         return result
```

### Comparing `carbonation-0.1.0/src/carbonation/measurand/utils.py` & `carbonation-0.1.0rc1/src/carbonation/measurand/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pyarrow as pa
 import pyarrow.compute as pac
 from numpy.typing import DTypeLike
 
 
-def size_to_uint(size: int) -> DTypeLike:
+def _size_to_uint(size: int) -> DTypeLike:
     if size <= 8:
         return "uint8"
     elif size <= 16:
         return "uint16"
     elif size <= 32:
         return "uint32"
     elif size <= 64:
@@ -34,30 +34,24 @@
             return list(range(a, b + 1))
         else:
             return list(reversed(range(b, a + 1)))
     else:
         return list([int(list_spec)])
 
 
-_RE_RAWPARAM_RANGE = re.compile(
-    r"^(?P<range>\d+-\d+)(?P<bits>[^;]*)(?P<etc>.*)$", re.IGNORECASE
-)
+_RE_RAWPARAM_RANGE = re.compile(r"^(?P<range>\d+-\d+)(?P<rest>.*)$", re.IGNORECASE)
 
 
 def _expand_component_range(spec: str) -> str:
     component_range = _RE_RAWPARAM_RANGE.match(spec)
     if component_range:
         word_range = component_range.group("range")
-        additional = component_range.group("bits")
-        etc = component_range.group("etc")
-        print(word_range, additional, etc)
-        print(f"range = {word_range!r}, add = {additional!r}, etc = {etc!r}")
+        additional = component_range.group("rest")
         words = _expand_list(word_range)
         spec = "+".join([f"{word}{additional}" for word in words])
-        spec = f"{spec}{etc}"
     return spec
 
 
 def _bit_range_to_mask_and_shift(lsb: int, msb: int) -> int:
     if msb < lsb:
         lsb, msb = msb, lsb
     shift = lsb
@@ -79,15 +73,15 @@
     return result
 
 
 ONE = np.uint8(1)
 
 
 def _reverse_bits_paarray(arr: pa.Array, size: int) -> pa.Array:
-    dtype = size_to_uint(size)
+    dtype = _size_to_uint(size)
     if isinstance(arr, pa.ChunkedArray):
         result = pa.chunked_array(
             [np.zeros(len(chunk), dtype=dtype) for chunk in arr.chunks]
         )
     else:
         result = pa.array(np.zeros(len(arr), dtype=dtype))
```

### Comparing `carbonation-0.1.0/tests/measurand/cases.py` & `carbonation-0.1.0rc1/tests/measurand/cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,14 @@
     Example("1-3", 0b0000000001_0000000010_0000000011, word_size=10, size=30),
 ] + component_test_cases
 
 measurand_test_cases = (
     [
         Example("1;2c", result=1, word_size=8, size=8),
         Example("255;2c", result=-1, word_size=8, size=8),
-        Example("1-4;u", 0x01020304, word_size=8, size=32),
-        Example("1-3;u", 0b0000000001_0000000010_0000000011, word_size=10, size=30),
         # MIL-STD-1750A32
         Example("127+255+255+127;1750a32", result=0.9999998 * 2**127),
         # (0x7FFFFF7F, 0.9999998 * 2**127),
         Example("64+256+256+127;1750a32", result=0.5 * 2**127),
         # (0x4000007F, 0.5 * 2**127),
         Example("80+256+256+4;1750a32", result=0.625 * 2**4),
         # (0x50000004, 0.625 * 2**4),
```

### Comparing `carbonation-0.1.0/tests/measurand/conftest.py` & `carbonation-0.1.0rc1/tests/measurand/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import pyarrow as pa
-from carbonation.measurand.utils import size_to_uint
+
+from carbonation.measurand.utils import _size_to_uint
 
 ARRAY_SIZE = 100
 
 
 def _make_sample_data(word_size: int) -> np.ndarray:
-    dtype = size_to_uint(word_size)
+    dtype = _size_to_uint(word_size)
     stop = 2**word_size + 1
     one = np.arange(start=1, stop=stop, dtype=np.uint16)
     one = np.fmod(one, np.uint16(2**word_size))
     return np.repeat(np.atleast_2d(one), ARRAY_SIZE, axis=0).astype(dtype)
 
 
 SAMPLE_NDARRAY = {word_size: _make_sample_data(word_size) for word_size in [8, 10, 12]}
```

### Comparing `carbonation-0.1.0/tests/measurand/strategies.py` & `carbonation-0.1.0rc1/tests/measurand/strategies.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/tests/measurand/test_component.py` & `carbonation-0.1.0rc1/tests/measurand/test_component.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/tests/measurand/test_euc.py` & `carbonation-0.1.0rc1/tests/measurand/test_euc.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/tests/measurand/test_interp.py` & `carbonation-0.1.0rc1/tests/measurand/test_interp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import numpy as np
 import pyarrow as pa
 import pytest
+from hypothesis import assume, given
+from hypothesis import strategies as st
+
 from carbonation.measurand.interp import (
     IEEE16,
     IEEE32,
     IEEE64,
     TI32,
     TI40,
     Interp,
     InvalidInterpSize,
     MilStd1750A32,
     MilStd1750A48,
     OnesComplement,
     TwosComplement,
     Unsigned,
 )
-from carbonation.measurand.utils import size_to_uint
-from hypothesis import assume, given
-from hypothesis import strategies as st
+from carbonation.measurand.utils import _size_to_uint
 
 from . import strategies as cst
 from .conftest import ARRAY_SIZE
 
 
 @given(cst.uint_and_size())
 def test_unsigned(things):
     uint, size = things
-    dtype = size_to_uint(size)
+    dtype = _size_to_uint(size)
     data = np.array([uint] * 10, dtype=dtype)
     result = Unsigned().apply_ndarray(data, size)
     assert list(result) == [uint] * 10
 
 
 @given(cst.uint_and_size())
 def test_onescomp(things):
     uint, size = things
-    dtype = size_to_uint(size)
+    dtype = _size_to_uint(size)
     data = np.array([uint] * 10, dtype=dtype)
     result = OnesComplement().apply_ndarray(data, size)
     assert result.shape[0] == 10
 
 
 @given(cst.uint_and_size())
 def test_twoscomp(things):
     uint, size = things
-    dtype = size_to_uint(size)
+    dtype = _size_to_uint(size)
     data = np.array([uint] * 10, dtype=dtype)
     result = TwosComplement().apply_ndarray(data, size)
     assert result.shape[0] == 10
 
 
 @given(cst.uint(16))
 def test_ieee16(uint):
```

### Comparing `carbonation-0.1.0/tests/measurand/test_measurand.py` & `carbonation-0.1.0rc1/tests/measurand/test_measurand.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/tests/measurand/test_parameter.py` & `carbonation-0.1.0rc1/tests/measurand/test_parameter.py`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/tests/measurand/test_utils.py` & `carbonation-0.1.0rc1/tests/measurand/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import numpy as np
 import pyarrow as pa
 import pytest
+from hypothesis import assume, given
+from hypothesis import strategies as st
+
 from carbonation.measurand.utils import (
     _bit_range_to_mask_and_shift,
     _expand_component_range,
     _expand_list,
     _range_to_tuple,
     _reverse_bits_ndarray,
     _reverse_bits_paarray,
-    size_to_uint,
+    _size_to_uint,
 )
-from hypothesis import assume, given
-from hypothesis import strategies as st
 
 from .conftest import ARRAY_SIZE
 
 
 @pytest.mark.parametrize(
     "spec,result",
     [
         ("1-4", "1+2+3+4"),
         ("4-1", "4+3+2+1"),
-        ("1-4;u", "1+2+3+4;u"),
-        ("1-4;ieee32", "1+2+3+4;ieee32"),
         ("1-2R", "1R+2R"),
         ("1-4:2-9", "1:2-9+2:2-9+3:2-9+4:2-9"),
     ],
 )
 def test_expand_component_range(spec, result):
     assert _expand_component_range(spec) == result
 
@@ -122,23 +121,23 @@
 )
 def test_bit_spec_to_mask_and_rshift_exception(a, b):
     with pytest.raises(TypeError):
         _bit_range_to_mask_and_shift(a, b)
 
 
 @given(st.integers(min_value=1, max_value=64))
-def testsize_to_uint(size):
-    dtype = np.dtype(size_to_uint(size))
+def test_size_to_uint(size):
+    dtype = np.dtype(_size_to_uint(size))
     assert size / (dtype.itemsize * 8) <= 1.0
 
 
 @given(st.integers(min_value=65, max_value=128))
-def testsize_to_uint_too_big(size):
+def test_size_to_uint_too_big(size):
     with pytest.raises(ValueError):
-        size_to_uint(size)
+        _size_to_uint(size)
 
 
 @pytest.mark.parametrize(
     "input, output, dtype, word_size",
     [
         (0x00, 0x00, "u1", 8),
         (0x0F, 0xF0, "u1", 8),
```

### Comparing `carbonation-0.1.0/LICENSE.txt` & `carbonation-0.1.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/README.md` & `carbonation-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `carbonation-0.1.0/pyproject.toml` & `carbonation-0.1.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,34 +28,27 @@
   "typeconvert==0.2",
   "numpy<1.26,>=1.19 ",
   "numba>=0.57",
   "pyarrow>=7.0.0",
   "pydantic>=2.0",
 ]
 
-[project.optional-dependencies]
-cli = ["python-dateutil"]
-
-[project.scripts]
-meas = "carbonation.cli.measurand:main"
-reframe = "carbonation.cli.reframe:main"
-
 [project.urls]
-Documentation = "https://github.com/jolsten/carbonation#readme"
-Issues = "https://github.com/jolsten/carbonation/issues"
-Source = "https://github.com/jolsten/carbonation"
+Documentation = "https://github.com/unknown/carbonation#readme"
+Issues = "https://github.com/unknown/carbonation/issues"
+Source = "https://github.com/unknown/carbonation"
 
 [tool.hatch.version]
 source = "vcs"
 
 [template.plugins.default]
 src-layout = true
 
 [tool.hatch.build.hooks.vcs]
-version-file = "src/carbonation/__about__.py"
+version-file = "src/carbonation/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
   "hypothesis",
 ]
```

### Comparing `carbonation-0.1.0/PKG-INFO` & `carbonation-0.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: carbonation
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: You can't have fizz without carbonation
-Project-URL: Documentation, https://github.com/jolsten/carbonation#readme
-Project-URL: Issues, https://github.com/jolsten/carbonation/issues
-Project-URL: Source, https://github.com/jolsten/carbonation
+Project-URL: Documentation, https://github.com/unknown/carbonation#readme
+Project-URL: Issues, https://github.com/unknown/carbonation/issues
+Project-URL: Source, https://github.com/unknown/carbonation
 Author-email: Jonathan Olsten <jonathan.olsten@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,16 +19,14 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: numba>=0.57
 Requires-Dist: numpy<1.26,>=1.19
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pydantic>=2.0
 Requires-Dist: typeconvert==0.2
-Provides-Extra: cli
-Requires-Dist: python-dateutil; extra == 'cli'
 Description-Content-Type: text/markdown
 
 # Carbonation
 
 [![PyPI - Version](https://img.shields.io/pypi/v/carbonation.svg)](https://pypi.org/project/carbonation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/carbonation.svg)](https://pypi.org/project/carbonation)
```

