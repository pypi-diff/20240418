# Comparing `tmp/pyturbseq-0.0.8.tar.gz` & `tmp/pyturbseq-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyturbseq-0.0.8.tar", last modified: Mon Feb 26 01:59:33 2024, max compression
+gzip compressed data, was "pyturbseq-0.0.9.tar", last modified: Fri Mar 22 01:09:52 2024, max compression
```

## Comparing `pyturbseq-0.0.8.tar` & `pyturbseq-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-02-26 02:08:13.342491 pyturbseq-0.0.8/
--rw-rw-r--   0 awinters  (1011) awinters  (1011)     1500 2024-02-08 14:35:04.000000 pyturbseq-0.0.8/LICENSE
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      617 2024-02-26 02:08:13.341492 pyturbseq-0.0.8/PKG-INFO
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      412 2024-02-09 20:40:53.000000 pyturbseq-0.0.8/README.md
--rw-rw-r--   0 awinters  (1011) awinters  (1011)       97 2024-02-08 14:35:04.000000 pyturbseq-0.0.8/pyproject.toml
-drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-02-26 02:08:13.331492 pyturbseq-0.0.8/pyturbseq/
--rw-rw-r--   0 awinters  (1011) awinters  (1011)        0 2023-11-28 19:58:44.000000 pyturbseq-0.0.8/pyturbseq/__init__.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)    13981 2024-02-13 21:12:43.000000 pyturbseq-0.0.8/pyturbseq/calling.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)     3365 2024-02-11 05:47:55.000000 pyturbseq-0.0.8/pyturbseq/cellranger.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)     4312 2024-02-26 01:51:31.000000 pyturbseq-0.0.8/pyturbseq/de.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      810 2024-02-08 14:35:04.000000 pyturbseq-0.0.8/pyturbseq/guides.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)    38282 2024-02-25 20:48:22.000000 pyturbseq-0.0.8/pyturbseq/interaction.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)     9284 2024-02-14 00:38:51.000000 pyturbseq-0.0.8/pyturbseq/plot.py
--rw-rw-r--   0 awinters  (1011) awinters  (1011)    20859 2024-02-21 03:48:58.000000 pyturbseq-0.0.8/pyturbseq/utils.py
-drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-02-26 02:08:13.339491 pyturbseq-0.0.8/pyturbseq.egg-info/
--rw-r--r--   0 awinters  (1011) awinters  (1011)      617 2024-02-26 02:08:12.000000 pyturbseq-0.0.8/pyturbseq.egg-info/PKG-INFO
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      370 2024-02-26 02:08:12.000000 pyturbseq-0.0.8/pyturbseq.egg-info/SOURCES.txt
--rw-rw-r--   0 awinters  (1011) awinters  (1011)        1 2024-02-26 02:08:12.000000 pyturbseq-0.0.8/pyturbseq.egg-info/dependency_links.txt
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      162 2024-02-26 02:08:12.000000 pyturbseq-0.0.8/pyturbseq.egg-info/requires.txt
--rw-rw-r--   0 awinters  (1011) awinters  (1011)       10 2024-02-26 02:08:12.000000 pyturbseq-0.0.8/pyturbseq.egg-info/top_level.txt
--rw-rw-r--   0 awinters  (1011) awinters  (1011)       38 2024-02-26 02:08:13.342491 pyturbseq-0.0.8/setup.cfg
--rw-rw-r--   0 awinters  (1011) awinters  (1011)      819 2024-02-26 02:05:50.000000 pyturbseq-0.0.8/setup.py
+drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-03-22 01:18:40.604800 pyturbseq-0.0.9/
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)     1500 2024-02-08 14:35:04.000000 pyturbseq-0.0.9/LICENSE
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      617 2024-03-22 01:18:40.603800 pyturbseq-0.0.9/PKG-INFO
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      412 2024-02-09 20:40:53.000000 pyturbseq-0.0.9/README.md
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)       97 2024-02-08 14:35:04.000000 pyturbseq-0.0.9/pyproject.toml
+drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-03-22 01:18:40.550800 pyturbseq-0.0.9/pyturbseq/
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)        0 2023-11-28 19:58:44.000000 pyturbseq-0.0.9/pyturbseq/__init__.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)    16412 2024-03-22 01:16:34.000000 pyturbseq-0.0.9/pyturbseq/calling.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)     3467 2024-03-22 01:16:34.000000 pyturbseq-0.0.9/pyturbseq/cellranger.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)     4295 2024-03-22 01:16:34.000000 pyturbseq-0.0.9/pyturbseq/de.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      810 2024-02-08 14:35:04.000000 pyturbseq-0.0.9/pyturbseq/guides.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)    38093 2024-02-27 03:30:02.000000 pyturbseq-0.0.9/pyturbseq/interaction.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)     9318 2024-03-22 01:16:34.000000 pyturbseq-0.0.9/pyturbseq/plot.py
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)    23934 2024-03-22 01:16:34.000000 pyturbseq-0.0.9/pyturbseq/utils.py
+drwxrwxr-x   0 awinters  (1011) awinters  (1011)        0 2024-03-22 01:18:40.601800 pyturbseq-0.0.9/pyturbseq.egg-info/
+-rw-r--r--   0 awinters  (1011) awinters  (1011)      617 2024-03-22 01:18:39.000000 pyturbseq-0.0.9/pyturbseq.egg-info/PKG-INFO
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      370 2024-03-22 01:18:39.000000 pyturbseq-0.0.9/pyturbseq.egg-info/SOURCES.txt
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)        1 2024-03-22 01:18:39.000000 pyturbseq-0.0.9/pyturbseq.egg-info/dependency_links.txt
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      155 2024-03-22 01:18:39.000000 pyturbseq-0.0.9/pyturbseq.egg-info/requires.txt
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)       10 2024-03-22 01:18:39.000000 pyturbseq-0.0.9/pyturbseq.egg-info/top_level.txt
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)       38 2024-03-22 01:18:40.604800 pyturbseq-0.0.9/setup.cfg
+-rw-rw-r--   0 awinters  (1011) awinters  (1011)      812 2024-03-22 01:18:05.000000 pyturbseq-0.0.9/setup.py
```

### Comparing `pyturbseq-0.0.8/LICENSE` & `pyturbseq-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyturbseq-0.0.8/PKG-INFO` & `pyturbseq-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyturbseq
-Version: 0.0.8
+Version: 0.0.9
 Author: Aidan Winters
 Author-email: aidanfwinters@gmail.com
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyturbseq
```

### Comparing `pyturbseq-0.0.8/pyturbseq/calling.py` & `pyturbseq-0.0.9/pyturbseq/calling.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sklearn.mixture import GaussianMixture
 from joblib import Parallel, delayed
 from tqdm import tqdm
 
 from scipy.sparse import csr_matrix
 
 
-def gm(counts, n_components=2, prob_threshold=0.5, subset=False, subset_minimum=50, nonzero=False, seed=99, **kwargs):
+def gm(counts, n_components=2, prob_threshold=0.5, subset=False, subset_minimum=50, nonzero=False, calling_min_count=1, seed=99, **kwargs):
     """
     Fits a Gaussian Mixture Model to the input data.
     Args:
         x: numpy array of data to fit
         n_components: number of components to fit. Default 2
         subset: fraction of data to fit on, this speeds up computation. Default 0.2
         subset_minimum: minimum number of cells to fit on, if subset is too small. Default 50
@@ -29,28 +29,33 @@
     """
     
     counts = counts.reshape(-1, 1)
 
     if nonzero:
         counts = counts[counts > 0].reshape(-1,1)
 
+    if counts.max() < calling_min_count:
+        print(f"max count ({counts.max()}) is less than calling_min_count ({calling_min_count}). Returning no calls.")
+        #return preds of -1
+        return np.repeat(0, counts.shape[0])
+
     counts = np.log10(counts + 1)
 
     if counts.shape[0] < 10:
-        print(f"too few cells ({counts.shape[0]}) to run GMM. Returning -1")
+        print(f"too few cells ({counts.shape[0]}) to run GMM. Returning no calls.")
         #return preds of -1
         return np.repeat(-1, counts.shape[0]), np.repeat(-1, counts.shape[0])
 
     if subset: #optionally subset the data to fit on only a fraction, this speeds up computation
         s = min(int(counts.shape[0]*subset), subset_minimum)
         # print(f"subsetting to {subset}. {int(dat_in.shape[0]*subset)} cells of {dat_in.shape[0]}")
         counts = counts[np.random.choice(counts.shape[0], size=s, replace=False), :]
 
     try:
-        gmm = GaussianMixture(n_components=n_components, random_state=seed, covariance_type="tied", n_init=3, **kwargs)
+        gmm = GaussianMixture(n_components=n_components, random_state=seed, covariance_type="tied", n_init=5, **kwargs)
         pred = gmm.fit(counts)
     except:
         print(f"failed to fit GMM. Returning -1")
         #return preds of -1
         return np.repeat(-1, counts.shape[0]), np.repeat(-1, counts.shape[0])
 
     #get probability per class
@@ -58,41 +63,82 @@
     #get probability for the 'postitive'
     means = gmm.means_.flatten()
     positive = np.argmax(means)
     probs_positive = probs[:,positive]
 
     return probs_positive > prob_threshold #return confident (ie above threshold) positive calls
 
-def call_features(features, n_jobs=1, inplace=True, quiet=True, **kwargs):
+def call_features(features, feature_type=None, min_feature_umi=1, n_jobs=1, inplace=True, quiet=True, **kwargs):
     """
     Accepts an anndata object with adata.X containing the counts of each guide.
     In parallel, fits a GMM to each guide and returns the predicted class for each guide.
     Args:
         features: anndata object with adata.X containing the counts of each guide
     Returns:
         anndata object with adata.X containing the predicted class for each guide
     """
     vp = print if not quiet else lambda *a, **k: None
 
-    lil = features.X.T.tolil()
+    if feature_type is not None:
+        #confirm feature type is in var['feature_type']
+        vp(f"Subsetting features to {feature_type}...")
+        assert feature_type in features.var['feature_types'].unique(), f"feature_type {feature_type} not found in var['feature_types']"
+        feature_list = features.var.index[features.var['feature_types'] == feature_type]
+        lil = features[:,features.var.index[features.var['feature_types'] == feature_type]].X.T.tolil()
+    else:
+        feature_list = features.var.index
+        lil = features.X.T.tolil()
 
     vp(f'Running GMM with {n_jobs} workers...')
     #add tqdm to results call
     results = Parallel(n_jobs=n_jobs)(delayed(gm)(lst.toarray(), **kwargs) for lst in tqdm(lil, disable=quiet))
     called = csr_matrix(results).T.astype('uint8')
 
+    # Remove calls for features that do not pass threshold (indicating issue with that guide)
+
     if not inplace:
         vp(f"Creating copy AnnData object with guide calls...")
         features = features.copy()
 
     vp(f"Updating AnnData object with guide calls...")
-    features.layers['calls'] = called
+    features.obsm['calls'] = called
+    features.uns['features'] = feature_list
     features.obs['num_features'] = called.toarray().sum(axis=1).flatten()
-    features.obs['feature_call'] = ['|'.join(features.var_names.values[called[x,:].toarray().flatten() == 1]) for x in range(features.shape[0])]
-    features.obs['feature_umi'] = ['|'.join(features.var_names.values[features.X[x,:].toarray().flatten() == 1]) for x in range(features.X.shape[0])]
+    features.obs['feature_call'] = ['|'.join(feature_list[called[x,:].toarray().flatten() == 1]) for x in range(features.shape[0])]
+    features.obs['feature_umi'] = ['|'.join(features[x,feature_list].X.toarray().astype('int').astype('str').flatten()) for x in range(features.X.shape[0])]
+    if not inplace:
+        return features
+
+
+
+def calculate_feature_call_metrics(features, feature_type='CRISPR Guide Capture', inplace=True, quiet=False):
+    vp = print if not quiet else lambda *a, **k: None
+
+    if feature_type is not None:
+        features_subset = features[:,features.var.index[features.var['feature_types'] == feature_type]]
+
+    if not inplace:
+        vp(f"Creating copy AnnData object with guide calls...")
+        features = features.copy()
+
+    features.obs['total_feature_counts'] = features_subset.X.sum(axis=1)
+    features.obs['proportion_counts_in_top_feature'] = features_subset.X.max(axis=1).toarray().flatten() / features.obs['total_feature_counts'].values
+
+    x_sorted = features_subset.X.toarray().argsort(axis=1)
+    features.obs['ratio_2nd_1st_feature'] = (x_sorted[:,-2]+1) / (x_sorted[:,-1]+1)
+    features.obs['log2_ratio_2nd_1st_feature'] = np.log2(features.obs['ratio_2nd_1st_feature'])
+
+    features.obs['log1p_total_feature_counts'] = np.log1p(features_subset.X.sum(axis=1))
+    features.obs['log10_total_feature_counts'] = np.log10(features_subset.X.sum(axis=1)+1)
+
+    # features.var['total_counts'] = features_subset.X.toarray().sum(axis=0)
+    # features.var['log1p_total_counts'] = np.log1p(features.var['total_counts'])
+    # features.var['log10_total_counts'] = np.log10(features.var['total_counts'])
+    # features.var['pct_cells_with_feature'] = (features_subset.X > 0).toarray().sum(axis=0) / adata.X.shape[0]
+
     if not inplace:
         return features
 
 ########################################################################################################################
 ########################################################################################################################
 ############# GUIDE CALLING FUNCTIONS ##################################################################################
 ########################################################################################################################
```

### Comparing `pyturbseq-0.0.8/pyturbseq/cellranger.py` & `pyturbseq-0.0.9/pyturbseq/cellranger.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,21 +85,27 @@
 
 
 def add_CR_sgRNA(
     adata,
     sgRNA_analysis_out,
     calls_file="protospacer_calls_per_cell.csv",
     library_ref_file=None,
+    inplace=True,
     quiet=False,
     ):
     """
     Uses the cellranger calls and merges them with anndata along with some metrics
     """
     calls = pd.read_csv(sgRNA_analysis_out + calls_file, index_col=0)
     inds = calls.index.intersection(adata.obs.index)
     if not quiet: print(f'Found sgRNA information for {len(inds)}/{adata.obs.shape[0]} ({round(len(inds) / adata.obs.shape[0] * 100, 2)}%) of cell barcodes')
     calls = calls.loc[inds, :]
 
     #merge with anndata obs
+    if not inplace: 
+        adata = adata.copy()
+        
     for col in calls.columns:
         adata.obs.loc[inds, col] = calls[col]
-    return adata
+
+    if not inplace:
+        return adata
```

### Comparing `pyturbseq-0.0.8/pyturbseq/de.py` & `pyturbseq-0.0.9/pyturbseq/de.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from tqdm import tqdm
 import pandas as pd
 from pydeseq2.dds import DeseqDataSet
 from pydeseq2.ds import DeseqStats
+from pydeseq2.default_inference import DefaultInference
 from statsmodels.stats.multitest import multipletests
 import numpy as np
 import multiprocessing
+import math
 
 from joblib import Parallel, delayed
 
 
 def get_degs(adata, design_col, ref_val=None, n_cpus=16, quiet=False):
     """
     Run DESeq2 analysis on single-cell RNA sequencing data.
@@ -20,38 +22,41 @@
     ref_val (str, optional): Reference value for the design matrix. Defaults to None.
     n_cpus (int, optional): Number of CPUs to use for DESeq2. Defaults to 16.
     quiet (bool, optional): Flag to suppress DESeq2 output. Defaults to True.
 
     Returns:
     pd.DataFrame: DataFrame containing DESeq2 results.
     """
+
+    ref_level = [design_col, ref_val] if ref_val is not None else None
+
+    inference = DefaultInference(n_cpus=n_cpus)
     dds = DeseqDataSet(
         counts=pd.DataFrame(
             adata.X.toarray() if type(adata.X) is not np.ndarray else adata.X,
             index=adata.obs.index, columns=adata.var.index
         ),
         metadata=adata.obs,
         design_factors=design_col,
-        n_cpus=n_cpus,
+        inference=inference,
+        min_replicates=math.inf, 
+        min_mu=1e-6,
+        ref_level=ref_level,
+        refit_cooks=True,
         quiet=quiet,  # Passing the quiet argument
     )
 
     dds.deseq2()  # Passing the quiet argument
     # Setting up contrast for DESeq2
     if ref_val is None:
         contrast = [design_col] + list(adata.obs[design_col].unique())
     else:
-        design_vals = adata.obs[design_col].unique()
-        alt_val = [x for x in design_vals if x != ref_val]
-        if len(alt_val) > 1:
-            raise ValueError(f"More than one alternative value for {design_col} in adata. This is currently not supported.")
-        contrast = [design_col, alt_val[0], ref_val]
-
-    # Running the statistical analysis
-    stat_res = DeseqStats(dds, contrast=contrast, n_cpus=n_cpus, quiet=quiet)
+        contrast=None
+        
+    stat_res = DeseqStats(dds, contrast=contrast, quiet=quiet, inference=inference)
     stat_res.summary()
 
     df = stat_res.results_df
     df['padj_bh'] = multipletests(df['pvalue'], method='fdr_bh')[1]
 
     return df
```

### Comparing `pyturbseq-0.0.8/pyturbseq/guides.py` & `pyturbseq-0.0.9/pyturbseq/guides.py`

 * *Files identical despite different names*

### Comparing `pyturbseq-0.0.8/pyturbseq/interaction.py` & `pyturbseq-0.0.9/pyturbseq/interaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,22 +471,17 @@
 
     # invert term2pert
     pert2term = {v: k for k, v in term2pert.items()}
 
     return term2pert, pert2term, split
 
 
-def breakdown_triple_wRef(input_str, third_pos="css", ref="control", delim="|"):
+def breakdown_triple_wRef(input_str,  ref="control", delim="|"):
     split = input_str.split(delim)
     # confirm third pos is in split and if so make sure at the end
-    if third_pos in split:
-        split.remove(third_pos)
-        split.append(third_pos)
-    else:
-        raise ValueError(f"third_pos {third_pos} not in split {split}")
     term2pert = {}
     term2pert["ref"] = delim.join([ref] * 3)
     term2pert["a"] = split[0] + delim + ref + delim + ref
     term2pert["b"] = split[1] + delim + ref + delim + ref
     term2pert["c"] = split[2] + delim + ref + delim + ref
     term2pert["ab"] = split[0] + delim + split[1] + delim + ref
     term2pert["ac"] = split[0] + delim + split[2] + delim + ref
```

### Comparing `pyturbseq-0.0.8/pyturbseq/plot.py` & `pyturbseq-0.0.9/pyturbseq/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,41 +234,41 @@
 ##########################################################################
 
 
 
 ## plot ratio of top 2 against counts: 
 def plot_top2ratio_counts(features, show=False):
         #plot QC for guide metrics
-    g = sns.jointplot(data = features.obs, y = 'log10_total_counts', x = 'log2_ratio_2nd_1st', kind = 'hex')
+    g = sns.jointplot(data = features.obs, y = 'log10_total_feature_counts', x = 'log2_ratio_2nd_1st_feature', kind = 'hex')
     g.ax_joint.set_ylabel('log10(total counts/cell)')
-    g.ax_joint.set_xlabel('log2(2nd top sgRNA / top sgRNA)')
+    g.ax_joint.set_xlabel('log2(2nd top feature / top feature)')
     g.fig.suptitle('Cell level metrics')
     g.fig.tight_layout()
     if show:
         plt.show()
 
     return g
     
 
 #plot guide call proportions
 def plot_feature_count_metrics(features, ntc_var=None, show=False, ax=None):
     if ax is None:
         fig, ax = plt.subplots(1,1)
 
-    sns.scatterplot(data = features.var, y = 'pct_cells_with_guide', x = 'log10_total_counts', hue=ntc_var, ax=ax)
+    sns.scatterplot(data = features.var, y = 'pct_cells_with_feature', x = 'log10_total_feature_counts', hue=ntc_var, ax=ax)
     # uniform coverage expectation
     if ntc_var in features.var.columns:
         unif = (1/features.var.query(f'{ntc_var} == False').shape[0])/2
         ax.axhline(unif, color='r', linestyle='--')
     #add label to axhline
         xmax = ax.get_xlim()[1]
         ax.text(xmax, unif, 'Expected %', ha='right', va='bottom', color='r')
         ax.legend(title='Negative Control')
-    ax.set_xlabel('log10(total counts/guide)')
-    ax.set_ylabel('% cells with guide')
+    ax.set_xlabel('log10(total counts/feature)')
+    ax.set_ylabel('% cells with feature')
     ax.set_ylim(0,0.2)
     #change y ticks to be multiplied by 100
     ax.set_yticks(plt.yticks()[0], [f'{int(x*100)}%' for x in plt.yticks()[0]])
     if show: 
         plt.show()
     return ax
```

### Comparing `pyturbseq-0.0.8/pyturbseq/utils.py` & `pyturbseq-0.0.9/pyturbseq/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 
 ########################################################################################################################
 ########################################################################################################################
 ############# ADATA FILTERING FUNCTIONS ################################################################################
 ########################################################################################################################
 
 def filter_adata(adata, obs_filters=None, var_filters=None, copy=True):
+    
+    if copy: 
+        adata = adata.copy()
     if obs_filters is not None:
         for f in obs_filters:
             adata = adata[adata.obs.query(f).index, :]
         
     if var_filters is not None:
         for f in var_filters:
             adata = adata[:, adata.var.query(f).index]
 
-    if copy:
-        return adata.copy()
     return adata
 
 def filter_to_feature_type(
     adata,
     feature_type='Gene Expression'
     ):
     """
@@ -248,14 +249,15 @@
 def calculate_target_change(
     adata,
     perturbation_column=None,
     reference_value=None,
     perturbation_gene_map=None,
     check_norm=True,
     quiet=False,
+    inplace = True,
     ):
     """
     Compute the "percent change" for each cell against a reference.
     
     Parameters:
     - adata: anndata.AnnData object containing expression data. assumed to be transformed as desired
     - perturbation_column: column in adata.obs indicating the perturbation/knockdown. If passed, then perturbation matrix is regenerated. Else, looks for adata.obsm['perturbation'].
@@ -264,15 +266,18 @@
     - check_norm: if True, checks if data is normalized to counts per cell. If not, normalizes.
     - quiet: if False, prints progress
     
     Returns:
     - An AnnData object with an additional column in obs containing the "percent knocked down" for each cell.
     """
 
-    final_adata = adata    
+    if not inplace:
+        final_adata = adata.copy()   
+    else: 
+        final_adata = adata
     if not quiet: print(f"Computing percent change for '{perturbation_column}' across {adata.shape[0]} cells...")
 
     #check inputs: 
     duplicated_genes = adata.var.index.duplicated()
     if sum(duplicated_genes) > 0:
         raise ValueError(f"Duplicated gene names found in adata.var.index. Please remove duplicated gene names before running this function. \nGene names found: {list(adata.var.index[duplicated_genes])}")
 
@@ -348,14 +353,17 @@
 
         # pm = pm.stack()
         final_adata.obs.loc[~ref_bool, 'target_pct_change'] = pct_change_matr[pm.values]
         final_adata.obs.loc[~ref_bool, 'target_zscore'] = zscore_matr[pm.values]
         final_adata.obs.loc[~ref_bool, 'target_log2fc'] = log2fc_matr[pm.values]
         final_adata.obs.loc[~ref_bool, 'target_gene_expression'] = target_gex_matr[pm.values]
 
+    if not inplace: 
+        return final_adata
+
 ############################################################################################################
 ##### Perturbation Similarity Analysis  #####
 ############################################################################################################
 
 from scipy.spatial.distance import pdist, squareform
 from hdbscan import HDBSCAN
 
@@ -494,7 +502,76 @@
     """
     adpb = ADPBulk(adata, groupby=groupby, **kwargs)
     pseudobulk_matrix = adpb.fit_transform()
     sample_meta = adpb.get_meta().set_index('SampleName')
     adata = sc.AnnData(pseudobulk_matrix, obs=sample_meta, var=adata.var)
 
     return adata
+
+
+##############################################################################################################################
+############## DOWNSAMPLE AND SUBSAMPLE FUNCTIONS ############################################################################
+##############################################################################################################################
+
+#randonly select N cells from each label in column
+def subsample_on_covariate(adata, column, num_cells=100, copy=True):
+
+    #set num_cells to minimum of all groups
+    num_cells = min(min(adata.obs[column].value_counts()), num_cells)
+    print(num_cells)
+
+    #get the indices of the cells
+    inds = []
+    for group in adata.obs[column].unique():
+        inds.extend(np.random.choice(adata.obs[adata.obs[column] == group].index, num_cells, replace=False))
+
+    if copy:
+        return adata[inds, :].copy()
+    else:
+        return adata[inds, :]
+
+
+def subsample_on_multiple_covariates(adata, columns, num_cells=100, min_cols=None, copy=True):
+    """
+    Subsamples the AnnData object based on multiple covariates.
+    
+    Parameters:
+    - adata: AnnData object
+    - columns: list of columns to subsample on
+    - num_cells: target number of cells to subsample per group combination
+    - min_cols: the columns to calculate the minimum count for each group within this column
+    - copy: whether to return a copy of the subsampled AnnData object
+    
+    Returns:
+    - Subsampled AnnData object
+    """
+
+    #check to make sure index names are unique
+    assert len(adata.obs.index) == len(set(adata.obs.index)), 'Index names are not unique'
+    
+    # Initialize DataFrame to track group sizes
+    group_sizes = pd.DataFrame(adata.obs, columns=columns)
+    
+    # Calculate group sizes for combinations of covariates
+    group_sizes = group_sizes.groupby(columns).size().reset_index(name='count')
+    
+     # If a minimum column is specified, calculate the minimum count for each group within this column
+    if min_cols:
+        #get the covariate that are not in min_cols
+        other_cols = [col for col in columns if col not in min_cols]
+        min_counts = group_sizes.groupby(other_cols).agg({'count': 'min'}).reset_index()
+        group_sizes = pd.merge(group_sizes[group_sizes.columns[:-1]], min_counts, on=other_cols, how='left')
+        print(group_sizes.sort_values(other_cols))
+    group_sizes['count'] = group_sizes['count'].apply(lambda x: min(x, num_cells))
+    
+    # Sample indices from each group
+    inds = []
+    for _, row in group_sizes.iterrows():
+        filter_condition = (adata.obs[columns] == row[columns]).all(axis=1)
+        eligible_indices = adata.obs[filter_condition].index
+        sampled_indices = np.random.choice(eligible_indices, int(row['count']), replace=False)
+        inds.extend(sampled_indices)
+    
+    if copy:
+        return adata[inds, :].copy()
+    else:
+        return adata[inds, :]
```

### Comparing `pyturbseq-0.0.8/pyturbseq.egg-info/PKG-INFO` & `pyturbseq-0.0.9/pyturbseq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyturbseq
-Version: 0.0.8
+Version: 0.0.9
 Author: Aidan Winters
 Author-email: aidanfwinters@gmail.com
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyturbseq
```

### Comparing `pyturbseq-0.0.8/setup.py` & `pyturbseq-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyturbseq',
     author='Aidan Winters',
     author_email='aidanfwinters@gmail.com',
-    version='0.0.8',
+    version='0.0.9',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['pyturbseq'],
     python_requires='>=3.8,<3.12',
     install_requires=[
         'scanpy',
         'scipy',
@@ -21,15 +21,15 @@
         'numpy',
         'pandas',
         'matplotlib',
         'seaborn',
         'tqdm',
         'fastcluster',
         'adjusttext',
-        'pydeseq2==0.4.1',
+        'pydeseq2',
         'statsmodels==0.13.5',
         'adpbulk',
         'anndata',
         'hdbscan',
         'dcor',
     ]
 )
```

