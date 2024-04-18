# Comparing `tmp/GSG-0.3.tar.gz` & `tmp/GSG-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.3.tar", last modified: Mon Apr 15 06:47:17 2024, max compression
+gzip compressed data, was "dist/GSG-0.4.2.tar", last modified: Thu Apr 18 04:47:45 2024, max compression
```

## Comparing `GSG-0.3.tar` & `GSG-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-15 06:47:17.000000 GSG-0.3/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       68 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      165 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-15 06:47:17.000000 GSG-0.3/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    36678 2024-04-15 06:47:16.000000 GSG-0.3/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       68 2024-04-15 06:47:17.000000 GSG-0.3/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2854 2023-06-08 05:59:08.000000 GSG-0.3/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-15 06:47:17.000000 GSG-0.3/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.3/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.3/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-15 06:47:17.000000 GSG-0.3/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.3/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.3/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.3/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.3/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.3/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.3/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.3/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-15 06:47:17.000000 GSG-0.3/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      487 2024-04-15 04:20:15.000000 GSG-0.3/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-15 06:47:17.000000 GSG-0.3/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.3/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.3/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.3/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.3/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.3/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.3/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      165 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-18 04:47:45.000000 GSG-0.4.2/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40574 2024-04-18 04:41:51.000000 GSG-0.4.2/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       70 2024-04-18 04:47:45.000000 GSG-0.4.2/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2854 2023-06-08 05:59:08.000000 GSG-0.4.2/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.4.2/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.4.2/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.4.2/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.4.2/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.4.2/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.4.2/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.4.2/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-18 04:47:45.000000 GSG-0.4.2/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      489 2024-04-18 04:47:41.000000 GSG-0.4.2/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 04:47:45.000000 GSG-0.4.2/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.4.2/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.4.2/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.4.2/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.4.2/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.4.2/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.4.2/tools/utils.py
```

### Comparing `GSG-0.3/GSG.py` & `GSG-0.4.2/GSG.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sklearn.metrics import (adjusted_rand_score, normalized_mutual_info_score, 
                              silhouette_score, calinski_harabasz_score,
                              davies_bouldin_score,fowlkes_mallows_score)
 from tqdm import tqdm
-from graphmae.models import build_model
+from models import build_model
 import anndata as ad
 import scanpy as sc
 import pandas as pd
 import numpy as np
 import dgl
 import torch
 import os
@@ -20,14 +20,77 @@
     drawPicture,
     mkdir,
 )
 warnings.filterwarnings("ignore")
 from scipy.spatial.distance import pdist, squareform
 from scipy import sparse
 
+def build_args():
+    parser = argparse.ArgumentParser(description="GAT")
+    parser.add_argument("--seeds", type=int, nargs="+", default=[0])
+    parser.add_argument("--device", type=int, default=-1)
+    parser.add_argument("--warmup_steps", type=int, default=-1)
+    parser.add_argument("--num_heads", type=int, default=4,
+                        help="number of hidden attention heads")
+    parser.add_argument("--num_out_heads", type=int, default=1,
+                        help="number of output attention heads")
+    parser.add_argument("--residual", action="store_true", default=False,
+                        help="use residual connection")
+    parser.add_argument("--in_drop", type=float, default=0.2,
+                        help="input feature dropout")
+    parser.add_argument("--attn_drop", type=float, default=0.1,
+                        help="attention dropout")
+    parser.add_argument("--weight_decay", type=float, default=2e-4,
+                        help="weight decay")
+    parser.add_argument("--negative_slope", type=float, default=0.2,
+                        help="the negative slope of leaky relu for GAT")
+    parser.add_argument("--drop_edge_rate", type=float, default=0.0)
+    parser.add_argument("--optimizer", type=str, default="adam")
+    parser.add_argument("--max_epoch_f", type=int, default=300)
+    parser.add_argument("--lr_f", type=float, default=0.01, help="learning rate for evaluation")
+    parser.add_argument("--weight_decay_f", type=float, default=1e-4, help="weight decay for evaluation")
+    parser.add_argument("--linear_prob", action="store_true", default=True)
+    parser.add_argument("--load_model", action="store_true")
+    parser.add_argument("--save_model", action="store_true")
+    parser.add_argument("--use_cfg", action="store_true")
+    parser.add_argument("--logging", action="store_true")
+    parser.add_argument("--scheduler", action="store_true", default=True)
+    parser.add_argument("--concat_hidden", action="store_true", default=False)
+    # for graph classification
+    parser.add_argument("--pooling", type=str, default="mean")
+    parser.add_argument("--deg4feat", action="store_true", default=False, help="use node degree as input feature")
+    parser.add_argument("--batch_size", type=int, default=32)
+    # adjustable parameters
+    parser.add_argument("--mask_rate", type=float, default=0.8)
+    parser.add_argument("--encoder", type=str, default="gin")
+    parser.add_argument("--decoder", type=str, default="gin")
+    parser.add_argument("--num_hidden", type=int, default=128,
+                        help="number of hidden units")
+    parser.add_argument("--num_layers", type=int, default=3,
+                        help="number of hidden layers")
+    parser.add_argument("--activation", type=str, default="elu")
+    parser.add_argument("--max_epoch", type=int, default=500,
+                        help="number of training epochs")
+    parser.add_argument("--lr", type=float, default=0.001 ,
+                        help="learning rate")
+    parser.add_argument("--alpha_l", type=float, default=4, help="`pow`inddex for `sce` loss")
+    parser.add_argument("--loss_fn", type=str, default="sce")
+    parser.add_argument("--replace_rate", type=float, default=0.05)
+    parser.add_argument("--norm", type=str, default="batchnorm")
+    # GSG parameter
+    parser.add_argument("--feature_dim_method", type=str, default="PCA")
+    parser.add_argument("--num_features", type=int, default=600)
+    parser.add_argument("--threshold_radius", type=int, default=25)
+    parser.add_argument("--folder_name", type=str, default="data/10X/")
+    parser.add_argument("--sample_name", type=str, default="151673")
+    parser.add_argument("--cluster_label", type=str, default= "")
+    parser.add_argument("--num_classes", type=int, default=7,help = "The number of clusters")
+    # read parameters
+    args = parser.parse_args()
+    return args
 
 def GSG_Spatial_Pic(adata,args, result_file_path):
     if(args.cluster_label != ""):
         adata.obs[args.cluster_label] = adata.obs[args.cluster_label].astype('category').cat.add_categories(['None'])
         adata.obs[args.cluster_label] = adata.obs[args.cluster_label].fillna("None")
         drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute=args.cluster_label,save_file = result_file_path + "/Ground_true.pdf",is_show=False,is_save= True)
         drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute="GSG_Kmeans_cluster_str",save_file = result_file_path + "/GSG_Cluster_Spatial.pdf",is_show=False,is_save= True)
@@ -685,9 +748,9 @@
         used_adata = adata
         sc.tl.paga(used_adata, groups="GSG_Kmeans_cluster_str")
     sc.pl.paga_compare(used_adata, legend_fontsize=15, node_size_scale= 4, frameon=False, size=50,max_edge_width = 10,right_margin=0.2,
                         legend_fontoutline=5,title="PAGA_SHOW", show=False)
     plt.savefig( result_file + "/" + filename,bbox_inches='tight',dpi =1000)
 
 
-def save_file(adata,result_file):
-    adata_X = adata.X
+# def save_file(adata,result_file):
+#     adata_X = adata.X
```

### Comparing `GSG-0.3/README.md` & `GSG-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `GSG-0.3/datasets/data_util.py` & `GSG-0.4.2/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/__init__.py` & `GSG-0.4.2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/dot_gat.py` & `GSG-0.4.2/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/edcoder.py` & `GSG-0.4.2/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/gat.py` & `GSG-0.4.2/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/gcn.py` & `GSG-0.4.2/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/gin.py` & `GSG-0.4.2/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/models/loss_func.py` & `GSG-0.4.2/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/tools/batch_remove.py` & `GSG-0.4.2/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/tools/evaluation.py` & `GSG-0.4.2/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/tools/parameters_dict.py` & `GSG-0.4.2/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/tools/test.py` & `GSG-0.4.2/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.3/tools/utils.py` & `GSG-0.4.2/tools/utils.py`

 * *Files identical despite different names*

