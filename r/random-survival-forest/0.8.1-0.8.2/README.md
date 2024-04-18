# Comparing `tmp/random_survival_forest-0.8.1.tar.gz` & `tmp/random_survival_forest-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_survival_forest-0.8.1.tar", last modified: Wed Oct 19 07:41:57 2022, max compression
+gzip compressed data, was "dist/random_survival_forest-0.8.2.tar", last modified: Thu Apr 18 15:03:31 2024, max compression
```

## Comparing `random_survival_forest-0.8.1.tar` & `random_survival_forest-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-10-19 07:41:57.194404 random_survival_forest-0.8.1/
--rw-r--r--   0 spaethju   (501) staff       (20)     1057 2022-04-20 20:45:39.000000 random_survival_forest-0.8.1/LICENSE.txt
--rw-r--r--   0 spaethju   (501) staff       (20)     2609 2022-10-19 07:41:57.194497 random_survival_forest-0.8.1/PKG-INFO
--rw-r--r--   0 spaethju   (501) staff       (20)     1759 2022-10-18 12:54:44.000000 random_survival_forest-0.8.1/README.md
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-10-19 07:41:57.193476 random_survival_forest-0.8.1/random_survival_forest/
--rw-r--r--   0 spaethju   (501) staff       (20)      276 2022-10-18 12:48:41.000000 random_survival_forest-0.8.1/random_survival_forest/__init__.py
--rw-r--r--   0 spaethju   (501) staff       (20)    13430 2022-10-18 12:55:52.000000 random_survival_forest-0.8.1/random_survival_forest/models.py
--rw-r--r--   0 spaethju   (501) staff       (20)     2628 2022-04-20 20:45:39.000000 random_survival_forest-0.8.1/random_survival_forest/scoring.py
--rw-r--r--   0 spaethju   (501) staff       (20)     2813 2022-05-01 20:14:57.000000 random_survival_forest-0.8.1/random_survival_forest/splitting.py
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-10-19 07:41:57.194279 random_survival_forest-0.8.1/random_survival_forest.egg-info/
--rw-r--r--   0 spaethju   (501) staff       (20)     2609 2022-10-19 07:41:57.000000 random_survival_forest-0.8.1/random_survival_forest.egg-info/PKG-INFO
--rw-r--r--   0 spaethju   (501) staff       (20)      407 2022-10-19 07:41:57.000000 random_survival_forest-0.8.1/random_survival_forest.egg-info/SOURCES.txt
--rw-r--r--   0 spaethju   (501) staff       (20)        1 2022-10-19 07:41:57.000000 random_survival_forest-0.8.1/random_survival_forest.egg-info/dependency_links.txt
--rw-r--r--   0 spaethju   (501) staff       (20)       56 2022-10-19 07:41:57.000000 random_survival_forest-0.8.1/random_survival_forest.egg-info/requires.txt
--rw-r--r--   0 spaethju   (501) staff       (20)       23 2022-10-19 07:41:57.000000 random_survival_forest-0.8.1/random_survival_forest.egg-info/top_level.txt
--rw-r--r--   0 spaethju   (501) staff       (20)      148 2022-10-19 07:41:57.194820 random_survival_forest-0.8.1/setup.cfg
--rw-r--r--   0 spaethju   (501) staff       (20)     1216 2022-10-19 07:41:26.000000 random_survival_forest-0.8.1/setup.py
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2024-04-18 15:03:31.633705 random_survival_forest-0.8.2/
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2024-04-18 15:03:31.611618 random_survival_forest-0.8.2/.github/
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2024-04-18 15:03:31.615129 random_survival_forest-0.8.2/.github/workflows/
+-rw-r--r--   0 spaethju   (501) staff       (20)      669 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/.github/workflows/pylint.yml
+-rw-r--r--   0 spaethju   (501) staff       (20)     1222 2024-04-18 14:56:51.000000 random_survival_forest-0.8.2/.gitignore
+-rw-r--r--   0 spaethju   (501) staff       (20)      267 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/CITATION.cff
+-rw-r--r--   0 spaethju   (501) staff       (20)     1057 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/LICENSE.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)     3175 2024-04-18 15:03:31.633556 random_survival_forest-0.8.2/PKG-INFO
+-rw-r--r--   0 spaethju   (501) staff       (20)     2179 2024-04-18 14:56:51.000000 random_survival_forest-0.8.2/README.md
+-rw-r--r--   0 spaethju   (501) staff       (20)      237 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/build.sh
+-rw-r--r--   0 spaethju   (501) staff       (20)      847 2024-04-18 14:56:51.000000 random_survival_forest-0.8.2/example.py
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2024-04-18 15:03:31.616829 random_survival_forest-0.8.2/random_survival_forest/
+-rw-r--r--   0 spaethju   (501) staff       (20)      292 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/random_survival_forest/__init__.py
+-rw-r--r--   0 spaethju   (501) staff       (20)    13433 2024-04-18 14:56:51.000000 random_survival_forest-0.8.2/random_survival_forest/models.py
+-rw-r--r--   0 spaethju   (501) staff       (20)     2628 2024-04-16 12:18:01.000000 random_survival_forest-0.8.2/random_survival_forest/scoring.py
+-rw-r--r--   0 spaethju   (501) staff       (20)     2919 2024-04-18 14:56:51.000000 random_survival_forest-0.8.2/random_survival_forest/splitting.py
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2024-04-18 15:03:31.633159 random_survival_forest-0.8.2/random_survival_forest.egg-info/
+-rw-r--r--   0 spaethju   (501) staff       (20)     3175 2024-04-18 15:03:31.000000 random_survival_forest-0.8.2/random_survival_forest.egg-info/PKG-INFO
+-rw-r--r--   0 spaethju   (501) staff       (20)      497 2024-04-18 15:03:31.000000 random_survival_forest-0.8.2/random_survival_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)        1 2024-04-18 15:03:31.000000 random_survival_forest-0.8.2/random_survival_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)       56 2024-04-18 15:03:31.000000 random_survival_forest-0.8.2/random_survival_forest.egg-info/requires.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)       23 2024-04-18 15:03:31.000000 random_survival_forest-0.8.2/random_survival_forest.egg-info/top_level.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)       55 2023-01-31 14:45:20.000000 random_survival_forest-0.8.2/requirements.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)      148 2024-04-18 15:03:31.635612 random_survival_forest-0.8.2/setup.cfg
+-rw-r--r--   0 spaethju   (501) staff       (20)     1216 2024-04-18 15:03:19.000000 random_survival_forest-0.8.2/setup.py
```

### Comparing `random_survival_forest-0.8.1/LICENSE.txt` & `random_survival_forest-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `random_survival_forest-0.8.1/PKG-INFO` & `random_survival_forest-0.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random_survival_forest
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Random Survival Forest implementation inspired by Ishwaran et al.
 Home-page: https://github.com/julianspaeth/random-survival-forest
 Download-URL: https://github.com/julianspaeth/random-survival-forest/archive/v0.1-beta.tar.gz
 Author: Julian Späth
 Author-email: spaethju@posteo.de
 License: MIT License
 Keywords: survival-analysis,survival-prediction,machine-learning,random-forest,random-survival-forest
@@ -12,14 +12,20 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: joblib
+Requires-Dist: multiprocess
+Requires-Dist: lifelines
+Requires-Dist: scikit-learn
 
 # Random Survival Forest
 
 [![DOI](https://zenodo.org/badge/201053930.svg)](https://zenodo.org/badge/latestdoi/201053930)
 
 The Random Survival Forest package provides a python implementation of the survival prediction method originally published by Ishwaran et al. (2008).
 
@@ -33,44 +39,52 @@
 $ pip install random-survival-forest
 ```
 
 ## Contribute
 
 - Source Code: https://github.com/julianspaeth/random-survival-forest
 
+## Performance
+This implemention is not optimized for being highly performant. It is programmed in pure python. If you have large datasets (large sample size) or use a very high number of trees, I suggest using the scikit-survival package.
+
+
 ## Getting Started
 
 ```python
-from random_survival_forest.models import RandomSurvivalForest
-from random_survival_forest.scoring import concordance_index
+import time
+
 from lifelines import datasets
 from sklearn.model_selection import train_test_split
 
+from random_survival_forest.models import RandomSurvivalForest
+from random_survival_forest.scoring import concordance_index
 
 rossi = datasets.load_rossi()
-# Attention: duration column must be index 0, event column index 1 in y
-y = rossi.loc[:, ["week", "arrest"]]
+# Attention: duration column (time until event occurs) must be index 1, event column index 0 in y
+y = rossi.loc[:, ["arrest", "week"]]
 X = rossi.drop(["arrest", "week"], axis=1)
-X, X_test, y, y_test = train_test_split(X, y, test_size=0.25)
-
+X, X_test, y, y_test = train_test_split(X, y, test_size=0.33, random_state=10)
 
-rsf = RandomSurvivalForest(n_estimators=20, n_jobs=-1)
+print("Start training...")
+start_time = time.time()
+rsf = RandomSurvivalForest(n_estimators=10, n_jobs=-1, random_state=10)
 rsf = rsf.fit(X, y)
+print(f'--- {round(time.time() - start_time, 3)} seconds ---')
 y_pred = rsf.predict(X_test)
 c_val = concordance_index(y_time=y_test["week"], y_pred=y_pred, y_event=y_test["arrest"])
-print("C-index", round(c_val, 3))
+print(f'C-index {round(c_val, 3)}')
 ```
 
 ## Feedback
 
 If you are having issues or feedback, please let me know. I am happy to fix some bug or implement feature requests.
 
 julian.alexander.spaeth@uni-hamburg..de
 
-This package is completely open-source. If it helped you or you even use it comercially, I would be happy about a little support:
+This package is open-source. If it helped you or you even use it comercially, I would be happy about a little support:
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/julianspaeth)
 
 ## License
 MIT
```

### Comparing `random_survival_forest-0.8.1/README.md` & `random_survival_forest-0.8.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -14,44 +14,52 @@
 $ pip install random-survival-forest
 ```
 
 ## Contribute
 
 - Source Code: https://github.com/julianspaeth/random-survival-forest
 
+## Performance
+This implemention is not optimized for being highly performant. It is programmed in pure python. If you have large datasets (large sample size) or use a very high number of trees, I suggest using the scikit-survival package.
+
+
 ## Getting Started
 
 ```python
-from random_survival_forest.models import RandomSurvivalForest
-from random_survival_forest.scoring import concordance_index
+import time
+
 from lifelines import datasets
 from sklearn.model_selection import train_test_split
 
+from random_survival_forest.models import RandomSurvivalForest
+from random_survival_forest.scoring import concordance_index
 
 rossi = datasets.load_rossi()
-# Attention: duration column must be index 0, event column index 1 in y
-y = rossi.loc[:, ["week", "arrest"]]
+# Attention: duration column (time until event occurs) must be index 1, event column index 0 in y
+y = rossi.loc[:, ["arrest", "week"]]
 X = rossi.drop(["arrest", "week"], axis=1)
-X, X_test, y, y_test = train_test_split(X, y, test_size=0.25)
-
+X, X_test, y, y_test = train_test_split(X, y, test_size=0.33, random_state=10)
 
-rsf = RandomSurvivalForest(n_estimators=20, n_jobs=-1)
+print("Start training...")
+start_time = time.time()
+rsf = RandomSurvivalForest(n_estimators=10, n_jobs=-1, random_state=10)
 rsf = rsf.fit(X, y)
+print(f'--- {round(time.time() - start_time, 3)} seconds ---')
 y_pred = rsf.predict(X_test)
 c_val = concordance_index(y_time=y_test["week"], y_pred=y_pred, y_event=y_test["arrest"])
-print("C-index", round(c_val, 3))
+print(f'C-index {round(c_val, 3)}')
 ```
 
 ## Feedback
 
 If you are having issues or feedback, please let me know. I am happy to fix some bug or implement feature requests.
 
 julian.alexander.spaeth@uni-hamburg..de
 
-This package is completely open-source. If it helped you or you even use it comercially, I would be happy about a little support:
+This package is open-source. If it helped you or you even use it comercially, I would be happy about a little support:
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/julianspaeth)
 
 ## License
 MIT
```

### Comparing `random_survival_forest-0.8.1/random_survival_forest/models.py` & `random_survival_forest-0.8.2/random_survival_forest/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         except Exception:
             raise (
                 "Timeline seems to contain float values. Please provide a custom timeline in the RandomSurvivalForest "
                 "constructor. "
                 "For example: RandomSurivalForest(timeline=range(y.iloc[:, 1].min(), y.iloc[:, 1].max(), 0.1)")
 
         self.bootstrap_idxs = self._draw_bootstrap_samples(x)
-
         num_cores = multiprocessing.cpu_count()
 
         if self.n_jobs > num_cores or self.n_jobs == -1:
             self.n_jobs = num_cores
         elif self.n_jobs is None:
             self.n_jobs = 1
 
@@ -70,15 +69,15 @@
                 self.bootstraps.append(self.bootstrap_idxs[i])
 
         if self.oob_score:
             self.oob_score = self.compute_oob_score(x, y)
 
         return self
 
-    def _create_tree(self, x, y, i: list):
+    def _create_tree(self, x, y, i):
         """
         Grows a survival tree for the bootstrap samples.
         :param y: label data frame y with survival time as the first column and event as second
         :param x: feature data frame x
         :param i: Indices
         :return: SurvivalTree
         """
@@ -195,15 +194,15 @@
         self.grow_tree()
 
     def grow_tree(self):
         """
         Grow the survival tree recursively as nodes.
         :return: self
         """
-        unique_deaths = self.y.iloc[:, 0].reset_index().drop_duplicates().sum()[1]
+        unique_deaths = self.y.iloc[:, 0].reset_index().drop_duplicates().sum().iloc[1]
 
         self.score, self.split_val, self.split_var, lhs_idxs_opt, rhs_idxs_opt = _find_split(self)
 
         if self.split_var is not None and unique_deaths > self.unique_deaths:
             self.prediction_possible = True
             lf_idxs, rf_idxs = _select_new_feature_indices(self.x, self.n_features, self.random_instance)
 
@@ -270,15 +269,15 @@
         self.grow_tree()
 
     def grow_tree(self):
         """
         Grow tree by calculating the Nodes recursively.
         :return: self
         """
-        unique_deaths = self.y.iloc[:, 0].reset_index().drop_duplicates().sum()[1]
+        unique_deaths = self.y.iloc[:, 0].reset_index().drop_duplicates().sum().iloc[1]
 
         if unique_deaths <= self.unique_deaths:
             self.compute_terminal_node()
             return self
 
         self.score, self.split_val, self.split_var, lhs_idxs_opt, rhs_idxs_opt = _find_split(self)
```

### Comparing `random_survival_forest-0.8.1/random_survival_forest/scoring.py` & `random_survival_forest-0.8.2/random_survival_forest/scoring.py`

 * *Files identical despite different names*

### Comparing `random_survival_forest-0.8.1/random_survival_forest.egg-info/PKG-INFO` & `random_survival_forest-0.8.2/random_survival_forest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: random-survival-forest
-Version: 0.8.1
+Name: random_survival_forest
+Version: 0.8.2
 Summary: A Random Survival Forest implementation inspired by Ishwaran et al.
 Home-page: https://github.com/julianspaeth/random-survival-forest
 Download-URL: https://github.com/julianspaeth/random-survival-forest/archive/v0.1-beta.tar.gz
 Author: Julian Späth
 Author-email: spaethju@posteo.de
 License: MIT License
 Keywords: survival-analysis,survival-prediction,machine-learning,random-forest,random-survival-forest
@@ -12,14 +12,20 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: joblib
+Requires-Dist: multiprocess
+Requires-Dist: lifelines
+Requires-Dist: scikit-learn
 
 # Random Survival Forest
 
 [![DOI](https://zenodo.org/badge/201053930.svg)](https://zenodo.org/badge/latestdoi/201053930)
 
 The Random Survival Forest package provides a python implementation of the survival prediction method originally published by Ishwaran et al. (2008).
 
@@ -33,44 +39,52 @@
 $ pip install random-survival-forest
 ```
 
 ## Contribute
 
 - Source Code: https://github.com/julianspaeth/random-survival-forest
 
+## Performance
+This implemention is not optimized for being highly performant. It is programmed in pure python. If you have large datasets (large sample size) or use a very high number of trees, I suggest using the scikit-survival package.
+
+
 ## Getting Started
 
 ```python
-from random_survival_forest.models import RandomSurvivalForest
-from random_survival_forest.scoring import concordance_index
+import time
+
 from lifelines import datasets
 from sklearn.model_selection import train_test_split
 
+from random_survival_forest.models import RandomSurvivalForest
+from random_survival_forest.scoring import concordance_index
 
 rossi = datasets.load_rossi()
-# Attention: duration column must be index 0, event column index 1 in y
-y = rossi.loc[:, ["week", "arrest"]]
+# Attention: duration column (time until event occurs) must be index 1, event column index 0 in y
+y = rossi.loc[:, ["arrest", "week"]]
 X = rossi.drop(["arrest", "week"], axis=1)
-X, X_test, y, y_test = train_test_split(X, y, test_size=0.25)
-
+X, X_test, y, y_test = train_test_split(X, y, test_size=0.33, random_state=10)
 
-rsf = RandomSurvivalForest(n_estimators=20, n_jobs=-1)
+print("Start training...")
+start_time = time.time()
+rsf = RandomSurvivalForest(n_estimators=10, n_jobs=-1, random_state=10)
 rsf = rsf.fit(X, y)
+print(f'--- {round(time.time() - start_time, 3)} seconds ---')
 y_pred = rsf.predict(X_test)
 c_val = concordance_index(y_time=y_test["week"], y_pred=y_pred, y_event=y_test["arrest"])
-print("C-index", round(c_val, 3))
+print(f'C-index {round(c_val, 3)}')
 ```
 
 ## Feedback
 
 If you are having issues or feedback, please let me know. I am happy to fix some bug or implement feature requests.
 
 julian.alexander.spaeth@uni-hamburg..de
 
-This package is completely open-source. If it helped you or you even use it comercially, I would be happy about a little support:
+This package is open-source. If it helped you or you even use it comercially, I would be happy about a little support:
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/julianspaeth)
 
 ## License
 MIT
```

### Comparing `random_survival_forest-0.8.1/setup.py` & `random_survival_forest-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='random_survival_forest',
     packages=['random_survival_forest'],
-    version='0.8.1',
+    version='0.8.2',
     license="MIT License",
     long_description=readme,
     long_description_content_type="text/markdown",
     description='A Random Survival Forest implementation inspired by Ishwaran et al.',
     author='Julian Späth',
     author_email='spaethju@posteo.de',
     url='https://github.com/julianspaeth/random-survival-forest',
```

