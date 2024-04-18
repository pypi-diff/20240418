# Comparing `tmp/sc-instant-1.1.tar.gz` & `tmp/sc_instant-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-instant-1.1.tar", last modified: Tue Jan 16 16:05:11 2024, max compression
+gzip compressed data, was "sc_instant-1.2.tar", last modified: Thu Apr 18 19:14:13 2024, max compression
```

## Comparing `sc-instant-1.1.tar` & `sc_instant-1.2.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.819787 sc-instant-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.815787 sc-instant-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.819787 sc-instant-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-16 16:04:41.000000 sc-instant-1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-16 16:04:41.000000 sc-instant-1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.819787 sc-instant-1.1/InSTAnT/
--rwxr-xr-x   0 runner    (1001) docker     (127)    75927 2024-01-16 16:04:41.000000 sc-instant-1.1/InSTAnT/InSTAnT.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-16 16:04:41.000000 sc-instant-1.1/InSTAnT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-01-16 16:04:41.000000 sc-instant-1.1/InSTAnT/poibin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-16 16:04:41.000000 sc-instant-1.1/InSTAnT/poisson_binomial.py
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-01-16 16:05:11.819787 sc-instant-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-01-16 16:04:41.000000 sc-instant-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.819787 sc-instant-1.1/README_files/
--rw-r--r--   0 runner    (1001) docker     (127)    35369 2024-01-16 16:04:41.000000 sc-instant-1.1/README_files/README_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-16 16:04:41.000000 sc-instant-1.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-16 16:04:41.000000 sc-instant-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-16 16:04:41.000000 sc-instant-1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 16:05:11.819787 sc-instant-1.1/sc_instant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-01-16 16:05:11.000000 sc-instant-1.1/sc_instant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-16 16:05:11.000000 sc-instant-1.1/sc_instant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 16:05:11.000000 sc-instant-1.1/sc_instant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-16 16:05:11.000000 sc-instant-1.1/sc_instant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-16 16:05:11.000000 sc-instant-1.1/sc_instant.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-01-16 16:05:11.819787 sc-instant-1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1171 2024-01-16 16:04:41.000000 sc-instant-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 19:13:43.000000 sc_instant-1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 19:13:43.000000 sc_instant-1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/InSTAnT/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    83230 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/InSTAnT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/InSTAnT/gspan_mining/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/gspan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/gspan_mining/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/poibin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-18 19:13:43.000000 sc_instant-1.2/InSTAnT/poisson_binomial.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1062 2024-04-18 19:13:43.000000 sc_instant-1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-18 19:14:13.501282 sc_instant-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-18 19:13:43.000000 sc_instant-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 19:13:43.000000 sc_instant-1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 19:13:43.000000 sc_instant-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 19:13:43.000000 sc_instant-1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:14:13.501282 sc_instant-1.2/sc_instant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-18 19:14:13.000000 sc_instant-1.2/sc_instant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-18 19:14:13.000000 sc_instant-1.2/sc_instant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:14:13.000000 sc_instant-1.2/sc_instant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 19:14:13.000000 sc_instant-1.2/sc_instant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 19:14:13.000000 sc_instant-1.2/sc_instant.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-04-18 19:14:13.505282 sc_instant-1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1235 2024-04-18 19:13:43.000000 sc_instant-1.2/setup.py
```

### Comparing `sc-instant-1.1/.github/workflows/python-publish.yml` & `sc_instant-1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sc-instant-1.1/InSTAnT/InSTAnT.py` & `sc_instant-1.2/InSTAnT/InSTAnT.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 import timeit
 import subprocess
 import pandas as pd
 import numpy as np
 from pathlib import Path
 import multiprocessing as mp
 import matplotlib.pyplot as plt
-from InSTAnT.poibin import PoiBin
 from scipy.spatial import cKDTree
 from collections import Counter
 from scipy.stats import hypergeom
-from scipy.stats import binom_test
+from scipy.stats import binomtest
 from scipy.optimize import minimize
 from sklearn.preprocessing import LabelEncoder
 from scipy.stats import multivariate_hypergeom
-from InSTAnT.poisson_binomial import PoissonBinomial
+# from .poisson_binomial import PoissonBinomial
+# from .poibin import PoiBin
+from .poibin import PoiBin
+from .poisson_binomial import PoissonBinomial
+from .gspan_mining.config import parser
+from .gspan_mining.main import main
 import anndata as ad
+import networkx as nx
+import os
 
 class ConditionalGlobalColocalization():
     '''
         Performs conditional global colocalization
         Requires output from ProximalPairs()
         Arguments: 
             - all_pvals: (Array) Gene-Gene pairwise pvalues for all cells calcuated using ProximalPairs().
@@ -183,16 +189,19 @@
         self.obs = self.obs_trial_pairs()
         self.p_vals = self.compute_p_val()
     
     def compute_p_val(self):
         p_vals = np.ones((len(self.geneList), len(self.geneList)))
         for i in range(self.obs.shape[0]):
             for j in range(i,self.obs.shape[1]):
-                p_vals[i,j] = binom_test(self.obs[i,j], self.num_trial[i,j], \
-                self.prob_null, alternative = 'greater')
+                if self.num_trial[i,j] >= 1:
+                    p_vals[i,j] = binomtest(self.obs[i,j], self.num_trial[i,j], \
+                    self.prob_null, alternative = 'greater').pvalue
+                else:
+                    p_vals[i,j] = 1
                 p_vals[j,i] = p_vals[i,j]
         return p_vals
 
     def prob_null_hypothesis(self):
         '''
         Using a KDTree, find all pairs of genes in a cell that are under distance `distance_threshold`
         '''
@@ -205,15 +214,15 @@
         return prob_null
 
     def num_trial_pairs(self):  #Reindexed with geneList
         '''
         Count for each gene pair, the number of times they are proximal given the `distance_threshold`
         '''
         genecount = pd.DataFrame.from_dict(Counter(self.genes) , orient='index').reindex(self.geneList).fillna(0)
-        num_trial_pairs = np.dot(genecount, genecount.T)   #n1*n2  #using numpy here now
+        num_trial_pairs = np.dot(genecount, genecount.T).astype(np.int64)   #n1*n2  #using numpy here now
         return genecount, num_trial_pairs
 
     def obs_trial_pairs(self): #debug for large d
         '''
         After counting all gene pairs within the distance threshold, create a pivot table to create a 2d represtation
         and fill in the missing genes.
         '''
@@ -228,15 +237,15 @@
             for row_na in row_na_genes:
                 obs_df.loc[row_na] = 0
             obs_df = obs_df.reindex(index = self.geneList, columns = self.geneList)
         else:                                       #if no entry less than dist thresh
             obs_df = pd.DataFrame(0, self.geneList, self.geneList)
         temp= obs_df.values
         arr2 = temp + temp.T - temp*np.identity(len(temp))
-        return arr2
+        return arr2.astype(np.int64)
     
 class ProximalPairs3D():
     '''
         Calculates proximal pairs for all gene-gene pairs for a given cell.
         Arguments: 
             - geneList: (Array) List of genes.
             - df_loc: (DataFrame) Coordinates of the gene transcript.
@@ -282,22 +291,25 @@
             genecount_all = np.array(genecount_all).sum(axis = 0)
             prob_null_all = sum(x * y for x, y in zip(prob_null_all, len_prob_null_all))/sum(len_prob_null_all)
         else:       #useless cells, edge case
             obs_all = np.zeros((len(self.geneList), len(self.geneList)))
             num_trial_all = np.zeros((len(self.geneList), len(self.geneList)))
             genecount_all = np.zeros(len(self.geneList))
             prob_null_all = 1      
-        return obs_all, num_trial_all, genecount_all, prob_null_all
+        return obs_all, num_trial_all.astype(np.int64), genecount_all.astype(np.int64), prob_null_all
 
     def compute_p_val(self):
         p_vals = np.ones((len(self.geneList), len(self.geneList)))
         for i in range(obs.shape[0]):
             for j in range(i, obs.shape[1]):
-                p_vals[i,j] = binom_test(obs[i,j], self.num_trial[i,j], \
-                self.prob_null, alternative = 'greater')
+                if self.num_trial[i,j] >= 1:
+                    p_vals[i,j] = binomtest(obs[i,j], self.num_trial[i,j], \
+                    self.prob_null, alternative = 'greater').pvalue
+                else:
+                    p_vals[i,j] = 1
                 p_vals[j,i] = p_vals[i,j]
         return p_vals
 
 
 class SpatialModulation:
     def __init__(self, edge_all_cells, pos_cells, dist, geneList, file_name, min_num_neighbor = 1, threads = 1, adata_filename = None):
         self.edge_all_cells = edge_all_cells
@@ -583,40 +595,142 @@
         print("Unconditional Completed ....")
 
         all_pairs_cond_df = pd.DataFrame(all_pairs_cond, index = self.geneList, columns = self.geneList)
         all_pairs_uncond_df = pd.DataFrame(all_pairs_uncond, index = self.geneList, columns = self.geneList)
         all_pairs_g1_df = pd.DataFrame(all_pairs_g1, index = self.geneList)
         return all_pairs_cond_df, all_pairs_uncond_df, all_pairs_g1_df
 
+class CreateGraphFSM():
+    def __init__(self, filename, distance_threshold, alpha=0.001, self_loop=False):
+        adata = ad.read_h5ad(filename)
+        self.alpha = alpha
+        self.all_p_val = adata.uns[f'pp_test_d{distance_threshold}_pvalues']
+        self.self_loop = self_loop
+        self.adj_matrices = self.adj_matrix_all_cells()
+        self.geneList = adata.uns['geneList']
+        del adata
+        self.create_graph_all()
+
+    def adj_matrix_all_cells(self):
+        adj_matrices = np.zeros(self.all_p_val.shape)
+        adj_matrices[self.all_p_val <= self.alpha] = 1
+        return adj_matrices
+
+    def create_graph_all(self):
+        num_cells = self.adj_matrices.shape[0]
+        myfile = open('graph.txt', 'w+')
+        for i in range(num_cells):
+            self.create_graph(i, myfile)
+        myfile.write("t # %d \n" %(-1))
+
+    def create_graph(self, i, myfile):
+        curr_adj_mat = self.adj_matrices[i,:,:]
+        if not self.self_loop:
+            np.fill_diagonal(curr_adj_mat, 0)
+        if (curr_adj_mat.sum()):
+            node_indices = range(curr_adj_mat.shape[0])
+            node_indices = [['v', node_indices[i], self.geneList[node_indices[i]]] for i in range(len(node_indices))]
+            myfile.write("t # %d \n" %(i))
+            np.savetxt(myfile, node_indices, delimiter=',', fmt='%s %s %s') 
+            [edge_x, edge_y] = np.nonzero(curr_adj_mat)
+            edge_indices = [['e', edge_x[i],edge_y[i],1] for i in range(len(edge_x))]
+            np.savetxt(myfile, edge_indices, delimiter=',', fmt= '%s %s %s %s') 
+
 class GeneModuleDiscovery():
     '''
-    TODO #Globalcolo MAP , Frequent subgraph mining(using gspan)
+    Frequent subgraph mining(using gspan)
     '''
-    def __init__(self) -> None:
-        pass
+    def __init__(self, n_vertices, distance_threshold, alpha, clique = True, n_edges = None, filename = None, fsm_name = None):
+        self.n_vertices = n_vertices
+        self.fsm_name = fsm_name
+        if clique == True:
+            self.n_edges = np.math.comb(n_vertices, 2)
+        else:
+            self.n_edges = n_edges
+        if not os.path.exists("graph.txt"):
+            print("Creating graph file")
+            CreateGraphFSM(filename, alpha = alpha, distance_threshold = distance_threshold)
+        adata = ad.read_h5ad(filename)
+        adata = self._run_gspan(adata)
+        adata.write(Path(filename), compression="gzip")
+    
+    def _is_clique(self, g):
+        vertices = g.vertices
+        deg_list = [len(vertices[v].edges) for v in vertices]
+        edge_count = int(np.sum(deg_list)//2)
+        v_count = len(vertices)
+        if edge_count == v_count*(v_count-1)/2:
+            return True
+        return False
+    
+    def _prob_format(self, g):
+        vertices = g.vertices
+        vertex_map = dict([(vertices[v].vid, vertices[v].vlb) for v in vertices])
+        edge_dict_lists = [vertices[v].edges for v in vertices]
+        all_edge_list = []
+        for edge_dict in edge_dict_lists:
+            for key in list(edge_dict.keys()):
+                new_edge = (edge_dict[key].frm, edge_dict[key].to)
+                all_edge_list.append(new_edge)
+        G = nx.from_edgelist(all_edge_list)
+        adj_mat = nx.to_numpy_array(G)
+        np.fill_diagonal(adj_mat, 0)
+        return vertex_map, adj_mat
+    
+    def _node_count(self, g):
+        vertices = g.vertices
+        return len(vertices)
+    
+    def _edge_count(self, g):
+        vertices = g.vertices
+        deg_list = [len(vertices[v].edges) for v in vertices]
+        edge_count = int(np.sum(deg_list)//2)
+        return edge_count
+    
+    def _run_gspan(self, adata):
+        args_str = f"graph.txt -s 5 -d False -p False -w False -t False -v False -l {self.n_vertices} -e {self.n_edges}"
+        FLAGS, _ = parser.parse_known_args(args=args_str.split())
+        gs = main(FLAGS)
+        filtered_subgraphs = gs.filtered_subgraphs
+        support_list = []
+        cliques = []
+        for g, support in filtered_subgraphs:
+            if self._edge_count(g) == self.n_edges and self._node_count(g) == self.n_vertices:
+                vertex_map, adj_mat  = self._prob_format(g)
+                cliques.append([support, ','.join(vertex_map.values()), self.n_edges])   
+                support_list.append(support)
+        sorted_cliques = sorted(cliques, key=lambda x: x[0], reverse=True)
+        support_list.sort(reverse=True)
+        df = pd.DataFrame(sorted_cliques, columns=["Support", "Vertices", "Number of Edges"])
+        if self.fsm_name == None:
+            adata.uns[f"nV{self.n_vertices}_cliques"] = df
+        else:
+            adata.uns[self.fsm_name] = df
+        return adata
 
 class Instant():
     '''
     Intracellular Spatial Transcriptomic Analysis Toolkit (InSTAnT).
     This class is used to calculate the proximal gene pairs in each cell and 
     used to find which gene pairs are d-cololocalised across all the cells.
         Arguments: 
             - threads: (Integer) Number of threads to use.
             - min_intensity: (Optional) (Integer) Minimum intensity for Merfish.
             - min_area: (Optional) (Integer) Minimum Area for Merfish.
     '''
-    def __init__(self, threads = 1, precision_mode = "high", min_intensity = 0, min_area = 0):
+    def __init__(self, distance_threshold, threads = 1, precision_mode = "high", min_intensity = 0, min_area = 0):
+        self.distance_threshold = distance_threshold
         self.min_intensity, self.min_area = min_intensity, min_area
         self.threads = threads
         if precision_mode:
             self.precision_mode = np.float64
         else:
             self.precision_mode = np.float16
 
-    def load_preprocessed_data(self, data, inNucleus = False):
+    def load_preprocessed_data(self, data, adata_name = None, inNucleus = False, force_csv = False):
         '''
         Load preprocessed data. Data can either be a '.csv' or a '.h5ad' file.
         If AnnData file is passed, the csv file is expected in `adata.uns['transcripts']`
         The csv should have should have the following columns - 
             ['gene', 'absX', 'absY', 'uID'] with 'gene' being the 1st column
             Arguments: 
                 - data: (String) Path to dataframe in the required format.
@@ -625,26 +739,31 @@
         if Path(self.filename).suffix.lower() == ".csv":
             self.df = pd.read_csv(data)
             counts = pd.crosstab(self.df.uID, self.df.gene)
             adata = ad.AnnData(counts.values)
             adata.obs_names = counts.index.values
             adata.var_names = counts.columns.values
             adata.uns["transcripts"] = self.df
-            adata.write(Path(self.filename).with_suffix('.h5ad'), compression="gzip")
-            self.filename = Path(self.filename).with_suffix('.h5ad')
+            if force_csv == False:
+                if adata_name == None:
+                    adata.write(Path(self.filename).with_suffix('.h5ad'), compression="gzip")
+                    self.filename = Path(self.filename).with_suffix('.h5ad')
+                else:
+                    self.filename = (Path(self.filename).parent / adata_name).with_suffix('.h5ad')
+                    adata.write(Path(self.filename), compression="gzip")
             self.df = self.df.set_index('gene').sort_index()
         elif Path(self.filename).suffix.lower() == ".h5ad":
             adata = ad.read_h5ad(self.filename)
             self.df = adata.uns['transcripts']
             self.df = self.df.set_index('gene').sort_index()
         else:
             raise("Input File Format Incorrect")
         if inNucleus:
             self.df = self.df[self.df.inNucleus == 1]
-        self.geneList = self.df.index.unique()
+        self.geneList = np.unique(self.df.index)
         print("Loaded Data. Number of Transcripts: ", len(self.df), ", Number of Genes: ", len(self.geneList), 
               ", Number of Cells: ", len(self.df.uID.unique()))
     
     def load_preprocessed_data_randomize(self, data):
         '''
         Load preprocessed data and randomize the genes (to establish baselines). Data should have the following columns - 
             ['gene', 'absX', 'absY', 'uID'] with 'gene' being the 1st column
@@ -888,19 +1007,19 @@
                 print(f"Running PP now on {self.threads} threads for, {len(valid_cell_data)} cells, {num_transcripts} transcripts")
                 results = pool.map(self._calculate_ProximalPairs, valid_cell_data)
         self.all_pval = np.ones((num_cells, len(self.geneList), len(self.geneList)), dtype = self.precision_mode)
         self.all_gene_count = np.zeros((num_cells, len(self.geneList)), dtype = self.precision_mode) 
         for cell_i_result in results:
             self.all_pval[cell_i_result[0]] = cell_i_result[1]
             self.all_gene_count[cell_i_result[0]] = cell_i_result[2]
-        print(f"Time to complete PP : ", timeit.default_timer() - check)
         if Path(self.filename).suffix.lower() == ".h5ad":
             adata = ad.read_h5ad(self.filename)
             adata.obsm['genecount'] = self.all_gene_count
-            adata.uns['pp_test_pvalues'] = self.all_pval
+            adata.uns[f'pp_test_d{self.distance_threshold}_pvalues'] = self.all_pval
+            adata.uns['geneList'] = self.geneList
             adata.write(self.filename, compression="gzip")
         if pval_matrix_name:
             self._save_pval_matrix(pval_matrix_name)
         if gene_count_name:
             self._save_gene_count(gene_count_name)
         self.df = df_copy
         del df_copy
@@ -923,15 +1042,15 @@
                 - pval_matrix_name: (String) (Optional) if provided saves pvalue matrix using pickle at the input path.
                 - gene_count_name: (String) (Optional) if provided saves gene expression count matrix using pickle at the input path.
         '''
         self.distance_threshold = distance_threshold
         cell_ids = np.unique(self.df.uID)
         num_cells = len(cell_ids)
         num_genes = len(self.geneList)
-        print(f"Initialised PP now on {self.threads} threads")
+        print(f"Initialised PP-3D now on {self.threads} threads")
         print("Number of cells: ", num_cells, ", Number of Genes: ", num_genes)
         start = timeit.default_timer()
         valid_cell_data = []
         num_transcripts = 0
         celllabel_encoder = LabelEncoder()
         cell_labels = celllabel_encoder.fit_transform(self.df['uID'])
         self.df['uID_encoded'] = cell_labels
@@ -955,19 +1074,19 @@
             print(f"Running PP-3D now on {self.threads} threads for, {len(valid_cell_data)} cells, {num_transcripts} transcripts")
             results = pool.map(self._calculate_ProximalPairs3D, valid_cell_data)
         self.all_pval = np.ones((num_cells, len(self.geneList), len(self.geneList)), dtype = self.precision_mode)
         self.all_gene_count = np.zeros((num_cells, len(self.geneList)), dtype = self.precision_mode) 
         for cell_i_result in results:
             self.all_pval[cell_i_result[0]] = cell_i_result[1]
             self.all_gene_count[cell_i_result[0]] = cell_i_result[2]
-        print(f"Time to complete PP : ", timeit.default_timer() - check)
         if Path(self.filename).suffix.lower() == ".h5ad":
             adata = ad.read_h5ad(self.filename)
             adata.obsm['genecount'] = self.all_gene_count
-            adata.uns['pp_test_pvalues'] = self.all_pval
+            adata.uns[f'pp_test_d{self.distance_threshold}_pvalues'] = self.all_pval
+            adata.uns['geneList'] = self.geneList
             adata.write(self.filename, compression="gzip")
         if pval_matrix_name:
             self._save_pval_matrix(pval_matrix_name)
         if gene_count_name:
             self._save_gene_count(gene_count_name)
         self.df = df_copy
         del df_copy
@@ -1093,15 +1212,15 @@
                 - gene_count_name: (String) (Optional) if provided saves gene expression count matrix using pickle at the input path.
         '''
         self.distance_threshold = distance_threshold
         self.min_genecount = min_genecount
         cell_ids = np.unique(self.df.uID)
         num_cells = len(cell_ids)
         num_genes = len(self.geneList)
-        print(f"Initialised PP-3D now on {self.threads} threads")
+        print(f"Initialised PP-3D slice now on {self.threads} threads")
         print("Number of cells: ", num_cells, ", Number of Genes: ", num_genes)
         start = timeit.default_timer()
         valid_cell_data = []
         num_transcripts = 0
         celllabel_encoder = LabelEncoder()
         cell_labels = celllabel_encoder.fit_transform(self.df['uID'])
         self.df['uID_encoded'] = cell_labels
@@ -1118,26 +1237,26 @@
         df = self.df.copy()
         del self.df
         position_matrix_3d = df[['absX', 'absY', 'absZ', 'uID_encoded']].to_numpy().copy(order='C')
         share_pp3d = mp.RawArray('d', len(position_matrix_3d)*4)
         share_pp3d_np = np.frombuffer(share_pp3d).reshape(position_matrix_3d.shape)
         np.copyto(share_pp3d_np, position_matrix_3d)
         print(f"Running PP-3D slice now on {self.threads} threads for, {len(valid_cell_data)} cells, {num_transcripts} transcripts")
-        with mp.Pool(processes=self.threads, initializer=self._initializer_func_pp, initargs=(position_matrix_3d, position_matrix_3d.shape), maxtasksperchild = 1) as pool:
+        with mp.pool.Pool(processes=self.threads, initializer=self._initializer_func_pp, initargs=(position_matrix_3d, position_matrix_3d.shape)) as pool:
             results = pool.map(self._calculate_ProximalPairs3D_slice, valid_cell_data)
         self.all_pval = np.ones((num_cells, len(self.geneList), len(self.geneList)), dtype = self.precision_mode)
         self.all_gene_count = np.zeros((num_cells, len(self.geneList)), dtype = self.precision_mode) 
         for cell_i_result in results:
             self.all_pval[cell_i_result[0]] = cell_i_result[1]
             self.all_gene_count[cell_i_result[0]] = cell_i_result[2]
-        print(f"Time to complete PP : ", timeit.default_timer() - check)
         if Path(self.filename).suffix.lower() == ".h5ad":
             adata = ad.read_h5ad(self.filename)
             adata.obsm['genecount'] = self.all_gene_count
-            adata.uns['pp_test_pvalues'] = self.all_pval
+            adata.uns[f'pp_test_d{self.distance_threshold}_pvalues'] = self.all_pval
+            adata.uns['geneList'] = self.geneList
             adata.write(self.filename, compression="gzip")
         if pval_matrix_name:
             self._save_pval_matrix(pval_matrix_name)
         if gene_count_name:
             self._save_gene_count(gene_count_name)
         self.df = df
         del df
@@ -1160,15 +1279,15 @@
                 if Path(cell_locations).suffix.lower() == ".csv":
                     self.cell_locations = pd.read_csv(cell_locations)
             else:
                 try:
                     self.cell_locations = adata.uns['cell_locations']
                 except:
                     raise("Cell Locations file format incorrect")  
-            self.all_pval = adata.uns['pp_test_pvalues']
+            self.all_pval = adata.uns[f'pp_test_d{self.distance_threshold}_pvalues']
             self.all_gene_count = adata.obsm['genecount']
         binary_pp_pval = np.zeros(self.all_pval.shape)
         binary_pp_pval[self.all_pval < alpha] = 1
         if randomize:
             self.cell_locations.uID = np.random.permutation(self.cell_locations.uID.values)
         SpatialModulation(binary_pp_pval, self.cell_locations, inter_cell_distance, file_name = spatial_modulation_name, geneList = self.geneList, threads = self.threads, adata_filename = self.filename)
 
@@ -1199,19 +1318,25 @@
                     self.cell_labels = pd.read_csv(cell_labels)
             else:
                 try:
                     self.cell_labels = adata.obs
                     self.cell_labels['uID'] = self.cell_labels.index.values
                 except:
                     raise("Cell Label file format incorrect")        
-            self.all_pval = adata.uns['pp_test_pvalues']
+            self.all_pval = adata.uns[f'pp_test_d{self.distance_threshold}_pvalues']
             self.all_gene_count = adata.obsm['genecount']
             if 'differential_colocalization' not in adata.uns:
                 adata.uns['differential_colocalization'] = {}
             adata.write(self.filename, compression="gzip")
+        else:
+            if cell_labels != None:
+                if Path(cell_labels).suffix.lower() == ".csv":
+                    self.cell_labels = pd.read_csv(cell_labels)
+            else:
+                raise("Cell Label file format incorrect")
         start = timeit.default_timer()
         print(f"Running Differential Colocalization now on {self.threads} threads")
         if mode == "1va":
             selected_cell_ids = self.cell_labels[self.cell_labels.cell_type == cell_type].uID.values
             rest_cell_ids = list(set(self.cell_labels.uID.values).difference(set(selected_cell_ids)))
             selected_cell_indices = [np.where(cell_ids == celllabel_encoder.transform([x])[0])[0][0] for x in selected_cell_ids]
             rest_cell_indices = [np.where(cell_ids == celllabel_encoder.transform([x])[0])[0][0] for x in rest_cell_ids]
@@ -1301,15 +1426,15 @@
             - glob_coloc_name: (String) (Optional) if provided saves global colocalization matrix as a csv at the input path.
             - exp_coloc_name: (String) (Optional) if provided saves expected colocalization matrix as a csv at the input path.
             - unstacked_pvals_name: (String) (Optional) if provided saves interpretable global colocalization matrix as a csv at the input path.
         '''
         print(f"Running Global Colocalization now on {self.threads} threads")
         if Path(self.filename).suffix.lower() == ".h5ad":
             adata = ad.read_h5ad(self.filename)
-            self.all_pval = adata.uns['pp_test_pvalues']
+            self.all_pval = adata.uns[f'pp_test_d{self.distance_threshold}_pvalues']
             self.all_gene_count = adata.obsm['genecount']
         start = timeit.default_timer()
         global_coloc_model = ConditionalGlobalColocalization(all_pvals = self.all_pval, transcript_count = self.all_gene_count, alpha_cellwise = alpha_cellwise, min_transcript = min_transcript, threads = self.threads, high_precision = high_precision, precision_mode = self.precision_mode)
         global_coloc, expected_coloc = global_coloc_model.global_colocalization()
         self.global_coloc_df = pd.DataFrame(global_coloc, index = self.geneList, columns = self.geneList)
         self.expected_coloc_df = pd.DataFrame(expected_coloc, index = self.geneList, columns = self.geneList)
         if Path(self.filename).suffix.lower() == ".h5ad":
@@ -1317,8 +1442,25 @@
             adata.write(self.filename, compression="gzip")
         if glob_coloc_name:
             self._save_globcolocal_csv(glob_coloc_name)
         if exp_coloc_name:
             self._save_expcolocal_csv(exp_coloc_name)
         if unstacked_pvals_name:
             self._save_unstacked_pvals(unstacked_pvals_name, alpha_cellwise, min_transcript)
-        print(f"Cell-wise Global Colocalization Time : {round(timeit.default_timer() - start, 2)} seconds")
+        print(f"Cell-wise Global Colocalization Time : {round(timeit.default_timer() - start, 2)} seconds")
+
+    def run_fsm(self, n_vertices, alpha = 0.001, clique = True, n_edges = None, fsm_name = None):
+        '''
+        Finds networks of genes colocalized in many cells using gSpan(https://github.com/betterenvi/gSpan). FSM can be used to find networks with a pre-specified minimum size that are supported by a large number of cells
+        Requires `run_ProximalPairs()` be run first to generate the p-value matrix for all cells. Processes the p-value matrix to create a graph(saved as graph.txt) with edges based on alpha(p-value threshold).
+        Generates a dataframe with all such networks found.
+        Arguments: 
+            - n_vertices: (int) Minimum number of vertices in the network.
+            - alpha: (Float) (Float) pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.001.
+            - clique: (Boolean) Forces networks found to be fully connected. Number of edges is number of vertices choose 2. Default = False.
+            - n_edges: (int) (Optional) Minimum number of edges in the network. Works only when clique == False.
+            - fsm_name: (String) (Optional) Name of adata.uns key to save output in. Be sure to specify if `run_fsm` is ran multiple times because it will overwrite. Default = "nV{x}_cliques" where x is the number of vertices.
+        '''
+        print(f"Running Frequent Subgraph Mining")
+        start = timeit.default_timer()
+        GeneModuleDiscovery(n_vertices = n_vertices, alpha = alpha, clique = clique, filename = self.filename, fsm_name = fsm_name, n_edges = n_edges, distance_threshold = self.distance_threshold)
+        print(f"Frequent Subgraph Mining Time : {round(timeit.default_timer() - start, 2)} seconds")
```

### Comparing `sc-instant-1.1/InSTAnT/poibin.py` & `sc_instant-1.2/InSTAnT/poibin.py`

 * *Files identical despite different names*

### Comparing `sc-instant-1.1/InSTAnT/poisson_binomial.py` & `sc_instant-1.2/InSTAnT/poisson_binomial.py`

 * *Files identical despite different names*

### Comparing `sc-instant-1.1/PKG-INFO` & `sc_instant-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-instant
-Version: 1.1
+Version: 1.2
 Summary: InSTAnT is a toolkit to identify gene pairs which are d-colocalized from single molecule measurement data.
 Home-page: https://github.com/anurendra, https://github.com/Chokerino
 Author: Anurendra Kumar, Bhavay Aggarwal
 Author-email: anu.ankesh@gmail.com, bhavayaggarwal07@gmail.com
 License: MIT
 Keywords: InSTAnT,Python
 Classifier: Development Status :: 3 - Alpha
@@ -12,57 +12,75 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Requires-Dist: contourpy==1.1.1
-Requires-Dist: cycler==0.12.1
-Requires-Dist: et-xmlfile==1.1.0
-Requires-Dist: fonttools==4.43.1
-Requires-Dist: joblib==1.3.2
-Requires-Dist: kiwisolver==1.4.5
-Requires-Dist: matplotlib==3.8.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: packaging==23.2
-Requires-Dist: pillow==10.1.0
-Requires-Dist: psutil==5.9.6
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.3
-Requires-Dist: threadpoolctl==3.2.0
-Requires-Dist: pandas==2.1.4
-Requires-Dist: anndata==0.10.4
+License-File: LICENSE.txt
+Requires-Dist: contourpy>=1.1.1
+Requires-Dist: cycler>=0.12.1
+Requires-Dist: et-xmlfile>=1.1.0
+Requires-Dist: fonttools>=4.43.1
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: kiwisolver>=1.4.5
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: packaging>=23.2
+Requires-Dist: pillow>=10.1.0
+Requires-Dist: psutil>=5.9.6
+Requires-Dist: pyparsing>=3.1.1
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: scipy>=1.11.3
+Requires-Dist: threadpoolctl>=3.2.0
+Requires-Dist: pandas>=2.1.4
+Requires-Dist: anndata>=0.10.4
+Requires-Dist: gspan-mining>=0.2.3
+Requires-Dist: networkx>=3.2.1
 
 InSTAnT
 =========
 
+[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/bhavaygg/InSTAnT/blob/main/LICENSE.txt)
+[![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/sc-instant/)
+[![Downloads](https://pepy.tech/badge/sc-instant)](https://www.pepy.tech/projects/sc-instant)
+
+
 **InSTAnT** is a toolkit to identify gene pairs which are d-colocalized
 from single molecule measurement data e.g. MERFISH or SeqFISH. A gene
 pair is d-colocalized when their transcripts are within distance d
 across many cells.
 
 This repository contains implementation of PP Test and CPB test and demo
 on a U2OS dataset. The dataset can be downloaded from here (Moffit et
 al., 2016, PNAS ) -
 http://zhuang.harvard.edu/MERFISHData/data_for_release.zip 
 
-### UPDATE: Added support for AnnData input/output.
+Paper Preprint Link - https://pubmed.ncbi.nlm.nih.gov/36747718/
+
+
+### UPDATE: Added support for AnnData input/output. Added Frequent Subgraph Mining.
 
 We recommend using our `environment.yml` file to create a new conda environment to avoid issues with package incompatibility.
 
 ```
 conda env create -f environment.yml
 ```
-This will create a new conda environment with the name `instant` and has all dependancies installed. 
+This will create a new conda environment with the name `instant` and has all dependencies installed. 
+
+Alternatively, the package can be installed using pip.
+
+```
+pip install sc-instant
+```
 
-First we will initialise the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
+First, we will initialize the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
 
 ```
+from InSTAnT import Instant
 obj = Instant(threads = threads, precision_mode = 'high', min_intensity = 10**0.75, min_area = 3)
 ```
 
 To load MERFISH data, we use the function `preprocess_and_load_data()`. `preprocess_and_load_data()` is used to preprocess and load MERFISH data ***only***. The final data is stored as a pandas DataFrame and the following columns `['gene', 'uID', 'absX', 'absY']`. Below is an example table for a 2D data (if the data is 3D, `absZ` column is also expected) - 
 
 | gene | uID | absX | absY |
 | :---         |     :---:      |          ---: |           ---: |
@@ -93,17 +111,17 @@
 ```
 obj.run_ProximalPairs(distance_threshold = 4, min_genecount = 20, 
     pval_matrix_name = f"data/u2os/rep3/rep3_pvals.pkl", 
     gene_count_name = f"data/u2os/rep3/rep3_gene_count.pkl")
 ```
 Proximal Pairs calculation has 3 variants - 
   - `run_ProximalPairs()` - Designed for 2D subcellular spatial transcriptomics data.
-  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continuos z-axis.
+  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continous z-axis.
   - `run_ProximalPairs3D_slice()` - Designed for 3D subcellular spatial transcriptomics data with discrete/sliced z-axis.
-(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_pvalues']`.)
+(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_d{distance_threshold}_pvalues']`.)
 
 All subsequent analysis require `run_ProximalPairs()` to be run first to generate the p-value matrix for all cells.
 
 Next, we can use the output to find which gene pairs are significantly colocalized globally using the `run_GlobalColocalization()` function. The following arguments are used by `run_GlobalColocalization()`
   - `alpha_cellwise`: *(Float)* Pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.05.
   - `min_transcript`: *(Float)* Gene expression lower threshold. Default = 0.
   - `high_precision`: *(Boolean*) High precision pvalue. Expect a longer compute time. Default = False.
@@ -215,7 +233,37 @@
     | Slc17a6, Syt4   | 2.27E-75 | 6.75E-08  | 6.67E-64  | 5.8E-304        | 1.48E-17        | 5.8E-304 | 1       | 22      | 1        |
     | Cbln1, Slc17a6  | 2.58E-58 | 6.29E-14  | 5.01E-12  | 2.1E-131        | 5.8E-304        | 5.8E-304 | 2       | 1       | 1        |
     | Gabra1, Slc17a6 | 1.01E-53 | 6.75E-45  | 5.89E-06  | 4.39E-13        | 5.8E-304        | 5.8E-304 | 27      | 1       | 1        |
     | Cbln1, Gpr165   | 6.64E-39 | 1.5E-08   | 6.27E-43  | 2.1E-131        | 0.999642        | 2.1E-131 | 2       | 95      | 2        |
     | Cbln1, Syt4     | 4.29E-36 | 1.55E-10  | 1.35E-32  | 2.1E-131        | 1.48E-17        | 2.1E-131 | 2       | 22      | 2        |
 
 (**Note** - For AnnData objects. These results are stored in `adata.uns['differential_colocalization']`. `adata.uns['differential_colocalization']` is a dictionary with keys based on the analysis done. For `1va` and `ava`, the key is `{cell_type}` and for `1v1`, the key is `{cell_type)_vs_{cell_type_2}`).
+
+### UPDATE: Frequent Subgraph Mining.
+
+Finds networks of genes colocalized in many cells using [gSpan](https://github.com/betterenvi/gSpan). The networks found are potential candidates for groups of cells and genes exhibiting interesting subcellular patterns, in this case colocalization.
+Such colocalization networks could potentially be underlying factors for specific biological processes.
+
+```
+obj.run_fsm(n_vertices = 4, alpha = 0.001)
+```
+
+Arguments: 
+  - `n_vertices`: *(int)* Minimum number of vertices in the network.
+  - `alpha`: *(Float)* *(Float)* pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.001.
+  - `clique`: *(Boolean)* Forces networks found to be fully connected. Number of edges is number of vertices choose 2. Default = False.
+  - `n_edges`: *(int) *(Optional)* Minimum number of edges in the network. Works only when clique == False.
+  - `fsm_name`: *(String)* *(Optional)* Name of adata.uns key to save output in. Be sure to specify if `run_fsm` is ran multiple times because it will overwrite. Default = "nV{x}_cliques" where x is the number of vertices.
+
+THe function will create a dataframe in `adata.uns` with all the gene pair networks found. Ny default the key is `nV{x}_cliques` where x is the number of vertices but using the attribute `fsm_name` it can be changed. 
+
+## Citation 
+
+```
+@article{kumar2023intracellular,
+  title={Intracellular Spatial Transcriptomic Analysis Toolkit (InSTAnT)},
+  author={Kumar, Anurendra and Schrader, Alex W and Boroojeny, Ali Ebrahimpour and Asadian, Marisa and Lee, Juyeon and Song, You Jin and Zhao, Sihai Dave and Han, Hee-Sun and Sinha, Saurabh},
+  journal={Research Square},
+  year={2023},
+  publisher={American Journal Experts}
+}
+```
```

### Comparing `sc-instant-1.1/README.md` & `sc_instant-1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 InSTAnT
 =========
 
+[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/bhavaygg/InSTAnT/blob/main/LICENSE.txt)
+[![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/sc-instant/)
+[![Downloads](https://pepy.tech/badge/sc-instant)](https://www.pepy.tech/projects/sc-instant)
+
+
 **InSTAnT** is a toolkit to identify gene pairs which are d-colocalized
 from single molecule measurement data e.g. MERFISH or SeqFISH. A gene
 pair is d-colocalized when their transcripts are within distance d
 across many cells.
 
 This repository contains implementation of PP Test and CPB test and demo
 on a U2OS dataset. The dataset can be downloaded from here (Moffit et
 al., 2016, PNAS ) -
 http://zhuang.harvard.edu/MERFISHData/data_for_release.zip 
 
-### UPDATE: Added support for AnnData input/output.
+Paper Preprint Link - https://pubmed.ncbi.nlm.nih.gov/36747718/
+
+
+### UPDATE: Added support for AnnData input/output. Added Frequent Subgraph Mining.
 
 We recommend using our `environment.yml` file to create a new conda environment to avoid issues with package incompatibility.
 
 ```
 conda env create -f environment.yml
 ```
-This will create a new conda environment with the name `instant` and has all dependancies installed. 
+This will create a new conda environment with the name `instant` and has all dependencies installed. 
+
+Alternatively, the package can be installed using pip.
+
+```
+pip install sc-instant
+```
 
-First we will initialise the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
+First, we will initialize the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
 
 ```
+from InSTAnT import Instant
 obj = Instant(threads = threads, precision_mode = 'high', min_intensity = 10**0.75, min_area = 3)
 ```
 
 To load MERFISH data, we use the function `preprocess_and_load_data()`. `preprocess_and_load_data()` is used to preprocess and load MERFISH data ***only***. The final data is stored as a pandas DataFrame and the following columns `['gene', 'uID', 'absX', 'absY']`. Below is an example table for a 2D data (if the data is 3D, `absZ` column is also expected) - 
 
 | gene | uID | absX | absY |
 | :---         |     :---:      |          ---: |           ---: |
@@ -57,17 +72,17 @@
 ```
 obj.run_ProximalPairs(distance_threshold = 4, min_genecount = 20, 
     pval_matrix_name = f"data/u2os/rep3/rep3_pvals.pkl", 
     gene_count_name = f"data/u2os/rep3/rep3_gene_count.pkl")
 ```
 Proximal Pairs calculation has 3 variants - 
   - `run_ProximalPairs()` - Designed for 2D subcellular spatial transcriptomics data.
-  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continuos z-axis.
+  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continous z-axis.
   - `run_ProximalPairs3D_slice()` - Designed for 3D subcellular spatial transcriptomics data with discrete/sliced z-axis.
-(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_pvalues']`.)
+(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_d{distance_threshold}_pvalues']`.)
 
 All subsequent analysis require `run_ProximalPairs()` to be run first to generate the p-value matrix for all cells.
 
 Next, we can use the output to find which gene pairs are significantly colocalized globally using the `run_GlobalColocalization()` function. The following arguments are used by `run_GlobalColocalization()`
   - `alpha_cellwise`: *(Float)* Pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.05.
   - `min_transcript`: *(Float)* Gene expression lower threshold. Default = 0.
   - `high_precision`: *(Boolean*) High precision pvalue. Expect a longer compute time. Default = False.
@@ -179,7 +194,37 @@
     | Slc17a6, Syt4   | 2.27E-75 | 6.75E-08  | 6.67E-64  | 5.8E-304        | 1.48E-17        | 5.8E-304 | 1       | 22      | 1        |
     | Cbln1, Slc17a6  | 2.58E-58 | 6.29E-14  | 5.01E-12  | 2.1E-131        | 5.8E-304        | 5.8E-304 | 2       | 1       | 1        |
     | Gabra1, Slc17a6 | 1.01E-53 | 6.75E-45  | 5.89E-06  | 4.39E-13        | 5.8E-304        | 5.8E-304 | 27      | 1       | 1        |
     | Cbln1, Gpr165   | 6.64E-39 | 1.5E-08   | 6.27E-43  | 2.1E-131        | 0.999642        | 2.1E-131 | 2       | 95      | 2        |
     | Cbln1, Syt4     | 4.29E-36 | 1.55E-10  | 1.35E-32  | 2.1E-131        | 1.48E-17        | 2.1E-131 | 2       | 22      | 2        |
 
 (**Note** - For AnnData objects. These results are stored in `adata.uns['differential_colocalization']`. `adata.uns['differential_colocalization']` is a dictionary with keys based on the analysis done. For `1va` and `ava`, the key is `{cell_type}` and for `1v1`, the key is `{cell_type)_vs_{cell_type_2}`).
+
+### UPDATE: Frequent Subgraph Mining.
+
+Finds networks of genes colocalized in many cells using [gSpan](https://github.com/betterenvi/gSpan). The networks found are potential candidates for groups of cells and genes exhibiting interesting subcellular patterns, in this case colocalization.
+Such colocalization networks could potentially be underlying factors for specific biological processes.
+
+```
+obj.run_fsm(n_vertices = 4, alpha = 0.001)
+```
+
+Arguments: 
+  - `n_vertices`: *(int)* Minimum number of vertices in the network.
+  - `alpha`: *(Float)* *(Float)* pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.001.
+  - `clique`: *(Boolean)* Forces networks found to be fully connected. Number of edges is number of vertices choose 2. Default = False.
+  - `n_edges`: *(int) *(Optional)* Minimum number of edges in the network. Works only when clique == False.
+  - `fsm_name`: *(String)* *(Optional)* Name of adata.uns key to save output in. Be sure to specify if `run_fsm` is ran multiple times because it will overwrite. Default = "nV{x}_cliques" where x is the number of vertices.
+
+THe function will create a dataframe in `adata.uns` with all the gene pair networks found. Ny default the key is `nV{x}_cliques` where x is the number of vertices but using the attribute `fsm_name` it can be changed. 
+
+## Citation 
+
+```
+@article{kumar2023intracellular,
+  title={Intracellular Spatial Transcriptomic Analysis Toolkit (InSTAnT)},
+  author={Kumar, Anurendra and Schrader, Alex W and Boroojeny, Ali Ebrahimpour and Asadian, Marisa and Lee, Juyeon and Song, You Jin and Zhao, Sihai Dave and Han, Hee-Sun and Sinha, Saurabh},
+  journal={Research Square},
+  year={2023},
+  publisher={American Journal Experts}
+}
+```
```

### Comparing `sc-instant-1.1/environment.yml` & `sc_instant-1.2/environment.yml`

 * *Files 12% similar despite different names*

```diff
@@ -51,7 +51,9 @@
       - packaging==23.2
       - pillow==10.1.0
       - psutil==5.9.6
       - pyparsing==3.1.1
       - scikit-learn==1.3.2
       - scipy==1.11.3
       - threadpoolctl==3.2.0
+      - pandas==2.1.4
+      - anndata==0.10.4
```

### Comparing `sc-instant-1.1/sc_instant.egg-info/PKG-INFO` & `sc_instant-1.2/sc_instant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-instant
-Version: 1.1
+Version: 1.2
 Summary: InSTAnT is a toolkit to identify gene pairs which are d-colocalized from single molecule measurement data.
 Home-page: https://github.com/anurendra, https://github.com/Chokerino
 Author: Anurendra Kumar, Bhavay Aggarwal
 Author-email: anu.ankesh@gmail.com, bhavayaggarwal07@gmail.com
 License: MIT
 Keywords: InSTAnT,Python
 Classifier: Development Status :: 3 - Alpha
@@ -12,57 +12,75 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Requires-Dist: contourpy==1.1.1
-Requires-Dist: cycler==0.12.1
-Requires-Dist: et-xmlfile==1.1.0
-Requires-Dist: fonttools==4.43.1
-Requires-Dist: joblib==1.3.2
-Requires-Dist: kiwisolver==1.4.5
-Requires-Dist: matplotlib==3.8.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: packaging==23.2
-Requires-Dist: pillow==10.1.0
-Requires-Dist: psutil==5.9.6
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.3
-Requires-Dist: threadpoolctl==3.2.0
-Requires-Dist: pandas==2.1.4
-Requires-Dist: anndata==0.10.4
+License-File: LICENSE.txt
+Requires-Dist: contourpy>=1.1.1
+Requires-Dist: cycler>=0.12.1
+Requires-Dist: et-xmlfile>=1.1.0
+Requires-Dist: fonttools>=4.43.1
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: kiwisolver>=1.4.5
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: packaging>=23.2
+Requires-Dist: pillow>=10.1.0
+Requires-Dist: psutil>=5.9.6
+Requires-Dist: pyparsing>=3.1.1
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: scipy>=1.11.3
+Requires-Dist: threadpoolctl>=3.2.0
+Requires-Dist: pandas>=2.1.4
+Requires-Dist: anndata>=0.10.4
+Requires-Dist: gspan-mining>=0.2.3
+Requires-Dist: networkx>=3.2.1
 
 InSTAnT
 =========
 
+[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/bhavaygg/InSTAnT/blob/main/LICENSE.txt)
+[![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/sc-instant/)
+[![Downloads](https://pepy.tech/badge/sc-instant)](https://www.pepy.tech/projects/sc-instant)
+
+
 **InSTAnT** is a toolkit to identify gene pairs which are d-colocalized
 from single molecule measurement data e.g. MERFISH or SeqFISH. A gene
 pair is d-colocalized when their transcripts are within distance d
 across many cells.
 
 This repository contains implementation of PP Test and CPB test and demo
 on a U2OS dataset. The dataset can be downloaded from here (Moffit et
 al., 2016, PNAS ) -
 http://zhuang.harvard.edu/MERFISHData/data_for_release.zip 
 
-### UPDATE: Added support for AnnData input/output.
+Paper Preprint Link - https://pubmed.ncbi.nlm.nih.gov/36747718/
+
+
+### UPDATE: Added support for AnnData input/output. Added Frequent Subgraph Mining.
 
 We recommend using our `environment.yml` file to create a new conda environment to avoid issues with package incompatibility.
 
 ```
 conda env create -f environment.yml
 ```
-This will create a new conda environment with the name `instant` and has all dependancies installed. 
+This will create a new conda environment with the name `instant` and has all dependencies installed. 
+
+Alternatively, the package can be installed using pip.
+
+```
+pip install sc-instant
+```
 
-First we will initialise the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
+First, we will initialize the Instant class object. This object will allow us to calculate the proximal pairs and find global colocalized genes. The primary argument is `threads` which controls the number of threads the program uses. If you run into memory issues with the default settings, we suggest setting the `precision_mode` to `low`. The arguments `min_intensity` and `min_area` are used only for MERFISH data preprocessing and can be skipped otherwise.
 
 ```
+from InSTAnT import Instant
 obj = Instant(threads = threads, precision_mode = 'high', min_intensity = 10**0.75, min_area = 3)
 ```
 
 To load MERFISH data, we use the function `preprocess_and_load_data()`. `preprocess_and_load_data()` is used to preprocess and load MERFISH data ***only***. The final data is stored as a pandas DataFrame and the following columns `['gene', 'uID', 'absX', 'absY']`. Below is an example table for a 2D data (if the data is 3D, `absZ` column is also expected) - 
 
 | gene | uID | absX | absY |
 | :---         |     :---:      |          ---: |           ---: |
@@ -93,17 +111,17 @@
 ```
 obj.run_ProximalPairs(distance_threshold = 4, min_genecount = 20, 
     pval_matrix_name = f"data/u2os/rep3/rep3_pvals.pkl", 
     gene_count_name = f"data/u2os/rep3/rep3_gene_count.pkl")
 ```
 Proximal Pairs calculation has 3 variants - 
   - `run_ProximalPairs()` - Designed for 2D subcellular spatial transcriptomics data.
-  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continuos z-axis.
+  - `run_ProximalPairs3D()` - Designed for 3D subcellular spatial transcriptomics data with continous z-axis.
   - `run_ProximalPairs3D_slice()` - Designed for 3D subcellular spatial transcriptomics data with discrete/sliced z-axis.
-(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_pvalues']`.)
+(**Note** - For AnnData objects. These results are stored in `adata.uns['pp_test_d{distance_threshold}_pvalues']`.)
 
 All subsequent analysis require `run_ProximalPairs()` to be run first to generate the p-value matrix for all cells.
 
 Next, we can use the output to find which gene pairs are significantly colocalized globally using the `run_GlobalColocalization()` function. The following arguments are used by `run_GlobalColocalization()`
   - `alpha_cellwise`: *(Float)* Pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.05.
   - `min_transcript`: *(Float)* Gene expression lower threshold. Default = 0.
   - `high_precision`: *(Boolean*) High precision pvalue. Expect a longer compute time. Default = False.
@@ -215,7 +233,37 @@
     | Slc17a6, Syt4   | 2.27E-75 | 6.75E-08  | 6.67E-64  | 5.8E-304        | 1.48E-17        | 5.8E-304 | 1       | 22      | 1        |
     | Cbln1, Slc17a6  | 2.58E-58 | 6.29E-14  | 5.01E-12  | 2.1E-131        | 5.8E-304        | 5.8E-304 | 2       | 1       | 1        |
     | Gabra1, Slc17a6 | 1.01E-53 | 6.75E-45  | 5.89E-06  | 4.39E-13        | 5.8E-304        | 5.8E-304 | 27      | 1       | 1        |
     | Cbln1, Gpr165   | 6.64E-39 | 1.5E-08   | 6.27E-43  | 2.1E-131        | 0.999642        | 2.1E-131 | 2       | 95      | 2        |
     | Cbln1, Syt4     | 4.29E-36 | 1.55E-10  | 1.35E-32  | 2.1E-131        | 1.48E-17        | 2.1E-131 | 2       | 22      | 2        |
 
 (**Note** - For AnnData objects. These results are stored in `adata.uns['differential_colocalization']`. `adata.uns['differential_colocalization']` is a dictionary with keys based on the analysis done. For `1va` and `ava`, the key is `{cell_type}` and for `1v1`, the key is `{cell_type)_vs_{cell_type_2}`).
+
+### UPDATE: Frequent Subgraph Mining.
+
+Finds networks of genes colocalized in many cells using [gSpan](https://github.com/betterenvi/gSpan). The networks found are potential candidates for groups of cells and genes exhibiting interesting subcellular patterns, in this case colocalization.
+Such colocalization networks could potentially be underlying factors for specific biological processes.
+
+```
+obj.run_fsm(n_vertices = 4, alpha = 0.001)
+```
+
+Arguments: 
+  - `n_vertices`: *(int)* Minimum number of vertices in the network.
+  - `alpha`: *(Float)* *(Float)* pvalue signifcance threshold (>alpha_cellwise are converted to 1). Default = 0.001.
+  - `clique`: *(Boolean)* Forces networks found to be fully connected. Number of edges is number of vertices choose 2. Default = False.
+  - `n_edges`: *(int) *(Optional)* Minimum number of edges in the network. Works only when clique == False.
+  - `fsm_name`: *(String)* *(Optional)* Name of adata.uns key to save output in. Be sure to specify if `run_fsm` is ran multiple times because it will overwrite. Default = "nV{x}_cliques" where x is the number of vertices.
+
+THe function will create a dataframe in `adata.uns` with all the gene pair networks found. Ny default the key is `nV{x}_cliques` where x is the number of vertices but using the attribute `fsm_name` it can be changed. 
+
+## Citation 
+
+```
+@article{kumar2023intracellular,
+  title={Intracellular Spatial Transcriptomic Analysis Toolkit (InSTAnT)},
+  author={Kumar, Anurendra and Schrader, Alex W and Boroojeny, Ali Ebrahimpour and Asadian, Marisa and Lee, Juyeon and Song, You Jin and Zhao, Sihai Dave and Han, Hee-Sun and Sinha, Saurabh},
+  journal={Research Square},
+  year={2023},
+  publisher={American Journal Experts}
+}
+```
```

