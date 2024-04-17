# Comparing `tmp/foamlib-0.3.0.tar.gz` & `tmp/foamlib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.0.tar", last modified: Mon Apr 15 18:07:21 2024, max compression
+gzip compressed data, was "foamlib-0.3.1.tar", last modified: Wed Apr 17 23:03:10 2024, max compression
```

## Comparing `foamlib-0.3.0.tar` & `foamlib-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:07:21.424259 foamlib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-15 18:07:16.000000 foamlib-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-15 18:07:21.424259 foamlib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-15 18:07:16.000000 foamlib-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:07:21.420259 foamlib-0.3.0/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:07:21.424259 foamlib-0.3.0/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:07:16.000000 foamlib-0.3.0/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:07:21.424259 foamlib-0.3.0/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-15 18:07:21.000000 foamlib-0.3.0/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 18:07:21.000000 foamlib-0.3.0/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:07:21.000000 foamlib-0.3.0/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 18:07:21.000000 foamlib-0.3.0/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 18:07:21.000000 foamlib-0.3.0/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 18:07:16.000000 foamlib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:07:21.424259 foamlib-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:03:10.995256 foamlib-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-17 23:03:06.000000 foamlib-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-17 23:03:10.995256 foamlib-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-17 23:03:06.000000 foamlib-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:03:10.991256 foamlib-0.3.1/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:03:10.995256 foamlib-0.3.1/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:03:06.000000 foamlib-0.3.1/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:03:10.995256 foamlib-0.3.1/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-17 23:03:10.000000 foamlib-0.3.1/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 23:03:10.000000 foamlib-0.3.1/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:03:10.000000 foamlib-0.3.1/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 23:03:10.000000 foamlib-0.3.1/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 23:03:10.000000 foamlib-0.3.1/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-17 23:03:06.000000 foamlib-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:03:10.995256 foamlib-0.3.1/setup.cfg
```

### Comparing `foamlib-0.3.0/LICENSE.txt` & `foamlib-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/PKG-INFO` & `foamlib-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.0/README.md` & `foamlib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/foamlib/_cases.py` & `foamlib-0.3.1/foamlib/_cases.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/foamlib/_files/_base.py` & `foamlib-0.3.1/foamlib/_files/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import sys
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Dict, NamedTuple, Optional, Union
+from typing import Dict, NamedTuple, Optional, Tuple, Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping, Sequence
 else:
     from typing import Mapping, Sequence
 
 try:
     import numpy as np
-    from numpy.typing import NDArray
 except ModuleNotFoundError:
     pass
 
 
 class FoamDict:
     class DimensionSet(NamedTuple):
         mass: Union[int, float] = 0
@@ -55,8 +54,20 @@
     _Dict = Dict[str, Union["Data", "_Dict"]]
 
     @abstractmethod
     def as_dict(self) -> _Dict:
         """Return a nested dict representation of the dictionary."""
         raise NotImplementedError
 
-    _SetData = Union[Data, "NDArray[np.generic]"]
+    _SetData = Union[
+        str,
+        int,
+        float,
+        bool,
+        Dimensioned,
+        DimensionSet,
+        Sequence["_SetData"],
+        Mapping[str, "_SetData"],
+        "np.ndarray[Tuple[()], np.dtype[np.generic]]",
+        "np.ndarray[Tuple[int], np.dtype[np.generic]]",
+        "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
+    ]
```

### Comparing `foamlib-0.3.0/foamlib/_files/_fields.py` & `foamlib-0.3.1/foamlib/_files/_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 else:
     from typing import Sequence
 
 from ._files import FoamFile
 
 try:
     import numpy as np
-    from numpy.typing import NDArray
 except ModuleNotFoundError:
     pass
 
 
 class FoamFieldFile(FoamFile):
     """An OpenFOAM dictionary file representing a field as a mutable mapping."""
 
@@ -54,30 +53,34 @@
         @property
         def value(
             self,
         ) -> Union[
             int,
             float,
             Sequence[Union[int, float, Sequence[Union[int, float]]]],
-            "NDArray[np.generic]",
+            "np.ndarray[Tuple[()], np.dtype[np.generic]]",
+            "np.ndarray[Tuple[int], np.dtype[np.generic]]",
+            "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
         ]:
             """Alias of `self["value"]`."""
             ret = self["value"]
             if not isinstance(ret, (int, float, Sequence)):
                 raise TypeError("value is not a field")
             return cast(Union[int, float, Sequence[Union[int, float]]], ret)
 
         @value.setter
         def value(
             self,
             value: Union[
                 int,
                 float,
                 Sequence[Union[int, float, Sequence[Union[int, float]]]],
-                "NDArray[np.generic]",
+                "np.ndarray[Tuple[()], np.dtype[np.generic]]",
+                "np.ndarray[Tuple[int], np.dtype[np.generic]]",
+                "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
             ],
         ) -> None:
             self["value"] = value
 
         @value.deleter
         def value(self) -> None:
             del self["value"]
@@ -124,30 +127,34 @@
     @property
     def internal_field(
         self,
     ) -> Union[
         int,
         float,
         Sequence[Union[int, float, Sequence[Union[int, float]]]],
-        "NDArray[np.generic]",
+        "np.ndarray[Tuple[()], np.dtype[np.generic]]",
+        "np.ndarray[Tuple[int], np.dtype[np.generic]]",
+        "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
     ]:
         """Alias of `self["internalField"]`."""
         ret = self["internalField"]
         if not isinstance(ret, (int, float, Sequence)):
             raise TypeError("internalField is not a field")
         return cast(Union[int, float, Sequence[Union[int, float]]], ret)
 
     @internal_field.setter
     def internal_field(
         self,
         value: Union[
             int,
             float,
             Sequence[Union[int, float, Sequence[Union[int, float]]]],
-            "NDArray[np.generic]",
+            "np.ndarray[Tuple[()], np.dtype[np.generic]]",
+            "np.ndarray[Tuple[int], np.dtype[np.generic]]",
+            "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
         ],
     ) -> None:
         self["internalField"] = value
 
     @property
     def boundary_field(self) -> "FoamFieldFile.BoundariesSubDict":
         """Alias of `self["boundaryField"]`."""
```

### Comparing `foamlib-0.3.0/foamlib/_files/_files.py` & `foamlib-0.3.1/foamlib/_files/_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if sys.version_info >= (3, 9):
     from collections.abc import Iterator, Mapping, MutableMapping
 else:
     from typing import Iterator, Mapping, MutableMapping
 
 from ._base import FoamDict
 from ._io import FoamFileIO
-from ._serialization import serialize_keyword_entry
+from ._serialization import serialize
 
 
 class FoamFile(
     FoamDict,
     MutableMapping[
         Union[str, Tuple[str, ...]], Union["FoamFile.Data", "FoamFile.SubDict"]
     ],
@@ -130,24 +130,24 @@
             with self:
                 if isinstance(data, FoamDict):
                     data = data.as_dict()
 
                 start, end = parsed.entry_location(keywords, missing_ok=True)
 
                 self._write(
-                    f"{contents[:start]}\n{serialize_keyword_entry(keywords[-1], {})}\n{contents[end:]}"
+                    f"{contents[:start]}\n{serialize({keywords[-1]: {}})}\n{contents[end:]}"
                 )
 
                 for k, v in data.items():
                     self[(*keywords, k)] = v
         else:
             start, end = parsed.entry_location(keywords, missing_ok=True)
 
             self._write(
-                f"{contents[:start]}\n{serialize_keyword_entry(keywords[-1], data, assume_field=assume_field, assume_dimensions=assume_dimensions)}\n{contents[end:]}"
+                f"{contents[:start]}\n{serialize({keywords[-1]: data}, assume_field=assume_field, assume_dimensions=assume_dimensions)}\n{contents[end:]}"
             )
 
     def __setitem__(
         self,
         keywords: Union[str, Tuple[str, ...]],
         data: "FoamFile._SetData",
     ) -> None:
```

### Comparing `foamlib-0.3.0/foamlib/_files/_io.py` & `foamlib-0.3.1/foamlib/_files/_io.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/foamlib/_files/_parsing.py` & `foamlib-0.3.1/foamlib/_files/_parsing.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/foamlib/_util.py` & `foamlib-0.3.1/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.0/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.1/foamlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.0/pyproject.toml` & `foamlib-0.3.1/pyproject.toml`

 * *Files identical despite different names*

