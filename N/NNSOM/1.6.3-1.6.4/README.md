# Comparing `tmp/nnsom-1.6.3.tar.gz` & `tmp/nnsom-1.6.4.tar.gz`

## Comparing `nnsom-1.6.3.tar` & `nnsom-1.6.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nnsom-1.6.3/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77373 2020-02-02 00:00:00.000000 nnsom-1.6.3/src/NNSOM/plots.py
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.6.3/src/NNSOM/som.py
--rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.6.3/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.3/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.3/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/som.py
+-rw-r--r--   0        0        0    23705 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.4/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.4/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.4/PKG-INFO
```

### Comparing `nnsom-1.6.3/src/NNSOM/plots.py` & `nnsom-1.6.4/src/NNSOM/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from matplotlib.widgets import Button
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.colors as mcolors
 
+
 class SOMPlots(SOM):
     """
     SOMPlots extends the SOM class by adding visualization capabilities to
     the Self-Organizing Map (SOM). It allows for the graphical representation
     of the SOM's structure, the distribution of input data across its neurons,
     and various other analytical visualizations that aid in the interpretation
     of the SOM's behavior and characteristics.
```

### Comparing `nnsom-1.6.3/src/NNSOM/som.py` & `nnsom-1.6.4/src/NNSOM/som.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .utils import *
+from .utils import calculate_positions, distances, normalize_position, spread_positions
+
 import numpy as np
-from tensorflow.keras.utils import to_categorical
 from datetime import datetime
 from scipy.spatial.distance import cdist
 import pickle
 import warnings
 
-class SOM():
+class SOM:
     """
     A class to represent a Self-Organizing Map (SOM), a type of artificial neural network
     trained using unsupervised learning to produce a two-dimensional, discretized representation
     of the input space of the training samples.
 
     Attributes
     ----------
@@ -73,15 +73,15 @@
         # Calculate distances between neurons
         self.neuron_dist = distances(self.pos)
         # Initialize the weight matrix with empty list
         self.w = []
         # Set simulation flag to True,  needs to do simulation
         self.sim_flag = True
         # Initialize the output of simulation
-        self.output = None
+        self.outputs = None
         # Initialize a normalize() function
         self.norm_func = None
 
         # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
         self.sub_som = {}
 
     def init_w(self, x, norm_func=None):
@@ -181,15 +181,15 @@
         #     n[jj] = np.sum((x - wj)**2, axis=0)
 
         # n = -np.sqrt(n)
         #print(n)
 
         # Find out which center was closest to the input
         maxRows = np.argmax(n, axis=0)
-        a = to_categorical(maxRows, num_classes=n.shape[0]) #made correction-added number of class
+        a = self._to_categorical(maxRows, num_classes=n.shape[0])   # made correction-added number of class
         # a = tf.constant(a, shape=[np.transpose(n).shape[0],np.transpose(n).shape[1]])  # made change
         return np.transpose(a)
 
     def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
         """
         Trains the SOM using the batch SOM algorithm on the input data x.
 
@@ -254,15 +254,15 @@
 
             dw[loserIndex] = 0
 
             w = w + np.array(dw)
 
             step = step + 1
 
-            if step%50==0:
+            if step % 50 == 0:
                 print(step)
                 now = datetime.now()
                 current_time = now.strftime("%H:%M:%S")
                 print("Current Time =", current_time)
 
         self.w = w
         self.outputs = self.sim_som(x)
@@ -527,7 +527,39 @@
             raise ValueError('data_format must be one of: pkl')
 
         if data_format == 'pkl':
             with open(path + filename, 'rb') as f:
                 som = pickle.load(f)
 
         return som
+
+    def _to_categorical(self, x, num_classes=None):
+        """ Converts a class vector (integers) to binary class matrix.
+
+        Args:
+        x: Array-like with class values to be converted into a matrix
+            (integers from 0 to `num_classes - 1`).
+        num_classes: Total number of classes. If `None`, this would be inferred
+            as `max(x) + 1`. Defaults to `None`.
+
+        Returns:
+        A binary matrix representation of the input as a NumPy or Cupy array. The class
+        axis is placed last.
+
+        """
+        x = np.array(x, dtype="int64")
+        input_shape = x.shape
+
+        # Shrink the last dimension if the shape is (..., 1).
+        if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
+            input_shape = tuple(input_shape[:-1])
+
+        x = x.reshape(-1)
+        if not num_classes:
+            num_classes = np.max(x) + 1
+        batch_size = x.shape[0]
+        categorical = np.zeros((batch_size, num_classes))
+        categorical[np.arange(batch_size), x] = 1
+        output_shape = input_shape + (num_classes,)
+        categorical = np.reshape(categorical, output_shape)
+
+        return categorical
```

### Comparing `nnsom-1.6.3/src/NNSOM/utils.py` & `nnsom-1.6.4/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.3/.gitignore` & `nnsom-1.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.3/pyproject.toml` & `nnsom-1.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.6.3"
+version = "1.6.4"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.6.3/PKG-INFO` & `nnsom-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.6.3
+Version: 1.6.4
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

