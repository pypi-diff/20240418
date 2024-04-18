# Comparing `tmp/flightdata-0.2.5.tar.gz` & `tmp/flightdata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightdata-0.2.5.tar", last modified: Wed Mar 20 17:18:52 2024, max compression
+gzip compressed data, was "flightdata-0.2.6.tar", last modified: Thu Apr 18 12:02:58 2024, max compression
```

## Comparing `flightdata-0.2.5.tar` & `flightdata-0.2.6.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.005312 flightdata-0.2.5/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:19.000000 flightdata-0.2.5/LICENSE
--rw-r--r--   0 td6834    (1001) td6834    (1001)     5603 2024-03-20 17:18:52.005312 flightdata-0.2.5/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5252 2023-12-19 08:55:40.000000 flightdata-0.2.5/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      211 2024-01-25 10:44:54.000000 flightdata-0.2.5/flightdata/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata/base/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      121 2024-01-27 20:38:52.000000 flightdata-0.2.5/flightdata/base/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3464 2024-01-27 20:38:52.000000 flightdata-0.2.5/flightdata/base/collection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2281 2023-12-19 08:55:40.000000 flightdata-0.2.5/flightdata/base/constructs.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      397 2023-12-19 08:55:40.000000 flightdata-0.2.5/flightdata/base/numpy_encoder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    15955 2024-03-16 11:52:09.000000 flightdata-0.2.5/flightdata/base/table.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      743 2024-01-16 15:43:56.000000 flightdata-0.2.5/flightdata/coefficients.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata/environment/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-12-19 08:55:40.000000 flightdata-0.2.5/flightdata/environment/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1898 2024-01-27 20:38:52.000000 flightdata-0.2.5/flightdata/environment/environment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4259 2023-12-19 08:55:40.000000 flightdata-0.2.5/flightdata/environment/wind.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata/flight/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       69 2023-12-19 08:55:40.000000 flightdata-0.2.5/flightdata/flight/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      510 2024-02-26 08:11:32.000000 flightdata-0.2.5/flightdata/flight/ardupilot.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4691 2024-02-26 08:11:32.000000 flightdata-0.2.5/flightdata/flight/fields.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    18981 2024-02-26 08:11:32.000000 flightdata-0.2.5/flightdata/flight/flight.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1457 2024-02-26 08:11:32.000000 flightdata-0.2.5/flightdata/flow.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata/model/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      258 2024-01-16 15:43:56.000000 flightdata-0.2.5/flightdata/model/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      810 2024-01-27 20:38:52.000000 flightdata-0.2.5/flightdata/model/aerodynamic.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      185 2024-01-16 15:43:56.000000 flightdata-0.2.5/flightdata/model/thrust.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4501 2024-01-25 15:52:52.000000 flightdata-0.2.5/flightdata/origin.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    21516 2024-03-16 11:52:09.000000 flightdata-0.2.5/flightdata/state.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.001312 flightdata-0.2.5/flightdata.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)     5603 2024-03-20 17:18:51.000000 flightdata-0.2.5/flightdata.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      830 2024-03-20 17:18:51.000000 flightdata-0.2.5/flightdata.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-03-20 17:18:51.000000 flightdata-0.2.5/flightdata.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       26 2024-03-20 17:18:51.000000 flightdata-0.2.5/flightdata.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       11 2024-03-20 17:18:51.000000 flightdata-0.2.5/flightdata.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      389 2024-03-20 17:18:52.005312 flightdata-0.2.5/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      672 2023-03-28 15:54:19.000000 flightdata-0.2.5/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:18:52.005312 flightdata-0.2.5/test/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      379 2023-12-19 08:55:40.000000 flightdata-0.2.5/test/test_fields.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2791 2024-02-26 08:11:32.000000 flightdata-0.2.5/test/test_flight.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      846 2023-12-19 08:55:40.000000 flightdata-0.2.5/test/test_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-18 12:02:27.000000 flightdata-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-18 12:02:58.916330 flightdata-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 12:02:27.000000 flightdata-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.908330 flightdata-0.2.6/flightdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15997 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/coefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/flight/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/ardupilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/aerodynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/thrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21516 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/flightdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-18 12:02:27.000000 flightdata-0.2.6/scripts/collect_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 12:02:27.000000 flightdata-0.2.6/scripts/flightline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 12:02:58.916330 flightdata-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 12:02:27.000000 flightdata-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_origin.py
```

### Comparing `flightdata-0.2.5/LICENSE` & `flightdata-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/base/collection.py` & `flightdata-0.2.6/flightdata/base/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Dict, List, Union, Any, Self, TypeVar, Iterable
-import numpy as np
+from typing import Union, Any, Self, TypeVar, Iterable
 import pandas as pd
 
 
 T = TypeVar('T')
 
 class Collection:
     VType: T = None
@@ -41,15 +40,15 @@
             return self.data[getattr(key, self.__class__.uid)]
         raise ValueError(f"Invalid Key or Indexer {key}")
 
     def __iter__(self) -> Iterable[T]:
         for v in self.data.values():
             yield v
 
-    def to_list(self) -> List[T]:
+    def to_list(self) -> list[T]:
         return list(self.data.values())
     
     def to_dicts(self, *args, **kwargs) -> list[dict[str, Any]]:
         return [v.to_dict(*args, **kwargs) for v in self.data.values()]
 
     def to_dict(self, *args, **kwargs) -> dict[str, dict[str, Any]]:
         return {k: v.to_dict(*args, **kwargs) for k, v in self.data.items()}
@@ -95,8 +94,12 @@
     def __str__(self) -> str:
         return str(pd.Series({k: str(v) for k, v in self.data.items()}))
     
     def __repr__(self) -> str:
         return str(pd.Series({k: repr(v) for k, v in self.data.items()}))
     
     def __len__(self) -> int:
-        return len(self.data)
+        return len(self.data)
+    
+    @property
+    def uids(self) -> list[str]:
+        return list(self.data.keys())
```

### Comparing `flightdata-0.2.5/flightdata/base/constructs.py` & `flightdata-0.2.6/flightdata/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/base/table.py` & `flightdata-0.2.6/flightdata/base/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import numpy as np
 import pandas as pd
 import numpy.typing as npt
 from geometry import Base, Time
-from typing import Union, Self, Tuple
+from typing import Self, Tuple
 from .constructs import SVar, Constructs
 from numbers import Number
 from time import time
 
 
 def make_time(tab):
     return Time.from_t(tab.t)
@@ -18,15 +18,15 @@
         SVar("time", Time,        ["t", "dt"]               , make_time )
     ])
 
     def __init__(self, data: pd.DataFrame, fill=True, min_len=1):
         if len(data) < min_len:
             raise Exception(f"State constructor length check failed, data length = {len(data)}, min_len = {min_len}")
         self.base_cols = [c for c in data.columns if c in self.constructs.cols()]
-        self.label_cols = [c for c in data.columns if not c in self.constructs.cols()]
+        self.label_cols = [c for c in data.columns if c not in self.constructs.cols()]
     
         self.data = data
 
         self.data.index = self.data.index - self.data.index[0]
         
         if fill:
             missing = self.constructs.missing(self.data.columns)
@@ -41,15 +41,15 @@
             bcs = self.constructs.cols()
         else:
             bcs = self.base_cols
         if np.any(np.isnan(self.data.loc[:,bcs])):
             raise ValueError("nan values in data")
         
 
-    def __getattr__(self, name: str) -> Union[pd.DataFrame, Base]:
+    def __getattr__(self, name: str) -> npt.NDArray | Base:
         if name in self.data.columns:
             return self.data[name].to_numpy()
         elif name in self.constructs.data.keys():
             con = self.constructs.data[name]
             return con.obj(self.data.loc[:, con.keys])
         else:
             raise AttributeError(f"Unknown column or construct {name}")
@@ -69,15 +69,15 @@
 
     def __len__(self):
         return len(self.data)
     
     @property
     def duration(self):
         return self.data.index[-1] - self.data.index[0]
-
+    
     def __getitem__(self, sli):
         if isinstance(sli, Number):
             if sli<0:
                 return self.__class__(self.data.iloc[[int(sli)], :])
 
             return self.__class__(
                 self.data.iloc[self.data.index.get_indexer([sli], method="nearest"), :]
@@ -196,17 +196,18 @@
     def get_label_len(self, **kwargs) -> int:
         try:
             return len(self.get_subset_df(**kwargs))
         except Exception:
             return 0
 
     def unique_labels(self, cols = None) -> pd.DataFrame:
-        '''TODO Fix This'''
         if cols is None:
             cols = self.label_cols
+        elif isinstance(cols, str):
+            cols = [cols]
         return self.data.loc[:, cols].reset_index(drop=True).drop_duplicates().reset_index(drop=True)
 
     def shift_labels(self, col, elname, offset, allow_label_loss=True) -> Self:
         """Move the end of a label forwards or backwards by offset seconds.
         TODO this should be part of shift_label. current implementation doesn't allow
         min label length, and only allows indexing by element"""
         new_t = self.label_ts("element")[elname][1] +  offset
@@ -250,15 +251,15 @@
             if offset < 0:
                 labels.iloc[ranges.iloc[i].end+offset:ranges.iloc[i].end+1, labcols] = ranges.iloc[i+1].loc[kwargs.keys()]
         return self.label(**labels.to_dict(orient='list'))
     
     @classmethod
     def shift_multi(Cls, steps: int, tb1: Self, tb2: Self, min_len=2) -> Tuple(Self, Self):
         '''Take datapoints off the start of tb2 and add to the end tb1'''
-        if (steps>0 and len(tb2)-min_len<steps) or (steps<0 and len(tb1)-2<min_len):
+        if (steps>0 and len(tb2)-min_len<steps) or (steps<0 and min_len - len(tb1) > steps):
             raise ValueError(f'Cannot Squash a Table to less than {min_len} datapoints')
         dfj = Cls.stack([tb1, tb2], overlap=0).data
         return Cls(dfj.iloc[:len(tb1)+steps, :]), \
                Cls(dfj.iloc[len(tb1)+steps:, :])
     
     def shift_label_ratio(self, ratio: float, min_len=None, **kwargs) -> Self:
         '''shift a label within its allowable bounds, with a ratio of
@@ -276,15 +277,15 @@
     def shift_labels_ratios(self, ratios: list[float], min_len: int) -> Self:
         assert len(ratios) == len(self.unique_labels())-1
         res = self
         for lab, ratio in zip([r[1] for r in self.unique_labels()[:-1].iterrows()], ratios):
             res = res.shift_label_ratio(ratio, min_len, **lab)
         return res
     
-    def get_label_id(self, **kwargs) -> Union[int, float]:
+    def get_label_id(self, **kwargs) -> int | float:
         dfo = self.unique_labels()
         for k, v in kwargs.items():
             dfo = dfo.loc[dfo[k] == v, :]            
         return dfo.index[0]
     
     def label_range(self, t=False, **kwargs) -> tuple[int]:
         '''Get the first and last index of a label. 
@@ -313,15 +314,15 @@
     def label_lens(self) -> dict[str, int]:
         return {k: len(v) for k, v in self.split_labels().items()}
 
     def extract_single_label(self, lab) -> Self:
         labs = np.array(self.single_labels())
         return self.__class__(self.data[labs == lab])
 
-    def split_labels(self, cols=None) -> dict[str, Self]:
+    def split_labels(self, cols:list[str]|str = None) -> dict[str, Self]:
         '''Split into multiple tables based on the labels'''
         res = {}
         for label in self.unique_labels(cols).iterrows():
             ld = label[1].to_dict()
             res['_'.join(ld.values())] = self.get_label_subset(**ld)
         return res
```

### Comparing `flightdata-0.2.5/flightdata/coefficients.py` & `flightdata-0.2.6/flightdata/coefficients.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/environment/environment.py` & `flightdata-0.2.6/flightdata/environment/environment.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/environment/wind.py` & `flightdata-0.2.6/flightdata/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/flight/fields.py` & `flightdata-0.2.6/flightdata/flight/fields.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/flight/flight.py` & `flightdata-0.2.6/flightdata/flight/flight.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,15 @@
     def to_json(self, file: str) -> str:
         with open(file, 'w') as f:
             dump(self.to_dict(), f, cls=NumpyEncoder, indent=2)
         return file
 
     @staticmethod
     def from_json(file: str) -> Self:
-        with open(file, 'r') as f:
-            return Flight.from_dict(load(f))
+        return Flight.from_dict(load(open(file, 'r')))
 
     @staticmethod
     def build_cols(**kwargs):
         df = pd.DataFrame(columns=list(fields.data.keys()))
         for k, v in kwargs.items():
             df[k] = v
         return df.dropna(axis=1, how='all')
```

### Comparing `flightdata-0.2.5/flightdata/flow.py` & `flightdata-0.2.6/flightdata/flow.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/model/aerodynamic.py` & `flightdata-0.2.6/flightdata/model/aerodynamic.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata/origin.py` & `flightdata-0.2.6/flightdata/origin.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,52 +87,51 @@
         direction = centre - pilot
         return Origin(
             name,
             pilot,
             np.arctan2(direction.y[0], direction.x[0])
         )
 
-    def to_f3a_zone(self):
+    def to_f3a_zone(self, file: str):
         
         centre = self.pilot_position.offset(
             100 * g.Point(np.cos(self.heading), np.sin(self.heading), 0.0)
         )
 
-        oformat = lambda val: "{}".format(val)
-
-        return "\n".join([
-            "Emailed box data for F3A Zone Pro - please DON'T modify!",
-            self.name,
-            oformat(self.pilot_position.lat[0]),
-            oformat(self.pilot_position.long[0]),
-            oformat(centre.lat[0]),
-            oformat(centre.long[0]),
-            "120"
-        ])
-
-
+        with open(file, 'w') as f:
+            for line in [
+                "Emailed box data for F3A Zone Pro - please DON'T modify!",
+                self.name,
+                self.pilot_position.lat[0],
+                self.pilot_position.long[0],
+                centre.lat[0],
+                centre.long[0],
+                self.pilot_position.alt[0]
+            ]:
+                print(line, file=f)
+                
     @staticmethod
     def from_f3a_zone(file_path: str):
         if hasattr(file_path, "read"):
             lines = file_path.read().splitlines()
         else:
             with open(file_path, "r") as f:
                 lines = f.read().splitlines()
         return Origin.from_points(
             lines[1],
-            g.GPS(float(lines[2]), float(lines[3]), 0),
-            g.GPS(float(lines[4]), float(lines[5]), 0)
+            g.GPS(float(lines[2]), float(lines[3]), float(lines[6])),
+            g.GPS(float(lines[4]), float(lines[5]), float(lines[6]))
         )
 
     @staticmethod
     def from_fcjson_parmameters(data: dict):
         return Origin.from_points(
             "FCJ_box",
-            g.GPS(float(data['pilotLat']), float(data['pilotLng']), 0),
-            g.GPS(float(data['centerLat']), float(data['centerLng']), 0)
+            g.GPS(float(data['pilotLat']), float(data['pilotLng']), float(data['pilotAlt'])),
+            g.GPS(float(data['centerLat']), float(data['centerLng']), float(data['centerAlt']))
         )
 
 
     def gps_to_point(self, gps: g.GPS) -> g.Point:
         pned = gps - self.pilot_position
         return self.rotation.transform_point(g.Point(pned.y, pned.x, -pned.z ))
```

### Comparing `flightdata-0.2.5/flightdata/state.py` & `flightdata-0.2.6/flightdata/state.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/flightdata.egg-info/SOURCES.txt` & `flightdata-0.2.6/flightdata.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,10 +23,12 @@
 flightdata/flight/__init__.py
 flightdata/flight/ardupilot.py
 flightdata/flight/fields.py
 flightdata/flight/flight.py
 flightdata/model/__init__.py
 flightdata/model/aerodynamic.py
 flightdata/model/thrust.py
+scripts/collect_logs.py
+scripts/flightline.py
 test/test_fields.py
 test/test_flight.py
 test/test_origin.py
```

### Comparing `flightdata-0.2.5/setup.py` & `flightdata-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/test/test_flight.py` & `flightdata-0.2.6/test/test_flight.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.5/test/test_origin.py` & `flightdata-0.2.6/test/test_origin.py`

 * *Files identical despite different names*

