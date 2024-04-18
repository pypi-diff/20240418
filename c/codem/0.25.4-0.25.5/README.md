# Comparing `tmp/codem-0.25.4.tar.gz` & `tmp/codem-0.25.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codem-0.25.4.tar", last modified: Fri Nov  3 16:47:24 2023, max compression
+gzip compressed data, was "codem-0.25.5.tar", last modified: Thu Apr 18 20:14:46 2024, max compression
```

## Comparing `codem-0.25.4.tar` & `codem-0.25.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.960774 codem-0.25.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-03 16:47:10.000000 codem-0.25.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-11-03 16:47:24.960774 codem-0.25.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2023-11-03 16:47:11.000000 codem-0.25.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-11-03 16:47:11.000000 codem-0.25.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 16:47:24.960774 codem-0.25.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.952774 codem-0.25.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.952774 codem-0.25.4/src/codem/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/codem/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/lib/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/lib/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/lib/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/codem/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33253 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/codem/registration/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17924 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/registration/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)    25131 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/registration/dsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18195 2023-11-03 16:47:11.000000 codem-0.25.4/src/codem/registration/icp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/codem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-03 16:47:24.000000 codem-0.25.4/src/codem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/vcd/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.956774 codem-0.25.4/src/vcd/meshing/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/meshing/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.960774 codem-0.25.4/src/vcd/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2023-11-03 16:47:11.000000 codem-0.25.4/src/vcd/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:47:24.960774 codem-0.25.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2023-11-03 16:47:11.000000 codem-0.25.4/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.943987 codem-0.25.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 20:14:34.000000 codem-0.25.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-18 20:14:46.939988 codem-0.25.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-18 20:14:35.000000 codem-0.25.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-18 20:14:35.000000 codem-0.25.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:14:46.943987 codem-0.25.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.935988 codem-0.25.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.935988 codem-0.25.5/src/codem/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/codem/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/lib/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/lib/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/lib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22108 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/codem/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33335 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/codem/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/registration/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25131 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/registration/dsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-04-18 20:14:35.000000 codem-0.25.5/src/codem/registration/icp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/codem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 20:14:46.000000 codem-0.25.5/src/codem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/vcd/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/vcd/meshing/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/meshing/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/src/vcd/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-18 20:14:35.000000 codem-0.25.5/src/vcd/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:14:46.939988 codem-0.25.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-18 20:14:35.000000 codem-0.25.5/tests/test_registration.py
```

### Comparing `codem-0.25.4/LICENSE` & `codem-0.25.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/PKG-INFO` & `codem-0.25.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.4
+Version: 0.25.5
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.4/pyproject.toml` & `codem-0.25.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 [project.scripts]
 codem = "codem.main:main"
 vcd = "vcd.main:main"
 
 [tool.black]
 line-length = 88
-target-version = ['py37']
+target-version = ['py39']
 include = '\.py(i|t)?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
```

### Comparing `codem-0.25.4/readme.md` & `codem-0.25.5/readme.md`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/codem/lib/log.py` & `codem-0.25.5/src/codem/lib/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 try:
     import websocket
     from pythonjsonlogger import jsonlogger
 except ImportError:
     pass
 else:
-
     class CustomJsonFormatter(jsonlogger.JsonFormatter):
         def add_fields(
             self,
             log_record: Dict[str, Any],
             record: logging.LogRecord,
             message_dict: Dict[str, Any],
         ) -> None:
@@ -35,28 +34,29 @@
             else:
                 log_record["level"] = record.levelname
 
             if log_record.get("type") is None:
                 log_record["type"] = "log_message"
             return None
 
-    class WebSocketHandler(logging.Handler):
-        def __init__(self, level: str, websocket: "websocket.WebSocket") -> None:
-            super().__init__(level)
-            self.ws = websocket
-            # TODO: check if websocket is already connected?
-
-        def emit(self, record: logging.LogRecord) -> None:
-            msg = self.format(record)
-            _ = self.ws.send(msg)
-            return None
 
-        def close(self) -> None:
-            self.ws.close()
-            return super().close()
+class WebSocketHandler(logging.Handler):
+    def __init__(self, level: str, websocket: "websocket.WebSocket") -> None:
+        super().__init__(level)
+        self.ws = websocket
+        # TODO: check if websocket is already connected?
+
+    def emit(self, record: logging.LogRecord) -> None:
+        msg = self.format(record)
+        _ = self.ws.send(msg)
+        return None
+
+    def close(self) -> None:
+        self.ws.close()
+        return super().close()
 
 
 class Log:
     def __init__(self, config: Dict[str, Any]):
         """
         Creates logging formatting and structure
```

### Comparing `codem-0.25.4/src/codem/lib/progress.py` & `codem-0.25.5/src/codem/lib/progress.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/codem/main.py` & `codem-0.25.5/src/codem/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import dataclasses
 import math
 import os
 import time
 import warnings
 from contextlib import ContextDecorator
 from typing import Any
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import yaml
 from codem import __version__
 from codem.lib.log import Log
@@ -70,14 +69,20 @@
     DSM_WEAK_FILTER: float = 1.0
     ICP_ANGLE_THRESHOLD: float = 0.001
     ICP_DISTANCE_THRESHOLD: float = 0.001
     ICP_MAX_ITER: int = 100
     ICP_RMSE_THRESHOLD: float = 0.0001
     ICP_ROBUST: bool = True
     ICP_SOLVE_SCALE: bool = True
+    OFFSET_X: str= 'auto'
+    OFFSET_Y: str = 'auto'
+    OFFSET_Z: str = 'auto'
+    SCALE_X: str = "0.01"
+    SCALE_Y: str = "0.01"
+    SCALE_Z: str = "0.01"
     VERBOSE: bool = False
     ICP_SAVE_RESIDUALS: bool = False
     OUTPUT_DIR: Optional[str] = None
     TIGHT_SEARCH: bool = False
     LOG_TYPE: str = "rich"
     WEBSOCKET_URL: str = "127.0.0.1:8889"
 
@@ -133,14 +138,33 @@
             raise ValueError(
                 "Maximum number of ICP iterations must be a positive integer."
             )
         if self.ICP_RMSE_THRESHOLD <= 0:
             raise ValueError(
                 "ICP minimum change in RMSE convergence threshold must be greater than 0."
             )
+        for offset in [self.OFFSET_X, self.OFFSET_Y, self.OFFSET_Z]:
+            if (
+                offset != "auto"
+                and not offset.isnumeric()
+            ):
+                raise ValueError(
+                    "Offset values need to be set to 'auto' or an integer"
+                )
+        for scale in [self.SCALE_X, self.SCALE_Y, self.SCALE_Z]:
+            if (
+                isinstance(scale, str)
+                and scale != "auto"
+            ):
+                try:
+                    float(scale)
+                except ValueError as e:
+                    raise ValueError(
+                        "Offset values need to be set to 'auto' or an float"
+                    ) from e
 
         # dump config
         config_path = os.path.join(self.OUTPUT_DIR, "config.yml")
         with open(config_path, "w") as f:
             yaml.safe_dump(
                 dataclasses.asdict(self),
                 f,
@@ -269,14 +293,77 @@
     )
     ap.add_argument(
         "--icp-save-residuals",
         action="store_true",
         help="Write ICP residual information",
     )
     ap.add_argument(
+        "--offset-x",
+        type=str,
+        default='auto',
+        help=(
+            "Offset to be subtracted from the X nominal value, before "
+            "the value is scaled. The special value auto can be specified, which causes "
+            "the writer to set the offset to the minimum value of the dimension. "
+        )
+    )
+    ap.add_argument(
+        "--offset-y",
+        type=str,
+        default='auto',
+        help=(
+            "Offset to be subtracted from the Y nominal value, before "
+            "the value is scaled. The special value auto can be specified, which causes "
+            "the writer to set the offset to the minimum value of the dimension. "
+        )
+    )
+    ap.add_argument(
+        "--offset-z",
+        type=str,
+        default='auto',
+        help=(
+            "Offset to be subtracted from the Z nominal value, before "
+            "the value is scaled. The special value auto can be specified, which causes "
+            "the writer to set the offset to the minimum value of the dimension. "
+        )
+    )
+    ap.add_argument(
+        "--scale-x",
+        type=str,
+        default='.01',
+        help=(
+            "Scale to be divided from the X nominal value, "
+            "after the offset has been applied. The special value auto can be specified, "
+            "which causes the writer to select a scale to set the stored values of the "
+            "dimensions to range from [0, 2147483647]."
+        )
+    )
+    ap.add_argument(
+        "--scale-y",
+        type=str,
+        default='.01',
+        help=(
+            "Scale to be divided from the Y nominal value, "
+            "after the offset has been applied. The special value auto can be specified, "
+            "which causes the writer to select a scale to set the stored values of the "
+            "dimensions to range from [0, 2147483647]."
+        )
+    )
+    ap.add_argument(
+        "--scale-z",
+        type=str,
+        default='.01',
+        help=(
+            "Scale to be divided from the Z nominal value, "
+            "after the offset has been applied. The special value auto can be specified, "
+            "which causes the writer to select a scale to set the stored values of the "
+            "dimensions to range from [0, 2147483647]."
+        )
+    )   
+    ap.add_argument(
         "--verbose", "-v", action="store_true", help="turn on verbose logging"
     )
     ap.add_argument(
         "--tight-search",
         "-ts",
         action="store_true",
         help=(
@@ -323,14 +410,20 @@
         DSM_WEAK_FILTER=float(args.dsm_weak_filter),
         ICP_ANGLE_THRESHOLD=float(args.icp_angle_threshold),
         ICP_DISTANCE_THRESHOLD=float(args.icp_distance_threshold),
         ICP_MAX_ITER=int(args.icp_max_iter),
         ICP_RMSE_THRESHOLD=float(args.icp_rmse_threshold),
         ICP_ROBUST=args.icp_robust,
         ICP_SOLVE_SCALE=args.icp_solve_scale,
+        SCALE_X=args.scale_x,
+        SCALE_Y=args.scale_y,
+        SCALE_Z=args.scale_z,
+        OFFSET_X=args.offset_x,
+        OFFSET_Y=args.offset_y,
+        OFFSET_Z=args.offset_z,
         VERBOSE=args.verbose,
         ICP_SAVE_RESIDUALS=args.icp_save_residuals,
         TIGHT_SEARCH=args.tight_search,
         OUTPUT_DIR=args.output_dir,
         LOG_TYPE=args.log_type,
         WEBSOCKET_URL=args.websocket_url
     )
```

### Comparing `codem-0.25.4/src/codem/preprocessing/preprocess.py` & `codem-0.25.5/src/codem/preprocessing/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 * instantiate - method for auto-instantiating the appropriate class
 """
 import json
 import logging
 import math
 import os
 import tempfile
-from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import codem.lib.resources as r
 import cv2
 import numpy as np
@@ -66,14 +65,20 @@
     DSM_WEAK_FILTER: float
     ICP_ANGLE_THRESHOLD: float
     ICP_DISTANCE_THRESHOLD: float
     ICP_MAX_ITER: int
     ICP_RMSE_THRESHOLD: float
     ICP_ROBUST: bool
     ICP_SOLVE_SCALE: bool
+    OFFSET_X: str
+    OFFSET_Y: str
+    OFFSET_Z: str
+    SCALE_X: str
+    SCALE_Y: str
+    SCALE_Z: str
     VERBOSE: bool
     ICP_SAVE_RESIDUALS: bool
     OUTPUT_DIR: str
     TIGHT_SEARCH: bool
     LOG_TYPE: str
     WEBSOCKET_URL: str
     log: Log
```

### Comparing `codem-0.25.4/src/codem/registration/apply.py` & `codem-0.25.5/src/codem/registration/apply.py`

 * *Files 6% similar despite different names*

```diff
@@ -338,14 +338,21 @@
         """
         pipeline = pdal.Reader(self.aoi_file)
         pipeline |= self.get_registration_transformation()
 
         writer_kwargs = {"filename": self.out_name}
         if self.fnd_crs is not None:
             writer_kwargs["a_srs"] = self.fnd_crs.to_wkt()
+        writer_kwargs["forward"] = "all"
+        writer_kwargs["offset_x"] = self.config["OFFSET_X"]
+        writer_kwargs["offset_y"] = self.config["OFFSET_Y"]
+        writer_kwargs['offset_z'] = self.config["OFFSET_Z"]
+        writer_kwargs["scale_x"] = self.config["SCALE_X"]
+        writer_kwargs["scale_y"] = self.config["SCALE_Y"]
+        writer_kwargs['scale_z'] = self.config["SCALE_Z"]
         pipeline |= pdal.Writer.las(**writer_kwargs)
 
         pipeline.execute()
         self.logger.info(
             f"Registration has been applied to AOI-PCLOUD and saved to: {self.out_name}"
         )
```

### Comparing `codem-0.25.4/src/codem/registration/dsm.py` & `codem-0.25.5/src/codem/registration/dsm.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/codem/registration/icp.py` & `codem-0.25.5/src/codem/registration/icp.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/codem.egg-info/PKG-INFO` & `codem-0.25.5/src/codem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.4
+Version: 0.25.5
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.4/src/codem.egg-info/SOURCES.txt` & `codem-0.25.5/src/codem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/vcd/main.py` & `codem-0.25.5/src/vcd/main.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/vcd/meshing/mesh.py` & `codem-0.25.5/src/vcd/meshing/mesh.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/src/vcd/preprocessing/preprocess.py` & `codem-0.25.5/src/vcd/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.4/tests/test_registration.py` & `codem-0.25.5/tests/test_registration.py`

 * *Files identical despite different names*

