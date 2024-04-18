# Comparing `tmp/sightvision-0.2.1.tar.gz` & `tmp/sightvision-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sightvision-0.2.1.tar", last modified: Thu Aug  3 16:48:40 2023, max compression
+gzip compressed data, was "sightvision-0.2.2.tar", last modified: Thu Apr 18 15:49:28 2024, max compression
```

## Comparing `sightvision-0.2.1.tar` & `sightvision-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,4 @@
-drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.770466 sightvision-0.2.1/
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1065 2023-07-21 15:53:52.000000 sightvision-0.2.1/LICENSE.txt
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5769 2023-08-03 16:48:40.770466 sightvision-0.2.1/PKG-INFO
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     4814 2023-07-25 01:46:28.000000 sightvision-0.2.1/README.md
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       79 2023-08-03 16:48:40.770466 sightvision-0.2.1/setup.cfg
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2123 2023-08-03 16:48:35.000000 sightvision-0.2.1/setup.py
-drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.766466 sightvision-0.2.1/sightvision/
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2265 2023-07-22 17:28:26.000000 sightvision-0.2.1/sightvision/ClassificationModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3756 2023-07-21 22:24:48.000000 sightvision-0.2.1/sightvision/ColorModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1559 2023-07-22 11:47:16.000000 sightvision-0.2.1/sightvision/FPS.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3360 2023-07-31 22:14:02.000000 sightvision-0.2.1/sightvision/FaceDetectionModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3607 2023-07-21 19:32:34.000000 sightvision-0.2.1/sightvision/FaceMeshModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     7350 2023-07-21 22:19:48.000000 sightvision-0.2.1/sightvision/HandTrackingModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2235 2023-07-22 12:03:22.000000 sightvision-0.2.1/sightvision/PIDModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3423 2023-07-21 22:22:52.000000 sightvision-0.2.1/sightvision/PlotModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5536 2023-07-21 22:22:26.000000 sightvision-0.2.1/sightvision/PoseModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1670 2023-07-21 22:21:52.000000 sightvision-0.2.1/sightvision/SelfiSegmentationModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2213 2023-07-21 22:21:28.000000 sightvision-0.2.1/sightvision/SerialModule.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     6541 2023-07-21 22:20:48.000000 sightvision-0.2.1/sightvision/Utils.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)      663 2023-07-22 17:31:02.000000 sightvision-0.2.1/sightvision/__init__.py
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       34 2023-07-28 23:19:22.000000 sightvision-0.2.1/sightvision/config.py
-drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.766466 sightvision-0.2.1/sightvision.egg-info/
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5769 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/PKG-INFO
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)      606 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/SOURCES.txt
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)        1 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/dependency_links.txt
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       57 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/requires.txt
--rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       12 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/top_level.txt
+drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2024-04-18 15:49:28.555760 sightvision-0.2.2/
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)      637 2024-04-18 15:49:28.555760 sightvision-0.2.2/PKG-INFO
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       39 2024-04-18 15:40:41.538148 sightvision-0.2.2/setup.cfg
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1017 2024-04-18 15:49:20.539857 sightvision-0.2.2/setup.py
```

