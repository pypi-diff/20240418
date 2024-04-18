# Comparing `tmp/nnsom-1.6.7.tar.gz` & `tmp/nnsom-1.6.8.tar.gz`

## Comparing `nnsom-1.6.7.tar` & `nnsom-1.6.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.6.7/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.7/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.7/src/NNSOM/som.py
--rw-r--r--   0        0        0    23705 2020-02-02 00:00:00.000000 nnsom-1.6.7/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    22097 2020-02-02 00:00:00.000000 nnsom-1.6.7/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.7/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.7/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.8/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.8/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.8/PKG-INFO
```

### Comparing `nnsom-1.6.7/src/NNSOM/plots.py` & `nnsom-1.6.8/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.7/src/NNSOM/som.py` & `nnsom-1.6.8/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.7/src/NNSOM/som_gpu.py` & `nnsom-1.6.8/src/NNSOM/som_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,23 @@
             num = len(tempclust)
             cluster_sizes.append(num)
 
             # Save the maximum distance to any input in the cluster from cluster center
             if num > 0:
                 max_cluster_distances[i] = tempdist[-1]
 
+        # Convert clusters to a list of lists
+        clusters = [clust.get().tolist() for clust in clusters]
+        # Convert cluster_distances to a list of lists
+        cluster_distances = [dist.get().tolist() for dist in cluster_distances]
+        # Convert max_cluster_distances to a NumPy array
+        max_cluster_distances = max_cluster_distances.get()
+        # Convert cluster_sizes to a NumPy array
+        cluster_sizes = np.array(cluster_sizes)
+
         return clusters, cluster_distances, max_cluster_distances, cluster_sizes
 
     def normalize(self, x, norm_func=None):
         """
         Normalize the input data using a custom function.
 
         Parameters
```

### Comparing `nnsom-1.6.7/src/NNSOM/utils.py` & `nnsom-1.6.8/src/NNSOM/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from scipy import sparse
 import numpy as np
 import networkx as nx
 from matplotlib.widgets import Button
 
 
 def preminmax(p):
-    p = np.asarray(p)
     # Normalize the inputs to be in the range [-1, 1]
     minp = np.amin(p, 1)
     maxp = np.amax(p, 1)
 
     equal = np.equal(minp, maxp)
     nequal = np.logical_not(equal)
 
@@ -55,34 +54,28 @@
         len1 = newlen
         center = 0.5
 
     return position
 
 
 def cart2pol(x, y):
-    x = np.asarray(x)
-    y = np.asarray(y)
-
     # Convert cartesian coordinates to polar coordinates
     theta = np.arctan2(y, x)
     rho = np.hypot(x, y)
     return theta, rho
 
 
 def pol2cart(theta, rho):
     # Convert polar coordinates to cartesian coordinates
     x = rho * np.cos(theta)
     y = rho * np.sin(theta)
     return x, y
 
 
 def rotate_xy(x1, y1, angle):
-    x1 = np.asarray(x1)
-    y1 = np.asarray(y1)
-
     # Rotate the coordinates x1, y1 by angle
     [a, r] = cart2pol(x1, y1)
     a = a + angle
     x2, y2 = pol2cart(a, r)
     return x2, y2
 
 
@@ -153,17 +146,14 @@
         A list where each element is an array of indices for data points in the corresponding cluster.
 
     Returns
     -------
     cluster_data_list : list of numpy arrays
         A list where each element is a numpy array containing the data points of a cluster.
     """
-    data = np.asarray(data)
-    clust = np.asarray(clust)
-
     cluster_data_list = []
     for cluster_indices in clust:
         if len(cluster_indices) > 0:
             # Ensure cluster_indices are integers and within the range of data
             cluster_indices = np.array(cluster_indices, dtype=int)
             cluster_data = data[cluster_indices]
             cluster_data_list.append(cluster_data)
@@ -185,17 +175,14 @@
         A list of cluster arrays, each containing indices sorted by distances.
 
     Returns
     -------
     cluster_array : numpy.ndarray
         A NumPy array where each element is an array of feature values for that cluster.
     """
-    feature = np.asarray(feature)
-    clust = np.asarray(clust)
-
     cluster_array = np.empty(len(clust), dtype=object)
 
     for i, cluster_indices in enumerate(clust):
         if len(cluster_indices) > 0:
             cluster_array[i] = feature[cluster_indices]
         else:
             cluster_array[i] = np.array([])  # Store an empty array if the cluster is empty
@@ -215,17 +202,14 @@
         A list of cluster arrays, each containing indices sorted by distances.
 
     Returns
     -------
     cluster_avg : numpy array
         A cluster array with the average value of the feature for each cluster.
     """
-    feature = np.asarray(feature)
-    clust = np.asarray(clust)
-
     cluster_array = get_cluster_array(feature, clust)
     cluster_avg = np.zeros(len(cluster_array))
     for i in range(len(cluster_array)):
         if len(cluster_array[i]) > 0:
             cluster_avg[i] = np.mean(cluster_array[i])
 
     return cluster_avg
@@ -243,17 +227,14 @@
         A cluster array of indices sorted by distances.
 
     Returns
     -------
     closest_class : numpy array
         A cluster array with the closest class for each cluster.
     """
-    cat_feature = np.asarray(cat_feature)
-    clust = np.asarray(clust)
-
     closest_class = np.zeros(len(clust))
     for i in range(len(clust)):
         cluster_indices = clust[i]
         if len(cluster_indices) > 0:
             closest_class[i] = cat_feature[cluster_indices[0]]
         else:
             closest_class[i] = None  # Avoid division by zero if the cluster is empty
@@ -273,17 +254,14 @@
         A cluster array of indices sorted by distances.
 
     Returns
     -------
     majority_class : numpy array
         A cluster array with the majority class
     """
-    cat_feature = np.asarray(cat_feature)
-    clust = np.asarray(clust)
-
     majority_class = np.zeros(len(clust))
     for i in range(len(clust)):
         cluster_indices = clust[i]
         if len(cluster_indices) > 0:
             majority_class[i] = np.argmax(np.bincount(cat_feature[cluster_indices]))
         else:
             majority_class[i] = None  # Avoid division by zero if the cluster is empty
@@ -305,18 +283,14 @@
         A cluster array of indices sorted by distances.
 
     Returns
     -------
     cluster_array : numpy array
         A cluster array with the percentage of target class.
     """
-    cat_feature = np.asarray(cat_feature)
-    target = np.asarray(target)
-    clust = np.asarray(clust)
-
     # Create Cluster Array with the percentage of target class
     cluster_array = np.zeros(len(clust))
     for i in range(len(clust)):
         cluster_indices = clust[i]
         if len(cluster_indices) > 0:
             cluster_array[i] = np.sum(cat_feature[cluster_indices] == target) / len(cluster_indices)
         else:
@@ -338,17 +312,14 @@
         A list of arrays, each containing the indices of elements in a cluster.
 
     Returns
     -------
     cluster_counts : numpy array
         A 2D array with counts of each class in each cluster.
     """
-    cat_feature = np.asarray(cat_feature)
-    clust = np.asarray(clust)
-
     unique_classes, _ = np.unique(cat_feature, return_counts=True)
     num_classes = len(unique_classes)
 
     # Initialize the array to hold class counts for each cluster
     cluster_counts = np.zeros((len(clust), num_classes), dtype=int)
 
     # Loop over clusters to count class occurrences
@@ -393,16 +364,14 @@
     >>> ind4 = np.array([10, 11, 12])
     >>> get_sizes_clust(clust, ind1, ind2, ind3, ind4)
     array([[0, 2, 1, 0],
            [1, 0, 1, 0],
            [1, 0, 0, 2],
            [1, 1, 1, 0]])
     """
-    clust = np.asarray(clust)
-
     numst = list(args)
 
     cluster_sizes_matrix = np.zeros((len(numst), len(clust)))
 
     for i, ind in enumerate(numst):
         for j, cluster in enumerate(clust):
             cluster_sizes_matrix[i][j] = np.sum(np.isin(cluster, ind))
@@ -423,17 +392,14 @@
         The predicted values.
 
     Returns
     -------
     misclassified_indices : list
         List of indices of misclassified items.
     """
-    target = np.asarray(target)
-    prediction = np.asarray(prediction)
-
     misclassified_indices = np.where(target != prediction)[0]
 
     return misclassified_indices
 
 
 def get_perc_misclassified(target, prediction, clust):
     """
@@ -449,18 +415,14 @@
         List of arrays, each containing the indices of elements in a cluster.
 
     Returns
     -------
     proportion_misclassified : numpy array
         Percentage of misclassified items in each cluster.
     """
-    target = np.asarray(target)
-    prediction = np.asarray(prediction)
-    clust = np.asarray(clust)
-
     # Get the indices of misclassified items.
     misclassified_indices = get_ind_misclassified(target, prediction)
 
     # Initialize array to store proportion of misclassified items
     proportion_misclassified = np.zeros(len(clust))
 
     for i, cluster_indices in enumerate(clust):
@@ -492,17 +454,14 @@
     tn_index : numpy array
         Indices of True Negatives.
     fp_index : numpy array
         Indices of False Positives.
     fn_index : numpy array
         Indices of False Negatives.
     """
-    target = np.asarray(target)
-    results = np.asarray(results)
-
     tp_index = np.where((target == target_class) & (results == target_class))[0]
     tn_index = np.where((target != target_class) & (results != target_class))[0]
     fp_index = np.where((target != target_class) & (results == target_class))[0]
     fn_index = np.where((target == target_class) & (results != target_class))[0]
 
     return tp_index, tn_index, fp_index, fn_index
 
@@ -520,17 +479,14 @@
         Variable number of arrays, each representing majority error types for each class.
 
     Returns:
     ---------------
     array-like (som.numNeurons, )
         List of majority error type for each cluster corresponding to the dominant class.
     """
-    dominant_classes = np.asarray(dominant_classes)
-    error_types = np.asarray(error_types)
-
     if len(error_types) < np.max([dc for dc in dominant_classes if not np.isnan(dc)]) + 1:
         raise ValueError("Not enough error type arrays provided for all classes.")
 
     # Initialize the output array with NaNs to handle possible missing classes
     output_error_types = np.full(len(dominant_classes), np.nan)
 
     # Map the correct error type based on the dominant class
@@ -576,15 +532,14 @@
     Args:
         data: A nested list of integers. The structure can be of any depth.
 
     Returns:
         A tuple (min_value, max_value) where min_value is the minimum value
         in the data, and max_value is the maximum value.
     """
-    data = np.asarray(data)
     flat_list = flatten(data)
     return min(flat_list), max(flat_list)
 
 
 def get_edge_widths(indices, clust):
     """ Calculate edge width for each cluster based on the number of indices in the cluster.
 
@@ -594,17 +549,14 @@
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
 
     Returns:
         lwidth: 1-d array
             Array of edge widths for each cluster.
     """
-    indices = np.asarray(indices)
-    clust = np.asarray(clust)
-
     lwidth = np.zeros(len(clust))
 
     for i in range(len(clust)):
         if len(clust[i]) != 0:
             if len(np.intersect1d(clust[i], indices)) > 0:
                 lwidth[i] = 20. * len(np.intersect1d(clust[i], indices)) / len(clust[i])
             else:
@@ -621,16 +573,14 @@
     Args:
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
 
         *args: 1-d array
             A list of indices where the specific class is present.
     """
-    clust = np.asarray(clust)
-
     # Validate if the user have provided at least one class indices
     if len(listOfIndices) == 0:
         raise ValueError('At least one class indices must be provided.')
 
     # Validate if the arg is a list or numpy array and unpack them
     numst = []
     for arg in listOfIndices:
@@ -643,15 +593,14 @@
     color_labels = np.zeros(len(clust))
 
     # When there is only one list provides,
     # check if the cluster contains the indices of the class.
     # If that class is majority in the cluster, assign 1, otherwise 0.
     if len(numst) == 1:
         indices = numst[0]
-        indices = np.asarray(indices)
         for i in range(len(clust)):
             if len(clust[i]) != 0:
                 num_class = len(np.intersect1d(clust[i], indices))
                 if num_class > len(clust[i]) / 2:
                     color_labels[i] = 1
                 else:
                     color_labels[i] = 0
```

### Comparing `nnsom-1.6.7/.gitignore` & `nnsom-1.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.7/pyproject.toml` & `nnsom-1.6.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.6.7"
+version = "1.6.8"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.6.7/PKG-INFO` & `nnsom-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.6.7
+Version: 1.6.8
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

