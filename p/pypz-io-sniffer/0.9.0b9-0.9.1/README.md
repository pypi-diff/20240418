# Comparing `tmp/pypz-io-sniffer-0.9.0b9.tar.gz` & `tmp/pypz_io_sniffer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypz-io-sniffer-0.9.0b9.tar", last modified: Tue Feb 13 09:32:40 2024, max compression
+gzip compressed data, was "pypz_io_sniffer-0.9.1.tar", last modified: Thu Apr 18 05:48:40 2024, max compression
```

## Comparing `pypz-io-sniffer-0.9.0b9.tar` & `pypz_io_sniffer-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:40.625316 pypz-io-sniffer-0.9.0b9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-13 09:32:40.625316 pypz-io-sniffer-0.9.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:32:40.625316 pypz-io-sniffer-0.9.0b9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:40.621316 pypz-io-sniffer-0.9.0b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:40.621316 pypz-io-sniffer-0.9.0b9/src/pypz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:40.621316 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-02-13 09:32:28.000000 pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:40.625316 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-13 09:32:40.000000 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-13 09:32:40.000000 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:32:40.000000 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-13 09:32:40.000000 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 09:32:40.000000 pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:40.658630 pypz_io_sniffer-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-18 05:48:40.658630 pypz_io_sniffer-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:48:40.658630 pypz_io_sniffer-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:40.654630 pypz_io_sniffer-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:40.654630 pypz_io_sniffer-0.9.1/src/pypz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:40.654630 pypz_io_sniffer-0.9.1/src/pypz/sniffer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-04-18 05:48:34.000000 pypz_io_sniffer-0.9.1/src/pypz/sniffer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:40.658630 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-18 05:48:40.000000 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 05:48:40.000000 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:48:40.000000 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 05:48:40.000000 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 05:48:40.000000 pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/top_level.txt
```

### Comparing `pypz-io-sniffer-0.9.0b9/LICENSE` & `pypz_io_sniffer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypz-io-sniffer-0.9.0b9/PKG-INFO` & `pypz_io_sniffer-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: pypz-io-sniffer
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: A small tool that is capable to sniff and visualize the control messages between Operators.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,sniffer
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the experimental implementation of the IO Sniffer.
 The Sniffer allows you to visualize the control plane of the IO ports of
 the operators, so you can have a better understanding, what happens during
 the execution of your pipeline.
```

### Comparing `pypz-io-sniffer-0.9.0b9/README.md` & `pypz_io_sniffer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/__main__.py` & `pypz_io_sniffer-0.9.1/src/pypz/sniffer/__main__.py`

 * *Files identical despite different names*

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/sniffer.py` & `pypz_io_sniffer-0.9.1/src/pypz/sniffer/sniffer.py`

 * *Files identical despite different names*

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/utils.py` & `pypz_io_sniffer-0.9.1/src/pypz/sniffer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
        [4] - {G}
 
     This information can then be used amongst more to draw the operators in the proper
     order and position to visualize their connections.
     Note that this method is capable to handle circular dependencies.
     """
 
-    paths = list()
+    paths: list = list()
     # Step 1)
     # Extracting the paths. Using the example in the docs, the expected result:
     # [0] - [A, C, D, F, G]
     # [1] - [A, C, E, G]
     # [2] - [B, C, E, G]
     # [3] - [B, C, D, F, G]
     # =========================================================================
@@ -111,15 +111,15 @@
     # Converting path into list of sets. Using the example in the docs, the expected result:
     # [0] -> {A, B}
     # [1] -> {C}
     # [2] -> {D, E}
     # [3] -> {F, G}
     # [4] -> {G}
     # =======================================================================================
-    dependency_levels = []
+    dependency_levels: list = []
     for path in cleaned_paths:
         for idx, node in enumerate(path):
             if idx == len(dependency_levels):
                 dependency_levels.append(set())
             dependency_levels[idx].add(node)
 
     # Step 4)
```

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/viewer.py` & `pypz_io_sniffer-0.9.1/src/pypz/sniffer/viewer.py`

 * *Files identical despite different names*

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz/sniffer/views.py` & `pypz_io_sniffer-0.9.1/src/pypz/sniffer/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import tkinter as tk
+from typing import Optional
 
 from pypz.abstracts.channel_ports import ChannelInputPort, ChannelOutputPort
 from pypz.core.channels.status import ChannelStatusMessage, ChannelStatus
 from pypz.core.specs.operator import Operator
 
 
 class ViewConfig:
@@ -52,37 +53,41 @@
         self.canvas = canvas
 
         self.channel_reader_idx = channel_reader_idx
         self.channel_writer_idx = channel_writer_idx
         self.channel_reader_views: list[ChannelRWView] = list()
         self.channel_writer_views: list[ChannelRWView] = list()
 
-        self.x1 = None
-        self.y1 = None
-        self.x2 = None
-        self.y2 = None
+        self.x1: Optional[int] = None
+        self.y1: Optional[int] = None
+        self.x2: Optional[int] = None
+        self.y2: Optional[int] = None
 
     def draw(self, next_available_y_position: int):
-        first_channel_reader = min(self.channel_reader_views, key=lambda cr: cr.top)
-        last_channel_reader = max(self.channel_reader_views, key=lambda cr: cr.top)
-        first_channel_writer = min(self.channel_writer_views, key=lambda cr: cr.top)
-        last_channel_writer = max(self.channel_writer_views, key=lambda cr: cr.top)
-
-        channel_reader_x_min = first_channel_reader.left
-        channel_reader_y_min = first_channel_reader.top + (first_channel_reader.bottom - first_channel_reader.top) / 2
-        channel_reader_y_max = last_channel_reader.top + (last_channel_reader.bottom - last_channel_reader.top) / 2
-
-        channel_writer_x_max = first_channel_writer.right
-        channel_writer_y_min = first_channel_writer.top + (first_channel_writer.bottom - first_channel_writer.top) / 2
-        channel_writer_y_max = last_channel_writer.top + (last_channel_writer.bottom - last_channel_writer.top) / 2
-
-        self.x1 = channel_reader_x_min - 50 - 20 * self.channel_reader_idx
-        self.y1 = channel_reader_y_min + (channel_reader_y_max - channel_reader_y_min) / 2
-        self.x2 = channel_writer_x_max + 50 + 20 * self.channel_writer_idx
-        self.y2 = channel_writer_y_min + (channel_writer_y_max - channel_writer_y_min) / 2
+        first_channel_reader: ChannelRWView = min(self.channel_reader_views, key=lambda cr: cr.top)
+        last_channel_reader: ChannelRWView = max(self.channel_reader_views, key=lambda cr: cr.top)
+        first_channel_writer: ChannelRWView = min(self.channel_writer_views, key=lambda cr: cr.top)
+        last_channel_writer: ChannelRWView = max(self.channel_writer_views, key=lambda cr: cr.top)
+
+        channel_reader_x_min: float = first_channel_reader.left
+        channel_reader_y_min: float = \
+            first_channel_reader.top + (first_channel_reader.bottom - first_channel_reader.top) / 2
+        channel_reader_y_max: float = \
+            last_channel_reader.top + (last_channel_reader.bottom - last_channel_reader.top) / 2
+
+        channel_writer_x_max: float = first_channel_writer.right
+        channel_writer_y_min: float = \
+            first_channel_writer.top + (first_channel_writer.bottom - first_channel_writer.top) / 2
+        channel_writer_y_max: float = \
+            last_channel_writer.top + (last_channel_writer.bottom - last_channel_writer.top) / 2
+
+        self.x1 = int(channel_reader_x_min - 50 - 20 * self.channel_reader_idx)
+        self.y1 = int(channel_reader_y_min + (channel_reader_y_max - channel_reader_y_min) / 2)
+        self.x2 = int(channel_writer_x_max + 50 + 20 * self.channel_writer_idx)
+        self.y2 = int(channel_writer_y_min + (channel_writer_y_max - channel_writer_y_min) / 2)
 
         for idx, channel_reader in enumerate(self.channel_reader_views):
             self.canvas.create_line(self.x1,
                                     channel_reader.top + (channel_reader.bottom - channel_reader.top) / 2,
                                     channel_reader_x_min - 5,
                                     channel_reader.top + (channel_reader.bottom - channel_reader.top) / 2,
                                     arrow=tk.LAST)
@@ -120,18 +125,18 @@
         self.canvas = canvas
 
         self.channel_box = None
         self.channel_text = None
         self.status_display_l = None
         self.status_display_r = None
 
-        self.left = None
-        self.top = None
-        self.right = None
-        self.bottom = None
+        self.left: Optional[int] = None
+        self.top: Optional[int] = None
+        self.right: Optional[int] = None
+        self.bottom: Optional[int] = None
 
         self.is_finished: bool = False
         self.is_error: bool = False
         self.last_status_message_timestamp: int = 0
 
     def on_update(self, status_message: ChannelStatusMessage):
         self.last_status_message_timestamp = status_message.timestamp
```

### Comparing `pypz-io-sniffer-0.9.0b9/src/pypz_io_sniffer.egg-info/PKG-INFO` & `pypz_io_sniffer-0.9.1/src/pypz_io_sniffer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: pypz-io-sniffer
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: A small tool that is capable to sniff and visualize the control messages between Operators.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,sniffer
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the experimental implementation of the IO Sniffer.
 The Sniffer allows you to visualize the control plane of the IO ports of
 the operators, so you can have a better understanding, what happens during
 the execution of your pipeline.
```

