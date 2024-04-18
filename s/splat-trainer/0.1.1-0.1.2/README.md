# Comparing `tmp/splat_trainer-0.1.1.tar.gz` & `tmp/splat_trainer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splat_trainer-0.1.1.tar", last modified: Wed Apr 17 07:30:30 2024, max compression
+gzip compressed data, was "splat_trainer-0.1.2.tar", last modified: Thu Apr 18 08:09:01 2024, max compression
```

## Comparing `splat_trainer-0.1.1.tar` & `splat_trainer-0.1.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.944532 splat_trainer-0.1.1/
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2137 2024-03-01 14:39:10.000000 splat_trainer-0.1.1/.gitignore
--rw-r--r--   0 owb14    (10479) domain users (1000002)      684 2024-04-17 07:30:30.937776 splat_trainer-0.1.1/PKG-INFO
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1271 2024-04-17 07:27:14.000000 splat_trainer-0.1.1/pyproject.toml
--rw-r--r--   0 owb14    (10479) domain users (1000002)       38 2024-04-17 07:30:30.946479 splat_trainer-0.1.1/setup.cfg
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.474947 splat_trainer-0.1.1/splat_trainer/
--rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-20 05:09:02.000000 splat_trainer-0.1.1/splat_trainer/__init__.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.539939 splat_trainer-0.1.1/splat_trainer/camera_table/
--rw-r--r--   0 owb14    (10479) domain users (1000002)     3550 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/camera_table/camera_table.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2278 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/camera_table/pose_table.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.554020 splat_trainer-0.1.1/splat_trainer/config/
--rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-20 04:37:36.000000 splat_trainer-0.1.1/splat_trainer/config/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      848 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/config/config.yaml
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.578947 splat_trainer-0.1.1/splat_trainer/config/controller/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      121 2024-03-16 11:58:41.000000 splat_trainer-0.1.1/splat_trainer/config/controller/static.yaml
--rw-r--r--   0 owb14    (10479) domain users (1000002)      313 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/config/controller/target.yaml
--rw-r--r--   0 owb14    (10479) domain users (1000002)      277 2024-03-16 06:06:53.000000 splat_trainer-0.1.1/splat_trainer/config/controller/threshold.yaml
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.594510 splat_trainer-0.1.1/splat_trainer/config/dataset/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      276 2024-03-18 05:23:50.000000 splat_trainer-0.1.1/splat_trainer/config/dataset/colmap.yaml
--rw-r--r--   0 owb14    (10479) domain users (1000002)      227 2024-03-18 05:23:55.000000 splat_trainer-0.1.1/splat_trainer/config/dataset/scan.yaml
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.610554 splat_trainer-0.1.1/splat_trainer/config/logger/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      115 2024-02-29 03:20:33.000000 splat_trainer-0.1.1/splat_trainer/config/logger/tensorboard.yaml
--rw-r--r--   0 owb14    (10479) domain users (1000002)      112 2024-02-29 05:01:49.000000 splat_trainer-0.1.1/splat_trainer/config/logger/wandb.yaml
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.626828 splat_trainer-0.1.1/splat_trainer/config/scene/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      269 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/config/scene/sh.yaml
--rw-r--r--   0 owb14    (10479) domain users (1000002)      381 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/config/scene/tcnn.yaml
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.658718 splat_trainer-0.1.1/splat_trainer/controller/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      310 2024-03-16 05:52:51.000000 splat_trainer-0.1.1/splat_trainer/controller/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      733 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/controller/controller.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     5395 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/controller/target_controller.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     3468 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/controller/threshold_controller.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.675907 splat_trainer-0.1.1/splat_trainer/dataset/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      298 2024-03-17 09:27:12.000000 splat_trainer-0.1.1/splat_trainer/dataset/__init__.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.699330 splat_trainer-0.1.1/splat_trainer/dataset/colmap/
--rw-------   0 owb14    (10479) domain users (1000002)        0 2024-03-17 09:27:23.000000 splat_trainer-0.1.1/splat_trainer/dataset/colmap/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     3957 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/dataset/colmap/dataset.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2019 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/dataset/colmap/loading.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      735 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/dataset/dataset.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.733103 splat_trainer-0.1.1/splat_trainer/dataset/scan/
--rw-r--r--   0 owb14    (10479) domain users (1000002)       60 2024-02-22 02:33:42.000000 splat_trainer-0.1.1/splat_trainer/dataset/scan/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     3124 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/dataset/scan/dataset.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2150 2024-04-07 12:06:43.000000 splat_trainer-0.1.1/splat_trainer/dataset/scan/loading.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1481 2024-02-22 02:33:42.000000 splat_trainer-0.1.1/splat_trainer/dataset/scan/visibility.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.750240 splat_trainer-0.1.1/splat_trainer/gaussians/
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1196 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/gaussians/loading.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2380 2024-03-18 05:27:15.000000 splat_trainer-0.1.1/splat_trainer/gaussians/split.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1637 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/image_scaler.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.792219 splat_trainer-0.1.1/splat_trainer/logger/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      238 2024-02-22 02:33:42.000000 splat_trainer-0.1.1/splat_trainer/logger/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2828 2024-02-25 23:24:12.000000 splat_trainer-0.1.1/splat_trainer/logger/histogram.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1046 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/logger/logger.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     3221 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/logger/tensorboard.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2927 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/logger/wandb.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.801482 splat_trainer-0.1.1/splat_trainer/modules/
--rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-21 03:10:54.000000 splat_trainer-0.1.1/splat_trainer/modules/__init__.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.841838 splat_trainer-0.1.1/splat_trainer/scene/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      291 2024-03-16 06:06:10.000000 splat_trainer-0.1.1/splat_trainer/scene/__init__.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     5011 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scene/io.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1184 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scene/scene.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     4235 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scene/sh_scene.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     7904 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scene/tcnn_scene.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      847 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scheduler.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.865638 splat_trainer-0.1.1/splat_trainer/scripts/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      943 2024-03-14 02:33:28.000000 splat_trainer-0.1.1/splat_trainer/scripts/test_split.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1719 2024-03-13 13:56:15.000000 splat_trainer-0.1.1/splat_trainer/scripts/test_tcnn.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1285 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/scripts/train_scan.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)    10488 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/trainer.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.918906 splat_trainer-0.1.1/splat_trainer/util/
--rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-07 04:13:17.000000 splat_trainer-0.1.1/splat_trainer/util/__init__.py
--rw-------   0 owb14    (10479) domain users (1000002)      545 2024-03-16 12:23:46.000000 splat_trainer-0.1.1/splat_trainer/util/colorize.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      592 2024-02-20 07:41:25.000000 splat_trainer-0.1.1/splat_trainer/util/config.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)      149 2024-03-01 14:37:30.000000 splat_trainer-0.1.1/splat_trainer/util/containers.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1113 2024-03-18 11:01:28.000000 splat_trainer-0.1.1/splat_trainer/util/misc.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1760 2024-02-26 05:46:10.000000 splat_trainer-0.1.1/splat_trainer/util/pointcloud.py
--rw-r--r--   0 owb14    (10479) domain users (1000002)     1290 2024-04-17 07:02:25.000000 splat_trainer-0.1.1/splat_trainer/util/transforms.py
-drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-17 07:30:30.927987 splat_trainer-0.1.1/splat_trainer.egg-info/
--rw-r--r--   0 owb14    (10479) domain users (1000002)      684 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/PKG-INFO
--rw-r--r--   0 owb14    (10479) domain users (1000002)     2136 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 owb14    (10479) domain users (1000002)        1 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 owb14    (10479) domain users (1000002)       72 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/entry_points.txt
--rw-r--r--   0 owb14    (10479) domain users (1000002)      145 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/requires.txt
--rw-r--r--   0 owb14    (10479) domain users (1000002)       14 2024-04-17 07:30:30.000000 splat_trainer-0.1.1/splat_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.816330 splat_trainer-0.1.2/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2137 2024-03-01 14:39:10.000000 splat_trainer-0.1.2/.gitignore
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      684 2024-04-18 08:09:01.810076 splat_trainer-0.1.2/PKG-INFO
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1362 2024-04-18 08:08:25.000000 splat_trainer-0.1.2/pyproject.toml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)       38 2024-04-18 08:09:01.818000 splat_trainer-0.1.2/setup.cfg
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.381205 splat_trainer-0.1.2/splat_trainer/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-20 05:09:02.000000 splat_trainer-0.1.2/splat_trainer/__init__.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.439867 splat_trainer-0.1.2/splat_trainer/camera_table/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     3550 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/camera_table/camera_table.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2278 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/camera_table/pose_table.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.453265 splat_trainer-0.1.2/splat_trainer/config/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-20 04:37:36.000000 splat_trainer-0.1.2/splat_trainer/config/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      848 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/config/config.yaml
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.476259 splat_trainer-0.1.2/splat_trainer/config/controller/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      121 2024-03-16 11:58:41.000000 splat_trainer-0.1.2/splat_trainer/config/controller/static.yaml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      313 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/config/controller/target.yaml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      277 2024-03-16 06:06:53.000000 splat_trainer-0.1.2/splat_trainer/config/controller/threshold.yaml
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.491370 splat_trainer-0.1.2/splat_trainer/config/dataset/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      276 2024-03-18 05:23:50.000000 splat_trainer-0.1.2/splat_trainer/config/dataset/colmap.yaml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      227 2024-03-18 05:23:55.000000 splat_trainer-0.1.2/splat_trainer/config/dataset/scan.yaml
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.505766 splat_trainer-0.1.2/splat_trainer/config/logger/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      115 2024-02-29 03:20:33.000000 splat_trainer-0.1.2/splat_trainer/config/logger/tensorboard.yaml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      112 2024-02-29 05:01:49.000000 splat_trainer-0.1.2/splat_trainer/config/logger/wandb.yaml
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.520663 splat_trainer-0.1.2/splat_trainer/config/scene/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      269 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/config/scene/sh.yaml
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      381 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/config/scene/tcnn.yaml
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.550685 splat_trainer-0.1.2/splat_trainer/controller/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      310 2024-03-16 05:52:51.000000 splat_trainer-0.1.2/splat_trainer/controller/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      733 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/controller/controller.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     5395 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/controller/target_controller.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     3468 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/controller/threshold_controller.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.565928 splat_trainer-0.1.2/splat_trainer/dataset/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      298 2024-03-17 09:27:12.000000 splat_trainer-0.1.2/splat_trainer/dataset/__init__.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.588961 splat_trainer-0.1.2/splat_trainer/dataset/colmap/
+-rw-------   0 owb14    (10479) domain users (1000002)        0 2024-03-17 09:27:23.000000 splat_trainer-0.1.2/splat_trainer/dataset/colmap/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     3957 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/dataset/colmap/dataset.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2019 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/dataset/colmap/loading.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      735 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/dataset/dataset.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.618815 splat_trainer-0.1.2/splat_trainer/dataset/scan/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)       60 2024-02-22 02:33:42.000000 splat_trainer-0.1.2/splat_trainer/dataset/scan/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     3124 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/dataset/scan/dataset.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2150 2024-04-07 12:06:43.000000 splat_trainer-0.1.2/splat_trainer/dataset/scan/loading.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1481 2024-02-22 02:33:42.000000 splat_trainer-0.1.2/splat_trainer/dataset/scan/visibility.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.634266 splat_trainer-0.1.2/splat_trainer/gaussians/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1196 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/gaussians/loading.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2380 2024-03-18 05:27:15.000000 splat_trainer-0.1.2/splat_trainer/gaussians/split.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1637 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/image_scaler.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.671657 splat_trainer-0.1.2/splat_trainer/logger/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      238 2024-02-22 02:33:42.000000 splat_trainer-0.1.2/splat_trainer/logger/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2828 2024-02-25 23:24:12.000000 splat_trainer-0.1.2/splat_trainer/logger/histogram.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1046 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/logger/logger.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     3221 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/logger/tensorboard.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2928 2024-04-18 07:55:07.000000 splat_trainer-0.1.2/splat_trainer/logger/wandb.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.680810 splat_trainer-0.1.2/splat_trainer/modules/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-21 03:10:54.000000 splat_trainer-0.1.2/splat_trainer/modules/__init__.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.717077 splat_trainer-0.1.2/splat_trainer/scene/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      291 2024-03-16 06:06:10.000000 splat_trainer-0.1.2/splat_trainer/scene/__init__.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     5011 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scene/io.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1184 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scene/scene.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     4235 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scene/sh_scene.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     7904 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scene/tcnn_scene.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      847 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scheduler.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.739665 splat_trainer-0.1.2/splat_trainer/scripts/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      943 2024-03-14 02:33:28.000000 splat_trainer-0.1.2/splat_trainer/scripts/test_split.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1719 2024-03-13 13:56:15.000000 splat_trainer-0.1.2/splat_trainer/scripts/test_tcnn.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1285 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/scripts/train_scan.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)    10488 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/trainer.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.792387 splat_trainer-0.1.2/splat_trainer/util/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)        0 2024-02-07 04:13:17.000000 splat_trainer-0.1.2/splat_trainer/util/__init__.py
+-rw-------   0 owb14    (10479) domain users (1000002)      545 2024-03-16 12:23:46.000000 splat_trainer-0.1.2/splat_trainer/util/colorize.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      592 2024-02-20 07:41:25.000000 splat_trainer-0.1.2/splat_trainer/util/config.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      149 2024-03-01 14:37:30.000000 splat_trainer-0.1.2/splat_trainer/util/containers.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1113 2024-03-18 11:01:28.000000 splat_trainer-0.1.2/splat_trainer/util/misc.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1760 2024-02-26 05:46:10.000000 splat_trainer-0.1.2/splat_trainer/util/pointcloud.py
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     1290 2024-04-17 07:02:25.000000 splat_trainer-0.1.2/splat_trainer/util/transforms.py
+drwxr-xr-x   0 owb14    (10479) domain users (1000002)        0 2024-04-18 08:09:01.801332 splat_trainer-0.1.2/splat_trainer.egg-info/
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      684 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 owb14    (10479) domain users (1000002)     2136 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 owb14    (10479) domain users (1000002)        1 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 owb14    (10479) domain users (1000002)       72 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/entry_points.txt
+-rw-r--r--   0 owb14    (10479) domain users (1000002)      145 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/requires.txt
+-rw-r--r--   0 owb14    (10479) domain users (1000002)       14 2024-04-18 08:09:01.000000 splat_trainer-0.1.2/splat_trainer.egg-info/top_level.txt
```

### Comparing `splat_trainer-0.1.1/.gitignore` & `splat_trainer-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/PKG-INFO` & `splat_trainer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splat-trainer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Gaussian Splatting scene reconstruction with taichi-splatting
 Maintainer-email: Oliver Batchelor <oliver.batchelor@canterbury.ac.nz>
 Project-URL: Homepage, https://github.com/uc-vision/splat-trainer
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: taichi-splatting>=0.12.0
 Requires-Dist: tqdm
```

### Comparing `splat_trainer-0.1.1/pyproject.toml` & `splat_trainer-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "splat-trainer"  
-version = "0.1.1"  
+version = "0.1.2"  
 description = "Gaussian Splatting scene reconstruction with taichi-splatting"  
 readme = "README.md" 
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 
 maintainers = [
   {name = "Oliver Batchelor", email = "oliver.batchelor@canterbury.ac.nz" } 
@@ -20,15 +20,16 @@
   'roma>=1.4',
   'tabulate',
   'torchmetrics',
   'opencv-python',
   'pycolmap',
   'scipy',
   'tensorboard',
-  'wandb'
+  'wandb',
+#  'tinycudann @ git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch'
 ]
 
 
 [tool.setuptools.packages.find]
 include = ["splat_trainer"]
 exclude = ["profiles", "benchmarks"]
```

### Comparing `splat_trainer-0.1.1/splat_trainer/camera_table/camera_table.py` & `splat_trainer-0.1.2/splat_trainer/camera_table/camera_table.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/camera_table/pose_table.py` & `splat_trainer-0.1.2/splat_trainer/camera_table/pose_table.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/config/config.yaml` & `splat_trainer-0.1.2/splat_trainer/config/config.yaml`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/controller/controller.py` & `splat_trainer-0.1.2/splat_trainer/controller/controller.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/controller/target_controller.py` & `splat_trainer-0.1.2/splat_trainer/controller/target_controller.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/controller/threshold_controller.py` & `splat_trainer-0.1.2/splat_trainer/controller/threshold_controller.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/colmap/dataset.py` & `splat_trainer-0.1.2/splat_trainer/dataset/colmap/dataset.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/colmap/loading.py` & `splat_trainer-0.1.2/splat_trainer/dataset/colmap/loading.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/dataset.py` & `splat_trainer-0.1.2/splat_trainer/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/scan/dataset.py` & `splat_trainer-0.1.2/splat_trainer/dataset/scan/dataset.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/scan/loading.py` & `splat_trainer-0.1.2/splat_trainer/dataset/scan/loading.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/dataset/scan/visibility.py` & `splat_trainer-0.1.2/splat_trainer/dataset/scan/visibility.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/gaussians/loading.py` & `splat_trainer-0.1.2/splat_trainer/gaussians/loading.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/gaussians/split.py` & `splat_trainer-0.1.2/splat_trainer/gaussians/split.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/image_scaler.py` & `splat_trainer-0.1.2/splat_trainer/image_scaler.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/logger/histogram.py` & `splat_trainer-0.1.2/splat_trainer/logger/histogram.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/logger/logger.py` & `splat_trainer-0.1.2/splat_trainer/logger/logger.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/logger/tensorboard.py` & `splat_trainer-0.1.2/splat_trainer/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/logger/wandb.py` & `splat_trainer-0.1.2/splat_trainer/logger/wandb.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from splat_trainer.logger.histogram import Histogram
 from splat_trainer.util.pointcloud import PointCloud
 
 from .logger import Logger
 
 class WandbLogger(Logger):
   def __init__(self, project:str | None, log_config:dict, name:str | None=None, dir:str | None = None):
+
     if dir is not None:
       dir = Path(dir).mkdir(parents=True, exist_ok=True)
     self.run = wandb.init(project=project, name=name, config=log_config, dir=dir, settings=wandb.Settings(start_method='thread'))
 
     self.queue = Queue()
     self.log_thread = Thread(target=self.worker)
     self.log_thread.start()
```

### Comparing `splat_trainer-0.1.1/splat_trainer/scene/io.py` & `splat_trainer-0.1.2/splat_trainer/scene/io.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scene/scene.py` & `splat_trainer-0.1.2/splat_trainer/scene/scene.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scene/sh_scene.py` & `splat_trainer-0.1.2/splat_trainer/scene/sh_scene.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scene/tcnn_scene.py` & `splat_trainer-0.1.2/splat_trainer/scene/tcnn_scene.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scheduler.py` & `splat_trainer-0.1.2/splat_trainer/scheduler.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scripts/test_split.py` & `splat_trainer-0.1.2/splat_trainer/scripts/test_split.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scripts/test_tcnn.py` & `splat_trainer-0.1.2/splat_trainer/scripts/test_tcnn.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/scripts/train_scan.py` & `splat_trainer-0.1.2/splat_trainer/scripts/train_scan.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/trainer.py` & `splat_trainer-0.1.2/splat_trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/util/colorize.py` & `splat_trainer-0.1.2/splat_trainer/util/colorize.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/util/config.py` & `splat_trainer-0.1.2/splat_trainer/util/config.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/util/misc.py` & `splat_trainer-0.1.2/splat_trainer/util/misc.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/util/pointcloud.py` & `splat_trainer-0.1.2/splat_trainer/util/pointcloud.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer/util/transforms.py` & `splat_trainer-0.1.2/splat_trainer/util/transforms.py`

 * *Files identical despite different names*

### Comparing `splat_trainer-0.1.1/splat_trainer.egg-info/PKG-INFO` & `splat_trainer-0.1.2/splat_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splat-trainer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Gaussian Splatting scene reconstruction with taichi-splatting
 Maintainer-email: Oliver Batchelor <oliver.batchelor@canterbury.ac.nz>
 Project-URL: Homepage, https://github.com/uc-vision/splat-trainer
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: taichi-splatting>=0.12.0
 Requires-Dist: tqdm
```

### Comparing `splat_trainer-0.1.1/splat_trainer.egg-info/SOURCES.txt` & `splat_trainer-0.1.2/splat_trainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

