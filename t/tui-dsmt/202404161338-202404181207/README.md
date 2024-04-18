# Comparing `tmp/tui_dsmt-202404161338.tar.gz` & `tmp/tui_dsmt-202404181207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404161338.tar", last modified: Tue Apr 16 13:38:34 2024, max compression
+gzip compressed data, was "tui_dsmt-202404181207.tar", last modified: Thu Apr 18 12:07:34 2024, max compression
```

## Comparing `tui_dsmt-202404161338.tar` & `tui_dsmt-202404181207.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.380922 tui_dsmt-202404161338/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.384922 tui_dsmt-202404161338/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.384922 tui_dsmt-202404161338/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.388923 tui_dsmt-202404161338/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112120 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5539 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-16 12:44:34.000000 tui_dsmt-202404161338/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404161338/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404161338/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:38:34.392922 tui_dsmt-202404161338/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-16 13:38:34.000000 tui_dsmt-202404161338/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-16 13:38:34.000000 tui_dsmt-202404161338/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 13:38:34.000000 tui_dsmt-202404161338/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-16 13:38:34.000000 tui_dsmt-202404161338/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-16 13:38:34.000000 tui_dsmt-202404161338/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.230165 tui_dsmt-202404181207/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.234165 tui_dsmt-202404181207/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.234165 tui_dsmt-202404181207/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.238165 tui_dsmt-202404181207/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-18 12:07:26.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-18 12:07:26.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-18 12:07:26.000000 tui_dsmt-202404181207/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:34.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2024-04-18 12:07:26.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-18 12:07:26.000000 tui_dsmt-202404181207/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404181207/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404181207/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:07:34.246166 tui_dsmt-202404181207/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-18 12:07:34.000000 tui_dsmt-202404181207/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-18 12:07:34.000000 tui_dsmt-202404181207/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 12:07:34.000000 tui_dsmt-202404181207/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-18 12:07:34.000000 tui_dsmt-202404181207/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 12:07:34.000000 tui_dsmt-202404181207/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404161338/PKG-INFO` & `tui_dsmt-202404181207/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404161338
+Version: 202404181207
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404161338/setup.py` & `tui_dsmt-202404181207/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/__init__.py` & `tui_dsmt-202404181207/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404181207/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404181207/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404181207/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202404181207/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404181207/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict
 
-from .FPTree import FPTree
 from .ConditionalFPTree import ConditionalFPTree
+from .FPTree import FPTree
 from ..jpanim import JupyterAnimation
 
 
+# Das rumgepatche am Namen mit [::-1] fällt mir noch auf die Füße...
 class ConditionalPatternBase(JupyterAnimation):
     def __init__(self, fp_tree: FPTree, prefix: str = ''):
         self._fp_tree: FPTree = fp_tree
         self._prefix: str = prefix
 
         # generate some required values
         names = {key: value for key, value in self._tree_to_names(fp_tree.fp_tree)}
@@ -29,30 +30,36 @@
                     <td>{fi}</td>
                     <td>{{{{frame.{fi}_text}}}}</td>
                     <td>{{{{frame.{fi}_cpb}}}}</td>
                 </tr>     
             '''
 
         # frame initialization
+        def edge_color(u, v):
+            if len(u) == 0 or len(v) == 0 or u[-1] != v[-1]:
+                return 'rgba(99, 110, 250, 0.5)'
+            else:
+                return 'transparent'
+
         frames = {
             'Ende der Transaktionen': {
                 **{
-                    f'name_{node}': f'{node[-1]} ({names[node]})' if len(node) > 0 else fp_tree.head_name
+                    f'name_{node}': f'{node[-1]} ({names[node]})' if len(node) > 0 else fp_tree.head_name[::-1]
                     for node in fp_tree.graph.nodes
                 },
                 **{
                     f'node_{node}': {
                         'backgroundColor': '#636EFA',
                         'color': 'whitesmoke'
                     }
                     for node in fp_tree.graph.nodes
                 },
                 **{
                     f'edge_{u}_{v}': {
-                        'backgroundColor': 'rgba(99, 110, 250, 0.5)'
+                        'backgroundColor': edge_color(u, v)
                     }
                     for u, v in fp_tree.graph.edges
                 },
                 **{
                     f'{fi}_text': ', '.join(f'{fi} ({v})' for v in links[fi])
                     for fi in fp_tree.frequent_items
                 },
@@ -138,15 +145,16 @@
             [
                 fp_tree.graph_css,
                 fp_tree.layout_css
             ]
         )
 
     def conditional_fp_tree(self, itemset):
-        return ConditionalFPTree(self._fp_tree, self.cpb[itemset], itemset)
+        new_prefix = self._prefix + itemset
+        return ConditionalFPTree(self._fp_tree, self.cpb[new_prefix], new_prefix)
 
     @staticmethod
     def _tree_to_names(fp_tree: Dict):
         if len(fp_tree) == 0:
             return
 
         for key, (value, children) in fp_tree.items():
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/FPTree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-from typing import List, Tuple, Dict, Union
+from typing import List, Tuple, Dict, Union, Iterator, Any
 
 import networkx as nx
 
 from .Itemset import Itemset
 from ..graph.html import graph_to_html
 from ..jpanim import JupyterAnimation
+from .. import color_secondary
 
 TRANSACTION_LIST = List[Tuple[int, Union[Itemset, Tuple]]]
 
 
+# Das rumgepatche am Namen mit [::-1] fällt mir noch auf die Füße...
 class FPTree(JupyterAnimation):
-    def __init__(self, transactions: TRANSACTION_LIST, min_supp: int, head_name: str = '{}', sort: bool = True):
+    def __init__(self, transactions: TRANSACTION_LIST, min_supp: int, head_name: str = '{}', sort: bool = True,
+                 custom_item_order: Iterator = None):
         self.transactions: TRANSACTION_LIST = transactions
         self.min_supp: int = min_supp
         self.head_name: str = head_name
 
+        if custom_item_order is None:
+            self.custom_item_order: Dict[Any, int] = {}
+        else:
+            self.custom_item_order = {k: -i for i, k in enumerate(custom_item_order)}
+
         self.fp_tree, self.frequent_items = self._fp_tree(transactions, min_supp, sort)
 
         # build a graph layout
         if len(self.fp_tree) == 0:
-            raise AssertionError('FPTree is empty')
-
-        self.graph = self._fp_tree_to_graph(self.fp_tree)
+            # raise AssertionError('FPTree is empty')
+            self.graph = nx.Graph()
+            self.graph.add_node('')
+        else:
+            self.graph = self._fp_tree_to_graph(self.fp_tree)
 
         pos = {''.join(key): (x, y) for key, x, y in self._fp_tree_to_pos(self.fp_tree)}
         pos[''] = (0.5, 0)
 
         # convert to html
         self.graph_html, self.graph_css = graph_to_html(self.graph, pos,
                                                         display_height='15rem',
-                                                        node_width='5rem', node_height='2rem')
+                                                        node_width='4rem', node_height='2rem')
 
         # header table
         header_table_html = ''
         for fi in self.frequent_items:
             header_table_html += f'''
                 <tr>
                     <td>{fi}</td>
@@ -44,15 +54,15 @@
 
         # frame generation
         frames = {
             'Initialisierung': {
                 'current_transaction': '',
                 'cleaned_transaction': '',
                 **{
-                    f'name_{node}': node[-1] if len(node) > 0 else head_name
+                    f'name_{node}': node[-1] if len(node) > 0 else (head_name if head_name == '{}' else head_name[::-1])
                     for node in self.graph.nodes
                 },
                 **{
                     f'node_{node}': {
                         'backgroundColor': '#636EFA',
                         'color': 'whitesmoke',
                         'display': 'none' if node != '' else 'flex'
@@ -142,62 +152,74 @@
             prefix = ''
         else:
             prefix = self.head_name
 
         from .ConditionalPatternBase import ConditionalPatternBase
         return ConditionalPatternBase(self, prefix)
 
-    @staticmethod
-    def _fp_tree(transactions: TRANSACTION_LIST, min_supp: int, sort: bool):
+    def _fp_tree(self, transactions: TRANSACTION_LIST, min_supp: int, sort: bool):
         # count 1-itemsets
         counts = {}
         for _, itemset in transactions:
             for element in itemset:
                 counts[element] = counts.get(element, 0) + 1
 
         # initialize tree and header table
         fp_tree = {}
 
         # iterate over itemsets
         for _, itemset in transactions:
             # filter and sort important items
             relevant_items = tuple(x for x in itemset if counts[x] >= min_supp)
             if sort:
-                relevant_items = tuple(sorted(relevant_items, key=lambda x: (counts[x], x), reverse=True))
+                relevant_items = tuple(sorted(relevant_items,
+                                              key=lambda x: (counts[x], self.custom_item_order.get(x, 0), x),
+                                              reverse=True))
 
             # integrate into fp_tree
             node = fp_tree
             for d, element in enumerate(relevant_items, start=1):
                 unique_name = relevant_items[:d]
                 if unique_name not in node:
                     node[unique_name] = [0, {}]
 
                 node[unique_name][0] += 1
                 node = node[unique_name][1]
 
         # return
         frequent_itemsets = sorted((key for key, count in counts.items() if count >= min_supp),
-                                   key=lambda x: (counts[x], x), reverse=True)
+                                   key=lambda x: (counts[x], self.custom_item_order.get(x, 0), x),
+                                   reverse=True)
         return fp_tree, frequent_itemsets
 
     @staticmethod
-    def _fp_tree_to_graph(fp_tree: Dict, graph: nx.Graph = None):
+    def _fp_tree_to_graph(fp_tree: Dict, graph: nx.Graph = None, recent_nodes: Dict = None):
         if len(fp_tree) == 0:
             return
 
         if graph is None:
             graph = nx.Graph()
+            recent_nodes = {}
+
             for key in fp_tree:
                 graph.add_edge('', ''.join(key))
 
         for key, (_, children) in fp_tree.items():
+            parent_key = ''.join(key)
+            parent_name = key[-1]
+
+            if parent_name in recent_nodes:
+                graph.add_edge(recent_nodes[parent_name], parent_key)
+            recent_nodes[parent_name] = parent_key
+
             for child in children:
-                graph.add_edge(''.join(key), ''.join(child))
+                child_key = ''.join(child)
+                graph.add_edge(parent_key, child_key)
 
-            FPTree._fp_tree_to_graph(children, graph)
+            FPTree._fp_tree_to_graph(children, graph, recent_nodes)
 
         return graph
 
     @staticmethod
     def _fp_tree_to_pos(fp_tree: Dict, y: int = 1, left: float = 0., right: float = 1.):
         if len(fp_tree) == 0:
             return
@@ -219,42 +241,58 @@
         for _, itemset in self.transactions:
             for element in itemset:
                 counts[element] = counts.get(element, 0) + 1
 
         fp_tree = {}
         header_table = {}
 
+        recent = {}
         unlocked_nodes = {''}
 
         for tid, itemset in self.transactions:
             frame = {
                 'current_transaction': 'Transaktion ' + str(tid) + ': {' + ', '.join(itemset) + '}',
                 **{
                     f'node_{node}': {
                         'backgroundColor': '#636EFA',
                         'color': 'whitesmoke'
                     }
                     for node in unlocked_nodes
                 }
             }
 
-            relevant_items = itemset.filter(lambda x: counts[x] >= self.min_supp).sort(lambda x: (counts[x], x), True)
-            frame['cleaned_transaction'] = 'Bereinigt und sortiert: {' + ', '.join(relevant_items) + '}'
+            relevant_items = itemset.filter(
+                lambda x: counts[x] >= self.min_supp
+            ).sort(
+                lambda x: (counts[x], self.custom_item_order.get(x, 0), x), True
+            )
+            frame['cleaned_transaction'] = 'Bereinigt und sortiert: [' + ', '.join(relevant_items) + ']'
 
             node = fp_tree
             previous_unique_name_str = ''
 
             frame['node_'] = {
                 'backgroundColor': '#EF553B',
                 'color': 'whitesmoke'
             }
 
             for d, element in enumerate(relevant_items, start=1):
                 unique_name = relevant_items[:d]
                 unique_name_str = ''.join(unique_name)
+                last_char = unique_name[-1]
+
+                if last_char in recent:
+                    recent_unique_name_str = recent[last_char]
+                    for edge_name in (f'edge_{recent_unique_name_str}_{unique_name_str}',
+                                      f'edge_{unique_name_str}_{recent_unique_name_str}'):
+                        frame[edge_name] = {
+                            'backgroundColor': f'rgba({color_secondary}, 0.67)',
+                            'dash': '10,10'
+                        }
+                recent[last_char] = unique_name_str
 
                 if unique_name not in node:
                     node[unique_name] = [0, {}]
 
                     if element not in header_table:
                         header_table[element] = []
                     header_table[element].append(node[unique_name])
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404181207/src/tui_dsmt/fpm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,22 @@
     (200, Itemset('a', 'b', 'c', 'f', 'l', 'm', 'o')),
     (300, Itemset('b', 'f', 'm', 'h', 'j', 'o')),
     (400, Itemset('b', 'c', 'k', 's', 'p')),
     (500, Itemset('a', 'f', 'c', 'e', 'l', 'p', 'm', 'n')),
     (600, Itemset('f', 'c', 'p', 'n')),
 )
 
+characters2 = TransactionDatabase(
+    (100, Itemset('f', 'a', 'c', 'd', 'g', 'i', 'm', 'p')),
+    (200, Itemset('a', 'b', 'c', 'f', 'l', 'm', 'o')),
+    (300, Itemset('b', 'f', 'h', 'j', 'o')),
+    (400, Itemset('b', 'c', 'k', 's', 'p')),
+    (500, Itemset('a', 'f', 'c', 'e', 'l', 'p', 'm', 'n')),
+)
+
 dna = SequentialDatabase(
     (1, SequentialItemset(*'AGAAGT')),
     (2, SequentialItemset(*'TGACAG')),
     (3, SequentialItemset(*'GAAGT'))
 )
 
 website_tracking = SequentialDatabase(
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/html.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,23 @@
         if max_y is None or py > max_y:
             max_y = py
 
     nodes_html = []
     nodes_positions = {}
 
     for key, (px, py) in layout.items():
-        left = (px - min_x) / (max_x - min_x) * 100 if min_x < max_x else 50
-        top = (py - min_y) / (max_y - min_y) * 100
+        if max_x == min_x:
+            left = 50
+        else:
+            left = (px - min_x) / (max_x - min_x) * 100 if min_x < max_x else 50
+
+        if max_y == min_y:
+            top = 0
+        else:
+            top = (py - min_y) / (max_y - min_y) * 100
 
         nodes_html.append(f'''
             <div class="node"
                  style="left: calc({left}% - {node_width} / 2); top: calc({top}% - {node_height} / 2)"
                  :style="frame.node_{key}">
                 {{{{frame.name_{key}}}}}
             </div>
@@ -88,15 +95,16 @@
                               :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
                               {arrow}="url(#head-{marker_id})" />
                     ''')
                 else:
                     lines_svg.append(f'''
                         <line id="{id}" 
                               x1="{x1}%" y1="{y1}%" x2="{x2}%" y2="{y2}%"
-                              :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor" />
+                              :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
+                              :stroke-dasharray="{attr}.dash" />
                     ''')
 
                 if weights is not None:
                     weight = graph.get_edge_data(source_node, target_node)[weights]
                 else:
                     weight = f'{{{{{attr}.text}}}}'
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404181207/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404161338/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404181207/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class JupyterAnimation(HTML):
     def __init__(self,
                  html: str, frames: Dict[str, Dict],
-                 style: Optional[List[str] | str] = None, js: List[str] | str = None),
+                 style: Optional[List[str] | str] = None, js: List[str] | str = None,
                  fast_forward: bool = False):
         self._html: str = html
         self._frames: Dict[str, Dict] = frames
         self._fast_forward: bool = fast_forward
 
         if isinstance(style, list):
             self._style: str = '\n'.join(style)
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404181207/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404161338
+Version: 202404181207
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404161338/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404181207/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

