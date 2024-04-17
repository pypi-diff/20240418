# Comparing `tmp/ecdf_estimator-0.1.6.tar.gz` & `tmp/ecdf_estimator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecdf_estimator-0.1.6.tar", last modified: Mon Feb 12 15:20:23 2024, max compression
+gzip compressed data, was "ecdf_estimator-0.1.7.tar", last modified: Wed Apr 17 22:04:18 2024, max compression
```

## Comparing `ecdf_estimator-0.1.6.tar` & `ecdf_estimator-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-02-12 15:20:23.804532 ecdf_estimator-0.1.6/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4526 2024-02-12 15:20:23.804532 ecdf_estimator-0.1.6/PKG-INFO
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     3803 2023-02-01 20:30:53.000000 ecdf_estimator-0.1.6/README.md
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-02-12 15:20:23.800532 ecdf_estimator-0.1.6/ecdf_estimator/
--rw-rw-r--   0 andreas   (1000) andreas   (1000)      104 2022-12-19 19:13:38.000000 ecdf_estimator-0.1.6/ecdf_estimator/__init__.py
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     5983 2023-03-18 13:10:11.000000 ecdf_estimator-0.1.6/ecdf_estimator/objective_function.py
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     3049 2022-12-19 19:13:38.000000 ecdf_estimator-0.1.6/ecdf_estimator/output.py
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     4799 2024-02-12 15:19:00.000000 ecdf_estimator-0.1.6/ecdf_estimator/select_bins.py
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     9342 2024-02-12 15:19:00.000000 ecdf_estimator-0.1.6/ecdf_estimator/utils.py
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-02-12 15:20:23.800532 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4526 2024-02-12 15:20:23.000000 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/PKG-INFO
--rw-rw-r--   0 andreas   (1000) andreas   (1000)      365 2024-02-12 15:20:23.000000 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/SOURCES.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)        1 2024-02-12 15:20:23.000000 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/dependency_links.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       30 2024-02-12 15:20:23.000000 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/requires.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       15 2024-02-12 15:20:23.000000 ecdf_estimator-0.1.6/ecdf_estimator.egg-info/top_level.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)      763 2024-02-12 15:19:00.000000 ecdf_estimator-0.1.6/pyproject.toml
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       38 2024-02-12 15:20:23.804532 ecdf_estimator-0.1.6/setup.cfg
--rw-rw-r--   0 andreas   (1000) andreas   (1000)      674 2024-02-12 15:19:00.000000 ecdf_estimator-0.1.6/setup.py
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-17 22:04:18.621406 ecdf_estimator-0.1.7/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4560 2024-04-17 22:04:18.621406 ecdf_estimator-0.1.7/PKG-INFO
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     3803 2023-02-01 20:30:53.000000 ecdf_estimator-0.1.7/README.md
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-17 22:04:18.617406 ecdf_estimator-0.1.7/ecdf_estimator/
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)      104 2022-12-19 19:13:38.000000 ecdf_estimator-0.1.7/ecdf_estimator/__init__.py
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     6447 2024-04-16 13:36:21.000000 ecdf_estimator-0.1.7/ecdf_estimator/objective_function.py
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     3049 2022-12-19 19:13:38.000000 ecdf_estimator-0.1.7/ecdf_estimator/output.py
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     4629 2024-04-10 20:33:55.000000 ecdf_estimator-0.1.7/ecdf_estimator/select_bins.py
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     9534 2024-04-17 21:58:25.000000 ecdf_estimator-0.1.7/ecdf_estimator/utils.py
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-17 22:04:18.621406 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4560 2024-04-17 22:04:18.000000 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/PKG-INFO
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)      365 2024-04-17 22:04:18.000000 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/SOURCES.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)        1 2024-04-17 22:04:18.000000 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/dependency_links.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       46 2024-04-17 22:04:18.000000 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/requires.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       15 2024-04-17 22:04:18.000000 ecdf_estimator-0.1.7/ecdf_estimator.egg-info/top_level.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)      808 2024-04-17 21:51:28.000000 ecdf_estimator-0.1.7/pyproject.toml
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       38 2024-04-17 22:04:18.621406 ecdf_estimator-0.1.7/setup.cfg
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)      793 2024-04-17 21:53:58.000000 ecdf_estimator-0.1.7/setup.py
```

### Comparing `ecdf_estimator-0.1.6/PKG-INFO` & `ecdf_estimator-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ecdf_estimator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for parameter estimation of random data
 Home-page: https://github.com/AndreasRupp/ecdf_estimator
 Author: Andreas Rupp
 Author-email: Andreas Rupp <info@rupp.ink>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/AndreasRupp/ecdf_estimator
 Project-URL: Bug Tracker, https://github.com/AndreasRupp/ecdf_estimator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11.6
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: matplotlib>=3.6
+Requires-Dist: numpy>=1.25.0
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: matplotlib>=3.7.1
 
 # Welcome to ecdf_estimator
 
 [![PyPI Version](https://badge.fury.io/py/ecdf_estimator.svg)](
 https://badge.fury.io/py/ecdf_estimator)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/ecdf_estimator.svg?label=PyPI%20downloads)](
 https://pypi.org/project/ecdf_estimator/)
```

### Comparing `ecdf_estimator-0.1.6/README.md` & `ecdf_estimator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ecdf_estimator-0.1.6/ecdf_estimator/objective_function.py` & `ecdf_estimator-0.1.7/ecdf_estimator/objective_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from inspect import signature
 import ecdf_estimator.utils as ecdf_aux
 
 
 # --------------------------------------------------------------------------------------------------
 # Standard objective function:
 # --------------------------------------------------------------------------------------------------
 
@@ -35,31 +36,45 @@
     self.error_printed  = False
 
   ## \private
   def evaluate_ecdf(self, dataset):
     if len(dataset) not in self.subset_sizes:
       print("WARNING: Dataset size is different!")
     
+    n_params = len(signature(self.distance_fct).parameters)
+    comparison_ind = []
     if self.compare_all:
-      comparison_ind = np.random.randint( len(self.subset_sizes) )
+      for _ in range(n_params-1):
+        helper = np.random.randint( len(self.subset_sizes) )
+        while helper in comparison_ind:
+          helper = np.random.randint( len(self.subset_sizes) )
+        comparison_ind.append(helper)
     else:
-      comparison_ind = [ i for i in range(len(self.subset_sizes)) \
-                         if self.subset_sizes[i] == len(dataset) ]
-      comparison_ind = comparison_ind[np.random.randint(len(comparison_ind))]
-    
-    distance_list = ecdf_aux.create_distance_matrix(self.dataset, dataset,
-      self.distance_fct, self.subset_indices[comparison_ind], self.subset_indices[comparison_ind+1])
+      for _ in range(n_params-1):
+        helper = helper_ind[np.random.randint(len(helper_ind))]
+        while helper in comparison_ind:
+          helper = np.random.randint( len(self.subset_sizes) )
+        comparison_ind.append(helper)
+
+    dataset_list = [dataset] + [self.dataset] * (n_params-1)
+    start_index_list = [0] + [ self.subset_indices[index] for index in comparison_ind ]
+    end_index_list = [len(dataset)] + [ self.subset_indices[index+1] for index in comparison_ind ]
+
+    distance_list = ecdf_aux.create_distance_matrix(
+      dataset_list, self.distance_fct, start_index_list, end_index_list )
+
     while isinstance(distance_list[0], list):
       distance_list = [item for sublist in distance_list for item in sublist]
+
     return ecdf_aux.empirical_cumulative_distribution_vector(distance_list, self.bins)
 
   ## \private
   def evaluate( self, dataset ):
-    return ecdf_aux.evaluate_from_empirical_cumulative_distribution_functions( self,
-      self.evaluate_ecdf(dataset) )
+    return ecdf_aux.evaluate_from_empirical_cumulative_distribution_functions(
+      self, self.evaluate_ecdf(dataset) )
 
 # --------------------------------------------------------------------------------------------------
 # Objective function for bootstrapping:
 # --------------------------------------------------------------------------------------------------
 
 ## \brief  Objective function assembled via bootstrapping.
 class bootstrap:
@@ -89,16 +104,16 @@
 
   ## \private
   def evaluate_ecdf( self, dataset ):
     if len(dataset) != self.n_elements_a:
       print("WARNING: Size of the dataset should equal n_elements_a!")
     
     comparison_set = [ dataset[i] for i in np.random.randint(len(dataset), size=self.n_elements_b) ]
-    distance_list  = ecdf_aux.create_distance_matrix(comparison_set, dataset, self.distance_fct)
-    distance_list  = [item for sublist in distance_list for item in sublist]
+    dataset_list = [dataset, comparison_set]
+    distance_list  = ecdf_aux.create_distance_matrix(dataset_list, self.distance_fct)
     return ecdf_aux.empirical_cumulative_distribution_vector(distance_list, self.bins)
 
   ## \private
   def evaluate( self, dataset ):
     return ecdf_aux.evaluate_from_empirical_cumulative_distribution_functions( self,
       self.evaluate_ecdf(dataset) )
```

### Comparing `ecdf_estimator-0.1.6/ecdf_estimator/output.py` & `ecdf_estimator-0.1.7/ecdf_estimator/output.py`

 * *Files identical despite different names*

### Comparing `ecdf_estimator-0.1.6/ecdf_estimator/select_bins.py` & `ecdf_estimator-0.1.7/ecdf_estimator/select_bins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import numpy as np
 from inspect import signature
 import ecdf_estimator.utils as ecdf_aux
+import itertools as it
 
 
 ## \brief  Heuristically determine region in which useful bin/radii values are located.
 #
-#  \param   dataset_a        Subset of the overall dataset.
-#  \param   dataset_b        Different subset of the poverall dataset.
+#  \param   data             The whole training data from which some subsets are selected.
+#  \param   subset_sizes     The size of the subsets.
 #  \param   distance_fct     Functions that evaluates (generalized) distance between subset members.
 #  \param   rel_offset       Relative offset to determin interval of reasonable bin values.
 #  \param   rel_cutoff       Relative cutoff of the interval of reasonable bin values.            
 #  \retval  target_val       The value of the target function.
-def estimate_radii_values( dataset_a, dataset_b, distance_fct, rel_offset=0.05, rel_cutoff=0.05 ):
-  n_params = len(signature(distance_fct).parameters)
-  if n_params < 1 or n_params > 2:
-    raise Exception("Distance function must accept one or two arguments.")
+def estimate_radii_values( data, subset_sizes, distance_fct, rel_offset=0.05, rel_cutoff=0.05 ):
+  n_params, n_elem = len(signature(distance_fct).parameters), 0
+  datasets = []
+  for i in range(n_params):
+    datasets.append(data[ n_elem : n_elem + subset_sizes[i] ])
+    n_elem += subset_sizes[i]
 
-  if n_params == 1:
-    distance_data = [ distance_fct(data_a) for data_a in dataset_a ]
-  else:
-    distance_data = [ distance_fct(data_a, data_b) for data_b in dataset_b for data_a in dataset_a ]
-
-  while isinstance(distance_data[0], list):
-    distance_data = [item for sublist in distance_data for item in sublist]
+  distance_data = [ distance_fct(*item) for item in it.product(*datasets) ]
   distance_data = np.sort(distance_data)
 
   data_offset = round(len(distance_data) * rel_offset)
   radius_max  = distance_data[-(data_offset + 1)]
   radius_min  = distance_data[data_offset]
 
   upper_bound = radius_max + rel_cutoff * (radius_max - radius_min)
```

### Comparing `ecdf_estimator-0.1.6/ecdf_estimator/utils.py` & `ecdf_estimator-0.1.7/ecdf_estimator/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from inspect import signature
+import itertools as it
+import collections.abc
 
 
 ## \brief   Create list of ECDF values.
 #
 #  This function creates the empirical cumulative distribution functions from a list of distances
 #  and a list of bin values. That is, each element of the resulting list tells how many elements of
 #  the distance list are smaller than the respective bin value.
@@ -11,66 +13,64 @@
 #  \param   distance_list  List of distances to be grouped into the bins.
 #  \param   bins           List of bins.
 #  \retval  ecdf_list      Resulting list of amout of distances that are smaller than resp. bins.
 def empirical_cumulative_distribution_vector( distance_list, bins ):
   return [ np.sum( [distance < basket for distance in distance_list] ) / len(distance_list) \
            for basket in bins ]  # np.sum appears to be much faster than Python's standard sum!
 
-## \brief   Assemble matrix of (generalized) distances between elemenst of datasets.
+
+## \brief   Assemble list of (generalized) distances between elemenst of datasets.
 #
-#  This function creates a matrix whose (i,j)th entry corresponds to the distance between element
-#  i of a subset of dataset_a and element j of a subset of dataset_b. The respective subsets are
-#  characterized by the indices of the respective first and last elements.
-#  Notably, the matrix entries can be numbers or more general data types (such as lists). If
-#  dataset_b is None, all entries of dataset_a in [start_a, end_a] are compared against one another.
-#
-#  \param   dataset_a      First dataset, whose subset is compared to second dataset.
-#  \param   dataset_b      Second dataset, whose subset is compared to first dataset.
-#  \param   distance_fct   Function generating a generalized distance between members of datasets.
-#  \param   start_a        Starting index of considered subset of dataset_a. Defaults to 0. 
-#  \param   end_a          Last (exclusive) index of consideres subset. Defaults to len(dataset).
-#  \param   start_b        Starting index of considered subset of dataset_b. Defaults to 0. 
-#  \param   end_b          Last (exclusive) index of consideres subset. Defaults to len(dataset).
-#  \retval  distance_mat   Matrix of generalized distances.
-def create_distance_matrix( dataset_a, dataset_b, distance_fct, 
-  start_a=0, end_a=None, start_b=0, end_b=None ):
+#  This function creates a list of distances between elements of subsets which are compared to 
+#  each other. The amount of subsets compared to each other is defined by the number of arguments
+#  in the distance function. The distances of all value combinations of these subsets are computed. 
+#
+#  \param   dataset_list       The list of datasets which are compared to each other.
+#  \param   distance_fct       Generalized distance function  among several datasets.
+#  \param   start_index_list   Starting indices of the datasets. Defaults to None.
+#  \param   end_index_list     Ending indices of the datasets. Defaults to None.
+#  \retval  distance_mat       Matrix of generalized distances.
+def create_distance_matrix(dataset_list, distance_fct, start_index_list=None, end_index_list=None):
+  if start_index_list is None:  start_index_list = [0] * len(dataset_list)
+  if end_index_list is None:    
+    if isinstance(dataset_list[0], collections.abc.Sequence):
+      end_index_list = [ len(item) for item in dataset_list ]
+    else:
+      end_index_list = [0] * len(dataset_list)  
+
   n_params = len(signature(distance_fct).parameters)
 
-  if end_a is None:   end_a = len(dataset_a)
-  if end_a < start_a: raise Exception("Invalid subset indices chosen.")
-  if n_params < 1 or n_params > 2:
-    raise Exception("Distance function must accept one or two arguments.")
+  if ( n_params != 2 or len(dataset_list) != 1 )  and  ( len(dataset_list) != n_params or \
+    len(start_index_list) != n_params or len(end_index_list) != n_params ):
+    raise Exception("Length of dataset list must be equal to the length of the start index list, "+\
+      "the length of the end index list, and the number of arguments of the distance function. "+\
+      "\nAlternatively, you can use a single dataset with a binary distance function.")
+  
+  for k in range(0,len(start_index_list)):
+    if end_index_list[k] < start_index_list[k]: raise Exception("Invalid subset indices chosen.")
 
   if n_params == 1:
-    return [ distance_fct(dataset_a[i]) for i in range(start_a, end_a) ]
-  # end: if n_params == 1
+    return [distance_fct(dataset_list[0][i]) for i in range(start_index_list[0], end_index_list[0])]
+
+  if (len(dataset_list[0]) == len(dataset_list[1])):
+    return [distance_fct(*item) for item in it.product(*dataset_list)]
 
-  if dataset_b is None:
-    if end_a != len(dataset_a) or start_a != 0: raise Exception("You need to use the whole dataset")
-    
-    matrix = [ [0.] * (end_a - start_a) for _ in range(start_a, end_a) ]
-    for i in range(end_a):
-      for j in range(i):
-        matrix[i][j] = distance_fct(dataset_a[i], dataset_a[j])
-        matrix[j][i] = matrix[i][j]
-    return matrix
-  # end: if dataset_b is None
+  sets = [dataset_list[i][start_index_list[i]:end_index_list[i]] for i in range(len(dataset_list))]
 
-  if end_b is None:   end_b = len(dataset_b)
-  if end_b < start_b: raise Exception("Invalid subset indices chosen.")
+  return [distance_fct(*item) for item in it.product(*sets)]
 
-  return [ [ distance_fct(dataset_a[i], dataset_b[j]) for j in range(start_b, end_b) ] \
-             for i in range(start_a, end_a) ]
 
 
 ## \brief   Assemble ecdf vector, whose elements are list of values for all subset combinations.
 #
 #  This function assembles a list of ecdf vectors for all possible combinations of subsets of the
-#  dataset. Importantly, none of the subsets are compared to themselves and subsets i and j are
-#  compared only once (not i with j and j with i).
+#  dataset. Importantly, none of the subsets are compared to themselves. The subset combinations and
+#  their indexes are chosen. Then, the distances are computed by create_distance_matrix function
+#  and added to a matrix. 
+#
 #  The first dimension of the result refers to the index of the bin / ecdf vector. The second index
 #  of the result refers to the subset combination.
 #
 #  \param   dataset        First dataset, whose subset are compared to one another.
 #  \param   bins           List of bins.
 #  \param   distance_fct   Function generating a generalized distance between members of dataset.
 #  \param   subset_indices List of starting (and ending) indices of disjointly subdivided dataset.
@@ -81,37 +81,39 @@
   n_params = len(signature(distance_fct).parameters)
   matrix = []
 
   if not all(subset_indices[i] <= subset_indices[i+1] for i in range(len(subset_indices)-1)):
     raise Exception("Subset indices are out of order.")
   if subset_indices[0] != 0 or subset_indices[-1] != len(dataset):
     raise Exception("Not all elements of the dataset are distributed into subsets.")
-  if n_params < 1 or n_params > 2:
-    raise Exception("Distance function must accept one or two arguments.")
 
   if n_params == 1:
     for i in range(len(subset_indices)-1):
-      distance_list = create_distance_matrix(dataset, None, distance_fct,
-        subset_indices[i], subset_indices[i+1])
+      distance_list = create_distance_matrix(
+        [dataset], distance_fct, [subset_indices[i]], [subset_indices[i+1]] )
+      
       while isinstance(distance_list[0], list):
         distance_list = [item for sublist in distance_list for item in sublist]
       matrix.append( empirical_cumulative_distribution_vector(distance_list, bins) )
+
     return np.transpose(matrix)
   # end: if n_params == 1
 
-  for i in range(len(subset_indices)-1):
-    for j in range(i):
-      if not compare_all and \
-        subset_indices[i+1] - subset_indices[i] == subset_indices[j+1] - subset_indices[j]:
-        continue
-      distance_list = create_distance_matrix(dataset, dataset, distance_fct, 
-        subset_indices[i], subset_indices[i+1], subset_indices[j], subset_indices[j+1])
-      while isinstance(distance_list[0], list):
-        distance_list = [item for sublist in distance_list for item in sublist]
-      matrix.append( empirical_cumulative_distribution_vector(distance_list, bins) )
+  combinations = it.combinations(list(range(0,len(subset_indices)-1)), n_params)
+  dataset_list = []
+  for combo in combinations:
+    dataset_list = [ dataset[subset_indices[combo[i]]:subset_indices[combo[i]+1]] \
+                     for i in range(len(combo)) ]
+    start_index_list = [subset_indices[index] for index in combo]
+    end_index_list = [subset_indices[index+1] for index in combo]
+
+    distance_list = create_distance_matrix(
+      dataset_list, distance_fct, start_index_list, end_index_list )
+    matrix.append(empirical_cumulative_distribution_vector( distance_list, bins ))
+    dataset_list = []
 
   return np.transpose(matrix)
 
 
 ## \brief   Same as empirical_cumulative_distribution_vector_list, but for bootstrapping.
 #
 #  \param   dataset        Dataset, whose elements are compared to one another.
@@ -119,33 +121,42 @@
 #  \param   n_elements_b   Number of elements in second (larger) subset.
 #  \param   bins           List of bins.
 #  \param   distance_fct   Function generating a generalized distance between members of dataset.
 #  \param   n_samples      Number of perturbatins of the datasets.
 #  \retval  ecdf_list      ecdf vector enlisting values for subset combinations.
 def empirical_cumulative_distribution_vector_list_bootstrap(
   dataset, bins, distance_fct, n_elements_a, n_elements_b, n_samples ):
-  distance_matrix = np.array( create_distance_matrix(dataset, None, distance_fct) )
-  matrix = []
-  for _ in range(n_samples):
-    select_a = np.random.randint(len(dataset), size=n_elements_a)
-    indices  = [ i for i in range(len(dataset)) if i not in select_a ]
-    select_b = [ indices[x] for x in np.random.randint(len(indices), size=n_elements_b) ]
+  n_params = len(signature(distance_fct).parameters)
+  dataset_list = []
+
+  if n_params == 2:
+    dataset_list.append(dataset[0:n_elements_a])
+    dataset_list.append(dataset[n_elements_a:n_elements_a+n_elements_b])
+    distance_matrix = np.array( create_distance_matrix(dataset_list, distance_fct) )
+
+    matrix = []
+    for _ in range(n_samples):
+      select_a = np.random.randint(len(distance_matrix), size=n_elements_a)
+      indices  = [ i for i in range(len(distance_matrix)) if i not in select_a ]
+      select_b = [ indices[x] for x in np.random.randint(len(indices), size=n_elements_b) ]
 
-    distance_list = np.ndarray.flatten( distance_matrix[np.ix_(select_a,select_b)] )
-    matrix.append( empirical_cumulative_distribution_vector(distance_list, bins) )
+      distance_list = [ distance_matrix[i] for sublist in [select_a, select_b] for i in sublist ]
+      matrix.append( empirical_cumulative_distribution_vector(distance_list, bins) )
+      
   return np.transpose(matrix)
 
 
 ## \brief  Vector of means of the ecdf vectors.
 #
 #  \param   ecdf_list      Usually the result of empirical_cumulative_distribution_vector_list.
 #  \retval  ecdf_means     Element-wise mean values of the ecdf vectors.
 def mean_of_ecdf_vectors( ecdf_vector_list ):
   return [ np.mean(vector) for vector in ecdf_vector_list ]
 
+
 ## \brief  Covariance matrix of ecdf vectors.
 #
 #  \param   ecdf_list      Usually the result of empirical_cumulative_distribution_vector_list.
 #  \retval  ecdf_covar     Covariance matrix associated to the ecdf vectors.
 def covariance_of_ecdf_vectors( ecdf_vector_list ):
   return np.cov( ecdf_vector_list )
 
@@ -156,23 +167,25 @@
 #
 #  \param   estimator      The estimator class defining the specifics of the target function.
 #  \param   dataset        The dataset with respect to which the target function is evaluated.
 #  \retval  target_val     The value of the target function.
 def evaluate( estimator, dataset ):
   return estimator.evaluate( dataset )
 
+
 ## \brief  Evaluate target/objective/cost function associated to estimator type from ecdf vector.
 #
 #  Evaluate the negative log-likelihood in the way that is characterized by the estimator.
 #
 #  \param   estimator      The estimator class defining the specifics of the target function.
 #  \param   ecdf_vector    The vector of ecdf, which is the argument for the target function.
 #  \retval  target_val     The value of the target function.
 def evaluate_from_empirical_cumulative_distribution_functions( estimator, vector ):
   mean_deviation = np.subtract( estimator.mean_vector , vector )
   if not estimator.error_printed:
     try:
+      x = np.linalg.solve(estimator.covar_matrix, mean_deviation)
       return np.dot( mean_deviation , np.linalg.solve(estimator.covar_matrix, mean_deviation) )
     except np.linalg.LinAlgError as error:
       estimator.error_printed = True
       print("WARNING: Covariance matrix is singular. CIL_estimator uses different topology.")
   return np.dot( mean_deviation , mean_deviation )
```

### Comparing `ecdf_estimator-0.1.6/ecdf_estimator.egg-info/PKG-INFO` & `ecdf_estimator-0.1.7/ecdf_estimator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ecdf-estimator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for parameter estimation of random data
 Home-page: https://github.com/AndreasRupp/ecdf_estimator
 Author: Andreas Rupp
 Author-email: Andreas Rupp <info@rupp.ink>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/AndreasRupp/ecdf_estimator
 Project-URL: Bug Tracker, https://github.com/AndreasRupp/ecdf_estimator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11.6
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: matplotlib>=3.6
+Requires-Dist: numpy>=1.25.0
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: matplotlib>=3.7.1
 
 # Welcome to ecdf_estimator
 
 [![PyPI Version](https://badge.fury.io/py/ecdf_estimator.svg)](
 https://badge.fury.io/py/ecdf_estimator)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/ecdf_estimator.svg?label=PyPI%20downloads)](
 https://pypi.org/project/ecdf_estimator/)
```

### Comparing `ecdf_estimator-0.1.6/pyproject.toml` & `ecdf_estimator-0.1.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = [
   "setuptools == 68.2.2",
-  "numpy>=1.19.5",
-  "matplotlib>=3.6"
+  "numpy>=1.25.0",
+  "scipy>=1.10.1",
+  "matplotlib>=3.7.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ecdf_estimator"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Andreas Rupp", email="info@rupp.ink" },
 ]
 description = "Python package for parameter estimation of random data"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11.6"
 dependencies = [
-  "numpy>=1.19.5",
-  "matplotlib>=3.6"
+  "numpy>=1.25.0",
+  "scipy>=1.10.1",
+  "matplotlib>=3.7.1"
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
   "Operating System :: OS Independent",
 ]
```

### Comparing `ecdf_estimator-0.1.6/setup.py` & `ecdf_estimator-0.1.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import setuptools
+import sys
+
+if sys.version_info < (3,11):
+    sys.exit('Sorry, Python < 3.11 is not supported')
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name='ecdf_estimator',
-  version='0.1.6',
+  version='0.1.7',
   author='Andreas Rupp',
   author_email='info@rupp.ink',
   description='Python package for parameter estimation of random data',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/AndreasRupp/ecdf_estimator',
   project_urls = {
     "Bug Tracker": "https://github.com/AndreasRupp/ecdf_estimator/issues"
   },
   license='LGPL-2.1',
   packages=['ecdf_estimator'],
   install_requires=[
     'requests',
-    'numpy>=1.19.5',
-    'matplotlib>=3.6'
+    'numpy>=1.25.0',
+    'scipy>=1.10.1',
+    'matplotlib>=3.7.1'
   ],
 )
```

