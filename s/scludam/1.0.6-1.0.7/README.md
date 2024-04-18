# Comparing `tmp/scludam-1.0.6-py3-none-any.whl.zip` & `tmp/scludam-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 124531 bytes, number of entries: 33
+Zip file size: 125465 bytes, number of entries: 33
 -rw-rw-r--  2.0 unx     2230 b- defN 24-Apr-14 22:09 scludam/__init__.py
 -rw-rw-r--  2.0 unx     1222 b- defN 24-Apr-15 23:06 scludam/cli.py
--rw-rw-r--  2.0 unx    14538 b- defN 24-Apr-15 23:47 scludam/cli_analysis.py
+-rw-rw-r--  2.0 unx    14548 b- defN 24-Apr-17 01:24 scludam/cli_analysis.py
 -rw-rw-r--  2.0 unx     6933 b- defN 24-Apr-15 23:52 scludam/cli_input.py
 -rw-rw-r--  2.0 unx    12391 b- defN 24-Apr-15 23:45 scludam/cli_utils.py
 -rw-rw-r--  2.0 unx    38242 b- defN 23-Nov-30 22:54 scludam/detection.py
 -rw-rw-r--  2.0 unx    24162 b- defN 22-Nov-12 22:56 scludam/fetcher.py
--rw-rw-r--  2.0 unx    29858 b- defN 24-Apr-15 23:31 scludam/hkde.py
+-rw-rw-r--  2.0 unx    31455 b- defN 24-Apr-18 01:35 scludam/hkde.py
 -rw-rw-r--  2.0 unx     7447 b- defN 22-Oct-08 02:29 scludam/masker.py
 -rw-rw-r--  2.0 unx    18095 b- defN 23-Nov-30 23:23 scludam/membership.py
--rw-rw-r--  2.0 unx    22184 b- defN 23-Nov-30 23:23 scludam/pipeline.py
+-rw-rw-r--  2.0 unx    24182 b- defN 24-Apr-17 23:38 scludam/pipeline.py
 -rw-rw-r--  2.0 unx    28380 b- defN 23-Nov-30 23:41 scludam/plots.py
 -rw-rw-r--  2.0 unx     4816 b- defN 23-Jun-25 22:01 scludam/rutils.py
 -rw-rw-r--  2.0 unx    31030 b- defN 23-Jun-25 22:01 scludam/shdbscan.py
 -rw-rw-r--  2.0 unx    23021 b- defN 23-Jun-25 13:46 scludam/stat_tests.py
 -rw-rw-r--  2.0 unx    38632 b- defN 22-Jul-13 00:03 scludam/synthetic.py
 -rw-rw-r--  2.0 unx     2609 b- defN 22-Nov-12 22:56 scludam/type_utils.py
 -rw-rw-r--  2.0 unx     7928 b- defN 23-Jun-25 21:59 scludam/utils.py
@@ -23,13 +23,13 @@
 -rw-rw-r--  2.0 unx     9993 b- defN 23-Jun-25 22:01 tests/test_membership.py
 -rw-rw-r--  2.0 unx    10177 b- defN 23-Jun-25 22:01 tests/test_pipeline.py
 -rw-rw-r--  2.0 unx    17500 b- defN 22-Jul-13 00:03 tests/test_shdbscan.py
 -rw-rw-r--  2.0 unx     5054 b- defN 22-Dec-16 04:18 tests/test_stat_tests.py
 -rw-rw-r--  2.0 unx    16673 b- defN 22-Jun-09 03:55 tests/test_synthetic.py
 -rw-rw-r--  2.0 unx     3009 b- defN 22-Aug-27 02:10 tests/test_utils.py
 -rw-rw-r--  2.0 unx      611 b- defN 22-Jul-13 00:03 tests/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-16 00:02 scludam-1.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5384 b- defN 24-Apr-16 00:02 scludam-1.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 00:02 scludam-1.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 24-Apr-16 00:02 scludam-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-16 00:02 scludam-1.0.6.dist-info/RECORD
-33 files, 469629 bytes uncompressed, 120591 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-18 13:40 scludam-1.0.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5384 b- defN 24-Apr-18 13:40 scludam-1.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 13:40 scludam-1.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-Apr-18 13:40 scludam-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-18 13:40 scludam-1.0.7.dist-info/RECORD
+33 files, 473234 bytes uncompressed, 121525 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -78,23 +78,23 @@
 
 Filename: tests/test_utils.py
 Comment: 
 
 Filename: tests/utils.py
 Comment: 
 
-Filename: scludam-1.0.6.dist-info/LICENSE
+Filename: scludam-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: scludam-1.0.6.dist-info/METADATA
+Filename: scludam-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: scludam-1.0.6.dist-info/WHEEL
+Filename: scludam-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: scludam-1.0.6.dist-info/top_level.txt
+Filename: scludam-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: scludam-1.0.6.dist-info/RECORD
+Filename: scludam-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scludam/cli_analysis.py

```diff
@@ -35,15 +35,15 @@
             f"Select the bin shape estimation method for {var}:",
             options,
             values,
             default_index=0,
             custom_prompt="Enter custom bandwidth as comma separated numbers (e.g. 0.1,0.2,0.3):",
         )
         if type(selected) == str:
-            return selected.split(",").remove(" ")
+            return selected.replace(" ", "").split(",")
         else:
             return selected
 
     pm_bin_shapes_to_try = select_auto_bin_shape_to_try("pm", [.3, .4, .5, .6, .7, .8, .9, 1])
     parallax_bin_shapes_to_try = select_auto_bin_shape_to_try("parallax", [.01, .02, .03, .04, .05, .06, .07, .08, .09, .1])
 
     min_score = prompt_cli_int_input("Enter the minimum score to consider a peak:", default=1)
@@ -137,15 +137,15 @@
             "Select the columns to be used for detection:",
             [gaia3params['label'], gaia2params['label']],
             [gaia3params['columns'], gaia2params['columns']],
             default_index=0,
             custom_prompt="Enter columns separated by commas:",
         )
         if type(selected) == str:
-            return selected.split(",").remove(" ")
+            return selected.replace(" ", "").split(",")
         else:
             return selected
     det_cols = select_detection_columns()
 
     # parameters
     selected = prompt_cli_selector(
         "Select the bin shape estimation method:",
```

## scludam/hkde.py

```diff
@@ -52,14 +52,16 @@
     NumericArray,
     OptionalNumeric1DArrayLike,
     OptionalNumeric2DArray,
     OptionalNumericArray,
     _type,
 )
 
+from tqdm import tqdm
+
 disable_r_warnings()
 disable_r_console_output()
 load_r_packages(r, ["ks"])
 
 
 class BandwidthSelector:
     """Base class for bandwidth selector."""
@@ -558,53 +560,67 @@
 
     def _calculate_biggest_hypersphere(self):
         
         def _get_biggest_cov_that_still_contributes(self, percentile):
             # If sum of diagonal is bigger when correlations are small, then matrix is bigger
             # get the self._covariances matrix which diagonal sums the biggest
             sums = np.array([np.diagonal(cc).sum() for cc in self._covariances])
-            # get the a certain percentile of the sums
-            # the bigger, the more "precise" the result
+            # get a certain percentile of the sums, because biggest sum tends to be
+            # exceptionally big, and will result in no benefit from
+            # using ball tree
+            # the bigger, the more "precise" the result, because it takes into
+            # account more contributions.
             # the smaller, the more "skips" in the calculation, the faster it runs
-            biggest_cov = np.percentile(sums, percentile)
-            closest_cov = np.argmin(np.abs(sums - biggest_cov))
-            # get the index of the biggest matrix
-            biggest_matrix = self._covariances[closest_cov]
-            # get the biggest matrix
+            biggest_sum = np.percentile(sums, percentile)
+            # abs(sums - biggest_sum) gets the distance between the biggest_cov and all the sums
+            # so as to get the index of the corresponding matrix
+            biggest_matrix_index = np.argmin(np.abs(sums - biggest_sum))
+            biggest_matrix = self._covariances[biggest_matrix_index]
+
             # create a multivariate normal around 0 with the biggest matrix, accounting for dims
             biggest_kde = multivariate_normal(
                 np.zeros(self._d),
                 biggest_matrix,
             )
-            # determine where the pdf is <= 1e-08 in all dimensions
+            # determine the furhtest point where the pdf turns to "practical 0",
+            # that is, <= 1e-08 in all dimensions
             # and take the distance between 0 and that point
-            # as the radius of the biggest sphere
+            # as the radius of the biggest needed sphere
             grid_range = (-3, 3)
+            # a bigger resolution is impractical for dim 5 or more
             resolution = 10
             threshold = 1e-08
             grid_linspace = np.linspace(grid_range[0], grid_range[1], resolution)
             dim = self._d
+            # get the points as list of coordinates instead of meshgrid
             points = np.array(list(product(grid_linspace, repeat=dim)))
+            # calculate pdf value for each point
             pdf_values = biggest_kde.pdf(points)
             points_above_threshold = points[pdf_values > threshold]
             if points_above_threshold.shape[0] == 0:
                 return None
+            # return the coordinates of the points that are not 0
             return points_above_threshold
 
         points_above_threshold = None
         percentile = 99
 
         # this process should take only a couple of iterations
         while points_above_threshold is None and percentile > 0:
             # todo: maybe throw warn?
             points_above_threshold = _get_biggest_cov_that_still_contributes(self, percentile)
             percentile -= 1
 
+        # from the coordinates of the points that are not 0 in pdf
+        # get the furthest point from the origin of coordinates
+        # which is the norm of the vectors of the points
         distances = np.linalg.norm(points_above_threshold, axis=1)
-        max_distance = np.min(distances)
+        max_distance = np.max(distances)
+        # this distance will serve as ball tree radius, defining
+        # the extent of the search of points that will contribute 
         return max_distance
 
     def _build_tree_ball(self, radius: float, neighbours: Numeric2DArray, eval_points: Numeric2DArray):
         from sklearn.neighbors import BallTree
         # build a ball tree with the data
         tree = BallTree(neighbours)
         # get the indexes of the points that are inside the ball
@@ -626,42 +642,55 @@
         pdf = np.zeros(obs)
         all_covariances = self._covariances
         weights = self._weights[self._eff_mask]
         covariances = self._covariances[self._eff_mask]
         data = self._data[self._eff_mask]
         n = self._n_eff
 
-        tree = self._build_tree_ball(self._calculate_biggest_hypersphere(), data, self._data)
+        radius = self._calculate_biggest_hypersphere()
+        tree = self._build_tree_ball(radius, data, self._data)
 
         # put weights and normalization toghether in each step
         # pdf(point) = sum(ki(point)*wi/(sum(w)-wi))
         norm_weigths = weights / (n - weights)
         pdf = np.zeros(self._n)
-        for j, p in enumerate(eval_points):
-            # print(f'hkde progress: {round(j/self._n * 100, 2)}')
+        for j, p in enumerate(tqdm(eval_points)):
+
+            # for p point, we are going to sum all the contrubutions
+            # from surrounding points
             # get the indexes of the points that are inside the ball
             indexes = tree[j]
             # get the covariances of the points that are inside the ball
             point_cov = all_covariances[j]
+            # contribution accumulator
             applied_ks = 0
             for idx in indexes:
+                # location of the contributting point
+                # as mean of the multivariate normal
                 mean = data[idx]
+                # if the point is the same as the one being evaluated
+                # (we are doing always leave1out)
                 if not np.allclose(mean, p):
+                    # convolve the covariances of the eval and contributting points
                     cov = covariances[idx] + point_cov
                     k = multivariate_normal(
                         mean,
                         cov
                     )
+                    # apply the kernel to the point and get the contribution
                     tosum = k.pdf(p) * norm_weigths[idx]
+                    # add the contribution to the accumulator
                     applied_ks += tosum
+            # put the result of the accumulator in the resulting pdf array
             pdf[j] = applied_ks
 
         if obs == 1:
             # return as float value
             return pdf[0]
+        
         return pdf
 
     def pdf(self, eval_points: Numeric2DArray, leave1out: bool = True):
         """Probability density function.
 
         Evaluate the probability density function at the provided
         points, using the fitted KDE model.
```

## scludam/pipeline.py

```diff
@@ -163,14 +163,17 @@
     estimators: List = Factory(list)
     is_clusterable: List = Factory(list)
 
     # internal attributes
     _df: pd.DataFrame = None
     _colnames: Colnames = None
     _objects: pd.DataFrame = None
+    _not_nan_mask: np.ndarray = None
+    _needed_cols: set = None
+    _original_df: pd.DataFrame = None
 
     @test_cols.validator
     def _test_cols_validator(self, attr, value):
         if len(value) != len(self.tests):
             raise ValueError("test_cols must have the same length as tests")
 
     def __attrs_post_init__(self):
@@ -278,14 +281,53 @@
 
         # estimate membershipts
         estimator = copy.deepcopy(self.estimator)
         estimator.fit(data=data, init_proba=clusterer.proba, err=err, corr=corr)
         self.estimators.append(estimator)
 
         return estimator.posteriors
+    
+    def _prepare_data(self, df: pd.DataFrame):
+
+        # store original df for output
+        self._original_df = df
+
+        # get basic needed cols
+        needed_cols = set(self.det_cols +\
+                            self.mem_cols +\
+                            [item for sublist in self.test_cols for item in sublist]
+        )
+        
+        # check needed cols exist
+        self._colnames = Colnames(df.columns)
+        self._check_cols(self.det_cols)
+        self._check_cols(self.mem_cols)
+        for i in range(len(self.test_cols)):
+            self._check_cols(self.test_cols[i])
+
+        # get err and corr for mem_cols and include them
+        # if they are sufficient to complete full
+        # covariance matrix
+        err_corr_cols = set()
+        err_cols = self._colnames.error(self.mem_cols)
+        corr_cols = self._colnames.corr(self.mem_cols)
+        if not self._colnames.missing_error(self.mem_cols):
+            err_corr_cols.update(err_cols)
+        if not self._colnames.missing_corr(self.mem_cols):
+            err_corr_cols.update(corr_cols)
+        needed_cols.update(err_corr_cols)
+
+        self._needed_cols = needed_cols
+
+        # get analysis df only with needed cols and dropping nan
+        self._not_nan_mask = df[needed_cols].notna().all(axis=1)
+        self._df = df[self._not_nan_mask][needed_cols]
+        if self._df.empty:
+            raise ValueError("No data to use after dropping nans for needed cols.")
+
 
     @beartype
     def fit(self, df: pd.DataFrame):
         """Perform the detection and membership estimation.
 
         NaNs are dropped from the dataframe copy and are
         not taken into account.
@@ -297,27 +339,22 @@
 
         Returns
         -------
         DEP
             Fitted instance of DEP.
 
         """
-        df = df.dropna()
-
-        self._df = df
+        
+        # this sets self._df, self._colnames, self._needed_cols
+        # self._non_nan_mask, self._original_df
+        self._prepare_data(df)
+        df = self._df
 
         n, d = df.shape
 
-        # check all columns
-        self._colnames = Colnames(df.columns)
-        self._check_cols(self.det_cols)
-        self._check_cols(self.mem_cols)
-        for i in range(len(self.test_cols)):
-            self._check_cols(self.test_cols[i])
-
         # detect
         print("detecting overdensities...")
         self.detection_result = self._detect(df)
 
         # if no clusters detected, return full noise probs
         if not self.detection_result.centers.size:
             self.n_detected = 0
@@ -379,15 +416,15 @@
 
         return self
 
     def _is_fitted(self):
         return self.proba is not None
 
     @beartype
-    def proba_df(self):
+    def proba_df(self, original: bool = True):
         """Return the data frame with the probabilities.
 
         Returns the full dataframe used for the process
         added columns for the labels and the probabilites.
 
         Returns
         -------
@@ -402,14 +439,25 @@
         """
         if not self._is_fitted():
             raise Exception("Not fitted, try running fit()")
 
         cols = [f"proba({i-1})" for i in range(self.proba.shape[1])]
         df = pd.DataFrame(self.proba, columns=cols)
         df["label"] = self.labels
+
+        if original:
+            # create empty columns for the original dataframe
+            empty_cols = df.columns.difference(self._original_df.columns)
+            original_df = self._original_df.copy()
+            for col in empty_cols:
+                original_df[col] = np.nan
+            # fill the values taking into account the mask
+            original_df.loc[self._not_nan_mask, df.columns] = df
+            return original_df
+
         return pd.concat(
             [self._df.reset_index(drop=True), df.reset_index(drop=True)],
             axis=1,
             sort=False,
         )
 
     @beartype
@@ -484,15 +532,15 @@
         ------
         Exception
             If DEP instance is not fitted.
 
         """
         if not self._is_fitted():
             raise Exception("Not fitted, try running fit()")
-        df = self._df[cols]
+        df = self._original_df[self._not_nan_mask][cols]
         ax = scatter2dprobaplot(df, self.proba, self.labels, plotcols, **kwargs)
         ax.invert_yaxis()
         if plot_objects:
             self._plot_objects(ax, cols)
         return ax
 
     @beartype
@@ -536,15 +584,15 @@
         ------
         Exception
             If DEP instance is not fitted.
 
         """
         if not self._is_fitted():
             raise Exception("Not fitted, try running fit()")
-        df = self._df[cols]
+        df = self._original_df[self._not_nan_mask][cols]
         ax = scatter2dprobaplot(df, self.proba, self.labels, plotcols, **kwargs)
         ax.invert_xaxis()
         if plot_objects:
             self._plot_objects(ax, cols)
         return ax
 
     @beartype
@@ -587,15 +635,15 @@
         ------
         Exception
             If DEP instance is not fitted.
 
         """
         if not self._is_fitted():
             raise Exception("Not fitted, try running fit()")
-        df = self._df[cols]
+        df = self._original_df[self._not_nan_mask][cols]
         ax = scatter2dprobaplot(df, self.proba, self.labels, plotcols, **kwargs)
         if plot_objects:
             self._plot_objects(ax, cols)
         return ax
 
     def _plot_objects(self, ax, cols, otype="Cl*"):
         try:
```

## Comparing `scludam-1.0.6.dist-info/LICENSE` & `scludam-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scludam-1.0.6.dist-info/METADATA` & `scludam-1.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scludam
-Version: 1.0.6
+Version: 1.0.7
 Summary: Star cluster detection and membership estimation based on GAIA data.
 Home-page: http://packages.python.org/scludam
 Author: Simón Pedro González
 Author-email: simon.pedro.g@gmail.com
 License: GPL-3
 Keywords: star cluster detection membership probabilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `scludam-1.0.6.dist-info/RECORD` & `scludam-1.0.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 scludam/__init__.py,sha256=K2F0TbLqJj09bSRkLjQgFpf_xhnT_WmCOjP3ogojVBU,2230
 scludam/cli.py,sha256=jvbtUrD3ATB5nrL1qJaRj34bCQVtNk1HhzzIdcRnQvo,1222
-scludam/cli_analysis.py,sha256=BGiqM8yveQg373ve9UvBPEssQ98jIQDcHKAYFcElomE,14538
+scludam/cli_analysis.py,sha256=FTNHnbot6OvwZ7GiJt9upMcYr_dLAsQsU1A9FUAlbZg,14548
 scludam/cli_input.py,sha256=FQ21TiU0q1rnodaAd9b444ayO_E2f9b6NB2crkcgefs,6933
 scludam/cli_utils.py,sha256=946vw2WG325z7qFZBhZ0TNcnl3_S6Rb1Uaes5dbra_o,12391
 scludam/detection.py,sha256=lLOUf6jyVuEuUOZJLRZvpVj2Bzp10gRWI0ulPL0Ow-g,38242
 scludam/fetcher.py,sha256=gTUdQThPb-4wMxD_SaEbJ3jXOQ4Jnyx-KZUonArbb4A,24162
-scludam/hkde.py,sha256=2zt0P4bHBwu_qZ4hKT4rKbwgunFndttaneqaKNr4ey8,29858
+scludam/hkde.py,sha256=RoKIBy_xaNMtBYa0oZcQHqBV5bxP17BS09kgo8Pi1s0,31455
 scludam/masker.py,sha256=n0Esyvy8ltK-KC_jKA0lLYtnzLANB8EbcMWD0OhTeW4,7447
 scludam/membership.py,sha256=DwbyyXd4ZomFYcgZJEz7RR1dUf20UZ5E2jjtqdmdVbA,18095
-scludam/pipeline.py,sha256=7A-q7rYT7dwCIV3cmQNPZpSdX-9uPkCXXhLH1fuf6f0,22184
+scludam/pipeline.py,sha256=ZSxKw0ZrdReyyWHDsocuq2Qb3TzuEkTWFfwny1NZLYo,24182
 scludam/plots.py,sha256=8CQ4NtOdpIvPL6UtbWNS8iEmha2N5c65pm20eARGoTM,28380
 scludam/rutils.py,sha256=Q77YqMUbTVnoBEDzWA3NMfb2nZn0xdy1uxit-DC9-Dk,4816
 scludam/shdbscan.py,sha256=3YWmhdMy9CSFP3QTLuv47xNYG_s_xzkXFnKV-YJepHs,31030
 scludam/stat_tests.py,sha256=U7JSKG4PaT6wohaH_wR9DDqZe_45UjOEkzLx9HRwFTk,23021
 scludam/synthetic.py,sha256=tBMyPyM1FyRXTkpiideq48agrn__RjGyoAEwnI0FOBg,38632
 scludam/type_utils.py,sha256=GhsRBF5TK65WZkomBeTL3gD4nZr-4wEUP7QmjOBg1-U,2609
 scludam/utils.py,sha256=uP391UX7m3xyaGfReFrnedHvvdIw4mZ1du1wnmhcFGQ,7928
@@ -22,12 +22,12 @@
 tests/test_membership.py,sha256=bhaGpr2KTGTnFHVzhVC8hBTYvl1K6w4kBAR8S5EouMw,9993
 tests/test_pipeline.py,sha256=A_H6wXnKeunFeVm4UHk5T4J2d_AM3aXMAiY1kQgAtEI,10177
 tests/test_shdbscan.py,sha256=CM8FIqpfXDTUn2OOH8jdH6aIyR9fk5lA9Qx8foITmHs,17500
 tests/test_stat_tests.py,sha256=PMlJVP8lw8llm_BCawk0EewdUGUy_Wq769WMaMgAsbo,5054
 tests/test_synthetic.py,sha256=0YeYIjRM4kWCKAeVvtIWNpIxgg2iDrYqEDbQUitZqmE,16673
 tests/test_utils.py,sha256=oCXOmGRvnWWVTVGnO44AYm0N9S8weLQWLPbwo9AYTkM,3009
 tests/utils.py,sha256=dEG0wWDV1twH_epZACm7WMeq5Sp-RNmW92la4BfMqno,611
-scludam-1.0.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-scludam-1.0.6.dist-info/METADATA,sha256=rV7afOgGQdER-t0TLNsAamxSqxXGoMYsGRPnxeo6ZWY,5384
-scludam-1.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-scludam-1.0.6.dist-info/top_level.txt,sha256=o1ZchBQ1yRGNlnzajlmexEPcjlq8wyPsyFafvNVKmqw,14
-scludam-1.0.6.dist-info/RECORD,,
+scludam-1.0.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+scludam-1.0.7.dist-info/METADATA,sha256=qW8RwcLmriK5GR84BbfXBRbbCuCjWTBiPpnKY6U_wSQ,5384
+scludam-1.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+scludam-1.0.7.dist-info/top_level.txt,sha256=o1ZchBQ1yRGNlnzajlmexEPcjlq8wyPsyFafvNVKmqw,14
+scludam-1.0.7.dist-info/RECORD,,
```

