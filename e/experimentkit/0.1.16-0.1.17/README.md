# Comparing `tmp/experimentkit-0.1.16.tar.gz` & `tmp/experimentkit-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimentkit-0.1.16.tar", max compression
+gzip compressed data, was "experimentkit-0.1.17.tar", max compression
```

## Comparing `experimentkit-0.1.16.tar` & `experimentkit-0.1.17.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1079 2024-02-20 20:15:42.917677 experimentkit-0.1.16/LICENSE
--rw-r--r--   0        0        0      818 2024-02-20 20:15:42.917677 experimentkit-0.1.16/README.md
--rw-r--r--   0        0        0       75 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/__init__.py
--rw-r--r--   0        0        0      122 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/_config.py
--rw-r--r--   0        0        0     2032 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/environment.py
--rw-r--r--   0        0        0       60 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/evaluation/__init__.py
--rw-r--r--   0        0        0     1523 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/evaluation/regression.py
--rw-r--r--   0        0        0     2024 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/funx.py
--rw-r--r--   0        0        0        0 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/generators/__init__.py
--rw-r--r--   0        0        0     3857 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/generators/time_series.py
--rw-r--r--   0        0        0     1223 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/logger_config.py
--rw-r--r--   0        0        0     4966 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/metricsreport.py
--rw-r--r--   0        0        0     1562 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/monitor.py
--rw-r--r--   0        0        0     1845 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/reporting.py
--rw-r--r--   0        0        0    10147 2024-02-20 20:15:42.917677 experimentkit-0.1.16/experimentkit/visualization.py
--rw-r--r--   0        0        0      700 2024-02-20 20:15:42.917677 experimentkit-0.1.16/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 experimentkit-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-18 21:51:30.080395 experimentkit-0.1.17/LICENSE
+-rw-r--r--   0        0        0      818 2024-04-18 21:51:30.080395 experimentkit-0.1.17/README.md
+-rw-r--r--   0        0        0       70 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/_config.py
+-rw-r--r--   0        0        0     2050 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/environment.py
+-rw-r--r--   0        0        0       60 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/evaluation/__init__.py
+-rw-r--r--   0        0        0     1524 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/evaluation/regression.py
+-rw-r--r--   0        0        0     2490 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/funx.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/generators/__init__.py
+-rw-r--r--   0        0        0     3857 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/generators/time_series.py
+-rw-r--r--   0        0        0     1223 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/logger_config.py
+-rw-r--r--   0        0        0     4997 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/metricsreport.py
+-rw-r--r--   0        0        0     1562 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/monitor.py
+-rw-r--r--   0        0        0     1845 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/reporting.py
+-rw-r--r--   0        0        0       56 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/study_setup/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/study_setup/project_structures.py
+-rw-r--r--   0        0        0     2490 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/study_setup/study_setup.py
+-rw-r--r--   0        0        0    10147 2024-04-18 21:51:30.084395 experimentkit-0.1.17/experimentkit/visualization.py
+-rw-r--r--   0        0        0      734 2024-04-18 21:51:30.084395 experimentkit-0.1.17/pyproject.toml
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 experimentkit-0.1.17/PKG-INFO
```

### Comparing `experimentkit-0.1.16/LICENSE` & `experimentkit-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `experimentkit-0.1.16/README.md` & `experimentkit-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `experimentkit-0.1.16/experimentkit/environment.py` & `experimentkit-0.1.17/experimentkit/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """ Environment and profiling functions
 """
 
+import json
+import logging
 import platform
 import re
-import uuid, json, psutil, logging
 import sys
 import timeit
+import uuid
 from typing import Iterable
 
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
+import psutil
 
 
 def getsizeof_in(var, targetUnit):
     """Get size of a variable in specific units of measurement."""
     from sys import getsizeof
 
     shifts_to = {
```

### Comparing `experimentkit-0.1.16/experimentkit/evaluation/regression.py` & `experimentkit-0.1.17/experimentkit/evaluation/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict
+
 import numpy as np
 from sklearn import metrics
 
 
 def regression_report(y_true: np.ndarray, y_pred: np.ndarray) -> Dict[str, float]:
     """Regression Report
```

### Comparing `experimentkit-0.1.16/experimentkit/funx.py` & `experimentkit-0.1.17/experimentkit/funx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-""" Utility functions 
+""" Utility functions
 
 """
 
-import matplotlib.pyplot as plt
-import numpy as np
 import os
 import pickle
 import time
+from typing import Dict, Optional
 
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
+import yaml
 
 
 def compare_sample_from_data(
     data: torch.Tensor, y_true: torch.Tensor, y_pred: torch.Tensor, n_samples: int = 3
 ) -> np.ndarray:
     sampled_idxs = torch.randint(len(data), (1, n_samples)).flatten()
 
@@ -54,18 +56,35 @@
     if os.path.getsize(fpath) == 0:
         print(f"The file '{fpath}' is empty")
     with open(fpath, "rb") as handle:
         f = pickle.load(handle)
     return f
 
 
-def generate_random_name(length: str = 22, with_timestamp: bool = True) -> str:
+def generate_random_name(length: int = 22, with_timestamp: bool = True) -> str:
     bank = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
     tstamp = str(time.time()).replace(".", "d") if with_timestamp else ""
     to_len = length - len(tstamp)
     if to_len < 0:
         raise Exception(
             "If you want generate a random name with time_stamp, "
             + f"length must be greater than 18"
         )
     rand_chars = "".join([bank[ci] for ci in np.random.choice(len(bank), to_len)])
     return f"{tstamp}-{rand_chars}"
+
+
+def load_yaml(fpath: str = "../params.yaml") -> Optional[Dict[str, object]]:
+    params = None
+    with open(fpath, "r") as stream:
+        try:
+            params = yaml.safe_load(stream)
+            print(params)
+        except yaml.YAMLError as e:
+            print(e)
+    return params
+
+
+def yaml_save_dict(fpath: str, d: dict) -> str:
+    with open(fpath, "w") as file:
+        yaml.dump(d, file)
+    return fpath
```

### Comparing `experimentkit-0.1.16/experimentkit/generators/time_series.py` & `experimentkit-0.1.17/experimentkit/generators/time_series.py`

 * *Files identical despite different names*

### Comparing `experimentkit-0.1.16/experimentkit/logger_config.py` & `experimentkit-0.1.17/experimentkit/logger_config.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pathlib import Path
 import logging.config
+from pathlib import Path
 
 
 def setup_logger(
     logger_name: str, log_level: str = "INFO", log_file: str or None = None
 ) -> logging.Logger:
     """
     Example
```

### Comparing `experimentkit-0.1.16/experimentkit/metricsreport.py` & `experimentkit-0.1.17/experimentkit/metricsreport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import copy
 from typing import List
 
-import torch
 import matplotlib.pyplot as plt
-import pandas as pd
 import numpy as np
+import pandas as pd
 import seaborn as sns
-from sklearn.metrics import accuracy_score, precision_score, f1_score, confusion_matrix
+import torch
+from sklearn.metrics import (accuracy_score, confusion_matrix, f1_score,
+                             precision_score)
 
 from .funx import *
 
 
 class MetricsReport:
     """
     Examples
```

### Comparing `experimentkit-0.1.16/experimentkit/monitor.py` & `experimentkit-0.1.17/experimentkit/monitor.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 
 """
 
-from IPython import get_ipython
 import matplotlib.pyplot as plt
+from IPython import get_ipython
 
 
 class Monitor:
     def __init__(
         self,
         x,
         y,
```

### Comparing `experimentkit-0.1.16/experimentkit/reporting.py` & `experimentkit-0.1.17/experimentkit/reporting.py`

 * *Files identical despite different names*

### Comparing `experimentkit-0.1.16/experimentkit/visualization.py` & `experimentkit-0.1.17/experimentkit/visualization.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Visualization utilities"""
 
 from typing import Dict, Iterable, List, Optional, Tuple
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import numpy as np
-import seaborn as sns
 import scienceplots
+import seaborn as sns
 
 
 def plot_n_examples(X: np.ndarray, n: int, cols: int = 2, labels: List[str] = None):
     """
 
     Arguments
     ---------
```

### Comparing `experimentkit-0.1.16/pyproject.toml` & `experimentkit-0.1.17/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "experimentkit"
-version = "0.1.16"
+version = "0.1.17"
 description = "A toolkit for easily running research experiments"
 authors = ["gianfa <gian.angelini@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "experimentkit"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -23,11 +23,13 @@
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest = "^7.2.2"
 pre-commit = "^3.6.1"
 black = "^24.2.0"
+mypy = "^1.8.0"
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `experimentkit-0.1.16/PKG-INFO` & `experimentkit-0.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimentkit
-Version: 0.1.16
+Version: 0.1.17
 Summary: A toolkit for easily running research experiments
 Author: gianfa
 Author-email: gian.angelini@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

