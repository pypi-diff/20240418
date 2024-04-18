# Comparing `tmp/heat-1.3.1.tar.gz` & `tmp/heat-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-1.3.1.tar", last modified: Thu Nov 23 09:32:54 2023, max compression
+gzip compressed data, was "heat-1.4.0.tar", last modified: Thu Apr 18 08:33:38 2024, max compression
```

## Comparing `heat-1.3.1.tar` & `heat-1.4.0.tar`

### file list

```diff
@@ -1,112 +1,119 @@
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.631971 heat-1.3.1/
--rw-r--r--   0 c.comito   (501) staff       (20)     1192 2022-07-21 04:14:34.000000 heat-1.3.1/LICENSE
--rw-r--r--   0 c.comito   (501) staff       (20)    10472 2023-11-23 09:32:54.631775 heat-1.3.1/PKG-INFO
--rw-r--r--   0 c.comito   (501) staff       (20)     9085 2023-11-22 10:50:22.000000 heat-1.3.1/README.md
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.599239 heat-1.3.1/heat/
--rw-r--r--   0 c.comito   (501) staff       (20)      373 2023-11-22 10:50:22.000000 heat-1.3.1/heat/__init__.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.601578 heat-1.3.1/heat/classification/
--rw-r--r--   0 c.comito   (501) staff       (20)       79 2022-07-21 04:14:34.000000 heat-1.3.1/heat/classification/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4716 2023-11-20 04:19:08.000000 heat-1.3.1/heat/classification/kneighborsclassifier.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.603903 heat-1.3.1/heat/cluster/
--rw-r--r--   0 c.comito   (501) staff       (20)      185 2022-07-21 04:14:34.000000 heat-1.3.1/heat/cluster/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     9597 2023-11-22 10:50:22.000000 heat-1.3.1/heat/cluster/_kcluster.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5336 2023-11-20 04:19:08.000000 heat-1.3.1/heat/cluster/kmeans.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5391 2023-11-20 04:19:08.000000 heat-1.3.1/heat/cluster/kmedians.py
--rw-r--r--   0 c.comito   (501) staff       (20)     6087 2023-11-20 04:19:08.000000 heat-1.3.1/heat/cluster/kmedoids.py
--rw-r--r--   0 c.comito   (501) staff       (20)     8174 2023-11-20 04:19:08.000000 heat-1.3.1/heat/cluster/spectral.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.615743 heat-1.3.1/heat/core/
--rw-r--r--   0 c.comito   (501) staff       (20)      761 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    19854 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/_operations.py
--rw-r--r--   0 c.comito   (501) staff       (20)    35693 2023-11-22 15:43:59.000000 heat-1.3.1/heat/core/arithmetics.py
--rw-r--r--   0 c.comito   (501) staff       (20)     7395 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/base.py
--rw-r--r--   0 c.comito   (501) staff       (20)    70818 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/communication.py
--rw-r--r--   0 c.comito   (501) staff       (20)     3166 2022-07-21 04:14:34.000000 heat-1.3.1/heat/core/complex_math.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1072 2022-07-21 04:14:34.000000 heat-1.3.1/heat/core/constants.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4951 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/devices.py
--rw-r--r--   0 c.comito   (501) staff       (20)    73359 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/dndarray.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10997 2022-07-21 04:14:34.000000 heat-1.3.1/heat/core/exponential.py
--rw-r--r--   0 c.comito   (501) staff       (20)    56979 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/factories.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5399 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/indexing.py
--rw-r--r--   0 c.comito   (501) staff       (20)    43828 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/io.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.617740 heat-1.3.1/heat/core/linalg/
--rw-r--r--   0 c.comito   (501) staff       (20)      160 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/linalg/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    89467 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/linalg/basics.py
--rw-r--r--   0 c.comito   (501) staff       (20)    44959 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/linalg/qr.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10320 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/linalg/solver.py
--rw-r--r--   0 c.comito   (501) staff       (20)      566 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/linalg/svd.py
--rw-r--r--   0 c.comito   (501) staff       (20)    25597 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/linalg/svdtools.py
--rw-r--r--   0 c.comito   (501) staff       (20)    17929 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/logical.py
--rw-r--r--   0 c.comito   (501) staff       (20)   152131 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/manipulations.py
--rw-r--r--   0 c.comito   (501) staff       (20)     2942 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/memory.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10383 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/printing.py
--rw-r--r--   0 c.comito   (501) staff       (20)    37382 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/random.py
--rw-r--r--   0 c.comito   (501) staff       (20)    13166 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/relational.py
--rw-r--r--   0 c.comito   (501) staff       (20)    15182 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/rounding.py
--rw-r--r--   0 c.comito   (501) staff       (20)    12399 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/sanitation.py
--rw-r--r--   0 c.comito   (501) staff       (20)     7345 2023-11-22 03:34:22.000000 heat-1.3.1/heat/core/signal.py
--rw-r--r--   0 c.comito   (501) staff       (20)    75639 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/statistics.py
--rw-r--r--   0 c.comito   (501) staff       (20)     6688 2023-11-22 10:50:22.000000 heat-1.3.1/heat/core/stride_tricks.py
--rw-r--r--   0 c.comito   (501) staff       (20)    52201 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/tiling.py
--rw-r--r--   0 c.comito   (501) staff       (20)    16274 2022-07-21 04:14:34.000000 heat-1.3.1/heat/core/trigonometrics.py
--rw-r--r--   0 c.comito   (501) staff       (20)    28107 2023-11-20 04:19:08.000000 heat-1.3.1/heat/core/types.py
--rw-r--r--   0 c.comito   (501) staff       (20)      534 2023-11-23 09:22:38.000000 heat-1.3.1/heat/core/version.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.621211 heat-1.3.1/heat/datasets/
--rw-r--r--   0 c.comito   (501) staff       (20)       50 2023-09-07 14:38:44.000000 heat-1.3.1/heat/datasets/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    25312 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/diabetes.h5
--rw-r--r--   0 c.comito   (501) staff       (20)     2400 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     6944 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris.h5
--rw-r--r--   0 c.comito   (501) staff       (20)    11040 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris.nc
--rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_X_test.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_X_train.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      300 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_labels.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     5669 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_y_pred_proba.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_y_test.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.3.1/heat/datasets/iris_y_train.csv
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.621691 heat-1.3.1/heat/graph/
--rw-r--r--   0 c.comito   (501) staff       (20)       86 2022-07-21 04:14:34.000000 heat-1.3.1/heat/graph/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4962 2022-07-21 04:14:34.000000 heat-1.3.1/heat/graph/laplacian.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.622192 heat-1.3.1/heat/naive_bayes/
--rw-r--r--   0 c.comito   (501) staff       (20)       88 2022-07-21 04:14:34.000000 heat-1.3.1/heat/naive_bayes/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    22124 2023-11-20 04:19:08.000000 heat-1.3.1/heat/naive_bayes/gaussianNB.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.623183 heat-1.3.1/heat/nn/
--rw-r--r--   0 c.comito   (501) staff       (20)     2265 2023-09-07 14:38:44.000000 heat-1.3.1/heat/nn/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    16357 2023-11-20 04:19:08.000000 heat-1.3.1/heat/nn/data_parallel.py
--rw-r--r--   0 c.comito   (501) staff       (20)      630 2023-09-07 14:38:44.000000 heat-1.3.1/heat/nn/functional.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.625052 heat-1.3.1/heat/optim/
--rw-r--r--   0 c.comito   (501) staff       (20)     2507 2023-09-07 14:38:44.000000 heat-1.3.1/heat/optim/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    38305 2023-11-22 10:50:22.000000 heat-1.3.1/heat/optim/dp_optimizer.py
--rw-r--r--   0 c.comito   (501) staff       (20)      380 2023-09-07 14:38:44.000000 heat-1.3.1/heat/optim/lr_scheduler.py
--rw-r--r--   0 c.comito   (501) staff       (20)     7171 2022-07-21 04:14:34.000000 heat-1.3.1/heat/optim/utils.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.625524 heat-1.3.1/heat/regression/
--rw-r--r--   0 c.comito   (501) staff       (20)       80 2022-07-21 04:14:34.000000 heat-1.3.1/heat/regression/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5637 2023-11-22 15:43:59.000000 heat-1.3.1/heat/regression/lasso.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.627205 heat-1.3.1/heat/sparse/
--rw-r--r--   0 c.comito   (501) staff       (20)      194 2023-09-07 14:38:44.000000 heat-1.3.1/heat/sparse/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5681 2023-09-07 14:38:44.000000 heat-1.3.1/heat/sparse/_operations.py
--rw-r--r--   0 c.comito   (501) staff       (20)     3276 2023-09-07 14:38:44.000000 heat-1.3.1/heat/sparse/arithmetics.py
--rw-r--r--   0 c.comito   (501) staff       (20)     9922 2023-09-07 14:38:44.000000 heat-1.3.1/heat/sparse/dcsr_matrix.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10088 2023-11-20 04:19:08.000000 heat-1.3.1/heat/sparse/factories.py
--rw-r--r--   0 c.comito   (501) staff       (20)     3000 2023-11-22 10:50:22.000000 heat-1.3.1/heat/sparse/manipulations.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.627684 heat-1.3.1/heat/spatial/
--rw-r--r--   0 c.comito   (501) staff       (20)       93 2022-07-21 04:14:34.000000 heat-1.3.1/heat/spatial/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    18018 2023-11-20 04:19:08.000000 heat-1.3.1/heat/spatial/distance.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.628462 heat-1.3.1/heat/utils/
--rw-r--r--   0 c.comito   (501) staff       (20)      112 2022-07-21 04:14:34.000000 heat-1.3.1/heat/utils/__init__.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.630428 heat-1.3.1/heat/utils/data/
--rw-r--r--   0 c.comito   (501) staff       (20)      195 2023-09-07 14:38:44.000000 heat-1.3.1/heat/utils/data/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    13358 2023-11-20 04:19:08.000000 heat-1.3.1/heat/utils/data/_utils.py
--rw-r--r--   0 c.comito   (501) staff       (20)    17539 2022-07-21 04:14:34.000000 heat-1.3.1/heat/utils/data/datatools.py
--rw-r--r--   0 c.comito   (501) staff       (20)     6354 2023-11-22 10:50:22.000000 heat-1.3.1/heat/utils/data/matrixgallery.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4849 2023-11-20 04:19:08.000000 heat-1.3.1/heat/utils/data/mnist.py
--rw-r--r--   0 c.comito   (501) staff       (20)    15496 2023-11-20 04:19:08.000000 heat-1.3.1/heat/utils/data/partial_dataset.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1994 2023-09-07 14:38:44.000000 heat-1.3.1/heat/utils/data/spherical.py
--rw-r--r--   0 c.comito   (501) staff       (20)      606 2023-09-07 14:38:44.000000 heat-1.3.1/heat/utils/vision_transforms.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-11-23 09:32:54.630783 heat-1.3.1/heat.egg-info/
--rw-r--r--   0 c.comito   (501) staff       (20)    10472 2023-11-23 09:32:54.000000 heat-1.3.1/heat.egg-info/PKG-INFO
--rw-r--r--   0 c.comito   (501) staff       (20)     2325 2023-11-23 09:32:54.000000 heat-1.3.1/heat.egg-info/SOURCES.txt
--rw-r--r--   0 c.comito   (501) staff       (20)        1 2023-11-23 09:32:54.000000 heat-1.3.1/heat.egg-info/dependency_links.txt
--rw-r--r--   0 c.comito   (501) staff       (20)      263 2023-11-23 09:32:54.000000 heat-1.3.1/heat.egg-info/requires.txt
--rw-r--r--   0 c.comito   (501) staff       (20)        5 2023-11-23 09:32:54.000000 heat-1.3.1/heat.egg-info/top_level.txt
--rw-r--r--   0 c.comito   (501) staff       (20)       31 2022-07-21 04:14:34.000000 heat-1.3.1/pyproject.toml
--rw-r--r--   0 c.comito   (501) staff       (20)      327 2023-11-23 09:32:54.632416 heat-1.3.1/setup.cfg
--rw-r--r--   0 c.comito   (501) staff       (20)     1704 2023-11-23 08:44:08.000000 heat-1.3.1/setup.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.881997 heat-1.4.0/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1192 2023-07-24 13:32:34.000000 heat-1.4.0/LICENSE
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13291 2024-04-18 08:33:38.880998 heat-1.4.0/PKG-INFO
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11851 2024-04-15 09:38:15.000000 heat-1.4.0/README.md
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.499989 heat-1.4.0/heat/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      419 2024-04-03 10:40:08.000000 heat-1.4.0/heat/__init__.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.526019 heat-1.4.0/heat/classification/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       79 2023-07-24 13:32:35.000000 heat-1.4.0/heat/classification/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4717 2024-04-03 10:40:08.000000 heat-1.4.0/heat/classification/kneighborsclassifier.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.551998 heat-1.4.0/heat/cluster/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      224 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11575 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/_kcluster.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18439 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/batchparallelclustering.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5481 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/kmeans.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5543 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/kmedians.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     6088 2024-04-03 10:40:08.000000 heat-1.4.0/heat/cluster/kmedoids.py
+-rwx------   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8174 2023-10-30 07:50:09.000000 heat-1.4.0/heat/cluster/spectral.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.669994 heat-1.4.0/heat/core/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      790 2024-02-01 10:00:28.000000 heat-1.4.0/heat/core/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    20752 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/_operations.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)   115820 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/arithmetics.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8724 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/base.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75974 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/communication.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3166 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/complex_math.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1072 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/constants.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4951 2023-11-22 13:39:03.000000 heat-1.4.0/heat/core/devices.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75015 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/dndarray.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10997 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/exponential.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    58349 2024-04-17 13:50:50.000000 heat-1.4.0/heat/core/factories.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5399 2023-11-22 13:39:03.000000 heat-1.4.0/heat/core/indexing.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    45033 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/io.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.691996 heat-1.4.0/heat/core/linalg/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      160 2024-01-22 14:35:17.000000 heat-1.4.0/heat/core/linalg/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    89776 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/basics.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    14456 2024-04-18 07:47:42.000000 heat-1.4.0/heat/core/linalg/qr.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10346 2024-04-17 12:15:23.000000 heat-1.4.0/heat/core/linalg/solver.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      567 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/svd.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    25582 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/svdtools.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18390 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/logical.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)   153593 2024-04-03 12:29:03.000000 heat-1.4.0/heat/core/manipulations.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3211 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/memory.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11279 2024-02-01 10:00:28.000000 heat-1.4.0/heat/core/printing.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    37383 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/random.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13167 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/relational.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    15188 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/rounding.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11512 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/sanitation.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7557 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/signal.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75387 2024-04-08 09:45:59.000000 heat-1.4.0/heat/core/statistics.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8109 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/stride_tricks.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    52200 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/tiling.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    16274 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/trigonometrics.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    28107 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/types.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      533 2024-04-18 07:49:51.000000 heat-1.4.0/heat/core/version.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.748990 heat-1.4.0/heat/datasets/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       50 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    25312 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/diabetes.h5
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2400 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     6944 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.h5
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11040 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.nc
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1800 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_X_test.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1800 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_X_train.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      300 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_labels.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5669 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_pred_proba.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      150 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_test.csv
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      150 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_train.csv
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.755990 heat-1.4.0/heat/fft/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       76 2024-04-03 10:40:08.000000 heat-1.4.0/heat/fft/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    46743 2024-04-03 10:40:08.000000 heat-1.4.0/heat/fft/fft.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.762995 heat-1.4.0/heat/graph/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       86 2023-07-24 13:32:35.000000 heat-1.4.0/heat/graph/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4963 2024-04-03 10:40:08.000000 heat-1.4.0/heat/graph/laplacian.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.769993 heat-1.4.0/heat/naive_bayes/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       88 2023-07-24 13:32:35.000000 heat-1.4.0/heat/naive_bayes/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    22137 2024-04-03 10:40:08.000000 heat-1.4.0/heat/naive_bayes/gaussianNB.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.780994 heat-1.4.0/heat/nn/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2265 2023-07-24 13:32:35.000000 heat-1.4.0/heat/nn/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    16358 2024-04-03 10:40:08.000000 heat-1.4.0/heat/nn/data_parallel.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      630 2023-10-30 07:50:10.000000 heat-1.4.0/heat/nn/functional.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.794997 heat-1.4.0/heat/optim/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2507 2023-07-24 13:32:35.000000 heat-1.4.0/heat/optim/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    39179 2024-04-03 10:40:08.000000 heat-1.4.0/heat/optim/dp_optimizer.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      380 2023-10-30 07:50:10.000000 heat-1.4.0/heat/optim/lr_scheduler.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7171 2023-07-24 13:32:35.000000 heat-1.4.0/heat/optim/utils.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.801999 heat-1.4.0/heat/preprocessing/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      104 2024-02-01 10:00:28.000000 heat-1.4.0/heat/preprocessing/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    22404 2024-04-08 09:45:59.000000 heat-1.4.0/heat/preprocessing/preprocessing.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.809990 heat-1.4.0/heat/regression/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       80 2023-07-24 13:32:35.000000 heat-1.4.0/heat/regression/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5637 2024-04-03 10:40:08.000000 heat-1.4.0/heat/regression/lasso.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.829994 heat-1.4.0/heat/sparse/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      194 2023-10-30 07:50:10.000000 heat-1.4.0/heat/sparse/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5682 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/_operations.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3277 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/arithmetics.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     9923 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/dcsr_matrix.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10096 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/factories.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4033 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/manipulations.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.836997 heat-1.4.0/heat/spatial/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       93 2023-07-24 13:32:35.000000 heat-1.4.0/heat/spatial/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18019 2024-04-03 10:40:08.000000 heat-1.4.0/heat/spatial/distance.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.844008 heat-1.4.0/heat/utils/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      112 2023-07-24 13:32:35.000000 heat-1.4.0/heat/utils/__init__.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.870993 heat-1.4.0/heat/utils/data/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      195 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/__init__.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13358 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/_utils.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    17539 2023-11-22 13:39:03.000000 heat-1.4.0/heat/utils/data/datatools.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8982 2024-04-03 10:40:08.000000 heat-1.4.0/heat/utils/data/matrixgallery.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4849 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/mnist.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    15496 2023-11-22 13:39:03.000000 heat-1.4.0/heat/utils/data/partial_dataset.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7019 2024-04-15 09:38:15.000000 heat-1.4.0/heat/utils/data/spherical.py
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      606 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/vision_transforms.py
+drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.875995 heat-1.4.0/heat.egg-info/
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13291 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/PKG-INFO
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2469 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/SOURCES.txt
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        1 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/dependency_links.txt
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      265 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/requires.txt
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        5 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/top_level.txt
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       31 2023-07-24 13:32:35.000000 heat-1.4.0/pyproject.toml
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      327 2024-04-18 08:33:38.885996 heat-1.4.0/setup.cfg
+-rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1756 2024-04-17 13:50:50.000000 heat-1.4.0/setup.py
```

### Comparing `heat-1.3.1/LICENSE` & `heat-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/PKG-INFO` & `heat-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,193 @@
-Metadata-Version: 2.1
-Name: heat
-Version: 1.3.1
-Summary: A framework for high-performance data analytics and machine learning.
-Home-page: https://github.com/helmholtz-analytics/heat
-Author: Helmholtz Association
-Author-email: martin.siggel@dlr.de
-Keywords: data,analytics,tensors,distributed,gpu
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: mpi4py>=3.0.0
-Requires-Dist: numpy>=1.20.0
-Requires-Dist: torch<2.0.2,>=1.8.0
-Requires-Dist: scipy>=0.14.0
-Requires-Dist: pillow>=6.0.0
-Requires-Dist: torchvision>=0.8.0
-Provides-Extra: docutils
-Requires-Dist: docutils>=0.16; extra == "docutils"
-Provides-Extra: hdf5
-Requires-Dist: h5py>=2.8.0; extra == "hdf5"
-Provides-Extra: netcdf
-Requires-Dist: netCDF4>=1.5.6; extra == "netcdf"
-Provides-Extra: dev
-Requires-Dist: pre-commit>=1.18.3; extra == "dev"
-Provides-Extra: examples
-Requires-Dist: scikit-learn>=0.24.0; extra == "examples"
-Requires-Dist: matplotlib>=3.1.0; extra == "examples"
-Provides-Extra: cb
-Requires-Dist: perun>=0.2.0; extra == "cb"
-
 <div align="center">
   <img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/logo.png">
 </div>
 
 ---
 
 Heat is a distributed tensor framework for high performance data analytics.
 
 # Project Status
 
-[![pipeline status](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
+[![CPU/CUDA/ROCm tests](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
 [![Documentation Status](https://readthedocs.org/projects/heat/badge/?version=latest)](https://heat.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![coverage](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
 [![license: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/heat)](https://pypi.org/project/heat/)
 [![Downloads](https://pepy.tech/badge/heat)](https://pepy.tech/project/heat)
-[![Github-Pages - Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/heat/badges/version.svg)](https://anaconda.org/conda-forge/heat)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/helmholtz-analytics/heat/badge)](https://securityscorecards.dev/viewer/?uri=github.com/helmholtz-analytics/heat)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7688/badge)](https://bestpractices.coreinfrastructure.org/projects/7688)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2531472.svg)](https://doi.org/10.5281/zenodo.2531472)
+[![Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-# Goals
+# Table of Contents
+  - [What is Heat for?](#what-is-heat-for)
+  - [Features](#features)
+  - [Getting Started](#getting-started)
+  - [Installation](#installation)
+    - [Requirements](#requirements)
+    - [pip](#pip)
+    - [conda](#conda)
+  - [Support Channels](#support-channels)
+  - [Contribution guidelines](#contribution-guidelines)
+    - [Resources](#resources)
+  - [License](#license)
+  - [Citing Heat](#citing-heat)
+  - [FAQ](#faq)
+  - [Acknowledgements](#acknowledgements)
 
-Heat is a flexible and seamless open-source software for high performance data
-analytics and machine learning. It provides highly optimized algorithms and data
-structures for tensor computations using CPUs, GPUs and distributed cluster
-systems on top of MPI. The goal of Heat is to fill the gap between data
-analytics and machine learning libraries with a strong focus on single-node
-performance, and traditional high-performance computing (HPC). Heat's generic
-Python-first programming interface integrates seamlessly with the existing data
-science ecosystem and makes it as effortless as using numpy to write scalable
-scientific and data science applications.
 
-Heat allows you to tackle your actual Big Data challenges that go beyond the
-computational and memory needs of your laptop and desktop.
+# What is Heat for?
 
-# Features
+Heat builds on [PyTorch](https://pytorch.org/) and [mpi4py](https://mpi4py.readthedocs.io) to provide high-performance computing infrastructure for memory-intensive applications within the NumPy/SciPy ecosystem.
 
-* High-performance n-dimensional tensors
-* CPU, GPU and distributed computation using MPI
-* Powerful data analytics and machine learning methods
-* Abstracted communication via split tensors
-* Python API
 
-# Support Channels
+With Heat you can:
+- port existing NumPy/SciPy code from single-CPU to multi-node clusters with minimal coding effort;
+- exploit the entire, cumulative RAM of your many nodes for memory-intensive operations and algorithms;
+- run your NumPy/SciPy code on GPUs (CUDA, ROCm, coming up: Apple MPS).
 
-We use [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions) as a forum for questions about Heat.
-If you found a bug or miss a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
+For a example that highlights the benefits of multi-node parallelism, hardware acceleration, and how easy this can be done with the help of Heat, see, e.g., our [blog post on trucated SVD of a 200GB data set](https://helmholtz-analytics.github.io/heat/2023/06/16/new-feature-hsvd.html).
 
-# Requirements
+Check out our [coverage tables](coverage_tables.md) to see which NumPy, SciPy, scikit-learn functions are already supported.
 
-Heat requires Python 3.7 or newer.
-Heat is based on [PyTorch](https://pytorch.org/). Specifically, we are exploiting
-PyTorch's support for GPUs *and* MPI parallelism. For MPI support we utilize
-[mpi4py](https://mpi4py.readthedocs.io). Both packages can be installed via pip
-or automatically using the setup.py.
+ If you need a functionality that is not yet supported:
+  - [search existing issues](https://github.com/helmholtz-analytics/heat/issues) and make sure to leave a comment if someone else already requested it;
+  - [open a new issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
 
-# Installation
 
-Tagged releases are made available on the
-[Python Package Index (PyPI)](https://pypi.org/project/heat/). You can typically
-install the latest version with
+Check out our [features](#features) and the [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html) for a complete list of functionalities.
 
-```
-$ pip install heat[hdf5,netcdf]
-```
+# Features
 
-where the part in brackets is a list of optional dependencies. You can omit
-it, if you do not need HDF5 or NetCDF support.
+* High-performance n-dimensional arrays
+* CPU, GPU, and distributed computation using MPI
+* Powerful data analytics and machine learning methods
+* Seamless integration with the NumPy/SciPy ecosystem
+* Python array API (work in progress)
 
-**It is recommended to use the most recent supported version of PyTorch!**
 
-**It is also very important to ensure that the PyTorch version is compatible with the local CUDA installation.**
-More information can be found [here](https://pytorch.org/get-started/locally/).
+# Getting Started
 
-# Hacking
+Go to [Quick Start](quick_start.md) for a quick overview. For more details, see [Installation](#installation).
 
-If you want to work with the development version, you can check out the sources using
+**You can test your setup** by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
 
-```
-$ git clone <https://github.com/helmholtz-analytics/heat.git>
+```shell
+mpirun -n 2 python heat_test.py
 ```
 
-The installation can then be done from the checked-out sources with
+It should print something like this:
 
+```shell
+x is distributed:  True
+Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
+Global DNDarray x:
+Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
+Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
 ```
-$ pip install heat[hdf5,netcdf,dev]
-```
-
-# Getting Started
-
-TL;DR: [Quick Start](quick_start.md) (Read this to get a quick overview of Heat).
 
-Check out our Jupyter Notebook [**Tutorial**](https://github.com/helmholtz-analytics/heat/blob/main/scripts/)
-right here on Github or in the /scripts directory, to learn and understand about the basics and working of Heat.
+Check out our Jupyter Notebook [**Tutorials**](https://github.com/helmholtz-analytics/heat/blob/main/tutorials/), choose `local` to try things out on your machine, or `hpc` if you have access to an HPC system.
 
 The complete documentation of the latest version is always deployed on
 [Read the Docs](https://heat.readthedocs.io/).
 
-***Try your first Heat program***
 
-```shell
-$ python
-```
+<!-- # Goals
 
-```python
->>> import heat as ht
->>> x = ht.arange(10,split=0)
->>> print(x)
-DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
->>> y = ht.ones(10,split=0)
->>> print(y)
-DNDarray([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.], dtype=ht.float32, device=cpu:0, split=0)
->>> print(x + y)
-DNDarray([ 1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.], dtype=ht.float32, device=cpu:0, split=0)
-```
+Heat is a flexible and seamless open-source software for high performance data
+analytics and machine learning. It provides highly optimized algorithms and data structures for tensor computations using CPUs, GPUs, and distributed cluster systems on top of MPI. The goal of Heat is to fill the gap between single-node data analytics and machine learning libraries, and  high-performance computing (HPC). Heat's interface integrates seamlessly with the existing data science ecosystem and makes  writing scalable
+scientific and data science applications as effortless as using NumPy.
 
-### Also, you can test your setup by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
+Heat allows you to tackle your actual Big Data challenges that go beyond the
+computational and memory needs of your laptop and desktop.
+ -->
+# Installation
 
-```shell
-mpirun -n 2 python heat_test.py
-```
+## Requirements
 
-### It should print something like this:
+### Basics
+- python >= 3.8
+- MPI (OpenMPI, MPICH, Intel MPI, etc.)
+- mpi4py >= 3.0.0
+- pytorch >= 1.8.0
 
-```shell
-x is distributed:  True
-Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
-Global DNDarray x:
-Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
-Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
-```
+### Parallel I/O
+- h5py
+- netCDF4
 
-## Resources:
+### GPU support
+In order to do computations on your GPU(s):
+- your CUDA or ROCm installation must match your hardware and its drivers;
+- your [PyTorch installation](https://pytorch.org/get-started/locally/) must be compiled with CUDA/ROCm support.
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
-* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+### HPC systems
+On most HPC-systems you will not be able to install/compile MPI or CUDA/ROCm yourself. Instead, you will most likely need to load a pre-installed MPI and/or CUDA/ROCm module from the module system. Maybe, you will even find PyTorch, h5py, or mpi4py as (part of) such a module. Note that for optimal performance on GPU, you need to usa an MPI library that has been compiled with CUDA/ROCm support (e.g., so-called "CUDA-aware MPI").
 
-### Parallel Computing and MPI:
 
-* @davidhenty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
-* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+## pip
+Install the latest version with
 
-### mpi4py
+```bash
+pip install heat[hdf5,netcdf]
+```
+where the part in brackets is a list of optional dependencies. You can omit
+it, if you do not need HDF5 or NetCDF support.
 
-* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
-* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
+## **conda**
 
-# Contribution guidelines
+The conda build includes all dependencies **including OpenMPI**.
+```bash
+ conda install -c conda-forge heat
+ ```
+
+# Support Channels
 
-**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) before getting started!**
+Go ahead and ask questions on [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions). If you found a bug or are missing a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose). You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
-We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion, and You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo). You can sign up with your GitHub credentials. Once you log in, you can introduce yourself on the `Town Square` channel.
 
-Small improvements or fixes are always appreciated; issues labeled as **"good first issue"** may be a good starting point.
+# Contribution guidelines
+
+**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) and [Resources](#resources)  before getting started!**
+
+We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion. You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
+
+## Resources
+
+* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+
+### Parallel Computing and MPI:
+
+* David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
+* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+* Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
+
+### mpi4py
+
+* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
+* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
 # License
 
 Heat is distributed under the MIT license, see our
 [LICENSE](LICENSE) file.
 
 # Citing Heat
 
-If you find Heat helpful for your research, please mention it in your publications. You can cite:
+<!-- If you find Heat helpful for your research, please mention it in your publications. You can cite: -->
+
+Please do mention Heat in your publications if it helped your research. You can cite:
 
 * Götz, M., Debus, C., Coquelin, D., Krajsek, K., Comito, C., Knechtges, P., Hagemeier, B., Tarnawa, M., Hanselmann, S., Siggel, S., Basermann, A. & Streit, A. (2020). HeAT - a Distributed and GPU-accelerated Tensor Framework for Data Analytics. In 2020 IEEE International Conference on Big Data (Big Data) (pp. 276-287). IEEE, DOI: 10.1109/BigData50022.2020.9378050.
 
 ```
 @inproceedings{heat2020,
     title={{HeAT -- a Distributed and GPU-accelerated Tensor Framework for Data Analytics}},
     author={
@@ -225,19 +208,29 @@
     year={2020},
     pages={276-287},
     month={December},
     publisher={IEEE},
     doi={10.1109/BigData50022.2020.9378050}
 }
 ```
+# FAQ
+Work in progress...
+
+  <!-- - Users
+  - Developers
+  - Students
+  - system administrators -->
 
 ## Acknowledgements
 
 *This work is supported by the [Helmholtz Association Initiative and
 Networking Fund](https://www.helmholtz.de/en/about_us/the_association/initiating_and_networking/)
 under project number ZT-I-0003 and the Helmholtz AI platform grant.*
 
+*This project has received funding from Google Summer of Code (GSoC) in 2022.*
+
+
 ---
 
 <div align="center">
-  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
+  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
 </div>
```

### Comparing `heat-1.3.1/README.md` & `heat-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,232 @@
+Metadata-Version: 2.1
+Name: heat
+Version: 1.4.0
+Summary: A framework for high-performance data analytics and machine learning.
+Home-page: https://github.com/helmholtz-analytics/heat
+Author: Helmholtz Association
+Author-email: martin.siggel@dlr.de
+Keywords: data,analytics,tensors,distributed,gpu
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mpi4py>=3.0.0
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: torch<2.2.3,>=1.11.0
+Requires-Dist: scipy>=1.10.0
+Requires-Dist: pillow>=6.0.0
+Requires-Dist: torchvision>=0.12.0
+Provides-Extra: docutils
+Requires-Dist: docutils>=0.16; extra == "docutils"
+Provides-Extra: hdf5
+Requires-Dist: h5py>=2.8.0; extra == "hdf5"
+Provides-Extra: netcdf
+Requires-Dist: netCDF4>=1.5.6; extra == "netcdf"
+Provides-Extra: dev
+Requires-Dist: pre-commit>=1.18.3; extra == "dev"
+Provides-Extra: examples
+Requires-Dist: scikit-learn>=0.24.0; extra == "examples"
+Requires-Dist: matplotlib>=3.1.0; extra == "examples"
+Provides-Extra: cb
+Requires-Dist: perun>=0.2.0; extra == "cb"
+
 <div align="center">
   <img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/logo.png">
 </div>
 
 ---
 
 Heat is a distributed tensor framework for high performance data analytics.
 
 # Project Status
 
-[![pipeline status](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
+[![CPU/CUDA/ROCm tests](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
 [![Documentation Status](https://readthedocs.org/projects/heat/badge/?version=latest)](https://heat.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![coverage](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
 [![license: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/heat)](https://pypi.org/project/heat/)
 [![Downloads](https://pepy.tech/badge/heat)](https://pepy.tech/project/heat)
-[![Github-Pages - Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/heat/badges/version.svg)](https://anaconda.org/conda-forge/heat)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/helmholtz-analytics/heat/badge)](https://securityscorecards.dev/viewer/?uri=github.com/helmholtz-analytics/heat)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7688/badge)](https://bestpractices.coreinfrastructure.org/projects/7688)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2531472.svg)](https://doi.org/10.5281/zenodo.2531472)
+[![Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-# Goals
+# Table of Contents
+  - [What is Heat for?](#what-is-heat-for)
+  - [Features](#features)
+  - [Getting Started](#getting-started)
+  - [Installation](#installation)
+    - [Requirements](#requirements)
+    - [pip](#pip)
+    - [conda](#conda)
+  - [Support Channels](#support-channels)
+  - [Contribution guidelines](#contribution-guidelines)
+    - [Resources](#resources)
+  - [License](#license)
+  - [Citing Heat](#citing-heat)
+  - [FAQ](#faq)
+  - [Acknowledgements](#acknowledgements)
 
-Heat is a flexible and seamless open-source software for high performance data
-analytics and machine learning. It provides highly optimized algorithms and data
-structures for tensor computations using CPUs, GPUs and distributed cluster
-systems on top of MPI. The goal of Heat is to fill the gap between data
-analytics and machine learning libraries with a strong focus on single-node
-performance, and traditional high-performance computing (HPC). Heat's generic
-Python-first programming interface integrates seamlessly with the existing data
-science ecosystem and makes it as effortless as using numpy to write scalable
-scientific and data science applications.
 
-Heat allows you to tackle your actual Big Data challenges that go beyond the
-computational and memory needs of your laptop and desktop.
+# What is Heat for?
 
-# Features
+Heat builds on [PyTorch](https://pytorch.org/) and [mpi4py](https://mpi4py.readthedocs.io) to provide high-performance computing infrastructure for memory-intensive applications within the NumPy/SciPy ecosystem.
 
-* High-performance n-dimensional tensors
-* CPU, GPU and distributed computation using MPI
-* Powerful data analytics and machine learning methods
-* Abstracted communication via split tensors
-* Python API
 
-# Support Channels
+With Heat you can:
+- port existing NumPy/SciPy code from single-CPU to multi-node clusters with minimal coding effort;
+- exploit the entire, cumulative RAM of your many nodes for memory-intensive operations and algorithms;
+- run your NumPy/SciPy code on GPUs (CUDA, ROCm, coming up: Apple MPS).
 
-We use [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions) as a forum for questions about Heat.
-If you found a bug or miss a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
+For a example that highlights the benefits of multi-node parallelism, hardware acceleration, and how easy this can be done with the help of Heat, see, e.g., our [blog post on trucated SVD of a 200GB data set](https://helmholtz-analytics.github.io/heat/2023/06/16/new-feature-hsvd.html).
 
-# Requirements
+Check out our [coverage tables](coverage_tables.md) to see which NumPy, SciPy, scikit-learn functions are already supported.
 
-Heat requires Python 3.7 or newer.
-Heat is based on [PyTorch](https://pytorch.org/). Specifically, we are exploiting
-PyTorch's support for GPUs *and* MPI parallelism. For MPI support we utilize
-[mpi4py](https://mpi4py.readthedocs.io). Both packages can be installed via pip
-or automatically using the setup.py.
+ If you need a functionality that is not yet supported:
+  - [search existing issues](https://github.com/helmholtz-analytics/heat/issues) and make sure to leave a comment if someone else already requested it;
+  - [open a new issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
 
-# Installation
 
-Tagged releases are made available on the
-[Python Package Index (PyPI)](https://pypi.org/project/heat/). You can typically
-install the latest version with
+Check out our [features](#features) and the [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html) for a complete list of functionalities.
 
-```
-$ pip install heat[hdf5,netcdf]
-```
+# Features
 
-where the part in brackets is a list of optional dependencies. You can omit
-it, if you do not need HDF5 or NetCDF support.
+* High-performance n-dimensional arrays
+* CPU, GPU, and distributed computation using MPI
+* Powerful data analytics and machine learning methods
+* Seamless integration with the NumPy/SciPy ecosystem
+* Python array API (work in progress)
 
-**It is recommended to use the most recent supported version of PyTorch!**
 
-**It is also very important to ensure that the PyTorch version is compatible with the local CUDA installation.**
-More information can be found [here](https://pytorch.org/get-started/locally/).
+# Getting Started
 
-# Hacking
+Go to [Quick Start](quick_start.md) for a quick overview. For more details, see [Installation](#installation).
 
-If you want to work with the development version, you can check out the sources using
+**You can test your setup** by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
 
-```
-$ git clone <https://github.com/helmholtz-analytics/heat.git>
+```shell
+mpirun -n 2 python heat_test.py
 ```
 
-The installation can then be done from the checked-out sources with
+It should print something like this:
 
+```shell
+x is distributed:  True
+Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
+Global DNDarray x:
+Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
+Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
 ```
-$ pip install heat[hdf5,netcdf,dev]
-```
-
-# Getting Started
-
-TL;DR: [Quick Start](quick_start.md) (Read this to get a quick overview of Heat).
 
-Check out our Jupyter Notebook [**Tutorial**](https://github.com/helmholtz-analytics/heat/blob/main/scripts/)
-right here on Github or in the /scripts directory, to learn and understand about the basics and working of Heat.
+Check out our Jupyter Notebook [**Tutorials**](https://github.com/helmholtz-analytics/heat/blob/main/tutorials/), choose `local` to try things out on your machine, or `hpc` if you have access to an HPC system.
 
 The complete documentation of the latest version is always deployed on
 [Read the Docs](https://heat.readthedocs.io/).
 
-***Try your first Heat program***
 
-```shell
-$ python
-```
+<!-- # Goals
 
-```python
->>> import heat as ht
->>> x = ht.arange(10,split=0)
->>> print(x)
-DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
->>> y = ht.ones(10,split=0)
->>> print(y)
-DNDarray([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.], dtype=ht.float32, device=cpu:0, split=0)
->>> print(x + y)
-DNDarray([ 1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.], dtype=ht.float32, device=cpu:0, split=0)
-```
+Heat is a flexible and seamless open-source software for high performance data
+analytics and machine learning. It provides highly optimized algorithms and data structures for tensor computations using CPUs, GPUs, and distributed cluster systems on top of MPI. The goal of Heat is to fill the gap between single-node data analytics and machine learning libraries, and  high-performance computing (HPC). Heat's interface integrates seamlessly with the existing data science ecosystem and makes  writing scalable
+scientific and data science applications as effortless as using NumPy.
 
-### Also, you can test your setup by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
+Heat allows you to tackle your actual Big Data challenges that go beyond the
+computational and memory needs of your laptop and desktop.
+ -->
+# Installation
 
-```shell
-mpirun -n 2 python heat_test.py
-```
+## Requirements
 
-### It should print something like this:
+### Basics
+- python >= 3.8
+- MPI (OpenMPI, MPICH, Intel MPI, etc.)
+- mpi4py >= 3.0.0
+- pytorch >= 1.8.0
 
-```shell
-x is distributed:  True
-Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
-Global DNDarray x:
-Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
-Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
-```
+### Parallel I/O
+- h5py
+- netCDF4
 
-## Resources:
+### GPU support
+In order to do computations on your GPU(s):
+- your CUDA or ROCm installation must match your hardware and its drivers;
+- your [PyTorch installation](https://pytorch.org/get-started/locally/) must be compiled with CUDA/ROCm support.
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
-* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+### HPC systems
+On most HPC-systems you will not be able to install/compile MPI or CUDA/ROCm yourself. Instead, you will most likely need to load a pre-installed MPI and/or CUDA/ROCm module from the module system. Maybe, you will even find PyTorch, h5py, or mpi4py as (part of) such a module. Note that for optimal performance on GPU, you need to usa an MPI library that has been compiled with CUDA/ROCm support (e.g., so-called "CUDA-aware MPI").
 
-### Parallel Computing and MPI:
 
-* @davidhenty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
-* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+## pip
+Install the latest version with
 
-### mpi4py
+```bash
+pip install heat[hdf5,netcdf]
+```
+where the part in brackets is a list of optional dependencies. You can omit
+it, if you do not need HDF5 or NetCDF support.
 
-* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
-* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
+## **conda**
 
-# Contribution guidelines
+The conda build includes all dependencies **including OpenMPI**.
+```bash
+ conda install -c conda-forge heat
+ ```
+
+# Support Channels
 
-**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) before getting started!**
+Go ahead and ask questions on [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions). If you found a bug or are missing a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose). You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
-We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion, and You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo). You can sign up with your GitHub credentials. Once you log in, you can introduce yourself on the `Town Square` channel.
 
-Small improvements or fixes are always appreciated; issues labeled as **"good first issue"** may be a good starting point.
+# Contribution guidelines
+
+**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) and [Resources](#resources)  before getting started!**
+
+We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion. You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
+
+## Resources
+
+* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+
+### Parallel Computing and MPI:
+
+* David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
+* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+* Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
+
+### mpi4py
+
+* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
+* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
 # License
 
 Heat is distributed under the MIT license, see our
 [LICENSE](LICENSE) file.
 
 # Citing Heat
 
-If you find Heat helpful for your research, please mention it in your publications. You can cite:
+<!-- If you find Heat helpful for your research, please mention it in your publications. You can cite: -->
+
+Please do mention Heat in your publications if it helped your research. You can cite:
 
 * Götz, M., Debus, C., Coquelin, D., Krajsek, K., Comito, C., Knechtges, P., Hagemeier, B., Tarnawa, M., Hanselmann, S., Siggel, S., Basermann, A. & Streit, A. (2020). HeAT - a Distributed and GPU-accelerated Tensor Framework for Data Analytics. In 2020 IEEE International Conference on Big Data (Big Data) (pp. 276-287). IEEE, DOI: 10.1109/BigData50022.2020.9378050.
 
 ```
 @inproceedings{heat2020,
     title={{HeAT -- a Distributed and GPU-accelerated Tensor Framework for Data Analytics}},
     author={
@@ -187,19 +247,29 @@
     year={2020},
     pages={276-287},
     month={December},
     publisher={IEEE},
     doi={10.1109/BigData50022.2020.9378050}
 }
 ```
+# FAQ
+Work in progress...
+
+  <!-- - Users
+  - Developers
+  - Students
+  - system administrators -->
 
 ## Acknowledgements
 
 *This work is supported by the [Helmholtz Association Initiative and
 Networking Fund](https://www.helmholtz.de/en/about_us/the_association/initiating_and_networking/)
 under project number ZT-I-0003 and the Helmholtz AI platform grant.*
 
+*This project has received funding from Google Summer of Code (GSoC) in 2022.*
+
+
 ---
 
 <div align="center">
-  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
+  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
 </div>
```

### Comparing `heat-1.3.1/heat/classification/kneighborsclassifier.py` & `heat-1.4.0/heat/classification/kneighborsclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implements the k-nearest neighbors (kNN) classifier"""
+
 from typing import Callable
 
 import heat as ht
 
 from heat.core.dndarray import DNDarray
```

### Comparing `heat-1.3.1/heat/cluster/_kcluster.py` & `heat-1.4.0/heat/cluster/_kcluster.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     n_clusters : int
         The number of clusters to form as well as the number of centroids to generate.
     init : str or DNDarray, default: ‘random’
         Method for initialization:
 
         - ‘probability_based’ : selects initial cluster centers for the clustering in a smart way to speed up convergence (k-means++)
         - ‘random’: choose k observations (rows) at random from data for the initial centroids.
+        - 'batchparallel': use the batch parallel algorithm to initialize the centroids, only available for split=0 and KMeans or KMedians
         - ``DNDarray``: gives the initial centers, should be of Shape = (n_clusters, n_features)
     max_iter : int
         Maximum number of iterations for a single run.
     tol : float, default: 1e-4
         Relative tolerance with regards to inertia to declare convergence.
     random_state : int
         Determines random number generation for centroid initialization.
@@ -46,17 +47,19 @@
         self.max_iter = max_iter
         self.tol = tol
         self.random_state = random_state
 
         # in-place properties
         self._metric = metric
         self._cluster_centers = None
+        self._functional_value = None
         self._labels = None
         self._inertia = None
         self._n_iter = None
+        self._p = None
 
     @property
     def cluster_centers_(self) -> DNDarray:
         """
         Returns the coordinates of the cluster centers.
         If the algorithm stops before fully converging (see ``tol`` and ``max_iter``),
         these will not be consistent with :func:`labels_`.
@@ -80,14 +83,21 @@
     @property
     def n_iter_(self) -> int:
         """
         Returns the number of iterations run.
         """
         return self._n_iter
 
+    @property
+    def functional_value_(self) -> DNDarray:
+        """
+        Returns the K-Clustering functional value of the clustering algorithm
+        """
+        return self._functional_value
+
     def _initialize_cluster_centers(self, x: DNDarray):
         """
         Initializes the K-Means centroids.
 
         Parameters
         ----------
         x : DNDarray
@@ -128,15 +138,15 @@
 
             self._cluster_centers = centroids
 
         # directly passed centroids
         elif isinstance(self.init, DNDarray):
             if len(self.init.shape) != 2:
                 raise ValueError(
-                    "passed centroids need to be two-dimensional, but are {}".format(len(self.init))
+                    f"passed centroids need to be two-dimensional, but are {len(self.init)}"
                 )
             if self.init.shape[0] != self.n_clusters or self.init.shape[1] != x.shape[1]:
                 raise ValueError("passed centroids do not match cluster count or data shape")
             self._cluster_centers = self.init.resplit(None)
 
         # Smart centroid guessing, random sampling with probability weight proportional to distance to existing centroids
         elif self.init == "probability_based":
@@ -182,34 +192,66 @@
                     xi.comm.Bcast(xi, root=proc)
                     centroids[i, :] = xi
 
             else:
                 raise NotImplementedError("Not implemented for other splitting-axes")
             self._cluster_centers = centroids
 
+        elif self.init == "batchparallel":
+            if x.split == 0:
+                if self._p == 2:
+                    batch_parallel_clusterer = ht.cluster.BatchParallelKMeans(
+                        n_clusters=self.n_clusters,
+                        init="k-means++",
+                        max_iter=100,
+                        random_state=self.random_state,
+                    )
+                elif self._p == 1:
+                    batch_parallel_clusterer = ht.cluster.BatchParallelKMedians(
+                        n_clusters=self.n_clusters,
+                        init="k-medians++",
+                        max_iter=100,
+                        random_state=self.random_state,
+                    )
+                else:
+                    raise ValueError(
+                        "Batch parallel initialization only implemented for KMeans and KMedians"
+                    )
+                batch_parallel_clusterer.fit(x)
+                self._cluster_centers = batch_parallel_clusterer.cluster_centers_
+            else:
+                raise NotImplementedError(
+                    f"Batch parallel initalization only implemented for split = 0, but split was {x.split}"
+                )
+
         else:
             raise ValueError(
-                'init needs to be one of "random", ht.DNDarray or "kmeans++", but was {}'.format(
+                'init needs to be one of "random", ht.DNDarray, "kmeans++", or "batchparallel", but was {}'.format(
                     self.init
                 )
             )
 
-    def _assign_to_cluster(self, x: DNDarray):
+    def _assign_to_cluster(self, x: DNDarray, eval_functional_value: bool = False):
         """
         Assigns the passed data points to the centroids based on the respective metric
 
         Parameters
         ----------
         x : DNDarray
             Data points, Shape = (n_samples, n_features)
+        eval_functional_value : bool, default: False
+            If True, the current K-Clustering functional value of the clustering algorithm is evaluated
         """
         # calculate the distance matrix and determine the closest centroid
         distances = self._metric(x, self._cluster_centers)
         matching_centroids = distances.argmin(axis=1, keepdims=True)
 
+        if eval_functional_value:
+            self._functional_value = ht.norm(distances.min(axis=1), ord=self._p) ** self._p
+
         return matching_centroids
 
     def _update_centroids(self, x: DNDarray, matching_centroids: DNDarray):
         """
         The Update strategy is algorithm specific (e.g. calculate mean of assigned points for kmeans, median for kmedians, etc.)
 
         Parameters
@@ -247,8 +289,8 @@
             New data to predict. Shape = (n_samples, n_features)
         """
         # input sanitation
         if not isinstance(x, DNDarray):
             raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
 
         # determine the centroids
-        return self._assign_to_cluster(x)
+        return self._assign_to_cluster(x, eval_functional_value=True)
```

### Comparing `heat-1.3.1/heat/cluster/kmeans.py` & `heat-1.4.0/heat/cluster/kmeans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module Implementing the Kmeans Algorithm
 """
+
 from typing import Optional, Union, TypeVar
 
 import heat as ht
 from heat.cluster._kcluster import _KCluster
 from heat.core.dndarray import DNDarray
 
 self = TypeVar("self")
@@ -19,14 +20,15 @@
     n_clusters : int
         The number of clusters to form as well as the number of centroids to generate.
     init : str or DNDarray
         Method for initialization:
 
         - ‘k-means++’ : selects initial cluster centers for the clustering in a smart way to speed up convergence [2].
         - ‘random’: choose k observations (rows) at random from data for the initial centroids.
+        - 'batchparallel': initialize by using the batch parallel algorithm (see BatchParallelKMeans for more information).
         - DNDarray: it should be of shape (n_clusters, n_features) and gives the initial centers.
     max_iter : int
         Maximum number of iterations of the k-means algorithm for a single run.
     tol : float
         Relative tolerance with regards to inertia to declare convergence.
     random_state : int
         Determines random number generation for centroid initialization.
@@ -65,14 +67,15 @@
             metric=lambda x, y: ht.spatial.distance.cdist(x, y, quadratic_expansion=True),
             n_clusters=n_clusters,
             init=init,
             max_iter=max_iter,
             tol=tol,
             random_state=random_state,
         )
+        self._p = 2
 
     def _update_centroids(self, x: DNDarray, matching_centroids: DNDarray):
         """
         Compute coordinates of new centroid as mean of the data points in ``x`` that are assigned to this centroid.
 
         Parameters
         ----------
```

### Comparing `heat-1.3.1/heat/cluster/kmedians.py` & `heat-1.4.0/heat/cluster/kmedians.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module Implementing the Kmedians Algorithm
 """
+
 import heat as ht
 from heat.cluster._kcluster import _KCluster
 from heat.core.dndarray import DNDarray
 from typing import Optional, Union, TypeVar
 
 
 class KMedians(_KCluster):
@@ -17,14 +18,15 @@
     n_clusters : int, optional, default: 8
         The number of clusters to form as well as the number of centroids to generate.
     init : str or DNDarray, default: ‘random’
         Method for initialization:
 
              - ‘k-medians++’ : selects initial cluster centers for the clustering in a smart way to speed up convergence [2].
              - ‘random’: choose k observations (rows) at random from data for the initial centroids.
+             - 'batchparallel': initialize by using the batch parallel algorithm (see BatchParallelKMedians for more information).
              - DNDarray: gives the initial centers, should be of Shape = (n_clusters, n_features)
     max_iter : int, default: 300
         Maximum number of iterations of the k-means algorithm for a single run.
     tol : float, default: 1e-4
         Relative tolerance with regards to inertia to declare convergence.
     random_state : int
         Determines random number generation for centroid initialization.
@@ -49,14 +51,15 @@
             metric=lambda x, y: ht.spatial.distance.manhattan(x, y, expand=True),
             n_clusters=n_clusters,
             init=init,
             max_iter=max_iter,
             tol=tol,
             random_state=random_state,
         )
+        self._p = 1
 
     def _update_centroids(self, x: DNDarray, matching_centroids: DNDarray):
         """
         Compute coordinates of new centroid as median of the data points in ``x`` that are assigned to it
 
         Parameters
         ----------
```

### Comparing `heat-1.3.1/heat/cluster/kmedoids.py` & `heat-1.4.0/heat/cluster/kmedoids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module Implementing the Kmedoids Algorithm
 """
+
 import heat as ht
 from heat.cluster._kcluster import _KCluster
 from heat.core.dndarray import DNDarray
 from typing import Optional, Union, TypeVar
 
 
 class KMedoids(_KCluster):
```

### Comparing `heat-1.3.1/heat/cluster/spectral.py` & `heat-1.4.0/heat/cluster/spectral.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/__init__.py` & `heat-1.4.0/heat/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ._operations import *
 from .printing import *
 from . import random
 from .relational import *
 from .rounding import *
 from .sanitation import *
 from .statistics import *
+from .stride_tricks import *
 from .dndarray import *
 from .tiling import *
 from .trigonometrics import *
 from .types import *
 from .signal import *
 from .types import finfo, iinfo
 from . import version
```

### Comparing `heat-1.3.1/heat/core/_operations.py` & `heat-1.4.0/heat/core/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def __binary_op(
     operation: Callable,
     t1: Union[DNDarray, int, float],
     t2: Union[DNDarray, int, float],
     out: Optional[DNDarray] = None,
-    where: Optional[DNDarray] = None,
+    where: Union[bool, DNDarray] = True,
     fn_kwargs: Optional[Dict] = {},
 ) -> DNDarray:
     """
     Generic wrapper for element-wise binary operations of two operands (either can be tensor or scalar).
     Takes the operation function and the two operands involved in the operation as arguments.
 
     Parameters
@@ -80,14 +80,40 @@
         )
     if not np.isscalar(t2) and not isinstance(t2, DNDarray):
         raise TypeError(
             f"Only DNDarrays and numeric scalars are supported, but input was {type(t2)}"
         )
     promoted_type = types.result_type(t1, t2).torch_type()
 
+    # Type check for in-place operators
+    in_place_arithmetics = {
+        "wrap_add_",
+        "wrap_bitwise_and_",
+        "wrap_bitwise_or_",
+        "wrap_bitwise_xor_",
+        "wrap_div_",
+        "wrap_floordiv_",
+        "wrap_fmod_",
+        "wrap_gcd_",
+        "wrap_hypot_",
+        "wrap_lcm_",
+        "wrap_bitwise_left_shift_",
+        "wrap_mul_",
+        "wrap_pow_",
+        "wrap_remainder_",
+        "wrap_bitwise_right_shift_",
+        "wrap_sub_",
+    }
+    if operation.__name__ in in_place_arithmetics:
+        if not types.can_cast(types.heat_type_of(t2), types.heat_type_of(t1)):
+            raise TypeError(
+                f"Cannot cast from {types.heat_type_of(t2)} to {types.heat_type_of(t1)} for "
+                + "in-place operations."
+            )
+
     # Make inputs Dndarrays
     if np.isscalar(t1) and np.isscalar(t2):
         try:
             t1 = factories.array(t1)
             t2 = factories.array(t2)
         except (ValueError, TypeError):
             raise TypeError(f"Data type not supported, inputs were {type(t1)} and {type(t2)}")
@@ -100,15 +126,15 @@
         try:
             t2 = factories.array(t2, device=t1.device, comm=t1.comm)
         except (ValueError, TypeError):
             raise TypeError(f"Data type not supported, input was {type(t2)}")
 
     # Make inputs have the same dimensionality
     output_shape = stride_tricks.broadcast_shape(t1.shape, t2.shape)
-    if where is not None:
+    if where is not True:
         output_shape = stride_tricks.broadcast_shape(where.shape, output_shape)
         while len(where.shape) < len(output_shape):
             where = where.expand_dims(axis=0)
     # Broadcasting allows additional empty dimensions on the left side
     # TODO simplify this once newaxis-indexing is supported to get rid of the loops
     while len(t1.shape) < len(output_shape):
         t1 = t1.expand_dims(axis=0)
@@ -169,26 +195,26 @@
 
     if out is not None:
         sanitation.sanitize_out(out, output_shape, output_split, output_device, output_comm)
         t1, t2 = sanitation.sanitize_distribution(t1, t2, target=out)
 
     result = operation(t1.larray.to(promoted_type), t2.larray.to(promoted_type), **fn_kwargs)
 
-    if out is None and where is None:
+    if out is None and where is True:
         return DNDarray(
             result,
             output_shape,
             types.heat_type_of(result),
             output_split,
             device=output_device,
             comm=output_comm,
             balanced=output_balanced,
         )
 
-    if where is not None:
+    if where is not True:
         if out is None:
             out = factories.empty(
                 output_shape,
                 dtype=promoted_type,
                 split=output_split,
                 device=output_device,
                 comm=output_comm,
@@ -355,25 +381,24 @@
             x.gshape,
             types.canonical_heat_type(result.dtype),
             x.split,
             x.device,
             x.comm,
             x.balanced,
         )
-
     # output buffer writing requires a bit more work
     # we need to determine whether the operands are broadcastable and the multiple of the broadcasting
     # reason: manually repetition for each dimension as PyTorch does not conform to numpy's broadcast semantic
     # PyTorch always recreates the input shape and ignores broadcasting for too large buffers
     broadcast_shape = stride_tricks.broadcast_shape(x.lshape, out.lshape)
     padded_shape = (1,) * (len(broadcast_shape) - len(x.lshape)) + x.lshape
     multiples = [(int(a / b) if b > 0 else 0) for a, b in zip(broadcast_shape, padded_shape)]
     needs_repetition = builtins.any(multiple > 1 for multiple in multiples)
 
-    # do an inplace operation into a provided buffer
+    # do an in-place operation into a provided buffer
     casted = x.larray.type(torch_type)
     operation(casted.repeat(multiples) if needs_repetition else casted, out=out.larray, **kwargs)
 
     return out
 
 
 def __reduce_op(
@@ -433,16 +458,20 @@
             device=x.device.torch_device,
         )
     else:
         partial = x.larray
 
     # apply the partial reduction operation to the local tensor
     if axis is None:
-        partial = partial_op(partial).reshape(-1)
-        output_shape = (1,)
+        partial = partial_op(partial)
+        if partial.ndim > 0:
+            partial = partial.reshape(-1)
+            output_shape = (1,)
+        else:
+            output_shape = ()
         balanced = True
     else:
         output_shape = x.gshape
         for dim in axis:
             if not (
                 partial.shape.numel() == 0 and partial_op.__name__ in ("local_max", "local_min")
             ):  # no neutral element for max/min
```

### Comparing `heat-1.3.1/heat/core/base.py` & `heat-1.4.0/heat/core/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .dndarray import DNDarray
 
 self = TypeVar("self")
 
 
 class BaseEstimator:
     """
-    Abstract base class for all estimators, i.e. parametrized analysis algorithms, in HeAT. Can be used as mixin.
+    Abstract base class for all estimators, i.e. parametrized analysis algorithms, in Heat. Can be used as mixin.
     """
 
     @classmethod
     def _parameter_names(cls) -> List[str]:
         """
         Get the names of all parameters that can be set inside the constructor of the estimator.
         """
@@ -59,15 +59,15 @@
         Returns a printable representation of the object.
 
         Parameters
         ----------
         indent : int, default: 1
             Indicates the indentation for the top-level output.
         """
-        return "{}({})".format(self.__class__.__name__, json.dumps(self.get_params(), indent=4))
+        return f"{self.__class__.__name__}({json.dumps(self.get_params(), indent=4)})"
 
     def set_params(self, **params: Dict[str, object]) -> self:
         """
         Set the parameters of this estimator. The method works on simple estimators as well as on nested objects
         (such as pipelines). The latter have to be nested dictionaries.
 
         Parameters
@@ -91,15 +91,15 @@
                 setattr(self, key, value)
 
         return self
 
 
 class ClassificationMixin:
     """
-    Mixin for all classifiers in HeAT.
+    Mixin for all classifiers in Heat.
     """
 
     def fit(self, x: DNDarray, y: DNDarray):
         """
         Fits the classification model.
 
         Parameters
@@ -136,17 +136,58 @@
         ----------
         x : DNDarray
             Values to predict the classes for. Shape = (n_samples, n_features)
         """
         raise NotImplementedError()
 
 
+class TransformMixin:
+    """
+    Mixin for all transformations in Heat.
+    """
+
+    def fit(self, x: DNDarray):
+        """
+        Fits the transformation model.
+
+        Parameters
+        ----------
+        x : DNDarray
+            Training instances to train on. Shape = (n_samples, n_features)
+        """
+        raise NotImplementedError()
+
+    def fit_transform(self, x: DNDarray) -> DNDarray:
+        """
+        Fits model and returns transformed data for each input sample
+        Convenience method; equivalent to calling :func:`fit` followed by :func:`transform`.
+
+        Parameters
+        ----------
+        x : DNDarray
+            Input data to be transformed. Shape = (n_samples, n_features)
+        """
+        self.fit(x)
+        return self.transform(x)
+
+    def transform(self, x: DNDarray) -> DNDarray:
+        """
+        Transforms the input data.
+
+         Parameters
+         ----------
+         x : DNDarray
+             Values to transform. Shape = (n_samples, n_features)
+        """
+        raise NotImplementedError()
+
+
 class ClusteringMixin:
     """
-    Clustering mixin for all clusterers in HeAT.
+    Clustering mixin for all clusterers in Heat.
     """
 
     def fit(self, x: DNDarray):
         """
         Computes the clustering.
 
         Parameters
@@ -169,15 +210,15 @@
         """
         self.fit(x)
         return self.predict(x)
 
 
 class RegressionMixin:
     """
-    Mixin for all regression estimators in HeAT.
+    Mixin for all regression estimators in Heat.
     """
 
     def fit(self, x: DNDarray, y: DNDarray):
         """
         Fits the regression model.
 
         Parameters
@@ -224,14 +265,26 @@
     ----------
     estimator : object
         Estimator object to test.
     """
     return isinstance(estimator, ClassificationMixin)
 
 
+def is_transformer(estimator: object) -> bool:
+    """
+    Return ``True`` if the given estimator is a transformer, ``False`` otherwise.
+
+    Parameters
+    ----------
+    estimator : object
+        Estimator object to test.
+    """
+    return isinstance(estimator, TransformMixin)
+
+
 def is_estimator(estimator: object) -> bool:
     """
     Return ``True`` if the given estimator is an estimator, ``False`` otherwise.
 
     Parameters
     ----------
     estimator : object
```

### Comparing `heat-1.3.1/heat/core/communication.py` & `heat-1.4.0/heat/core/communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Module implementing the communication layer of HeAT
 """
+
 from __future__ import annotations
 
 import numpy as np
 import os
 import subprocess
 import torch
-
 from mpi4py import MPI
-from typing import Any, Callable, Optional, List, Tuple, Union
 
+from typing import Any, Callable, Optional, List, Tuple, Union
 from .stride_tricks import sanitize_axis
 
 CUDA_AWARE_MPI = False
 # check whether OpenMPI support CUDA-aware MPI
 if "openmpi" in os.environ.get("MPI_SUFFIX", "").lower():
     buffer = subprocess.check_output(["ompi_info", "--parsable", "--all"])
     CUDA_AWARE_MPI = b"mpi_built_with_cuda_support:value:true" in buffer
@@ -59,22 +59,18 @@
         self.permutation = permutation
 
     def Wait(self, status: MPI.Status = None):
         """
         Waits for an MPI request to complete
         """
         self.handle.Wait(status)
-        if (
-            self.tensor is not None
-            and isinstance(self.tensor, torch.Tensor)
-            and self.tensor.is_cuda
-            and not CUDA_AWARE_MPI
-        ):
+        if self.tensor is not None and isinstance(self.tensor, torch.Tensor):
             if self.permutation is not None:
                 self.recvbuf = self.recvbuf.permute(self.permutation)
+        if self.tensor is not None and self.tensor.is_cuda and not CUDA_AWARE_MPI:
             self.tensor.copy_(self.recvbuf)
 
     def __getattr__(self, name: str) -> Callable:
         """
         Default pass-through for the communicator methods.
 
         Parameters
@@ -804,26 +800,51 @@
         # MPI requires send and receive buffers to be of same type and length. If the torch tensors are either not both
         # contiguous or differently strided, they have to be made matching (if possible) first.
         if isinstance(sendbuf, torch.Tensor):
             # convert the send buffer to a pointer, number of elements and type are identical to the receive buffer
             dummy = (
                 sendbuf.contiguous()
             )  # make a contiguous copy and reassign the storage, old will be collected
-            sendbuf.set_(
-                dummy.storage(), dummy.storage_offset(), size=dummy.shape, stride=dummy.stride()
-            )
+            # In PyTorch Version >= 2.0.0 we can use untyped_storage() instead of storage
+            # to keep backward compatibility with earlier PyTorch versions (where no untyped_storage() exists) we use a try/except
+            # (this applies to all places of Heat where untyped_storage() is used without further comment)
+            try:
+                sendbuf.set_(
+                    dummy.untyped_storage(),
+                    dummy.storage_offset(),
+                    size=dummy.shape,
+                    stride=dummy.stride(),
+                )
+            except AttributeError:
+                sendbuf.set_(
+                    dummy.storage(),
+                    dummy.storage_offset(),
+                    size=dummy.shape,
+                    stride=dummy.stride(),
+                )
             sbuf = sendbuf if CUDA_AWARE_MPI else sendbuf.cpu()
             sendbuf = self.as_buffer(sbuf)
         if isinstance(recvbuf, torch.Tensor):
             buf = recvbuf
             # nothing matches, the buffers have to be made contiguous
             dummy = recvbuf.contiguous()
-            recvbuf.set_(
-                dummy.storage(), dummy.storage_offset(), size=dummy.shape, stride=dummy.stride()
-            )
+            try:
+                recvbuf.set_(
+                    dummy.untyped_storage(),
+                    dummy.storage_offset(),
+                    size=dummy.shape,
+                    stride=dummy.stride(),
+                )
+            except AttributeError:
+                recvbuf.set_(
+                    dummy.storage(),
+                    dummy.storage_offset(),
+                    size=dummy.shape,
+                    stride=dummy.stride(),
+                )
             rbuf = recvbuf if CUDA_AWARE_MPI else recvbuf.cpu()
             if sendbuf is MPI.IN_PLACE:
                 recvbuf = self.as_buffer(rbuf)
             else:
                 recvbuf = (self.as_mpi_memory(rbuf), sendbuf[1], sendbuf[2])
 
         # perform the actual reduction operation
@@ -1123,17 +1144,17 @@
             Buffer address where to store the result
         recv_axis: int
             Concatenation axis: The axis along which ``sendbuf`` is packed and along which ``recvbuf`` puts together individual chunks
         """
         ret, sbuf, rbuf, buf, permutation = self.__allgather_like(
             self.handle.Allgather, sendbuf, recvbuf, recv_axis
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Allgather.__doc__ = MPI.Comm.Allgather.__doc__
 
     def Allgatherv(
         self,
@@ -1152,17 +1173,17 @@
             Buffer address where to store the result
         recv_axis: int
             Concatenation axis: The axis along which ``sendbuf`` is packed and along which ``recvbuf`` puts together individual chunks
         """
         ret, sbuf, rbuf, buf, permutation = self.__allgather_like(
             self.handle.Allgatherv, sendbuf, recvbuf, recv_axis
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Allgatherv.__doc__ = MPI.Comm.Allgatherv.__doc__
 
     def Iallgather(
         self,
@@ -1341,15 +1362,15 @@
                 if CUDA_AWARE_MPI or not isinstance(recvbuf, torch.Tensor)
                 else recvbuf.cpu()
             )
             mpi_sendbuf = self.alltoall_sendbuffer(sbuf)
             mpi_recvbuf = self.alltoall_recvbuffer(rbuf)
 
             exit_code = self.handle.Alltoallw(mpi_sendbuf, mpi_recvbuf, **kwargs)
-            # original_recvbuf.set_(recvbuf.storage(), recvbuf.storage_offset(), original_recvbuf.shape, original_recvbuf.stride())
+            # original_recvbuf.set_(recvbuf.untyped_storage(), recvbuf.storage_offset(), original_recvbuf.shape, original_recvbuf.stride())
             recv_axis_permutation = list(np.argsort(np.array(axis_permutation)))
 
         return exit_code, sbuf, rbuf, original_recvbuf, recv_axis_permutation
 
     def Alltoall(
         self,
         sendbuf: Union[DNDarray, torch.Tensor, Any],
@@ -1374,17 +1395,17 @@
                 - if ``send_axis`` or ``recv_axis`` are ``None``, an error will be thrown
         recv_axis: int
             Prior split axis, along which blocks are received from the individual ranks
         """
         ret, sbuf, rbuf, buf, permutation = self.__alltoall_like(
             self.handle.Alltoall, sendbuf, recvbuf, send_axis, recv_axis
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Alltoall.__doc__ = MPI.Comm.Alltoall.__doc__
 
     def Alltoallv(
         self,
@@ -1410,17 +1431,17 @@
                 - if ``send_axis`` or ``recv_axis`` are ``None``, an error will be thrown
         recv_axis: int
             Prior split axis, along which blocks are received from the individual ranks
         """
         ret, sbuf, rbuf, buf, permutation = self.__alltoall_like(
             self.handle.Alltoallv, sendbuf, recvbuf, send_axis, recv_axis
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Alltoallv.__doc__ = MPI.Comm.Alltoallv.__doc__
 
     def Ialltoall(
         self,
@@ -1479,27 +1500,27 @@
         """
         return MPIRequest(
             *self.__alltoall_like(self.handle.Ialltoallv, sendbuf, recvbuf, send_axis, recv_axis)
         )
 
     Ialltoallv.__doc__ = MPI.Comm.Ialltoallv.__doc__
 
-    def __scatter_like(
+    def __gather_like(
         self,
         func: Callable,
         sendbuf: Union[DNDarray, torch.Tensor, Any],
         recvbuf: Union[DNDarray, torch.Tensor, Any],
         send_axis: int,
         recv_axis: int,
         send_factor: int = 1,
         recv_factor: int = 1,
         **kwargs,
     ):
         """
-        Generic function for scatter and gather operations.
+        Generic function for gather operations.
 
         Parameters
         ----------
         func: Callable
             Type of MPI Scatter/Gather function
         sendbuf: Union[DNDarray, torch.Tensor, Any]
             Buffer address of the send message
@@ -1520,41 +1541,41 @@
         if recv_axis is None:
             recv_axis = send_axis
 
         # dummy allocation for *v calls
         send_counts, send_displs, recv_counts, recv_displs = None, None, None, None
 
         # unpack the send buffer
-        if isinstance(sendbuf, tuple):
-            sendbuf, send_counts, send_displs = sendbuf
+        # if isinstance(sendbuf, tuple):
+        #     sendbuf, send_counts, send_displs = sendbuf
         if isinstance(sendbuf, DNDarray):
             sendbuf = sendbuf.larray
         if not isinstance(sendbuf, torch.Tensor) and send_axis != 0:
             raise TypeError(f"sendbuf of type {type(sendbuf)} does not support send_axis != 0")
 
         # unpack the receive buffer
         if isinstance(recvbuf, tuple):
             recvbuf, recv_counts, recv_displs = recvbuf
         if isinstance(recvbuf, DNDarray):
             recvbuf = recvbuf.larray
-        if not isinstance(recvbuf, torch.Tensor) and send_axis != 0:
-            raise TypeError(f"recvbuf of type {type(recvbuf)} does not support send_axis != 0")
+        if not isinstance(recvbuf, torch.Tensor) and recv_axis != 0:
+            raise TypeError(f"recvbuf of type {type(recvbuf)} does not support recv_axis != 0")
 
         # keep a reference to the original buffer object
         original_recvbuf = recvbuf
 
         # permute the send_axis order so that the split send_axis is the first to be transmitted
-        send_axis_permutation = list(range(recvbuf.ndimension()))
+        send_axis_permutation = list(range(sendbuf.ndimension()))
         send_axis_permutation[0], send_axis_permutation[send_axis] = send_axis, 0
-        if self.rank == kwargs.get("root", -1) or send_counts is not None:
-            sendbuf = sendbuf.permute(*send_axis_permutation)
+        sendbuf = sendbuf.permute(*send_axis_permutation)
 
-        recv_axis_permutation = list(range(recvbuf.ndimension()))
-        recv_axis_permutation[0], recv_axis_permutation[recv_axis] = recv_axis, 0
-        recvbuf = recvbuf.permute(*recv_axis_permutation)
+        if self.rank == kwargs.get("root"):
+            recv_axis_permutation = list(range(recvbuf.ndimension()))
+            recv_axis_permutation[0], recv_axis_permutation[recv_axis] = recv_axis, 0
+            recvbuf = recvbuf.permute(*recv_axis_permutation)
 
         # prepare buffer objects
         sbuf = sendbuf if CUDA_AWARE_MPI or not isinstance(sendbuf, torch.Tensor) else sendbuf.cpu()
         rbuf = recvbuf if CUDA_AWARE_MPI or not isinstance(recvbuf, torch.Tensor) else recvbuf.cpu()
 
         if sendbuf is not MPI.IN_PLACE:
             mpi_sendbuf = self.as_buffer(sbuf, send_counts, send_displs)
@@ -1571,15 +1592,15 @@
 
         # perform the scatter operation
         exit_code = func(mpi_sendbuf, mpi_recvbuf, **kwargs)
 
         # undo the recvbuf permutation and assign the temporary buffer to the original recvbuf
         # if recv_axis != 0:
         #    recvbuf = recvbuf.permute(*recv_axis_permutation)
-        #    original_recvbuf.set_(recvbuf.storage(), recvbuf.storage_offset(), recvbuf.shape, recvbuf.stride())
+        #    original_recvbuf.set_(recvbuf.untyped_storage(), recvbuf.storage_offset(), recvbuf.shape, recvbuf.stride())
 
         return exit_code, sbuf, rbuf, original_recvbuf, recv_axis_permutation
 
     def Gather(
         self,
         sendbuf: Union[DNDarray, torch.Tensor, Any],
         recvbuf: Union[DNDarray, torch.Tensor, Any],
@@ -1599,20 +1620,20 @@
         root: int
             Rank of receiving process
         axis: int
             The axis along which ``sendbuf`` is packed
         recv_axis: int
             The axis along which ``recvbuf`` is packed
         """
-        ret, sbuf, rbuf, buf, permutation = self.__scatter_like(
+        ret, sbuf, rbuf, buf, permutation = self.__gather_like(
             self.handle.Gather, sendbuf, recvbuf, axis, recv_axis, root=root, recv_factor=self.size
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Gather.__doc__ = MPI.Comm.Gather.__doc__
 
     def Gatherv(
         self,
@@ -1634,20 +1655,20 @@
         root: int
             Rank of receiving process
         axis: int
             The axis along which ``sendbuf`` is packed
         recv_axis: int
             The axis along which ``recvbuf`` is packed
         """
-        ret, sbuf, rbuf, buf, permutation = self.__scatter_like(
+        ret, sbuf, rbuf, buf, permutation = self.__gather_like(
             self.handle.Gatherv, sendbuf, recvbuf, axis, recv_axis, root=root
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Gatherv.__doc__ = MPI.Comm.Gatherv.__doc__
 
     def Igather(
         self,
@@ -1670,15 +1691,15 @@
             Rank of receiving process
         axis: int
             The axis along which ``sendbuf`` is packed
         recv_axis: int
             The axis along which ``recvbuf`` is packed
         """
         return MPIRequest(
-            *self.__scatter_like(
+            *self.__gather_like(
                 self.handle.Igather,
                 sendbuf,
                 recvbuf,
                 axis,
                 recv_axis,
                 root=root,
                 recv_factor=self.size,
@@ -1708,27 +1729,123 @@
             Rank of receiving process
         axis: int
             The axis along which ``sendbuf`` is packed
         recv_axis: int
             The axis along which ``recvbuf`` is packed
         """
         return MPIRequest(
-            *self.__scatter_like(
+            *self.__gather_like(
                 self.handle.Igatherv,
                 sendbuf,
                 recvbuf,
                 axis,
                 recv_axis,
                 root=root,
                 recv_factor=self.size,
             )
         )
 
     Igatherv.__doc__ = MPI.Comm.Igatherv.__doc__
 
+    def __scatter_like(
+        self,
+        func: Callable,
+        sendbuf: Union[DNDarray, torch.Tensor, Any],
+        recvbuf: Union[DNDarray, torch.Tensor, Any],
+        send_axis: int,
+        recv_axis: int,
+        send_factor: int = 1,
+        recv_factor: int = 1,
+        **kwargs,
+    ):
+        """
+        Generic function for scatter operations.
+
+        Parameters
+        ----------
+        func: Callable
+            Type of MPI Scatter/Gather function
+        sendbuf: Union[DNDarray, torch.Tensor, Any]
+            Buffer address of the send message
+        recvbuf: Union[DNDarray, torch.Tensor, Any]
+            Buffer address where to store the result
+        send_axis: int
+            The axis along which ``sendbuf`` is packed
+        recv_axis: int
+            The axis along which ``recvbuf`` is packed
+        send_factor: int
+            Number of elements to be scattered (vor non-v-calls)
+        recv_factor: int
+            Number of elements to be gathered (vor non-v-calls)
+        """
+        sbuf, rbuf, recv_axis_permutation = None, None, None
+
+        # align the output buffer in the same way as the input buffer by default
+        if recv_axis is None:
+            recv_axis = send_axis
+
+        # dummy allocation for *v calls
+        send_counts, send_displs, recv_counts, recv_displs = None, None, None, None
+
+        # unpack the send buffer
+        if isinstance(sendbuf, tuple):
+            sendbuf, send_counts, send_displs = sendbuf
+        if isinstance(sendbuf, DNDarray):
+            sendbuf = sendbuf.larray
+        if not isinstance(sendbuf, torch.Tensor) and send_axis != 0:
+            raise TypeError(f"sendbuf of type {type(sendbuf)} does not support send_axis != 0")
+
+        # unpack the receive buffer
+        # if isinstance(recvbuf, tuple):
+        #     recvbuf, recv_counts, recv_displs = recvbuf
+        if isinstance(recvbuf, DNDarray):
+            recvbuf = recvbuf.larray
+        if not isinstance(recvbuf, torch.Tensor) and recv_axis != 0:
+            raise TypeError(f"recvbuf of type {type(recvbuf)} does not support recv_axis != 0")
+
+        # keep a reference to the original buffer object
+        original_recvbuf = recvbuf
+
+        # permute the send_axis order so that the split send_axis is the first to be transmitted
+        if self.rank == kwargs.get("root"):
+            send_axis_permutation = list(range(sendbuf.ndimension()))
+            send_axis_permutation[0], send_axis_permutation[send_axis] = send_axis, 0
+            sendbuf = sendbuf.permute(*send_axis_permutation)
+
+        recv_axis_permutation = list(range(recvbuf.ndimension()))
+        recv_axis_permutation[0], recv_axis_permutation[recv_axis] = recv_axis, 0
+        recvbuf = recvbuf.permute(*recv_axis_permutation)
+
+        # prepare buffer objects
+        sbuf = sendbuf if CUDA_AWARE_MPI or not isinstance(sendbuf, torch.Tensor) else sendbuf.cpu()
+        rbuf = recvbuf if CUDA_AWARE_MPI or not isinstance(recvbuf, torch.Tensor) else recvbuf.cpu()
+
+        if sendbuf is not MPI.IN_PLACE:
+            mpi_sendbuf = self.as_buffer(sbuf, send_counts, send_displs)
+            if send_counts is None:
+                mpi_sendbuf[1] //= send_factor
+        else:
+            mpi_sendbuf = sbuf
+        if recvbuf is not MPI.IN_PLACE:
+            mpi_recvbuf = self.as_buffer(rbuf, recv_counts, recv_displs)
+            if recv_counts is None:
+                mpi_recvbuf[1] //= recv_factor
+        else:
+            mpi_recvbuf = rbuf
+
+        # perform the scatter operation
+        exit_code = func(mpi_sendbuf, mpi_recvbuf, **kwargs)
+
+        # undo the recvbuf permutation and assign the temporary buffer to the original recvbuf
+        # if recv_axis != 0:
+        #    recvbuf = recvbuf.permute(*recv_axis_permutation)
+        #    original_recvbuf.set_(recvbuf.untyped_storage(), recvbuf.storage_offset(), recvbuf.shape, recvbuf.stride())
+
+        return exit_code, sbuf, rbuf, original_recvbuf, recv_axis_permutation
+
     def Iscatter(
         self,
         sendbuf: Union[DNDarray, torch.Tensor, Any],
         recvbuf: Union[DNDarray, torch.Tensor, Any],
         root: int = 0,
         axis: int = 0,
         recv_axis: int = None,
@@ -1824,17 +1941,17 @@
             The axis along which ``sendbuf`` is packed
         recv_axis: int
             The axis along which ``recvbuf`` is packed
         """
         ret, sbuf, rbuf, buf, permutation = self.__scatter_like(
             self.handle.Scatter, sendbuf, recvbuf, axis, recv_axis, root=root, send_factor=self.size
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Scatter.__doc__ = MPI.Comm.Scatter.__doc__
 
     def Scatterv(
         self,
@@ -1865,17 +1982,17 @@
             sendbuf,
             recvbuf,
             axis,
             recv_axis,
             root=root,
             send_factor=self.size,
         )
-        if buf is not None and isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
-            if permutation is not None:
-                rbuf = rbuf.permute(permutation)
+        if buf is not None and isinstance(buf, torch.Tensor) and permutation is not None:
+            rbuf = rbuf.permute(permutation)
+        if isinstance(buf, torch.Tensor) and buf.is_cuda and not CUDA_AWARE_MPI:
             buf.copy_(rbuf)
         return ret
 
     Scatterv.__doc__ = MPI.Comm.Scatterv.__doc__
 
     def __getattr__(self, name: str):
         """
```

### Comparing `heat-1.3.1/heat/core/complex_math.py` & `heat-1.4.0/heat/core/complex_math.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/constants.py` & `heat-1.4.0/heat/core/constants.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/devices.py` & `heat-1.4.0/heat/core/devices.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/dndarray.py` & `heat-1.4.0/heat/core/dndarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides HeAT's core data structure, the DNDarray, a distributed n-dimensional array"""
+
 from __future__ import annotations
 
 import math
 import numpy as np
 import torch
 import warnings
 
@@ -336,15 +337,18 @@
 
     @property
     def strides(self) -> Tuple[int]:
         """
         Returns bytes to step in each dimension when traversing a ``DNDarray``. numpy-like usage: ``self.strides()``
         """
         steps = list(self.larray.stride())
-        itemsize = self.larray.storage().element_size()
+        try:
+            itemsize = self.larray.untyped_storage().element_size()
+        except AttributeError:
+            itemsize = self.larray.storage().element_size()
         strides = tuple(step * itemsize for step in steps)
         return strides
 
     @property
     def T(self):
         """
         Reverse the dimensions of a DNDarray.
@@ -562,14 +566,61 @@
             is_empty = np.prod(self.__array.shape) == 0
             root = self.comm.allreduce(0 if is_empty else self.comm.rank, op=MPI.SUM)
 
             return self.comm.bcast(None if is_empty else cast_function(self.__array), root=root)
 
         raise TypeError("only size-1 arrays can be converted to Python scalars")
 
+    def collect_(self, target_rank: Optional[int] = 0) -> None:
+        """
+        A method collecting a distributed DNDarray to one MPI rank, chosen by the `target_rank` variable.
+        It is a specific case of the ``redistribute_`` method.
+
+        Parameters
+        ----------
+        target_rank : int, optional
+            The rank to which the DNDarray will be collected. Default: 0.
+
+        Raises
+        ------
+        TypeError
+            If the target rank is not an integer.
+        ValueError
+            If the target rank is out of bounds.
+
+        Examples
+        --------
+        >>> st = ht.ones((50, 81, 67), split=2)
+        >>> print(st.lshape)
+        [0/2] (50, 81, 23)
+        [1/2] (50, 81, 22)
+        [2/2] (50, 81, 22)
+        >>> st.collect_()
+        >>> print(st.lshape)
+        [0/2] (50, 81, 67)
+        [1/2] (50, 81, 0)
+        [2/2] (50, 81, 0)
+        >>> st.collect_(1)
+        >>> print(st.lshape)
+        [0/2] (50, 81, 0)
+        [1/2] (50, 81, 67)
+        [2/2] (50, 81, 0)
+        """
+        if not isinstance(target_rank, int):
+            raise TypeError(f"target rank must be of type int , but was {type(target_rank)}")
+        if target_rank >= self.comm.size:
+            raise ValueError("target rank is out of bounds")
+        if not self.is_distributed():
+            return
+
+        target_map = self.lshape_map.clone()
+        target_map[:, self.split] = 0
+        target_map[target_rank, self.split] = self.gshape[self.split]
+        self.redistribute_(target_map=target_map)
+
     def __complex__(self) -> DNDarray:
         """
         Complex scalar casting.
         """
         return self.__cast(complex)
 
     def counts_displs(self) -> Tuple[Tuple[int], Tuple[int]]:
```

### Comparing `heat-1.3.1/heat/core/exponential.py` & `heat-1.4.0/heat/core/exponential.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/factories.py` & `heat-1.4.0/heat/core/factories.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 
 from typing import Callable, Iterable, Optional, Sequence, Tuple, Type, Union, List
 
 from .communication import MPI, sanitize_comm, Communication
 from .devices import Device
 from .dndarray import DNDarray
-from .memory import sanitize_memory_layout
+from .memory import sanitize_memory_layout, copy as memory_copy
 from .sanitation import sanitize_in, sanitize_sequence
 from .stride_tricks import sanitize_axis, sanitize_shape
 from .types import datatype
 
 from . import devices
 from . import types
 
@@ -233,29 +233,29 @@
     (24, 8)
     >>> b = ht.array(a)
     >>> b
     DNDarray([[0, 1, 2],
               [3, 4, 5]], dtype=ht.int64, device=cpu:0, split=None)
     >>> b.strides
     (24, 8)
-    >>> b.larray.storage()
+    >>> b.larray.untyped_storage()
      0
      1
      2
      3
      4
      5
     [torch.LongStorage of size 6]
     >>> c = ht.array(a, order='F')
     >>> c
     DNDarray([[0, 1, 2],
               [3, 4, 5]], dtype=ht.int64, device=cpu:0, split=None)
     >>> c.strides
     (8, 16)
-    >>> c.larray.storage()
+    >>> c.larray.untyped_storage()
      0
      3
      1
      4
      2
      5
     [torch.LongStorage of size 6]
@@ -267,15 +267,15 @@
     DNDarray([[ 0,  1,  2],
               [ 3,  4,  5],
               [ 6,  7,  8],
               [ 9, 10, 11]], dtype=ht.int64, device=cpu:0, split=0)
     >>> b.strides
     [0/2] (8, 16)
     [1/2] (8, 16)
-    >>> b.larray.storage()
+    >>> b.larray.untyped_storage()
     [0/2] 0
           3
           1
           4
           2
           5
          [torch.LongStorage of size 6]
@@ -283,85 +283,109 @@
           9
           7
           10
           8
           11
          [torch.LongStorage of size 6]
     """
-    # array already exists; no copy
-    if isinstance(obj, DNDarray):
-        if not copy:
-            if (
-                (dtype is None or dtype == obj.dtype)
-                and (split is None or split == obj.split)
-                and (is_split is None or is_split == obj.split)
-                and (device is None or device == obj.device)
-            ):
-                return obj
-        # extract the internal tensor
-        obj = obj.larray
-
     # sanitize the data type
     if dtype is not None:
         dtype = types.canonical_heat_type(dtype)
 
     # sanitize device
     if device is not None:
         device = devices.sanitize_device(device)
 
+    if split is not None and is_split is not None:
+        raise ValueError("split and is_split are mutually exclusive parameters")
+
+    # array already exists; no copy
+    if isinstance(obj, DNDarray):
+        if (
+            (dtype is None or dtype == obj.dtype)
+            and (split is None or split == obj.split)
+            and (is_split is None or is_split == obj.split)
+            and (device is None or device == obj.device)
+        ):
+            if copy is True:
+                return memory_copy(obj)
+            else:
+                return obj
+        elif split is not None and obj.split is not None and split != obj.split:
+            raise ValueError(
+                f"'split' argument does not match existing 'split' dimention ({split} != {obj.split}).\nIf you are trying to create a new DNDarray with a new split from an existing DNDarray, use the function `ht.resplit()` instead."
+            )
+        elif is_split is not None and obj.split is not None and is_split != obj.split:
+            raise ValueError(
+                f"'is_split' and the split axis of the object do not match ({is_split} != {obj.split}).\nIf you are trying to resplit an existing DNDarray in-place, use the method `DNDarray.resplit_()` instead."
+            )
+        elif device is not None and device != obj.device and copy is False:
+
+            raise ValueError(
+                "argument `copy` is set to False, but copy of input object is necessary as the array is being copied across devices.\nUse the method `DNDarray.cpu()` or  `DNDarray.gpu()` to move the array to the desired device."
+            )
+
+        # extract the internal tensor
+        obj = obj.larray
+
     # initialize the array
     if bool(copy):
         if isinstance(obj, torch.Tensor):
             # TODO: watch out. At the moment clone() implies losing the underlying memory layout.
             # pytorch fix in progress
             obj = obj.clone().detach()
         else:
             try:
                 obj = torch.tensor(
                     obj,
-                    device=device.torch_device
-                    if device is not None
-                    else devices.get_device().torch_device,
+                    device=(
+                        device.torch_device
+                        if device is not None
+                        else devices.get_device().torch_device
+                    ),
                 )
             except RuntimeError:
-                raise TypeError("invalid data of type {}".format(type(obj)))
+                raise TypeError(f"invalid data of type {type(obj)}")
     else:
         if copy is False and not np.isscalar(obj) and not isinstance(obj, (Tuple, List)):
             # Python array-API compliance, cf. https://data-apis.org/array-api/2022.12/API_specification/generated/array_api.asarray.html
             if not (
                 (dtype is None or dtype == types.canonical_heat_type(obj.dtype))
                 and (
                     device is None
-                    or device.torch_device
-                    == str(getattr(obj, "device", devices.get_device().torch_device))
+                    or device.torch_device.split(":")[0]
+                    == str(getattr(obj, "device", devices.get_device().torch_device)).split(":")[0]
                 )
             ):
                 raise ValueError(
                     "argument `copy` is set to False, but copy of input object is necessary. \n Set copy=None to reuse the memory buffer whenever possible and allow for copies otherwise."
                 )
         try:
-            obj = torch.as_tensor(
-                obj,
-                device=device.torch_device
-                if device is not None
-                else devices.get_device().torch_device,
-            )
+            if not isinstance(obj, torch.Tensor):
+                obj = torch.as_tensor(
+                    obj,
+                    device=(
+                        device.torch_device
+                        if device is not None
+                        else devices.get_device().torch_device
+                    ),
+                )
         except RuntimeError:
-            raise TypeError("invalid data of type {}".format(type(obj)))
+            raise TypeError(f"invalid data of type {type(obj)}")
 
     # infer dtype from obj if not explicitly given
     if dtype is None:
         dtype = types.canonical_heat_type(obj.dtype)
     else:
         torch_dtype = dtype.torch_type()
         if obj.dtype != torch_dtype:
             obj = obj.type(torch_dtype)
 
     # infer device from obj if not explicitly given
-    if device is None:
+    if device is None and hasattr(obj, "device"):
         device = devices.sanitize_device(obj.device.type)
 
     if str(obj.device) != device.torch_device:
         warnings.warn(
             f"Array 'obj' is not on device '{device}'. It will be moved to it.",
             UserWarning,
         )
@@ -377,16 +401,14 @@
         obj = obj.reshape(obj.shape + ndmin_abs * (1,))
     if ndmin_abs > 0 > ndmin:
         obj = obj.reshape(ndmin_abs * (1,) + obj.shape)
 
     # sanitize the split axes, ensure mutual exclusiveness
     split = sanitize_axis(obj.shape, split)
     is_split = sanitize_axis(obj.shape, is_split)
-    if split is not None and is_split is not None:
-        raise ValueError("split and is_split are mutually exclusive parameters")
 
     # sanitize comm object
     comm = sanitize_comm(comm)
 
     # determine the local and the global shape. If split is None, they are identical
     gshape = list(obj.shape)
     lshape = gshape.copy()
@@ -396,15 +418,15 @@
     if comm.size == 1 or split is None and is_split is None:
         obj = sanitize_memory_layout(obj, order=order)
         split = is_split if is_split is not None else split
 
     elif split is not None:
         # only keep local slice
         _, _, slices = comm.chunk(gshape, split)
-        _ = obj[slices].clone()
+        _ = obj[slices].contiguous()
         del obj
 
         obj = sanitize_memory_layout(_, order=order)
 
     # check with the neighboring rank whether the local shape would fit into a global shape
     elif is_split is not None:
         obj = sanitize_memory_layout(obj, order=order)
```

### Comparing `heat-1.3.1/heat/core/indexing.py` & `heat-1.4.0/heat/core/indexing.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/io.py` & `heat-1.4.0/heat/core/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Enables parallel I/O with data on disk."""
+
 from __future__ import annotations
 
 import os.path
 from math import log10
 import numpy as np
 import torch
 import warnings
@@ -30,15 +31,15 @@
 
 try:
     import h5py
 except ImportError:
     # HDF5 support is optional
     def supports_hdf5() -> bool:
         """
-        Returns ``True`` if HeAT supports reading from and writing to HDF5 files, ``False`` otherwise.
+        Returns ``True`` if Heat supports reading from and writing to HDF5 files, ``False`` otherwise.
         """
         return False
 
 else:
     # add functions to exports
     __all__.extend(["load_hdf5", "save_hdf5"])
 
@@ -46,22 +47,23 @@
     if not h5py.get_config().mpi and MPI_WORLD.rank == 0:
         warnings.warn(
             "h5py does not support parallel I/O, falling back to slower serial I/O", ImportWarning
         )
 
     def supports_hdf5() -> bool:
         """
-        Returns ``True`` if HeAT supports reading from and writing to HDF5 files, ``False`` otherwise.
+        Returns ``True`` if Heat supports reading from and writing to HDF5 files, ``False`` otherwise.
         """
         return True
 
     def load_hdf5(
         path: str,
         dataset: str,
         dtype: datatype = types.float32,
+        load_fraction: float = 1.0,
         split: Optional[int] = None,
         device: Optional[str] = None,
         comm: Optional[Communication] = None,
     ) -> DNDarray:
         """
         Loads data from an HDF5 file. The data may be distributed among multiple processing nodes via the split flag.
 
@@ -69,14 +71,18 @@
         ----------
         path : str
             Path to the HDF5 file to be read.
         dataset : str
             Name of the dataset to be read.
         dtype : datatype, optional
             Data type of the resulting array.
+        load_fraction : float between 0. (excluded) and 1. (included), default is 1.
+            if 1. (default), the whole dataset is loaded from the file specified in path
+            else, the dataset is loaded partially, with the fraction of the dataset (along the split axis) specified by load_fraction
+            If split is None, load_fraction is automatically set to 1., i.e. the whole dataset is loaded.
         split : int or None, optional
             The axis along which the data is distributed among the processing cores.
         device : str, optional
             The device id on which to place the data, defaults to globally set default device.
         comm : Communication, optional
             The communication to use for the data distribution.
 
@@ -101,28 +107,40 @@
         >>> b.lshape
         [0/2] (3,)
         [1/2] (2,)
         """
         if not isinstance(path, str):
             raise TypeError(f"path must be str, not {type(path)}")
         elif not isinstance(dataset, str):
-            raise TypeError("dataset must be str, not {}".format(type(dataset)))
+            raise TypeError(f"dataset must be str, not {type(dataset)}")
         elif split is not None and not isinstance(split, int):
             raise TypeError(f"split must be None or int, not {type(split)}")
 
+        if not isinstance(load_fraction, float):
+            raise TypeError(f"load_fraction must be float, but is {type(load_fraction)}")
+        else:
+            if split is not None and (load_fraction <= 0.0 or load_fraction > 1.0):
+                raise ValueError(
+                    f"load_fraction must be between 0. (excluded) and 1. (included), but is {load_fraction}."
+                )
+
         # infer the type and communicator for the loaded array
         dtype = types.canonical_heat_type(dtype)
         # determine the comm and device the data will be placed on
         device = devices.sanitize_device(device)
         comm = sanitize_comm(comm)
 
         # actually load the data from the HDF5 file
         with h5py.File(path, "r") as handle:
             data = handle[dataset]
-            gshape = tuple(data.shape)
+            gshape = data.shape
+            if split is not None:
+                gshape = np.array(gshape)
+                gshape[split] = int(gshape[split] * load_fraction)
+                gshape = tuple(gshape)
             dims = len(gshape)
             split = sanitize_axis(gshape, split)
             _, _, indices = comm.chunk(gshape, split)
             balanced = True
             if split is None:
                 data = torch.tensor(
                     data[indices], dtype=dtype.torch_type(), device=device.torch_device
@@ -231,15 +249,15 @@
 
 try:
     import netCDF4 as nc
 except ImportError:
     # netCDF4 support is optional
     def supports_netcdf() -> bool:
         """
-        Returns ``True`` if HeAT supports reading from and writing to netCDF4 files, ``False`` otherwise.
+        Returns ``True`` if Heat supports reading from and writing to netCDF4 files, ``False`` otherwise.
         """
         return False
 
 else:
     # add functions to visible exports
     __all__.extend(["load_netcdf", "save_netcdf"])
 
@@ -255,15 +273,15 @@
         warnings.warn(
             "netCDF4 does not support parallel I/O, falling back to slower serial I/O",
             ImportWarning,
         )
 
     def supports_netcdf() -> bool:
         """
-        Returns ``True`` if HeAT supports reading from and writing to netCDF4 files, ``False`` otherwise.
+        Returns ``True`` if Heat supports reading from and writing to netCDF4 files, ``False`` otherwise.
         """
         return True
 
     def load_netcdf(
         path: str,
         variable: str,
         dtype: datatype = types.float32,
@@ -389,19 +407,19 @@
 
         Examples
         --------
         >>> x = ht.arange(100, split=0)
         >>> ht.save_netcdf(x, 'data.nc', dataset='DATA')
         """
         if not isinstance(data, DNDarray):
-            raise TypeError("data must be heat tensor, not {}".format(type(data)))
+            raise TypeError(f"data must be heat tensor, not {type(data)}")
         if not isinstance(path, str):
-            raise TypeError("path must be str, not {}".format(type(path)))
+            raise TypeError(f"path must be str, not {type(path)}")
         if not isinstance(variable, str):
-            raise TypeError("variable must be str, not {}".format(type(path)))
+            raise TypeError(f"variable must be str, not {type(path)}")
         if dimension_names is None:
             dimension_names = [
                 __NETCDF_DIM_TEMPLATE.format(variable, dim) for dim, _ in enumerate(data.shape)
             ]
         elif isinstance(dimension_names, str):
             dimension_names = [dimension_names]
         elif isinstance(dimension_names, tuple):
@@ -409,23 +427,19 @@
         elif not isinstance(dimension_names, list):
             raise TypeError(
                 "dimension_names must be list or tuple or string, not{}".format(
                     type(dimension_names)
                 )
             )
         elif not len(dimension_names) == len(data.shape):
-            raise ValueError(
-                "{0} names given for {1} dimensions".format(len(dimension_names), len(data.shape))
-            )
+            raise ValueError(f"{len(dimension_names)} names given for {len(data.shape)} dimensions")
 
         # we only support a subset of possible modes
         if mode not in __VALID_WRITE_MODES:
-            raise ValueError(
-                "mode was {}, not in possible modes {}".format(mode, __VALID_WRITE_MODES)
-            )
+            raise ValueError(f"mode was {mode}, not in possible modes {__VALID_WRITE_MODES}")
 
         failed = 0
         excep = None
         # chunk the data, if no split is set maximize parallel I/O and chunk first axis
         is_split = data.split is not None
         _, _, slices = data.comm.chunk(data.gshape, data.split if is_split else 0)
 
@@ -447,31 +461,29 @@
 
             Raises
             -------
             ValueError
                 If resulting shapes do not match.
             """
             if np.prod(shape) != np.prod(expanded_shape):
-                raise ValueError(
-                    "Shapes %s and %s do not have the same size" % (shape, expanded_shape)
-                )
+                raise ValueError(f"Shapes {shape} and {expanded_shape} do not have the same size")
             if np.prod(shape) == 1:  # size 1 array
                 return split
             if len(shape) == len(expanded_shape):  # actually not expanded at all
                 return split
             if split is None:  # not split at all
                 return None
             # Get indices of non-empty dimensions and squeezed shapes
             enumerated = [[i, v] for i, v in enumerate(shape) if v != 1]
             ind_nonempty, sq_shape = list(zip(*enumerated))  # transpose
             enumerated = [[i, v] for i, v in enumerate(expanded_shape) if v != 1]
             ex_ind_nonempty, sq_ex = list(zip(*enumerated))  # transpose
             if not sq_shape == sq_ex:
                 raise ValueError(
-                    "Shapes %s and %s differ in non-empty dimensions" % (shape, expanded_shape)
+                    f"Shapes {shape} and {expanded_shape} differ in non-empty dimensions"
                 )
             if split in ind_nonempty:  # split along non-empty dimension
                 split_sq = ind_nonempty.index(split)  # split-axis in squeezed shape
                 return ex_ind_nonempty[split_sq]
             # split along empty dimension: split doesnt matter, only one process contains data
             # return the last empty dimension (in expanded shape) before (the first nonempty dimension after split)
             # number of nonempty elems before split
@@ -643,15 +655,15 @@
 
         failed = data.comm.allreduce(failed, op=MPI.MAX)
         if failed - 1 == data.comm.rank:
             data.comm.bcast(excep, root=failed - 1)
             raise excep
         elif failed:
             excep = data.comm.bcast(excep, root=failed - 1)
-            excep.args = "raised by process rank {}".format(failed - 1), *excep.args
+            excep.args = f"raised by process rank {failed - 1}", *excep.args
             raise excep from None  # raise the same error but without traceback
             # because that is on a different process
 
     DNDarray.save_netcdf = lambda self, path, variable, mode="w", **kwargs: save_netcdf(
         self, path, variable, mode, **kwargs
     )
     DNDarray.save_netcdf.__doc__ = save_netcdf.__doc__
@@ -889,16 +901,29 @@
                     sep_values = [float(val) for val in line.split(sep)]
                     local_tensor[actual_length] = torch.tensor(sep_values, dtype=dtype.torch_type())
                     actual_length += 1
 
         # In case there are some empty lines in the csv file
         local_tensor = local_tensor[:actual_length]
 
-        resulting_tensor = factories.array(
-            local_tensor, dtype=dtype, is_split=0, device=device, comm=comm
+        total_actual_lines = torch.tensor(
+            actual_length, dtype=torch.int64, device=local_tensor.device
+        )
+        comm.Allreduce(MPI.IN_PLACE, total_actual_lines, MPI.SUM)
+
+        gshape = (total_actual_lines.item(), columns[0].item())
+
+        resulting_tensor = DNDarray(
+            local_tensor,
+            gshape=gshape,
+            dtype=dtype,
+            split=0,
+            device=device,
+            comm=comm,
+            balanced=None,
         )
         resulting_tensor.balance_()
 
     elif split == 1:
         data = []
 
         with open(path) as f:
```

### Comparing `heat-1.3.1/heat/core/linalg/basics.py` & `heat-1.4.0/heat/core/linalg/basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Basic linear algebra operations on distributed ``DNDarray``
 """
+
 import itertools
 import numpy as np
 import torch
 import warnings
 
 from typing import List, Callable, Union, Optional, Tuple
 
@@ -480,14 +481,17 @@
                   [26.,  9., 10., 11.]])
     [1/1] tensor([[11., 12., 13.],
                   [ 9., 10., 11.],
                   [10., 11., 12.],
                   [11., 12., 13.],
                   [12., 13., 14.]])
     """
+    sanitation.sanitize_in(a)
+    sanitation.sanitize_in(b)
+
     if a.gshape[-1] != b.gshape[0]:
         raise ValueError(
             f"If the last dimension of a ({a.gshape[-1]}) is not the same size as the second-to-last dimension of b. ({b.gshape[-2]})"
         )
 
     # determine if a larger type is needed for c
     c_type = types.promote_types(a.dtype, b.dtype)
@@ -1090,15 +1094,25 @@
             res = res.squeeze()
         c = factories.array(res, split=split, device=a.device, comm=a.comm)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
         return c
 
 
-DNDarray.__matmul__ = lambda self, other: matmul(self, other)
+def _matmul(self, other):
+    try:
+        return matmul(self, other)
+    except TypeError:
+        return NotImplemented
+
+
+DNDarray.__matmul__ = _matmul
+DNDarray.__matmul__.__doc__ = matmul.__doc__
+DNDarray.__rmatmul__ = lambda self, other: _matmul(other, self)
+DNDarray.__rmatmul__.__doc__ = matmul.__doc__
 
 
 def matrix_norm(
     x: DNDarray,
     axis: Optional[Tuple[int, int]] = None,
     keepdims: bool = False,
     ord: Optional[Union[int, str]] = None,
```

### Comparing `heat-1.3.1/heat/core/linalg/solver.py` & `heat-1.4.0/heat/core/linalg/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Collection of solvers for systems of linear equations.
 """
+
 import heat as ht
 from ..dndarray import DNDarray
 from ..sanitation import sanitize_out
 from typing import List, Dict, Any, TypeVar, Union, Tuple, Optional
+from .. import factories
 
 import torch
 
 __all__ = ["cg", "lanczos"]
 
 
 def cg(A: DNDarray, b: DNDarray, x0: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
```

### Comparing `heat-1.3.1/heat/core/linalg/svd.py` & `heat-1.4.0/heat/core/linalg/svd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 file for future "full" SVD implementation
 """
+
 from typing import Tuple
 from ..dndarray import DNDarray
 
 __all__ = ["svd"]
 
 
 def svd(A: DNDarray) -> Tuple[DNDarray, DNDarray, DNDarray]:
```

### Comparing `heat-1.3.1/heat/core/linalg/svdtools.py` & `heat-1.4.0/heat/core/linalg/svdtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 distributed hierarchical SVD
 """
+
 import numpy as np
 import collections
 import torch
 from typing import Type, Callable, Dict, Any, TypeVar, Union, Tuple, Optional
 
 from ..communication import MPICommunication
 from ..dndarray import DNDarray
@@ -81,15 +82,15 @@
     :func:`hsvd_rtol`
         References
         -------
         [1] Iwen, Ong. A distributed and incremental SVD algorithm for agglomerative data analysis on large networks. SIAM J. Matrix Anal. Appl., 37(4), 2016.
         [2] Himpe, Leibner, Rave. Hierarchical approximate proper orthogonal decomposition. SIAM J. Sci. Comput., 40 (5), 2018.
     """
     if not isinstance(A, DNDarray):
-        raise TypeError("Argument needs to be a DNDarray but is {}.".format(type(A)))
+        raise TypeError(f"Argument needs to be a DNDarray but is {type(A)}.")
     if not A.ndim == 2:
         raise ValueError("A needs to be a 2D matrix")
     if not A.dtype == types.float32 and not A.dtype == types.float64:
         raise TypeError(
             "Argument needs to be a DNDarray with datatype float32 or float64, but data type is {}.".format(
                 A.dtype
             )
@@ -193,15 +194,15 @@
     :func:`hsvd_rank`
         References
         -------
         [1] Iwen, Ong. A distributed and incremental SVD algorithm for agglomerative data analysis on large networks. SIAM J. Matrix Anal. Appl., 37(4), 2016.
         [2] Himpe, Leibner, Rave. Hierarchical approximate proper orthogonal decomposition. SIAM J. Sci. Comput., 40 (5), 2018.
     """
     if not isinstance(A, DNDarray):
-        raise TypeError("Argument needs to be a DNDarray but is {}.".format(type(A)))
+        raise TypeError(f"Argument needs to be a DNDarray but is {type(A)}.")
     if not A.ndim == 2:
         raise ValueError("A needs to be a 2D matrix")
     if not A.dtype == types.float32 and not A.dtype == types.float64:
         raise TypeError(
             "Argument needs to be a DNDarray with datatype float32 or float64, but data type is {}.".format(
                 A.dtype
             )
```

### Comparing `heat-1.3.1/heat/core/logical.py` & `heat-1.4.0/heat/core/logical.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import torch
 
 from typing import Callable, Optional, Tuple, Union
 
 from . import factories
 from . import manipulations
+from . import sanitation
 
 from . import _operations
 from . import stride_tricks
 from . import types
 
 from .communication import MPI
 from .dndarray import DNDarray
@@ -157,18 +158,18 @@
     # If x is distributed, then y is also distributed along the same axis
     if t1.comm.is_distributed():
         t1.comm.Allreduce(MPI.IN_PLACE, _local_allclose, MPI.LAND)
 
     return bool(_local_allclose.item())
 
 
-DNDarray.allclose: Callable[
-    [DNDarray, DNDarray, float, float, bool], bool
-] = lambda self, other, rtol=1e-05, atol=1e-08, equal_nan=False: allclose(
-    self, other, rtol, atol, equal_nan
+DNDarray.allclose: Callable[[DNDarray, DNDarray, float, float, bool], bool] = (
+    lambda self, other, rtol=1e-05, atol=1e-08, equal_nan=False: allclose(
+        self, other, rtol, atol, equal_nan
+    )
 )
 DNDarray.allclose.__doc__ = all.__doc__
 
 
 def any(
     x, axis: Optional[int] = None, out: Optional[DNDarray] = None, keepdims: bool = False
 ) -> DNDarray:
@@ -215,17 +216,17 @@
         axis = tuple(range(x.ndim))
 
     return _operations.__reduce_op(
         x, local_any, MPI.LOR, axis=axis, out=out, neutral=0, keepdims=keepdims
     )
 
 
-DNDarray.any: Callable[
-    [DNDarray, Optional[int], Optional[DNDarray], bool], DNDarray
-] = lambda self, axis=None, out=None, keepdims=False: any(self, axis, out, keepdims)
+DNDarray.any: Callable[[DNDarray, Optional[int], Optional[DNDarray], bool], DNDarray] = (
+    lambda self, axis=None, out=None, keepdims=False: any(self, axis, out, keepdims)
+)
 DNDarray.any.__doc__ = any.__doc__
 
 
 def isclose(
     x: DNDarray, y: DNDarray, rtol: float = 1e-05, atol: float = 1e-08, equal_nan: bool = False
 ) -> DNDarray:
     """
@@ -372,18 +373,18 @@
     --------
     >>> ht.isnan(ht.array([1, ht.inf, -ht.inf, ht.nan]))
     DNDarray([False, True, False, False], dtype=ht.bool, device=cpu:0, split=None)
     """
     return _operations.__local_op(torch.isposinf, x, out, no_cast=True)
 
 
-DNDarray.isclose: Callable[
-    [DNDarray, DNDarray, float, float, bool], DNDarray
-] = lambda self, other, rtol=1e-05, atol=1e-08, equal_nan=False: isclose(
-    self, other, rtol, atol, equal_nan
+DNDarray.isclose: Callable[[DNDarray, DNDarray, float, float, bool], DNDarray] = (
+    lambda self, other, rtol=1e-05, atol=1e-08, equal_nan=False: isclose(
+        self, other, rtol, atol, equal_nan
+    )
 )
 DNDarray.isclose.__doc__ = isclose.__doc__
 
 
 def logical_and(x: DNDarray, y: DNDarray) -> DNDarray:
     """
     Compute the truth value of ``x`` AND ``y`` element-wise. Returns a boolean :class:`~heat.core.dndarray.DNDarray` containing the truth value of ``x`` AND ``y`` element-wise.
@@ -512,17 +513,24 @@
             x = factories.array(x, dtype=dtype, device=device)
 
         return x
 
     x = sanitize_input_type(x, y)
     y = sanitize_input_type(y, x)
 
-    # if one of the tensors is distributed, unsplit/gather it
-    if x.split is not None and y.split is None:
-        t1 = manipulations.resplit(x, axis=None)
+    # if one of the DNDarrays is distributed and the other is not
+    if x.is_distributed() and not y.is_distributed() and y.ndim > 0:
+        t2 = factories.array(y.larray, device=x.device, split=x.split)
+        x, t2 = sanitation.sanitize_distribution(x, t2, target=x)
+        return x, t2
+
+    # if y is distributed, x is not distributed, and x is not a scalar
+    elif y.is_distributed() and not x.is_distributed() and x.ndim > 0:
+        t1 = factories.array(x.larray, device=y.device, split=y.split)
+        t1, y = sanitation.sanitize_distribution(t1, y, target=y)
         return t1, y
 
     elif x.split != y.split:
         t2 = manipulations.resplit(y, axis=x.split)
         return x, t2
 
     else:
```

### Comparing `heat-1.3.1/heat/core/manipulations.py` & `heat-1.4.0/heat/core/manipulations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manipulation operations for (potentially distributed) `DNDarray`s.
 """
+
 from __future__ import annotations
 
 import numpy as np
 import torch
 import warnings
 
 from typing import Iterable, Type, List, Callable, Union, Tuple, Sequence, Optional
@@ -22,14 +23,15 @@
 from . import types
 from . import _operations
 
 __all__ = [
     "balance",
     "broadcast_arrays",
     "broadcast_to",
+    "collect",
     "column_stack",
     "concatenate",
     "diag",
     "diagonal",
     "dsplit",
     "expand_dims",
     "flatten",
@@ -240,14 +242,60 @@
         )
         broadcasted += x
         del x
 
     return broadcasted
 
 
+def collect(arr: DNDarray, target_rank: Optional[int] = 0) -> DNDarray:
+    """
+    A function collecting a distributed DNDarray to one rank, chosen by the `target_rank` variable.
+    It is a specific case of the ``redistribute_`` method.
+
+    Parameters
+    ----------
+    arr : DNDarray
+        The DNDarray to be collected.
+    target_rank : int, optional
+        The rank to which the DNDarray will be collected. Default: 0.
+
+    Raises
+    ------
+    TypeError
+        If the target rank is not an integer.
+    ValueError
+        If the target rank is out of bounds.
+
+    Examples
+    --------
+    >>> st = ht.ones((50, 81, 67), split=2)
+    >>> print(st.lshape)
+    [0/2] (50, 81, 23)
+    [1/2] (50, 81, 22)
+    [2/2] (50, 81, 22)
+    >>> collected_st = collect(st)
+    >>> print(collected_st)
+    [0/2] (50, 81, 67)
+    [1/2] (50, 81, 0)
+    [2/2] (50, 81, 0)
+    >>> collected_st = collect(collected_st, 1)
+    >>> print(st.lshape)
+    [0/2] (50, 81, 0)
+    [1/2] (50, 81, 67)
+    [2/2] (50, 81, 0)
+    """
+    arr2 = arr.copy()
+    arr2.collect_(target_rank=target_rank)
+    return arr2
+
+
+DNDarray.collect = lambda arr, target_rank=0: redistribute(arr, target_rank)
+DNDarray.collect.__doc__ = collect.__doc__
+
+
 def column_stack(arrays: Sequence[DNDarray, ...]) -> DNDarray:
     """
     Stack 1-D or 2-D `DNDarray`s as columns into a 2-D `DNDarray`.
     If the input arrays are 1-D, they will be stacked as columns. If they are 2-D,
     they will be concatenated along the second axis.
 
     Parameters
@@ -1981,15 +2029,15 @@
               [0., 0., 0.]], dtype=ht.float32, device=cpu:0, split=None)
     >>> a = ht.linspace(0, 14, 8, split=0)
     >>> ht.reshape(a, (2,4))
     (1/2) tensor([[0., 2., 4., 6.]])
     (2/2) tensor([[ 8., 10., 12., 14.]])
     """
     if not isinstance(a, DNDarray):
-        raise TypeError("'a' must be a DNDarray, currently {}".format(type(a)))
+        raise TypeError(f"'a' must be a DNDarray, currently {type(a)}")
 
     # use numpys _ShapeLike but expand to handle torch and heat Tensors
     np_proxy = np.lib.stride_tricks.as_strided(np.ones(1), a.gshape, [0] * a.ndim, writeable=False)
     try:
         np_proxy.reshape(shape)  # numpy defines their own _ShapeLike
     except TypeError as e:  # handle Tensors and DNDarrays
         try:  # make shape a np.ndarray
@@ -2959,17 +3007,17 @@
         split=split,
         device=x.device,
         comm=x.comm,
         balanced=x.balanced,
     )
 
 
-DNDarray.squeeze: Callable[
-    [DNDarray, Union[int, Tuple[int, ...]]], DNDarray
-] = lambda self, axis=None: squeeze(self, axis)
+DNDarray.squeeze: Callable[[DNDarray, Union[int, Tuple[int, ...]]], DNDarray] = (
+    lambda self, axis=None: squeeze(self, axis)
+)
 DNDarray.squeeze.__doc__ = squeeze.__doc__
 
 
 def stack(
     arrays: Sequence[DNDarray, ...], axis: int = 0, out: Optional[DNDarray] = None
 ) -> DNDarray:
     """
@@ -3353,18 +3401,18 @@
     return_value = result
     if return_inverse:
         return_value = [return_value, inverse_indices.to(a.device.torch_device)]
 
     return return_value
 
 
-DNDarray.unique: Callable[
-    [DNDarray, bool, bool, int], Tuple[DNDarray, torch.tensor]
-] = lambda self, sorted=False, return_inverse=False, axis=None: unique(
-    self, sorted, return_inverse, axis
+DNDarray.unique: Callable[[DNDarray, bool, bool, int], Tuple[DNDarray, torch.tensor]] = (
+    lambda self, sorted=False, return_inverse=False, axis=None: unique(
+        self, sorted, return_inverse, axis
+    )
 )
 DNDarray.unique.__doc__ = unique.__doc__
 
 
 def vsplit(x: DNDarray, indices_or_sections: Iterable) -> List[DNDarray, ...]:
     """
     Split array into multiple sub-DNDNarrays along the 1st axis (vertically/row-wise).
@@ -3980,15 +4028,15 @@
         if out[0].dtype != a.dtype:
             raise RuntimeError(
                 "dtypes of 'out[0]' and 'a' do not match, found {} != {}".format(
                     out[0].dtype, a.dtype
                 )
             )
         if out[1].dtype != types.int64:
-            raise RuntimeError("dtype of 'out[1]' is not ht.int64, found {}".format(out[1].dtype))
+            raise RuntimeError(f"dtype of 'out[1]' is not ht.int64, found {out[1].dtype}")
 
     dim = stride_tricks.sanitize_axis(a.gshape, dim)
 
     neutral_value = sanitation.sanitize_infinity(a)
     if largest:
         neutral_value = -neutral_value
 
@@ -4069,16 +4117,20 @@
     if out is not None:
         if out[0].shape != final_array.shape or out[1].shape != final_indices.shape:
             raise ValueError(
                 "Expecting output buffer tuple of shape ({}, {}), got ({}, {})".format(
                     gres.shape, gindices.shape, out[0].shape, out[1].shape
                 )
             )
-        out[0].larray.storage().copy_(final_array.larray.storage())
-        out[1].larray.storage().copy_(final_indices.larray.storage())
+        try:
+            out[0].larray.untyped_storage().copy_(final_array.larray.untyped_storage())
+            out[1].larray.untyped_storage().copy_(final_indices.larray.untyped_storage())
+        except AttributeError:
+            out[0].larray.storage().copy_(final_array.larray.storage())
+            out[1].larray.storage().copy_(final_indices.larray.storage())
 
         out[0]._DNDarray__dtype = a.dtype
         out[1]._DNDarray__dtype = types.int64
 
     return final_array, final_indices
```

### Comparing `heat-1.3.1/heat/core/memory.py` & `heat-1.4.0/heat/core/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,19 +70,27 @@
         del column_major, row_major
         return x
     if (order == "C" and column_major) or (order == "F" and row_major):
         dims = list(range(x.ndim))
         dims = tuple(reversed(dims))
         y = torch.empty_like(x)
         permutation = x.permute(dims).contiguous()
-        y = y.set_(
-            permutation.storage(),
-            x.storage_offset(),
-            x.shape,
-            tuple(reversed(permutation.stride())),
-        )
+        try:
+            y = y.set_(
+                permutation.untyped_storage(),
+                x.storage_offset(),
+                x.shape,
+                tuple(reversed(permutation.stride())),
+            )
+        except AttributeError:
+            y = y.set_(
+                permutation.storage(),
+                x.storage_offset(),
+                x.shape,
+                tuple(reversed(permutation.stride())),
+            )
         del permutation, dims, column_major, row_major, x
         return y
     else:
         raise ValueError(
             f"combination of order and layout not permitted, order: {order} column major: {column_major} row major: {row_major}"
         )
```

### Comparing `heat-1.3.1/heat/core/printing.py` & `heat-1.4.0/heat/core/printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,37 +234,57 @@
         for i in range(ndims):
             # skip over dimensions that are smaller than twice the number of edge items to display
             if dndarray.gshape[i] <= double_items:
                 continue
 
             # non-split dimension, can slice locally
             if i != dndarray.split:
-                start_tensor = torch.index_select(data, i, torch.arange(edgeitems + 1))
+                start_tensor = torch.index_select(
+                    data, i, torch.arange(edgeitems + 1, device=data.device)
+                )
                 end_tensor = torch.index_select(
-                    data, i, torch.arange(dndarray.lshape[i] - edgeitems, dndarray.lshape[i])
+                    data,
+                    i,
+                    torch.arange(
+                        dndarray.lshape[i] - edgeitems, dndarray.lshape[i], device=data.device
+                    ),
                 )
                 data = torch.cat([start_tensor, end_tensor], dim=i)
             # split-dimension , need to respect the global offset
             elif i == dndarray.split and dndarray.gshape[i] > double_items:
                 offset, _, _ = dndarray.comm.chunk(dndarray.gshape, i)
 
                 if offset < edgeitems + 1:
                     end = min(dndarray.lshape[i], edgeitems + 1 - offset)
-                    data = torch.index_select(data, i, torch.arange(end))
+                    data = torch.index_select(data, i, torch.arange(end, device=data.device))
                 elif dndarray.gshape[i] - edgeitems < offset - dndarray.lshape[i]:
                     global_start = dndarray.gshape[i] - edgeitems
                     data = torch.index_select(
-                        data, i, torch.arange(max(0, global_start - offset), dndarray.lshape[i])
+                        data,
+                        i,
+                        torch.arange(
+                            max(0, global_start - offset),
+                            dndarray.lshape[i],
+                            device=data.device,
+                        ),
                     )
         # exchange data
-        received = dndarray.comm.gather(data)
+        exchange_sizes = dndarray.comm.gather(torch.tensor(data.shape), root=0)
         if dndarray.comm.rank == 0:
-            # concatenate data along the split axis
-            data = torch.cat(received, dim=dndarray.split)
-
+            counts = tuple([s[dndarray.split] for s in exchange_sizes])
+            displs = (0,) + tuple(torch.cumsum(torch.tensor(counts), dim=0)[:-1])
+            recv_size = exchange_sizes[0].clone()
+            recv_size[dndarray.split] = sum(counts)
+            recv_buf = torch.empty(tuple(recv_size), dtype=data.dtype, device=data.device)
+            recv_buf = (recv_buf, counts, displs)
+        else:
+            recv_buf = torch.empty(0)
+        dndarray.comm.Gatherv(data, recv_buf, axis=dndarray.split, recv_axis=dndarray.split)
+        if dndarray.comm.rank == 0:
+            data = recv_buf[0]
     return data
 
 
 def _tensor_str(dndarray, indent: int) -> str:
     """
     Computes a string representation of the passed DNDarray.
```

### Comparing `heat-1.3.1/heat/core/random.py` & `heat-1.4.0/heat/core/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides parallel random number generators (pRNG)"""
+
 from __future__ import annotations
 
 import time
 import torch
 
 from typing import List, Optional, Tuple, Type, Union
```

### Comparing `heat-1.3.1/heat/core/relational.py` & `heat-1.4.0/heat/core/relational.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functions for relational oprations, i.e. equal/no equal...
 """
+
 from __future__ import annotations
 
 import torch
 import numpy as np
 
 from typing import Union
```

### Comparing `heat-1.3.1/heat/core/rounding.py` & `heat-1.4.0/heat/core/rounding.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     if dtype is not None:
         absolute_values.larray = absolute_values.larray.type(dtype.torch_type())
         absolute_values._DNDarray__dtype = dtype
 
     return absolute_values
 
 
-DNDarray.abs: Callable[
-    [DNDarray, Optional[DNDarray], Optional[datatype]], DNDarray
-] = lambda self, out=None, dtype=None: abs(self, out, dtype)
+DNDarray.abs: Callable[[DNDarray, Optional[DNDarray], Optional[datatype]], DNDarray] = (
+    lambda self, out=None, dtype=None: abs(self, out, dtype)
+)
 DNDarray.abs.__doc__ = abs.__doc__
 
 
 def absolute(
     x: DNDarray, out: Optional[DNDarray] = None, dtype: Optional[Type[datatype]] = None
 ) -> DNDarray:
     """
@@ -83,17 +83,17 @@
     dtype : datatype, optional
         Determines the data type of the output array. The values are cast to this type with potential loss of
         precision.
     """
     return abs(x, out, dtype)
 
 
-DNDarray.absolute: Callable[
-    [DNDarray, Optional[DNDarray], Optional[datatype]], DNDarray
-] = lambda self, out=None, dtype=None: absolute(self, out, dtype)
+DNDarray.absolute: Callable[[DNDarray, Optional[DNDarray], Optional[datatype]], DNDarray] = (
+    lambda self, out=None, dtype=None: absolute(self, out, dtype)
+)
 DNDarray.absolute.__doc__ = absolute.__doc__
 
 
 def ceil(x: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Return the ceil of the input, element-wise. Result is a :class:`~heat.core.dndarray.DNDarray` of the same shape as
     ``x``. The ceil of the scalar ``x`` is the smallest integer i, such that ``i>=x``. It is often denoted as
@@ -326,17 +326,17 @@
     if dtype is not None:
         rounded_values.larray = rounded_values.larray.type(dtype.torch_type())
         rounded_values._DNDarray__dtype = dtype
 
     return rounded_values
 
 
-DNDarray.round: Callable[
-    [DNDarray, int, Optional[DNDarray], Optional[datatype]], DNDarray
-] = lambda self, decimals=0, out=None, dtype=None: round(self, decimals, out, dtype)
+DNDarray.round: Callable[[DNDarray, int, Optional[DNDarray], Optional[datatype]], DNDarray] = (
+    lambda self, decimals=0, out=None, dtype=None: round(self, decimals, out, dtype)
+)
 DNDarray.round.__doc__ = round.__doc__
 
 
 def sgn(x: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Returns an indication of the sign of a number, element-wise. The definition for complex values is equivalent to :math:`x / |x|`.
```

### Comparing `heat-1.3.1/heat/core/sanitation.py` & `heat-1.4.0/heat/core/sanitation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Collection of validation/sanitation routines.
 """
+
 from __future__ import annotations
 
 import numpy as np
 import torch
 import warnings
 from typing import Any, Union, Sequence, List, Tuple
 
@@ -248,26 +249,26 @@
         return
     raise ValueError(
         f"Shape of local tensor along non-split axes is inconsistent with global DNDarray: tensor.shape is {tshape}, DNDarray is {gshape}"
     )
 
 
 def sanitize_out(
-    out: Any,
+    out: DNDarray,
     output_shape: Tuple,
     output_split: int,
     output_device: str,
     output_comm: Communication = None,
 ):
     """
     Validate output buffer ``out``.
 
     Parameters
     ----------
-    out : Any
+    out : DNDarray
           the `out` buffer where the result of some operation will be stored
 
     output_shape : Tuple
                    the calculated shape returned by the operation
 
     output_split : Int
                    the calculated split axis returned by the operation
@@ -284,54 +285,27 @@
         if ``out`` is not a ``DNDarray``.
     ValueError
         if shape, split direction, or device of the output buffer ``out`` do not match the operation result.
     """
     if not isinstance(out, DNDarray):
         raise TypeError(f"expected `out` to be None or a DNDarray, but was {type(out)}")
 
-    out_proxy = out.__torch_proxy__()
-    out_proxy.names = [
-        "split" if (out.split is not None and i == out.split) else f"_{i}"
-        for i in range(out_proxy.ndim)
-    ]
-    out_proxy = out_proxy.squeeze()
-
-    check_proxy = torch.ones(1).expand(output_shape)
-    check_proxy.names = [
-        "split" if (output_split is not None and i == output_split) else f"_{i}"
-        for i in range(check_proxy.ndim)
-    ]
-    check_proxy = check_proxy.squeeze()
-
-    if out_proxy.shape != check_proxy.shape:
-        raise ValueError(f"Expecting output buffer of shape {output_shape}, got {out.shape}")
-    count_split = int(out.split is not None) + int(output_split is not None)
-    if count_split == 1:
-        raise ValueError(
-            "Split axis of output buffer is inconsistent with split semantics for this operation."
-        )
-    elif count_split == 2:
-        if out.shape[out.split] > 1:  # split axis is not squeezed out
-            if out_proxy.names.index("split") != check_proxy.names.index("split"):
-                raise ValueError(
-                    "Split axis of output buffer is inconsistent with split semantics for this operation."
-                )
-        else:  # split axis is squeezed out
-            num_dim_before_split = len(
-                [name for name in out_proxy.names if int(name[1:]) < out.split]
-            )
-            check_num_dim_before_split = len(
-                [name for name in check_proxy.names if int(name[1:]) < output_split]
-            )
-            if num_dim_before_split != check_num_dim_before_split:
-                raise ValueError(
-                    "Split axis of output buffer is inconsistent with split semantics for this operation."
-                )
-    if out.device != output_device:
-        raise ValueError(f"Device mismatch: out is on {out.device}, should be on {output_device}")
+    control_values = [output_shape, output_split, output_device]
+    out_values = [out.shape, out.split, out.device]
+    # bulk-check if the two lists differ
+    if control_values != out_values:
+        # if so, check each value individually
+        if output_shape != out.shape:
+            raise ValueError(f"Expecting output buffer of shape {output_shape}, got {out.shape}")
+        if output_split != out.split:
+            raise ValueError(f"Expecting output buffer of split {output_split}, got {out.split}")
+        if output_device != out.device:
+            raise ValueError(f"Expecting output buffer on device {output_device}, got {out.device}")
+
+    # check that communicators match
     if output_comm is not None and out.comm != output_comm:
         try:
             raise NotImplementedError(
                 f"Not implemented for other comms, found {out.comm.name} and {output_comm.name}"
             )
         except Exception:
             raise NotImplementedError("Not implemented for other comms")
@@ -366,10 +340,22 @@
     Turn a scalar ``DNDarray`` into a 1-D ``DNDarray`` with 1 element.
 
     Parameters
     ----------
     x : DNDarray
         with `x.ndim = 0`
     """
-    return factories.array(
-        x.larray.unsqueeze(0), dtype=x.dtype, split=x.split, comm=x.comm, device=x.device
+    if x.ndim != 0:
+        if x.ndim == 1 and x.gnumel == 1:
+            return x
+        raise ValueError(
+            f"Input needs to be a scalar DNDarray,but was found to be {x.ndim}d DNDarray"
+        )
+    return DNDarray(
+        x.larray.unsqueeze(0),
+        gshape=(1,),
+        dtype=x.dtype,
+        split=None,
+        comm=x.comm,
+        device=x.device,
+        balanced=True,
     )
```

### Comparing `heat-1.3.1/heat/core/signal.py` & `heat-1.4.0/heat/core/signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,20 @@
                 signal_filtered = zeros(
                     gshape, dtype=a.dtype, split=a.split, device=a.device, comm=a.comm
                 )
                 start_idx = 0
 
             # accumulate relevant slice of filtered signal
             # note, this is a binary operation between unevenly distributed dndarrays and will require communication, check out _operations.__binary_op()
-            signal_filtered += global_signal_filtered[start_idx : start_idx + gshape]
+            try:
+                signal_filtered += global_signal_filtered[start_idx : start_idx + gshape]
+            except (ValueError, TypeError):
+                signal_filtered = (
+                    signal_filtered + global_signal_filtered[start_idx : start_idx + gshape]
+                )
             if r != size - 1:
                 start_idx += v.lshape_map[r + 1][0].item()
         return signal_filtered
 
     else:
         # apply torch convolution operator
         signal_filtered = fc.conv1d(signal, weight)
```

### Comparing `heat-1.3.1/heat/core/statistics.py` & `heat-1.4.0/heat/core/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Distributed statistical operations.
 """
+
 import numpy as np
 import torch
 from typing import Any, Callable, Union, Tuple, List, Optional
 
 from .communication import MPI
 from . import arithmetics
 from . import exponential
@@ -95,26 +96,26 @@
             offset, _, _ = x.comm.chunk(shape, x.split)
             indices += torch.tensor(offset, dtype=indices.dtype)
 
         return torch.cat([maxima.double(), indices.double()])
 
     # axis sanitation
     if axis is not None and not isinstance(axis, int):
-        raise TypeError("axis must be None or int, was {}".format(type(axis)))
+        raise TypeError(f"axis must be None or int, was {type(axis)}")
 
     # perform the global reduction
     smallest_value = -sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
         x, local_argmax, MPI_ARGMAX, axis=axis, out=out, neutral=smallest_value, **kwargs
     )
 
 
-DNDarray.argmax: Callable[
-    [DNDarray, int, DNDarray, object], DNDarray
-] = lambda self, axis=None, out=None, **kwargs: argmax(self, axis, out, **kwargs)
+DNDarray.argmax: Callable[[DNDarray, int, DNDarray, object], DNDarray] = (
+    lambda self, axis=None, out=None, **kwargs: argmax(self, axis, out, **kwargs)
+)
 DNDarray.argmax.__doc__ = argmax.__doc__
 
 
 def argmin(
     x: DNDarray, axis: Optional[int] = None, out: Optional[DNDarray] = None, **kwargs: object
 ) -> DNDarray:
     """
@@ -167,26 +168,26 @@
             offset, _, _ = x.comm.chunk(shape, x.split)
             indices += torch.tensor(offset, dtype=indices.dtype)
 
         return torch.cat([minimums.double(), indices.double()])
 
     # axis sanitation
     if axis is not None and not isinstance(axis, int):
-        raise TypeError("axis must be None or int, was {}".format(type(axis)))
+        raise TypeError(f"axis must be None or int, was {type(axis)}")
 
     # perform the global reduction
     largest_value = sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
         x, local_argmin, MPI_ARGMIN, axis=axis, out=out, neutral=largest_value, **kwargs
     )
 
 
-DNDarray.argmin: Callable[
-    [DNDarray, int, DNDarray, object], DNDarray
-] = lambda self, axis=None, out=None, **kwargs: argmin(self, axis, out, **kwargs)
+DNDarray.argmin: Callable[[DNDarray, int, DNDarray, object], DNDarray] = (
+    lambda self, axis=None, out=None, **kwargs: argmin(self, axis, out, **kwargs)
+)
 DNDarray.argmin.__doc__ = argmin.__doc__
 
 
 def average(
     x: DNDarray,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     weights: Optional[DNDarray] = None,
@@ -769,17 +770,17 @@
         return res.item() if res.gnumel == 1 else res
     elif isinstance(axis, (list, tuple)):
         raise TypeError(f"axis cannot be a list or a tuple, currently {type(axis)}")
     else:
         return __moment_w_axis(__torch_kurtosis, x, axis, None, unbiased, Fischer)
 
 
-DNDarray.kurtosis: Callable[
-    [DNDarray, int, bool, bool], DNDarray
-] = lambda x, axis=None, unbiased=True, Fischer=True: kurtosis(x, axis, unbiased, Fischer)
+DNDarray.kurtosis: Callable[[DNDarray, int, bool, bool], DNDarray] = (
+    lambda x, axis=None, unbiased=True, Fischer=True: kurtosis(x, axis, unbiased, Fischer)
+)
 DNDarray.kurtosis.__doc__ = average.__doc__
 
 
 def max(
     x: DNDarray,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     out: Optional[DNDarray] = None,
@@ -828,17 +829,17 @@
 
     smallest_value = -sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
         x, local_max, MPI.MAX, axis=axis, out=out, neutral=smallest_value, keepdims=keepdims
     )
 
 
-DNDarray.max: Callable[
-    [DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray
-] = lambda x, axis=None, out=None, keepdims=None: max(x, axis, out, keepdims)
+DNDarray.max: Callable[[DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray] = (
+    lambda x, axis=None, out=None, keepdims=None: max(x, axis, out, keepdims)
+)
 DNDarray.max.__doc__ = max.__doc__
 
 
 def maximum(x1: DNDarray, x2: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Compares two ``DNDarrays`` and returns a new :class:`~heat.core.dndarray.DNDarray` containing the element-wise maxima.
     The ``DNDarrays`` must have the same shape, or shapes that can be broadcast to a single shape.
@@ -1031,17 +1032,17 @@
     keepdims : bool, optional
         If True, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result can broadcast correctly against the original array ``a``.
     """
     return percentile(x, q=50, axis=axis, keepdims=keepdims)
 
 
-DNDarray.median: Callable[
-    [DNDarray, int, bool], DNDarray
-] = lambda x, axis=None, keepdims=False: median(x, axis, keepdims)
+DNDarray.median: Callable[[DNDarray, int, bool], DNDarray] = (
+    lambda x, axis=None, keepdims=False: median(x, axis, keepdims)
+)
 DNDarray.mean.__doc__ = mean.__doc__
 
 
 def __merge_moments(
     m1: torch.Tensor, m2: torch.Tensor, unbiased: bool = True
 ) -> Tuple[torch.Tensor, ...]:
     """
@@ -1160,17 +1161,17 @@
 
     largest_value = sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
         x, local_min, MPI.MIN, axis=axis, out=out, neutral=largest_value, keepdims=keepdims
     )
 
 
-DNDarray.min: Callable[
-    [DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray
-] = lambda self, axis=None, out=None, keepdims=None: min(self, axis, out, keepdims)
+DNDarray.min: Callable[[DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray] = (
+    lambda self, axis=None, out=None, keepdims=None: min(self, axis, out, keepdims)
+)
 DNDarray.min.__doc__ = min.__doc__
 
 
 def minimum(x1: DNDarray, x2: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Compares two ``DNDarrays`` and returns a new :class:`~heat.core.dndarray.DNDarray`  containing the element-wise minima.
     If one of the elements being compared is ``NaN``, then that element is returned. They must have the same shape,
@@ -1488,42 +1489,40 @@
             percentile.unsqueeze_(dim=axis + 1)
 
         return percentile
 
     # SANITATION
     # sanitize input
     if not isinstance(x, DNDarray):
-        raise TypeError("expected x to be a DNDarray, but was {}".format(type(x)))
+        raise TypeError(f"expected x to be a DNDarray, but was {type(x)}")
     if isinstance(axis, (list, tuple)):
         raise NotImplementedError("ht.percentile(), tuple axis not implemented yet")
 
     if axis is None:
         if x.ndim > 1:
             x = x.flatten()
         axis = 0
 
     gshape = x.gshape
     split = x.split
     t_x = x.larray
 
     # sanitize q
+    t_perc_dtype = torch.promote_types(t_x.dtype, torch.float32)
     if isinstance(q, (list, tuple)):
-        t_perc_dtype = torch.promote_types(type(q[0]), torch.float32)
         t_q = torch.tensor(q, dtype=t_perc_dtype, device=t_x.device)
     elif np.isscalar(q):
-        t_perc_dtype = torch.promote_types(type(q), torch.float32)
         t_q = torch.tensor([q], dtype=t_perc_dtype, device=t_x.device)
     elif isinstance(q, DNDarray):
         if x.comm.is_distributed() and q.split is not None:
             # q needs to be local
             q.resplit_(axis=None)
         t_q = q.larray
-        t_perc_dtype = torch.promote_types(t_q.dtype, torch.float32)
     else:
-        raise TypeError("DNDarray, list or tuple supported, but q was {}".format(type(q)))
+        raise TypeError(f"DNDarray, list or tuple supported, but q was {type(q)}")
 
     nperc = t_q.numel()
     perc_dtype = types.canonical_heat_type(t_perc_dtype)
 
     # q must be 1-D
     if t_q.ndim > 1:
         t_q = t_q.flatten()
@@ -1533,25 +1532,21 @@
         output_shape = (nperc,) + gshape[:axis] + (1,) + gshape[axis + 1 :]
     else:
         output_shape = (nperc,) + gshape[:axis] + gshape[axis + 1 :]
 
     # sanitize out
     if out is not None:
         if not isinstance(out, DNDarray):
-            raise TypeError("out must be DNDarray, was {}".format(type(out)))
+            raise TypeError(f"out must be DNDarray, was {type(out)}")
         if out.dtype is not perc_dtype:
-            raise TypeError(
-                "Wrong datatype for out: expected {}, got {}".format(perc_dtype, out.dtype)
-            )
+            raise TypeError(f"Wrong datatype for out: expected {perc_dtype}, got {out.dtype}")
         if out.gshape != output_shape:
-            raise ValueError("out must have shape {}, got {}".format(output_shape, out.gshape))
+            raise ValueError(f"out must have shape {output_shape}, got {out.gshape}")
         if out.split is not None:
-            raise ValueError(
-                "Split dimension mismatch for out: expected {}, got {}".format(None, out.split)
-            )
+            raise ValueError(f"Split dimension mismatch for out: expected {None}, got {out.split}")
     # END OF SANITATION
 
     # edge-case: x is a scalar. Return x
     if x.ndim == 0:
         percentile = t_x * torch.ones(nperc, dtype=t_perc_dtype, device=t_x.device)
         return DNDarray(
             percentile,
@@ -1709,17 +1704,17 @@
     elif isinstance(axis, (list, tuple)):
         raise TypeError(f"axis cannot be a list or a tuple, currently {type(axis)}")
     else:
         # if multiple axes are required, need to add a reduce_skews_elementwise function
         return __moment_w_axis(__torch_skew, x, axis, None, unbiased)
 
 
-DNDarray.skew: Callable[
-    [DNDarray, int, bool], DNDarray
-] = lambda self, axis=None, unbiased=True: skew(self, axis, unbiased)
+DNDarray.skew: Callable[[DNDarray, int, bool], DNDarray] = (
+    lambda self, axis=None, unbiased=True: skew(self, axis, unbiased)
+)
 DNDarray.skew.__doc__ = skew.__doc__
 
 
 def std(
     x: DNDarray, axis: Union[int, Tuple[int], List[int]] = None, ddof: int = 0, **kwargs: object
 ) -> DNDarray:
     """
@@ -1772,17 +1767,17 @@
         loc = np.std(x.larray.numpy(), axis=axis, ddof=ddof)
         if loc.size == 1:
             return loc.item()
         return factories.array(loc, copy=False)
     return exponential.sqrt(var(x, axis, ddof, **kwargs), out=None)
 
 
-DNDarray.std: Callable[
-    [DNDarray, Union[int, Tuple[int], List[int]], int, object], DNDarray
-] = lambda self, axis=None, ddof=0, **kwargs: std(self, axis, ddof, **kwargs)
+DNDarray.std: Callable[[DNDarray, Union[int, Tuple[int], List[int]], int, object], DNDarray] = (
+    lambda self, axis=None, ddof=0, **kwargs: std(self, axis, ddof, **kwargs)
+)
 DNDarray.std.__doc__ = std.__doc__
 
 
 def __torch_skew(
     torch_tensor: torch.Tensor, dim: int = None, unbiased: bool = False
 ) -> torch.Tensor:
     """
@@ -1988,11 +1983,11 @@
                 )
             return var_tot[0][0]
 
     else:  # axis is given
         return __moment_w_axis(torch.var, x, axis, reduce_vars_elementwise, unbiased)
 
 
-DNDarray.var: Callable[
-    [DNDarray, Union[int, Tuple[int], List[int]], int, object], DNDarray
-] = lambda self, axis=None, ddof=0, **kwargs: var(self, axis, ddof, **kwargs)
+DNDarray.var: Callable[[DNDarray, Union[int, Tuple[int], List[int]], int, object], DNDarray] = (
+    lambda self, axis=None, ddof=0, **kwargs: var(self, axis, ddof, **kwargs)
+)
 DNDarray.var.__doc__ = var.__doc__
```

### Comparing `heat-1.3.1/heat/core/stride_tricks.py` & `heat-1.4.0/heat/core/stride_tricks.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,59 @@
         raise TypeError(f"operands must be tuples of ints, not {shape_a} and {shape_b}")
     except RuntimeError:
         raise ValueError(f"operands could not be broadcast, input shapes {shape_a} {shape_b}")
 
     return tuple(resulting_shape)
 
 
+def broadcast_shapes(*shapes: Tuple[int, ...]) -> Tuple[int, ...]:
+    """
+    Infers, if possible, the broadcast output shape of multiple operands.
+
+    Parameters
+    ----------
+    *shapes : Tuple[int,...]
+        Shapes of operands.
+
+    Returns
+    -------
+    Tuple[int, ...]
+        The broadcast output shape.
+
+    Raises
+    -------
+    ValueError
+        If the shapes cannot be broadcast.
+
+    Examples
+    --------
+    >>> import heat as ht
+    >>> ht.broadcast_shapes((5,4),(4,))
+    (5, 4)
+    >>> ht.broadcast_shapes((1,100,1),(10,1,5))
+    (10, 100, 5)
+    >>> ht.broadcast_shapes((8,1,6,1),(7,1,5,))
+    (8,7,6,5))
+    >>> ht.broadcast_shapes((2,1),(8,4,3))
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+      File "heat/core/stride_tricks.py", line 100, in broadcast_shapes
+        "operands could not be broadcast, input shapes {}".format(shapes))
+    ValueError: operands could not be broadcast, input shapes ((2, 1), (8, 4, 3))
+    """
+    try:
+        resulting_shape = torch.broadcast_shapes(*shapes)
+    except TypeError:
+        raise TypeError(f"operands must be tuples of ints, not {shapes}")
+    except RuntimeError:
+        raise ValueError(f"operands could not be broadcast, input shapes {shapes}")
+
+    return tuple(resulting_shape)
+
+
 def sanitize_axis(
     shape: Tuple[int, ...], axis: Union[int, None, Tuple[int, ...]]
 ) -> Union[int, None, Tuple[int, ...]]:
     """
     Checks conformity of an axis with respect to a given shape. The axis will be converted to its positive equivalent
     and is checked to be within bounds
 
@@ -102,33 +147,38 @@
       File "<stdin>", line 1, in <module>
       File "heat/heat/core/stride_tricks.py", line 99, in sanitize_axis
         raise TypeError("axis must be None or int or tuple, but was {}".format(type(axis)))
     TypeError: axis must be None or int or tuple, but was <class 'float'>
 
     """
     # scalars are handled like unsplit matrices
-    if len(shape) == 0:
+    original_axis = axis
+    ndim = len(shape)
+
+    if ndim == 0:
         axis = None
 
     if axis is not None and not isinstance(axis, int) and not isinstance(axis, tuple):
         raise TypeError(f"axis must be None or int or tuple, but was {type(axis)}")
     if isinstance(axis, tuple):
         axis = tuple(dim + len(shape) if dim < 0 else dim for dim in axis)
         for dim in axis:
             if dim < 0 or dim >= len(shape):
-                raise ValueError(f"axis {axis} is out of bounds for shape {shape}")
+                raise ValueError(
+                    f"axis {original_axis} is out of bounds for {ndim}-dimensional array"
+                )
         return axis
 
     if axis is None or 0 <= axis < len(shape):
         return axis
     elif axis < 0:
         axis += len(shape)
 
     if axis < 0 or axis >= len(shape):
-        raise ValueError(f"axis {axis} is out of bounds for shape {shape}")
+        raise ValueError(f"axis {original_axis} is out of bounds for {ndim}-dimensional array")
 
     return axis
 
 
 def sanitize_shape(shape: Union[int, Tuple[int, ...]], lval: int = 0) -> Tuple[int, ...]:
     """
     Verifies and normalizes the given shape.
```

### Comparing `heat-1.3.1/heat/core/tiling.py` & `heat-1.4.0/heat/core/tiling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Tiling functions/classes. With these classes, you can classes you can address blocks of data in a DNDarray
 """
 
-
 from __future__ import annotations
 import itertools
 import torch
 from typing import List, Tuple, Union
 
 from .dndarray import DNDarray
```

### Comparing `heat-1.3.1/heat/core/trigonometrics.py` & `heat-1.4.0/heat/core/trigonometrics.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/core/types.py` & `heat-1.4.0/heat/core/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
         HeAT type to check
     """
     return ht_dtype in _inexact
 
 
 def heat_type_is_complexfloating(ht_dtype: Type[datatype]) -> bool:
     """
-    Check if HeAT type is a complex floading point number, i.e complex64
+    Check if HeAT type is a complex floating point number, i.e complex64
 
     Parameters
     ----------
     ht_dtype: ht.dtype
         HeAT type to check
 
     Returns
```

### Comparing `heat-1.3.1/heat/core/version.py` & `heat-1.4.0/heat/core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """This module contains Heat's version information."""
 
-
 major: int = 1
 """Indicates Heat's main version."""
-minor: int = 3
+minor: int = 4
 """Indicates feature extension."""
-micro: int = 1
+micro: int = 0
 """Indicates revisions for bugfixes."""
 extension: str = None
 """Indicates special builds, e.g. for specific hardware."""
 
 if not extension:
     __version__: str = f"{major}.{minor}.{micro}"
     """The combined version string, consisting out of major, minor, micro and possibly extension."""
```

### Comparing `heat-1.3.1/heat/datasets/diabetes.h5` & `heat-1.4.0/heat/datasets/diabetes.h5`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris.csv` & `heat-1.4.0/heat/datasets/iris.csv`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris.h5` & `heat-1.4.0/heat/datasets/iris.h5`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris.nc` & `heat-1.4.0/heat/datasets/iris.nc`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris_X_test.csv` & `heat-1.4.0/heat/datasets/iris_X_test.csv`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris_X_train.csv` & `heat-1.4.0/heat/datasets/iris_X_train.csv`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/datasets/iris_y_pred_proba.csv` & `heat-1.4.0/heat/datasets/iris_y_pred_proba.csv`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/graph/laplacian.py` & `heat-1.4.0/heat/graph/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module for graph-based classes
 """
+
 from __future__ import annotations
 
 from typing import Callable
 import torch
 import heat as ht
 from heat.core.dndarray import DNDarray
```

### Comparing `heat-1.3.1/heat/naive_bayes/gaussianNB.py` & `heat-1.4.0/heat/naive_bayes/gaussianNB.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Distributed Gaussian Naive-Bayes classifier.
 """
+
 from __future__ import annotations
 
 from typing import Tuple, Union, Optional
 import heat as ht
 from heat.core.dndarray import DNDarray
 import torch
 
@@ -386,16 +387,17 @@
         Returns a ``DNDarray`` `joint_log_likelihood(n_samples, n_classes)`.
         """
         jll_size = self.classes_.larray.numel()
         jll_shape = (x.shape[0], jll_size)
         joint_log_likelihood = ht.empty(jll_shape, dtype=x.dtype, split=x.split, device=x.device)
         for i in range(jll_size):
             jointi = ht.log(self.class_prior_[i])
-            n_ij = -0.5 * ht.sum(ht.log(2.0 * ht.pi * self.sigma_[i, :]))
-            n_ij -= 0.5 * ht.sum(((x - self.theta_[i, :]) ** 2) / (self.sigma_[i, :]), 1)
+            n_ij = -0.5 * ht.sum(ht.log(2.0 * ht.pi * self.sigma_[i, :])) - 0.5 * ht.sum(
+                ((x - self.theta_[i, :]) ** 2) / (self.sigma_[i, :]), 1
+            )
             joint_log_likelihood[:, i] = jointi + n_ij
         return joint_log_likelihood
 
     def logsumexp(
         self,
         a: DNDarray,
         axis: Optional[Union[int, Tuple[int, ...]]] = None,
```

### Comparing `heat-1.3.1/heat/nn/__init__.py` & `heat-1.4.0/heat/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/nn/data_parallel.py` & `heat-1.4.0/heat/nn/data_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file is for the general data parallel neural network classes.
 """
+
 import warnings
 import torch
 import torch.distributed
 import torch.nn as tnn
 
 from collections import OrderedDict
 from typing import Any, Callable, Dict, List, Union, Tuple
```

### Comparing `heat-1.3.1/heat/nn/functional.py` & `heat-1.4.0/heat/nn/functional.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/optim/__init__.py` & `heat-1.4.0/heat/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/optim/dp_optimizer.py` & `heat-1.4.0/heat/optim/dp_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,44 @@
 
 
 __all__ = ["DataParallelOptimizer", "DASO"]
 
 
 def __sum_f16_cb(buffer_a, buffer_b, _):
     # MPI custom sum function to use torch.half
-    tens_a = torch.HalfTensor().set_(torch.HalfStorage.from_buffer(buffer_a, "native"))
-    tens_b = torch.HalfTensor().set_(torch.HalfStorage.from_buffer(buffer_b, "native"))
+    # try/except is used to use UntypedStorages from Pytorch version >= 2.0.0 while keeping backward compatibility
+    try:
+        tens_a = torch.HalfTensor().set_(
+            torch.UntypedStorage.from_buffer(buffer_a, "native", dtype=torch.half)
+        )
+        tens_b = torch.HalfTensor().set_(
+            torch.UntypedStorage.from_buffer(buffer_b, "native", dtype=torch.half)
+        )
+    except AttributeError:
+        tens_a = torch.HalfTensor().set_(torch.HalfStorage.from_buffer(buffer_a, "native"))
+        tens_b = torch.HalfTensor().set_(torch.HalfStorage.from_buffer(buffer_b, "native"))
     tens_b += tens_a
     nelem = torch.prod(torch.tensor(tens_b.shape)).item()
     new_buff = MPI.memory.fromaddress(tens_b.data_ptr(), nbytes=tens_b.element_size() * nelem)
     buffer_b[:] = new_buff
 
 
 def __sum_bfloat_cb(buffer_a, buffer_b, _):
     # MPI custom sum function to use torch.bfloat16
-    tens_a = torch.BFloat16Tensor().set_(torch.BFloat16Storage.from_buffer(buffer_a, "native"))
-    tens_b = torch.BFloat16Tensor().set_(torch.BFloat16Storage.from_buffer(buffer_b, "native"))
+    # try/except is used to use UntypedStorages from Pytorch version >= 2.0.0 while keeping backward compatibility
+    try:
+        tens_a = torch.BFloat16Tensor().set_(
+            torch.UntypedStorage.from_buffer(buffer_a, "native", dtype=torch.bfloat16)
+        )
+        tens_b = torch.BFloat16Tensor().set_(
+            torch.UntypedStorage.from_buffer(buffer_b, "native", dtype=torch.bfloat16)
+        )
+    except AttributeError:
+        tens_a = torch.BFloat16Tensor().set_(torch.BFloat16Storage.from_buffer(buffer_a, "native"))
+        tens_b = torch.BFloat16Tensor().set_(torch.BFloat16Storage.from_buffer(buffer_b, "native"))
     tens_b += tens_a
     nelem = int(tens_b.numel())
     new_buff = MPI.memory.fromaddress(tens_b.data_ptr(), nbytes=nelem * tens_b.element_size())
     buffer_b[:] = new_buff
 
 
 # create new MPI OPs
```

### Comparing `heat-1.3.1/heat/optim/utils.py` & `heat-1.4.0/heat/optim/utils.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/regression/lasso.py` & `heat-1.4.0/heat/regression/lasso.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/sparse/_operations.py` & `heat-1.4.0/heat/sparse/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generalized operations for DCSR_matrix"""
+
 import torch
 import numpy as np
 
 from heat.sparse.dcsr_matrix import DCSR_matrix
 
 from . import factories
 from ..core.communication import MPI
```

### Comparing `heat-1.3.1/heat/sparse/arithmetics.py` & `heat-1.4.0/heat/sparse/arithmetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Arithmetic functions for Dcsr_matrices"""
+
 from __future__ import annotations
 
 import torch
 
 from .dcsr_matrix import DCSR_matrix
 
 from . import _operations
```

### Comparing `heat-1.3.1/heat/sparse/dcsr_matrix.py` & `heat-1.4.0/heat/sparse/dcsr_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides DCSR_matrix, a distributed compressed sparse row matrix"""
+
 from __future__ import annotations
 
 import torch
 from mpi4py import MPI
 from typing import Union, Tuple, TypeVar
 
 from ..core.devices import Device
```

### Comparing `heat-1.3.1/heat/sparse/factories.py` & `heat-1.4.0/heat/sparse/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
             size=obj.shape,
         )
 
     if not isinstance(obj, torch.Tensor):
         try:
             obj = torch.tensor(
                 obj,
-                device=device.torch_device
-                if device is not None
-                else devices.get_device().torch_device,
+                device=(
+                    device.torch_device if device is not None else devices.get_device().torch_device
+                ),
             )
         except RuntimeError:
             raise TypeError(f"Invalid data of type {type(obj)}")
 
     if obj.ndim != 2:
         raise ValueError(f"The number of dimensions must be 2, found {str(obj.ndim)}")
```

### Comparing `heat-1.3.1/heat/sparse/manipulations.py` & `heat-1.4.0/heat/sparse/manipulations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,60 @@
 """Manipulation operations for (potentially distributed) `DCSR_matrix`."""
+
 from __future__ import annotations
 
 from heat.sparse.dcsr_matrix import DCSR_matrix
-
+from heat.sparse.factories import sparse_csr_matrix
 from ..core.memory import sanitize_memory_layout
 from ..core.dndarray import DNDarray
 from ..core.factories import empty
 
 __all__ = [
-    "todense",
+    "to_dense",
+    "to_sparse",
 ]
 
 
-def todense(sparse_matrix: DCSR_matrix, order="C", out: DNDarray = None) -> DNDarray:
+def to_sparse(array: DNDarray) -> DCSR_matrix:
+    """
+    Convert the distributed array to a sparse DCSR_matrix representation.
+
+    Parameters
+    ----------
+    array : DNDarray
+        The distributed array to be converted to a sparse DCSR_matrix.
+
+    Returns
+    -------
+    DCSR_matrix
+        A sparse DCSR_matrix representation of the input DNDarray.
+
+    Notes
+    -----
+    This method allows for the conversion of a DNDarray into a sparse DCSR_matrix representation,
+    which is useful for handling large and sparse datasets efficiently.
+
+    Examples
+    --------
+    >>> dense_array = ht.array([[1, 0, 0], [0, 0, 2], [0, 3, 0]])
+    >>> sparse_matrix = dense_array.to_sparse()
+
+    """
+    array.balance_()
+    result = sparse_csr_matrix(
+        array.larray, dtype=array.dtype, device=array.device, comm=array.comm, is_split=array.split
+    )
+    return result
+
+
+DNDarray.to_sparse = to_sparse
+DNDarray.to_sparse.__doc__ = to_sparse.__doc__
+
+
+def to_dense(sparse_matrix: DCSR_matrix, order="C", out: DNDarray = None) -> DNDarray:
     """
     Convert :class:`~heat.sparse.DCSR_matrix` to a dense :class:`~heat.core.DNDarray`.
     Output follows the same distribution among processes as the input
 
     Parameters
     ----------
     sparse_matrix : :class:`~heat.sparse.DCSR_matrix`
@@ -71,9 +109,9 @@
             order=order,
         )
 
     out.larray = sanitize_memory_layout(sparse_matrix.larray.to_dense(), order=order)
     return out
 
 
-DCSR_matrix.todense = lambda self, order="C", out=None: todense(self, order, out)
-DCSR_matrix.to_dense = lambda self, order="C", out=None: todense(self, order, out)
+DCSR_matrix.todense = lambda self, order="C", out=None: to_dense(self, order, out)
+DCSR_matrix.to_dense = lambda self, order="C", out=None: to_dense(self, order, out)
```

### Comparing `heat-1.3.1/heat/spatial/distance.py` & `heat-1.4.0/heat/spatial/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module for (pairwise) distance functions
 """
+
 import torch
 import numpy as np
 from mpi4py import MPI
 from typing import Callable
 
 from ..core import factories
 from ..core import types
```

### Comparing `heat-1.3.1/heat/utils/data/_utils.py` & `heat-1.4.0/heat/utils/data/_utils.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/utils/data/datatools.py` & `heat-1.4.0/heat/utils/data/datatools.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/utils/data/mnist.py` & `heat-1.4.0/heat/utils/data/mnist.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/utils/data/partial_dataset.py` & `heat-1.4.0/heat/utils/data/partial_dataset.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat/utils/vision_transforms.py` & `heat-1.4.0/heat/utils/vision_transforms.py`

 * *Files identical despite different names*

### Comparing `heat-1.3.1/heat.egg-info/PKG-INFO` & `heat-1.4.0/heat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: heat
-Version: 1.3.1
+Version: 1.4.0
 Summary: A framework for high-performance data analytics and machine learning.
 Home-page: https://github.com/helmholtz-analytics/heat
 Author: Helmholtz Association
 Author-email: martin.siggel@dlr.de
 Keywords: data,analytics,tensors,distributed,gpu
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mpi4py>=3.0.0
-Requires-Dist: numpy>=1.20.0
-Requires-Dist: torch<2.0.2,>=1.8.0
-Requires-Dist: scipy>=0.14.0
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: torch<2.2.3,>=1.11.0
+Requires-Dist: scipy>=1.10.0
 Requires-Dist: pillow>=6.0.0
-Requires-Dist: torchvision>=0.8.0
+Requires-Dist: torchvision>=0.12.0
 Provides-Extra: docutils
 Requires-Dist: docutils>=0.16; extra == "docutils"
 Provides-Extra: hdf5
 Requires-Dist: h5py>=2.8.0; extra == "hdf5"
 Provides-Extra: netcdf
 Requires-Dist: netCDF4>=1.5.6; extra == "netcdf"
 Provides-Extra: dev
@@ -42,169 +43,190 @@
 
 ---
 
 Heat is a distributed tensor framework for high performance data analytics.
 
 # Project Status
 
-[![pipeline status](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
+[![CPU/CUDA/ROCm tests](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
 [![Documentation Status](https://readthedocs.org/projects/heat/badge/?version=latest)](https://heat.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![coverage](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
 [![license: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/heat)](https://pypi.org/project/heat/)
 [![Downloads](https://pepy.tech/badge/heat)](https://pepy.tech/project/heat)
-[![Github-Pages - Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/heat/badges/version.svg)](https://anaconda.org/conda-forge/heat)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/helmholtz-analytics/heat/badge)](https://securityscorecards.dev/viewer/?uri=github.com/helmholtz-analytics/heat)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7688/badge)](https://bestpractices.coreinfrastructure.org/projects/7688)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2531472.svg)](https://doi.org/10.5281/zenodo.2531472)
+[![Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-# Goals
+# Table of Contents
+  - [What is Heat for?](#what-is-heat-for)
+  - [Features](#features)
+  - [Getting Started](#getting-started)
+  - [Installation](#installation)
+    - [Requirements](#requirements)
+    - [pip](#pip)
+    - [conda](#conda)
+  - [Support Channels](#support-channels)
+  - [Contribution guidelines](#contribution-guidelines)
+    - [Resources](#resources)
+  - [License](#license)
+  - [Citing Heat](#citing-heat)
+  - [FAQ](#faq)
+  - [Acknowledgements](#acknowledgements)
 
-Heat is a flexible and seamless open-source software for high performance data
-analytics and machine learning. It provides highly optimized algorithms and data
-structures for tensor computations using CPUs, GPUs and distributed cluster
-systems on top of MPI. The goal of Heat is to fill the gap between data
-analytics and machine learning libraries with a strong focus on single-node
-performance, and traditional high-performance computing (HPC). Heat's generic
-Python-first programming interface integrates seamlessly with the existing data
-science ecosystem and makes it as effortless as using numpy to write scalable
-scientific and data science applications.
 
-Heat allows you to tackle your actual Big Data challenges that go beyond the
-computational and memory needs of your laptop and desktop.
+# What is Heat for?
 
-# Features
+Heat builds on [PyTorch](https://pytorch.org/) and [mpi4py](https://mpi4py.readthedocs.io) to provide high-performance computing infrastructure for memory-intensive applications within the NumPy/SciPy ecosystem.
 
-* High-performance n-dimensional tensors
-* CPU, GPU and distributed computation using MPI
-* Powerful data analytics and machine learning methods
-* Abstracted communication via split tensors
-* Python API
 
-# Support Channels
+With Heat you can:
+- port existing NumPy/SciPy code from single-CPU to multi-node clusters with minimal coding effort;
+- exploit the entire, cumulative RAM of your many nodes for memory-intensive operations and algorithms;
+- run your NumPy/SciPy code on GPUs (CUDA, ROCm, coming up: Apple MPS).
 
-We use [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions) as a forum for questions about Heat.
-If you found a bug or miss a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
+For a example that highlights the benefits of multi-node parallelism, hardware acceleration, and how easy this can be done with the help of Heat, see, e.g., our [blog post on trucated SVD of a 200GB data set](https://helmholtz-analytics.github.io/heat/2023/06/16/new-feature-hsvd.html).
 
-# Requirements
+Check out our [coverage tables](coverage_tables.md) to see which NumPy, SciPy, scikit-learn functions are already supported.
 
-Heat requires Python 3.7 or newer.
-Heat is based on [PyTorch](https://pytorch.org/). Specifically, we are exploiting
-PyTorch's support for GPUs *and* MPI parallelism. For MPI support we utilize
-[mpi4py](https://mpi4py.readthedocs.io). Both packages can be installed via pip
-or automatically using the setup.py.
+ If you need a functionality that is not yet supported:
+  - [search existing issues](https://github.com/helmholtz-analytics/heat/issues) and make sure to leave a comment if someone else already requested it;
+  - [open a new issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
 
-# Installation
 
-Tagged releases are made available on the
-[Python Package Index (PyPI)](https://pypi.org/project/heat/). You can typically
-install the latest version with
+Check out our [features](#features) and the [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html) for a complete list of functionalities.
 
-```
-$ pip install heat[hdf5,netcdf]
-```
+# Features
 
-where the part in brackets is a list of optional dependencies. You can omit
-it, if you do not need HDF5 or NetCDF support.
+* High-performance n-dimensional arrays
+* CPU, GPU, and distributed computation using MPI
+* Powerful data analytics and machine learning methods
+* Seamless integration with the NumPy/SciPy ecosystem
+* Python array API (work in progress)
 
-**It is recommended to use the most recent supported version of PyTorch!**
 
-**It is also very important to ensure that the PyTorch version is compatible with the local CUDA installation.**
-More information can be found [here](https://pytorch.org/get-started/locally/).
+# Getting Started
 
-# Hacking
+Go to [Quick Start](quick_start.md) for a quick overview. For more details, see [Installation](#installation).
 
-If you want to work with the development version, you can check out the sources using
+**You can test your setup** by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
 
-```
-$ git clone <https://github.com/helmholtz-analytics/heat.git>
+```shell
+mpirun -n 2 python heat_test.py
 ```
 
-The installation can then be done from the checked-out sources with
+It should print something like this:
 
+```shell
+x is distributed:  True
+Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
+Global DNDarray x:
+Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
+Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
 ```
-$ pip install heat[hdf5,netcdf,dev]
-```
-
-# Getting Started
 
-TL;DR: [Quick Start](quick_start.md) (Read this to get a quick overview of Heat).
-
-Check out our Jupyter Notebook [**Tutorial**](https://github.com/helmholtz-analytics/heat/blob/main/scripts/)
-right here on Github or in the /scripts directory, to learn and understand about the basics and working of Heat.
+Check out our Jupyter Notebook [**Tutorials**](https://github.com/helmholtz-analytics/heat/blob/main/tutorials/), choose `local` to try things out on your machine, or `hpc` if you have access to an HPC system.
 
 The complete documentation of the latest version is always deployed on
 [Read the Docs](https://heat.readthedocs.io/).
 
-***Try your first Heat program***
 
-```shell
-$ python
-```
+<!-- # Goals
 
-```python
->>> import heat as ht
->>> x = ht.arange(10,split=0)
->>> print(x)
-DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
->>> y = ht.ones(10,split=0)
->>> print(y)
-DNDarray([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.], dtype=ht.float32, device=cpu:0, split=0)
->>> print(x + y)
-DNDarray([ 1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.], dtype=ht.float32, device=cpu:0, split=0)
-```
+Heat is a flexible and seamless open-source software for high performance data
+analytics and machine learning. It provides highly optimized algorithms and data structures for tensor computations using CPUs, GPUs, and distributed cluster systems on top of MPI. The goal of Heat is to fill the gap between single-node data analytics and machine learning libraries, and  high-performance computing (HPC). Heat's interface integrates seamlessly with the existing data science ecosystem and makes  writing scalable
+scientific and data science applications as effortless as using NumPy.
 
-### Also, you can test your setup by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
+Heat allows you to tackle your actual Big Data challenges that go beyond the
+computational and memory needs of your laptop and desktop.
+ -->
+# Installation
 
-```shell
-mpirun -n 2 python heat_test.py
-```
+## Requirements
 
-### It should print something like this:
+### Basics
+- python >= 3.8
+- MPI (OpenMPI, MPICH, Intel MPI, etc.)
+- mpi4py >= 3.0.0
+- pytorch >= 1.8.0
 
-```shell
-x is distributed:  True
-Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
-Global DNDarray x:
-Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
-Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
-```
+### Parallel I/O
+- h5py
+- netCDF4
 
-## Resources:
+### GPU support
+In order to do computations on your GPU(s):
+- your CUDA or ROCm installation must match your hardware and its drivers;
+- your [PyTorch installation](https://pytorch.org/get-started/locally/) must be compiled with CUDA/ROCm support.
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
-* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+### HPC systems
+On most HPC-systems you will not be able to install/compile MPI or CUDA/ROCm yourself. Instead, you will most likely need to load a pre-installed MPI and/or CUDA/ROCm module from the module system. Maybe, you will even find PyTorch, h5py, or mpi4py as (part of) such a module. Note that for optimal performance on GPU, you need to usa an MPI library that has been compiled with CUDA/ROCm support (e.g., so-called "CUDA-aware MPI").
 
-### Parallel Computing and MPI:
 
-* @davidhenty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
-* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+## pip
+Install the latest version with
 
-### mpi4py
+```bash
+pip install heat[hdf5,netcdf]
+```
+where the part in brackets is a list of optional dependencies. You can omit
+it, if you do not need HDF5 or NetCDF support.
 
-* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
-* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
+## **conda**
 
-# Contribution guidelines
+The conda build includes all dependencies **including OpenMPI**.
+```bash
+ conda install -c conda-forge heat
+ ```
 
-**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) before getting started!**
+# Support Channels
 
-We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion, and You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo). You can sign up with your GitHub credentials. Once you log in, you can introduce yourself on the `Town Square` channel.
+Go ahead and ask questions on [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions). If you found a bug or are missing a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose). You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
-Small improvements or fixes are always appreciated; issues labeled as **"good first issue"** may be a good starting point.
+
+# Contribution guidelines
+
+**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) and [Resources](#resources)  before getting started!**
+
+We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion. You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo) (sign up with your GitHub credentials). Once you log in, you can introduce yourself on the `Town Square` channel.
 
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
+
+## Resources
+
+* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+
+### Parallel Computing and MPI:
+
+* David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
+* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+* Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
+
+### mpi4py
+
+* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
+* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
 # License
 
 Heat is distributed under the MIT license, see our
 [LICENSE](LICENSE) file.
 
 # Citing Heat
 
-If you find Heat helpful for your research, please mention it in your publications. You can cite:
+<!-- If you find Heat helpful for your research, please mention it in your publications. You can cite: -->
+
+Please do mention Heat in your publications if it helped your research. You can cite:
 
 * Götz, M., Debus, C., Coquelin, D., Krajsek, K., Comito, C., Knechtges, P., Hagemeier, B., Tarnawa, M., Hanselmann, S., Siggel, S., Basermann, A. & Streit, A. (2020). HeAT - a Distributed and GPU-accelerated Tensor Framework for Data Analytics. In 2020 IEEE International Conference on Big Data (Big Data) (pp. 276-287). IEEE, DOI: 10.1109/BigData50022.2020.9378050.
 
 ```
 @inproceedings{heat2020,
     title={{HeAT -- a Distributed and GPU-accelerated Tensor Framework for Data Analytics}},
     author={
@@ -225,19 +247,29 @@
     year={2020},
     pages={276-287},
     month={December},
     publisher={IEEE},
     doi={10.1109/BigData50022.2020.9378050}
 }
 ```
+# FAQ
+Work in progress...
+
+  <!-- - Users
+  - Developers
+  - Students
+  - system administrators -->
 
 ## Acknowledgements
 
 *This work is supported by the [Helmholtz Association Initiative and
 Networking Fund](https://www.helmholtz.de/en/about_us/the_association/initiating_and_networking/)
 under project number ZT-I-0003 and the Helmholtz AI platform grant.*
 
+*This project has received funding from Google Summer of Code (GSoC) in 2022.*
+
+
 ---
 
 <div align="center">
-  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/master/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
+  <a href="https://www.dlr.de/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/dlr_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.fz-juelich.de/portal/EN/Home/home_node.html"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/fzj_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="http://www.kit.edu/english/index.php"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/kit_logo.svg" height="50px" hspace="3%" vspace="20px"></a><a href="https://www.helmholtz.de/en/"><img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/helmholtz_logo.svg" height="50px" hspace="3%" vspace="20px"></a>
 </div>
```

### Comparing `heat-1.3.1/heat.egg-info/SOURCES.txt` & `heat-1.4.0/heat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 heat.egg-info/dependency_links.txt
 heat.egg-info/requires.txt
 heat.egg-info/top_level.txt
 heat/classification/__init__.py
 heat/classification/kneighborsclassifier.py
 heat/cluster/__init__.py
 heat/cluster/_kcluster.py
+heat/cluster/batchparallelclustering.py
 heat/cluster/kmeans.py
 heat/cluster/kmedians.py
 heat/cluster/kmedoids.py
 heat/cluster/spectral.py
 heat/core/__init__.py
 heat/core/_operations.py
 heat/core/arithmetics.py
@@ -58,25 +59,29 @@
 heat/datasets/iris.nc
 heat/datasets/iris_X_test.csv
 heat/datasets/iris_X_train.csv
 heat/datasets/iris_labels.csv
 heat/datasets/iris_y_pred_proba.csv
 heat/datasets/iris_y_test.csv
 heat/datasets/iris_y_train.csv
+heat/fft/__init__.py
+heat/fft/fft.py
 heat/graph/__init__.py
 heat/graph/laplacian.py
 heat/naive_bayes/__init__.py
 heat/naive_bayes/gaussianNB.py
 heat/nn/__init__.py
 heat/nn/data_parallel.py
 heat/nn/functional.py
 heat/optim/__init__.py
 heat/optim/dp_optimizer.py
 heat/optim/lr_scheduler.py
 heat/optim/utils.py
+heat/preprocessing/__init__.py
+heat/preprocessing/preprocessing.py
 heat/regression/__init__.py
 heat/regression/lasso.py
 heat/sparse/__init__.py
 heat/sparse/_operations.py
 heat/sparse/arithmetics.py
 heat/sparse/dcsr_matrix.py
 heat/sparse/factories.py
```

### Comparing `heat-1.3.1/setup.py` & `heat-1.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,25 +23,26 @@
     keywords=["data", "analytics", "tensors", "distributed", "gpu"],
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
     ],
     install_requires=[
         "mpi4py>=3.0.0",
-        "numpy>=1.20.0",
-        "torch>=1.8.0, <2.0.2",
-        "scipy>=0.14.0",
+        "numpy>=1.22.0",
+        "torch>=1.11.0, <2.2.3",
+        "scipy>=1.10.0",
         "pillow>=6.0.0",
-        "torchvision>=0.8.0",
+        "torchvision>=0.12.0",
     ],
     extras_require={
         "docutils": ["docutils>=0.16"],
         "hdf5": ["h5py>=2.8.0"],
         "netcdf": ["netCDF4>=1.5.6"],
         "dev": ["pre-commit>=1.18.3"],
         "examples": ["scikit-learn>=0.24.0", "matplotlib>=3.1.0"],
```

