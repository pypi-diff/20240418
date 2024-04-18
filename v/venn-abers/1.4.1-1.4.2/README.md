# Comparing `tmp/venn-abers-1.4.1.tar.gz` & `tmp/venn-abers-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venn-abers-1.4.1.tar", last modified: Wed Oct 18 05:19:38 2023, max compression
+gzip compressed data, was "venn-abers-1.4.2.tar", last modified: Thu Apr 18 16:15:59 2024, max compression
```

## Comparing `venn-abers-1.4.1.tar` & `venn-abers-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2023-10-18 05:19:38.377322 venn-abers-1.4.1/
--rw-r--r--   0 ivanpetej   (501) staff       (20)     1062 2023-08-28 14:02:08.000000 venn-abers-1.4.1/LICENSE.TXT
--rw-r--r--   0 ivanpetej   (501) staff       (20)     2856 2023-10-18 05:19:38.377405 venn-abers-1.4.1/PKG-INFO
--rw-r--r--   0 ivanpetej   (501) staff       (20)     2260 2023-08-28 15:49:32.000000 venn-abers-1.4.1/README.md
--rw-r--r--   0 ivanpetej   (501) staff       (20)       79 2023-10-18 05:19:38.377628 venn-abers-1.4.1/setup.cfg
--rw-r--r--   0 ivanpetej   (501) staff       (20)      902 2023-10-18 05:06:45.000000 venn-abers-1.4.1/setup.py
-drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2023-10-18 05:19:38.376329 venn-abers-1.4.1/src/
--rw-r--r--   0 ivanpetej   (501) staff       (20)       88 2023-08-28 14:19:29.000000 venn-abers-1.4.1/src/__init__.py
--rw-r--r--   0 ivanpetej   (501) staff       (20)      900 2023-10-15 19:32:06.000000 venn-abers-1.4.1/src/test.py
--rw-r--r--   0 ivanpetej   (501) staff       (20)    37127 2023-10-18 05:02:20.000000 venn-abers-1.4.1/src/venn_abers.py
-drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2023-10-18 05:19:38.377231 venn-abers-1.4.1/venn_abers.egg-info/
--rw-r--r--   0 ivanpetej   (501) staff       (20)     2856 2023-10-18 05:19:38.000000 venn-abers-1.4.1/venn_abers.egg-info/PKG-INFO
--rw-r--r--   0 ivanpetej   (501) staff       (20)      255 2023-10-18 05:19:38.000000 venn-abers-1.4.1/venn_abers.egg-info/SOURCES.txt
--rw-r--r--   0 ivanpetej   (501) staff       (20)        1 2023-10-18 05:19:38.000000 venn-abers-1.4.1/venn_abers.egg-info/dependency_links.txt
--rw-r--r--   0 ivanpetej   (501) staff       (20)       26 2023-10-18 05:19:38.000000 venn-abers-1.4.1/venn_abers.egg-info/requires.txt
--rw-r--r--   0 ivanpetej   (501) staff       (20)       11 2023-10-18 05:19:38.000000 venn-abers-1.4.1/venn_abers.egg-info/top_level.txt
+drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2024-04-18 16:15:59.504403 venn-abers-1.4.2/
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     1062 2023-08-28 14:02:08.000000 venn-abers-1.4.2/LICENSE.TXT
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     2856 2024-04-18 16:15:59.504466 venn-abers-1.4.2/PKG-INFO
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     2260 2023-08-28 15:49:32.000000 venn-abers-1.4.2/README.md
+-rw-r--r--   0 ivanpetej   (501) staff       (20)       79 2024-04-18 16:15:59.504736 venn-abers-1.4.2/setup.cfg
+-rw-r--r--   0 ivanpetej   (501) staff       (20)      902 2024-04-18 05:38:14.000000 venn-abers-1.4.2/setup.py
+drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2024-04-18 16:15:59.503023 venn-abers-1.4.2/src/
+-rw-r--r--   0 ivanpetej   (501) staff       (20)       88 2023-08-28 14:19:29.000000 venn-abers-1.4.2/src/__init__.py
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     3726 2024-04-11 16:33:12.000000 venn-abers-1.4.2/src/abbers_without_classifier.py
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     4714 2024-04-18 05:03:59.000000 venn-abers-1.4.2/src/test_one_one.py
+-rw-r--r--   0 ivanpetej   (501) staff       (20)    38764 2024-04-16 16:43:45.000000 venn-abers-1.4.2/src/venn_abers.py
+drwxr-xr-x   0 ivanpetej   (501) staff       (20)        0 2024-04-18 16:15:59.504309 venn-abers-1.4.2/venn_abers.egg-info/
+-rw-r--r--   0 ivanpetej   (501) staff       (20)     2856 2024-04-18 16:15:59.000000 venn-abers-1.4.2/venn_abers.egg-info/PKG-INFO
+-rw-r--r--   0 ivanpetej   (501) staff       (20)      296 2024-04-18 16:15:59.000000 venn-abers-1.4.2/venn_abers.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanpetej   (501) staff       (20)        1 2024-04-18 16:15:59.000000 venn-abers-1.4.2/venn_abers.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanpetej   (501) staff       (20)       26 2024-04-18 16:15:59.000000 venn-abers-1.4.2/venn_abers.egg-info/requires.txt
+-rw-r--r--   0 ivanpetej   (501) staff       (20)       11 2024-04-18 16:15:59.000000 venn-abers-1.4.2/venn_abers.egg-info/top_level.txt
```

### Comparing `venn-abers-1.4.1/LICENSE.TXT` & `venn-abers-1.4.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `venn-abers-1.4.1/PKG-INFO` & `venn-abers-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: venn-abers
-Version: 1.4.1
+Version: 1.4.2
 Summary: Venn-ABERS calibration package
 Home-page: https://github.com/ip200/venn-abers
-Download-URL: https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_1.tar.gz
+Download-URL: https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_2.tar.gz
 Author: Ivan Petej
 Author-email: ivan.petej@gmail.com
 License: MIT
 Keywords: Probabilistic classification,calibration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `venn-abers-1.4.1/README.md` & `venn-abers-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `venn-abers-1.4.1/setup.py` & `venn-abers-1.4.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
   name='venn-abers',
   packages=['venn_abers'],
   package_dir={'venn_abers': 'src'},
-  version='1.4.1',
+  version='1.4.2',
   license='MIT',
   description='Venn-ABERS calibration package',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Ivan Petej',
   author_email='ivan.petej@gmail.com',
   url='https://github.com/ip200/venn-abers',
-  download_url='https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_1.tar.gz',
+  download_url='https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_2.tar.gz',
   keywords=['Probabilistic classification', 'calibration'],
   install_requires=[
           'numpy',
           'scikit-learn',
           'pandas'
       ],
   classifiers=[
```

### Comparing `venn-abers-1.4.1/src/venn_abers.py` & `venn-abers-1.4.2/src/venn_abers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 from sklearn.model_selection import StratifiedKFold, train_test_split
 from sklearn.multiclass import OneVsOneClassifier
-from sklearn.utils.validation import check_is_fitted
+from sklearn.utils.validation import check_is_fitted, check_X_y, check_array
 from sklearn.exceptions import NotFittedError
+from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn.utils.multiclass import unique_labels
 import pandas as pd
 
 np.seterr(divide='ignore', invalid='ignore')
 
 
 def calc_p0p1(p_cal, y_cal, precision=None):
     """Function that calculates isotonic calibration vectors required for Venn-ABERS calibration
@@ -213,14 +215,52 @@
     for c in missing_cols:
         _x_test_df[c] = 0
 
     _x_test_df = _x_test_df[train_columns]
 
     return _x_test_df.values
 
+
+def predict_proba_prefitted_va(p_cal, y_cal, p_test, precision=None):
+    classes = np.unique(y_cal)
+    class_pairs = []
+    for i in range(len(classes) - 1):
+        for j in range(i + 1, len(classes)):
+            class_pairs.append([i, j])
+
+    multiclass_probs = []
+    multiclass_p0p1 = []
+    for i, class_pair in enumerate(class_pairs):
+        pairwise_indices = (y_cal == class_pair[0]) + (y_cal == class_pair[1])
+        binary_cal_probs = p_cal[:, class_pair][pairwise_indices] / np.sum(p_cal[:, class_pair][pairwise_indices],
+                                                                           axis=1).reshape(-1, 1)
+        binary_test_probs = p_test[:, class_pair] / np.sum(p_test[:, class_pair], axis=1).reshape(-1, 1)
+        binary_classes = y_cal[pairwise_indices] == class_pair[1]
+
+        va = VennAbers()
+        va.fit(binary_cal_probs, binary_classes, precision=precision)
+        p_pr, p0_p1 = va.predict_proba(binary_test_probs)
+        multiclass_probs.append(p_pr)
+        multiclass_p0p1.append(p0_p1)
+
+    p_prime = np.zeros((len(p_test), len(classes)))
+
+    for i, cl_id, in enumerate(classes):
+        stack_i = [
+            p[:, 0].reshape(-1, 1) for i, p in enumerate(multiclass_probs) if class_pairs[i][0] == cl_id]
+        stack_j = [
+            p[:, 1].reshape(-1, 1) for i, p in enumerate(multiclass_probs) if class_pairs[i][1] == cl_id]
+        p_stack = stack_i + stack_j
+
+        p_prime[:, i] = 1 / (np.sum(np.hstack([(1 / p) for p in p_stack]), axis=1) - (len(classes) - 2))
+
+    p_prime = p_prime / np.sum(p_prime, axis=1).reshape(-1, 1)
+
+    return p_prime, multiclass_p0p1
+
 class VennAbers:
     """Implementation of the Venn-ABERS calibration for binary classification problems. Venn-ABERS calibration is a
         method of turning machine learning classification algorithms into probabilistic predictors
         that automatically enjoys a property of validity (perfect calibration) and is computationally efficient.
         The algorithm is described in [1].
 
 
@@ -327,15 +367,15 @@
             (https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html).
             If float, should be between 0.0 and 1.0 and represent the proportion
             of the dataset to include in the proper training / calibration split.
             If int, represents the absolute number of test samples. If None, the
             value is set to the complement of the train size. If ``train_size``
             is also None, it will be set to 0.25.
 
-        train_size : float or int, default=None
+        train_proper_size : float or int, default=None
             For IVAP only, if float, should be between 0.0 and 1.0 and represent the
             proportion of the dataset to include in the poroper training set split. If
             int, represents the absolute number of train samples. If None,
             the value is automatically set to the complement of the test size.
 
         random_state : int, RandomState instance or None, default=None
             Controls the shuffling applied to the data before applying the split.
@@ -385,28 +425,24 @@
             Input data for calibration consisting of training set numerical features
 
         _y_train : {array-like}, shape (n_samples,)
             Associated binary class labels.
         """
         if self.inductive:
             self.n_splits = 1
-            try:
-                check_is_fitted(self.estimator)
-                x_cal, y_cal = _x_train, _y_train
-            except NotFittedError:
-                x_train_proper, x_cal, y_train_proper, y_cal = train_test_split(
-                    _x_train,
-                    _y_train,
-                    test_size=self.cal_size,
-                    train_size=self.train_proper_size,
-                    random_state=self.random_state,
-                    shuffle=self.shuffle,
-                    stratify=self.stratify
-                )
-                self.estimator.fit(x_train_proper, y_train_proper.flatten())
+            x_train_proper, x_cal, y_train_proper, y_cal = train_test_split(
+                _x_train,
+                _y_train,
+                test_size=self.cal_size,
+                train_size=self.train_proper_size,
+                random_state=self.random_state,
+                shuffle=self.shuffle,
+                stratify=self.stratify
+            )
+            self.estimator.fit(x_train_proper, y_train_proper.flatten())
             clf_prob = self.estimator.predict_proba(x_cal)
             self.clf_p_cal.append(clf_prob)
             self.clf_y_cal.append(y_cal)
         else:
             kf = StratifiedKFold(n_splits=self.n_splits, shuffle=self.shuffle, random_state=self.random_state)
             for train_index, test_index in kf.split(_x_train, _y_train):
                 self.estimator.fit(_x_train[train_index], _y_train[train_index].flatten())
@@ -805,15 +841,15 @@
 
     def predict_proba(self, _x_test=None, p_cal=None, y_cal=None, p_test=None, loss='log', p0_p1_output=False):
         """ Generates Venn-ABERS calibrated probabilities.
 
             Parameters
             ----------
             _x_test : {array-like}, shape (n_samples,)
-                Training set numerical or cartegorical features (only for IVAP and CVAP when underlying classsifier
+                Training set numerical or categorical features (only for IVAP and CVAP when underlying classifier
                 is provided to fit). If categorical, features are one hot encoded using pandas.get_dummies()
 
             p_cal = {array-like}, shape (n_samples,)
                 Calibration set probabilities  (Manual Venn-ABERS only)
 
             y_cal = {array-like}, shape (n_samples,)
                 Calibration set labels (Manual Venn-ABERS only)
@@ -827,30 +863,33 @@
 
             p0_p1_output: bool, default = False
                 If True, function also returns p0_p1 probabilistic outputs for binary classification problems
                 (for manual Venn-ABERS only)
 
             Returns
             ----------
-            p_prime: {array-like}, shape (n_samples,n_classses)
+            p_prime: {array-like}, shape (n_samples, n_classes)
                 Venn-ABERS calibrated probabilities
         """
+
         if p_cal is None and self.estimator is None:
             raise Exception("Please provide either an underlying algorithm or a calibration set")
         if self.estimator is None:
-            if len(np.unique(y_cal)) > 2:
-                raise Exception("Venn ABERS without an underlying classifier \
-                                currently only available for binary classification problems")
-            elif p_cal is None or y_cal is None:
+            if p_cal is None or y_cal is None:
                 raise Exception("Please provide both a set of calibration probabilities and class labels to calibrate")
             elif p_test is None:
                 raise Exception("Please provide a set of test probabilities to calibrate")
-            va = VennAbers()
-            va.fit(p_cal, y_cal, self.precision)
-            p_prime, p0_p1 = va.predict_proba(p_test)
+            if len(np.unique(y_cal)) <= 2:
+                self.classes = np.unique(y_cal)
+                va = VennAbers()
+                va.fit(p_cal, y_cal, self.precision)
+                p_prime, p0_p1 = va.predict_proba(p_test)
+            else:
+                self.classes = np.unique(y_cal)
+                p_prime, p0_p1 = predict_proba_prefitted_va(p_cal, y_cal, p_test, precision=self.precision)
         else:
             if _x_test is None:
                 raise Exception("Please provide a feature test set to generate calibrated predictions")
 
             _x_test = adjust_categorical_test(self.train_columns, _x_test)
 
             p_prime = self.va_calibrator.predict_proba(_x_test, loss=loss)
@@ -863,15 +902,15 @@
 
     def predict(self, _x_test=None, p_cal=None, y_cal=None, p_test=None, loss='log', one_hot=True):
         """ Generates Venn-ABERS calibrated prediction labels.
 
                 Parameters
                 ----------
                 _x_test : {array-like}, shape (n_samples,)
-                    Training set numerical or vategorical features (only for IVAP and CVAP when underlying classsifier
+                    Training set numerical or categorical features (only for IVAP and CVAP when underlying classsifier
                     is provided to fit). If categorical, features are one hot encoded using pandas.get_dummies()
 
                 p_cal = {array-like}, shape (n_samples,)
                     Calibration set probabilities  (Manual Venn-ABERS only)
 
                 y_cal = {array-like}, shape (n_samples,)
                     Calibration set labels (Manual Venn-ABERS only)
```

### Comparing `venn-abers-1.4.1/venn_abers.egg-info/PKG-INFO` & `venn-abers-1.4.2/venn_abers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: venn-abers
-Version: 1.4.1
+Version: 1.4.2
 Summary: Venn-ABERS calibration package
 Home-page: https://github.com/ip200/venn-abers
-Download-URL: https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_1.tar.gz
+Download-URL: https://github.com/ip200/venn-abers/archive/refs/tags/v1_4_2.tar.gz
 Author: Ivan Petej
 Author-email: ivan.petej@gmail.com
 License: MIT
 Keywords: Probabilistic classification,calibration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

