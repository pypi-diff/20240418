# Comparing `tmp/ultralytics-8.1.9.tar.gz` & `tmp/ultralytics-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.1.9.tar", last modified: Thu Feb  1 22:36:55 2024, max compression
+gzip compressed data, was "ultralytics-8.2.0.tar", last modified: Wed Apr 17 04:38:38 2024, max compression
```

## Comparing `ultralytics-8.1.9.tar` & `ultralytics-8.2.0.tar`

### file list

```diff
@@ -1,243 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.298454 ultralytics-8.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-01 22:35:40.000000 ultralytics-8.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-02-01 22:36:55.298454 ultralytics-8.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36735 2024-02-01 22:35:40.000000 ultralytics-8.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-02-01 22:35:40.000000 ultralytics-8.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 22:36:55.298454 ultralytics-8.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.258454 ultralytics-8.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.258454 ultralytics-8.1.9/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.262454 ultralytics-8.1.9/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.262454 ultralytics-8.1.9/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.254454 ultralytics-8.1.9/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    52000 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51992 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    37636 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17832 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34306 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16190 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38765 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.290454 ultralytics-8.1.9/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.290454 ultralytics-8.1.9/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    36882 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27665 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21189 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53358 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25143 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.651996 ultralytics-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-17 04:37:19.000000 ultralytics-8.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-04-17 04:38:38.651996 ultralytics-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36734 2024-04-17 04:37:19.000000 ultralytics-8.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-17 04:37:19.000000 ultralytics-8.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:38:38.651996 ultralytics-8.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.607995 ultralytics-8.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22960 2024-04-17 04:37:19.000000 ultralytics-8.2.0/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.607995 ultralytics-8.2.0/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.607995 ultralytics-8.2.0/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.611995 ultralytics-8.2.0/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.615995 ultralytics-8.2.0/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.603995 ultralytics-8.2.0/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.615995 ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.615995 ultralytics-8.2.0/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.615995 ultralytics-8.2.0/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.615995 ultralytics-8.2.0/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.619995 ultralytics-8.2.0/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.619995 ultralytics-8.2.0/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.619995 ultralytics-8.2.0/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.623995 ultralytics-8.2.0/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.623995 ultralytics-8.2.0/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.623995 ultralytics-8.2.0/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.623995 ultralytics-8.2.0/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54476 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34933 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.627995 ultralytics-8.2.0/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.631995 ultralytics-8.2.0/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.635995 ultralytics-8.2.0/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.635995 ultralytics-8.2.0/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.635995 ultralytics-8.2.0/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.635995 ultralytics-8.2.0/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.635995 ultralytics-8.2.0/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.639995 ultralytics-8.2.0/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.639995 ultralytics-8.2.0/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.639995 ultralytics-8.2.0/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.643996 ultralytics-8.2.0/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39292 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.647996 ultralytics-8.2.0/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47558 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-17 04:37:19.000000 ultralytics-8.2.0/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:38:38.647996 ultralytics-8.2.0/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 04:38:38.000000 ultralytics-8.2.0/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.1.9/LICENSE` & `ultralytics-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/PKG-INFO` & `ultralytics-8.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.1.9
+Version: 8.2.0
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -15,26 +15,26 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: numpy>=1.22.2
 Requires-Dist: opencv-python>=4.6.0
 Requires-Dist: pillow>=7.1.2
 Requires-Dist: pyyaml>=5.3.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchvision>=0.9.0
@@ -47,38 +47,40 @@
 Provides-Extra: dev
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs-material>=9.5.9; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: mkdocs-redirects; extra == "dev"
-Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
+Requires-Dist: mkdocs-ultralytics-plugin>=0.0.44; extra == "dev"
 Provides-Extra: export
 Requires-Dist: onnx>=1.12.0; extra == "export"
-Requires-Dist: coremltools>=7.0; platform_system != "Windows" and extra == "export"
-Requires-Dist: openvino-dev>=2023.0; extra == "export"
-Requires-Dist: tensorflow<=2.13.1; extra == "export"
-Requires-Dist: tensorflowjs>=3.9.0; extra == "export"
+Requires-Dist: coremltools>=7.0; (platform_system != "Windows" and python_version <= "3.11") and extra == "export"
+Requires-Dist: openvino>=2024.0.0; extra == "export"
+Requires-Dist: tensorflow<=2.13.1; python_version <= "3.11" and extra == "export"
+Requires-Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra == "export"
+Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
-Requires-Dist: duckdb; extra == "explorer"
+Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 Provides-Extra: logging
 Requires-Dist: comet; extra == "logging"
 Requires-Dist: tensorboard>=2.13.0; extra == "logging"
 Requires-Dist: dvclive>=2.12.0; extra == "logging"
 Provides-Extra: extra
-Requires-Dist: hub-sdk>=0.0.2; extra == "extra"
+Requires-Dist: hub-sdk>=0.0.5; extra == "extra"
 Requires-Dist: ipython; extra == "extra"
 Requires-Dist: albumentations>=1.0.3; extra == "extra"
-Requires-Dist: pycocotools>=2.0.6; extra == "extra"
+Requires-Dist: pycocotools>=2.0.7; extra == "extra"
 
 <div align="center">
   <p>
     <a href="https://www.ultralytics.com/blog/ultralytics-yolov8-turns-one-a-year-of-breakthroughs-and-innovations" target="_blank">
       <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/im/banner-yolo-vision-2023.png" alt="YOLO Vision banner"></a>
   </p>
 
@@ -274,15 +276,15 @@
 | -------------------------------------------------------------------------------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8n-obb.pt) | 1024                  | 78.0               | 204.77                         | 3.57                                | 3.1                | 23.3              |
 | [YOLOv8s-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8s-obb.pt) | 1024                  | 79.5               | 424.88                         | 4.07                                | 11.4               | 76.3              |
 | [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8m-obb.pt) | 1024                  | 80.5               | 763.48                         | 7.61                                | 26.4               | 208.6             |
 | [YOLOv8l-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt) | 1024                  | 80.7               | 1278.42                        | 11.83                               | 44.5               | 433.8             |
 | [YOLOv8x-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024                  | 81.36              | 1759.10                        | 13.23                               | 69.5               | 676.7             |
 
-- **mAP<sup>test</sup>** values are for single-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
+- **mAP<sup>test</sup>** values are for single-model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
 - **Speed** averaged over DOTAv1 val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance. <br>Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification (ImageNet)</summary>
 
 See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models trained on [ImageNet](https://docs.ultralytics.com/datasets/classify/imagenet/), which include 1000 pretrained classes.
```

#### html2text {}

```diff
@@ -1,54 +1,57 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.1.9 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.0 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
 vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development Classifier: Topic :: Scientific/Engineering Classifier:
-Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Image Recognition Classifier: Operating System ::
-POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
-System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: matplotlib>=3.3.0 Requires-
-Dist: numpy>=1.22.2 Requires-Dist: opencv-python>=4.6.0 Requires-Dist:
-pillow>=7.1.2 Requires-Dist: pyyaml>=5.3.1 Requires-Dist: requests>=2.23.0
-Requires-Dist: scipy>=1.4.1 Requires-Dist: torch>=1.8.0 Requires-Dist:
-torchvision>=0.9.0 Requires-Dist: tqdm>=4.64.0 Requires-Dist: psutil Requires-
-Dist: py-cpuinfo Requires-Dist: thop>=0.1.1 Requires-Dist: pandas>=1.1.4
-Requires-Dist: seaborn>=0.11.0 Provides-Extra: dev Requires-Dist: ipython;
-extra == "dev" Requires-Dist: check-manifest; extra == "dev" Requires-Dist:
-pre-commit; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-pytest-cov; extra == "dev" Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocstrings
-[python]; extra == "dev" Requires-Dist: mkdocs-jupyter; extra == "dev"
-Requires-Dist: mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-
-ultralytics-plugin>=0.0.42; extra == "dev" Provides-Extra: export Requires-
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
+Engineering :: Image Recognition Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
+:: Windows Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: matplotlib>=3.3.0 Requires-Dist: opencv-
+python>=4.6.0 Requires-Dist: pillow>=7.1.2 Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: requests>=2.23.0 Requires-Dist: scipy>=1.4.1 Requires-Dist:
+torch>=1.8.0 Requires-Dist: torchvision>=0.9.0 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: psutil Requires-Dist: py-cpuinfo Requires-Dist: thop>=0.1.1
+Requires-Dist: pandas>=1.1.4 Requires-Dist: seaborn>=0.11.0 Provides-Extra: dev
+Requires-Dist: ipython; extra == "dev" Requires-Dist: check-manifest; extra ==
+"dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: coverage[toml];
+extra == "dev" Requires-Dist: mkdocs-material>=9.5.9; extra == "dev" Requires-
+Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mkdocs-jupyter; extra
+== "dev" Requires-Dist: mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-
+ultralytics-plugin>=0.0.44; extra == "dev" Provides-Extra: export Requires-
 Dist: onnx>=1.12.0; extra == "export" Requires-Dist: coremltools>=7.0;
-platform_system != "Windows" and extra == "export" Requires-Dist: openvino-
-dev>=2023.0; extra == "export" Requires-Dist: tensorflow<=2.13.1; extra ==
-"export" Requires-Dist: tensorflowjs>=3.9.0; extra == "export" Provides-Extra:
-explorer Requires-Dist: lancedb; extra == "explorer" Requires-Dist: duckdb;
-extra == "explorer" Requires-Dist: streamlit; extra == "explorer" Provides-
-Extra: logging Requires-Dist: comet; extra == "logging" Requires-Dist:
-tensorboard>=2.13.0; extra == "logging" Requires-Dist: dvclive>=2.12.0; extra
-== "logging" Provides-Extra: extra Requires-Dist: hub-sdk>=0.0.2; extra ==
-"extra" Requires-Dist: ipython; extra == "extra" Requires-Dist:
-albumentations>=1.0.3; extra == "extra" Requires-Dist: pycocotools>=2.0.6;
-extra == "extra"
+(platform_system != "Windows" and python_version <= "3.11") and extra ==
+"export" Requires-Dist: openvino>=2024.0.0; extra == "export" Requires-Dist:
+tensorflow<=2.13.1; python_version <= "3.11" and extra == "export" Requires-
+Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra ==
+"export" Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra
+== "export" Provides-Extra: explorer Requires-Dist: lancedb; extra ==
+"explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer" Requires-Dist:
+streamlit; extra == "explorer" Provides-Extra: logging Requires-Dist: comet;
+extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra == "logging"
+Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra: extra
+Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython; extra
+== "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra" Requires-
+Dist: pycocotools>=2.0.7; extra == "extra"
                              _[_Y_O_L_O_ _V_i_s_i_o_n_ _b_a_n_n_e_r_]
        [ä¸­æ](https://docs.ultralytics.com/zh/) | [íêµ­ì´](https://
  docs.ultralytics.com/ko/) | [æ¥æ¬èª](https://docs.ultralytics.com/ja/) |
     [Ð ÑÑÑÐºÐ¸Ð¹](https://docs.ultralytics.com/ru/) | [Deutsch](https://
  docs.ultralytics.com/de/) | [FranÃ§ais](https://docs.ultralytics.com/fr/) |
      [EspaÃ±ol](https://docs.ultralytics.com/es/) | [PortuguÃªs](https://
 docs.ultralytics.com/pt/) | [à¤¹à¤¿à¤¨à¥à¤¦à¥](https://docs.ultralytics.com/
@@ -281,15 +284,15 @@
 v8.1.0/yolov8s-obb.pt) | 1024 | 79.5 | 424.88 | 4.07 | 11.4 | 76.3 | |
 [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/
 yolov8m-obb.pt) | 1024 | 80.5 | 763.48 | 7.61 | 26.4 | 208.6 | | [YOLOv8l-obb]
 (https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt)
 | 1024 | 80.7 | 1278.42 | 11.83 | 44.5 | 433.8 | | [YOLOv8x-obb](https://
 github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024 |
 81.36 | 1759.10 | 13.23 | 69.5 | 676.7 | - **mAPtest** values are for single-
-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
+model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
 dataset.
 Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit
 merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/
 evaluation.html). - **Speed** averaged over DOTAv1 val images using an [Amazon
 EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
 Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 Classification (ImageNet) See [Classification Docs](https://
```

### Comparing `ultralytics-8.1.9/README.md` & `ultralytics-8.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 | -------------------------------------------------------------------------------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8n-obb.pt) | 1024                  | 78.0               | 204.77                         | 3.57                                | 3.1                | 23.3              |
 | [YOLOv8s-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8s-obb.pt) | 1024                  | 79.5               | 424.88                         | 4.07                                | 11.4               | 76.3              |
 | [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8m-obb.pt) | 1024                  | 80.5               | 763.48                         | 7.61                                | 26.4               | 208.6             |
 | [YOLOv8l-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt) | 1024                  | 80.7               | 1278.42                        | 11.83                               | 44.5               | 433.8             |
 | [YOLOv8x-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024                  | 81.36              | 1759.10                        | 13.23                               | 69.5               | 676.7             |
 
-- **mAP<sup>test</sup>** values are for single-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
+- **mAP<sup>test</sup>** values are for single-model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
 - **Speed** averaged over DOTAv1 val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance. <br>Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification (ImageNet)</summary>
 
 See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models trained on [ImageNet](https://docs.ultralytics.com/datasets/classify/imagenet/), which include 1000 pretrained classes.
```

#### html2text {}

```diff
@@ -234,15 +234,15 @@
 v8.1.0/yolov8s-obb.pt) | 1024 | 79.5 | 424.88 | 4.07 | 11.4 | 76.3 | |
 [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/
 yolov8m-obb.pt) | 1024 | 80.5 | 763.48 | 7.61 | 26.4 | 208.6 | | [YOLOv8l-obb]
 (https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt)
 | 1024 | 80.7 | 1278.42 | 11.83 | 44.5 | 433.8 | | [YOLOv8x-obb](https://
 github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024 |
 81.36 | 1759.10 | 13.23 | 69.5 | 676.7 | - **mAPtest** values are for single-
-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
+model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
 dataset.
 Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit
 merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/
 evaluation.html). - **Speed** averaged over DOTAv1 val images using an [Amazon
 EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
 Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 Classification (ImageNet) See [Classification Docs](https://
```

### Comparing `ultralytics-8.1.9/pyproject.toml` & `ultralytics-8.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # For development purposes, you can install the package in editable mode with: 'pip install -e .'
 # This approach allows for real-time code modifications without the need for re-installation.
 
 # Documentation:
 # For comprehensive documentation and usage instructions, visit: https://docs.ultralytics.com
 
 [build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
+requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 # Project settings -----------------------------------------------------------------------------------------------------
 [project]
 name = "ultralytics"
 dynamic = ["version"]
 description = "Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification."
@@ -48,27 +48,27 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Recognition",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 
 # Required dependencies ------------------------------------------------------------------------------------------------
 dependencies = [
     "matplotlib>=3.3.0",
-    "numpy>=1.22.2",
     "opencv-python>=4.6.0",
     "pillow>=7.1.2",
     "pyyaml>=5.3.1",
     "requests>=2.23.0",
     "scipy>=1.4.1",
     "torch>=1.8.0",
     "torchvision>=0.9.0",
@@ -85,47 +85,49 @@
 dev = [
     "ipython",
     "check-manifest",
     "pre-commit",
     "pytest",
     "pytest-cov",
     "coverage[toml]",
-    "mkdocs-material",
+    "mkdocs-material>=9.5.9",
     "mkdocstrings[python]",
     "mkdocs-jupyter", # for notebooks
     "mkdocs-redirects", # for 301 redirects
-    "mkdocs-ultralytics-plugin>=0.0.42", # for meta descriptions and images, dates and authors
+    "mkdocs-ultralytics-plugin>=0.0.44", # for meta descriptions and images, dates and authors
 ]
 export = [
     "onnx>=1.12.0", # ONNX export
-    "coremltools>=7.0; platform_system != 'Windows'", # CoreML only supported on macOS and Linux
-    "openvino-dev>=2023.0", # OpenVINO export
-    "tensorflow<=2.13.1", # TF bug https://github.com/ultralytics/ultralytics/issues/5161
-    "tensorflowjs>=3.9.0", # TF.js export, automatically installs tensorflow
+    "coremltools>=7.0; platform_system != 'Windows' and python_version <= '3.11'", # CoreML supported on macOS and Linux
+    "openvino>=2024.0.0", # OpenVINO export
+    "tensorflow<=2.13.1; python_version <= '3.11'", # TF bug https://github.com/ultralytics/ultralytics/issues/5161
+    "tensorflowjs>=3.9.0; python_version <= '3.11'", # TF.js export, automatically installs tensorflow
+    # "flatbuffers>=23.5.26,<100", # update old 'flatbuffers' included inside tensorflow package: WARNING Dockerfile error https://github.com/ultralytics/ultralytics/actions/runs/8715942435/job/23908971614
+    "numpy==1.23.5; platform_machine == 'aarch64'", # fix error: `np.bool` was a deprecated alias for the builtin `bool` when using TensorRT models on NVIDIA Jetson
+    "h5py!=3.11.0; platform_machine == 'aarch64'", # fix h5py build issues due to missing aarch64 wheels in 3.11 release
 ]
 explorer = [
     "lancedb", # vector search
-    "duckdb", # SQL queries, supports lancedb tables
+    "duckdb<=0.9.2", # SQL queries, duckdb==0.10.0 bug https://github.com/ultralytics/ultralytics/pull/8181
     "streamlit", # visualizing with GUI
 ]
 # tensorflow>=2.4.1,<=2.13.1  # TF exports (-cpu, -aarch64, -macos)
 # tflite-support  # for TFLite model metadata
-# scikit-learn==0.19.2  # CoreML quantization
 # nvidia-pyindex  # TensorRT export
 # nvidia-tensorrt  # TensorRT export
 logging = [
     "comet", # https://docs.ultralytics.com/integrations/comet/
     "tensorboard>=2.13.0",
     "dvclive>=2.12.0",
 ]
 extra = [
-    "hub-sdk>=0.0.2", # Ultralytics HUB
+    "hub-sdk>=0.0.5", # Ultralytics HUB
     "ipython", # interactive notebook
     "albumentations>=1.0.3", # training augmentations
-    "pycocotools>=2.0.6", # COCO mAP
+    "pycocotools>=2.0.7", # COCO mAP
 ]
 
 [project.urls]
 "Bug Reports" = "https://github.com/ultralytics/ultralytics/issues"
 "Funding" = "https://ultralytics.com"
 "Source" = "https://github.com/ultralytics/ultralytics/"
 
@@ -137,17 +139,21 @@
 [tool.setuptools]  # configuration specific to the `setuptools` build backend.
 packages = { find = { where = ["."], include = ["ultralytics", "ultralytics.*"] } }
 package-data = { "ultralytics" = ["**/*.yaml"], "ultralytics.assets" = ["*.jpg"] }
 
 [tool.setuptools.dynamic]
 version = { attr = "ultralytics.__version__" }
 
-[tool.pytest]
-norecursedirs = [".git", "dist", "build"]
+[tool.pytest.ini_options]
 addopts = "--doctest-modules --durations=30 --color=yes"
+markers = [
+    "slow: skip slow tests unless --slow is set",
+]
+norecursedirs = [".git", "dist", "build"]
+
 
 [tool.coverage.run]
 source = ["ultralytics/"]
 data_file = "tests/.coverage"
 omit = ["ultralytics/utils/callbacks/*"]
 
 [tool.isort]
```

### Comparing `ultralytics-8.1.9/tests/test_cli.py` & `ultralytics-8.2.0/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 import pytest
 
-from ultralytics.utils import ASSETS, WEIGHTS_DIR
-from ultralytics.utils.checks import cuda_device_count, cuda_is_available
+from ultralytics.utils import ASSETS, WEIGHTS_DIR, checks
 
-CUDA_IS_AVAILABLE = cuda_is_available()
-CUDA_DEVICE_COUNT = cuda_device_count()
+CUDA_IS_AVAILABLE = checks.cuda_is_available()
+CUDA_DEVICE_COUNT = checks.cuda_device_count()
 TASK_ARGS = [
     ("detect", "yolov8n", "coco8.yaml"),
     ("segment", "yolov8n-seg", "coco8-seg.yaml"),
     ("classify", "yolov8n-cls", "imagenet10"),
     ("pose", "yolov8n-pose", "coco8-pose.yaml"),
     ("obb", "yolov8n-obb", "dota8.yaml"),
 ]  # (task, model, data)
@@ -62,18 +61,19 @@
     """Test exporting a YOLO model to different formats."""
     run(f"yolo export model={WEIGHTS_DIR / model}.pt format={format} imgsz=32")
 
 
 def test_rtdetr(task="detect", model="yolov8n-rtdetr.yaml", data="coco8.yaml"):
     """Test the RTDETR functionality with the Ultralytics framework."""
     # Warning: MUST use imgsz=640
-    run(f"yolo train {task} model={model} data={data} --imgsz= 640 epochs =1, cache = disk")  # add coma, spaces to args
-    run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=640 save save_crop save_txt")
+    run(f"yolo train {task} model={model} data={data} --imgsz= 160 epochs =1, cache = disk")  # add coma, spaces to args
+    run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=160 save save_crop save_txt")
 
 
+@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="MobileSAM with CLIP is not supported in Python 3.12")
 def test_fastsam(task="segment", model=WEIGHTS_DIR / "FastSAM-s.pt", data="coco8-seg.yaml"):
     """Test FastSAM segmentation functionality within Ultralytics."""
     source = ASSETS / "bus.jpg"
 
     run(f"yolo segment val {task} model={model} data={data} imgsz=32")
     run(f"yolo segment predict model={model} source={source} imgsz=32 save save_crop save_txt")
```

### Comparing `ultralytics-8.1.9/tests/test_cuda.py` & `ultralytics-8.2.0/tests/test_cuda.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 
 
 def test_checks():
     """Validate CUDA settings against torch CUDA functions."""
     assert torch.cuda.is_available() == CUDA_IS_AVAILABLE
     assert torch.cuda.device_count() == CUDA_DEVICE_COUNT
 
+@pytest.mark.slow
+@pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
+def test_export_engine():
+    """Test exporting the YOLO model to NVIDIA TensorRT format."""
+    f = YOLO(MODEL).export(format="engine", device=0)
+    YOLO(f)(BUS, device=0)
+
 
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 def test_train():
     """Test model training on a minimal dataset."""
     device = 0 if CUDA_DEVICE_COUNT == 1 else [0, 1]
     YOLO(MODEL).train(data=DATA, imgsz=64, epochs=1, device=device)  # requires imgsz>=64
```

### Comparing `ultralytics-8.1.9/tests/test_engine.py` & `ultralytics-8.2.0/tests/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
+import sys
+from unittest import mock
+
 from ultralytics import YOLO
 from ultralytics.cfg import get_cfg
 from ultralytics.engine.exporter import Exporter
 from ultralytics.models.yolo import classify, detect, segment
 from ultralytics.utils import ASSETS, DEFAULT_CFG, WEIGHTS_DIR
 
 CFG_DET = "yolov8n.yaml"
@@ -45,16 +48,18 @@
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = detect.DetectionPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
-    result = pred(source=ASSETS, model=f"{MODEL}.pt")
-    assert len(result), "predictor test failed"
+    # Confirm there is no issue with sys.argv being empty.
+    with mock.patch.object(sys, "argv", []):
+        result = pred(source=ASSETS, model=f"{MODEL}.pt")
+        assert len(result), "predictor test failed"
 
     overrides["resume"] = trainer.last
     trainer = detect.DetectionTrainer(overrides=overrides)
     try:
         trainer.train()
     except Exception as e:
         print(f"Expected exception caught: {e}")
```

### Comparing `ultralytics-8.1.9/tests/test_explorer.py` & `ultralytics-8.2.0/tests/test_explorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
+import PIL
+import pytest
+
 from ultralytics import Explorer
 from ultralytics.utils import ASSETS
 
-import PIL
-
 
+@pytest.mark.slow
 def test_similarity():
     """Test similarity calculations and SQL queries for correctness and response length."""
     exp = Explorer()
     exp.create_embeddings_table()
     similar = exp.get_similar(idx=1)
     assert len(similar) == 25
     similar = exp.get_similar(img=ASSETS / "zidane.jpg")
@@ -18,37 +20,40 @@
     assert len(similar) == 10
     sim_idx = exp.similarity_index()
     assert len(sim_idx) > 0
     sql = exp.sql_query("WHERE labels LIKE '%person%'")
     assert len(sql) > 0
 
 
+@pytest.mark.slow
 def test_det():
     """Test detection functionalities and ensure the embedding table has bounding boxes."""
     exp = Explorer(data="coco8.yaml", model="yolov8n.pt")
     exp.create_embeddings_table(force=True)
     assert len(exp.table.head()["bboxes"]) > 0
     similar = exp.get_similar(idx=[1, 2], limit=10)
     assert len(similar) > 0
     # This is a loose test, just checks errors not correctness
     similar = exp.plot_similar(idx=[1, 2], limit=10)
     assert isinstance(similar, PIL.Image.Image)
 
 
+@pytest.mark.slow
 def test_seg():
     """Test segmentation functionalities and verify the embedding table includes masks."""
     exp = Explorer(data="coco8-seg.yaml", model="yolov8n-seg.pt")
     exp.create_embeddings_table(force=True)
     assert len(exp.table.head()["masks"]) > 0
     similar = exp.get_similar(idx=[1, 2], limit=10)
     assert len(similar) > 0
     similar = exp.plot_similar(idx=[1, 2], limit=10)
     assert isinstance(similar, PIL.Image.Image)
 
 
+@pytest.mark.slow
 def test_pose():
     """Test pose estimation functionalities and check the embedding table for keypoints."""
     exp = Explorer(data="coco8-pose.yaml", model="yolov8n-pose.pt")
     exp.create_embeddings_table(force=True)
     assert len(exp.table.head()["keypoints"]) > 0
     similar = exp.get_similar(idx=[1, 2], limit=10)
     assert len(similar) > 0
```

### Comparing `ultralytics-8.1.9/tests/test_integrations.py` & `ultralytics-8.2.0/tests/test_integrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,46 +26,79 @@
 @pytest.mark.skipif(not check_requirements("mlflow", install=False), reason="mlflow not installed")
 def test_mlflow():
     """Test training with MLflow tracking enabled."""
     SETTINGS["mlflow"] = True
     YOLO("yolov8n-cls.yaml").train(data="imagenet10", imgsz=32, epochs=3, plots=False, device="cpu")
 
 
+@pytest.mark.skipif(True, reason="Test failing in scheduled CI https://github.com/ultralytics/ultralytics/pull/8868")
+@pytest.mark.skipif(not check_requirements("mlflow", install=False), reason="mlflow not installed")
+def test_mlflow_keep_run_active():
+    import os
+
+    import mlflow
+
+    """Test training with MLflow tracking enabled."""
+    SETTINGS["mlflow"] = True
+    run_name = "Test Run"
+    os.environ["MLFLOW_RUN"] = run_name
+
+    # Test with MLFLOW_KEEP_RUN_ACTIVE=True
+    os.environ["MLFLOW_KEEP_RUN_ACTIVE"] = "True"
+    YOLO("yolov8n-cls.yaml").train(data="imagenet10", imgsz=32, epochs=1, plots=False, device="cpu")
+    status = mlflow.active_run().info.status
+    assert status == "RUNNING", "MLflow run should be active when MLFLOW_KEEP_RUN_ACTIVE=True"
+
+    run_id = mlflow.active_run().info.run_id
+
+    # Test with MLFLOW_KEEP_RUN_ACTIVE=False
+    os.environ["MLFLOW_KEEP_RUN_ACTIVE"] = "False"
+    YOLO("yolov8n-cls.yaml").train(data="imagenet10", imgsz=32, epochs=1, plots=False, device="cpu")
+    status = mlflow.get_run(run_id=run_id).info.status
+    assert status == "FINISHED", "MLflow run should be ended when MLFLOW_KEEP_RUN_ACTIVE=False"
+
+    # Test with MLFLOW_KEEP_RUN_ACTIVE not set
+    os.environ.pop("MLFLOW_KEEP_RUN_ACTIVE", None)
+    YOLO("yolov8n-cls.yaml").train(data="imagenet10", imgsz=32, epochs=1, plots=False, device="cpu")
+    status = mlflow.get_run(run_id=run_id).info.status
+    assert status == "FINISHED", "MLflow run should be ended by default when MLFLOW_KEEP_RUN_ACTIVE is not set"
+
+
 @pytest.mark.skipif(not check_requirements("tritonclient", install=False), reason="tritonclient[all] not installed")
 def test_triton():
     """Test NVIDIA Triton Server functionalities."""
     check_requirements("tritonclient[all]")
     import subprocess
     import time
 
     from tritonclient.http import InferenceServerClient  # noqa
 
     # Create variables
     model_name = "yolo"
-    triton_repo_path = TMP / "triton_repo"
-    triton_model_path = triton_repo_path / model_name
+    triton_repo = TMP / "triton_repo"  # Triton repo path
+    triton_model = triton_repo / model_name  # Triton model path
 
     # Export model to ONNX
     f = YOLO(MODEL).export(format="onnx", dynamic=True)
 
     # Prepare Triton repo
-    (triton_model_path / "1").mkdir(parents=True, exist_ok=True)
-    Path(f).rename(triton_model_path / "1" / "model.onnx")
-    (triton_model_path / "config.pbtxt").touch()
+    (triton_model / "1").mkdir(parents=True, exist_ok=True)
+    Path(f).rename(triton_model / "1" / "model.onnx")
+    (triton_model / "config.pbtxt").touch()
 
     # Define image https://catalog.ngc.nvidia.com/orgs/nvidia/containers/tritonserver
     tag = "nvcr.io/nvidia/tritonserver:23.09-py3"  # 6.4 GB
 
     # Pull the image
     subprocess.call(f"docker pull {tag}", shell=True)
 
     # Run the Triton server and capture the container ID
     container_id = (
         subprocess.check_output(
-            f"docker run -d --rm -v {triton_repo_path}:/models -p 8000:8000 {tag} tritonserver --model-repository=/models",
+            f"docker run -d --rm -v {triton_repo}:/models -p 8000:8000 {tag} tritonserver --model-repository=/models",
             shell=True,
         )
         .decode("utf-8")
         .strip()
     )
 
     # Wait for the Triton server to start
```

### Comparing `ultralytics-8.1.9/tests/test_python.py` & `ultralytics-8.2.0/tests/test_python.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from copy import copy
 from pathlib import Path
 
 import cv2
 import numpy as np
 import pytest
 import torch
+import yaml
 from PIL import Image
-from torchvision.transforms import ToTensor
 
 from ultralytics import RTDETR, YOLO
 from ultralytics.cfg import TASK2DATA
 from ultralytics.data.build import load_inference_source
 from ultralytics.utils import (
     ASSETS,
     DEFAULT_CFG,
@@ -23,17 +23,18 @@
     ONLINE,
     ROOT,
     WEIGHTS_DIR,
     WINDOWS,
     Retry,
     checks,
     is_dir_writeable,
+    IS_RASPBERRYPI,
 )
 from ultralytics.utils.downloads import download
-from ultralytics.utils.torch_utils import TORCH_1_9
+from ultralytics.utils.torch_utils import TORCH_1_9, TORCH_1_13
 
 MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
 CFG = "yolov8n.yaml"
 SOURCE = ASSETS / "bus.jpg"
 TMP = (ROOT / "../tests/tmp").resolve()  # temp directory for test files
 IS_TMP_WRITEABLE = is_dir_writeable(TMP)
 
@@ -103,28 +104,25 @@
         cv2.imread(str(SOURCE)),  # OpenCV
         Image.open(SOURCE),  # PIL
         np.zeros((320, 640, 3)),
     ]  # numpy
     assert len(model(batch, imgsz=32)) == len(batch)  # multiple sources in a batch
 
     # Test tensor inference
-    im = cv2.imread(str(SOURCE))  # OpenCV
-    t = cv2.resize(im, (32, 32))
-    t = ToTensor()(t)
-    t = torch.stack([t, t, t, t])
-    results = model(t, imgsz=32)
-    assert len(results) == t.shape[0]
-    results = seg_model(t, imgsz=32)
-    assert len(results) == t.shape[0]
-    results = cls_model(t, imgsz=32)
-    assert len(results) == t.shape[0]
-    results = pose_model(t, imgsz=32)
-    assert len(results) == t.shape[0]
-    results = obb_model(t, imgsz=32)
-    assert len(results) == t.shape[0]
+    im = torch.rand((4, 3, 32, 32))  # batch-size 4, FP32 0.0-1.0 RGB order
+    results = model(im, imgsz=32)
+    assert len(results) == im.shape[0]
+    results = seg_model(im, imgsz=32)
+    assert len(results) == im.shape[0]
+    results = cls_model(im, imgsz=32)
+    assert len(results) == im.shape[0]
+    results = pose_model(im, imgsz=32)
+    assert len(results) == im.shape[0]
+    results = obb_model(im, imgsz=32)
+    assert len(results) == im.shape[0]
 
 
 def test_predict_grey_and_4ch():
     """Test YOLO prediction on SOURCE converted to greyscale and 4-channel images."""
     im = Image.open(SOURCE)
     directory = TMP / "im4"
     directory.mkdir(parents=True, exist_ok=True)
@@ -165,16 +163,14 @@
 @pytest.mark.skipif(not IS_TMP_WRITEABLE, reason="directory is not writeable")
 def test_track_stream():
     """
     Test streaming tracking (short 10 frame video) with non-default ByteTrack tracker.
 
     Note imgsz=160 required for tracking for higher confidence and better matches
     """
-    import yaml
-
     video_url = "https://ultralytics.com/assets/decelera_portrait_min.mov"
     model = YOLO(MODEL)
     model.track(video_url, imgsz=160, tracker="bytetrack.yaml")
     model.track(video_url, imgsz=160, tracker="botsort.yaml", save_frames=True)  # test frame saving also
 
     # Test Global Motion Compensation (GMC) methods
     for gmc in "orb", "sift", "ecc":
@@ -214,28 +210,32 @@
 
 def test_export_onnx():
     """Test exporting the YOLO model to ONNX format."""
     f = YOLO(MODEL).export(format="onnx", dynamic=True)
     YOLO(f)(SOURCE)  # exported model inference
 
 
+@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="OpenVINO not supported in Python 3.12")
+@pytest.mark.skipif(not TORCH_1_13, reason="OpenVINO requires torch>=1.13")
 def test_export_openvino():
     """Test exporting the YOLO model to OpenVINO format."""
     f = YOLO(MODEL).export(format="openvino")
     YOLO(f)(SOURCE)  # exported model inference
 
 
+@pytest.mark.skipif(WINDOWS, reason="CoreML not supported on Windows")  # RuntimeError: BlobWriter not loaded
+@pytest.mark.skipif(IS_RASPBERRYPI, reason="CoreML not supported on Raspberry Pi")
+@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="CoreML not supported in Python 3.12")
 def test_export_coreml():
     """Test exporting the YOLO model to CoreML format."""
-    if not WINDOWS:  # RuntimeError: BlobWriter not loaded with coremltools 7.0 on windows
-        if MACOS:
-            f = YOLO(MODEL).export(format="coreml")
-            YOLO(f)(SOURCE)  # model prediction only supported on macOS for nms=False models
-        else:
-            YOLO(MODEL).export(format="coreml", nms=True)
+    if MACOS:
+        f = YOLO(MODEL).export(format="coreml")
+        YOLO(f)(SOURCE)  # model prediction only supported on macOS for nms=False models
+    else:
+        YOLO(MODEL).export(format="coreml", nms=True)
 
 
 def test_export_tflite(enabled=False):
     """
     Test exporting the YOLO model to TFLite format.
 
     Note TF suffers from install conflicts on Windows and macOS.
@@ -295,15 +295,15 @@
 
 
 def test_predict_callback_and_setup():
     """Test callback functionality during YOLO prediction."""
 
     def on_predict_batch_end(predictor):
         """Callback function that handles operations at the end of a prediction batch."""
-        path, im0s, _, _ = predictor.batch
+        path, im0s, _ = predictor.batch
         im0s = im0s if isinstance(im0s, list) else [im0s]
         bs = [predictor.dataset.bs for _ in range(len(path))]
         predictor.results = zip(predictor.results, im0s, bs)  # results is List[batch_size]
 
     model = YOLO(MODEL)
     model.add_callback("on_predict_batch_end", on_predict_batch_end)
 
@@ -328,14 +328,36 @@
             r.save_crop(save_dir=TMP / "runs/tests/crops/")
             r.tojson(normalize=True)
             r.plot(pil=True)
             r.plot(conf=True, boxes=True)
             print(r, len(r), r.path)
 
 
+def test_labels_and_crops():
+    """Test output from prediction args for saving detection labels and crops."""
+    imgs = [SOURCE, ASSETS / "zidane.jpg"]
+    results = YOLO(WEIGHTS_DIR / "yolov8n.pt")(imgs, imgsz=160, save_txt=True, save_crop=True)
+    save_path = Path(results[0].save_dir)
+    for r in results:
+        im_name = Path(r.path).stem
+        cls_idxs = r.boxes.cls.int().tolist()
+        # Check label path
+        labels = save_path / f"labels/{im_name}.txt"
+        assert labels.exists()
+        # Check detections match label count
+        assert len(r.boxes.data) == len([l for l in labels.read_text().splitlines() if l])
+        # Check crops path and files
+        crop_dirs = [p for p in (save_path / "crops").iterdir()]
+        crop_files = [f for p in crop_dirs for f in p.glob("*")]
+        # Crop directories match detections
+        assert all([r.names.get(c) in {d.name for d in crop_dirs} for c in cls_idxs])
+        # Same number of crops as detections
+        assert len([f for f in crop_files if im_name in f.name]) == len(r.boxes.data)
+
+
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
 def test_data_utils():
     """Test utility functions in ultralytics/data/utils.py."""
     from ultralytics.data.utils import HUBDatasetStats, autosplit
     from ultralytics.utils.downloads import zip_directory
 
     # from ultralytics.utils.files import WorkingDirectory
@@ -435,14 +457,15 @@
     m = Conv(64, 64, k=1, s=2)
 
     profile(x, [m], n=3)
     get_flops_with_torch_profiler(m)
     time_sync()
 
 
+@pytest.mark.slow
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
 def test_utils_downloads():
     """Test file download utilities."""
     from ultralytics.utils.downloads import get_google_drive_file_info
 
     get_google_drive_file_info("https://drive.google.com/file/d/1cqT-cJgANNrhIHCrEufUYhQ4RqiWG_lJ/view?usp=drive_link")
 
@@ -489,15 +512,16 @@
     with spaces_in_path(path) as new_path:
         print(new_path)
 
 
 @pytest.mark.slow
 def test_utils_patches_torch_save():
     """Test torch_save backoff when _torch_save throws RuntimeError."""
-    from unittest.mock import patch, MagicMock
+    from unittest.mock import MagicMock, patch
+
     from ultralytics.utils.patches import torch_save
 
     mock = MagicMock(side_effect=RuntimeError)
 
     with patch("ultralytics.utils.patches._torch_save", new=mock):
         with pytest.raises(RuntimeError):
             torch_save(torch.zeros(1), TMP / "test.pt")
@@ -548,29 +572,29 @@
     export_fmts_hub()
     logout()
     smart_request("GET", "https://github.com", progress=True)
 
 
 @pytest.fixture
 def image():
+    """Loads an image from a predefined source using OpenCV."""
     return cv2.imread(str(SOURCE))
 
 
 @pytest.mark.parametrize(
     "auto_augment, erasing, force_color_jitter",
     [
         (None, 0.0, False),
         ("randaugment", 0.5, True),
         ("augmix", 0.2, False),
         ("autoaugment", 0.0, True),
     ],
 )
 def test_classify_transforms_train(image, auto_augment, erasing, force_color_jitter):
-    import torchvision.transforms as T
-
+    """Tests classification transforms during training with various augmentation settings."""
     from ultralytics.data.augment import classify_augmentations
 
     transform = classify_augmentations(
         size=224,
         mean=(0.5, 0.5, 0.5),
         std=(0.5, 0.5, 0.5),
         scale=(0.08, 1.0),
@@ -579,15 +603,14 @@
         vflip=0.5,
         auto_augment=auto_augment,
         hsv_h=0.015,
         hsv_s=0.4,
         hsv_v=0.4,
         force_color_jitter=force_color_jitter,
         erasing=erasing,
-        interpolation=T.InterpolationMode.BILINEAR,
     )
 
     transformed_image = transform(Image.fromarray(cv2.cvtColor(image, cv2.COLOR_BGR2RGB)))
 
     assert transformed_image.shape == (3, 224, 224)
     assert torch.is_tensor(transformed_image)
     assert transformed_image.dtype == torch.float32
@@ -605,7 +628,39 @@
     """Test YOLO model embeddings."""
     model_detect = YOLO(MODEL)
     model_segment = YOLO(WEIGHTS_DIR / "yolov8n-seg.pt")
 
     for batch in [SOURCE], [SOURCE, SOURCE]:  # test batch size 1 and 2
         assert len(model_detect.embed(source=batch, imgsz=32)) == len(batch)
         assert len(model_segment.embed(source=batch, imgsz=32)) == len(batch)
+
+
+@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
+def test_yolo_world():
+    model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
+    model.set_classes(["tree", "window"])
+    model(ASSETS / "bus.jpg", conf=0.01)
+
+    # Training from yaml
+    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
+    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
+
+    model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
+    # val
+    model.val(data="coco8.yaml", imgsz=32, save_txt=True, save_json=True)
+    # Training from pretrain
+    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
+
+    # test WorWorldTrainerFromScratch
+    from ultralytics.models.yolo.world.train_world import WorldTrainerFromScratch
+
+    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
+    model.train(
+        data={"train": {"yolo_data": ["coco8.yaml"]}, "val": {"yolo_data": ["coco8.yaml"]}},
+        epochs=2,
+        imgsz=32,
+        cache="disk",
+        batch=-1,
+        close_mosaic=1,
+        name="yolo-world",
+        trainer=WorldTrainerFromScratch,
+    )
```

### Comparing `ultralytics-8.1.9/ultralytics/__init__.py` & `ultralytics-8.2.0/ultralytics/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.1.9"
+__version__ = "8.2.0"
 
 from ultralytics.data.explorer.explorer import Explorer
-from ultralytics.models import RTDETR, SAM, YOLO
+from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
-from ultralytics.utils import ASSETS, SETTINGS as settings
+from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
 from ultralytics.utils.downloads import download
 
+settings = SETTINGS
 __all__ = (
     "__version__",
     "ASSETS",
     "YOLO",
+    "YOLOWorld",
     "NAS",
     "SAM",
     "FastSAM",
     "RTDETR",
     "checks",
     "download",
     "settings",
```

### Comparing `ultralytics-8.1.9/ultralytics/assets/bus.jpg` & `ultralytics-8.2.0/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.0/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/__init__.py` & `ultralytics-8.2.0/ultralytics/cfg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     colorstr,
     deprecation_warn,
     yaml_load,
     yaml_print,
 )
 
 # Define valid tasks and modes
-MODES = "train", "val", "predict", "export", "track", "benchmark"
-TASKS = "detect", "segment", "classify", "pose", "obb"
+MODES = {"train", "val", "predict", "export", "track", "benchmark"}
+TASKS = {"detect", "segment", "classify", "pose", "obb"}
 TASK2DATA = {
     "detect": "coco8.yaml",
     "segment": "coco8-seg.yaml",
     "classify": "imagenet10",
     "pose": "coco8-pose.yaml",
     "obb": "dota8.yaml",
 }
@@ -50,16 +50,17 @@
     "detect": "metrics/mAP50-95(B)",
     "segment": "metrics/mAP50-95(M)",
     "classify": "metrics/accuracy_top1",
     "pose": "metrics/mAP50-95(P)",
     "obb": "metrics/mAP50-95(B)",
 }
 
+ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 CLI_HELP_MSG = f"""
-    Arguments received: {str(['yolo'] + sys.argv[1:])}. Ultralytics 'yolo' commands use the following syntax:
+    Arguments received: {str(['yolo'] + ARGV[1:])}. Ultralytics 'yolo' commands use the following syntax:
 
         yolo TASK MODE ARGS
 
         Where   TASK (optional) is one of {TASKS}
                 MODE (required) is one of {MODES}
                 ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                     See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
@@ -89,16 +90,16 @@
 
     Docs: https://docs.ultralytics.com
     Community: https://community.ultralytics.com
     GitHub: https://github.com/ultralytics/ultralytics
     """
 
 # Define keys for arg type checks
-CFG_FLOAT_KEYS = "warmup_epochs", "box", "cls", "dfl", "degrees", "shear", "time"
-CFG_FRACTION_KEYS = (
+CFG_FLOAT_KEYS = {"warmup_epochs", "box", "cls", "dfl", "degrees", "shear", "time", "workspace"}
+CFG_FRACTION_KEYS = {
     "dropout",
     "iou",
     "lr0",
     "lrf",
     "momentum",
     "weight_decay",
     "warmup_momentum",
@@ -108,37 +109,37 @@
     "hsv_s",
     "hsv_v",
     "translate",
     "scale",
     "perspective",
     "flipud",
     "fliplr",
+    "bgr",
     "mosaic",
     "mixup",
     "copy_paste",
     "conf",
     "iou",
     "fraction",
-)  # fraction floats 0.0 - 1.0
-CFG_INT_KEYS = (
+}  # fraction floats 0.0 - 1.0
+CFG_INT_KEYS = {
     "epochs",
     "patience",
     "batch",
     "workers",
     "seed",
     "close_mosaic",
     "mask_ratio",
     "max_det",
     "vid_stride",
     "line_width",
-    "workspace",
     "nbs",
     "save_period",
-)
-CFG_BOOL_KEYS = (
+}
+CFG_BOOL_KEYS = {
     "save",
     "exist_ok",
     "verbose",
     "deterministic",
     "single_cls",
     "rect",
     "cos_lr",
@@ -165,15 +166,15 @@
     "optimize",
     "int8",
     "dynamic",
     "simplify",
     "nms",
     "profile",
     "multi_scale",
-)
+}
 
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Args:
@@ -215,54 +216,67 @@
         if k in cfg and isinstance(cfg[k], (int, float)):
             cfg[k] = str(cfg[k])
     if cfg.get("name") == "model":  # assign model to 'name' arg
         cfg["name"] = cfg.get("model", "").split(".")[0]
         LOGGER.warning(f"WARNING ⚠️ 'name=model' automatically updated to 'name={cfg['name']}'.")
 
     # Type and Value checks
+    check_cfg(cfg)
+
+    # Return instance
+    return IterableSimpleNamespace(**cfg)
+
+
+def check_cfg(cfg, hard=True):
+    """Check Ultralytics configuration argument types and values."""
     for k, v in cfg.items():
         if v is not None:  # None values may be from optional args
             if k in CFG_FLOAT_KEYS and not isinstance(v, (int, float)):
-                raise TypeError(
-                    f"'{k}={v}' is of invalid type {type(v).__name__}. "
-                    f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
-                )
-            elif k in CFG_FRACTION_KEYS:
-                if not isinstance(v, (int, float)):
+                if hard:
                     raise TypeError(
                         f"'{k}={v}' is of invalid type {type(v).__name__}. "
                         f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
                     )
+                cfg[k] = float(v)
+            elif k in CFG_FRACTION_KEYS:
+                if not isinstance(v, (int, float)):
+                    if hard:
+                        raise TypeError(
+                            f"'{k}={v}' is of invalid type {type(v).__name__}. "
+                            f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
+                        )
+                    cfg[k] = v = float(v)
                 if not (0.0 <= v <= 1.0):
                     raise ValueError(f"'{k}={v}' is an invalid value. " f"Valid '{k}' values are between 0.0 and 1.0.")
             elif k in CFG_INT_KEYS and not isinstance(v, int):
-                raise TypeError(
-                    f"'{k}={v}' is of invalid type {type(v).__name__}. " f"'{k}' must be an int (i.e. '{k}=8')"
-                )
+                if hard:
+                    raise TypeError(
+                        f"'{k}={v}' is of invalid type {type(v).__name__}. " f"'{k}' must be an int (i.e. '{k}=8')"
+                    )
+                cfg[k] = int(v)
             elif k in CFG_BOOL_KEYS and not isinstance(v, bool):
-                raise TypeError(
-                    f"'{k}={v}' is of invalid type {type(v).__name__}. "
-                    f"'{k}' must be a bool (i.e. '{k}=True' or '{k}=False')"
-                )
-
-    # Return instance
-    return IterableSimpleNamespace(**cfg)
+                if hard:
+                    raise TypeError(
+                        f"'{k}={v}' is of invalid type {type(v).__name__}. "
+                        f"'{k}' must be a bool (i.e. '{k}=True' or '{k}=False')"
+                    )
+                cfg[k] = bool(v)
 
 
 def get_save_dir(args, name=None):
     """Return save_dir as created from train/val/predict arguments."""
 
     if getattr(args, "save_dir", None):
         save_dir = args.save_dir
     else:
         from ultralytics.utils.files import increment_path
 
         project = args.project or (ROOT.parent / "tests/tmp/runs" if TESTS_RUNNING else RUNS_DIR) / args.task
         name = name or args.name or f"{args.mode}"
-        save_dir = increment_path(Path(project) / name, exist_ok=args.exist_ok if RANK in (-1, 0) else True)
+        save_dir = increment_path(Path(project) / name, exist_ok=args.exist_ok if RANK in {-1, 0} else True)
 
     return Path(save_dir)
 
 
 def _handle_deprecation(custom):
     """Hardcoded function to handle deprecated config keys."""
 
@@ -392,15 +406,15 @@
     except Exception as e:
         LOGGER.warning(f"WARNING ⚠️ settings error: '{e}'. Please see {url} for help.")
 
 
 def handle_explorer():
     """Open the Ultralytics Explorer GUI."""
     checks.check_requirements("streamlit")
-    LOGGER.info(f"💡 Loading Explorer dashboard...")
+    LOGGER.info("💡 Loading Explorer dashboard...")
     subprocess.run(["streamlit", "run", ROOT / "data/explorer/gui/dash.py", "--server.maxMessageSize", "2048"])
 
 
 def parse_key_value_pair(pair):
     """Parse one 'key=value' pair and return key and value."""
     k, v = pair.split("=", 1)  # split on first '=' sign
     k, v = k.strip(), v.strip()  # remove spaces
@@ -434,15 +448,15 @@
     - specifying the mode, either 'train', 'val', 'test', or 'predict'
     - running special modes like 'checks'
     - passing overrides to the package's configuration
 
     It uses the package's default cfg and initializes it using the passed overrides.
     Then it calls the CLI function with the composed cfg
     """
-    args = (debug.split(" ") if debug else sys.argv)[1:]
+    args = (debug.split(" ") if debug else ARGV)[1:]
     if not args:  # no arguments passed
         LOGGER.info(CLI_HELP_MSG)
         return
 
     special = {
         "help": lambda: LOGGER.info(CLI_HELP_MSG),
         "checks": checks.collect_system_info,
@@ -460,18 +474,18 @@
     special.update({k[0]: v for k, v in special.items()})  # singular
     special.update({k[:-1]: v for k, v in special.items() if len(k) > 1 and k.endswith("s")})  # singular
     special = {**special, **{f"-{k}": v for k, v in special.items()}, **{f"--{k}": v for k, v in special.items()}}
 
     overrides = {}  # basic overrides, i.e. imgsz=320
     for a in merge_equals_args(args):  # merge spaces around '=' sign
         if a.startswith("--"):
-            LOGGER.warning(f"WARNING ⚠️ '{a}' does not require leading dashes '--', updating to '{a[2:]}'.")
+            LOGGER.warning(f"WARNING ⚠️ argument '{a}' does not require leading dashes '--', updating to '{a[2:]}'.")
             a = a[2:]
         if a.endswith(","):
-            LOGGER.warning(f"WARNING ⚠️ '{a}' does not require trailing comma ',', updating to '{a[:-1]}'.")
+            LOGGER.warning(f"WARNING ⚠️ argument '{a}' does not require trailing comma ',', updating to '{a[:-1]}'.")
             a = a[:-1]
         if "=" in a:
             try:
                 k, v = parse_key_value_pair(a)
                 if k == "cfg" and v is not None:  # custom.yaml passed
                     LOGGER.info(f"Overriding {DEFAULT_CFG_PATH} with {v}")
                     overrides = {k: val for k, val in yaml_load(checks.check_yaml(v)).items() if k != "cfg"}
@@ -500,15 +514,15 @@
     # Check keys
     check_dict_alignment(full_args_dict, overrides)
 
     # Mode
     mode = overrides.get("mode")
     if mode is None:
         mode = DEFAULT_CFG.mode or "predict"
-        LOGGER.warning(f"WARNING ⚠️ 'mode' is missing. Valid modes are {MODES}. Using default 'mode={mode}'.")
+        LOGGER.warning(f"WARNING ⚠️ 'mode' argument is missing. Valid modes are {MODES}. Using default 'mode={mode}'.")
     elif mode not in MODES:
         raise ValueError(f"Invalid 'mode={mode}'. Valid modes are {MODES}.\n{CLI_HELP_MSG}")
 
     # Task
     task = overrides.pop("task", None)
     if task:
         if task not in TASKS:
@@ -516,15 +530,15 @@
         if "model" not in overrides:
             overrides["model"] = TASK2MODEL[task]
 
     # Model
     model = overrides.pop("model", DEFAULT_CFG.model)
     if model is None:
         model = "yolov8n.pt"
-        LOGGER.warning(f"WARNING ⚠️ 'model' is missing. Using default 'model={model}'.")
+        LOGGER.warning(f"WARNING ⚠️ 'model' argument is missing. Using default 'model={model}'.")
     overrides["model"] = model
     stem = Path(model).stem.lower()
     if "rtdetr" in stem:  # guess architecture
         from ultralytics import RTDETR
 
         model = RTDETR(model)  # no task argument
     elif "fastsam" in stem:
@@ -548,25 +562,25 @@
             LOGGER.warning(
                 f"WARNING ⚠️ conflicting 'task={task}' passed with 'task={model.task}' model. "
                 f"Ignoring 'task={task}' and updating to 'task={model.task}' to match model."
             )
         task = model.task
 
     # Mode
-    if mode in ("predict", "track") and "source" not in overrides:
+    if mode in {"predict", "track"} and "source" not in overrides:
         overrides["source"] = DEFAULT_CFG.source or ASSETS
-        LOGGER.warning(f"WARNING ⚠️ 'source' is missing. Using default 'source={overrides['source']}'.")
-    elif mode in ("train", "val"):
+        LOGGER.warning(f"WARNING ⚠️ 'source' argument is missing. Using default 'source={overrides['source']}'.")
+    elif mode in {"train", "val"}:
         if "data" not in overrides and "resume" not in overrides:
             overrides["data"] = DEFAULT_CFG.data or TASK2DATA.get(task or DEFAULT_CFG.task, DEFAULT_CFG.data)
-            LOGGER.warning(f"WARNING ⚠️ 'data' is missing. Using default 'data={overrides['data']}'.")
+            LOGGER.warning(f"WARNING ⚠️ 'data' argument is missing. Using default 'data={overrides['data']}'.")
     elif mode == "export":
         if "format" not in overrides:
             overrides["format"] = DEFAULT_CFG.format or "torchscript"
-            LOGGER.warning(f"WARNING ⚠️ 'format' is missing. Using default 'format={overrides['format']}'.")
+            LOGGER.warning(f"WARNING ⚠️ 'format' argument is missing. Using default 'format={overrides['format']}'.")
 
     # Run command in python
     getattr(model, mode)(**overrides)  # default args from model
 
     # Show help
     LOGGER.info(f"💡 Learn more at https://docs.ultralytics.com/modes/{mode}")
```

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.0/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/default.yaml` & `ultralytics-8.2.0/ultralytics/cfg/default.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 mode: train # (str) YOLO mode, i.e. train, val, predict, export, track, benchmark
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: # (str, optional) path to model file, i.e. yolov8n.pt, yolov8n.yaml
 data: # (str, optional) path to data file, i.e. coco128.yaml
 epochs: 100 # (int) number of epochs to train for
 time: # (float, optional) number of hours to train for, overrides epochs if supplied
-patience: 50 # (int) epochs to wait for no observable improvement for early stopping of training
+patience: 100 # (int) epochs to wait for no observable improvement for early stopping of training
 batch: 16 # (int) number of images per batch (-1 for AutoBatch)
 imgsz: 640 # (int | list) input images size as int for train and val modes, or list[w,h] for predict and export modes
 save: True # (bool) save train checkpoints and predict results
 save_period: -1 # (int) Save checkpoint every x epochs (disabled if < 1)
 cache: False # (bool) True/ram, disk or False. Use cache for data loading
 device: # (int | str | list, optional) device to run on, i.e. cuda device=0 or device=0,1,2,3 or device=cpu
 workers: 8 # (int) number of worker threads for data loading (per RANK if DDP)
@@ -30,15 +30,15 @@
 cos_lr: False # (bool) use cosine learning rate scheduler
 close_mosaic: 10 # (int) disable mosaic augmentation for final epochs (0 to disable)
 resume: False # (bool) resume training from last checkpoint
 amp: True # (bool) Automatic Mixed Precision (AMP) training, choices=[True, False], True runs AMP check
 fraction: 1.0 # (float) dataset fraction to train on (default is 1.0, all images in train set)
 profile: False # (bool) profile ONNX and TensorRT speeds during training for loggers
 freeze: None # (int | list, optional) freeze first n layers, or freeze list of layer indices during training
-multi_scale: False # (bool) Whether to use multi-scale during training
+multi_scale: False # (bool) Whether to use multiscale during training
 # Segmentation
 overlap_mask: True # (bool) masks should overlap during training (segment train only)
 mask_ratio: 4 # (int) mask downsample ratio (segment train only)
 # Classification
 dropout: 0.0 # (float) use dropout regularization (classify train only)
 
 # Val/Test settings ----------------------------------------------------------------------------------------------------
@@ -107,19 +107,20 @@
 degrees: 0.0 # (float) image rotation (+/- deg)
 translate: 0.1 # (float) image translation (+/- fraction)
 scale: 0.5 # (float) image scale (+/- gain)
 shear: 0.0 # (float) image shear (+/- deg)
 perspective: 0.0 # (float) image perspective (+/- fraction), range 0-0.001
 flipud: 0.0 # (float) image flip up-down (probability)
 fliplr: 0.5 # (float) image flip left-right (probability)
+bgr: 0.0 # (float) image channel BGR (probability)
 mosaic: 1.0 # (float) image mosaic (probability)
 mixup: 0.0 # (float) image mixup (probability)
 copy_paste: 0.0 # (float) segment copy-paste (probability)
 auto_augment: randaugment # (str) auto augmentation policy for classification (randaugment, autoaugment, augmix)
-erasing: 0.4 # (float) probability of random erasing during classification training (0-1)
-crop_fraction: 1.0 # (float) image crop fraction for classification evaluation/inference (0-1)
+erasing: 0.4 # (float) probability of random erasing during classification training (0-0.9), 0 means no erasing, must be less than 1.0.
+crop_fraction: 1.0 # (float) image crop fraction for classification (0.1-1), 1.0 means no crop, must be greater than 0.
 
 # Custom config.yaml ---------------------------------------------------------------------------------------------------
 cfg: # (str, optional) for overriding defaults.yaml
 
 # Tracker settings ------------------------------------------------------------------------------------------------------
 tracker: botsort.yaml # (str) tracker type, choices=[botsort.yaml, bytetrack.yaml]
```

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.0/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.0/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.0/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/data/annotator.py` & `ultralytics-8.2.0/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/data/augment.py` & `ultralytics-8.2.0/ultralytics/data/augment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import random
 from copy import deepcopy
+from typing import Tuple, Union
 
 import cv2
 import numpy as np
 import torch
-import torchvision.transforms as T
+from PIL import Image
 
 from ultralytics.utils import LOGGER, colorstr
 from ultralytics.utils.checks import check_version
 from ultralytics.utils.instance import Instances
 from ultralytics.utils.metrics import bbox_ioa
 from ultralytics.utils.ops import segment2box, xyxyxyxy2xywhr
 from ultralytics.utils.torch_utils import TORCHVISION_0_10, TORCHVISION_0_11, TORCHVISION_0_13
+
 from .utils import polygons2masks, polygons2masks_overlap
 
 DEFAULT_MEAN = (0.0, 0.0, 0.0)
 DEFAULT_STD = (1.0, 1.0, 1.0)
-DEFAULT_CROP_FTACTION = 1.0
+DEFAULT_CROP_FRACTION = 1.0
 
 
 # TODO: we might need a BaseTransform to make all these augments be compatible with both classification and semantic
 class BaseTransform:
     """
     Base class for image transformations.
 
@@ -62,26 +64,49 @@
 
 
 class Compose:
     """Class for composing multiple image transformations."""
 
     def __init__(self, transforms):
         """Initializes the Compose object with a list of transforms."""
-        self.transforms = transforms
+        self.transforms = transforms if isinstance(transforms, list) else [transforms]
 
     def __call__(self, data):
         """Applies a series of transformations to input data."""
         for t in self.transforms:
             data = t(data)
         return data
 
     def append(self, transform):
         """Appends a new transform to the existing list of transforms."""
         self.transforms.append(transform)
 
+    def insert(self, index, transform):
+        """Inserts a new transform to the existing list of transforms."""
+        self.transforms.insert(index, transform)
+
+    def __getitem__(self, index: Union[list, int]) -> "Compose":
+        """Retrieve a specific transform or a set of transforms using indexing."""
+        assert isinstance(index, (int, list)), f"The indices should be either list or int type but got {type(index)}"
+        index = [index] if isinstance(index, int) else index
+        return Compose([self.transforms[i] for i in index])
+
+    def __setitem__(self, index: Union[list, int], value: Union[list, int]) -> None:
+        """Retrieve a specific transform or a set of transforms using indexing."""
+        assert isinstance(index, (int, list)), f"The indices should be either list or int type but got {type(index)}"
+        if isinstance(index, list):
+            assert isinstance(
+                value, list
+            ), f"The indices should be the same type as values, but got {type(index)} and {type(value)}"
+        if isinstance(index, int):
+            index, value = [index], [value]
+        for i, v in zip(index, value):
+            assert i < len(self.transforms), f"list index {i} out of range {len(self.transforms)}."
+            self.transforms[i] = v
+
     def tolist(self):
         """Converts the list of transforms to a standard Python list."""
         return self.transforms
 
     def __repr__(self):
         """Returns a string representation of the object."""
         return f"{self.__class__.__name__}({', '.join([f'{t}' for t in self.transforms])})"
@@ -114,27 +139,45 @@
         mix_labels = [self.dataset.get_image_and_label(i) for i in indexes]
 
         if self.pre_transform is not None:
             for i, data in enumerate(mix_labels):
                 mix_labels[i] = self.pre_transform(data)
         labels["mix_labels"] = mix_labels
 
+        # Update cls and texts
+        labels = self._update_label_text(labels)
         # Mosaic or MixUp
         labels = self._mix_transform(labels)
         labels.pop("mix_labels", None)
         return labels
 
     def _mix_transform(self, labels):
         """Applies MixUp or Mosaic augmentation to the label dictionary."""
         raise NotImplementedError
 
     def get_indexes(self):
         """Gets a list of shuffled indexes for mosaic augmentation."""
         raise NotImplementedError
 
+    def _update_label_text(self, labels):
+        """Update label text."""
+        if "texts" not in labels:
+            return labels
+
+        mix_texts = sum([labels["texts"]] + [x["texts"] for x in labels["mix_labels"]], [])
+        mix_texts = list({tuple(x) for x in mix_texts})
+        text2id = {text: i for i, text in enumerate(mix_texts)}
+
+        for label in [labels] + labels["mix_labels"]:
+            for i, cls in enumerate(label["cls"].squeeze(-1).tolist()):
+                text = label["texts"][int(cls)]
+                label["cls"][i] = text2id[tuple(text)]
+            label["texts"] = mix_texts
+        return labels
+
 
 class Mosaic(BaseMixTransform):
     """
     Mosaic augmentation.
 
     This class performs mosaic augmentation by combining multiple (4 or 9) images into a single mosaic image.
     The augmentation is applied to a dataset with a given probability.
@@ -145,15 +188,15 @@
         p (float, optional): Probability of applying the mosaic augmentation. Must be in the range 0-1. Default to 1.0.
         n (int, optional): The grid size, either 4 (for 2x2) or 9 (for 3x3).
     """
 
     def __init__(self, dataset, imgsz=640, p=1.0, n=4):
         """Initializes the object with a dataset, image size, probability, and border."""
         assert 0 <= p <= 1.0, f"The probability should be in range [0, 1], but got {p}."
-        assert n in (4, 9), "grid must be equal to 4 or 9."
+        assert n in {4, 9}, "grid must be equal to 4 or 9."
         super().__init__(dataset=dataset, p=p)
         self.dataset = dataset
         self.imgsz = imgsz
         self.border = (-imgsz // 2, -imgsz // 2)  # width, height
         self.n = n
 
     def get_indexes(self, buffer=True):
@@ -316,14 +359,16 @@
             "cls": np.concatenate(cls, 0),
             "instances": Instances.concatenate(instances, axis=0),
             "mosaic_border": self.border,
         }
         final_labels["instances"].clip(imgsz, imgsz)
         good = final_labels["instances"].remove_zero_area_boxes()
         final_labels["cls"] = final_labels["cls"][good]
+        if "texts" in mosaic_labels[0]:
+            final_labels["texts"] = mosaic_labels[0]["texts"]
         return final_labels
 
 
 class MixUp(BaseMixTransform):
     """Class for applying MixUp augmentation to the dataset."""
 
     def __init__(self, dataset, pre_transform=None, p=0.0) -> None:
@@ -637,15 +682,15 @@
 
         Args:
             p (float, optional): The probability of applying the flip. Must be between 0 and 1. Default is 0.5.
             direction (str, optional): The direction to apply the flip. Must be 'horizontal' or 'vertical'.
                 Default is 'horizontal'.
             flip_idx (array-like, optional): Index mapping for flipping keypoints, if any.
         """
-        assert direction in ["horizontal", "vertical"], f"Support direction `horizontal` or `vertical`, got {direction}"
+        assert direction in {"horizontal", "vertical"}, f"Support direction `horizontal` or `vertical`, got {direction}"
         assert 0 <= p <= 1.0
 
         self.p = p
         self.direction = direction
         self.flip_idx = flip_idx
 
     def __call__(self, labels):
@@ -882,36 +927,39 @@
         bbox_format (str): Format for bounding boxes. Default is 'xywh'.
         normalize (bool): Whether to normalize bounding boxes. Default is True.
         return_mask (bool): Return instance masks for segmentation. Default is False.
         return_keypoint (bool): Return keypoints for pose estimation. Default is False.
         mask_ratio (int): Downsample ratio for masks. Default is 4.
         mask_overlap (bool): Whether to overlap masks. Default is True.
         batch_idx (bool): Keep batch indexes. Default is True.
+        bgr (float): The probability to return BGR images. Default is 0.0.
     """
 
     def __init__(
         self,
         bbox_format="xywh",
         normalize=True,
         return_mask=False,
         return_keypoint=False,
         return_obb=False,
         mask_ratio=4,
         mask_overlap=True,
         batch_idx=True,
+        bgr=0.0,
     ):
         """Initializes the Format class with given parameters."""
         self.bbox_format = bbox_format
         self.normalize = normalize
         self.return_mask = return_mask  # set False when training detection only
         self.return_keypoint = return_keypoint
         self.return_obb = return_obb
         self.mask_ratio = mask_ratio
         self.mask_overlap = mask_overlap
         self.batch_idx = batch_idx  # keep the batch indexes
+        self.bgr = bgr
 
     def __call__(self, labels):
         """Return formatted image, classes, bounding boxes & keypoints to be used by 'collate_fn'."""
         img = labels.pop("img")
         h, w = img.shape[:2]
         cls = labels.pop("cls")
         instances = labels.pop("instances")
@@ -924,35 +972,41 @@
                 masks, instances, cls = self._format_segments(instances, cls, w, h)
                 masks = torch.from_numpy(masks)
             else:
                 masks = torch.zeros(
                     1 if self.mask_overlap else nl, img.shape[0] // self.mask_ratio, img.shape[1] // self.mask_ratio
                 )
             labels["masks"] = masks
-        if self.normalize:
-            instances.normalize(w, h)
         labels["img"] = self._format_img(img)
         labels["cls"] = torch.from_numpy(cls) if nl else torch.zeros(nl)
         labels["bboxes"] = torch.from_numpy(instances.bboxes) if nl else torch.zeros((nl, 4))
         if self.return_keypoint:
             labels["keypoints"] = torch.from_numpy(instances.keypoints)
+            if self.normalize:
+                labels["keypoints"][..., 0] /= w
+                labels["keypoints"][..., 1] /= h
         if self.return_obb:
             labels["bboxes"] = (
                 xyxyxyxy2xywhr(torch.from_numpy(instances.segments)) if len(instances.segments) else torch.zeros((0, 5))
             )
+        # NOTE: need to normalize obb in xywhr format for width-height consistency
+        if self.normalize:
+            labels["bboxes"][:, [0, 2]] /= w
+            labels["bboxes"][:, [1, 3]] /= h
         # Then we can use collate_fn
         if self.batch_idx:
             labels["batch_idx"] = torch.zeros(nl)
         return labels
 
     def _format_img(self, img):
         """Format the image for YOLO from Numpy array to PyTorch tensor."""
         if len(img.shape) < 3:
             img = np.expand_dims(img, -1)
-        img = np.ascontiguousarray(img.transpose(2, 0, 1)[::-1])
+        img = img.transpose(2, 0, 1)
+        img = np.ascontiguousarray(img[::-1] if random.uniform(0, 1) > self.bgr else img)
         img = torch.from_numpy(img)
         return img
 
     def _format_segments(self, instances, cls, w, h):
         """Convert polygon points to bitmap."""
         segments = instances.segments
         if self.mask_overlap:
@@ -962,14 +1016,91 @@
             cls = cls[sorted_idx]
         else:
             masks = polygons2masks((h, w), segments, color=1, downsample_ratio=self.mask_ratio)
 
         return masks, instances, cls
 
 
+class RandomLoadText:
+    """
+    Randomly sample positive texts and negative texts and update the class indices accordingly to the number of samples.
+
+    Attributes:
+        prompt_format (str): Format for prompt. Default is '{}'.
+        neg_samples (tuple[int]): A ranger to randomly sample negative texts, Default is (80, 80).
+        max_samples (int): The max number of different text samples in one image, Default is 80.
+        padding (bool): Whether to pad texts to max_samples. Default is False.
+        padding_value (str): The padding text. Default is "".
+    """
+
+    def __init__(
+        self,
+        prompt_format: str = "{}",
+        neg_samples: Tuple[int, int] = (80, 80),
+        max_samples: int = 80,
+        padding: bool = False,
+        padding_value: str = "",
+    ) -> None:
+        """Initializes the RandomLoadText class with given parameters."""
+        self.prompt_format = prompt_format
+        self.neg_samples = neg_samples
+        self.max_samples = max_samples
+        self.padding = padding
+        self.padding_value = padding_value
+
+    def __call__(self, labels: dict) -> dict:
+        """Return updated classes and texts."""
+        assert "texts" in labels, "No texts found in labels."
+        class_texts = labels["texts"]
+        num_classes = len(class_texts)
+        cls = np.asarray(labels.pop("cls"), dtype=int)
+        pos_labels = np.unique(cls).tolist()
+
+        if len(pos_labels) > self.max_samples:
+            pos_labels = set(random.sample(pos_labels, k=self.max_samples))
+
+        neg_samples = min(min(num_classes, self.max_samples) - len(pos_labels), random.randint(*self.neg_samples))
+        neg_labels = []
+        for i in range(num_classes):
+            if i not in pos_labels:
+                neg_labels.append(i)
+        neg_labels = random.sample(neg_labels, k=neg_samples)
+
+        sampled_labels = pos_labels + neg_labels
+        random.shuffle(sampled_labels)
+
+        label2ids = {label: i for i, label in enumerate(sampled_labels)}
+        valid_idx = np.zeros(len(labels["instances"]), dtype=bool)
+        new_cls = []
+        for i, label in enumerate(cls.squeeze(-1).tolist()):
+            if label not in label2ids:
+                continue
+            valid_idx[i] = True
+            new_cls.append([label2ids[label]])
+        labels["instances"] = labels["instances"][valid_idx]
+        labels["cls"] = np.array(new_cls)
+
+        # Randomly select one prompt when there's more than one prompts
+        texts = []
+        for label in sampled_labels:
+            prompts = class_texts[label]
+            assert len(prompts) > 0
+            prompt = self.prompt_format.format(prompts[random.randrange(len(prompts))])
+            texts.append(prompt)
+
+        if self.padding:
+            valid_labels = len(pos_labels) + len(neg_labels)
+            num_padding = self.max_samples - valid_labels
+            if num_padding > 0:
+                texts += [self.padding_value] * num_padding
+
+        labels["texts"] = texts
+        return labels
+
+
 def v8_transforms(dataset, imgsz, hyp, stretch=False):
     """Convert images to a size suitable for YOLOv8 training."""
     pre_transform = Compose(
         [
             Mosaic(dataset, imgsz=imgsz, p=hyp.mosaic),
             CopyPaste(p=hyp.copy_paste),
             RandomPerspective(
@@ -1004,74 +1135,75 @@
 
 
 # Classification augmentations -----------------------------------------------------------------------------------------
 def classify_transforms(
     size=224,
     mean=DEFAULT_MEAN,
     std=DEFAULT_STD,
-    interpolation: T.InterpolationMode = T.InterpolationMode.BILINEAR,
-    crop_fraction: float = DEFAULT_CROP_FTACTION,
+    interpolation=Image.BILINEAR,
+    crop_fraction: float = DEFAULT_CROP_FRACTION,
 ):
     """
     Classification transforms for evaluation/inference. Inspired by timm/data/transforms_factory.py.
 
     Args:
         size (int): image size
         mean (tuple): mean values of RGB channels
         std (tuple): std values of RGB channels
         interpolation (T.InterpolationMode): interpolation mode. default is T.InterpolationMode.BILINEAR.
         crop_fraction (float): fraction of image to crop. default is 1.0.
 
     Returns:
         (T.Compose): torchvision transforms
     """
+    import torchvision.transforms as T  # scope for faster 'import ultralytics'
 
     if isinstance(size, (tuple, list)):
         assert len(size) == 2
         scale_size = tuple(math.floor(x / crop_fraction) for x in size)
     else:
         scale_size = math.floor(size / crop_fraction)
         scale_size = (scale_size, scale_size)
 
-    # aspect ratio is preserved, crops center within image, no borders are added, image is lost
+    # Aspect ratio is preserved, crops center within image, no borders are added, image is lost
     if scale_size[0] == scale_size[1]:
-        # simple case, use torchvision built-in Resize w/ shortest edge mode (scalar size arg)
+        # Simple case, use torchvision built-in Resize with the shortest edge mode (scalar size arg)
         tfl = [T.Resize(scale_size[0], interpolation=interpolation)]
     else:
-        # resize shortest edge to matching target dim for non-square target
+        # Resize the shortest edge to matching target dim for non-square target
         tfl = [T.Resize(scale_size)]
     tfl += [T.CenterCrop(size)]
 
     tfl += [
         T.ToTensor(),
         T.Normalize(
             mean=torch.tensor(mean),
             std=torch.tensor(std),
         ),
     ]
 
     return T.Compose(tfl)
 
 
-# Classification augmentations train ---------------------------------------------------------------------------------------
+# Classification training augmentations --------------------------------------------------------------------------------
 def classify_augmentations(
     size=224,
     mean=DEFAULT_MEAN,
     std=DEFAULT_STD,
     scale=None,
     ratio=None,
     hflip=0.5,
     vflip=0.0,
     auto_augment=None,
     hsv_h=0.015,  # image HSV-Hue augmentation (fraction)
     hsv_s=0.4,  # image HSV-Saturation augmentation (fraction)
     hsv_v=0.4,  # image HSV-Value augmentation (fraction)
     force_color_jitter=False,
     erasing=0.0,
-    interpolation: T.InterpolationMode = T.InterpolationMode.BILINEAR,
+    interpolation=Image.BILINEAR,
 ):
     """
     Classification transforms with augmentation for training. Inspired by timm/data/transforms_factory.py.
 
     Args:
         size (int): image size
         scale (tuple): scale range of the image. default is (0.08, 1.0)
@@ -1087,15 +1219,17 @@
         force_color_jitter (bool): force to apply color jitter even if auto augment is enabled
         erasing (float): probability of random erasing
         interpolation (T.InterpolationMode): interpolation mode. default is T.InterpolationMode.BILINEAR.
 
     Returns:
         (T.Compose): torchvision transforms
     """
-    # Transforms to apply if albumentations not installed
+    # Transforms to apply if Albumentations not installed
+    import torchvision.transforms as T  # scope for faster 'import ultralytics'
+
     if not isinstance(size, int):
         raise TypeError(f"classify_transforms() size {size} must be integer, not (list, tuple)")
     scale = tuple(scale or (0.08, 1.0))  # default imagenet scale range
     ratio = tuple(ratio or (3.0 / 4.0, 4.0 / 3.0))  # default imagenet ratio range
     primary_tfl = [T.RandomResizedCrop(size, scale=scale, ratio=ratio, interpolation=interpolation)]
     if hflip > 0.0:
         primary_tfl += [T.RandomHorizontalFlip(p=hflip)]
```

### Comparing `ultralytics-8.1.9/ultralytics/data/base.py` & `ultralytics-8.2.0/ultralytics/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 import cv2
 import numpy as np
 import psutil
 from torch.utils.data import Dataset
 
 from ultralytics.utils import DEFAULT_CFG, LOCAL_RANK, LOGGER, NUM_THREADS, TQDM
-from .utils import HELP_URL, IMG_FORMATS
+
+from .utils import FORMATS_HELP_MSG, HELP_URL, IMG_FORMATS
 
 
 class BaseDataset(Dataset):
     """
     Base dataset class for loading and processing image data.
 
     Args:
@@ -82,21 +83,20 @@
             assert self.batch_size is not None
             self.set_rectangle()
 
         # Buffer thread for mosaic images
         self.buffer = []  # buffer size = batch size
         self.max_buffer_length = min((self.ni, self.batch_size * 8, 1000)) if self.augment else 0
 
-        # Cache images
-        if cache == "ram" and not self.check_cache_ram():
-            cache = False
+        # Cache images (options are cache = True, False, None, "ram", "disk")
         self.ims, self.im_hw0, self.im_hw = [None] * self.ni, [None] * self.ni, [None] * self.ni
         self.npy_files = [Path(f).with_suffix(".npy") for f in self.im_files]
-        if cache:
-            self.cache_images(cache)
+        self.cache = cache.lower() if isinstance(cache, str) else "ram" if cache is True else None
+        if (self.cache == "ram" and self.check_cache_ram()) or self.cache == "disk":
+            self.cache_images()
 
         # Transforms
         self.transforms = self.build_transforms(hyp=hyp)
 
     def get_img_files(self, img_path):
         """Read image files."""
         try:
@@ -112,19 +112,19 @@
                         parent = str(p.parent) + os.sep
                         f += [x.replace("./", parent) if x.startswith("./") else x for x in t]  # local to global path
                         # F += [p.parent / x.lstrip(os.sep) for x in t]  # local to global path (pathlib)
                 else:
                     raise FileNotFoundError(f"{self.prefix}{p} does not exist")
             im_files = sorted(x.replace("/", os.sep) for x in f if x.split(".")[-1].lower() in IMG_FORMATS)
             # self.img_files = sorted([x for x in f if x.suffix[1:].lower() in IMG_FORMATS])  # pathlib
-            assert im_files, f"{self.prefix}No images found in {img_path}"
+            assert im_files, f"{self.prefix}No images found in {img_path}. {FORMATS_HELP_MSG}"
         except Exception as e:
             raise FileNotFoundError(f"{self.prefix}Error loading data from {img_path}\n{HELP_URL}") from e
         if self.fraction < 1:
-            im_files = im_files[: round(len(im_files) * self.fraction)]
+            im_files = im_files[: round(len(im_files) * self.fraction)]  # retain a fraction of the dataset
         return im_files
 
     def update_labels(self, include_class: Optional[list]):
         """Update labels to include only these classes (optional)."""
         include_class_array = np.array(include_class).reshape(1, -1)
         for i in range(len(self.labels)):
             if include_class is not None:
@@ -169,34 +169,35 @@
 
             # Add to buffer if training with augmentations
             if self.augment:
                 self.ims[i], self.im_hw0[i], self.im_hw[i] = im, (h0, w0), im.shape[:2]  # im, hw_original, hw_resized
                 self.buffer.append(i)
                 if len(self.buffer) >= self.max_buffer_length:
                     j = self.buffer.pop(0)
-                    self.ims[j], self.im_hw0[j], self.im_hw[j] = None, None, None
+                    if self.cache != "ram":
+                        self.ims[j], self.im_hw0[j], self.im_hw[j] = None, None, None
 
             return im, (h0, w0), im.shape[:2]
 
         return self.ims[i], self.im_hw0[i], self.im_hw[i]
 
-    def cache_images(self, cache):
+    def cache_images(self):
         """Cache images to memory or disk."""
         b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
-        fcn = self.cache_images_to_disk if cache == "disk" else self.load_image
+        fcn, storage = (self.cache_images_to_disk, "Disk") if self.cache == "disk" else (self.load_image, "RAM")
         with ThreadPool(NUM_THREADS) as pool:
             results = pool.imap(fcn, range(self.ni))
             pbar = TQDM(enumerate(results), total=self.ni, disable=LOCAL_RANK > 0)
             for i, x in pbar:
-                if cache == "disk":
+                if self.cache == "disk":
                     b += self.npy_files[i].stat().st_size
                 else:  # 'ram'
                     self.ims[i], self.im_hw0[i], self.im_hw[i] = x  # im, hw_orig, hw_resized = load_image(self, i)
                     b += self.ims[i].nbytes
-                pbar.desc = f"{self.prefix}Caching images ({b / gb:.1f}GB {cache})"
+                pbar.desc = f"{self.prefix}Caching images ({b / gb:.1f}GB {storage})"
             pbar.close()
 
     def cache_images_to_disk(self, i):
         """Saves an image as an *.npy file for faster loading."""
         f = self.npy_files[i]
         if not f.exists():
             np.save(f.as_posix(), cv2.imread(self.im_files[i]), allow_pickle=False)
@@ -207,23 +208,23 @@
         n = min(self.ni, 30)  # extrapolate from 30 random images
         for _ in range(n):
             im = cv2.imread(random.choice(self.im_files))  # sample image
             ratio = self.imgsz / max(im.shape[0], im.shape[1])  # max(h, w)  # ratio
             b += im.nbytes * ratio**2
         mem_required = b * self.ni / n * (1 + safety_margin)  # GB required to cache dataset into RAM
         mem = psutil.virtual_memory()
-        cache = mem_required < mem.available  # to cache or not to cache, that is the question
-        if not cache:
+        success = mem_required < mem.available  # to cache or not to cache, that is the question
+        if not success:
+            self.cache = None
             LOGGER.info(
-                f'{self.prefix}{mem_required / gb:.1f}GB RAM required to cache images '
-                f'with {int(safety_margin * 100)}% safety margin but only '
-                f'{mem.available / gb:.1f}/{mem.total / gb:.1f}GB available, '
-                f"{'caching images ✅' if cache else 'not caching images ⚠️'}"
+                f"{self.prefix}{mem_required / gb:.1f}GB RAM required to cache images "
+                f"with {int(safety_margin * 100)}% safety margin but only "
+                f"{mem.available / gb:.1f}/{mem.total / gb:.1f}GB available, not caching images ⚠️"
             )
-        return cache
+        return success
 
     def set_rectangle(self):
         """Sets the shape of bounding boxes for YOLO detections as rectangles."""
         bi = np.floor(np.arange(self.ni) / self.batch_size).astype(int)  # batch index
         nb = bi[-1] + 1  # number of batches
 
         s = np.array([x.pop("shape") for x in self.labels])  # hw
```

### Comparing `ultralytics-8.1.9/ultralytics/data/build.py` & `ultralytics-8.2.0/ultralytics/data/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import dataloader, distributed
 
 from ultralytics.data.loaders import (
     LOADERS,
-    LoadImages,
+    LoadImagesAndVideos,
     LoadPilAndNumpy,
     LoadScreenshots,
     LoadStreams,
     LoadTensor,
     SourceTypes,
     autocast_list,
 )
 from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
 from ultralytics.utils import RANK, colorstr
 from ultralytics.utils.checks import check_file
-from .dataset import YOLODataset
+
+from .dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
 from .utils import PIN_MEMORY
 
 
 class InfiniteDataLoader(dataloader.DataLoader):
     """
     Dataloader that reuses workers.
 
@@ -78,17 +79,18 @@
 def seed_worker(worker_id):  # noqa
     """Set dataloader worker seed https://pytorch.org/docs/stable/notes/randomness.html#dataloader."""
     worker_seed = torch.initial_seed() % 2**32
     np.random.seed(worker_seed)
     random.seed(worker_seed)
 
 
-def build_yolo_dataset(cfg, img_path, batch, data, mode="train", rect=False, stride=32):
+def build_yolo_dataset(cfg, img_path, batch, data, mode="train", rect=False, stride=32, multi_modal=False):
     """Build YOLO Dataset."""
-    return YOLODataset(
+    dataset = YOLOMultiModalDataset if multi_modal else YOLODataset
+    return dataset(
         img_path=img_path,
         imgsz=cfg.imgsz,
         batch_size=batch,
         augment=mode == "train",  # augmentation
         hyp=cfg,  # TODO: probably add a get_hyps_from_cfg function
         rect=cfg.rect or rect,  # rectangular batches
         cache=cfg.cache or None,
@@ -99,14 +101,35 @@
         task=cfg.task,
         classes=cfg.classes,
         data=data,
         fraction=cfg.fraction if mode == "train" else 1.0,
     )
 
 
+def build_grounding(cfg, img_path, json_file, batch, mode="train", rect=False, stride=32):
+    """Build YOLO Dataset."""
+    return GroundingDataset(
+        img_path=img_path,
+        json_file=json_file,
+        imgsz=cfg.imgsz,
+        batch_size=batch,
+        augment=mode == "train",  # augmentation
+        hyp=cfg,  # TODO: probably add a get_hyps_from_cfg function
+        rect=cfg.rect or rect,  # rectangular batches
+        cache=cfg.cache or None,
+        single_cls=cfg.single_cls or False,
+        stride=int(stride),
+        pad=0.0 if mode == "train" else 0.5,
+        prefix=colorstr(f"{mode}: "),
+        task=cfg.task,
+        classes=cfg.classes,
+        fraction=cfg.fraction if mode == "train" else 1.0,
+    )
+
+
 def build_dataloader(dataset, batch, workers, shuffle=True, rank=-1):
     """Return an InfiniteDataLoader or DataLoader for training or validation set."""
     batch = min(batch, len(dataset))
     nd = torch.cuda.device_count()  # number of CUDA devices
     nw = min([os.cpu_count() // max(nd, 1), workers])  # number of workers
     sampler = None if rank == -1 else distributed.DistributedSampler(dataset, shuffle=shuffle)
     generator = torch.Generator()
@@ -125,15 +148,15 @@
 
 
 def check_source(source):
     """Check source type and return corresponding flag values."""
     webcam, screenshot, from_img, in_memory, tensor = False, False, False, False, False
     if isinstance(source, (str, int, Path)):  # int for local usb camera
         source = str(source)
-        is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
+        is_file = Path(source).suffix[1:] in (IMG_FORMATS | VID_FORMATS)
         is_url = source.lower().startswith(("https://", "http://", "rtsp://", "rtmp://", "tcp://"))
         webcam = source.isnumeric() or source.endswith(".streams") or (is_url and not is_file)
         screenshot = source.lower() == "screen"
         if is_url and is_file:
             source = check_file(source)  # download
     elif isinstance(source, LOADERS):
         in_memory = True
@@ -146,40 +169,41 @@
         tensor = True
     else:
         raise TypeError("Unsupported image type. For supported types see https://docs.ultralytics.com/modes/predict")
 
     return source, webcam, screenshot, from_img, in_memory, tensor
 
 
-def load_inference_source(source=None, vid_stride=1, buffer=False):
+def load_inference_source(source=None, batch=1, vid_stride=1, buffer=False):
     """
     Loads an inference source for object detection and applies necessary transformations.
 
     Args:
         source (str, Path, Tensor, PIL.Image, np.ndarray): The input source for inference.
+        batch (int, optional): Batch size for dataloaders. Default is 1.
         vid_stride (int, optional): The frame interval for video sources. Default is 1.
         buffer (bool, optional): Determined whether stream frames will be buffered. Default is False.
 
     Returns:
         dataset (Dataset): A dataset object for the specified input source.
     """
-    source, webcam, screenshot, from_img, in_memory, tensor = check_source(source)
-    source_type = source.source_type if in_memory else SourceTypes(webcam, screenshot, from_img, tensor)
+    source, stream, screenshot, from_img, in_memory, tensor = check_source(source)
+    source_type = source.source_type if in_memory else SourceTypes(stream, screenshot, from_img, tensor)
 
     # Dataloader
     if tensor:
         dataset = LoadTensor(source)
     elif in_memory:
         dataset = source
-    elif webcam:
+    elif stream:
         dataset = LoadStreams(source, vid_stride=vid_stride, buffer=buffer)
     elif screenshot:
         dataset = LoadScreenshots(source)
     elif from_img:
         dataset = LoadPilAndNumpy(source)
     else:
-        dataset = LoadImages(source, vid_stride=vid_stride)
+        dataset = LoadImagesAndVideos(source, batch=batch, vid_stride=vid_stride)
 
     # Attach source types to the dataset
     setattr(dataset, "source_type", source_type)
 
     return dataset
```

### Comparing `ultralytics-8.1.9/ultralytics/data/converter.py` & `ultralytics-8.2.0/ultralytics/data/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,30 +215,33 @@
 
 def convert_coco(
     labels_dir="../coco/annotations/",
     save_dir="coco_converted/",
     use_segments=False,
     use_keypoints=False,
     cls91to80=True,
+    lvis=False,
 ):
     """
     Converts COCO dataset annotations to a YOLO annotation format  suitable for training YOLO models.
 
     Args:
         labels_dir (str, optional): Path to directory containing COCO dataset annotation files.
         save_dir (str, optional): Path to directory to save results to.
         use_segments (bool, optional): Whether to include segmentation masks in the output.
         use_keypoints (bool, optional): Whether to include keypoint annotations in the output.
         cls91to80 (bool, optional): Whether to map 91 COCO class IDs to the corresponding 80 COCO class IDs.
+        lvis (bool, optional): Whether to convert data in lvis dataset way.
 
     Example:
         ```python
         from ultralytics.data.converter import convert_coco
 
         convert_coco('../datasets/coco/annotations/', use_segments=True, use_keypoints=False, cls91to80=True)
+        convert_coco('../datasets/lvis/annotations/', use_segments=True, use_keypoints=False, cls91to80=False, lvis=True)
         ```
 
     Output:
         Generates output files in the specified output directory.
     """
 
     # Create dataset directory
@@ -247,36 +250,46 @@
         p.mkdir(parents=True, exist_ok=True)  # make dir
 
     # Convert classes
     coco80 = coco91_to_coco80_class()
 
     # Import json
     for json_file in sorted(Path(labels_dir).resolve().glob("*.json")):
-        fn = Path(save_dir) / "labels" / json_file.stem.replace("instances_", "")  # folder name
+        lname = "" if lvis else json_file.stem.replace("instances_", "")
+        fn = Path(save_dir) / "labels" / lname  # folder name
         fn.mkdir(parents=True, exist_ok=True)
+        if lvis:
+            # NOTE: create folders for both train and val in advance,
+            # since LVIS val set contains images from COCO 2017 train in addition to the COCO 2017 val split.
+            (fn / "train2017").mkdir(parents=True, exist_ok=True)
+            (fn / "val2017").mkdir(parents=True, exist_ok=True)
         with open(json_file) as f:
             data = json.load(f)
 
         # Create image dict
         images = {f'{x["id"]:d}': x for x in data["images"]}
         # Create image-annotations dict
         imgToAnns = defaultdict(list)
         for ann in data["annotations"]:
             imgToAnns[ann["image_id"]].append(ann)
 
+        image_txt = []
         # Write labels file
         for img_id, anns in TQDM(imgToAnns.items(), desc=f"Annotations {json_file}"):
             img = images[f"{img_id:d}"]
-            h, w, f = img["height"], img["width"], img["file_name"]
+            h, w = img["height"], img["width"]
+            f = str(Path(img["coco_url"]).relative_to("http://images.cocodataset.org")) if lvis else img["file_name"]
+            if lvis:
+                image_txt.append(str(Path("./images") / f))
 
             bboxes = []
             segments = []
             keypoints = []
             for ann in anns:
-                if ann["iscrowd"]:
+                if ann.get("iscrowd", False):
                     continue
                 # The COCO box format is [top left x, top left y, width, height]
                 box = np.array(ann["bbox"], dtype=np.float64)
                 box[:2] += box[2:] / 2  # xy top-left corner to center
                 box[[0, 2]] /= w  # normalize x
                 box[[1, 3]] /= h  # normalize y
                 if box[2] <= 0 or box[3] <= 0:  # if w <= 0 and h <= 0
@@ -310,15 +323,20 @@
                         line = (*(keypoints[i]),)  # cls, box, keypoints
                     else:
                         line = (
                             *(segments[i] if use_segments and len(segments[i]) > 0 else bboxes[i]),
                         )  # cls, box or segments
                     file.write(("%g " * len(line)).rstrip() % line + "\n")
 
-    LOGGER.info(f"COCO data converted successfully.\nResults saved to {save_dir.resolve()}")
+        if lvis:
+            with open((Path(save_dir) / json_file.name.replace("lvis_v1_", "").replace(".json", ".txt")), "a") as f:
+                for l in image_txt:
+                    f.write(f"{l}\n")
+
+    LOGGER.info(f"{'LVIS' if lvis else 'COCO'} data converted successfully.\nResults saved to {save_dir.resolve()}")
 
 
 def convert_dota_to_yolo_obb(dota_root_path: str):
     """
     Converts DOTA dataset annotations to YOLO OBB (Oriented Bounding Box) format.
 
     The function processes images in the 'train' and 'val' folders of the DOTA dataset. For each image, it reads the
@@ -414,16 +432,16 @@
 
 
 def min_index(arr1, arr2):
     """
     Find a pair of indexes with the shortest distance between two arrays of 2D points.
 
     Args:
-        arr1 (np.array): A NumPy array of shape (N, 2) representing N 2D points.
-        arr2 (np.array): A NumPy array of shape (M, 2) representing M 2D points.
+        arr1 (np.ndarray): A NumPy array of shape (N, 2) representing N 2D points.
+        arr2 (np.ndarray): A NumPy array of shape (M, 2) representing M 2D points.
 
     Returns:
         (tuple): A tuple containing the indexes of the points with the shortest distance in arr1 and arr2 respectively.
     """
     dis = ((arr1[:, None, :] - arr2[None, :, :]) ** 2).sum(-1)
     return np.unravel_index(np.argmin(dis, axis=None), dis.shape)
 
@@ -459,23 +477,23 @@
                 if len(idx) == 2 and idx[0] > idx[1]:
                     idx = idx[::-1]
                     segments[i] = segments[i][::-1, :]
 
                 segments[i] = np.roll(segments[i], -idx[0], axis=0)
                 segments[i] = np.concatenate([segments[i], segments[i][:1]])
                 # Deal with the first segment and the last one
-                if i in [0, len(idx_list) - 1]:
+                if i in {0, len(idx_list) - 1}:
                     s.append(segments[i])
                 else:
                     idx = [0, idx[1] - idx[0]]
                     s.append(segments[i][idx[0] : idx[1] + 1])
 
         else:
             for i in range(len(idx_list) - 1, -1, -1):
-                if i not in [0, len(idx_list) - 1]:
+                if i not in {0, len(idx_list) - 1}:
                     idx = idx_list[i]
                     nidx = abs(idx[1] - idx[0])
                     s.append(segments[i][nidx:])
     return s
 
 
 def yolo_bbox2segment(im_dir, save_dir=None, sam_model="sam_b.pt"):
@@ -497,19 +515,20 @@
                 ├─ ..
                 └─ NNN.jpg
             - labels
                 ├─ 001.txt
                 ├─ ..
                 └─ NNN.txt
     """
+    from tqdm import tqdm
+
+    from ultralytics import SAM
     from ultralytics.data import YOLODataset
-    from ultralytics.utils.ops import xywh2xyxy
     from ultralytics.utils import LOGGER
-    from ultralytics import SAM
-    from tqdm import tqdm
+    from ultralytics.utils.ops import xywh2xyxy
 
     # NOTE: add placeholder to pass class index check
     dataset = YOLODataset(im_dir, data=dict(names=list(range(1000))))
     if len(dataset.labels[0]["segments"]) > 0:  # if it's segment data
         LOGGER.info("Segmentation labels detected, no need to generate new ones!")
         return
```

### Comparing `ultralytics-8.1.9/ultralytics/data/dataset.py` & `ultralytics-8.2.0/ultralytics/data/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
+
 import contextlib
+import json
+from collections import defaultdict
 from itertools import repeat
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
 import cv2
 import numpy as np
 import torch
-import torchvision
 from PIL import Image
+from torch.utils.data import ConcatDataset
 
-from ultralytics.utils import LOCAL_RANK, NUM_THREADS, TQDM, colorstr, is_dir_writeable
+from ultralytics.utils import LOCAL_RANK, NUM_THREADS, TQDM, colorstr
 from ultralytics.utils.ops import resample_segments
-from .augment import Compose, Format, Instances, LetterBox, classify_augmentations, classify_transforms, v8_transforms
+
+from .augment import (
+    Compose,
+    Format,
+    Instances,
+    LetterBox,
+    RandomLoadText,
+    classify_augmentations,
+    classify_transforms,
+    v8_transforms,
+)
 from .base import BaseDataset
-from .utils import HELP_URL, LOGGER, get_hash, img2label_paths, verify_image, verify_image_label
+from .utils import (
+    HELP_URL,
+    LOGGER,
+    get_hash,
+    img2label_paths,
+    load_dataset_cache_file,
+    save_dataset_cache_file,
+    verify_image,
+    verify_image_label,
+)
 
 # Ultralytics dataset *.cache version, >= 1.0.0 for YOLOv8
 DATASET_CACHE_VERSION = "1.0.3"
 
 
 class YOLODataset(BaseDataset):
     """
@@ -52,15 +74,15 @@
             (dict): labels.
         """
         x = {"labels": []}
         nm, nf, ne, nc, msgs = 0, 0, 0, 0, []  # number missing, found, empty, corrupt, messages
         desc = f"{self.prefix}Scanning {path.parent / path.stem}..."
         total = len(self.im_files)
         nkpt, ndim = self.data.get("kpt_shape", (0, 0))
-        if self.use_keypoints and (nkpt <= 0 or ndim not in (2, 3)):
+        if self.use_keypoints and (nkpt <= 0 or ndim not in {2, 3}):
             raise ValueError(
                 "'kpt_shape' in data.yaml missing or incorrect. Should be a list with [number of "
                 "keypoints, number of dims (2 for x,y or 3 for x,y,visible)], i.e. 'kpt_shape: [17, 3]'"
             )
         with ThreadPool(NUM_THREADS) as pool:
             results = pool.imap(
                 func=verify_image_label,
@@ -78,38 +100,38 @@
             for im_file, lb, shape, segments, keypoint, nm_f, nf_f, ne_f, nc_f, msg in pbar:
                 nm += nm_f
                 nf += nf_f
                 ne += ne_f
                 nc += nc_f
                 if im_file:
                     x["labels"].append(
-                        dict(
-                            im_file=im_file,
-                            shape=shape,
-                            cls=lb[:, 0:1],  # n, 1
-                            bboxes=lb[:, 1:],  # n, 4
-                            segments=segments,
-                            keypoints=keypoint,
-                            normalized=True,
-                            bbox_format="xywh",
-                        )
+                        {
+                            "im_file": im_file,
+                            "shape": shape,
+                            "cls": lb[:, 0:1],  # n, 1
+                            "bboxes": lb[:, 1:],  # n, 4
+                            "segments": segments,
+                            "keypoints": keypoint,
+                            "normalized": True,
+                            "bbox_format": "xywh",
+                        }
                     )
                 if msg:
                     msgs.append(msg)
                 pbar.desc = f"{desc} {nf} images, {nm + ne} backgrounds, {nc} corrupt"
             pbar.close()
 
         if msgs:
             LOGGER.info("\n".join(msgs))
         if nf == 0:
             LOGGER.warning(f"{self.prefix}WARNING ⚠️ No labels found in {path}. {HELP_URL}")
         x["hash"] = get_hash(self.label_files + self.im_files)
         x["results"] = nf, nm, ne, nc, len(self.im_files)
         x["msgs"] = msgs  # warnings
-        save_dataset_cache_file(self.prefix, path, x)
+        save_dataset_cache_file(self.prefix, path, x, DATASET_CACHE_VERSION)
         return x
 
     def get_labels(self):
         """Returns dictionary of labels for YOLO training."""
         self.label_files = img2label_paths(self.im_files)
         cache_path = Path(self.label_files[0]).parent.with_suffix(".cache")
         try:
@@ -117,15 +139,15 @@
             assert cache["version"] == DATASET_CACHE_VERSION  # matches current version
             assert cache["hash"] == get_hash(self.label_files + self.im_files)  # identical hash
         except (FileNotFoundError, AssertionError, AttributeError):
             cache, exists = self.cache_labels(cache_path), False  # run cache ops
 
         # Display cache
         nf, nm, ne, nc, n = cache.pop("results")  # found, missing, empty, corrupt, total
-        if exists and LOCAL_RANK in (-1, 0):
+        if exists and LOCAL_RANK in {-1, 0}:
             d = f"Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt"
             TQDM(None, desc=self.prefix + d, total=n, initial=n)  # display results
             if cache["msgs"]:
                 LOGGER.info("\n".join(cache["msgs"]))  # display warnings
 
         # Read cache
         [cache.pop(k) for k in ("hash", "version", "msgs")]  # remove items
@@ -163,14 +185,15 @@
                 normalize=True,
                 return_mask=self.use_segments,
                 return_keypoint=self.use_keypoints,
                 return_obb=self.use_obb,
                 batch_idx=True,
                 mask_ratio=hyp.mask_ratio,
                 mask_overlap=hyp.overlap_mask,
+                bgr=hyp.bgr if self.augment else 0.0,  # only affect training.
             )
         )
         return transforms
 
     def close_mosaic(self, hyp):
         """Sets mosaic, copy_paste and mixup options to 0.0 and builds transformations."""
         hyp.mosaic = 0.0  # set mosaic ratio=0.0
@@ -209,56 +232,204 @@
         new_batch = {}
         keys = batch[0].keys()
         values = list(zip(*[list(b.values()) for b in batch]))
         for i, k in enumerate(keys):
             value = values[i]
             if k == "img":
                 value = torch.stack(value, 0)
-            if k in ["masks", "keypoints", "bboxes", "cls", "segments", "obb"]:
+            if k in {"masks", "keypoints", "bboxes", "cls", "segments", "obb"}:
                 value = torch.cat(value, 0)
             new_batch[k] = value
         new_batch["batch_idx"] = list(new_batch["batch_idx"])
         for i in range(len(new_batch["batch_idx"])):
             new_batch["batch_idx"][i] += i  # add target image index for build_targets()
         new_batch["batch_idx"] = torch.cat(new_batch["batch_idx"], 0)
         return new_batch
 
 
-# Classification dataloaders -------------------------------------------------------------------------------------------
-class ClassificationDataset(torchvision.datasets.ImageFolder):
+class YOLOMultiModalDataset(YOLODataset):
     """
-    YOLO Classification Dataset.
+    Dataset class for loading object detection and/or segmentation labels in YOLO format.
 
     Args:
-        root (str): Dataset path.
+        data (dict, optional): A dataset YAML dictionary. Defaults to None.
+        task (str): An explicit arg to point current task, Defaults to 'detect'.
+
+    Returns:
+        (torch.utils.data.Dataset): A PyTorch dataset object that can be used for training an object detection model.
+    """
+
+    def __init__(self, *args, data=None, task="detect", **kwargs):
+        """Initializes a dataset object for object detection tasks with optional specifications."""
+        super().__init__(*args, data=data, task=task, **kwargs)
+
+    def update_labels_info(self, label):
+        """Add texts information for multi modal model training."""
+        labels = super().update_labels_info(label)
+        # NOTE: some categories are concatenated with its synonyms by `/`.
+        labels["texts"] = [v.split("/") for _, v in self.data["names"].items()]
+        return labels
+
+    def build_transforms(self, hyp=None):
+        """Enhances data transformations with optional text augmentation for multi-modal training."""
+        transforms = super().build_transforms(hyp)
+        if self.augment:
+            # NOTE: hard-coded the args for now.
+            transforms.insert(-1, RandomLoadText(max_samples=min(self.data["nc"], 80), padding=True))
+        return transforms
+
+
+class GroundingDataset(YOLODataset):
+    def __init__(self, *args, task="detect", json_file, **kwargs):
+        """Initializes a GroundingDataset for object detection, loading annotations from a specified JSON file."""
+        assert task == "detect", "`GroundingDataset` only support `detect` task for now!"
+        self.json_file = json_file
+        super().__init__(*args, task=task, data={}, **kwargs)
+
+    def get_img_files(self, img_path):
+        """The image files would be read in `get_labels` function, return empty list here."""
+        return []
+
+    def get_labels(self):
+        """Loads annotations from a JSON file, filters, and normalizes bounding boxes for each image."""
+        labels = []
+        LOGGER.info("Loading annotation file...")
+        with open(self.json_file, "r") as f:
+            annotations = json.load(f)
+        images = {f'{x["id"]:d}': x for x in annotations["images"]}
+        imgToAnns = defaultdict(list)
+        for ann in annotations["annotations"]:
+            imgToAnns[ann["image_id"]].append(ann)
+        for img_id, anns in TQDM(imgToAnns.items(), desc=f"Reading annotations {self.json_file}"):
+            img = images[f"{img_id:d}"]
+            h, w, f = img["height"], img["width"], img["file_name"]
+            im_file = Path(self.img_path) / f
+            if not im_file.exists():
+                continue
+            self.im_files.append(str(im_file))
+            bboxes = []
+            cat2id = {}
+            texts = []
+            for ann in anns:
+                if ann["iscrowd"]:
+                    continue
+                box = np.array(ann["bbox"], dtype=np.float32)
+                box[:2] += box[2:] / 2
+                box[[0, 2]] /= float(w)
+                box[[1, 3]] /= float(h)
+                if box[2] <= 0 or box[3] <= 0:
+                    continue
+
+                cat_name = " ".join([img["caption"][t[0] : t[1]] for t in ann["tokens_positive"]])
+                if cat_name not in cat2id:
+                    cat2id[cat_name] = len(cat2id)
+                    texts.append([cat_name])
+                cls = cat2id[cat_name]  # class
+                box = [cls] + box.tolist()
+                if box not in bboxes:
+                    bboxes.append(box)
+            lb = np.array(bboxes, dtype=np.float32) if len(bboxes) else np.zeros((0, 5), dtype=np.float32)
+            labels.append(
+                {
+                    "im_file": im_file,
+                    "shape": (h, w),
+                    "cls": lb[:, 0:1],  # n, 1
+                    "bboxes": lb[:, 1:],  # n, 4
+                    "normalized": True,
+                    "bbox_format": "xywh",
+                    "texts": texts,
+                }
+            )
+        return labels
+
+    def build_transforms(self, hyp=None):
+        """Configures augmentations for training with optional text loading; `hyp` adjusts augmentation intensity."""
+        transforms = super().build_transforms(hyp)
+        if self.augment:
+            # NOTE: hard-coded the args for now.
+            transforms.insert(-1, RandomLoadText(max_samples=80, padding=True))
+        return transforms
+
+
+class YOLOConcatDataset(ConcatDataset):
+    """
+    Dataset as a concatenation of multiple datasets.
+
+    This class is useful to assemble different existing datasets.
+    """
+
+    @staticmethod
+    def collate_fn(batch):
+        """Collates data samples into batches."""
+        return YOLODataset.collate_fn(batch)
+
+
+# TODO: support semantic segmentation
+class SemanticDataset(BaseDataset):
+    """
+    Semantic Segmentation Dataset.
+
+    This class is responsible for handling datasets used for semantic segmentation tasks. It inherits functionalities
+    from the BaseDataset class.
+
+    Note:
+        This class is currently a placeholder and needs to be populated with methods and attributes for supporting
+        semantic segmentation tasks.
+    """
+
+    def __init__(self):
+        """Initialize a SemanticDataset object."""
+        super().__init__()
+
+
+class ClassificationDataset:
+    """
+    Extends torchvision ImageFolder to support YOLO classification tasks, offering functionalities like image
+    augmentation, caching, and verification. It's designed to efficiently handle large datasets for training deep
+    learning models, with optional image transformations and caching mechanisms to speed up training.
+
+    This class allows for augmentations using both torchvision and Albumentations libraries, and supports caching images
+    in RAM or on disk to reduce IO overhead during training. Additionally, it implements a robust verification process
+    to ensure data integrity and consistency.
 
     Attributes:
-        cache_ram (bool): True if images should be cached in RAM, False otherwise.
-        cache_disk (bool): True if images should be cached on disk, False otherwise.
-        samples (list): List of samples containing file, index, npy, and im.
-        torch_transforms (callable): torchvision transforms applied to the dataset.
-        album_transforms (callable, optional): Albumentations transforms applied to the dataset if augment is True.
+        cache_ram (bool): Indicates if caching in RAM is enabled.
+        cache_disk (bool): Indicates if caching on disk is enabled.
+        samples (list): A list of tuples, each containing the path to an image, its class index, path to its .npy cache
+                        file (if caching on disk), and optionally the loaded image array (if caching in RAM).
+        torch_transforms (callable): PyTorch transforms to be applied to the images.
     """
 
-    def __init__(self, root, args, augment=False, cache=False, prefix=""):
+    def __init__(self, root, args, augment=False, prefix=""):
         """
         Initialize YOLO object with root, image size, augmentations, and cache settings.
 
         Args:
-            root (str): Dataset path.
-            args (Namespace): Argument parser containing dataset related settings.
-            augment (bool, optional): True if dataset should be augmented, False otherwise. Defaults to False.
-            cache (bool | str | optional): Cache setting, can be True, False, 'ram' or 'disk'. Defaults to False.
+            root (str): Path to the dataset directory where images are stored in a class-specific folder structure.
+            args (Namespace): Configuration containing dataset-related settings such as image size, augmentation
+                parameters, and cache settings. It includes attributes like `imgsz` (image size), `fraction` (fraction
+                of data to use), `scale`, `fliplr`, `flipud`, `cache` (disk or RAM caching for faster training),
+                `auto_augment`, `hsv_h`, `hsv_s`, `hsv_v`, and `crop_fraction`.
+            augment (bool, optional): Whether to apply augmentations to the dataset. Default is False.
+            prefix (str, optional): Prefix for logging and cache filenames, aiding in dataset identification and
+                debugging. Default is an empty string.
         """
-        super().__init__(root=root)
+        import torchvision  # scope for faster 'import ultralytics'
+
+        # Base class assigned as attribute rather than used as base class to allow for scoping slow torchvision import
+        self.base = torchvision.datasets.ImageFolder(root=root)
+        self.samples = self.base.samples
+        self.root = self.base.root
+
+        # Initialize attributes
         if augment and args.fraction < 1.0:  # reduce training fraction
             self.samples = self.samples[: round(len(self.samples) * args.fraction)]
         self.prefix = colorstr(f"{prefix}: ") if prefix else ""
-        self.cache_ram = cache is True or cache == "ram"
-        self.cache_disk = cache == "disk"
+        self.cache_ram = args.cache is True or str(args.cache).lower() == "ram"  # cache images into RAM
+        self.cache_disk = str(args.cache).lower() == "disk"  # cache images on hard drive as uncompressed *.npy files
         self.samples = self.verify_images()  # filter out bad images
         self.samples = [list(x) + [Path(x[0]).with_suffix(".npy"), None] for x in self.samples]  # file, index, npy, im
         scale = (1.0 - args.scale, 1.0)  # (0.08, 1.0)
         self.torch_transforms = (
             classify_augmentations(
                 size=args.imgsz,
                 scale=scale,
@@ -273,16 +444,17 @@
             if augment
             else classify_transforms(size=args.imgsz, crop_fraction=args.crop_fraction)
         )
 
     def __getitem__(self, i):
         """Returns subset of data and targets corresponding to given indices."""
         f, j, fn, im = self.samples[i]  # filename, index, filename.with_suffix('.npy'), image
-        if self.cache_ram and im is None:
-            im = self.samples[i][3] = cv2.imread(f)
+        if self.cache_ram:
+            if im is None:  # Warning: two separate if statements required here, do not combine this with previous line
+                im = self.samples[i][3] = cv2.imread(f)
         elif self.cache_disk:
             if not fn.exists():  # load npy
                 np.save(fn.as_posix(), cv2.imread(f), allow_pickle=False)
             im = np.load(fn)
         else:  # read image
             im = cv2.imread(f)  # BGR
         # Convert NumPy array to PIL image
@@ -300,15 +472,15 @@
         path = Path(self.root).with_suffix(".cache")  # *.cache file path
 
         with contextlib.suppress(FileNotFoundError, AssertionError, AttributeError):
             cache = load_dataset_cache_file(path)  # attempt to load a *.cache file
             assert cache["version"] == DATASET_CACHE_VERSION  # matches current version
             assert cache["hash"] == get_hash([x[0] for x in self.samples])  # identical hash
             nf, nc, n, samples = cache.pop("results")  # found, missing, empty, corrupt, total
-            if LOCAL_RANK in (-1, 0):
+            if LOCAL_RANK in {-1, 0}:
                 d = f"{desc} {nf} images, {nc} corrupt"
                 TQDM(None, desc=d, total=n, initial=n)
                 if cache["msgs"]:
                     LOGGER.info("\n".join(cache["msgs"]))  # display warnings
             return samples
 
         # Run scan if *.cache retrieval failed
@@ -326,50 +498,9 @@
                 pbar.desc = f"{desc} {nf} images, {nc} corrupt"
             pbar.close()
         if msgs:
             LOGGER.info("\n".join(msgs))
         x["hash"] = get_hash([x[0] for x in self.samples])
         x["results"] = nf, nc, len(samples), samples
         x["msgs"] = msgs  # warnings
-        save_dataset_cache_file(self.prefix, path, x)
+        save_dataset_cache_file(self.prefix, path, x, DATASET_CACHE_VERSION)
         return samples
-
-
-def load_dataset_cache_file(path):
-    """Load an Ultralytics *.cache dictionary from path."""
-    import gc
-
-    gc.disable()  # reduce pickle load time https://github.com/ultralytics/ultralytics/pull/1585
-    cache = np.load(str(path), allow_pickle=True).item()  # load dict
-    gc.enable()
-    return cache
-
-
-def save_dataset_cache_file(prefix, path, x):
-    """Save an Ultralytics dataset *.cache dictionary x to path."""
-    x["version"] = DATASET_CACHE_VERSION  # add cache version
-    if is_dir_writeable(path.parent):
-        if path.exists():
-            path.unlink()  # remove *.cache file if exists
-        np.save(str(path), x)  # save cache for next time
-        path.with_suffix(".cache.npy").rename(path)  # remove .npy suffix
-        LOGGER.info(f"{prefix}New cache created: {path}")
-    else:
-        LOGGER.warning(f"{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable, cache not saved.")
-
-
-# TODO: support semantic segmentation
-class SemanticDataset(BaseDataset):
-    """
-    Semantic Segmentation Dataset.
-
-    This class is responsible for handling datasets used for semantic segmentation tasks. It inherits functionalities
-    from the BaseDataset class.
-
-    Note:
-        This class is currently a placeholder and needs to be populated with methods and attributes for supporting
-        semantic segmentation tasks.
-    """
-
-    def __init__(self):
-        """Initialize a SemanticDataset object."""
-        super().__init__()
```

### Comparing `ultralytics-8.1.9/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.0/ultralytics/data/explorer/explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from io import BytesIO
 from pathlib import Path
 from typing import Any, List, Tuple, Union
 
 import cv2
 import numpy as np
 import torch
-from PIL import Image
 from matplotlib import pyplot as plt
-from pandas import DataFrame
+from PIL import Image
 from tqdm import tqdm
 
 from ultralytics.data.augment import Format
 from ultralytics.data.dataset import YOLODataset
 from ultralytics.data.utils import check_det_dataset
 from ultralytics.models.yolo.model import YOLO
-from ultralytics.utils import LOGGER, IterableSimpleNamespace, checks, USER_CONFIG_DIR
+from ultralytics.utils import LOGGER, USER_CONFIG_DIR, IterableSimpleNamespace, checks
+
 from .utils import get_sim_index_schema, get_table_schema, plot_query_result, prompt_sql_query, sanitize_batch
 
 
 class ExplorerDataset(YOLODataset):
     def __init__(self, *args, data: dict = None, **kwargs) -> None:
         super().__init__(*args, data=data, **kwargs)
 
@@ -55,15 +55,16 @@
 class Explorer:
     def __init__(
         self,
         data: Union[str, Path] = "coco128.yaml",
         model: str = "yolov8n.pt",
         uri: str = USER_CONFIG_DIR / "explorer",
     ) -> None:
-        checks.check_requirements(["lancedb>=0.4.3", "duckdb"])
+        # Note duckdb==0.10.0 bug https://github.com/ultralytics/ultralytics/pull/8181
+        checks.check_requirements(["lancedb>=0.4.3", "duckdb<=0.9.2"])
         import lancedb
 
         self.connection = lancedb.connect(uri)
         self.table_name = Path(data).name.lower() + "_" + model.lower()
         self.sim_idx_base_name = (
             f"{self.table_name}_sim_idx".lower()
         )  # Use this name and append thres and top_k to reuse the table
@@ -167,15 +168,15 @@
         embeds = self.model.embed(imgs)
         # Get avg if multiple images are passed (len > 1)
         embeds = torch.mean(torch.stack(embeds), 0).cpu().numpy() if len(embeds) > 1 else embeds[0].cpu().numpy()
         return self.table.search(embeds).limit(limit).to_arrow()
 
     def sql_query(
         self, query: str, return_type: str = "pandas"
-    ) -> Union[DataFrame, Any, None]:  # pandas.dataframe or pyarrow.Table
+    ) -> Union[Any, None]:  # pandas.DataFrame or pyarrow.Table
         """
         Run a SQL-Like query on the table. Utilizes LanceDB predicate pushdown.
 
         Args:
             query (str): SQL query to run.
             return_type (str): Type of the result to return. Can be either 'pandas' or 'arrow'. Defaults to 'pandas'.
 
@@ -199,15 +200,16 @@
         if self.table is None:
             raise ValueError("Table is not created. Please create the table first.")
 
         # Note: using filter pushdown would be a better long term solution. Temporarily using duckdb for this.
         table = self.table.to_arrow()  # noqa NOTE: Don't comment this. This line is used by DuckDB
         if not query.startswith("SELECT") and not query.startswith("WHERE"):
             raise ValueError(
-                f"Query must start with SELECT or WHERE. You can either pass the entire query or just the WHERE clause. found {query}"
+                f"Query must start with SELECT or WHERE. You can either pass the entire query or just the WHERE "
+                f"clause. found {query}"
             )
         if query.startswith("WHERE"):
             query = f"SELECT * FROM 'table' {query}"
         LOGGER.info(f"Running query: {query}")
 
         rs = duckdb.sql(query)
         if return_type == "arrow":
@@ -242,15 +244,15 @@
 
     def get_similar(
         self,
         img: Union[str, np.ndarray, List[str], List[np.ndarray]] = None,
         idx: Union[int, List[int]] = None,
         limit: int = 25,
         return_type: str = "pandas",
-    ) -> Union[DataFrame, Any]:  # pandas.dataframe or pyarrow.Table
+    ) -> Any:  # pandas.DataFrame or pyarrow.Table
         """
         Query the table for similar images. Accepts a single image or a list of images.
 
         Args:
             img (str or list): Path to the image or a list of paths to the images.
             idx (int or list): Index of the image in the table or a list of indexes.
             limit (int): Number of results to return. Defaults to 25.
@@ -307,28 +309,28 @@
         similar = self.get_similar(img, idx, limit, return_type="arrow")
         if len(similar) == 0:
             LOGGER.info("No results found.")
             return None
         img = plot_query_result(similar, plot_labels=labels)
         return Image.fromarray(img)
 
-    def similarity_index(self, max_dist: float = 0.2, top_k: float = None, force: bool = False) -> DataFrame:
+    def similarity_index(self, max_dist: float = 0.2, top_k: float = None, force: bool = False) -> Any:  # pd.DataFrame
         """
         Calculate the similarity index of all the images in the table. Here, the index will contain the data points that
         are max_dist or closer to the image in the embedding space at a given index.
 
         Args:
             max_dist (float): maximum L2 distance between the embeddings to consider. Defaults to 0.2.
-            top_k (float): Percentage of the closest data points to consider when counting. Used to apply limit when running
+            top_k (float): Percentage of the closest data points to consider when counting. Used to apply limit.
                            vector search. Defaults: None.
             force (bool): Whether to overwrite the existing similarity index or not. Defaults to True.
 
         Returns:
-            (pandas.DataFrame): A dataframe containing the similarity index. Each row corresponds to an image, and columns
-                                include indices of similar images and their respective distances.
+            (pandas.DataFrame): A dataframe containing the similarity index. Each row corresponds to an image,
+                and columns include indices of similar images and their respective distances.
 
         Example:
             ```python
             exp = Explorer()
             exp.create_embeddings_table()
             sim_idx = exp.similarity_index()
             ```
@@ -442,20 +444,19 @@
             exp = Explorer()
             exp.create_embeddings_table()
             answer = exp.ask_ai('Show images with 1 person and 2 dogs')
             ```
         """
         result = prompt_sql_query(query)
         try:
-            df = self.sql_query(result)
+            return self.sql_query(result)
         except Exception as e:
             LOGGER.error("AI generated query is not valid. Please try again with a different prompt")
             LOGGER.error(e)
             return None
-        return df
 
     def visualize(self, result):
         """
         Visualize the results of a query. TODO.
 
         Args:
             result (pyarrow.Table): Table containing the results of a query.
```

### Comparing `ultralytics-8.1.9/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.0/ultralytics/data/explorer/gui/dash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import time
 from threading import Thread
 
-import pandas as pd
-
 from ultralytics import Explorer
 from ultralytics.utils import ROOT, SETTINGS
 from ultralytics.utils.checks import check_requirements
 
 check_requirements(("streamlit>=1.29.0", "streamlit-select>=0.3"))
 
 import streamlit as st
@@ -140,24 +138,26 @@
         st.session_state["imgs"] = res.to_pydict()["im_file"]
         st.session_state["res"] = res
 
 
 def run_ai_query():
     """Execute SQL query and update session state with query results."""
     if not SETTINGS["openai_api_key"]:
-        st.session_state[
-            "error"
-        ] = 'OpenAI API key not found in settings. Please run yolo settings openai_api_key="..."'
+        st.session_state["error"] = (
+            'OpenAI API key not found in settings. Please run yolo settings openai_api_key="..."'
+        )
         return
+    import pandas  # scope for faster 'import ultralytics'
+
     st.session_state["error"] = None
     query = st.session_state.get("ai_query")
     if query.rstrip().lstrip():
         exp = st.session_state["explorer"]
         res = exp.ask_ai(query)
-        if not isinstance(res, pd.DataFrame) or res.empty:
+        if not isinstance(res, pandas.DataFrame) or res.empty:
             st.session_state["error"] = "No results found using AI generated query. Try another query or rerun it."
             return
         st.session_state["imgs"] = res["im_file"].to_list()
         st.session_state["res"] = res
 
 
 def reset_explorer():
```

### Comparing `ultralytics-8.1.9/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.0/ultralytics/data/explorer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import getpass
 from typing import List
 
 import cv2
 import numpy as np
-import pandas as pd
 
 from ultralytics.data.augment import LetterBox
 from ultralytics.utils import LOGGER as logger
 from ultralytics.utils import SETTINGS
 from ultralytics.utils.checks import check_requirements
 from ultralytics.utils.ops import xyxy2xywh
 from ultralytics.utils.plotting import plot_images
@@ -60,16 +59,18 @@
     """
     Plot images from the similar set.
 
     Args:
         similar_set (list): Pyarrow or pandas object containing the similar data points
         plot_labels (bool): Whether to plot labels or not
     """
+    import pandas  # scope for faster 'import ultralytics'
+
     similar_set = (
-        similar_set.to_dict(orient="list") if isinstance(similar_set, pd.DataFrame) else similar_set.to_pydict()
+        similar_set.to_dict(orient="list") if isinstance(similar_set, pandas.DataFrame) else similar_set.to_pydict()
     )
     empty_masks = [[[]]]
     empty_boxes = [[]]
     images = similar_set.get("im_file", [])
     bboxes = similar_set.get("bboxes", []) if similar_set.get("bboxes") is not empty_boxes else []
     masks = similar_set.get("masks") if similar_set.get("masks")[0] != empty_masks else []
     kpts = similar_set.get("keypoints") if similar_set.get("keypoints")[0] != empty_masks else []
```

### Comparing `ultralytics-8.1.9/ultralytics/data/loaders.py` & `ultralytics-8.2.0/ultralytics/data/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 
 import cv2
 import numpy as np
 import requests
 import torch
 from PIL import Image
 
-from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
-from ultralytics.utils import LOGGER, is_colab, is_kaggle, ops
+from ultralytics.data.utils import FORMATS_HELP_MSG, IMG_FORMATS, VID_FORMATS
+from ultralytics.utils import IS_COLAB, IS_KAGGLE, LOGGER, ops
 from ultralytics.utils.checks import check_requirements
 
 
 @dataclass
 class SourceTypes:
     """Class to represent various types of input sources for predictions."""
 
-    webcam: bool = False
+    stream: bool = False
     screenshot: bool = False
     from_img: bool = False
     tensor: bool = False
 
 
 class LoadStreams:
     """
-    Stream Loader for various types of video streams.
-
-    Suitable for use with `yolo predict source='rtsp://example.com/media.mp4'`, supports RTSP, RTMP, HTTP, and TCP streams.
+    Stream Loader for various types of video streams, Supports RTSP, RTMP, HTTP, and TCP streams.
 
     Attributes:
         sources (str): The source input paths or URLs for the video streams.
         vid_stride (int): Video frame-rate stride, defaults to 1.
         buffer (bool): Whether to buffer input streams, defaults to False.
         running (bool): Flag to indicate if the streaming thread is running.
         mode (str): Set to 'stream' indicating real-time capture.
@@ -53,41 +51,47 @@
     Methods:
         __init__: Initialize the stream loader.
         update: Read stream frames in daemon thread.
         close: Close stream loader and release resources.
         __iter__: Returns an iterator object for the class.
         __next__: Returns source paths, transformed, and original images for processing.
         __len__: Return the length of the sources object.
+
+    Example:
+         ```bash
+         yolo predict source='rtsp://example.com/media.mp4'
+         ```
     """
 
     def __init__(self, sources="file.streams", vid_stride=1, buffer=False):
         """Initialize instance variables and check for consistent input stream shapes."""
         torch.backends.cudnn.benchmark = True  # faster for fixed-size inference
         self.buffer = buffer  # buffer input streams
         self.running = True  # running flag for Thread
         self.mode = "stream"
         self.vid_stride = vid_stride  # video frame-rate stride
 
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
+        self.bs = n
         self.fps = [0] * n  # frames per second
         self.frames = [0] * n
         self.threads = [None] * n
         self.caps = [None] * n  # video capture objects
         self.imgs = [[] for _ in range(n)]  # images
         self.shape = [[] for _ in range(n)]  # image shapes
         self.sources = [ops.clean_str(x) for x in sources]  # clean source names for later
         for i, s in enumerate(sources):  # index, source
             # Start thread to read frames from video stream
             st = f"{i + 1}/{n}: {s}... "
-            if urlparse(s).hostname in ("www.youtube.com", "youtube.com", "youtu.be"):  # if source is YouTube video
+            if urlparse(s).hostname in {"www.youtube.com", "youtube.com", "youtu.be"}:  # if source is YouTube video
                 # YouTube format i.e. 'https://www.youtube.com/watch?v=Zgi9g1ksQHc' or 'https://youtu.be/LNwODJXcvt4'
                 s = get_best_youtube_url(s)
             s = eval(s) if s.isnumeric() else s  # i.e. s = '0' local webcam
-            if s == 0 and (is_colab() or is_kaggle()):
+            if s == 0 and (IS_COLAB or IS_KAGGLE):
                 raise NotImplementedError(
                     "'source=0' webcam not supported in Colab and Kaggle notebooks. "
                     "Try running 'source=0' in a local environment."
                 )
             self.caps[i] = cv2.VideoCapture(s)  # store video capture object
             if not self.caps[i].isOpened():
                 raise ConnectionError(f"{st}Failed to open {s}")
@@ -105,17 +109,14 @@
             self.imgs[i].append(im)
             self.shape[i] = im.shape
             self.threads[i] = Thread(target=self.update, args=([i, self.caps[i], s]), daemon=True)
             LOGGER.info(f"{st}Success ✅ ({self.frames[i]} frames of shape {w}x{h} at {self.fps[i]:.2f} FPS)")
             self.threads[i].start()
         LOGGER.info("")  # newline
 
-        # Check for common shapes
-        self.bs = self.__len__()
-
     def update(self, i, cap, stream):
         """Read stream `i` frames in daemon thread."""
         n, f = 0, self.frames[i]  # frame number, frame array
         while self.running and cap.isOpened() and n < (f - 1):
             if len(self.imgs[i]) < 30:  # keep a <=30-image buffer
                 n += 1
                 cap.grab()  # .read() = .grab() followed by .retrieve()
@@ -171,19 +172,19 @@
                 images.append(x.pop(0))
 
             # Get the last frame, and clear the rest from the imgs buffer
             else:
                 images.append(x.pop(-1) if x else np.zeros(self.shape[i], dtype=np.uint8))
                 x.clear()
 
-        return self.sources, images, None, ""
+        return self.sources, images, [""] * self.bs
 
     def __len__(self):
         """Return the length of the sources object."""
-        return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
+        return self.bs  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 class LoadScreenshots:
     """
     YOLOv8 screenshot dataloader.
 
     This class manages the loading of screenshot images for processing with YOLOv8.
@@ -220,14 +221,15 @@
             left, top, width, height = (int(x) for x in params)
         elif len(params) == 5:
             self.screen, left, top, width, height = (int(x) for x in params)
         self.mode = "stream"
         self.frame = 0
         self.sct = mss.mss()
         self.bs = 1
+        self.fps = 30
 
         # Parse monitor shape
         monitor = self.sct.monitors[self.screen]
         self.top = monitor["top"] if top is None else (monitor["top"] + top)
         self.left = monitor["left"] if left is None else (monitor["left"] + left)
         self.width = width or monitor["width"]
         self.height = height or monitor["height"]
@@ -239,18 +241,18 @@
 
     def __next__(self):
         """mss screen capture: get raw pixels from the screen as np array."""
         im0 = np.asarray(self.sct.grab(self.monitor))[:, :, :3]  # BGRA to BGR
         s = f"screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: "
 
         self.frame += 1
-        return [str(self.screen)], [im0], None, s  # screen, img, vid_cap, string
+        return [str(self.screen)], [im0], [s]  # screen, img, string
 
 
-class LoadImages:
+class LoadImagesAndVideos:
     """
     YOLOv8 image/video dataloader.
 
     This class manages the loading and pre-processing of image and video data for YOLOv8. It supports loading from
     various formats, including single image files, video files, and lists of image and video paths.
 
     Attributes:
@@ -265,15 +267,15 @@
         frames (int): Total number of frames in the video.
         count (int): Counter for iteration, initialized at 0 during `__iter__()`.
 
     Methods:
         _new_video(path): Create a new cv2.VideoCapture object for a given video path.
     """
 
-    def __init__(self, path, vid_stride=1):
+    def __init__(self, path, batch=1, vid_stride=1):
         """Initialize the Dataloader and raise FileNotFoundError if file not found."""
         parent = None
         if isinstance(path, str) and Path(path).suffix == ".txt":  # *.txt file with img/vid/dir on each line
             parent = Path(path).parent
             path = Path(path).read_text().splitlines()  # list of sources
         files = []
         for p in sorted(path) if isinstance(path, (list, tuple)) else [path]:
@@ -285,83 +287,107 @@
             elif os.path.isfile(a):
                 files.append(a)  # files (absolute or relative to CWD)
             elif parent and (parent / p).is_file():
                 files.append(str((parent / p).absolute()))  # files (relative to *.txt file parent)
             else:
                 raise FileNotFoundError(f"{p} does not exist")
 
-        images = [x for x in files if x.split(".")[-1].lower() in IMG_FORMATS]
-        videos = [x for x in files if x.split(".")[-1].lower() in VID_FORMATS]
+        # Define files as images or videos
+        images, videos = [], []
+        for f in files:
+            suffix = f.split(".")[-1].lower()  # Get file extension without the dot and lowercase
+            if suffix in IMG_FORMATS:
+                images.append(f)
+            elif suffix in VID_FORMATS:
+                videos.append(f)
         ni, nv = len(images), len(videos)
 
         self.files = images + videos
         self.nf = ni + nv  # number of files
+        self.ni = ni  # number of images
         self.video_flag = [False] * ni + [True] * nv
         self.mode = "image"
         self.vid_stride = vid_stride  # video frame-rate stride
-        self.bs = 1
+        self.bs = batch
         if any(videos):
             self._new_video(videos[0])  # new video
         else:
             self.cap = None
         if self.nf == 0:
-            raise FileNotFoundError(
-                f"No images or videos found in {p}. "
-                f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
-            )
+            raise FileNotFoundError(f"No images or videos found in {p}. {FORMATS_HELP_MSG}")
 
     def __iter__(self):
         """Returns an iterator object for VideoStream or ImageFolder."""
         self.count = 0
         return self
 
     def __next__(self):
-        """Return next image, path and metadata from dataset."""
-        if self.count == self.nf:
-            raise StopIteration
-        path = self.files[self.count]
-
-        if self.video_flag[self.count]:
-            # Read video
-            self.mode = "video"
-            for _ in range(self.vid_stride):
-                self.cap.grab()
-            success, im0 = self.cap.retrieve()
-            while not success:
-                self.count += 1
-                self.cap.release()
-                if self.count == self.nf:  # last video
+        """Returns the next batch of images or video frames along with their paths and metadata."""
+        paths, imgs, info = [], [], []
+        while len(imgs) < self.bs:
+            if self.count >= self.nf:  # end of file list
+                if len(imgs) > 0:
+                    return paths, imgs, info  # return last partial batch
+                else:
                     raise StopIteration
-                path = self.files[self.count]
-                self._new_video(path)
-                success, im0 = self.cap.read()
-
-            self.frame += 1
-            # im0 = self._cv2_rotate(im0)  # for use if cv2 autorotation is False
-            s = f"video {self.count + 1}/{self.nf} ({self.frame}/{self.frames}) {path}: "
 
-        else:
-            # Read image
-            self.count += 1
-            im0 = cv2.imread(path)  # BGR
-            if im0 is None:
-                raise FileNotFoundError(f"Image Not Found {path}")
-            s = f"image {self.count}/{self.nf} {path}: "
+            path = self.files[self.count]
+            if self.video_flag[self.count]:
+                self.mode = "video"
+                if not self.cap or not self.cap.isOpened():
+                    self._new_video(path)
 
-        return [path], [im0], self.cap, s
+                for _ in range(self.vid_stride):
+                    success = self.cap.grab()
+                    if not success:
+                        break  # end of video or failure
+
+                if success:
+                    success, im0 = self.cap.retrieve()
+                    if success:
+                        self.frame += 1
+                        paths.append(path)
+                        imgs.append(im0)
+                        info.append(f"video {self.count + 1}/{self.nf} (frame {self.frame}/{self.frames}) {path}: ")
+                        if self.frame == self.frames:  # end of video
+                            self.count += 1
+                            self.cap.release()
+                else:
+                    # Move to the next file if the current video ended or failed to open
+                    self.count += 1
+                    if self.cap:
+                        self.cap.release()
+                    if self.count < self.nf:
+                        self._new_video(self.files[self.count])
+            else:
+                self.mode = "image"
+                im0 = cv2.imread(path)  # BGR
+                if im0 is None:
+                    raise FileNotFoundError(f"Image Not Found {path}")
+                paths.append(path)
+                imgs.append(im0)
+                info.append(f"image {self.count + 1}/{self.nf} {path}: ")
+                self.count += 1  # move to the next file
+                if self.count >= self.ni:  # end of image list
+                    break
+
+        return paths, imgs, info
 
     def _new_video(self, path):
-        """Create a new video capture object."""
+        """Creates a new video capture object for the given path."""
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
+        self.fps = int(self.cap.get(cv2.CAP_PROP_FPS))
+        if not self.cap.isOpened():
+            raise FileNotFoundError(f"Failed to open video {path}")
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT) / self.vid_stride)
 
     def __len__(self):
-        """Returns the number of files in the object."""
-        return self.nf  # number of files
+        """Returns the number of batches in the object."""
+        return math.ceil(self.nf / self.bs)  # number of files
 
 
 class LoadPilAndNumpy:
     """
     Load images from PIL and Numpy arrays for batch processing.
 
     This class is designed to manage loading and pre-processing of image data from both PIL and Numpy formats.
@@ -369,28 +395,26 @@
     downstream processing.
 
     Attributes:
         paths (list): List of image paths or autogenerated filenames.
         im0 (list): List of images stored as Numpy arrays.
         mode (str): Type of data being processed, defaults to 'image'.
         bs (int): Batch size, equivalent to the length of `im0`.
-        count (int): Counter for iteration, initialized at 0 during `__iter__()`.
 
     Methods:
         _single_check(im): Validate and format a single image to a Numpy array.
     """
 
     def __init__(self, im0):
         """Initialize PIL and Numpy Dataloader."""
         if not isinstance(im0, list):
             im0 = [im0]
         self.paths = [getattr(im, "filename", f"image{i}.jpg") for i, im in enumerate(im0)]
         self.im0 = [self._single_check(im) for im in im0]
         self.mode = "image"
-        # Generate fake paths
         self.bs = len(self.im0)
 
     @staticmethod
     def _single_check(im):
         """Validate and format an image to numpy array."""
         assert isinstance(im, (Image.Image, np.ndarray)), f"Expected PIL/np.ndarray image type, but got {type(im)}"
         if isinstance(im, Image.Image):
@@ -405,15 +429,15 @@
         return len(self.im0)
 
     def __next__(self):
         """Returns batch paths, images, processed images, None, ''."""
         if self.count == 1:  # loop only once as it's batch inference
             raise StopIteration
         self.count += 1
-        return self.paths, self.im0, None, ""
+        return self.paths, self.im0, [""] * self.bs
 
     def __iter__(self):
         """Enables iteration for class LoadPilAndNumpy."""
         self.count = 0
         return self
 
 
@@ -470,15 +494,15 @@
         return self
 
     def __next__(self):
         """Return next item in the iterator."""
         if self.count == 1:
             raise StopIteration
         self.count += 1
-        return self.paths, self.im0, None, ""
+        return self.paths, self.im0, [""] * self.bs
 
     def __len__(self):
         """Returns the batch size."""
         return self.bs
 
 
 def autocast_list(source):
@@ -494,17 +518,14 @@
                 f"type {type(im).__name__} is not a supported Ultralytics prediction source type. \n"
                 f"See https://docs.ultralytics.com/modes/predict for supported source types."
             )
 
     return files
 
 
-LOADERS = LoadStreams, LoadPilAndNumpy, LoadImages, LoadScreenshots  # tuple
-
-
 def get_best_youtube_url(url, use_pafy=True):
     """
     Retrieves the URL of the best quality MP4 video stream from a given YouTube video.
 
     This function uses the pafy or yt_dlp library to extract the video info from YouTube. It then finds the highest
     quality MP4 format that has video codec but no audio codec, and returns the URL of this video stream.
 
@@ -527,7 +548,11 @@
         with yt_dlp.YoutubeDL({"quiet": True}) as ydl:
             info_dict = ydl.extract_info(url, download=False)  # extract info
         for f in reversed(info_dict.get("formats", [])):  # reversed because best is usually last
             # Find a format with video codec, no audio, *.mp4 extension at least 1920x1080 size
             good_size = (f.get("width") or 0) >= 1920 or (f.get("height") or 0) >= 1080
             if good_size and f["vcodec"] != "none" and f["acodec"] == "none" and f["ext"] == "mp4":
                 return f.get("url")
+
+
+# Define constants
+LOADERS = (LoadStreams, LoadPilAndNumpy, LoadImagesAndVideos, LoadScreenshots)
```

### Comparing `ultralytics-8.1.9/ultralytics/data/split_dota.py` & `ultralytics-8.2.0/ultralytics/data/split_dota.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 - images
                     - train
                     - val
                 - labels
                     - train
                     - val
     """
-    assert split in ["train", "val"]
+    assert split in {"train", "val"}, f"Split must be 'train' or 'val', not {split}."
     im_dir = Path(data_root) / "images" / split
     assert im_dir.exists(), f"Can't find {im_dir}, please check your data root."
     im_files = glob(str(Path(data_root) / "images" / split / "*"))
     lb_files = img2label_paths(im_files)
     annos = []
     for im_file, lb_file in zip(im_files, lb_files):
         w, h = exif_size(Image.open(im_file))
```

### Comparing `ultralytics-8.1.9/ultralytics/data/utils.py` & `ultralytics-8.2.0/ultralytics/data/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,27 @@
     NUM_THREADS,
     ROOT,
     SETTINGS_YAML,
     TQDM,
     clean_url,
     colorstr,
     emojis,
+    is_dir_writeable,
     yaml_load,
     yaml_save,
 )
 from ultralytics.utils.checks import check_file, check_font, is_ascii
 from ultralytics.utils.downloads import download, safe_download, unzip_file
 from ultralytics.utils.ops import segments2boxes
 
 HELP_URL = "See https://docs.ultralytics.com/datasets/detect for dataset formatting guidance."
-IMG_FORMATS = "bmp", "dng", "jpeg", "jpg", "mpo", "png", "tif", "tiff", "webp", "pfm"  # image suffixes
-VID_FORMATS = "asf", "avi", "gif", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ts", "wmv", "webm"  # video suffixes
+IMG_FORMATS = {"bmp", "dng", "jpeg", "jpg", "mpo", "png", "tif", "tiff", "webp", "pfm"}  # image suffixes
+VID_FORMATS = {"asf", "avi", "gif", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ts", "wmv", "webm"}  # video suffixes
 PIN_MEMORY = str(os.getenv("PIN_MEMORY", True)).lower() == "true"  # global pin_memory for dataloaders
+FORMATS_HELP_MSG = f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
 
 
 def img2label_paths(img_paths):
     """Define label paths as a function of image paths."""
     sa, sb = f"{os.sep}images{os.sep}", f"{os.sep}labels{os.sep}"  # /images/, /labels/ substrings
     return [sb.join(x.rsplit(sa, 1)).rsplit(".", 1)[0] + ".txt" for x in img_paths]
 
@@ -58,15 +60,15 @@
     """Returns exif-corrected PIL size."""
     s = img.size  # (width, height)
     if img.format == "JPEG":  # only support JPEG images
         with contextlib.suppress(Exception):
             exif = img.getexif()
             if exif:
                 rotation = exif.get(274, None)  # the EXIF key for the orientation tag is 274
-                if rotation in [6, 8]:  # rotation 270 or 90
+                if rotation in {6, 8}:  # rotation 270 or 90
                     s = s[1], s[0]
     return s
 
 
 def verify_image(args):
     """Verify one image."""
     (im_file, cls), prefix = args
@@ -74,16 +76,16 @@
     nf, nc, msg = 0, 0, ""
     try:
         im = Image.open(im_file)
         im.verify()  # PIL verify
         shape = exif_size(im)  # image size
         shape = (shape[1], shape[0])  # hw
         assert (shape[0] > 9) & (shape[1] > 9), f"image size {shape} <10 pixels"
-        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}"
-        if im.format.lower() in ("jpg", "jpeg"):
+        assert im.format.lower() in IMG_FORMATS, f"Invalid image format {im.format}. {FORMATS_HELP_MSG}"
+        if im.format.lower() in {"jpg", "jpeg"}:
             with open(im_file, "rb") as f:
                 f.seek(-2, 2)
                 if f.read() != b"\xff\xd9":  # corrupt JPEG
                     ImageOps.exif_transpose(Image.open(im_file)).save(im_file, "JPEG", subsampling=0, quality=100)
                     msg = f"{prefix}WARNING ⚠️ {im_file}: corrupt JPEG restored and saved"
         nf = 1
     except Exception as e:
@@ -100,16 +102,16 @@
     try:
         # Verify images
         im = Image.open(im_file)
         im.verify()  # PIL verify
         shape = exif_size(im)  # image size
         shape = (shape[1], shape[0])  # hw
         assert (shape[0] > 9) & (shape[1] > 9), f"image size {shape} <10 pixels"
-        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}"
-        if im.format.lower() in ("jpg", "jpeg"):
+        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}. {FORMATS_HELP_MSG}"
+        if im.format.lower() in {"jpg", "jpeg"}:
             with open(im_file, "rb") as f:
                 f.seek(-2, 2)
                 if f.read() != b"\xff\xd9":  # corrupt JPEG
                     ImageOps.exif_transpose(Image.open(im_file)).save(im_file, "JPEG", subsampling=0, quality=100)
                     msg = f"{prefix}WARNING ⚠️ {im_file}: corrupt JPEG restored and saved"
 
         # Verify labels
@@ -299,15 +301,15 @@
     # Resolve paths
     path = Path(extract_dir or data.get("path") or Path(data.get("yaml_file", "")).parent)  # dataset root
     if not path.is_absolute():
         path = (DATASETS_DIR / path).resolve()
 
     # Set paths
     data["path"] = path  # download scripts
-    for k in "train", "val", "test":
+    for k in "train", "val", "test", "minival":
         if data.get(k):  # prepend path
             if isinstance(data[k], str):
                 x = (path / data[k]).resolve()
                 if not x.exists() and data[k].startswith("../"):
                     x = (path / data[k][3:]).resolve()
                 data[k] = str(x)
             else:
@@ -331,15 +333,15 @@
                 safe_download(url=s, dir=DATASETS_DIR, delete=True)
             elif s.startswith("bash "):  # bash script
                 LOGGER.info(f"Running {s} ...")
                 r = os.system(s)
             else:  # python script
                 exec(s, {"yaml": data})
             dt = f"({round(time.time() - t, 1)}s)"
-            s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in (0, None) else f"failure {dt} ❌"
+            s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in {0, None} else f"failure {dt} ❌"
             LOGGER.info(f"Dataset download {s}\n")
     check_font("Arial.ttf" if is_ascii(data["names"]) else "Arial.Unicode.ttf")  # download fonts
 
     return data  # dictionary
 
 
 def check_cls_dataset(dataset, split=""):
@@ -361,14 +363,17 @@
             - 'nc' (int): The number of classes in the dataset.
             - 'names' (dict): A dictionary of class names in the dataset.
     """
 
     # Download (optional if dataset=https://file.zip is passed directly)
     if str(dataset).startswith(("http:/", "https:/")):
         dataset = safe_download(dataset, dir=DATASETS_DIR, unzip=True, delete=False)
+    elif Path(dataset).suffix in {".zip", ".tar", ".gz"}:
+        file = check_file(dataset)
+        dataset = safe_download(file, dir=DATASETS_DIR, unzip=True, delete=False)
 
     dataset = Path(dataset)
     data_dir = (dataset if dataset.is_dir() else (DATASETS_DIR / dataset)).resolve()
     if not data_dir.is_dir():
         LOGGER.warning(f"\nDataset not found ⚠️, missing path {data_dir}, attempting download...")
         t = time.time()
         if str(dataset) == "imagenet":
@@ -463,15 +468,14 @@
                 data = check_det_dataset(yaml_path, autodownload)  # dict
                 data["path"] = data_dir  # YAML path should be set to '' (relative) or parent (absolute)
             except Exception as e:
                 raise Exception("error/HUB/dataset_stats/init") from e
 
         self.hub_dir = Path(f'{data["path"]}-hub')
         self.im_dir = self.hub_dir / "images"
-        self.im_dir.mkdir(parents=True, exist_ok=True)  # makes /images
         self.stats = {"nc": len(data["names"]), "names": list(data["names"].values())}  # statistics dictionary
         self.data = data
 
     @staticmethod
     def _unzip(path):
         """Unzip data.zip."""
         if not str(path).endswith(".zip"):  # path is data.yaml
@@ -547,26 +551,28 @@
                         "per_class": (x > 0).sum(0).tolist(),
                     },
                     "labels": [{Path(k).name: _round(v)} for k, v in zip(dataset.im_files, dataset.labels)],
                 }
 
         # Save, print and return
         if save:
+            self.hub_dir.mkdir(parents=True, exist_ok=True)  # makes dataset-hub/
             stats_path = self.hub_dir / "stats.json"
             LOGGER.info(f"Saving {stats_path.resolve()}...")
             with open(stats_path, "w") as f:
                 json.dump(self.stats, f)  # save stats.json
         if verbose:
             LOGGER.info(json.dumps(self.stats, indent=2, sort_keys=False))
         return self.stats
 
     def process_images(self):
         """Compress images for Ultralytics HUB."""
         from ultralytics.data import YOLODataset  # ClassificationDataset
 
+        self.im_dir.mkdir(parents=True, exist_ok=True)  # makes dataset-hub/images/
         for split in "train", "val", "test":
             if self.data.get(split) is None:
                 continue
             dataset = YOLODataset(img_path=self.data[split], data=self.data)
             with ThreadPool(NUM_THREADS) as pool:
                 for _ in TQDM(pool.imap(self._hub_ops, dataset.im_files), total=len(dataset), desc=f"{split} images"):
                     pass
@@ -641,7 +647,30 @@
             (path.parent / x).unlink()  # remove existing
 
     LOGGER.info(f"Autosplitting images from {path}" + ", using *.txt labeled images only" * annotated_only)
     for i, img in TQDM(zip(indices, files), total=n):
         if not annotated_only or Path(img2label_paths([str(img)])[0]).exists():  # check label
             with open(path.parent / txt[i], "a") as f:
                 f.write(f"./{img.relative_to(path.parent).as_posix()}" + "\n")  # add image to txt file
+
+
+def load_dataset_cache_file(path):
+    """Load an Ultralytics *.cache dictionary from path."""
+    import gc
+
+    gc.disable()  # reduce pickle load time https://github.com/ultralytics/ultralytics/pull/1585
+    cache = np.load(str(path), allow_pickle=True).item()  # load dict
+    gc.enable()
+    return cache
+
+
+def save_dataset_cache_file(prefix, path, x, version):
+    """Save an Ultralytics dataset *.cache dictionary x to path."""
+    x["version"] = version  # add cache version
+    if is_dir_writeable(path.parent):
+        if path.exists():
+            path.unlink()  # remove *.cache file if exists
+        np.save(str(path), x)  # save cache for next time
+        path.with_suffix(".cache.npy").rename(path)  # remove .npy suffix
+        LOGGER.info(f"{prefix}New cache created: {path}")
+    else:
+        LOGGER.warning(f"{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable, cache not saved.")
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/exporter.py` & `ultralytics-8.2.0/ultralytics/engine/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 CoreML                  | `coreml`                  | yolov8n.mlpackage
 TensorFlow SavedModel   | `saved_model`             | yolov8n_saved_model/
 TensorFlow GraphDef     | `pb`                      | yolov8n.pb
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
-ncnn                    | `ncnn`                    | yolov8n_ncnn_model/
+NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
 
 Requirements:
     $ pip install "ultralytics[export]"
 
 Python:
     from ultralytics import YOLO
     model = YOLO('yolov8n.pt')
@@ -37,21 +37,23 @@
                          yolov8n.engine             # TensorRT
                          yolov8n.mlpackage          # CoreML (macOS-only)
                          yolov8n_saved_model        # TensorFlow SavedModel
                          yolov8n.pb                 # TensorFlow GraphDef
                          yolov8n.tflite             # TensorFlow Lite
                          yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                          yolov8n_paddle_model       # PaddlePaddle
+                         yolov8n_ncnn_model         # NCNN
 
 TensorFlow.js:
     $ cd .. && git clone https://github.com/zldrobit/tfjs-yolov5-example.git && cd tfjs-yolov5-example
     $ npm install
     $ ln -s ../../yolov5/yolov8n_web_model public/yolov8n_web_model
     $ npm start
 """
+
 import json
 import os
 import shutil
 import subprocess
 import time
 import warnings
 from copy import deepcopy
@@ -62,54 +64,55 @@
 import torch
 
 from ultralytics.cfg import get_cfg
 from ultralytics.data.dataset import YOLODataset
 from ultralytics.data.utils import check_det_dataset
 from ultralytics.nn.autobackend import check_class_names, default_class_names
 from ultralytics.nn.modules import C2f, Detect, RTDETRDecoder
-from ultralytics.nn.tasks import DetectionModel, SegmentationModel
+from ultralytics.nn.tasks import DetectionModel, SegmentationModel, WorldModel
 from ultralytics.utils import (
     ARM64,
     DEFAULT_CFG,
     LINUX,
     LOGGER,
     MACOS,
+    PYTHON_VERSION,
     ROOT,
     WINDOWS,
     __version__,
     callbacks,
     colorstr,
     get_default_args,
     yaml_save,
 )
 from ultralytics.utils.checks import check_imgsz, check_is_path_safe, check_requirements, check_version
 from ultralytics.utils.downloads import attempt_download_asset, get_github_assets
 from ultralytics.utils.files import file_size, spaces_in_path
 from ultralytics.utils.ops import Profile
-from ultralytics.utils.torch_utils import get_latest_opset, select_device, smart_inference_mode
+from ultralytics.utils.torch_utils import TORCH_1_13, get_latest_opset, select_device, smart_inference_mode
 
 
 def export_formats():
     """YOLOv8 export formats."""
-    import pandas
+    import pandas  # scope for faster 'import ultralytics'
 
     x = [
         ["PyTorch", "-", ".pt", True, True],
         ["TorchScript", "torchscript", ".torchscript", True, True],
         ["ONNX", "onnx", ".onnx", True, True],
         ["OpenVINO", "openvino", "_openvino_model", True, False],
         ["TensorRT", "engine", ".engine", False, True],
         ["CoreML", "coreml", ".mlpackage", True, False],
         ["TensorFlow SavedModel", "saved_model", "_saved_model", True, True],
         ["TensorFlow GraphDef", "pb", ".pb", True, True],
         ["TensorFlow Lite", "tflite", ".tflite", True, False],
         ["TensorFlow Edge TPU", "edgetpu", "_edgetpu.tflite", True, False],
         ["TensorFlow.js", "tfjs", "_web_model", True, False],
         ["PaddlePaddle", "paddle", "_paddle_model", True, True],
-        ["ncnn", "ncnn", "_ncnn_model", True, True],
+        ["NCNN", "ncnn", "_ncnn_model", True, True],
     ]
     return pandas.DataFrame(x, columns=["Format", "Argument", "Suffix", "CPU", "GPU"])
 
 
 def gd_outputs(gd):
     """TensorFlow GraphDef model output node names."""
     name_list, input_list = [], []
@@ -153,29 +156,29 @@
 
         Args:
             cfg (str, optional): Path to a configuration file. Defaults to DEFAULT_CFG.
             overrides (dict, optional): Configuration overrides. Defaults to None.
             _callbacks (dict, optional): Dictionary of callback functions. Defaults to None.
         """
         self.args = get_cfg(cfg, overrides)
-        if self.args.format.lower() in ("coreml", "mlmodel"):  # fix attempt for protobuf<3.20.x errors
+        if self.args.format.lower() in {"coreml", "mlmodel"}:  # fix attempt for protobuf<3.20.x errors
             os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"  # must run before TensorBoard callback
 
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
     def __call__(self, model=None):
         """Returns list of exported files/dirs after running callbacks."""
         self.run_callbacks("on_export_start")
         t = time.time()
         fmt = self.args.format.lower()  # to lowercase
-        if fmt in ("tensorrt", "trt"):  # 'engine' aliases
+        if fmt in {"tensorrt", "trt"}:  # 'engine' aliases
             fmt = "engine"
-        if fmt in ("mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"):  # 'coreml' aliases
+        if fmt in {"mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"}:  # 'coreml' aliases
             fmt = "coreml"
         fmts = tuple(export_formats()["Argument"][1:])  # available export formats
         flags = [x == fmt for x in fmts]
         if sum(flags) != 1:
             raise ValueError(f"Invalid export format='{fmt}'. Valid formats are {fmts}")
         jit, onnx, xml, engine, coreml, saved_model, pb, tflite, edgetpu, tfjs, paddle, ncnn = flags  # export booleans
 
@@ -195,14 +198,21 @@
             assert not self.args.dynamic, "half=True not compatible with dynamic=True, i.e. use only one."
         self.imgsz = check_imgsz(self.args.imgsz, stride=model.stride, min_dim=2)  # check image size
         if self.args.optimize:
             assert not ncnn, "optimize=True not compatible with format='ncnn', i.e. use optimize=False"
             assert self.device.type == "cpu", "optimize=True not compatible with cuda devices, i.e. use device='cpu'"
         if edgetpu and not LINUX:
             raise SystemError("Edge TPU export only supported on Linux. See https://coral.ai/docs/edgetpu/compiler/")
+        if isinstance(model, WorldModel):
+            LOGGER.warning(
+                "WARNING ⚠️ YOLOWorld (original version) export is not supported to any format.\n"
+                "WARNING ⚠️ YOLOWorldv2 models (i.e. 'yolov8s-worldv2.pt') only support export to "
+                "(torchscript, onnx, openvino, engine, coreml) formats. "
+                "See https://docs.ultralytics.com/models/yolo-world for details."
+            )
 
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(
             getattr(model, "pt_path", None) or getattr(model, "yaml_file", None) or model.yaml.get("yaml_file", "")
         )
         if file.suffix in {".yaml", ".yml"}:
@@ -212,15 +222,15 @@
         model = deepcopy(model).to(self.device)
         for p in model.parameters():
             p.requires_grad = False
         model.eval()
         model.float()
         model = model.fuse()
         for m in model.modules():
-            if isinstance(m, (Detect, RTDETRDecoder)):  # Segment and Pose use Detect base class
+            if isinstance(m, (Detect, RTDETRDecoder)):  # includes all Detect subclasses like Segment, Pose, OBB
                 m.dynamic = self.args.dynamic
                 m.export = True
                 m.format = self.args.format
             elif isinstance(m, C2f) and not any((saved_model, pb, tflite, edgetpu, tfjs)):
                 # EdgeTPU does not support FlexSplitV while split provides cleaner ONNX graph
                 m.forward = m.forward_split
 
@@ -246,17 +256,18 @@
         )
         self.pretty_name = Path(self.model.yaml.get("yaml_file", self.file)).stem.replace("yolo", "YOLO")
         data = model.args["data"] if hasattr(model, "args") and isinstance(model.args, dict) else ""
         description = f'Ultralytics {self.pretty_name} model {f"trained on {data}" if data else ""}'
         self.metadata = {
             "description": description,
             "author": "Ultralytics",
-            "license": "AGPL-3.0 https://ultralytics.com/license",
             "date": datetime.now().isoformat(),
             "version": __version__,
+            "license": "AGPL-3.0 License (https://ultralytics.com/license)",
+            "docs": "https://docs.ultralytics.com",
             "stride": int(max(model.stride)),
             "task": model.task,
             "batch": self.args.batch,
             "imgsz": self.imgsz,
             "names": model.names,
         }  # model metadata
         if model.task == "pose":
@@ -269,15 +280,15 @@
 
         # Exports
         f = [""] * len(fmts)  # exported filenames
         if jit or ncnn:  # TorchScript
             f[0], _ = self.export_torchscript()
         if engine:  # TensorRT required before ONNX
             f[1], _ = self.export_engine()
-        if onnx or xml:  # OpenVINO requires ONNX
+        if onnx:  # ONNX
             f[2], _ = self.export_onnx()
         if xml:  # OpenVINO
             f[3], _ = self.export_openvino()
         if coreml:  # CoreML
             f[4], _ = self.export_coreml()
         if any((saved_model, pb, tflite, edgetpu, tfjs)):  # TensorFlow formats
             self.args.int8 |= edgetpu
@@ -288,15 +299,15 @@
                 f[7], _ = self.export_tflite(keras_model=keras_model, nms=False, agnostic_nms=self.args.agnostic_nms)
             if edgetpu:
                 f[8], _ = self.export_edgetpu(tflite_model=Path(f[5]) / f"{self.file.stem}_full_integer_quant.tflite")
             if tfjs:
                 f[9], _ = self.export_tfjs()
         if paddle:  # PaddlePaddle
             f[10], _ = self.export_paddle()
-        if ncnn:  # ncnn
+        if ncnn:  # NCNN
             f[11], _ = self.export_ncnn()
 
         # Finish
         f = [str(x) for x in f if x]  # filter out '' and None
         if any(f):
             f = str(Path(f[-1]))
             square = self.imgsz[0] == self.imgsz[1]
@@ -339,14 +350,16 @@
 
     @try_export
     def export_onnx(self, prefix=colorstr("ONNX:")):
         """YOLOv8 ONNX export."""
         requirements = ["onnx>=1.12.0"]
         if self.args.simplify:
             requirements += ["onnxsim>=0.4.33", "onnxruntime-gpu" if torch.cuda.is_available() else "onnxruntime"]
+            if ARM64:
+                check_requirements("cmake")  # 'cmake' is needed to build onnxsim on aarch64
         check_requirements(requirements)
         import onnx  # noqa
 
         opset_version = self.args.opset or get_latest_opset()
         LOGGER.info(f"\n{prefix} starting export with onnx {onnx.__version__} opset {opset_version}...")
         f = str(self.file.with_suffix(".onnx"))
 
@@ -395,76 +408,93 @@
 
         onnx.save(model_onnx, f)
         return f, model_onnx
 
     @try_export
     def export_openvino(self, prefix=colorstr("OpenVINO:")):
         """YOLOv8 OpenVINO export."""
-        check_requirements("openvino-dev>=2023.0")  # requires openvino-dev: https://pypi.org/project/openvino-dev/
-        import openvino.runtime as ov  # noqa
-        from openvino.tools import mo  # noqa
+        check_requirements("openvino>=2024.0.0")  # requires openvino: https://pypi.org/project/openvino/
+        import openvino as ov
 
         LOGGER.info(f"\n{prefix} starting export with openvino {ov.__version__}...")
-        f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
-        fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
-        f_onnx = self.file.with_suffix(".onnx")
-        f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
-        fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
+        assert TORCH_1_13, f"OpenVINO export requires torch>=1.13.0 but torch=={torch.__version__} is installed"
+        ov_model = ov.convert_model(
+            self.model.cpu(),
+            input=None if self.args.dynamic else [self.im.shape],
+            example_input=self.im,
+        )
 
         def serialize(ov_model, file):
             """Set RT info, serialize and save metadata YAML."""
             ov_model.set_rt_info("YOLOv8", ["model_info", "model_type"])
             ov_model.set_rt_info(True, ["model_info", "reverse_input_channels"])
             ov_model.set_rt_info(114, ["model_info", "pad_value"])
             ov_model.set_rt_info([255.0], ["model_info", "scale_values"])
             ov_model.set_rt_info(self.args.iou, ["model_info", "iou_threshold"])
             ov_model.set_rt_info([v.replace(" ", "_") for v in self.model.names.values()], ["model_info", "labels"])
             if self.model.task != "classify":
                 ov_model.set_rt_info("fit_to_window_letterbox", ["model_info", "resize_type"])
 
-            ov.serialize(ov_model, file)  # save
+            ov.runtime.save_model(ov_model, file, compress_to_fp16=self.args.half)
             yaml_save(Path(file).parent / "metadata.yaml", self.metadata)  # add metadata.yaml
 
-        ov_model = mo.convert_model(
-            f_onnx, model_name=self.pretty_name, framework="onnx", compress_to_fp16=self.args.half
-        )  # export
-
         if self.args.int8:
+            fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
+            fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
             if not self.args.data:
                 self.args.data = DEFAULT_CFG.data or "coco128.yaml"
                 LOGGER.warning(
                     f"{prefix} WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
                     f"Using default 'data={self.args.data}'."
                 )
-            check_requirements("nncf>=2.5.0")
+            check_requirements("nncf>=2.8.0")
             import nncf
 
             def transform_fn(data_item):
                 """Quantization transform function."""
                 assert (
                     data_item["img"].dtype == torch.uint8
                 ), "Input image must be uint8 for the quantization preprocessing"
                 im = data_item["img"].numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
                 return np.expand_dims(im, 0) if im.ndim == 3 else im
 
             # Generate calibration data for integer quantization
             LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
             data = check_det_dataset(self.args.data)
-            dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
+            dataset = YOLODataset(data["val"], data=data, task=self.model.task, imgsz=self.imgsz[0], augment=False)
             n = len(dataset)
             if n < 300:
                 LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
             quantization_dataset = nncf.Dataset(dataset, transform_fn)
-            ignored_scope = nncf.IgnoredScope(types=["Multiply", "Subtract", "Sigmoid"])  # ignore operation
+
+            ignored_scope = None
+            if isinstance(self.model.model[-1], Detect):
+                # Includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
+                head_module_name = ".".join(list(self.model.named_modules())[-1][0].split(".")[:2])
+
+                ignored_scope = nncf.IgnoredScope(  # ignore operations
+                    patterns=[
+                        f".*{head_module_name}/.*/Add",
+                        f".*{head_module_name}/.*/Sub*",
+                        f".*{head_module_name}/.*/Mul*",
+                        f".*{head_module_name}/.*/Div*",
+                        f".*{head_module_name}\\.dfl.*",
+                    ],
+                    types=["Sigmoid"],
+                )
+
             quantized_ov_model = nncf.quantize(
                 ov_model, quantization_dataset, preset=nncf.QuantizationPreset.MIXED, ignored_scope=ignored_scope
             )
             serialize(quantized_ov_model, fq_ov)
             return fq, None
 
+        f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
+        f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
+
         serialize(ov_model, f_ov)
         return f, None
 
     @try_export
     def export_paddle(self, prefix=colorstr("PaddlePaddle:")):
         """YOLOv8 Paddle export."""
         check_requirements(("paddlepaddle", "x2paddle"))
@@ -475,39 +505,40 @@
         f = str(self.file).replace(self.file.suffix, f"_paddle_model{os.sep}")
 
         pytorch2paddle(module=self.model, save_dir=f, jit_type="trace", input_examples=[self.im])  # export
         yaml_save(Path(f) / "metadata.yaml", self.metadata)  # add metadata.yaml
         return f, None
 
     @try_export
-    def export_ncnn(self, prefix=colorstr("ncnn:")):
+    def export_ncnn(self, prefix=colorstr("NCNN:")):
         """
-        YOLOv8 ncnn export using PNNX https://github.com/pnnx/pnnx.
+        YOLOv8 NCNN export using PNNX https://github.com/pnnx/pnnx.
         """
-        check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires ncnn
+        check_requirements("ncnn")
         import ncnn  # noqa
 
-        LOGGER.info(f"\n{prefix} starting export with ncnn {ncnn.__version__}...")
+        LOGGER.info(f"\n{prefix} starting export with NCNN {ncnn.__version__}...")
         f = Path(str(self.file).replace(self.file.suffix, f"_ncnn_model{os.sep}"))
         f_ts = self.file.with_suffix(".torchscript")
 
         name = Path("pnnx.exe" if WINDOWS else "pnnx")  # PNNX filename
         pnnx = name if name.is_file() else ROOT / name
         if not pnnx.is_file():
             LOGGER.warning(
                 f"{prefix} WARNING ⚠️ PNNX not found. Attempting to download binary file from "
                 "https://github.com/pnnx/pnnx/.\nNote PNNX Binary file must be placed in current working directory "
                 f"or in {ROOT}. See PNNX repo for full installation instructions."
             )
-            system = ["macos"] if MACOS else ["windows"] if WINDOWS else ["ubuntu", "linux"]  # operating system
+            system = "macos" if MACOS else "windows" if WINDOWS else "linux-aarch64" if ARM64 else "linux"
             try:
-                _, assets = get_github_assets(repo="pnnx/pnnx", retry=True)
-                url = [x for x in assets if any(s in x for s in system)][0]
+                _, assets = get_github_assets(repo="pnnx/pnnx")
+                url = [x for x in assets if f"{system}.zip" in x][0]
+                assert url, "Unable to retrieve PNNX repo assets"
             except Exception as e:
-                url = f"https://github.com/pnnx/pnnx/releases/download/20231127/pnnx-20231127-{system[0]}.zip"
+                url = f"https://github.com/pnnx/pnnx/releases/download/20240410/pnnx-20240410-{system}.zip"
                 LOGGER.warning(f"{prefix} WARNING ⚠️ PNNX GitHub assets not found: {e}, using default {url}")
             asset = attempt_download_asset(url, repo="pnnx/pnnx", release="latest")
             if check_is_path_safe(Path.cwd(), asset):  # avoid path traversal security vulnerability
                 unzip_dir = Path(asset).with_suffix("")
                 (unzip_dir / name).rename(pnnx)  # move binary to ROOT
                 shutil.rmtree(unzip_dir)  # delete unzip dir
                 Path(asset).unlink()  # delete zip
@@ -591,18 +622,16 @@
                 import coremltools.optimize.coreml as cto
 
                 op_config = cto.OpPalettizerConfig(mode="kmeans", nbits=bits, weight_threshold=512)
                 config = cto.OptimizationConfig(global_config=op_config)
                 ct_model = cto.palettize_weights(ct_model, config=config)
         if self.args.nms and self.model.task == "detect":
             if mlmodel:
-                import platform
-
                 # coremltools<=6.2 NMS export requires Python<3.11
-                check_version(platform.python_version(), "<3.11", name="Python ", hard=True)
+                check_version(PYTHON_VERSION, "<3.11", name="Python ", hard=True)
                 weights_dir = None
             else:
                 ct_model.save(str(f))  # save otherwise weights_dir does not exist
                 weights_dir = str(f / "Data/com.apple.CoreML/weights")
             ct_model = self._pipeline_coreml(ct_model, weights_dir=weights_dir)
 
         m = self.metadata  # metadata dict
@@ -622,39 +651,40 @@
             ct_model.save(str(f))
         return f, ct_model
 
     @try_export
     def export_engine(self, prefix=colorstr("TensorRT:")):
         """YOLOv8 TensorRT export https://developer.nvidia.com/tensorrt."""
         assert self.im.device.type != "cpu", "export running on CPU but must be on GPU, i.e. use 'device=0'"
+        self.args.simplify = True
         f_onnx, _ = self.export_onnx()  # run before trt import https://github.com/ultralytics/ultralytics/issues/7016
 
         try:
             import tensorrt as trt  # noqa
         except ImportError:
             if LINUX:
                 check_requirements("nvidia-tensorrt", cmds="-U --index-url https://pypi.ngc.nvidia.com")
             import tensorrt as trt  # noqa
-
         check_version(trt.__version__, "7.0.0", hard=True)  # require tensorrt>=7.0.0
 
-        self.args.simplify = True
-
         LOGGER.info(f"\n{prefix} starting export with TensorRT {trt.__version__}...")
+        is_trt10 = int(trt.__version__.split(".")[0]) >= 10  # is TensorRT >= 10
         assert Path(f_onnx).exists(), f"failed to export ONNX file: {f_onnx}"
         f = self.file.with_suffix(".engine")  # TensorRT engine file
         logger = trt.Logger(trt.Logger.INFO)
         if self.args.verbose:
             logger.min_severity = trt.Logger.Severity.VERBOSE
 
         builder = trt.Builder(logger)
         config = builder.create_builder_config()
-        config.max_workspace_size = self.args.workspace * 1 << 30
-        # config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, workspace << 30)  # fix TRT 8.4 deprecation notice
-
+        workspace = int(self.args.workspace * (1 << 30))
+        if is_trt10:
+            config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, workspace)
+        else:  # TensorRT versions 7, 8
+            config.max_workspace_size = workspace
         flag = 1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
         network = builder.create_network(flag)
         parser = trt.OnnxParser(network, logger)
         if not parser.parse_from_file(f_onnx):
             raise RuntimeError(f"failed to load ONNX file: {f_onnx}")
 
         inputs = [network.get_input(i) for i in range(network.num_inputs)]
@@ -665,87 +695,97 @@
             LOGGER.info(f'{prefix} output "{out.name}" with shape{out.shape} {out.dtype}')
 
         if self.args.dynamic:
             shape = self.im.shape
             if shape[0] <= 1:
                 LOGGER.warning(f"{prefix} WARNING ⚠️ 'dynamic=True' model requires max batch size, i.e. 'batch=16'")
             profile = builder.create_optimization_profile()
+            min_shape = (1, shape[1], 32, 32)  # minimum input shape
+            opt_shape = (max(1, shape[0] // 2), *shape[1:])  # optimal input shape
+            max_shape = (*shape[:2], *(max(1, self.args.workspace) * d for d in shape[2:]))  # max input shape
             for inp in inputs:
-                profile.set_shape(inp.name, (1, *shape[1:]), (max(1, shape[0] // 2), *shape[1:]), shape)
+                profile.set_shape(inp.name, min_shape, opt_shape, max_shape)
             config.add_optimization_profile(profile)
 
-        LOGGER.info(
-            f"{prefix} building FP{16 if builder.platform_has_fast_fp16 and self.args.half else 32} engine as {f}"
-        )
-        if builder.platform_has_fast_fp16 and self.args.half:
+        half = builder.platform_has_fast_fp16 and self.args.half
+        LOGGER.info(f"{prefix} building FP{16 if half else 32} engine as {f}")
+        if half:
             config.set_flag(trt.BuilderFlag.FP16)
 
+        # Free CUDA memory
         del self.model
         torch.cuda.empty_cache()
 
         # Write file
-        with builder.build_engine(network, config) as engine, open(f, "wb") as t:
+        build = builder.build_serialized_network if is_trt10 else builder.build_engine
+        with build(network, config) as engine, open(f, "wb") as t:
             # Metadata
             meta = json.dumps(self.metadata)
             t.write(len(meta).to_bytes(4, byteorder="little", signed=True))
             t.write(meta.encode())
             # Model
-            t.write(engine.serialize())
+            t.write(engine if is_trt10 else engine.serialize())
 
         return f, None
 
     @try_export
     def export_saved_model(self, prefix=colorstr("TensorFlow SavedModel:")):
         """YOLOv8 TensorFlow SavedModel export."""
         cuda = torch.cuda.is_available()
         try:
             import tensorflow as tf  # noqa
         except ImportError:
-            check_requirements(f"tensorflow{'-macos' if MACOS else '-aarch64' if ARM64 else '' if cuda else '-cpu'}")
+            suffix = "-macos" if MACOS else "-aarch64" if ARM64 else "" if cuda else "-cpu"
+            version = "" if ARM64 else "<=2.13.1"
+            check_requirements(f"tensorflow{suffix}{version}")
             import tensorflow as tf  # noqa
+        if ARM64:
+            check_requirements("cmake")  # 'cmake' is needed to build onnxsim on aarch64
         check_requirements(
             (
-                "onnx",
+                "onnx>=1.12.0",
                 "onnx2tf>=1.15.4,<=1.17.5",
                 "sng4onnx>=1.0.1",
                 "onnxsim>=0.4.33",
                 "onnx_graphsurgeon>=0.3.26",
                 "tflite_support",
+                "flatbuffers>=23.5.26,<100",  # update old 'flatbuffers' included inside tensorflow package
                 "onnxruntime-gpu" if cuda else "onnxruntime",
             ),
             cmds="--extra-index-url https://pypi.ngc.nvidia.com",
         )  # onnx_graphsurgeon only on NVIDIA
 
         LOGGER.info(f"\n{prefix} starting export with tensorflow {tf.__version__}...")
         check_version(
             tf.__version__,
             "<=2.13.1",
             name="tensorflow",
             verbose=True,
             msg="https://github.com/ultralytics/ultralytics/issues/5161",
         )
+        import onnx2tf
+
         f = Path(str(self.file).replace(self.file.suffix, "_saved_model"))
         if f.is_dir():
-            import shutil
-
             shutil.rmtree(f)  # delete output folder
 
         # Pre-download calibration file to fix https://github.com/PINTO0309/onnx2tf/issues/545
         onnx2tf_file = Path("calibration_image_sample_data_20x128x128x3_float32.npy")
         if not onnx2tf_file.exists():
             attempt_download_asset(f"{onnx2tf_file}.zip", unzip=True, delete=True)
 
         # Export to ONNX
         self.args.simplify = True
         f_onnx, _ = self.export_onnx()
 
         # Export to TF
         tmp_file = f / "tmp_tflite_int8_calibration_images.npy"  # int8 calibration images file
+        np_data = None
         if self.args.int8:
-            verbosity = "--verbosity info"
+            verbosity = "info"
             if self.args.data:
                 # Generate calibration data for integer quantization
                 LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
                 data = check_det_dataset(self.args.data)
                 dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
                 images = []
                 for i, batch in enumerate(dataset):
@@ -754,24 +794,28 @@
                     im = batch["img"].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC
                     images.append(im)
                 f.mkdir()
                 images = torch.cat(images, 0).float()
                 # mean = images.view(-1, 3).mean(0)  # imagenet mean [123.675, 116.28, 103.53]
                 # std = images.view(-1, 3).std(0)  # imagenet std [58.395, 57.12, 57.375]
                 np.save(str(tmp_file), images.numpy())  # BHWC
-                int8 = f'-oiqt -qt per-tensor -cind images "{tmp_file}" "[[[[0, 0, 0]]]]" "[[[[255, 255, 255]]]]"'
-            else:
-                int8 = "-oiqt -qt per-tensor"
+                np_data = [["images", tmp_file, [[[[0, 0, 0]]]], [[[[255, 255, 255]]]]]]
         else:
-            verbosity = "--non_verbose"
-            int8 = ""
+            verbosity = "error"
 
-        cmd = f'onnx2tf -i "{f_onnx}" -o "{f}" -nuo {verbosity} {int8}'.strip()
-        LOGGER.info(f"{prefix} running '{cmd}'")
-        subprocess.run(cmd, shell=True)
+        LOGGER.info(f"{prefix} starting TFLite export with onnx2tf {onnx2tf.__version__}...")
+        onnx2tf.convert(
+            input_onnx_file_path=f_onnx,
+            output_folder_path=str(f),
+            not_use_onnxsim=True,
+            verbosity=verbosity,
+            output_integer_quantized_tflite=self.args.int8,
+            quant_type="per-tensor",  # "per-tensor" (faster) or "per-channel" (slower but more accurate)
+            custom_input_op_name_np_data_path=np_data,
+        )
         yaml_save(f / "metadata.yaml", self.metadata)  # add metadata.yaml
 
         # Remove/rename TFLite models
         if self.args.int8:
             tmp_file.unlink(missing_ok=True)
             for file in f.rglob("*_dynamic_range_quant.tflite"):
                 file.rename(file.with_name(file.stem.replace("_dynamic_range_quant", "_int8") + file.suffix))
@@ -844,16 +888,18 @@
         subprocess.run(cmd, shell=True)
         self._add_tflite_metadata(f)
         return f, None
 
     @try_export
     def export_tfjs(self, prefix=colorstr("TensorFlow.js:")):
         """YOLOv8 TensorFlow.js export."""
-        # JAX bug requiring install constraints in https://github.com/google/jax/issues/18978
-        check_requirements(["jax<=0.4.21", "jaxlib<=0.4.21", "tensorflowjs"])
+        check_requirements("tensorflowjs")
+        if ARM64:
+            # Fix error: `np.object` was a deprecated alias for the builtin `object` when exporting to TF.js on ARM64
+            check_requirements("numpy==1.23.5")
         import tensorflow as tf
         import tensorflowjs as tfjs  # noqa
 
         LOGGER.info(f"\n{prefix} starting export with tensorflowjs {tfjs.__version__}...")
         f = str(self.file).replace(self.file.suffix, "_web_model")  # js dir
         f_pb = str(self.file.with_suffix(".pb"))  # *.pb path
 
@@ -861,15 +907,18 @@
         with open(f_pb, "rb") as file:
             gd.ParseFromString(file.read())
         outputs = ",".join(gd_outputs(gd))
         LOGGER.info(f"\n{prefix} output node names: {outputs}")
 
         quantization = "--quantize_float16" if self.args.half else "--quantize_uint8" if self.args.int8 else ""
         with spaces_in_path(f_pb) as fpb_, spaces_in_path(f) as f_:  # exporter can not handle spaces in path
-            cmd = f'tensorflowjs_converter --input_format=tf_frozen_model {quantization} --output_node_names={outputs} "{fpb_}" "{f_}"'
+            cmd = (
+                "tensorflowjs_converter "
+                f'--input_format=tf_frozen_model {quantization} --output_node_names={outputs} "{fpb_}" "{f_}"'
+            )
             LOGGER.info(f"{prefix} running '{cmd}'")
             subprocess.run(cmd, shell=True)
 
         if " " in f:
             LOGGER.warning(f"{prefix} WARNING ⚠️ your model may not work correctly with spaces in path '{f}'.")
 
         # f_json = Path(f) / 'model.json'  # *.json path
@@ -1056,18 +1105,18 @@
         pipeline.spec.description.metadata.userDefined.update(
             {"IoU threshold": str(nms.iouThreshold), "Confidence threshold": str(nms.confidenceThreshold)}
         )
 
         # Save the model
         model = ct.models.MLModel(pipeline.spec, weights_dir=weights_dir)
         model.input_description["image"] = "Input image"
-        model.input_description["iouThreshold"] = f"(optional) IOU threshold override (default: {nms.iouThreshold})"
-        model.input_description[
-            "confidenceThreshold"
-        ] = f"(optional) Confidence threshold override (default: {nms.confidenceThreshold})"
+        model.input_description["iouThreshold"] = f"(optional) IoU threshold override (default: {nms.iouThreshold})"
+        model.input_description["confidenceThreshold"] = (
+            f"(optional) Confidence threshold override (default: {nms.confidenceThreshold})"
+        )
         model.output_description["confidence"] = 'Boxes × Class confidence (see user-defined metadata "classes")'
         model.output_description["coordinates"] = "Boxes × [x, y, width, height] (relative to image size)"
         LOGGER.info(f"{prefix} pipeline success")
         return model
 
     def add_callback(self, event: str, callback):
         """Appends the given callback."""
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/model.py` & `ultralytics-8.2.0/ultralytics/engine/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import inspect
-import sys
 from pathlib import Path
 from typing import Union
 
+import numpy as np
+import torch
+
 from ultralytics.cfg import TASK2DATA, get_cfg, get_save_dir
 from ultralytics.hub.utils import HUB_WEB_ROOT
 from ultralytics.nn.tasks import attempt_load_one_weight, guess_model_task, nn, yaml_model_load
-from ultralytics.utils import ASSETS, DEFAULT_CFG_DICT, LOGGER, RANK, SETTINGS, callbacks, checks, emojis, yaml_load
+from ultralytics.utils import (
+    ARGV,
+    ASSETS,
+    DEFAULT_CFG_DICT,
+    LOGGER,
+    RANK,
+    SETTINGS,
+    callbacks,
+    checks,
+    emojis,
+    yaml_load,
+)
 
 
 class Model(nn.Module):
     """
     A base class for implementing YOLO models, unifying APIs across different model types.
 
     This class provides a common interface for various operations related to YOLO models, such as training,
@@ -74,15 +87,20 @@
         ValueError: If the model file or configuration is invalid or unsupported.
         ImportError: If required dependencies for specific model types (like HUB SDK) are not installed.
         TypeError: If the model is not a PyTorch model when required.
         AttributeError: If required attributes or methods are not implemented or available.
         NotImplementedError: If a specific model task or mode is not supported.
     """
 
-    def __init__(self, model: Union[str, Path] = "yolov8n.pt", task=None, verbose=False) -> None:
+    def __init__(
+        self,
+        model: Union[str, Path] = "yolov8n.pt",
+        task: str = None,
+        verbose: bool = False,
+    ) -> None:
         """
         Initializes a new instance of the YOLO model class.
 
         This constructor sets up the model based on the provided model path or name. It handles various types of model
         sources, including local files, Ultralytics HUB models, and Triton Server models. The method initializes several
         important attributes of the model and prepares it for operations like training, prediction, or export.
 
@@ -107,51 +125,54 @@
         self.ckpt = None  # if loaded from *.pt
         self.cfg = None  # if loaded from *.yaml
         self.ckpt_path = None
         self.overrides = {}  # overrides for trainer object
         self.metrics = None  # validation/training metrics
         self.session = None  # HUB session
         self.task = task  # task type
-        self.model_name = model = str(model).strip()  # strip spaces
+        model = str(model).strip()
 
         # Check if Ultralytics HUB model from https://hub.ultralytics.com
         if self.is_hub_model(model):
             # Fetch model from HUB
-            checks.check_requirements("hub-sdk>0.0.2")
+            checks.check_requirements("hub-sdk>=0.0.6")
             self.session = self._get_hub_session(model)
             model = self.session.model_file
 
         # Check if Triton Server model
         elif self.is_triton_model(model):
-            self.model = model
+            self.model_name = self.model = model
             self.task = task
             return
 
         # Load or create new YOLO model
-        model = checks.check_model_file_from_stem(model)  # add suffix, i.e. yolov8n -> yolov8n.pt
-        if Path(model).suffix in (".yaml", ".yml"):
+        if Path(model).suffix in {".yaml", ".yml"}:
             self._new(model, task=task, verbose=verbose)
         else:
             self._load(model, task=task)
 
-        self.model_name = model
-
-    def __call__(self, source=None, stream=False, **kwargs):
+    def __call__(
+        self,
+        source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
+        stream: bool = False,
+        **kwargs,
+    ) -> list:
         """
         An alias for the predict method, enabling the model instance to be callable.
 
         This method simplifies the process of making predictions by allowing the model instance to be called directly
         with the required arguments for prediction.
 
         Args:
-            source (str | int | PIL.Image | np.ndarray, optional): The source of the image for making predictions.
-                Accepts various types, including file paths, URLs, PIL images, and numpy arrays. Defaults to None.
+            source (str | Path | int | PIL.Image | np.ndarray, optional): The source of the image for making
+                predictions. Accepts various types, including file paths, URLs, PIL images, and numpy arrays.
+                Defaults to None.
             stream (bool, optional): If True, treats the input source as a continuous stream for predictions.
                 Defaults to False.
-            **kwargs (dict): Additional keyword arguments for configuring the prediction process.
+            **kwargs (any): Additional keyword arguments for configuring the prediction process.
 
         Returns:
             (List[ultralytics.engine.results.Results]): A list of prediction results, encapsulated in the Results class.
         """
         return self.predict(source, stream, **kwargs)
 
     @staticmethod
@@ -159,33 +180,33 @@
         """Creates a session for Hub Training."""
         from ultralytics.hub.session import HUBTrainingSession
 
         session = HUBTrainingSession(model)
         return session if session.client.authenticated else None
 
     @staticmethod
-    def is_triton_model(model):
+    def is_triton_model(model: str) -> bool:
         """Is model a Triton Server URL string, i.e. <scheme>://<netloc>/<endpoint>/<task_name>"""
         from urllib.parse import urlsplit
 
         url = urlsplit(model)
         return url.netloc and url.path and url.scheme in {"http", "grpc"}
 
     @staticmethod
-    def is_hub_model(model):
+    def is_hub_model(model: str) -> bool:
         """Check if the provided model is a HUB model."""
         return any(
             (
                 model.startswith(f"{HUB_WEB_ROOT}/models/"),  # i.e. https://hub.ultralytics.com/models/MODEL_ID
-                [len(x) for x in model.split("_")] == [42, 20],  # APIKEY_MODELID
-                len(model) == 20 and not Path(model).exists() and all(x not in model for x in "./\\"),  # MODELID
+                [len(x) for x in model.split("_")] == [42, 20],  # APIKEY_MODEL
+                len(model) == 20 and not Path(model).exists() and all(x not in model for x in "./\\"),  # MODEL
             )
         )
 
-    def _new(self, cfg: str, task=None, model=None, verbose=False):
+    def _new(self, cfg: str, task=None, model=None, verbose=False) -> None:
         """
         Initializes a new model and infers the task type from the model definitions.
 
         Args:
             cfg (str): model configuration file
             task (str | None): model task
             model (BaseModel): Customized model.
@@ -197,51 +218,56 @@
         self.model = (model or self._smart_load("model"))(cfg_dict, verbose=verbose and RANK == -1)  # build model
         self.overrides["model"] = self.cfg
         self.overrides["task"] = self.task
 
         # Below added to allow export from YAMLs
         self.model.args = {**DEFAULT_CFG_DICT, **self.overrides}  # combine default and model args (prefer model args)
         self.model.task = self.task
+        self.model_name = cfg
 
-    def _load(self, weights: str, task=None):
+    def _load(self, weights: str, task=None) -> None:
         """
         Initializes a new model and infers the task type from the model head.
 
         Args:
             weights (str): model checkpoint to be loaded
             task (str | None): model task
         """
-        suffix = Path(weights).suffix
-        if suffix == ".pt":
+        if weights.lower().startswith(("https://", "http://", "rtsp://", "rtmp://", "tcp://")):
+            weights = checks.check_file(weights)  # automatically download and return local filename
+        weights = checks.check_model_file_from_stem(weights)  # add suffix, i.e. yolov8n -> yolov8n.pt
+
+        if Path(weights).suffix == ".pt":
             self.model, self.ckpt = attempt_load_one_weight(weights)
             self.task = self.model.args["task"]
             self.overrides = self.model.args = self._reset_ckpt_args(self.model.args)
             self.ckpt_path = self.model.pt_path
         else:
-            weights = checks.check_file(weights)
+            weights = checks.check_file(weights)  # runs in all cases, not redundant with above call
             self.model, self.ckpt = weights, None
             self.task = task or guess_model_task(weights)
             self.ckpt_path = weights
         self.overrides["model"] = weights
         self.overrides["task"] = self.task
+        self.model_name = weights
 
-    def _check_is_pytorch_model(self):
+    def _check_is_pytorch_model(self) -> None:
         """Raises TypeError is model is not a PyTorch model."""
         pt_str = isinstance(self.model, (str, Path)) and Path(self.model).suffix == ".pt"
         pt_module = isinstance(self.model, nn.Module)
         if not (pt_module or pt_str):
             raise TypeError(
                 f"model='{self.model}' should be a *.pt PyTorch model to run this method, but is a different format. "
                 f"PyTorch models can train, val, predict and export, i.e. 'model.train(data=...)', but exported "
                 f"formats like ONNX, TensorRT etc. only support 'predict' and 'val' modes, "
                 f"i.e. 'yolo predict model=yolov8n.onnx'.\nTo run CUDA or MPS inference please pass the device "
                 f"argument directly in your inference command, i.e. 'model.predict(source=..., device=0)'"
             )
 
-    def reset_weights(self):
+    def reset_weights(self) -> "Model":
         """
         Resets the model parameters to randomly initialized values, effectively discarding all training information.
 
         This method iterates through all modules in the model and resets their parameters if they have a
         'reset_parameters' method. It also ensures that all parameters have 'requires_grad' set to True, enabling them
         to be updated during training.
 
@@ -255,15 +281,15 @@
         for m in self.model.modules():
             if hasattr(m, "reset_parameters"):
                 m.reset_parameters()
         for p in self.model.parameters():
             p.requires_grad = True
         return self
 
-    def load(self, weights="yolov8n.pt"):
+    def load(self, weights: Union[str, Path] = "yolov8n.pt") -> "Model":
         """
         Loads parameters from the specified weights file into the model.
 
         This method supports loading weights from a file or directly from a weights object. It matches parameters by
         name and shape and transfers them to the model.
 
         Args:
@@ -277,32 +303,41 @@
         """
         self._check_is_pytorch_model()
         if isinstance(weights, (str, Path)):
             weights, self.ckpt = attempt_load_one_weight(weights)
         self.model.load(weights)
         return self
 
-    def save(self, filename="model.pt"):
+    def save(self, filename: Union[str, Path] = "saved_model.pt", use_dill=True) -> None:
         """
         Saves the current model state to a file.
 
         This method exports the model's checkpoint (ckpt) to the specified filename.
 
         Args:
-            filename (str): The name of the file to save the model to. Defaults to 'model.pt'.
+            filename (str | Path): The name of the file to save the model to. Defaults to 'saved_model.pt'.
+            use_dill (bool): Whether to try using dill for serialization if available. Defaults to True.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
         self._check_is_pytorch_model()
-        import torch
+        from datetime import datetime
+
+        from ultralytics import __version__
 
-        torch.save(self.ckpt, filename)
+        updates = {
+            "date": datetime.now().isoformat(),
+            "version": __version__,
+            "license": "AGPL-3.0 License (https://ultralytics.com/license)",
+            "docs": "https://docs.ultralytics.com",
+        }
+        torch.save({**self.ckpt, **updates}, filename, use_dill=use_dill)
 
-    def info(self, detailed=False, verbose=True):
+    def info(self, detailed: bool = False, verbose: bool = True):
         """
         Logs or returns model information.
 
         This method provides an overview or detailed information about the model, depending on the arguments passed.
         It can control the verbosity of the output.
 
         Args:
@@ -326,38 +361,49 @@
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
         self._check_is_pytorch_model()
         self.model.fuse()
 
-    def embed(self, source=None, stream=False, **kwargs):
+    def embed(
+        self,
+        source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
+        stream: bool = False,
+        **kwargs,
+    ) -> list:
         """
         Generates image embeddings based on the provided source.
 
         This method is a wrapper around the 'predict()' method, focusing on generating embeddings from an image source.
         It allows customization of the embedding process through various keyword arguments.
 
         Args:
             source (str | int | PIL.Image | np.ndarray): The source of the image for generating embeddings.
                 The source can be a file path, URL, PIL image, numpy array, etc. Defaults to None.
             stream (bool): If True, predictions are streamed. Defaults to False.
-            **kwargs (dict): Additional keyword arguments for configuring the embedding process.
+            **kwargs (any): Additional keyword arguments for configuring the embedding process.
 
         Returns:
             (List[torch.Tensor]): A list containing the image embeddings.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
         if not kwargs.get("embed"):
             kwargs["embed"] = [len(self.model.model) - 2]  # embed second-to-last layer if no indices passed
         return self.predict(source, stream, **kwargs)
 
-    def predict(self, source=None, stream=False, predictor=None, **kwargs):
+    def predict(
+        self,
+        source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
+        stream: bool = False,
+        predictor=None,
+        **kwargs,
+    ) -> list:
         """
         Performs predictions on the given image source using the YOLO model.
 
         This method facilitates the prediction process, allowing various configurations through keyword arguments.
         It supports predictions with custom predictors or the default predictor method. The method handles different
         types of image sources and can operate in a streaming mode. It also provides support for SAM-type models
         through 'prompts'.
@@ -369,47 +415,53 @@
 
         Args:
             source (str | int | PIL.Image | np.ndarray, optional): The source of the image for making predictions.
                 Accepts various types, including file paths, URLs, PIL images, and numpy arrays. Defaults to ASSETS.
             stream (bool, optional): Treats the input source as a continuous stream for predictions. Defaults to False.
             predictor (BasePredictor, optional): An instance of a custom predictor class for making predictions.
                 If None, the method uses a default predictor. Defaults to None.
-            **kwargs (dict): Additional keyword arguments for configuring the prediction process. These arguments allow
+            **kwargs (any): Additional keyword arguments for configuring the prediction process. These arguments allow
                 for further customization of the prediction behavior.
 
         Returns:
             (List[ultralytics.engine.results.Results]): A list of prediction results, encapsulated in the Results class.
 
         Raises:
             AttributeError: If the predictor is not properly set up.
         """
         if source is None:
             source = ASSETS
             LOGGER.warning(f"WARNING ⚠️ 'source' is missing. Using 'source={source}'.")
 
-        is_cli = (sys.argv[0].endswith("yolo") or sys.argv[0].endswith("ultralytics")) and any(
-            x in sys.argv for x in ("predict", "track", "mode=predict", "mode=track")
+        is_cli = (ARGV[0].endswith("yolo") or ARGV[0].endswith("ultralytics")) and any(
+            x in ARGV for x in ("predict", "track", "mode=predict", "mode=track")
         )
 
-        custom = {"conf": 0.25, "save": is_cli, "mode": "predict"}  # method defaults
+        custom = {"conf": 0.25, "batch": 1, "save": is_cli, "mode": "predict"}  # method defaults
         args = {**self.overrides, **custom, **kwargs}  # highest priority args on the right
         prompts = args.pop("prompts", None)  # for SAM-type models
 
         if not self.predictor:
             self.predictor = predictor or self._smart_load("predictor")(overrides=args, _callbacks=self.callbacks)
             self.predictor.setup_model(model=self.model, verbose=is_cli)
         else:  # only update args if predictor is already setup
             self.predictor.args = get_cfg(self.predictor.args, args)
             if "project" in args or "name" in args:
                 self.predictor.save_dir = get_save_dir(self.predictor.args)
         if prompts and hasattr(self.predictor, "set_prompts"):  # for SAM-type models
             self.predictor.set_prompts(prompts)
         return self.predictor.predict_cli(source=source) if is_cli else self.predictor(source=source, stream=stream)
 
-    def track(self, source=None, stream=False, persist=False, **kwargs):
+    def track(
+        self,
+        source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
+        stream: bool = False,
+        persist: bool = False,
+        **kwargs,
+    ) -> list:
         """
         Conducts object tracking on the specified input source using the registered trackers.
 
         This method performs object tracking using the model's predictors and optionally registered trackers. It is
         capable of handling different types of input sources such as file paths or video streams. The method supports
         customization of the tracking process through various keyword arguments. It registers trackers if they are not
         already present and optionally persists them based on the 'persist' flag.
@@ -417,32 +469,37 @@
         The method sets a default confidence threshold specifically for ByteTrack-based tracking, which requires low
         confidence predictions as input. The tracking mode is explicitly set in the keyword arguments.
 
         Args:
             source (str, optional): The input source for object tracking. It can be a file path, URL, or video stream.
             stream (bool, optional): Treats the input source as a continuous video stream. Defaults to False.
             persist (bool, optional): Persists the trackers between different calls to this method. Defaults to False.
-            **kwargs (dict): Additional keyword arguments for configuring the tracking process. These arguments allow
+            **kwargs (any): Additional keyword arguments for configuring the tracking process. These arguments allow
                 for further customization of the tracking behavior.
 
         Returns:
             (List[ultralytics.engine.results.Results]): A list of tracking results, encapsulated in the Results class.
 
         Raises:
             AttributeError: If the predictor does not have registered trackers.
         """
         if not hasattr(self.predictor, "trackers"):
             from ultralytics.trackers import register_tracker
 
             register_tracker(self, persist)
         kwargs["conf"] = kwargs.get("conf") or 0.1  # ByteTrack-based method needs low confidence predictions as input
+        kwargs["batch"] = kwargs.get("batch") or 1  # batch-size 1 for tracking in videos
         kwargs["mode"] = "track"
         return self.predict(source=source, stream=stream, **kwargs)
 
-    def val(self, validator=None, **kwargs):
+    def val(
+        self,
+        validator=None,
+        **kwargs,
+    ):
         """
         Validates the model using a specified dataset and validation configuration.
 
         This method facilitates the model validation process, allowing for a range of customization through various
         settings and configurations. It supports validation with a custom validator or the default validation approach.
         The method combines default configurations, method-specific defaults, and user-provided arguments to configure
         the validation process. After validation, it updates the model's metrics with the results obtained from the
@@ -450,15 +507,15 @@
 
         The method supports various arguments that allow customization of the validation process. For a comprehensive
         list of all configurable options, users should refer to the 'configuration' section in the documentation.
 
         Args:
             validator (BaseValidator, optional): An instance of a custom validator class for validating the model. If
                 None, the method uses a default validator. Defaults to None.
-            **kwargs (dict): Arbitrary keyword arguments representing the validation configuration. These arguments are
+            **kwargs (any): Arbitrary keyword arguments representing the validation configuration. These arguments are
                 used to customize various aspects of the validation process.
 
         Returns:
             (dict): Validation metrics obtained from the validation process.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
@@ -467,29 +524,32 @@
         args = {**self.overrides, **custom, **kwargs, "mode": "val"}  # highest priority args on the right
 
         validator = (validator or self._smart_load("validator"))(args=args, _callbacks=self.callbacks)
         validator(model=self.model)
         self.metrics = validator.metrics
         return validator.metrics
 
-    def benchmark(self, **kwargs):
+    def benchmark(
+        self,
+        **kwargs,
+    ):
         """
         Benchmarks the model across various export formats to evaluate performance.
 
         This method assesses the model's performance in different export formats, such as ONNX, TorchScript, etc.
         It uses the 'benchmark' function from the ultralytics.utils.benchmarks module. The benchmarking is configured
         using a combination of default configuration values, model-specific arguments, method-specific defaults, and
         any additional user-provided keyword arguments.
 
         The method supports various arguments that allow customization of the benchmarking process, such as dataset
         choice, image size, precision modes, device selection, and verbosity. For a comprehensive list of all
         configurable options, users should refer to the 'configuration' section in the documentation.
 
         Args:
-            **kwargs (dict): Arbitrary keyword arguments to customize the benchmarking process. These are combined with
+            **kwargs (any): Arbitrary keyword arguments to customize the benchmarking process. These are combined with
                 default configurations, model-specific arguments, and method defaults.
 
         Returns:
             (dict): A dictionary containing the results of the benchmarking process.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
@@ -505,27 +565,30 @@
             imgsz=args["imgsz"],
             half=args["half"],
             int8=args["int8"],
             device=args["device"],
             verbose=kwargs.get("verbose"),
         )
 
-    def export(self, **kwargs):
+    def export(
+        self,
+        **kwargs,
+    ):
         """
         Exports the model to a different format suitable for deployment.
 
         This method facilitates the export of the model to various formats (e.g., ONNX, TorchScript) for deployment
         purposes. It uses the 'Exporter' class for the export process, combining model-specific overrides, method
         defaults, and any additional arguments provided. The combined arguments are used to configure export settings.
 
         The method supports a wide range of arguments to customize the export process. For a comprehensive list of all
         possible arguments, refer to the 'configuration' section in the documentation.
 
         Args:
-            **kwargs (dict): Arbitrary keyword arguments to customize the export process. These are combined with the
+            **kwargs (any): Arbitrary keyword arguments to customize the export process. These are combined with the
                 model's overrides and method defaults.
 
         Returns:
             (object): The exported model in the specified format, or an object related to the export process.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
@@ -533,15 +596,19 @@
         self._check_is_pytorch_model()
         from .exporter import Exporter
 
         custom = {"imgsz": self.model.args["imgsz"], "batch": 1, "data": None, "verbose": False}  # method defaults
         args = {**self.overrides, **custom, **kwargs, "mode": "export"}  # highest priority args on the right
         return Exporter(overrides=args, _callbacks=self.callbacks)(model=self.model)
 
-    def train(self, trainer=None, **kwargs):
+    def train(
+        self,
+        trainer=None,
+        **kwargs,
+    ):
         """
         Trains the model using the specified dataset and training configuration.
 
         This method facilitates model training with a range of customizable settings and configurations. It supports
         training with a custom trainer or the default training approach defined in the method. The method handles
         different scenarios, such as resuming training from a checkpoint, integrating with Ultralytics HUB, and
         updating model and configuration after training.
@@ -550,15 +617,15 @@
         arguments and issues a warning if local arguments are provided. It checks for pip updates and combines default
         configurations, method-specific defaults, and user-provided arguments to configure the training process. After
         training, it updates the model and its configurations, and optionally attaches metrics.
 
         Args:
             trainer (BaseTrainer, optional): An instance of a custom trainer class for training the model. If None, the
                 method uses a default trainer. Defaults to None.
-            **kwargs (dict): Arbitrary keyword arguments representing the training configuration. These arguments are
+            **kwargs (any): Arbitrary keyword arguments representing the training configuration. These arguments are
                 used to customize various aspects of the training process.
 
         Returns:
             (dict | None): Training metrics if available and training is successful; otherwise, None.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
@@ -570,15 +637,20 @@
             if any(kwargs):
                 LOGGER.warning("WARNING ⚠️ using HUB training arguments, ignoring local training arguments.")
             kwargs = self.session.train_args  # overwrite kwargs
 
         checks.check_pip_update_available()
 
         overrides = yaml_load(checks.check_yaml(kwargs["cfg"])) if kwargs.get("cfg") else self.overrides
-        custom = {"data": DEFAULT_CFG_DICT["data"] or TASK2DATA[self.task]}  # method defaults
+        custom = {
+            # NOTE: handle the case when 'cfg' includes 'data'.
+            "data": overrides.get("data") or DEFAULT_CFG_DICT["data"] or TASK2DATA[self.task],
+            "model": self.overrides["model"],
+            "task": self.task,
+        }  # method defaults
         args = {**overrides, **custom, **kwargs, "mode": "train"}  # highest priority args on the right
         if args.get("resume"):
             args["resume"] = self.ckpt_path
 
         self.trainer = (trainer or self._smart_load("trainer"))(overrides=args, _callbacks=self.callbacks)
         if not args.get("resume"):  # manually set model only if not resuming
             self.trainer.model = self.trainer.get_model(weights=self.model if self.ckpt else None, cfg=self.model.yaml)
@@ -596,35 +668,41 @@
                 except (PermissionError, ModuleNotFoundError):
                     # Ignore PermissionError and ModuleNotFoundError which indicates hub-sdk not installed
                     pass
 
         self.trainer.hub_session = self.session  # attach optional HUB session
         self.trainer.train()
         # Update model and cfg after training
-        if RANK in (-1, 0):
+        if RANK in {-1, 0}:
             ckpt = self.trainer.best if self.trainer.best.exists() else self.trainer.last
             self.model, _ = attempt_load_one_weight(ckpt)
             self.overrides = self.model.args
             self.metrics = getattr(self.trainer.validator, "metrics", None)  # TODO: no metrics returned by DDP
         return self.metrics
 
-    def tune(self, use_ray=False, iterations=10, *args, **kwargs):
+    def tune(
+        self,
+        use_ray=False,
+        iterations=10,
+        *args,
+        **kwargs,
+    ):
         """
         Conducts hyperparameter tuning for the model, with an option to use Ray Tune.
 
         This method supports two modes of hyperparameter tuning: using Ray Tune or a custom tuning method.
         When Ray Tune is enabled, it leverages the 'run_ray_tune' function from the ultralytics.utils.tuner module.
         Otherwise, it uses the internal 'Tuner' class for tuning. The method combines default, overridden, and
         custom arguments to configure the tuning process.
 
         Args:
             use_ray (bool): If True, uses Ray Tune for hyperparameter tuning. Defaults to False.
             iterations (int): The number of tuning iterations to perform. Defaults to 10.
             *args (list): Variable length argument list for additional arguments.
-            **kwargs (dict): Arbitrary keyword arguments. These are combined with the model's overrides and defaults.
+            **kwargs (any): Arbitrary keyword arguments. These are combined with the model's overrides and defaults.
 
         Returns:
             (dict): A dictionary containing the results of the hyperparameter search.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
@@ -636,39 +714,45 @@
         else:
             from .tuner import Tuner
 
             custom = {}  # method defaults
             args = {**self.overrides, **custom, **kwargs, "mode": "train"}  # highest priority args on the right
             return Tuner(args=args, _callbacks=self.callbacks)(model=self, iterations=iterations)
 
-    def _apply(self, fn):
+    def _apply(self, fn) -> "Model":
         """Apply to(), cpu(), cuda(), half(), float() to model tensors that are not parameters or registered buffers."""
         self._check_is_pytorch_model()
         self = super()._apply(fn)  # noqa
         self.predictor = None  # reset predictor as device may have changed
         self.overrides["device"] = self.device  # was str(self.device) i.e. device(type='cuda', index=0) -> 'cuda:0'
         return self
 
     @property
-    def names(self):
+    def names(self) -> list:
         """
         Retrieves the class names associated with the loaded model.
 
         This property returns the class names if they are defined in the model. It checks the class names for validity
         using the 'check_class_names' function from the ultralytics.nn.autobackend module.
 
         Returns:
             (list | None): The class names of the model if available, otherwise None.
         """
         from ultralytics.nn.autobackend import check_class_names
 
-        return check_class_names(self.model.names) if hasattr(self.model, "names") else None
+        if hasattr(self.model, "names"):
+            return check_class_names(self.model.names)
+        else:
+            if not self.predictor:  # export formats will not have predictor defined until predict() is called
+                self.predictor = self._smart_load("predictor")(overrides=self.overrides, _callbacks=self.callbacks)
+                self.predictor.setup_model(model=self.model, verbose=False)
+            return self.predictor.model.names
 
     @property
-    def device(self):
+    def device(self) -> torch.device:
         """
         Retrieves the device on which the model's parameters are allocated.
 
         This property is used to determine whether the model's parameters are on CPU or GPU. It only applies to models
         that are instances of nn.Module.
 
         Returns:
@@ -684,15 +768,15 @@
         This property returns the transformations if they are defined in the model.
 
         Returns:
             (object | None): The transform object of the model if available, otherwise None.
         """
         return self.model.transforms if hasattr(self.model, "transforms") else None
 
-    def add_callback(self, event: str, func):
+    def add_callback(self, event: str, func) -> None:
         """
         Adds a callback function for a specified event.
 
         This method allows the user to register a custom callback function that is triggered on a specific event during
         model training or inference.
 
         Args:
@@ -700,62 +784,62 @@
             func (callable): The callback function to be registered.
 
         Raises:
             ValueError: If the event name is not recognized.
         """
         self.callbacks[event].append(func)
 
-    def clear_callback(self, event: str):
+    def clear_callback(self, event: str) -> None:
         """
         Clears all callback functions registered for a specified event.
 
         This method removes all custom and default callback functions associated with the given event.
 
         Args:
             event (str): The name of the event for which to clear the callbacks.
 
         Raises:
             ValueError: If the event name is not recognized.
         """
         self.callbacks[event] = []
 
-    def reset_callbacks(self):
+    def reset_callbacks(self) -> None:
         """
         Resets all callbacks to their default functions.
 
         This method reinstates the default callback functions for all events, removing any custom callbacks that were
         added previously.
         """
         for event in callbacks.default_callbacks.keys():
             self.callbacks[event] = [callbacks.default_callbacks[event][0]]
 
     @staticmethod
-    def _reset_ckpt_args(args):
+    def _reset_ckpt_args(args: dict) -> dict:
         """Reset arguments when loading a PyTorch model."""
         include = {"imgsz", "data", "task", "single_cls"}  # only remember these arguments when loading a PyTorch model
         return {k: v for k, v in args.items() if k in include}
 
     # def __getattr__(self, attr):
     #    """Raises error if object has no requested attribute."""
     #    name = self.__class__.__name__
     #    raise AttributeError(f"'{name}' object has no attribute '{attr}'. See valid attributes below.\n{self.__doc__}")
 
-    def _smart_load(self, key):
+    def _smart_load(self, key: str):
         """Load model/trainer/validator/predictor."""
         try:
             return self.task_map[self.task][key]
         except Exception as e:
             name = self.__class__.__name__
             mode = inspect.stack()[1][3]  # get the function name.
             raise NotImplementedError(
                 emojis(f"WARNING ⚠️ '{name}' model does not support '{mode}' mode for '{self.task}' task yet.")
             ) from e
 
     @property
-    def task_map(self):
+    def task_map(self) -> dict:
         """
         Map head to model, trainer, validator, and predictor classes.
 
         Returns:
             task_map (dict): The map of model task to mode classes.
         """
         raise NotImplementedError("Please provide task map for your model!")
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/predictor.py` & `ultralytics-8.2.0/ultralytics/engine/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,19 @@
                               yolov8n.engine             # TensorRT
                               yolov8n.mlpackage          # CoreML (macOS-only)
                               yolov8n_saved_model        # TensorFlow SavedModel
                               yolov8n.pb                 # TensorFlow GraphDef
                               yolov8n.tflite             # TensorFlow Lite
                               yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                               yolov8n_paddle_model       # PaddlePaddle
+                              yolov8n_ncnn_model         # NCNN
 """
+
 import platform
+import re
 import threading
 from pathlib import Path
 
 import cv2
 import numpy as np
 import torch
 
@@ -67,17 +70,15 @@
         args (SimpleNamespace): Configuration for the predictor.
         save_dir (Path): Directory to save results.
         done_warmup (bool): Whether the predictor has finished setup.
         model (nn.Module): Model used for prediction.
         data (dict): Data configuration.
         device (torch.device): Device used for prediction.
         dataset (Dataset): Dataset used for prediction.
-        vid_path (str): Path to video file.
-        vid_writer (cv2.VideoWriter): Video writer for saving video output.
-        data_path (str): Path to data.
+        vid_writer (dict): Dictionary of {save_path: video_writer, ...} writer for saving video output.
     """
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """
         Initializes the BasePredictor class.
 
         Args:
@@ -94,18 +95,19 @@
 
         # Usable if setup is done
         self.model = None
         self.data = self.args.data  # data_dict
         self.imgsz = None
         self.device = None
         self.dataset = None
-        self.vid_path, self.vid_writer, self.vid_frame = None, None, None
+        self.vid_writer = {}  # dict of {save_path: video_writer, ...}
         self.plotted_img = None
-        self.data_path = None
         self.source_type = None
+        self.seen = 0
+        self.windows = []
         self.batch = None
         self.results = None
         self.transforms = None
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         self.txt_path = None
         self._lock = threading.Lock()  # for automatic thread-safe inference
         callbacks.add_integration_callbacks(self)
@@ -145,56 +147,18 @@
 
         Args:
             im (List(np.ndarray)): (N, 3, h, w) for tensor, [(h, w, 3) x N] for list.
 
         Returns:
             (list): A list of transformed images.
         """
-        same_shapes = all(x.shape == im[0].shape for x in im)
+        same_shapes = len({x.shape for x in im}) == 1
         letterbox = LetterBox(self.imgsz, auto=same_shapes and self.model.pt, stride=self.model.stride)
         return [letterbox(image=x) for x in im]
 
-    def write_results(self, idx, results, batch):
-        """Write inference results to a file or directory."""
-        p, im, _ = batch
-        log_string = ""
-        if len(im.shape) == 3:
-            im = im[None]  # expand for batch dim
-        if self.source_type.webcam or self.source_type.from_img or self.source_type.tensor:  # batch_size >= 1
-            log_string += f"{idx}: "
-            frame = self.dataset.count
-        else:
-            frame = getattr(self.dataset, "frame", 0)
-        self.data_path = p
-        self.txt_path = str(self.save_dir / "labels" / p.stem) + ("" if self.dataset.mode == "image" else f"_{frame}")
-        log_string += "%gx%g " % im.shape[2:]  # print string
-        result = results[idx]
-        log_string += result.verbose()
-
-        if self.args.save or self.args.show:  # Add bbox to image
-            plot_args = {
-                "line_width": self.args.line_width,
-                "boxes": self.args.show_boxes,
-                "conf": self.args.show_conf,
-                "labels": self.args.show_labels,
-            }
-            if not self.args.retina_masks:
-                plot_args["im_gpu"] = im[idx]
-            self.plotted_img = result.plot(**plot_args)
-        # Write
-        if self.args.save_txt:
-            result.save_txt(f"{self.txt_path}.txt", save_conf=self.args.save_conf)
-        if self.args.save_crop:
-            result.save_crop(
-                save_dir=self.save_dir / "crops",
-                file_name=self.data_path.stem + ("" if self.dataset.mode == "image" else f"_{frame}"),
-            )
-
-        return log_string
-
     def postprocess(self, preds, img, orig_imgs):
         """Post-processes predictions for an image and returns them."""
         return preds
 
     def __call__(self, source=None, model=None, stream=False, *args, **kwargs):
         """Performs inference on an image or stream."""
         self.stream = stream
@@ -222,26 +186,28 @@
                 "transforms",
                 classify_transforms(self.imgsz[0], crop_fraction=self.args.crop_fraction),
             )
             if self.args.task == "classify"
             else None
         )
         self.dataset = load_inference_source(
-            source=source, vid_stride=self.args.vid_stride, buffer=self.args.stream_buffer
+            source=source,
+            batch=self.args.batch,
+            vid_stride=self.args.vid_stride,
+            buffer=self.args.stream_buffer,
         )
         self.source_type = self.dataset.source_type
         if not getattr(self, "stream", True) and (
-            self.dataset.mode == "stream"  # streams
-            or len(self.dataset) > 1000  # images
+            self.source_type.stream
+            or self.source_type.screenshot
+            or len(self.dataset) > 1000  # many images
             or any(getattr(self.dataset, "video_flag", [False]))
         ):  # videos
             LOGGER.warning(STREAM_WARNING)
-        self.vid_path = [None] * self.dataset.bs
-        self.vid_writer = [None] * self.dataset.bs
-        self.vid_frame = [None] * self.dataset.bs
+        self.vid_writer = {}
 
     @smart_inference_mode()
     def stream_inference(self, source=None, model=None, *args, **kwargs):
         """Streams real-time inference on camera feed and saves results to file."""
         if self.args.verbose:
             LOGGER.info("")
 
@@ -265,18 +231,17 @@
             self.seen, self.windows, self.batch = 0, [], None
             profilers = (
                 ops.Profile(device=self.device),
                 ops.Profile(device=self.device),
                 ops.Profile(device=self.device),
             )
             self.run_callbacks("on_predict_start")
-            for batch in self.dataset:
+            for self.batch in self.dataset:
                 self.run_callbacks("on_predict_batch_start")
-                self.batch = batch
-                path, im0s, vid_cap, s = batch
+                paths, im0s, s = self.batch
 
                 # Preprocess
                 with profilers[0]:
                     im = self.preprocess(im0s)
 
                 # Inference
                 with profilers[1]:
@@ -284,120 +249,147 @@
                     if self.args.embed:
                         yield from [preds] if isinstance(preds, torch.Tensor) else preds  # yield embedding tensors
                         continue
 
                 # Postprocess
                 with profilers[2]:
                     self.results = self.postprocess(preds, im, im0s)
-
                 self.run_callbacks("on_predict_postprocess_end")
+
                 # Visualize, save, write results
                 n = len(im0s)
                 for i in range(n):
                     self.seen += 1
                     self.results[i].speed = {
                         "preprocess": profilers[0].dt * 1e3 / n,
                         "inference": profilers[1].dt * 1e3 / n,
                         "postprocess": profilers[2].dt * 1e3 / n,
                     }
-                    p, im0 = path[i], None if self.source_type.tensor else im0s[i].copy()
-                    p = Path(p)
-
                     if self.args.verbose or self.args.save or self.args.save_txt or self.args.show:
-                        s += self.write_results(i, self.results, (p, im, im0))
-                    if self.args.save or self.args.save_txt:
-                        self.results[i].save_dir = self.save_dir.__str__()
-                    if self.args.show and self.plotted_img is not None:
-                        self.show(p)
-                    if self.args.save and self.plotted_img is not None:
-                        self.save_preds(vid_cap, i, str(self.save_dir / p.name))
+                        s[i] += self.write_results(i, Path(paths[i]), im, s)
+
+                # Print batch results
+                if self.args.verbose:
+                    LOGGER.info("\n".join(s))
 
                 self.run_callbacks("on_predict_batch_end")
                 yield from self.results
 
-                # Print time (inference-only)
-                if self.args.verbose:
-                    LOGGER.info(f"{s}{profilers[1].dt * 1E3:.1f}ms")
-
         # Release assets
-        if isinstance(self.vid_writer[-1], cv2.VideoWriter):
-            self.vid_writer[-1].release()  # release final video writer
+        for v in self.vid_writer.values():
+            if isinstance(v, cv2.VideoWriter):
+                v.release()
 
-        # Print results
+        # Print final results
         if self.args.verbose and self.seen:
             t = tuple(x.t / self.seen * 1e3 for x in profilers)  # speeds per image
             LOGGER.info(
                 f"Speed: %.1fms preprocess, %.1fms inference, %.1fms postprocess per image at shape "
-                f"{(1, 3, *im.shape[2:])}" % t
+                f"{(min(self.args.batch, self.seen), 3, *im.shape[2:])}" % t
             )
         if self.args.save or self.args.save_txt or self.args.save_crop:
             nl = len(list(self.save_dir.glob("labels/*.txt")))  # number of labels
             s = f"\n{nl} label{'s' * (nl > 1)} saved to {self.save_dir / 'labels'}" if self.args.save_txt else ""
             LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}{s}")
-
         self.run_callbacks("on_predict_end")
 
     def setup_model(self, model, verbose=True):
         """Initialize YOLO model with given parameters and set it to evaluation mode."""
         self.model = AutoBackend(
-            model or self.args.model,
+            weights=model or self.args.model,
             device=select_device(self.args.device, verbose=verbose),
             dnn=self.args.dnn,
             data=self.args.data,
             fp16=self.args.half,
+            batch=self.args.batch,
             fuse=True,
             verbose=verbose,
         )
 
         self.device = self.model.device  # update device
         self.args.half = self.model.fp16  # update half
         self.model.eval()
 
-    def show(self, p):
-        """Display an image in a window using OpenCV imshow()."""
-        im0 = self.plotted_img
-        if platform.system() == "Linux" and p not in self.windows:
-            self.windows.append(p)
-            cv2.namedWindow(str(p), cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)  # allow window resize (Linux)
-            cv2.resizeWindow(str(p), im0.shape[1], im0.shape[0])
-        cv2.imshow(str(p), im0)
-        cv2.waitKey(500 if self.batch[3].startswith("image") else 1)  # 1 millisecond
+    def write_results(self, i, p, im, s):
+        """Write inference results to a file or directory."""
+        string = ""  # print string
+        if len(im.shape) == 3:
+            im = im[None]  # expand for batch dim
+        if self.source_type.stream or self.source_type.from_img or self.source_type.tensor:  # batch_size >= 1
+            string += f"{i}: "
+            frame = self.dataset.count
+        else:
+            match = re.search(r"frame (\d+)/", s[i])
+            frame = int(match.group(1)) if match else None  # 0 if frame undetermined
 
-    def save_preds(self, vid_cap, idx, save_path):
+        self.txt_path = self.save_dir / "labels" / (p.stem + ("" if self.dataset.mode == "image" else f"_{frame}"))
+        string += "%gx%g " % im.shape[2:]
+        result = self.results[i]
+        result.save_dir = self.save_dir.__str__()  # used in other locations
+        string += result.verbose() + f"{result.speed['inference']:.1f}ms"
+
+        # Add predictions to image
+        if self.args.save or self.args.show:
+            self.plotted_img = result.plot(
+                line_width=self.args.line_width,
+                boxes=self.args.show_boxes,
+                conf=self.args.show_conf,
+                labels=self.args.show_labels,
+                im_gpu=None if self.args.retina_masks else im[i],
+            )
+
+        # Save results
+        if self.args.save_txt:
+            result.save_txt(f"{self.txt_path}.txt", save_conf=self.args.save_conf)
+        if self.args.save_crop:
+            result.save_crop(save_dir=self.save_dir / "crops", file_name=self.txt_path.stem)
+        if self.args.show:
+            self.show(str(p))
+        if self.args.save:
+            self.save_predicted_images(str(self.save_dir / p.name), frame)
+
+        return string
+
+    def save_predicted_images(self, save_path="", frame=0):
         """Save video predictions as mp4 at specified path."""
-        im0 = self.plotted_img
-        # Save imgs
-        if self.dataset.mode == "image":
-            cv2.imwrite(save_path, im0)
-        else:  # 'video' or 'stream'
+        im = self.plotted_img
+
+        # Save videos and streams
+        if self.dataset.mode in {"stream", "video"}:
+            fps = self.dataset.fps if self.dataset.mode == "video" else 30
             frames_path = f'{save_path.split(".", 1)[0]}_frames/'
-            if self.vid_path[idx] != save_path:  # new video
-                self.vid_path[idx] = save_path
+            if save_path not in self.vid_writer:  # new video
                 if self.args.save_frames:
                     Path(frames_path).mkdir(parents=True, exist_ok=True)
-                    self.vid_frame[idx] = 0
-                if isinstance(self.vid_writer[idx], cv2.VideoWriter):
-                    self.vid_writer[idx].release()  # release previous video writer
-                if vid_cap:  # video
-                    fps = int(vid_cap.get(cv2.CAP_PROP_FPS))  # integer required, floats produce error in MP4 codec
-                    w = int(vid_cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-                    h = int(vid_cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-                else:  # stream
-                    fps, w, h = 30, im0.shape[1], im0.shape[0]
                 suffix, fourcc = (".mp4", "avc1") if MACOS else (".avi", "WMV2") if WINDOWS else (".avi", "MJPG")
-                self.vid_writer[idx] = cv2.VideoWriter(
-                    str(Path(save_path).with_suffix(suffix)), cv2.VideoWriter_fourcc(*fourcc), fps, (w, h)
+                self.vid_writer[save_path] = cv2.VideoWriter(
+                    filename=str(Path(save_path).with_suffix(suffix)),
+                    fourcc=cv2.VideoWriter_fourcc(*fourcc),
+                    fps=fps,  # integer required, floats produce error in MP4 codec
+                    frameSize=(im.shape[1], im.shape[0]),  # (width, height)
                 )
-            # Write video
-            self.vid_writer[idx].write(im0)
 
-            # Write frame
+            # Save video
+            self.vid_writer[save_path].write(im)
             if self.args.save_frames:
-                cv2.imwrite(f"{frames_path}{self.vid_frame[idx]}.jpg", im0)
-                self.vid_frame[idx] += 1
+                cv2.imwrite(f"{frames_path}{frame}.jpg", im)
+
+        # Save images
+        else:
+            cv2.imwrite(save_path, im)
+
+    def show(self, p=""):
+        """Display an image in a window using OpenCV imshow()."""
+        im = self.plotted_img
+        if platform.system() == "Linux" and p not in self.windows:
+            self.windows.append(p)
+            cv2.namedWindow(p, cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)  # allow window resize (Linux)
+            cv2.resizeWindow(p, im.shape[1], im.shape[0])  # (width, height)
+        cv2.imshow(p, im)
+        cv2.waitKey(300 if self.dataset.mode == "image" else 1)  # 1 millisecond
 
     def run_callbacks(self, event: str):
         """Runs all registered callbacks for a specific event."""
         for callback in self.callbacks.get(event, []):
             callback(self)
 
     def add_callback(self, event: str, func):
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/results.py` & `ultralytics-8.2.0/ultralytics/engine/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,38 +63,55 @@
         return self.__class__(self.data[idx], self.orig_shape)
 
 
 class Results(SimpleClass):
     """
     A class for storing and manipulating inference results.
 
-    Args:
-        orig_img (numpy.ndarray): The original image as a numpy array.
-        path (str): The path to the image file.
-        names (dict): A dictionary of class names.
-        boxes (torch.tensor, optional): A 2D tensor of bounding box coordinates for each detection.
-        masks (torch.tensor, optional): A 3D tensor of detection masks, where each mask is a binary image.
-        probs (torch.tensor, optional): A 1D tensor of probabilities of each class for classification task.
-        keypoints (List[List[float]], optional): A list of detected keypoints for each object.
-
     Attributes:
-        orig_img (numpy.ndarray): The original image as a numpy array.
-        orig_shape (tuple): The original image shape in (height, width) format.
-        boxes (Boxes, optional): A Boxes object containing the detection bounding boxes.
-        masks (Masks, optional): A Masks object containing the detection masks.
-        probs (Probs, optional): A Probs object containing probabilities of each class for classification task.
-        keypoints (Keypoints, optional): A Keypoints object containing detected keypoints for each object.
-        speed (dict): A dictionary of preprocess, inference, and postprocess speeds in milliseconds per image.
-        names (dict): A dictionary of class names.
-        path (str): The path to the image file.
-        _keys (tuple): A tuple of attribute names for non-empty attributes.
+        orig_img (numpy.ndarray): Original image as a numpy array.
+        orig_shape (tuple): Original image shape in (height, width) format.
+        boxes (Boxes, optional): Object containing detection bounding boxes.
+        masks (Masks, optional): Object containing detection masks.
+        probs (Probs, optional): Object containing class probabilities for classification tasks.
+        keypoints (Keypoints, optional): Object containing detected keypoints for each object.
+        speed (dict): Dictionary of preprocess, inference, and postprocess speeds (ms/image).
+        names (dict): Dictionary of class names.
+        path (str): Path to the image file.
+
+    Methods:
+        update(boxes=None, masks=None, probs=None, obb=None): Updates object attributes with new detection results.
+        cpu(): Returns a copy of the Results object with all tensors on CPU memory.
+        numpy(): Returns a copy of the Results object with all tensors as numpy arrays.
+        cuda(): Returns a copy of the Results object with all tensors on GPU memory.
+        to(*args, **kwargs): Returns a copy of the Results object with tensors on a specified device and dtype.
+        new(): Returns a new Results object with the same image, path, and names.
+        plot(...): Plots detection results on an input image, returning an annotated image.
+        show(): Show annotated results to screen.
+        save(filename): Save annotated results to file.
+        verbose(): Returns a log string for each task, detailing detections and classifications.
+        save_txt(txt_file, save_conf=False): Saves detection results to a text file.
+        save_crop(save_dir, file_name=Path("im.jpg")): Saves cropped detection images.
+        tojson(normalize=False): Converts detection results to JSON format.
     """
 
     def __init__(self, orig_img, path, names, boxes=None, masks=None, probs=None, keypoints=None, obb=None) -> None:
-        """Initialize the Results class."""
+        """
+        Initialize the Results class.
+
+        Args:
+            orig_img (numpy.ndarray): The original image as a numpy array.
+            path (str): The path to the image file.
+            names (dict): A dictionary of class names.
+            boxes (torch.tensor, optional): A 2D tensor of bounding box coordinates for each detection.
+            masks (torch.tensor, optional): A 3D tensor of detection masks, where each mask is a binary image.
+            probs (torch.tensor, optional): A 1D tensor of probabilities of each class for classification task.
+            keypoints (torch.tensor, optional): A 2D tensor of keypoint coordinates for each detection.
+            obb (torch.tensor, optional): A 2D tensor of oriented bounding box coordinates for each detection.
+        """
         self.orig_img = orig_img
         self.orig_shape = orig_img.shape[:2]
         self.boxes = Boxes(boxes, self.orig_shape) if boxes is not None else None  # native size boxes
         self.masks = Masks(masks, self.orig_shape) if masks is not None else None  # native size or imgsz masks
         self.probs = Probs(probs) if probs is not None else None
         self.keypoints = Keypoints(keypoints, self.orig_shape) if keypoints is not None else None
         self.obb = OBB(obb, self.orig_shape) if obb is not None else None
@@ -177,14 +194,17 @@
         im_gpu=None,
         kpt_radius=5,
         kpt_line=True,
         labels=True,
         boxes=True,
         masks=True,
         probs=True,
+        show=False,
+        save=False,
+        filename=None,
     ):
         """
         Plots the detection results on an input RGB image. Accepts a numpy array (cv2) or a PIL Image.
 
         Args:
             conf (bool): Whether to plot the detection confidence score.
             line_width (float, optional): The line width of the bounding boxes. If None, it is scaled to the image size.
@@ -195,14 +215,17 @@
             im_gpu (torch.Tensor): Normalized image in gpu with shape (1, 3, 640, 640), for faster mask plotting.
             kpt_radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool): Whether to draw lines connecting keypoints.
             labels (bool): Whether to plot the label of bounding boxes.
             boxes (bool): Whether to plot the bounding boxes.
             masks (bool): Whether to plot the masks.
             probs (bool): Whether to plot classification probability
+            show (bool): Whether to display the annotated image directly.
+            save (bool): Whether to save the annotated image to `filename`.
+            filename (str): Filename to save image to if save is True.
 
         Returns:
             (numpy.ndarray): A numpy array of the annotated image.
 
         Example:
             ```python
             from PIL import Image
@@ -264,16 +287,35 @@
             annotator.text([x, x], text, txt_color=(255, 255, 255))  # TODO: allow setting colors
 
         # Plot Pose results
         if self.keypoints is not None:
             for k in reversed(self.keypoints.data):
                 annotator.kpts(k, self.orig_shape, radius=kpt_radius, kpt_line=kpt_line)
 
+        # Show results
+        if show:
+            annotator.show(self.path)
+
+        # Save results
+        if save:
+            annotator.save(filename)
+
         return annotator.result()
 
+    def show(self, *args, **kwargs):
+        """Show annotated results image."""
+        self.plot(show=True, *args, **kwargs)
+
+    def save(self, filename=None, *args, **kwargs):
+        """Save annotated results image."""
+        if not filename:
+            filename = f"results_{Path(self.path).name}"
+        self.plot(save=True, filename=filename, *args, **kwargs)
+        return filename
+
     def verbose(self):
         """Return log string for each task."""
         log_string = ""
         probs = self.probs
         boxes = self.boxes
         if len(self) == 0:
             return log_string if probs is not None else f"{log_string}(no detections), "
@@ -339,79 +381,100 @@
             save_one_box(
                 d.xyxy,
                 self.orig_img.copy(),
                 file=Path(save_dir) / self.names[int(d.cls)] / f"{Path(file_name)}.jpg",
                 BGR=True,
             )
 
-    def tojson(self, normalize=False):
-        """Convert the object to JSON format."""
+    def summary(self, normalize=False, decimals=5):
+        """Convert the results to a summarized format."""
         if self.probs is not None:
-            LOGGER.warning("Warning: Classify task do not support `tojson` yet.")
+            LOGGER.warning("Warning: Classify results do not support the `summary()` method yet.")
             return
 
-        import json
-
         # Create list of detection dictionaries
         results = []
         data = self.boxes.data.cpu().tolist()
         h, w = self.orig_shape if normalize else (1, 1)
         for i, row in enumerate(data):  # xyxy, track_id if tracking, conf, class_id
-            box = {"x1": row[0] / w, "y1": row[1] / h, "x2": row[2] / w, "y2": row[3] / h}
-            conf = row[-2]
+            box = {
+                "x1": round(row[0] / w, decimals),
+                "y1": round(row[1] / h, decimals),
+                "x2": round(row[2] / w, decimals),
+                "y2": round(row[3] / h, decimals),
+            }
+            conf = round(row[-2], decimals)
             class_id = int(row[-1])
-            name = self.names[class_id]
-            result = {"name": name, "class": class_id, "confidence": conf, "box": box}
+            result = {"name": self.names[class_id], "class": class_id, "confidence": conf, "box": box}
             if self.boxes.is_track:
                 result["track_id"] = int(row[-3])  # track ID
             if self.masks:
-                x, y = self.masks.xy[i][:, 0], self.masks.xy[i][:, 1]  # numpy array
-                result["segments"] = {"x": (x / w).tolist(), "y": (y / h).tolist()}
+                result["segments"] = {
+                    "x": (self.masks.xy[i][:, 0] / w).round(decimals).tolist(),
+                    "y": (self.masks.xy[i][:, 1] / h).round(decimals).tolist(),
+                }
             if self.keypoints is not None:
                 x, y, visible = self.keypoints[i].data[0].cpu().unbind(dim=1)  # torch Tensor
-                result["keypoints"] = {"x": (x / w).tolist(), "y": (y / h).tolist(), "visible": visible.tolist()}
+                result["keypoints"] = {
+                    "x": (x / w).numpy().round(decimals).tolist(),  # decimals named argument required
+                    "y": (y / h).numpy().round(decimals).tolist(),
+                    "visible": visible.numpy().round(decimals).tolist(),
+                }
             results.append(result)
 
-        # Convert detections to JSON
-        return json.dumps(results, indent=2)
+        return results
+
+    def tojson(self, normalize=False, decimals=5):
+        """Convert the results to JSON format."""
+        import json
+
+        return json.dumps(self.summary(normalize=normalize, decimals=decimals), indent=2)
 
 
 class Boxes(BaseTensor):
     """
-    A class for storing and manipulating detection boxes.
-
-    Args:
-        boxes (torch.Tensor | numpy.ndarray): A tensor or numpy array containing the detection boxes,
-            with shape (num_boxes, 6) or (num_boxes, 7). The last two columns contain confidence and class values.
-            If present, the third last column contains track IDs.
-        orig_shape (tuple): Original image size, in the format (height, width).
+    Manages detection boxes, providing easy access and manipulation of box coordinates, confidence scores, class
+    identifiers, and optional tracking IDs. Supports multiple formats for box coordinates, including both absolute and
+    normalized forms.
 
     Attributes:
-        xyxy (torch.Tensor | numpy.ndarray): The boxes in xyxy format.
-        conf (torch.Tensor | numpy.ndarray): The confidence values of the boxes.
-        cls (torch.Tensor | numpy.ndarray): The class values of the boxes.
-        id (torch.Tensor | numpy.ndarray): The track IDs of the boxes (if available).
-        xywh (torch.Tensor | numpy.ndarray): The boxes in xywh format.
-        xyxyn (torch.Tensor | numpy.ndarray): The boxes in xyxy format normalized by original image size.
-        xywhn (torch.Tensor | numpy.ndarray): The boxes in xywh format normalized by original image size.
-        data (torch.Tensor): The raw bboxes tensor (alias for `boxes`).
+        data (torch.Tensor): The raw tensor containing detection boxes and their associated data.
+        orig_shape (tuple): The original image size as a tuple (height, width), used for normalization.
+        is_track (bool): Indicates whether tracking IDs are included in the box data.
+
+    Properties:
+        xyxy (torch.Tensor | numpy.ndarray): Boxes in [x1, y1, x2, y2] format.
+        conf (torch.Tensor | numpy.ndarray): Confidence scores for each box.
+        cls (torch.Tensor | numpy.ndarray): Class labels for each box.
+        id (torch.Tensor | numpy.ndarray, optional): Tracking IDs for each box, if available.
+        xywh (torch.Tensor | numpy.ndarray): Boxes in [x, y, width, height] format, calculated on demand.
+        xyxyn (torch.Tensor | numpy.ndarray): Normalized [x1, y1, x2, y2] boxes, relative to `orig_shape`.
+        xywhn (torch.Tensor | numpy.ndarray): Normalized [x, y, width, height] boxes, relative to `orig_shape`.
 
     Methods:
-        cpu(): Move the object to CPU memory.
-        numpy(): Convert the object to a numpy array.
-        cuda(): Move the object to CUDA memory.
-        to(*args, **kwargs): Move the object to the specified device.
+        cpu(): Moves the boxes to CPU memory.
+        numpy(): Converts the boxes to a numpy array format.
+        cuda(): Moves the boxes to CUDA (GPU) memory.
+        to(device, dtype=None): Moves the boxes to the specified device.
     """
 
     def __init__(self, boxes, orig_shape) -> None:
-        """Initialize the Boxes class."""
+        """
+        Initialize the Boxes class.
+
+        Args:
+            boxes (torch.Tensor | numpy.ndarray): A tensor or numpy array containing the detection boxes, with
+                shape (num_boxes, 6) or (num_boxes, 7). The last two columns contain confidence and class values.
+                If present, the third last column contains track IDs.
+            orig_shape (tuple): Original image size, in the format (height, width).
+        """
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
-        assert n in (6, 7), f"expected 6 or 7 values but got {n}"  # xyxy, track_id, conf, cls
+        assert n in {6, 7}, f"expected 6 or 7 values but got {n}"  # xyxy, track_id, conf, cls
         super().__init__(boxes, orig_shape)
         self.is_track = n == 7
         self.orig_shape = orig_shape
 
     @property
     def xyxy(self):
         """Return the boxes in xyxy format."""
@@ -603,15 +666,15 @@
         orig_shape (tuple): Original image size, in the format (height, width).
 
     Attributes:
         xywhr (torch.Tensor | numpy.ndarray): The boxes in [x_center, y_center, width, height, rotation] format.
         conf (torch.Tensor | numpy.ndarray): The confidence values of the boxes.
         cls (torch.Tensor | numpy.ndarray): The class values of the boxes.
         id (torch.Tensor | numpy.ndarray): The track IDs of the boxes (if available).
-        xyxyxyxyn (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format normalized by original image size.
+        xyxyxyxyn (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format normalized by orig image size.
         xyxyxyxy (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format.
         xyxy (torch.Tensor | numpy.ndarray): The horizontal boxes in xyxyxyxy format.
         data (torch.Tensor): The raw OBB tensor (alias for `boxes`).
 
     Methods:
         cpu(): Move the object to CPU memory.
         numpy(): Convert the object to a numpy array.
@@ -620,15 +683,15 @@
     """
 
     def __init__(self, boxes, orig_shape) -> None:
         """Initialize the Boxes class."""
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
-        assert n in (7, 8), f"expected 7 or 8 values but got {n}"  # xywh, rotation, track_id, conf, cls
+        assert n in {7, 8}, f"expected 7 or 8 values but got {n}"  # xywh, rotation, track_id, conf, cls
         super().__init__(boxes, orig_shape)
         self.is_track = n == 8
         self.orig_shape = orig_shape
 
     @property
     def xywhr(self):
         """Return the rotated boxes in xywhr format."""
@@ -657,15 +720,15 @@
 
     @property
     @lru_cache(maxsize=2)
     def xyxyxyxyn(self):
         """Return the boxes in xyxyxyxy format, (N, 4, 2)."""
         xyxyxyxyn = self.xyxyxyxy.clone() if isinstance(self.xyxyxyxy, torch.Tensor) else np.copy(self.xyxyxyxy)
         xyxyxyxyn[..., 0] /= self.orig_shape[1]
-        xyxyxyxyn[..., 1] /= self.orig_shape[1]
+        xyxyxyxyn[..., 1] /= self.orig_shape[0]
         return xyxyxyxyn
 
     @property
     @lru_cache(maxsize=2)
     def xyxy(self):
         """
         Return the horizontal boxes in xyxy format, (N, 4).
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/trainer.py` & `ultralytics-8.2.0/ultralytics/engine/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from ultralytics.utils.autobatch import check_train_batch_size
 from ultralytics.utils.checks import check_amp, check_file, check_imgsz, check_model_file_from_stem, print_args
 from ultralytics.utils.dist import ddp_cleanup, generate_ddp_command
 from ultralytics.utils.files import get_latest_run
 from ultralytics.utils.torch_utils import (
     EarlyStopping,
     ModelEMA,
-    de_parallel,
+    convert_optimizer_state_dict_to_fp16,
     init_seeds,
     one_cycle,
     select_device,
     strip_optimizer,
 )
 
 
@@ -103,44 +103,34 @@
         self.plots = {}
         init_seeds(self.args.seed + 1 + RANK, deterministic=self.args.deterministic)
 
         # Dirs
         self.save_dir = get_save_dir(self.args)
         self.args.name = self.save_dir.name  # update name for loggers
         self.wdir = self.save_dir / "weights"  # weights dir
-        if RANK in (-1, 0):
+        if RANK in {-1, 0}:
             self.wdir.mkdir(parents=True, exist_ok=True)  # make dir
             self.args.save_dir = str(self.save_dir)
             yaml_save(self.save_dir / "args.yaml", vars(self.args))  # save run args
         self.last, self.best = self.wdir / "last.pt", self.wdir / "best.pt"  # checkpoint paths
         self.save_period = self.args.save_period
 
         self.batch_size = self.args.batch
         self.epochs = self.args.epochs
         self.start_epoch = 0
         if RANK == -1:
             print_args(vars(self.args))
 
         # Device
-        if self.device.type in ("cpu", "mps"):
+        if self.device.type in {"cpu", "mps"}:
             self.args.workers = 0  # faster CPU training as time dominated by inference, not dataloading
 
         # Model and Dataset
         self.model = check_model_file_from_stem(self.args.model)  # add suffix, i.e. yolov8n -> yolov8n.pt
-        try:
-            if self.args.task == "classify":
-                self.data = check_cls_dataset(self.args.data)
-            elif self.args.data.split(".")[-1] in ("yaml", "yml") or self.args.task in ("detect", "segment", "pose"):
-                self.data = check_det_dataset(self.args.data)
-                if "yaml_file" in self.data:
-                    self.args.data = self.data["yaml_file"]  # for validating 'yolo train data=url.zip' usage
-        except Exception as e:
-            raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
-
-        self.trainset, self.testset = self.get_dataset(self.data)
+        self.trainset, self.testset = self.get_dataset()
         self.ema = None
 
         # Optimization utils init
         self.lf = None
         self.scheduler = None
 
         # Epoch level metrics
@@ -150,15 +140,15 @@
         self.tloss = None
         self.loss_names = ["Loss"]
         self.csv = self.save_dir / "results.csv"
         self.plot_idx = [0, 1, 2]
 
         # Callbacks
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
-        if RANK in (-1, 0):
+        if RANK in {-1, 0}:
             callbacks.add_integration_callbacks(self)
 
     def add_callback(self, event: str, callback):
         """Appends the given callback."""
         self.callbacks[event].append(callback)
 
     def set_callback(self, event: str, callback):
@@ -216,17 +206,17 @@
         self.scheduler = optim.lr_scheduler.LambdaLR(self.optimizer, lr_lambda=self.lf)
 
     def _setup_ddp(self, world_size):
         """Initializes and sets the DistributedDataParallel parameters for training."""
         torch.cuda.set_device(RANK)
         self.device = torch.device("cuda", RANK)
         # LOGGER.info(f'DDP info: RANK {RANK}, WORLD_SIZE {world_size}, DEVICE {self.device}')
-        os.environ["NCCL_BLOCKING_WAIT"] = "1"  # set to enforce timeout
+        os.environ["TORCH_NCCL_BLOCKING_WAIT"] = "1"  # set to enforce timeout
         dist.init_process_group(
-            "nccl" if dist.is_nccl_available() else "gloo",
+            backend="nccl" if dist.is_nccl_available() else "gloo",
             timeout=timedelta(seconds=10800),  # 3 hours
             rank=RANK,
             world_size=world_size,
         )
 
     def _setup_train(self, world_size):
         """Builds dataloaders and optimizer on correct rank process."""
@@ -248,48 +238,48 @@
         always_freeze_names = [".dfl"]  # always freeze these layers
         freeze_layer_names = [f"model.{x}." for x in freeze_list] + always_freeze_names
         for k, v in self.model.named_parameters():
             # v.register_hook(lambda x: torch.nan_to_num(x))  # NaN to 0 (commented for erratic training results)
             if any(x in k for x in freeze_layer_names):
                 LOGGER.info(f"Freezing layer '{k}'")
                 v.requires_grad = False
-            elif not v.requires_grad:
+            elif not v.requires_grad and v.dtype.is_floating_point:  # only floating point Tensor can require gradients
                 LOGGER.info(
                     f"WARNING ⚠️ setting 'requires_grad=True' for frozen layer '{k}'. "
                     "See ultralytics.engine.trainer for customization of frozen layers."
                 )
                 v.requires_grad = True
 
         # Check AMP
         self.amp = torch.tensor(self.args.amp).to(self.device)  # True or False
-        if self.amp and RANK in (-1, 0):  # Single-GPU and DDP
+        if self.amp and RANK in {-1, 0}:  # Single-GPU and DDP
             callbacks_backup = callbacks.default_callbacks.copy()  # backup callbacks as check_amp() resets them
             self.amp = torch.tensor(check_amp(self.model), device=self.device)
             callbacks.default_callbacks = callbacks_backup  # restore callbacks
         if RANK > -1 and world_size > 1:  # DDP
             dist.broadcast(self.amp, src=0)  # broadcast the tensor from rank 0 to all other ranks (returns None)
         self.amp = bool(self.amp)  # as boolean
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.amp)
         if world_size > 1:
             self.model = nn.parallel.DistributedDataParallel(self.model, device_ids=[RANK])
 
         # Check imgsz
         gs = max(int(self.model.stride.max() if hasattr(self.model, "stride") else 32), 32)  # grid size (max stride)
         self.args.imgsz = check_imgsz(self.args.imgsz, stride=gs, floor=gs, max_dim=1)
-        self.stride = gs  # for multi-scale training
+        self.stride = gs  # for multiscale training
 
         # Batch size
         if self.batch_size == -1 and RANK == -1:  # single-GPU only, estimate best batch size
             self.args.batch = self.batch_size = check_train_batch_size(self.model, self.args.imgsz, self.amp)
 
         # Dataloaders
         batch_size = self.batch_size // max(world_size, 1)
         self.train_loader = self.get_dataloader(self.trainset, batch_size=batch_size, rank=RANK, mode="train")
-        if RANK in (-1, 0):
-            # NOTE: When training DOTA dataset, double batch size could get OOM cause some images got more than 2000 objects.
+        if RANK in {-1, 0}:
+            # Note: When training DOTA dataset, double batch size could get OOM on images with >2000 objects.
             self.test_loader = self.get_dataloader(
                 self.testset, batch_size=batch_size if self.args.task == "obb" else batch_size * 2, rank=-1, mode="val"
             )
             self.validator = self.get_validator()
             metric_keys = self.validator.metrics.keys + self.label_loss_items(prefix="val")
             self.metrics = dict(zip(metric_keys, [0] * len(metric_keys)))
             self.ema = ModelEMA(self.model)
@@ -333,28 +323,32 @@
             f'Using {self.train_loader.num_workers * (world_size or 1)} dataloader workers\n'
             f"Logging results to {colorstr('bold', self.save_dir)}\n"
             f'Starting training for ' + (f"{self.args.time} hours..." if self.args.time else f"{self.epochs} epochs...")
         )
         if self.args.close_mosaic:
             base_idx = (self.epochs - self.args.close_mosaic) * nb
             self.plot_idx.extend([base_idx, base_idx + 1, base_idx + 2])
-        epoch = self.epochs  # predefine for resume fully trained model edge cases
-        for epoch in range(self.start_epoch, self.epochs):
+        epoch = self.start_epoch
+        while True:
             self.epoch = epoch
             self.run_callbacks("on_train_epoch_start")
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")  # suppress 'Detected lr_scheduler.step() before optimizer.step()'
+                self.scheduler.step()
+
             self.model.train()
             if RANK != -1:
                 self.train_loader.sampler.set_epoch(epoch)
             pbar = enumerate(self.train_loader)
             # Update dataloader attributes (optional)
             if epoch == (self.epochs - self.args.close_mosaic):
                 self._close_dataloader_mosaic()
                 self.train_loader.reset()
 
-            if RANK in (-1, 0):
+            if RANK in {-1, 0}:
                 LOGGER.info(self.progress_string())
                 pbar = TQDM(enumerate(self.train_loader), total=nb)
             self.tloss = None
             self.optimizer.zero_grad()
             for i, batch in pbar:
                 self.run_callbacks("on_train_batch_start")
                 # Warmup
@@ -398,127 +392,147 @@
                         if self.stop:  # training time exceeded
                             break
 
                 # Log
                 mem = f"{torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0:.3g}G"  # (GB)
                 loss_len = self.tloss.shape[0] if len(self.tloss.shape) else 1
                 losses = self.tloss if loss_len > 1 else torch.unsqueeze(self.tloss, 0)
-                if RANK in (-1, 0):
+                if RANK in {-1, 0}:
                     pbar.set_description(
                         ("%11s" * 2 + "%11.4g" * (2 + loss_len))
                         % (f"{epoch + 1}/{self.epochs}", mem, *losses, batch["cls"].shape[0], batch["img"].shape[-1])
                     )
                     self.run_callbacks("on_batch_end")
                     if self.args.plots and ni in self.plot_idx:
                         self.plot_training_samples(batch, ni)
 
                 self.run_callbacks("on_train_batch_end")
 
             self.lr = {f"lr/pg{ir}": x["lr"] for ir, x in enumerate(self.optimizer.param_groups)}  # for loggers
             self.run_callbacks("on_train_epoch_end")
-            if RANK in (-1, 0):
-                final_epoch = epoch + 1 == self.epochs
+            if RANK in {-1, 0}:
+                final_epoch = epoch + 1 >= self.epochs
                 self.ema.update_attr(self.model, include=["yaml", "nc", "args", "names", "stride", "class_weights"])
 
                 # Validation
                 if self.args.val or final_epoch or self.stopper.possible_stop or self.stop:
                     self.metrics, self.fitness = self.validate()
                 self.save_metrics(metrics={**self.label_loss_items(self.tloss), **self.metrics, **self.lr})
-                self.stop |= self.stopper(epoch + 1, self.fitness)
+                self.stop |= self.stopper(epoch + 1, self.fitness) or final_epoch
                 if self.args.time:
                     self.stop |= (time.time() - self.train_time_start) > (self.args.time * 3600)
 
                 # Save model
                 if self.args.save or final_epoch:
                     self.save_model()
                     self.run_callbacks("on_model_save")
 
             # Scheduler
             t = time.time()
             self.epoch_time = t - self.epoch_time_start
             self.epoch_time_start = t
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore")  # suppress 'Detected lr_scheduler.step() before optimizer.step()'
-                if self.args.time:
-                    mean_epoch_time = (t - self.train_time_start) / (epoch - self.start_epoch + 1)
-                    self.epochs = self.args.epochs = math.ceil(self.args.time * 3600 / mean_epoch_time)
-                    self._setup_scheduler()
-                    self.scheduler.last_epoch = self.epoch  # do not move
-                    self.stop |= epoch >= self.epochs  # stop if exceeded epochs
-                self.scheduler.step()
+            if self.args.time:
+                mean_epoch_time = (t - self.train_time_start) / (epoch - self.start_epoch + 1)
+                self.epochs = self.args.epochs = math.ceil(self.args.time * 3600 / mean_epoch_time)
+                self._setup_scheduler()
+                self.scheduler.last_epoch = self.epoch  # do not move
+                self.stop |= epoch >= self.epochs  # stop if exceeded epochs
             self.run_callbacks("on_fit_epoch_end")
             torch.cuda.empty_cache()  # clear GPU memory at end of epoch, may help reduce CUDA out of memory errors
 
             # Early Stopping
             if RANK != -1:  # if DDP training
                 broadcast_list = [self.stop if RANK == 0 else None]
                 dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                 self.stop = broadcast_list[0]
             if self.stop:
                 break  # must break all DDP ranks
+            epoch += 1
 
-        if RANK in (-1, 0):
+        if RANK in {-1, 0}:
             # Do final val with best.pt
             LOGGER.info(
                 f"\n{epoch - self.start_epoch + 1} epochs completed in "
                 f"{(time.time() - self.train_time_start) / 3600:.3f} hours."
             )
             self.final_eval()
             if self.args.plots:
                 self.plot_metrics()
             self.run_callbacks("on_train_end")
         torch.cuda.empty_cache()
         self.run_callbacks("teardown")
 
     def save_model(self):
         """Save model training checkpoints with additional metadata."""
-        import pandas as pd  # scope for faster startup
+        import io
+
+        import pandas as pd  # scope for faster 'import ultralytics'
 
-        metrics = {**self.metrics, **{"fitness": self.fitness}}
-        results = {k.strip(): v for k, v in pd.read_csv(self.csv).to_dict(orient="list").items()}
-        ckpt = {
-            "epoch": self.epoch,
-            "best_fitness": self.best_fitness,
-            "model": deepcopy(de_parallel(self.model)).half(),
-            "ema": deepcopy(self.ema.ema).half(),
-            "updates": self.ema.updates,
-            "optimizer": self.optimizer.state_dict(),
-            "train_args": vars(self.args),  # save as dict
-            "train_metrics": metrics,
-            "train_results": results,
-            "date": datetime.now().isoformat(),
-            "version": __version__,
-        }
+        # Serialize ckpt to a byte buffer once (faster than repeated torch.save() calls)
+        buffer = io.BytesIO()
+        torch.save(
+            {
+                "epoch": self.epoch,
+                "best_fitness": self.best_fitness,
+                "model": None,  # resume and final checkpoints derive from EMA
+                "ema": deepcopy(self.ema.ema).half(),
+                "updates": self.ema.updates,
+                "optimizer": convert_optimizer_state_dict_to_fp16(deepcopy(self.optimizer.state_dict())),
+                "train_args": vars(self.args),  # save as dict
+                "train_metrics": {**self.metrics, **{"fitness": self.fitness}},
+                "train_results": {k.strip(): v for k, v in pd.read_csv(self.csv).to_dict(orient="list").items()},
+                "date": datetime.now().isoformat(),
+                "version": __version__,
+                "license": "AGPL-3.0 (https://ultralytics.com/license)",
+                "docs": "https://docs.ultralytics.com",
+            },
+            buffer,
+        )
+        serialized_ckpt = buffer.getvalue()  # get the serialized content to save
 
-        # Save last and best
-        torch.save(ckpt, self.last)
+        # Save checkpoints
+        self.last.write_bytes(serialized_ckpt)  # save last.pt
         if self.best_fitness == self.fitness:
-            torch.save(ckpt, self.best)
+            self.best.write_bytes(serialized_ckpt)  # save best.pt
         if (self.save_period > 0) and (self.epoch > 0) and (self.epoch % self.save_period == 0):
-            torch.save(ckpt, self.wdir / f"epoch{self.epoch}.pt")
+            (self.wdir / f"epoch{self.epoch}.pt").write_bytes(serialized_ckpt)  # save epoch, i.e. 'epoch3.pt'
 
-    @staticmethod
-    def get_dataset(data):
+    def get_dataset(self):
         """
         Get train, val path from data dict if it exists.
 
         Returns None if data format is not recognized.
         """
+        try:
+            if self.args.task == "classify":
+                data = check_cls_dataset(self.args.data)
+            elif self.args.data.split(".")[-1] in {"yaml", "yml"} or self.args.task in {
+                "detect",
+                "segment",
+                "pose",
+                "obb",
+            }:
+                data = check_det_dataset(self.args.data)
+                if "yaml_file" in data:
+                    self.args.data = data["yaml_file"]  # for validating 'yolo train data=url.zip' usage
+        except Exception as e:
+            raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
+        self.data = data
         return data["train"], data.get("val") or data.get("test")
 
     def setup_model(self):
         """Load/create/download model for any task."""
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
         model, weights = self.model, None
         ckpt = None
         if str(model).endswith(".pt"):
             weights, ckpt = attempt_load_one_weight(model)
-            cfg = ckpt["model"].yaml
+            cfg = weights.yaml
         else:
             cfg = model
         self.model = self.get_model(cfg=cfg, weights=weights, verbose=RANK == -1)  # calls Model(cfg, weights)
         return ckpt
 
     def optimizer_step(self):
         """Perform a single step of the training optimizer with gradient clipping and EMA update."""
@@ -632,46 +646,43 @@
                 # Check that resume data YAML exists, otherwise strip to force re-download of dataset
                 ckpt_args = attempt_load_weights(last).args
                 if not Path(ckpt_args["data"]).exists():
                     ckpt_args["data"] = self.args.data
 
                 resume = True
                 self.args = get_cfg(ckpt_args)
-                self.args.model = str(last)  # reinstate model
-                for k in "imgsz", "batch":  # allow arg updates to reduce memory on resume if crashed due to CUDA OOM
+                self.args.model = self.args.resume = str(last)  # reinstate model
+                for k in "imgsz", "batch", "device":  # allow arg updates to reduce memory or update device on resume
                     if k in overrides:
                         setattr(self.args, k, overrides[k])
 
             except Exception as e:
                 raise FileNotFoundError(
                     "Resume checkpoint not found. Please pass a valid checkpoint to resume from, "
                     "i.e. 'yolo train resume model=path/to/last.pt'"
                 ) from e
         self.resume = resume
 
     def resume_training(self, ckpt):
         """Resume YOLO training from given epoch and best fitness."""
-        if ckpt is None:
+        if ckpt is None or not self.resume:
             return
         best_fitness = 0.0
-        start_epoch = ckpt["epoch"] + 1
-        if ckpt["optimizer"] is not None:
+        start_epoch = ckpt.get("epoch", -1) + 1
+        if ckpt.get("optimizer", None) is not None:
             self.optimizer.load_state_dict(ckpt["optimizer"])  # optimizer
             best_fitness = ckpt["best_fitness"]
         if self.ema and ckpt.get("ema"):
             self.ema.ema.load_state_dict(ckpt["ema"].float().state_dict())  # EMA
             self.ema.updates = ckpt["updates"]
-        if self.resume:
-            assert start_epoch > 0, (
-                f"{self.args.model} training to {self.epochs} epochs is finished, nothing to resume.\n"
-                f"Start a new training without resuming, i.e. 'yolo train model={self.args.model}'"
-            )
-            LOGGER.info(
-                f"Resuming training from {self.args.model} from epoch {start_epoch + 1} to {self.epochs} total epochs"
-            )
+        assert start_epoch > 0, (
+            f"{self.args.model} training to {self.epochs} epochs is finished, nothing to resume.\n"
+            f"Start a new training without resuming, i.e. 'yolo train model={self.args.model}'"
+        )
+        LOGGER.info(f"Resuming training {self.args.model} from epoch {start_epoch + 1} to {self.epochs} total epochs")
         if self.epochs < start_epoch:
             LOGGER.info(
                 f"{self.model} has been trained for {ckpt['epoch']} epochs. Fine-tuning for {self.epochs} more epochs."
             )
             self.epochs += ckpt["epoch"]  # finetune additional epochs
         self.best_fitness = best_fitness
         self.start_epoch = start_epoch
@@ -724,15 +735,15 @@
                 if "bias" in fullname:  # bias (no decay)
                     g[2].append(param)
                 elif isinstance(module, bn):  # weight (no decay)
                     g[1].append(param)
                 else:  # weight (with decay)
                     g[0].append(param)
 
-        if name in ("Adam", "Adamax", "AdamW", "NAdam", "RAdam"):
+        if name in {"Adam", "Adamax", "AdamW", "NAdam", "RAdam"}:
             optimizer = getattr(optim, name, optim.Adam)(g[2], lr=lr, betas=(momentum, 0.999), weight_decay=0.0)
         elif name == "RMSProp":
             optimizer = optim.RMSprop(g[2], lr=lr, momentum=momentum)
         elif name == "SGD":
             optimizer = optim.SGD(g[2], lr=lr, momentum=momentum, nesterov=True)
         else:
             raise NotImplementedError(
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/tuner.py` & `ultralytics-8.2.0/ultralytics/engine/tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ```python
     from ultralytics import YOLO
 
     model = YOLO('yolov8n.pt')
     model.tune(data='coco8.yaml', epochs=10, iterations=300, optimizer='AdamW', plots=False, save=False, val=False)
     ```
 """
+
 import random
 import shutil
 import subprocess
 import time
 
 import numpy as np
 import torch
@@ -90,14 +91,15 @@
             "degrees": (0.0, 45.0),  # image rotation (+/- deg)
             "translate": (0.0, 0.9),  # image translation (+/- fraction)
             "scale": (0.0, 0.95),  # image scale (+/- gain)
             "shear": (0.0, 10.0),  # image shear (+/- deg)
             "perspective": (0.0, 0.001),  # image perspective (+/- fraction), range 0-0.001
             "flipud": (0.0, 1.0),  # image flip up-down (probability)
             "fliplr": (0.0, 1.0),  # image flip left-right (probability)
+            "bgr": (0.0, 1.0),  # image channel bgr (probability)
             "mosaic": (0.0, 1.0),  # image mixup (probability)
             "mixup": (0.0, 1.0),  # image mixup (probability)
             "copy_paste": (0.0, 1.0),  # segment copy-paste (probability)
         }
         self.args = get_cfg(overrides=args)
         self.tune_dir = get_save_dir(self.args, name="tune")
         self.tune_csv = self.tune_dir / "tune_results.csv"
@@ -183,19 +185,19 @@
             mutated_hyp = self._mutate()
             LOGGER.info(f"{self.prefix}Starting iteration {i + 1}/{iterations} with hyperparameters: {mutated_hyp}")
 
             metrics = {}
             train_args = {**vars(self.args), **mutated_hyp}
             save_dir = get_save_dir(get_cfg(train_args))
             weights_dir = save_dir / "weights"
-            ckpt_file = weights_dir / ("best.pt" if (weights_dir / "best.pt").exists() else "last.pt")
             try:
                 # Train YOLO model with mutated hyperparameters (run in subprocess to avoid dataloader hang)
                 cmd = ["yolo", "train", *(f"{k}={v}" for k, v in train_args.items())]
                 return_code = subprocess.run(cmd, check=True).returncode
+                ckpt_file = weights_dir / ("best.pt" if (weights_dir / "best.pt").exists() else "last.pt")
                 metrics = torch.load(ckpt_file)["train_metrics"]
                 assert return_code == 0, "training failed"
 
             except Exception as e:
                 LOGGER.warning(f"WARNING ❌️ training failure for hyperparameter tuning iteration {i + 1}\n{e}")
 
             # Save results and mutated_hyp to CSV
@@ -212,15 +214,15 @@
             best_is_current = best_idx == i
             if best_is_current:
                 best_save_dir = save_dir
                 best_metrics = {k: round(v, 5) for k, v in metrics.items()}
                 for ckpt in weights_dir.glob("*.pt"):
                     shutil.copy2(ckpt, self.tune_dir / "weights")
             elif cleanup:
-                shutil.rmtree(ckpt_file.parent)  # remove iteration weights/ dir to reduce storage space
+                shutil.rmtree(weights_dir, ignore_errors=True)  # remove iteration weights/ dir to reduce storage space
 
             # Plot tune results
             plot_tune_results(self.tune_csv)
 
             # Save and print tune results
             header = (
                 f'{self.prefix}{i + 1}/{iterations} iterations complete ✅ ({time.time() - t0:.2f}s)\n'
```

### Comparing `ultralytics-8.1.9/ultralytics/engine/validator.py` & `ultralytics-8.2.0/ultralytics/engine/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
                           yolov8n.engine             # TensorRT
                           yolov8n.mlpackage          # CoreML (macOS-only)
                           yolov8n_saved_model        # TensorFlow SavedModel
                           yolov8n.pb                 # TensorFlow GraphDef
                           yolov8n.tflite             # TensorFlow Lite
                           yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                           yolov8n_paddle_model       # PaddlePaddle
+                          yolov8n_ncnn_model         # NCNN
 """
+
 import json
 import time
 from pathlib import Path
 
 import numpy as np
 import torch
 
@@ -116,15 +118,15 @@
             # self.model = model
             self.loss = torch.zeros_like(trainer.loss_items, device=trainer.device)
             self.args.plots &= trainer.stopper.possible_stop or (trainer.epoch == trainer.epochs - 1)
             model.eval()
         else:
             callbacks.add_integration_callbacks(self)
             model = AutoBackend(
-                model or self.args.model,
+                weights=model or self.args.model,
                 device=select_device(self.args.device, self.args.batch),
                 dnn=self.args.dnn,
                 data=self.args.data,
                 fp16=self.args.half,
             )
             # self.model = model
             self.device = model.device  # update device
@@ -133,22 +135,22 @@
             imgsz = check_imgsz(self.args.imgsz, stride=stride)
             if engine:
                 self.args.batch = model.batch_size
             elif not pt and not jit:
                 self.args.batch = 1  # export.py models default to batch-size 1
                 LOGGER.info(f"Forcing batch=1 square inference (1,3,{imgsz},{imgsz}) for non-PyTorch models")
 
-            if str(self.args.data).split(".")[-1] in ("yaml", "yml"):
+            if str(self.args.data).split(".")[-1] in {"yaml", "yml"}:
                 self.data = check_det_dataset(self.args.data)
             elif self.args.task == "classify":
                 self.data = check_cls_dataset(self.args.data, split=self.args.split)
             else:
                 raise FileNotFoundError(emojis(f"Dataset '{self.args.data}' for task={self.args.task} not found ❌"))
 
-            if self.device.type in ("cpu", "mps"):
+            if self.device.type in {"cpu", "mps"}:
                 self.args.workers = 0  # faster CPU val as time dominated by inference, not dataloading
             if not pt:
                 self.args.rect = False
             self.stride = model.stride  # used in get_dataloader() for padding
             self.dataloader = self.dataloader or self.get_dataloader(self.data.get(self.args.split), self.args.batch)
 
             model.eval()
```

### Comparing `ultralytics-8.1.9/ultralytics/hub/__init__.py` & `ultralytics-8.2.0/ultralytics/hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         api_key (str, optional): API key to use for authentication.
             If not provided, it will be retrieved from SETTINGS or HUB_API_KEY environment variable.
         save (bool, optional): Whether to save the API key to SETTINGS if authentication is successful.
 
     Returns:
         (bool): True if authentication is successful, False otherwise.
     """
-    checks.check_requirements("hub-sdk>=0.0.2")
+    checks.check_requirements("hub-sdk>=0.0.6")
     from hub_sdk import HUBClient
 
     api_key_url = f"{HUB_WEB_ROOT}/settings?tab=api+keys"  # set the redirect URL
     saved_key = SETTINGS.get("api_key")
     active_key = api_key or saved_key
     credentials = {"api_key": active_key} if active_key and active_key != "" else None  # set credentials
 
@@ -44,15 +44,15 @@
             "New authentication successful ✅" if client.api_key == api_key or not credentials else "Authenticated ✅"
         )
         LOGGER.info(f"{PREFIX}{log_message}")
 
         return True
     else:
         # Failed to authenticate with HUB
-        LOGGER.info(f"{PREFIX}Retrieve API key from {api_key_url}")
+        LOGGER.info(f"{PREFIX}Get API key from {api_key_url} and then run 'yolo hub login API_KEY'")
         return False
 
 
 def logout():
     """
     Log out of Ultralytics HUB by removing the API key from the settings file. To log in again, use 'yolo hub login'.
```

### Comparing `ultralytics-8.1.9/ultralytics/hub/auth.py` & `ultralytics-8.2.0/ultralytics/hub/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import requests
 
 from ultralytics.hub.utils import HUB_API_ROOT, HUB_WEB_ROOT, PREFIX, request_with_credentials
-from ultralytics.utils import LOGGER, SETTINGS, emojis, is_colab
+from ultralytics.utils import IS_COLAB, LOGGER, SETTINGS, emojis
 
 API_KEY_URL = f"{HUB_WEB_ROOT}/settings?tab=api+keys"
 
 
 class Auth:
     """
     Manages authentication processes including API key handling, cookie-based authentication, and header generation.
@@ -46,29 +46,29 @@
                 if verbose:
                     LOGGER.info(f"{PREFIX}Authenticated ✅")
                 return
             else:
                 # Attempt to authenticate with the provided API key
                 success = self.authenticate()
         # If the API key is not provided and the environment is a Google Colab notebook
-        elif is_colab():
+        elif IS_COLAB:
             # Attempt to authenticate using browser cookies
             success = self.auth_with_cookies()
         else:
             # Request an API key
             success = self.request_api_key()
 
         # Update SETTINGS with the new API key after successful authentication
         if success:
             SETTINGS.update({"api_key": self.api_key})
             # Log that the new login was successful
             if verbose:
                 LOGGER.info(f"{PREFIX}New authentication successful ✅")
         elif verbose:
-            LOGGER.info(f"{PREFIX}Retrieve API key from {API_KEY_URL}")
+            LOGGER.info(f"{PREFIX}Get API key from {API_KEY_URL} and then run 'yolo hub login API_KEY'")
 
     def request_api_key(self, max_attempts=3):
         """
         Prompt the user to input their API key.
 
         Returns the model ID.
         """
@@ -105,15 +105,15 @@
         """
         Attempt to fetch authentication via cookies and set id_token. User must be logged in to HUB and running in a
         supported browser.
 
         Returns:
             (bool): True if authentication is successful, False otherwise.
         """
-        if not is_colab():
+        if not IS_COLAB:
             return False  # Currently only works with Colab
         try:
             authn = request_with_credentials(f"{HUB_API_ROOT}/v1/auth/auto")
             if authn.get("success", False):
                 self.id_token = authn.get("data", {}).get("idToken", None)
                 self.authenticate()
                 return True
```

### Comparing `ultralytics-8.1.9/ultralytics/hub/session.py` & `ultralytics-8.2.0/ultralytics/hub/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import threading
 import time
 from http import HTTPStatus
 from pathlib import Path
 
 import requests
 
-from ultralytics.hub.utils import HUB_WEB_ROOT, HELP_MSG, PREFIX, TQDM
-from ultralytics.utils import LOGGER, SETTINGS, __version__, checks, emojis, is_colab
+from ultralytics.hub.utils import HELP_MSG, HUB_WEB_ROOT, PREFIX, TQDM
+from ultralytics.utils import IS_COLAB, LOGGER, SETTINGS, __version__, checks, emojis
 from ultralytics.utils.errors import HUBModelError
 
-AGENT_NAME = f"python-{__version__}-colab" if is_colab() else f"python-{__version__}-local"
+AGENT_NAME = f"python-{__version__}-colab" if IS_COLAB else f"python-{__version__}-local"
 
 
 class HUBTrainingSession:
     """
     HUB training session for Ultralytics HUB YOLO models. Handles model initialization, heartbeats, and checkpointing.
 
     Attributes:
@@ -48,14 +48,15 @@
 
         self.rate_limits = {
             "metrics": 3.0,
             "ckpt": 900.0,
             "heartbeat": 300.0,
         }  # rate limits (seconds)
         self.metrics_queue = {}  # holds metrics for each epoch until upload
+        self.metrics_upload_failed_queue = {}  # holds metrics for each epoch if upload failed
         self.timers = {}  # holds timers in ultralytics/utils/callbacks/hub.py
 
         # Parse input
         api_key, model_id, self.filename = self._parse_identifier(identifier)
 
         # Get credentials
         active_key = api_key or SETTINGS.get("api_key")
@@ -165,58 +166,58 @@
                 raise HUBModelError(
                     f"model='{identifier}' could not be parsed. Check format is correct. "
                     f"Supported formats are Ultralytics HUB URL, apiKey_modelId, modelId, local pt or yaml file."
                 )
 
         return api_key, model_id, filename
 
-    def _set_train_args(self, **kwargs):
-        """Initializes training arguments and creates a model entry on the Ultralytics HUB."""
+    def _set_train_args(self):
+        """
+        Initializes training arguments and creates a model entry on the Ultralytics HUB.
+
+        This method sets up training arguments based on the model's state and updates them with any additional
+        arguments provided. It handles different states of the model, such as whether it's resumable, pretrained,
+        or requires specific file setup.
+
+        Raises:
+            ValueError: If the model is already trained, if required dataset information is missing, or if there are
+                issues with the provided training arguments.
+        """
         if self.model.is_trained():
-            # Model is already trained
             raise ValueError(emojis(f"Model is already trained and uploaded to {self.model_url} 🚀"))
 
         if self.model.is_resumable():
             # Model has saved weights
             self.train_args = {"data": self.model.get_dataset_url(), "resume": True}
             self.model_file = self.model.get_weights_url("last")
         else:
             # Model has no saved weights
-            def get_train_args(config):
-                """Parses an identifier to extract API key, model ID, and filename if applicable."""
-                return {
-                    "batch": config["batchSize"],
-                    "epochs": config["epochs"],
-                    "imgsz": config["imageSize"],
-                    "patience": config["patience"],
-                    "device": config["device"],
-                    "cache": config["cache"],
-                    "data": self.model.get_dataset_url(),
-                }
+            self.train_args = self.model.data.get("train_args")  # new response
 
-            self.train_args = get_train_args(self.model.data.get("config"))
             # Set the model file as either a *.pt or *.yaml file
             self.model_file = (
                 self.model.get_weights_url("parent") if self.model.is_pretrained() else self.model.get_architecture()
             )
 
-        if not self.train_args.get("data"):
-            raise ValueError("Dataset may still be processing. Please wait a minute and try again.")  # RF fix
+        if "data" not in self.train_args:
+            # RF bug - datasets are sometimes not exported
+            raise ValueError("Dataset may still be processing. Please wait a minute and try again.")
 
         self.model_file = checks.check_yolov5u_filename(self.model_file, verbose=False)  # YOLOv5->YOLOv5u
         self.model_id = self.model.id
 
     def request_queue(
         self,
         request_func,
         retry=3,
         timeout=30,
         thread=True,
         verbose=True,
         progress_total=None,
+        stream_reponse=None,
         *args,
         **kwargs,
     ):
         def retry_request():
             """Attempts to call `request_func` with retries, timeout, and optional threading."""
             t0 = time.time()  # Record the start time for the timeout
             for i in range(retry + 1):
@@ -228,16 +229,21 @@
                 if response is None:
                     LOGGER.warning(f"{PREFIX}Received no response from the request. {HELP_MSG}")
                     time.sleep(2**i)  # Exponential backoff before retrying
                     continue  # Skip further processing and retry
 
                 if progress_total:
                     self._show_upload_progress(progress_total, response)
+                elif stream_reponse:
+                    self._iterate_content(response)
 
                 if HTTPStatus.OK <= response.status_code < HTTPStatus.MULTIPLE_CHOICES:
+                    # if request related to metrics upload
+                    if kwargs.get("metrics"):
+                        self.metrics_upload_failed_queue = {}
                     return response  # Success, no need to retry
 
                 if i == 0:
                     # Initial attempt, check status code and provide messages
                     message = self._get_failure_message(response, retry, timeout)
 
                     if verbose:
@@ -245,14 +251,18 @@
 
                 if not self._should_retry(response.status_code):
                     LOGGER.warning(f"{PREFIX}Request failed. {HELP_MSG} ({response.status_code}")
                     break  # Not an error that should be retried, exit loop
 
                 time.sleep(2**i)  # Exponential backoff for retries
 
+            # if request related to metrics upload and exceed retries
+            if response is None and kwargs.get("metrics"):
+                self.metrics_upload_failed_queue.update(kwargs.get("metrics", None))
+
             return response
 
         if thread:
             # Start a new thread to run the retry_request function
             threading.Thread(target=retry_request, daemon=True).start()
         else:
             # If running in the main thread, call retry_request directly
@@ -324,14 +334,15 @@
                 is_best=is_best,
                 map=map,
                 final=final,
                 retry=10,
                 timeout=3600,
                 thread=not final,
                 progress_total=progress_total,
+                stream_reponse=True,
             )
         else:
             LOGGER.warning(f"{PREFIX}WARNING ⚠️ Model upload issue. Missing model {weights}.")
 
     def _show_upload_progress(self, content_length: int, response: requests.Response) -> None:
         """
         Display a progress bar to track the upload progress of a file download.
@@ -342,7 +353,20 @@
 
         Returns:
             None
         """
         with TQDM(total=content_length, unit="B", unit_scale=True, unit_divisor=1024) as pbar:
             for data in response.iter_content(chunk_size=1024):
                 pbar.update(len(data))
+
+    def _iterate_content(self, response: requests.Response) -> None:
+        """
+        Process the streamed HTTP response data.
+
+        Args:
+            response (requests.Response): The response object from the file download request.
+
+        Returns:
+            None
+        """
+        for data in response.iter_content(chunk_size=1024):
+            pass  # Do nothing with data chunks
```

### Comparing `ultralytics-8.1.9/ultralytics/hub/utils.py` & `ultralytics-8.2.0/ultralytics/hub/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import os
 import platform
 import random
-import sys
 import threading
 import time
 from pathlib import Path
 
 import requests
 
 from ultralytics.utils import (
+    ARGV,
     ENVIRONMENT,
+    IS_COLAB,
+    IS_GIT_DIR,
+    IS_PIP_PACKAGE,
     LOGGER,
     ONLINE,
     RANK,
     SETTINGS,
     TESTS_RUNNING,
     TQDM,
     TryExcept,
     __version__,
     colorstr,
     get_git_origin_url,
-    is_colab,
-    is_git_dir,
-    is_pip_package,
 )
 from ultralytics.utils.downloads import GITHUB_ASSETS_NAMES
 
 HUB_API_ROOT = os.environ.get("ULTRALYTICS_HUB_API", "https://api.ultralytics.com")
 HUB_WEB_ROOT = os.environ.get("ULTRALYTICS_HUB_WEB", "https://hub.ultralytics.com")
 
 PREFIX = colorstr("Ultralytics HUB: ")
@@ -44,15 +44,15 @@
 
     Returns:
         (any): The response data from the AJAX request.
 
     Raises:
         OSError: If the function is not run in a Google Colab environment.
     """
-    if not is_colab():
+    if not IS_COLAB:
         raise OSError("request_with_credentials() must run in a Colab environment")
     from google.colab import output  # noqa
     from IPython import display  # noqa
 
     display.display(
         display.Javascript(
             """
@@ -80,15 +80,15 @@
 def requests_with_progress(method, url, **kwargs):
     """
     Make an HTTP request using the specified method and URL, with an optional progress bar.
 
     Args:
         method (str): The HTTP method to use (e.g. 'GET', 'POST').
         url (str): The URL to send the request to.
-        **kwargs (dict): Additional keyword arguments to pass to the underlying `requests.request` function.
+        **kwargs (any): Additional keyword arguments to pass to the underlying `requests.request` function.
 
     Returns:
         (requests.Response): The response object from the HTTP request.
 
     Note:
         - If 'progress' is set to True, the progress bar will display the download progress for responses with a known
         content length.
@@ -118,15 +118,15 @@
         url (str): The URL to make the request to.
         retry (int, optional): Number of retries to attempt before giving up. Default is 3.
         timeout (int, optional): Timeout in seconds after which the function will give up retrying. Default is 30.
         thread (bool, optional): Whether to execute the request in a separate daemon thread. Default is True.
         code (int, optional): An identifier for the request, used for logging purposes. Default is -1.
         verbose (bool, optional): A flag to determine whether to print out to console or not. Default is True.
         progress (bool, optional): Whether to show a progress bar during the request. Default is False.
-        **kwargs (dict): Keyword arguments to be passed to the requests function specified in method.
+        **kwargs (any): Keyword arguments to be passed to the requests function specified in method.
 
     Returns:
         (requests.Response): The HTTP response object. If the request is executed in a separate thread, returns None.
     """
     retry_codes = (408, 500)  # retry only these codes
 
     @TryExcept(verbose=verbose)
@@ -184,28 +184,28 @@
 
     def __init__(self):
         """Initializes the Events object with default values for events, rate_limit, and metadata."""
         self.events = []  # events list
         self.rate_limit = 60.0  # rate limit (seconds)
         self.t = 0.0  # rate limit timer (seconds)
         self.metadata = {
-            "cli": Path(sys.argv[0]).name == "yolo",
-            "install": "git" if is_git_dir() else "pip" if is_pip_package() else "other",
+            "cli": Path(ARGV[0]).name == "yolo",
+            "install": "git" if IS_GIT_DIR else "pip" if IS_PIP_PACKAGE else "other",
             "python": ".".join(platform.python_version_tuple()[:2]),  # i.e. 3.10
             "version": __version__,
             "env": ENVIRONMENT,
             "session_id": round(random.random() * 1e15),
             "engagement_time_msec": 1000,
         }
         self.enabled = (
             SETTINGS["sync"]
-            and RANK in (-1, 0)
+            and RANK in {-1, 0}
             and not TESTS_RUNNING
             and ONLINE
-            and (is_pip_package() or get_git_origin_url() == "https://github.com/ultralytics/ultralytics.git")
+            and (IS_PIP_PACKAGE or get_git_origin_url() == "https://github.com/ultralytics/ultralytics.git")
         )
 
     def __call__(self, cfg):
         """
         Attempts to add a new event to the events list and send events if the rate limit is reached.
 
         Args:
```

### Comparing `ultralytics-8.1.9/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.0/ultralytics/models/fastsam/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 from pathlib import Path
 
 from ultralytics.engine.model import Model
+
 from .predict import FastSAMPredictor
 from .val import FastSAMValidator
 
 
 class FastSAM(Model):
     """
     FastSAM model interface.
@@ -20,14 +21,14 @@
         ```
     """
 
     def __init__(self, model="FastSAM-x.pt"):
         """Call the __init__ method of the parent class (YOLO) with the updated default model."""
         if str(model) == "FastSAM.pt":
             model = "FastSAM-x.pt"
-        assert Path(model).suffix not in (".yaml", ".yml"), "FastSAM models only support pre-trained models."
+        assert Path(model).suffix not in {".yaml", ".yml"}, "FastSAM models only support pre-trained models."
         super().__init__(model=model, task="segment")
 
     @property
     def task_map(self):
         """Returns a dictionary mapping segment task to corresponding predictor and validator classes."""
         return {"segment": {"predictor": FastSAMPredictor, "validator": FastSAMValidator}}
```

### Comparing `ultralytics-8.1.9/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.0/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.0/ultralytics/models/fastsam/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import os
 from pathlib import Path
 
 import cv2
-import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 
-from ultralytics.utils import TQDM
+from ultralytics.utils import TQDM, checks
 
 
 class FastSAMPrompt:
     """
     Fast Segment Anything Model class for image annotation and visualization.
 
     Attributes:
@@ -27,19 +26,17 @@
         """Initializes FastSAMPrompt with given source, results and device, and assigns clip for linear assignment."""
         self.device = device
         self.results = results
         self.source = source
 
         # Import and assign clip
         try:
-            import clip  # for linear_assignment
+            import clip
         except ImportError:
-            from ultralytics.utils.checks import check_requirements
-
-            check_requirements("git+https://github.com/openai/CLIP.git")
+            checks.check_requirements("git+https://github.com/ultralytics/CLIP.git")
             import clip
         self.clip = clip
 
     @staticmethod
     def _segment_image(image, bbox):
         """Segments the given image according to the provided bounding box coordinates."""
         image_array = np.array(image)
@@ -111,18 +108,21 @@
         Args:
             annotations (list): Annotations to be plotted.
             output (str or Path): Output directory for saving the plots.
             bbox (list, optional): Bounding box coordinates [x1, y1, x2, y2]. Defaults to None.
             points (list, optional): Points to be plotted. Defaults to None.
             point_label (list, optional): Labels for the points. Defaults to None.
             mask_random_color (bool, optional): Whether to use random color for masks. Defaults to True.
-            better_quality (bool, optional): Whether to apply morphological transformations for better mask quality. Defaults to True.
+            better_quality (bool, optional): Whether to apply morphological transformations for better mask quality.
+                Defaults to True.
             retina (bool, optional): Whether to use retina mask. Defaults to False.
             with_contours (bool, optional): Whether to plot contours. Defaults to True.
         """
+        import matplotlib.pyplot as plt
+
         pbar = TQDM(annotations, total=len(annotations))
         for ann in pbar:
             result_name = os.path.basename(ann.path)
             image = ann.orig_img[..., ::-1]  # BGR to RGB
             original_h, original_w = ann.orig_shape
             # For macOS only
             # plt.switch_backend('TkAgg')
@@ -199,14 +199,16 @@
             bbox (list, optional): Bounding box coordinates [x1, y1, x2, y2]. Defaults to None.
             points (list, optional): Points to be plotted. Defaults to None.
             pointlabel (list, optional): Labels for the points. Defaults to None.
             retinamask (bool, optional): Whether to use retina mask. Defaults to True.
             target_height (int, optional): Target height for resizing. Defaults to 960.
             target_width (int, optional): Target width for resizing. Defaults to 960.
         """
+        import matplotlib.pyplot as plt
+
         n, h, w = annotation.shape  # batch, height, width
 
         areas = np.sum(annotation, axis=(1, 2))
         annotation = annotation[np.argsort(areas)]
 
         index = (annotation != 0).argmax(axis=0)
         if random_color:
```

### Comparing `ultralytics-8.1.9/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.0/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.0/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/nas/model.py` & `ultralytics-8.2.0/ultralytics/models/nas/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from pathlib import Path
 
 import torch
 
 from ultralytics.engine.model import Model
 from ultralytics.utils.torch_utils import model_info, smart_inference_mode
+
 from .predict import NASPredictor
 from .val import NASValidator
 
 
 class NAS(Model):
     """
     YOLO NAS model for object detection.
@@ -41,15 +42,15 @@
 
     Note:
         YOLO-NAS models only support pre-trained models. Do not provide YAML configuration files.
     """
 
     def __init__(self, model="yolo_nas_s.pt") -> None:
         """Initializes the NAS model with the provided or default 'yolo_nas_s.pt' model."""
-        assert Path(model).suffix not in (".yaml", ".yml"), "YOLO-NAS models only support pre-trained models."
+        assert Path(model).suffix not in {".yaml", ".yml"}, "YOLO-NAS models only support pre-trained models."
         super().__init__(model, task="detect")
 
     @smart_inference_mode()
     def _load(self, weights: str, task: str):
         """Loads an existing NAS model weights or creates a new NAS model with pretrained weights if not provided."""
         import super_gradients
```

### Comparing `ultralytics-8.1.9/ultralytics/models/nas/predict.py` & `ultralytics-8.2.0/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/nas/val.py` & `ultralytics-8.2.0/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.0/ultralytics/models/rtdetr/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 
         Args:
             model (str): Path to the pre-trained model. Defaults to 'rtdetr-l.pt'.
 
         Raises:
             NotImplementedError: If the model file extension is not 'pt', 'yaml', or 'yml'.
         """
-        if model and model.split(".")[-1] not in ("pt", "yaml", "yml"):
-            raise NotImplementedError("RT-DETR only supports creating from *.pt, *.yaml, or *.yml files.")
         super().__init__(model=model, task="detect")
 
     @property
     def task_map(self) -> dict:
         """
         Returns a task map for RT-DETR, associating tasks with corresponding Ultralytics classes.
```

### Comparing `ultralytics-8.1.9/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.0/ultralytics/models/rtdetr/predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,22 +34,25 @@
     def postprocess(self, preds, img, orig_imgs):
         """
         Postprocess the raw predictions from the model to generate bounding boxes and confidence scores.
 
         The method filters detections based on confidence and class if specified in `self.args`.
 
         Args:
-            preds (torch.Tensor): Raw predictions from the model.
+            preds (list): List of [predictions, extra] from the model.
             img (torch.Tensor): Processed input images.
             orig_imgs (list or torch.Tensor): Original, unprocessed images.
 
         Returns:
             (list[Results]): A list of Results objects containing the post-processed bounding boxes, confidence scores,
                 and class labels.
         """
+        if not isinstance(preds, (list, tuple)):  # list for PyTorch inference but list[0] Tensor for export inference
+            preds = [preds, None]
+
         nd = preds[0].shape[-1]
         bboxes, scores = preds[0].split((4, nd - 4), dim=-1)
 
         if not isinstance(orig_imgs, list):  # input images are a torch.Tensor, not a list
             orig_imgs = ops.convert_torch2numpy_batch(orig_imgs)
 
         results = []
```

### Comparing `ultralytics-8.1.9/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.0/ultralytics/models/rtdetr/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import copy
 
 import torch
 
 from ultralytics.models.yolo.detect import DetectionTrainer
 from ultralytics.nn.tasks import RTDETRDetectionModel
 from ultralytics.utils import RANK, colorstr
+
 from .val import RTDETRDataset, RTDETRValidator
 
 
 class RTDETRTrainer(DetectionTrainer):
     """
     Trainer class for the RT-DETR model developed by Baidu for real-time object detection. Extends the DetectionTrainer
     class for YOLO to adapt to the specific features and architecture of RT-DETR. This model leverages Vision
```

### Comparing `ultralytics-8.1.9/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.0/ultralytics/models/rtdetr/val.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,17 @@
             cache=self.args.cache or None,
             prefix=colorstr(f"{mode}: "),
             data=self.data,
         )
 
     def postprocess(self, preds):
         """Apply Non-maximum suppression to prediction outputs."""
+        if not isinstance(preds, (list, tuple)):  # list for PyTorch inference but list[0] Tensor for export inference
+            preds = [preds, None]
+
         bs, _, nd = preds[0].shape
         bboxes, scores = preds[0].split((4, nd - 4), dim=-1)
         bboxes *= self.args.imgsz
         outputs = [torch.zeros((0, 6), device=bboxes.device)] * bs
         for i, bbox in enumerate(bboxes):  # (300, 4)
             bbox = ops.xywh2xyxy(bbox)
             score, cls = scores[i].max(-1)  # (300, )
@@ -118,15 +121,15 @@
         ori_shape = batch["ori_shape"][si]
         imgsz = batch["img"].shape[2:]
         ratio_pad = batch["ratio_pad"][si]
         if len(cls):
             bbox = ops.xywh2xyxy(bbox)  # target boxes
             bbox[..., [0, 2]] *= ori_shape[1]  # native-space pred
             bbox[..., [1, 3]] *= ori_shape[0]  # native-space pred
-        return dict(cls=cls, bbox=bbox, ori_shape=ori_shape, imgsz=imgsz, ratio_pad=ratio_pad)
+        return {"cls": cls, "bbox": bbox, "ori_shape": ori_shape, "imgsz": imgsz, "ratio_pad": ratio_pad}
 
     def _prepare_pred(self, pred, pbatch):
         """Prepares and returns a batch with transformed bounding boxes and class labels."""
         predn = pred.clone()
         predn[..., [0, 2]] *= pbatch["ori_shape"][1] / self.args.imgsz  # native-space pred
         predn[..., [1, 3]] *= pbatch["ori_shape"][0] / self.args.imgsz  # native-space pred
         return predn.float()
```

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/amg.py` & `ultralytics-8.2.0/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/build.py` & `ultralytics-8.2.0/ultralytics/models/sam/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from functools import partial
 
 import torch
 
 from ultralytics.utils.downloads import attempt_download_asset
+
 from .modules.decoders import MaskDecoder
 from .modules.encoders import ImageEncoderViT, PromptEncoder
 from .modules.sam import Sam
 from .modules.tiny_encoder import TinyViT
 from .modules.transformer import TwoWayTransformer
```

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/model.py` & `ultralytics-8.2.0/ultralytics/models/sam/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     - Trained on SA-1B dataset
 """
 
 from pathlib import Path
 
 from ultralytics.engine.model import Model
 from ultralytics.utils.torch_utils import model_info
+
 from .build import build_sam
 from .predict import Predictor
 
 
 class SAM(Model):
     """
     SAM (Segment Anything Model) interface class.
@@ -37,15 +38,15 @@
 
         Args:
             model (str): Path to the pre-trained SAM model file. File should have a .pt or .pth extension.
 
         Raises:
             NotImplementedError: If the model file extension is not .pt or .pth.
         """
-        if model and Path(model).suffix not in (".pt", ".pth"):
+        if model and Path(model).suffix not in {".pt", ".pth"}:
             raise NotImplementedError("SAM prediction requires pre-trained *.pt or *.pth model.")
         super().__init__(model=model, task="segment")
 
     def _load(self, weights: str, task=None):
         """
         Loads the specified weights into the SAM model.
```

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.0/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.0/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.0/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.0/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         super().__init__()
 
         self.input_resolution = input_resolution
         self.dim = dim
         self.out_dim = out_dim
         self.act = activation()
         self.conv1 = Conv2d_BN(dim, out_dim, 1, 1, 0)
-        stride_c = 1 if out_dim in [320, 448, 576] else 2
+        stride_c = 1 if out_dim in {320, 448, 576} else 2
         self.conv2 = Conv2d_BN(out_dim, out_dim, 3, stride_c, 1, groups=out_dim)
         self.conv3 = Conv2d_BN(out_dim, out_dim, 1, 1, 0)
 
     def forward(self, x):
         """Applies forward pass on the input utilizing convolution and activation layers, and returns the result."""
         if x.ndim == 3:
             H, W = self.input_resolution
@@ -580,17 +580,17 @@
         """
         Initializes the TinyViT model.
 
         Args:
             img_size (int, optional): The input image size. Defaults to 224.
             in_chans (int, optional): Number of input channels. Defaults to 3.
             num_classes (int, optional): Number of classification classes. Defaults to 1000.
-            embed_dims (List[int], optional): List of embedding dimensions for each layer. Defaults to [96, 192, 384, 768].
+            embed_dims (List[int], optional): List of embedding dimensions per layer. Defaults to [96, 192, 384, 768].
             depths (List[int], optional): List of depths for each layer. Defaults to [2, 2, 6, 2].
-            num_heads (List[int], optional): List of number of attention heads for each layer. Defaults to [3, 6, 12, 24].
+            num_heads (List[int], optional): List of number of attention heads per layer. Defaults to [3, 6, 12, 24].
             window_sizes (List[int], optional): List of window sizes for each layer. Defaults to [7, 7, 14, 7].
             mlp_ratio (float, optional): Ratio of MLP hidden dimension to embedding dimension. Defaults to 4.
             drop_rate (float, optional): Dropout rate. Defaults to 0.
             drop_path_rate (float, optional): Drop path rate for stochastic depth. Defaults to 0.1.
             use_checkpoint (bool, optional): Whether to use checkpointing for efficient memory usage. Defaults to False.
             mbconv_expand_ratio (float, optional): Expansion ratio for MBConv layer. Defaults to 4.0.
             local_conv_size (int, optional): Local convolution kernel size. Defaults to 3.
```

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.0/ultralytics/models/sam/modules/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
         Args:
             embedding_dim (int): The dimensionality of the input embeddings.
             num_heads (int): The number of attention heads.
             downsample_rate (int, optional): The factor by which the internal dimensions are downsampled. Defaults to 1.
 
         Raises:
-            AssertionError: If 'num_heads' does not evenly divide the internal dimension (embedding_dim / downsample_rate).
+            AssertionError: If 'num_heads' does not evenly divide the internal dim (embedding_dim / downsample_rate).
         """
         super().__init__()
         self.embedding_dim = embedding_dim
         self.internal_dim = embedding_dim // downsample_rate
         self.num_heads = num_heads
         assert self.internal_dim % num_heads == 0, "num_heads must divide embedding_dim."
```

### Comparing `ultralytics-8.1.9/ultralytics/models/sam/predict.py` & `ultralytics-8.2.0/ultralytics/models/sam/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 using SAM. It forms an integral part of the Ultralytics framework and is designed for high-performance, real-time image
 segmentation tasks.
 """
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-import torchvision
 
 from ultralytics.data.augment import LetterBox
 from ultralytics.engine.predictor import BasePredictor
 from ultralytics.engine.results import Results
 from ultralytics.utils import DEFAULT_CFG, ops
 from ultralytics.utils.torch_utils import select_device
+
 from .amg import (
     batch_iterator,
     batched_mask_to_box,
     build_all_layer_point_grids,
     calculate_stability_score,
     generate_crop_boxes,
     is_box_near_crop_edge,
@@ -124,18 +124,18 @@
         Perform image segmentation inference based on the given input cues, using the currently loaded image. This
         method leverages SAM's (Segment Anything Model) architecture consisting of image encoder, prompt encoder, and
         mask decoder for real-time and promptable segmentation tasks.
 
         Args:
             im (torch.Tensor): The preprocessed input image in tensor format, with shape (N, C, H, W).
             bboxes (np.ndarray | List, optional): Bounding boxes with shape (N, 4), in XYXY format.
-            points (np.ndarray | List, optional): Points indicating object locations with shape (N, 2), in pixel coordinates.
-            labels (np.ndarray | List, optional): Labels for point prompts, shape (N, ). 1 for foreground and 0 for background.
-            masks (np.ndarray, optional): Low-resolution masks from previous predictions. Shape should be (N, H, W). For SAM, H=W=256.
-            multimask_output (bool, optional): Flag to return multiple masks. Helpful for ambiguous prompts. Defaults to False.
+            points (np.ndarray | List, optional): Points indicating object locations with shape (N, 2), in pixels.
+            labels (np.ndarray | List, optional): Labels for point prompts, shape (N, ). 1 = foreground, 0 = background.
+            masks (np.ndarray, optional): Low-resolution masks from previous predictions shape (N,H,W). For SAM H=W=256.
+            multimask_output (bool, optional): Flag to return multiple masks. Helpful for ambiguous prompts.
 
         Returns:
             (tuple): Contains the following three elements.
                 - np.ndarray: The output masks in shape CxHxW, where C is the number of generated masks.
                 - np.ndarray: An array of length C containing quality scores predicted by the model for each mask.
                 - np.ndarray: Low-resolution logits of shape CxHxW for subsequent inference, where H=W=256.
         """
@@ -153,18 +153,18 @@
         """
         Internal function for image segmentation inference based on cues like bounding boxes, points, and masks.
         Leverages SAM's specialized architecture for prompt-based, real-time segmentation.
 
         Args:
             im (torch.Tensor): The preprocessed input image in tensor format, with shape (N, C, H, W).
             bboxes (np.ndarray | List, optional): Bounding boxes with shape (N, 4), in XYXY format.
-            points (np.ndarray | List, optional): Points indicating object locations with shape (N, 2), in pixel coordinates.
-            labels (np.ndarray | List, optional): Labels for point prompts, shape (N, ). 1 for foreground and 0 for background.
-            masks (np.ndarray, optional): Low-resolution masks from previous predictions. Shape should be (N, H, W). For SAM, H=W=256.
-            multimask_output (bool, optional): Flag to return multiple masks. Helpful for ambiguous prompts. Defaults to False.
+            points (np.ndarray | List, optional): Points indicating object locations with shape (N, 2), in pixels.
+            labels (np.ndarray | List, optional): Labels for point prompts, shape (N, ). 1 = foreground, 0 = background.
+            masks (np.ndarray, optional): Low-resolution masks from previous predictions shape (N,H,W). For SAM H=W=256.
+            multimask_output (bool, optional): Flag to return multiple masks. Helpful for ambiguous prompts.
 
         Returns:
             (tuple): Contains the following three elements.
                 - np.ndarray: The output masks in shape CxHxW, where C is the number of generated masks.
                 - np.ndarray: An array of length C containing quality scores predicted by the model for each mask.
                 - np.ndarray: Low-resolution logits of shape CxHxW for subsequent inference, where H=W=256.
         """
@@ -227,29 +227,31 @@
         This function segments an entire image into constituent parts by leveraging SAM's advanced architecture
         and real-time performance capabilities. It can optionally work on image crops for finer segmentation.
 
         Args:
             im (torch.Tensor): Input tensor representing the preprocessed image with dimensions (N, C, H, W).
             crop_n_layers (int): Specifies the number of layers for additional mask predictions on image crops.
                                  Each layer produces 2**i_layer number of image crops.
-            crop_overlap_ratio (float): Determines the extent of overlap between crops. Scaled down in subsequent layers.
+            crop_overlap_ratio (float): Determines the overlap between crops. Scaled down in subsequent layers.
             crop_downscale_factor (int): Scaling factor for the number of sampled points-per-side in each layer.
             point_grids (list[np.ndarray], optional): Custom grids for point sampling normalized to [0,1].
                                                       Used in the nth crop layer.
             points_stride (int, optional): Number of points to sample along each side of the image.
                                            Exclusive with 'point_grids'.
             points_batch_size (int): Batch size for the number of points processed simultaneously.
             conf_thres (float): Confidence threshold [0,1] for filtering based on the model's mask quality prediction.
             stability_score_thresh (float): Stability threshold [0,1] for mask filtering based on mask stability.
             stability_score_offset (float): Offset value for calculating stability score.
-            crop_nms_thresh (float): IoU cutoff for Non-Maximum Suppression (NMS) to remove duplicate masks between crops.
+            crop_nms_thresh (float): IoU cutoff for NMS to remove duplicate masks between crops.
 
         Returns:
             (tuple): A tuple containing segmented masks, confidence scores, and bounding boxes.
         """
+        import torchvision  # scope for faster 'import ultralytics'
+
         self.segment_all = True
         ih, iw = im.shape[2:]
         crop_regions, layer_idxs = generate_crop_boxes((ih, iw), crop_n_layers, crop_overlap_ratio)
         if point_grids is None:
             point_grids = build_all_layer_point_grids(points_stride, crop_n_layers, crop_downscale_factor)
         pred_masks, pred_scores, pred_bboxes, region_areas = [], [], [], []
         for crop_region, layer_idx in zip(crop_regions, layer_idxs):
@@ -346,16 +348,16 @@
         self.model.fp16 = False
         self.done_warmup = True
 
     def postprocess(self, preds, img, orig_imgs):
         """
         Post-processes SAM's inference outputs to generate object detection masks and bounding boxes.
 
-        The method scales masks and boxes to the original image size and applies a threshold to the mask predictions. The
-        SAM model uses advanced architecture and promptable segmentation tasks to achieve real-time performance.
+        The method scales masks and boxes to the original image size and applies a threshold to the mask predictions.
+        The SAM model uses advanced architecture and promptable segmentation tasks to achieve real-time performance.
 
         Args:
             preds (tuple): The output from SAM model inference, containing masks, scores, and optional bounding boxes.
             img (torch.Tensor): The processed input image tensor.
             orig_imgs (list | torch.Tensor): The original, unprocessed images.
 
         Returns:
@@ -445,14 +447,16 @@
             nms_thresh (float): The IoU threshold for the NMS algorithm. Defaults to 0.7.
 
         Returns:
             (tuple([torch.Tensor, List[int]])):
                 - new_masks (torch.Tensor): The processed masks with small regions removed. Shape is (N, H, W).
                 - keep (List[int]): The indices of the remaining masks post-NMS, which can be used to filter the boxes.
         """
+        import torchvision  # scope for faster 'import ultralytics'
+
         if len(masks) == 0:
             return masks
 
         # Filter small disconnected regions and holes
         new_masks = []
         scores = []
         for mask in masks:
```

### Comparing `ultralytics-8.1.9/ultralytics/models/utils/loss.py` & `ultralytics-8.2.0/ultralytics/models/utils/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ultralytics.utils.loss import FocalLoss, VarifocalLoss
 from ultralytics.utils.metrics import bbox_iou
+
 from .ops import HungarianMatcher
 
 
 class DETRLoss(nn.Module):
     """
     DETR (DEtection TRansformer) Loss class. This class calculates and returns the different loss components for the
     DETR object detection model. It computes classification loss, bounding box loss, GIoU loss, and optionally auxiliary
```

### Comparing `ultralytics-8.1.9/ultralytics/models/utils/ops.py` & `ultralytics-8.2.0/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.0/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.0/ultralytics/models/yolo/classify/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import torch
-import torchvision
 
 from ultralytics.data import ClassificationDataset, build_dataloader
 from ultralytics.engine.trainer import BaseTrainer
 from ultralytics.models import yolo
 from ultralytics.nn.tasks import ClassificationModel, attempt_load_one_weight
 from ultralytics.utils import DEFAULT_CFG, LOGGER, RANK, colorstr
 from ultralytics.utils.plotting import plot_images, plot_results
@@ -55,29 +54,31 @@
                 m.p = self.args.dropout  # set dropout
         for p in model.parameters():
             p.requires_grad = True  # for training
         return model
 
     def setup_model(self):
         """Load, create or download model for any task."""
+        import torchvision  # scope for faster 'import ultralytics'
+
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
         model, ckpt = str(self.model), None
         # Load a YOLO model locally, from torchvision, or from Ultralytics assets
         if model.endswith(".pt"):
             self.model, ckpt = attempt_load_one_weight(model, device="cpu")
             for p in self.model.parameters():
                 p.requires_grad = True  # for training
-        elif model.split(".")[-1] in ("yaml", "yml"):
+        elif model.split(".")[-1] in {"yaml", "yml"}:
             self.model = self.get_model(cfg=model)
         elif model in torchvision.models.__dict__:
             self.model = torchvision.models.__dict__[model](weights="IMAGENET1K_V1" if self.args.pretrained else None)
         else:
-            FileNotFoundError(f"ERROR: model={model} not found locally or online. Please check model name.")
+            raise FileNotFoundError(f"ERROR: model={model} not found locally or online. Please check model name.")
         ClassificationModel.reshape_outputs(self.model, self.data["nc"])
 
         return ckpt
 
     def build_dataset(self, img_path, mode="train", batch=None):
         """Creates a ClassificationDataset instance given an image path, and mode (train/test etc.)."""
         return ClassificationDataset(root=img_path, args=self.args, augment=mode == "train", prefix=mode)
```

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.0/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.0/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.0/ultralytics/models/yolo/detect/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             batch (int, optional): Size of batches, this is for `rect`. Defaults to None.
         """
         gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
         return build_yolo_dataset(self.args, img_path, batch, self.data, mode=mode, rect=mode == "val", stride=gs)
 
     def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode="train"):
         """Construct and return dataloader."""
-        assert mode in ["train", "val"]
+        assert mode in {"train", "val"}, f"Mode must be 'train' or 'val', not {mode}."
         with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
             dataset = self.build_dataset(dataset_path, mode, batch_size)
         shuffle = mode == "train"
         if getattr(dataset, "rect", False) and shuffle:
             LOGGER.warning("WARNING ⚠️ 'rect=True' is incompatible with DataLoader shuffle, setting shuffle=False")
             shuffle = False
         workers = self.args.workers if mode == "train" else self.args.workers * 2
```

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.0/ultralytics/models/yolo/detect/val.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,19 @@
     """
 
     def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, _callbacks=None):
         """Initialize detection model with necessary variables and settings."""
         super().__init__(dataloader, save_dir, pbar, args, _callbacks)
         self.nt_per_class = None
         self.is_coco = False
+        self.is_lvis = False
         self.class_map = None
         self.args.task = "detect"
         self.metrics = DetMetrics(save_dir=self.save_dir, on_plot=self.on_plot)
-        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
+        self.iouv = torch.linspace(0.5, 0.95, 10)  # IoU vector for mAP@0.5:0.95
         self.niou = self.iouv.numel()
         self.lb = []  # for autolabelling
 
     def preprocess(self, batch):
         """Preprocesses batch of images for YOLO training."""
         batch["img"] = batch["img"].to(self.device, non_blocking=True)
         batch["img"] = (batch["img"].half() if self.args.half else batch["img"].float()) / 255
@@ -62,16 +63,17 @@
 
         return batch
 
     def init_metrics(self, model):
         """Initialize evaluation metrics for YOLO."""
         val = self.data.get(self.args.split, "")  # validation path
         self.is_coco = isinstance(val, str) and "coco" in val and val.endswith(f"{os.sep}val2017.txt")  # is COCO
-        self.class_map = converter.coco80_to_coco91_class() if self.is_coco else list(range(1000))
-        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
+        self.is_lvis = isinstance(val, str) and "lvis" in val and not self.is_coco  # is LVIS
+        self.class_map = converter.coco80_to_coco91_class() if self.is_coco else list(range(len(model.names)))
+        self.args.save_json |= (self.is_coco or self.is_lvis) and not self.training  # run on final val if training COCO
         self.names = model.names
         self.nc = len(model.names)
         self.metrics.names = self.names
         self.metrics.plot = self.args.plots
         self.confusion_matrix = ConfusionMatrix(nc=self.nc, conf=self.args.conf)
         self.seen = 0
         self.jdict = []
@@ -100,15 +102,15 @@
         bbox = batch["bboxes"][idx]
         ori_shape = batch["ori_shape"][si]
         imgsz = batch["img"].shape[2:]
         ratio_pad = batch["ratio_pad"][si]
         if len(cls):
             bbox = ops.xywh2xyxy(bbox) * torch.tensor(imgsz, device=self.device)[[1, 0, 1, 0]]  # target boxes
             ops.scale_boxes(imgsz, bbox, ori_shape, ratio_pad=ratio_pad)  # native-space labels
-        return dict(cls=cls, bbox=bbox, ori_shape=ori_shape, imgsz=imgsz, ratio_pad=ratio_pad)
+        return {"cls": cls, "bbox": bbox, "ori_shape": ori_shape, "imgsz": imgsz, "ratio_pad": ratio_pad}
 
     def _prepare_pred(self, pred, pbatch):
         """Prepares a batch of images and annotations for validation."""
         predn = pred.clone()
         ops.scale_boxes(
             pbatch["imgsz"], predn[:, :4], pbatch["ori_shape"], ratio_pad=pbatch["ratio_pad"]
         )  # native-space pred
@@ -128,31 +130,29 @@
             cls, bbox = pbatch.pop("cls"), pbatch.pop("bbox")
             nl = len(cls)
             stat["target_cls"] = cls
             if npr == 0:
                 if nl:
                     for k in self.stats.keys():
                         self.stats[k].append(stat[k])
-                    # TODO: obb has not supported confusion_matrix yet.
-                    if self.args.plots and self.args.task != "obb":
+                    if self.args.plots:
                         self.confusion_matrix.process_batch(detections=None, gt_bboxes=bbox, gt_cls=cls)
                 continue
 
             # Predictions
             if self.args.single_cls:
                 pred[:, 5] = 0
             predn = self._prepare_pred(pred, pbatch)
             stat["conf"] = predn[:, 4]
             stat["pred_cls"] = predn[:, 5]
 
             # Evaluate
             if nl:
                 stat["tp"] = self._process_batch(predn, bbox, cls)
-                # TODO: obb has not supported confusion_matrix yet.
-                if self.args.plots and self.args.task != "obb":
+                if self.args.plots:
                     self.confusion_matrix.process_batch(predn, bbox, cls)
             for k in self.stats.keys():
                 self.stats[k].append(stat[k])
 
             # Save
             if self.args.save_json:
                 self.pred_to_json(predn, batch["im_file"][si])
@@ -264,38 +264,55 @@
         image_id = int(stem) if stem.isnumeric() else stem
         box = ops.xyxy2xywh(predn[:, :4])  # xywh
         box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
         for p, b in zip(predn.tolist(), box.tolist()):
             self.jdict.append(
                 {
                     "image_id": image_id,
-                    "category_id": self.class_map[int(p[5])],
+                    "category_id": self.class_map[int(p[5])]
+                    + (1 if self.is_lvis else 0),  # index starts from 1 if it's lvis
                     "bbox": [round(x, 3) for x in b],
                     "score": round(p[4], 5),
                 }
             )
 
     def eval_json(self, stats):
         """Evaluates YOLO output in JSON format and returns performance statistics."""
-        if self.args.save_json and self.is_coco and len(self.jdict):
-            anno_json = self.data["path"] / "annotations/instances_val2017.json"  # annotations
+        if self.args.save_json and (self.is_coco or self.is_lvis) and len(self.jdict):
             pred_json = self.save_dir / "predictions.json"  # predictions
-            LOGGER.info(f"\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...")
+            anno_json = (
+                self.data["path"]
+                / "annotations"
+                / ("instances_val2017.json" if self.is_coco else f"lvis_v1_{self.args.split}.json")
+            )  # annotations
+            pkg = "pycocotools" if self.is_coco else "lvis"
+            LOGGER.info(f"\nEvaluating {pkg} mAP using {pred_json} and {anno_json}...")
             try:  # https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocoEvalDemo.ipynb
-                check_requirements("pycocotools>=2.0.6")
-                from pycocotools.coco import COCO  # noqa
-                from pycocotools.cocoeval import COCOeval  # noqa
-
-                for x in anno_json, pred_json:
+                for x in pred_json, anno_json:
                     assert x.is_file(), f"{x} file not found"
-                anno = COCO(str(anno_json))  # init annotations api
-                pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
-                eval = COCOeval(anno, pred, "bbox")
+                check_requirements("pycocotools>=2.0.6" if self.is_coco else "lvis>=0.5.3")
                 if self.is_coco:
-                    eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
+                    from pycocotools.coco import COCO  # noqa
+                    from pycocotools.cocoeval import COCOeval  # noqa
+
+                    anno = COCO(str(anno_json))  # init annotations api
+                    pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
+                    eval = COCOeval(anno, pred, "bbox")
+                else:
+                    from lvis import LVIS, LVISEval
+
+                    anno = LVIS(str(anno_json))  # init annotations api
+                    pred = anno._load_json(str(pred_json))  # init predictions api (must pass string, not Path)
+                    eval = LVISEval(anno, pred, "bbox")
+                eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
                 eval.evaluate()
                 eval.accumulate()
                 eval.summarize()
-                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = eval.stats[:2]  # update mAP50-95 and mAP50
+                if self.is_lvis:
+                    eval.print_results()  # explicitly call print_results
+                # update mAP50-95 and mAP50
+                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = (
+                    eval.stats[:2] if self.is_coco else [eval.results["AP50"], eval.results["AP"]]
+                )
             except Exception as e:
-                LOGGER.warning(f"pycocotools unable to run: {e}")
+                LOGGER.warning(f"{pkg} unable to run: {e}")
         return stats
```

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.0/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.0/ultralytics/models/yolo/obb/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     A class extending the DetectionTrainer class for training based on an Oriented Bounding Box (OBB) model.
 
     Example:
         ```python
         from ultralytics.models.yolo.obb import OBBTrainer
 
-        args = dict(model='yolov8n-seg.pt', data='coco8-seg.yaml', epochs=3)
+        args = dict(model='yolov8n-obb.pt', data='dota8.yaml', epochs=3)
         trainer = OBBTrainer(overrides=args)
         trainer.train()
         ```
     """
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """Initialize a OBBTrainer object with given arguments."""
```

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.0/ultralytics/models/yolo/obb/val.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,19 @@
         )
 
     def _process_batch(self, detections, gt_bboxes, gt_cls):
         """
         Return correct prediction matrix.
 
         Args:
-            detections (torch.Tensor): Tensor of shape [N, 6] representing detections.
-                Each detection is of the format: x1, y1, x2, y2, conf, class.
-            labels (torch.Tensor): Tensor of shape [M, 5] representing labels.
-                Each label is of the format: class, x1, y1, x2, y2.
+            detections (torch.Tensor): Tensor of shape [N, 7] representing detections.
+                Each detection is of the format: x1, y1, x2, y2, conf, class, angle.
+            gt_bboxes (torch.Tensor): Tensor of shape [M, 5] representing rotated boxes.
+                Each box is of the format: x1, y1, x2, y2, angle.
+            labels (torch.Tensor): Tensor of shape [M] representing labels.
 
         Returns:
             (torch.Tensor): Correct prediction matrix of shape [N, 10] for 10 IoU levels.
         """
         iou = batch_probiou(gt_bboxes, torch.cat([detections[:, :4], detections[:, -1:]], dim=-1))
         return self.match_predictions(detections[:, 5], gt_cls, iou)
 
@@ -73,15 +74,15 @@
         bbox = batch["bboxes"][idx]
         ori_shape = batch["ori_shape"][si]
         imgsz = batch["img"].shape[2:]
         ratio_pad = batch["ratio_pad"][si]
         if len(cls):
             bbox[..., :4].mul_(torch.tensor(imgsz, device=self.device)[[1, 0, 1, 0]])  # target boxes
             ops.scale_boxes(imgsz, bbox, ori_shape, ratio_pad=ratio_pad, xywh=True)  # native-space labels
-        return dict(cls=cls, bbox=bbox, ori_shape=ori_shape, imgsz=imgsz, ratio_pad=ratio_pad)
+        return {"cls": cls, "bbox": bbox, "ori_shape": ori_shape, "imgsz": imgsz, "ratio_pad": ratio_pad}
 
     def _prepare_pred(self, pred, pbatch):
         """Prepares and returns a batch for OBB validation with scaled and padded bounding boxes."""
         predn = pred.clone()
         ops.scale_boxes(
             pbatch["imgsz"], predn[:, :4], pbatch["ori_shape"], ratio_pad=pbatch["ratio_pad"], xywh=True
         )  # native-space pred
```

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.0/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.0/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.0/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.0/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.0/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.0/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/nn/__init__.py` & `ultralytics-8.2.0/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/nn/autobackend.py` & `ultralytics-8.2.0/ultralytics/nn/autobackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import cv2
 import numpy as np
 import torch
 import torch.nn as nn
 from PIL import Image
 
-from ultralytics.utils import ARM64, LINUX, LOGGER, ROOT, yaml_load
+from ultralytics.utils import ARM64, IS_JETSON, IS_RASPBERRYPI, LINUX, LOGGER, ROOT, yaml_load
 from ultralytics.utils.checks import check_requirements, check_suffix, check_version, check_yaml
 from ultralytics.utils.downloads import attempt_download_asset, is_url
 
 
 def check_class_names(names):
     """
     Check class names.
@@ -68,40 +68,42 @@
             | CoreML                | *.mlpackage      |
             | TensorRT              | *.engine         |
             | TensorFlow SavedModel | *_saved_model    |
             | TensorFlow GraphDef   | *.pb             |
             | TensorFlow Lite       | *.tflite         |
             | TensorFlow Edge TPU   | *_edgetpu.tflite |
             | PaddlePaddle          | *_paddle_model   |
-            | ncnn                  | *_ncnn_model     |
+            | NCNN                  | *_ncnn_model     |
 
     This class offers dynamic backend switching capabilities based on the input model format, making it easier to deploy
     models across various platforms.
     """
 
     @torch.no_grad()
     def __init__(
         self,
         weights="yolov8n.pt",
         device=torch.device("cpu"),
         dnn=False,
         data=None,
         fp16=False,
+        batch=1,
         fuse=True,
         verbose=True,
     ):
         """
         Initialize the AutoBackend for inference.
 
         Args:
             weights (str): Path to the model weights file. Defaults to 'yolov8n.pt'.
             device (torch.device): Device to run the model on. Defaults to CPU.
             dnn (bool): Use OpenCV DNN module for ONNX inference. Defaults to False.
             data (str | Path | optional): Path to the additional data.yaml file containing class names. Optional.
             fp16 (bool): Enable half-precision inference. Supported only on specific backends. Defaults to False.
+            batch (int): Batch-size to assume for inference.
             fuse (bool): Fuse Conv2D + BatchNorm layers for optimization. Defaults to True.
             verbose (bool): Enable verbose logging. Defaults to True.
         """
         super().__init__()
         w = str(weights[0] if isinstance(weights, list) else weights)
         nn_module = isinstance(weights, torch.nn.Module)
         (
@@ -131,75 +133,97 @@
             device = torch.device("cpu")
             cuda = False
 
         # Download if not local
         if not (pt or triton or nn_module):
             w = attempt_download_asset(w)
 
-        # Load model
-        if nn_module:  # in-memory PyTorch model
+        # In-memory PyTorch model
+        if nn_module:
             model = weights.to(device)
-            model = model.fuse(verbose=verbose) if fuse else model
+            if fuse:
+                model = model.fuse(verbose=verbose)
             if hasattr(model, "kpt_shape"):
                 kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
             names = model.module.names if hasattr(model, "module") else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
             pt = True
-        elif pt:  # PyTorch
+
+        # PyTorch
+        elif pt:
             from ultralytics.nn.tasks import attempt_load_weights
 
             model = attempt_load_weights(
                 weights if isinstance(weights, list) else w, device=device, inplace=True, fuse=fuse
             )
             if hasattr(model, "kpt_shape"):
                 kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
             names = model.module.names if hasattr(model, "module") else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
-        elif jit:  # TorchScript
+
+        # TorchScript
+        elif jit:
             LOGGER.info(f"Loading {w} for TorchScript inference...")
             extra_files = {"config.txt": ""}  # model metadata
             model = torch.jit.load(w, _extra_files=extra_files, map_location=device)
             model.half() if fp16 else model.float()
             if extra_files["config.txt"]:  # load metadata dict
                 metadata = json.loads(extra_files["config.txt"], object_hook=lambda x: dict(x.items()))
-        elif dnn:  # ONNX OpenCV DNN
+
+        # ONNX OpenCV DNN
+        elif dnn:
             LOGGER.info(f"Loading {w} for ONNX OpenCV DNN inference...")
             check_requirements("opencv-python>=4.5.4")
             net = cv2.dnn.readNetFromONNX(w)
-        elif onnx:  # ONNX Runtime
+
+        # ONNX Runtime
+        elif onnx:
             LOGGER.info(f"Loading {w} for ONNX Runtime inference...")
             check_requirements(("onnx", "onnxruntime-gpu" if cuda else "onnxruntime"))
+            if IS_RASPBERRYPI or IS_JETSON:
+                # Fix error: module 'numpy.linalg._umath_linalg' has no attribute '_ilp64' when exporting to Tensorflow SavedModel on RPi and Jetson
+                check_requirements("numpy==1.23.5")
             import onnxruntime
 
             providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if cuda else ["CPUExecutionProvider"]
             session = onnxruntime.InferenceSession(w, providers=providers)
             output_names = [x.name for x in session.get_outputs()]
-            metadata = session.get_modelmeta().custom_metadata_map  # metadata
-        elif xml:  # OpenVINO
+            metadata = session.get_modelmeta().custom_metadata_map
+
+        # OpenVINO
+        elif xml:
             LOGGER.info(f"Loading {w} for OpenVINO inference...")
-            check_requirements("openvino>=2023.0")  # requires openvino-dev: https://pypi.org/project/openvino-dev/
-            from openvino.runtime import Core, Layout, get_batch  # noqa
+            check_requirements("openvino>=2024.0.0")
+            import openvino as ov
 
-            core = Core()
+            core = ov.Core()
             w = Path(w)
             if not w.is_file():  # if not *.xml
                 w = next(w.glob("*.xml"))  # get *.xml file from *_openvino_model dir
             ov_model = core.read_model(model=str(w), weights=w.with_suffix(".bin"))
             if ov_model.get_parameters()[0].get_layout().empty:
-                ov_model.get_parameters()[0].set_layout(Layout("NCHW"))
-            batch_dim = get_batch(ov_model)
-            if batch_dim.is_static:
-                batch_size = batch_dim.get_length()
-            ov_compiled_model = core.compile_model(ov_model, device_name="AUTO")  # AUTO selects best available device
+                ov_model.get_parameters()[0].set_layout(ov.Layout("NCHW"))
+
+            # OpenVINO inference modes are 'LATENCY', 'THROUGHPUT' (not recommended), or 'CUMULATIVE_THROUGHPUT'
+            inference_mode = "CUMULATIVE_THROUGHPUT" if batch > 1 else "LATENCY"
+            LOGGER.info(f"Using OpenVINO {inference_mode} mode for batch={batch} inference...")
+            ov_compiled_model = core.compile_model(
+                ov_model,
+                device_name="AUTO",  # AUTO selects best available device, do not modify
+                config={"PERFORMANCE_HINT": inference_mode},
+            )
+            input_name = ov_compiled_model.input().get_any_name()
             metadata = w.parent / "metadata.yaml"
-        elif engine:  # TensorRT
+
+        # TensorRT
+        elif engine:
             LOGGER.info(f"Loading {w} for TensorRT inference...")
             try:
                 import tensorrt as trt  # noqa https://developer.nvidia.com/nvidia-tensorrt-download
             except ImportError:
                 if LINUX:
                     check_requirements("nvidia-tensorrt", cmds="-U --index-url https://pypi.ngc.nvidia.com")
                 import tensorrt as trt  # noqa
@@ -209,49 +233,79 @@
             Binding = namedtuple("Binding", ("name", "dtype", "shape", "data", "ptr"))
             logger = trt.Logger(trt.Logger.INFO)
             # Read file
             with open(w, "rb") as f, trt.Runtime(logger) as runtime:
                 meta_len = int.from_bytes(f.read(4), byteorder="little")  # read metadata length
                 metadata = json.loads(f.read(meta_len).decode("utf-8"))  # read metadata
                 model = runtime.deserialize_cuda_engine(f.read())  # read engine
-            context = model.create_execution_context()
+
+            # Model context
+            try:
+                context = model.create_execution_context()
+            except Exception as e:  # model is None
+                LOGGER.error(f"ERROR: TensorRT model exported with a different version than {trt.__version__}\n")
+                raise e
+
             bindings = OrderedDict()
             output_names = []
             fp16 = False  # default updated below
             dynamic = False
-            for i in range(model.num_bindings):
-                name = model.get_binding_name(i)
-                dtype = trt.nptype(model.get_binding_dtype(i))
-                if model.binding_is_input(i):
-                    if -1 in tuple(model.get_binding_shape(i)):  # dynamic
-                        dynamic = True
-                        context.set_binding_shape(i, tuple(model.get_profile_shape(0, i)[2]))
-                    if dtype == np.float16:
-                        fp16 = True
-                else:  # output
-                    output_names.append(name)
-                shape = tuple(context.get_binding_shape(i))
+            is_trt10 = not hasattr(model, "num_bindings")
+            num = range(model.num_io_tensors) if is_trt10 else range(model.num_bindings)
+            for i in num:
+                if is_trt10:
+                    name = model.get_tensor_name(i)
+                    dtype = trt.nptype(model.get_tensor_dtype(name))
+                    is_input = model.get_tensor_mode(name) == trt.TensorIOMode.INPUT
+                    if is_input:
+                        if -1 in tuple(model.get_tensor_shape(name)):
+                            dynamic = True
+                            context.set_input_shape(name, tuple(model.get_tensor_profile_shape(name, 0)[1]))
+                            if dtype == np.float16:
+                                fp16 = True
+                    else:
+                        output_names.append(name)
+                    shape = tuple(context.get_tensor_shape(name))
+                else:  # TensorRT < 10.0
+                    name = model.get_binding_name(i)
+                    dtype = trt.nptype(model.get_binding_dtype(i))
+                    is_input = model.binding_is_input(i)
+                    if model.binding_is_input(i):
+                        if -1 in tuple(model.get_binding_shape(i)):  # dynamic
+                            dynamic = True
+                            context.set_binding_shape(i, tuple(model.get_profile_shape(0, i)[1]))
+                        if dtype == np.float16:
+                            fp16 = True
+                    else:
+                        output_names.append(name)
+                    shape = tuple(context.get_binding_shape(i))
                 im = torch.from_numpy(np.empty(shape, dtype=dtype)).to(device)
                 bindings[name] = Binding(name, dtype, shape, im, int(im.data_ptr()))
             binding_addrs = OrderedDict((n, d.ptr) for n, d in bindings.items())
             batch_size = bindings["images"].shape[0]  # if dynamic, this is instead max batch size
-        elif coreml:  # CoreML
+
+        # CoreML
+        elif coreml:
             LOGGER.info(f"Loading {w} for CoreML inference...")
             import coremltools as ct
 
             model = ct.models.MLModel(w)
             metadata = dict(model.user_defined_metadata)
-        elif saved_model:  # TF SavedModel
+
+        # TF SavedModel
+        elif saved_model:
             LOGGER.info(f"Loading {w} for TensorFlow SavedModel inference...")
             import tensorflow as tf
 
             keras = False  # assume TF1 saved_model
             model = tf.keras.models.load_model(w) if keras else tf.saved_model.load(w)
             metadata = Path(w) / "metadata.yaml"
-        elif pb:  # GraphDef https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
+
+        # TF GraphDef
+        elif pb:  # https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
             LOGGER.info(f"Loading {w} for TensorFlow GraphDef inference...")
             import tensorflow as tf
 
             from ultralytics.engine.exporter import gd_outputs
 
             def wrap_frozen_graph(gd, inputs, outputs):
                 """Wrap frozen graphs for deployment."""
@@ -259,14 +313,16 @@
                 ge = x.graph.as_graph_element
                 return x.prune(tf.nest.map_structure(ge, inputs), tf.nest.map_structure(ge, outputs))
 
             gd = tf.Graph().as_graph_def()  # TF GraphDef
             with open(w, "rb") as f:
                 gd.ParseFromString(f.read())
             frozen_func = wrap_frozen_graph(gd, inputs="x:0", outputs=gd_outputs(gd))
+
+        # TFLite or TFLite Edge TPU
         elif tflite or edgetpu:  # https://www.tensorflow.org/lite/guide/python#install_tensorflow_lite_for_python
             try:  # https://coral.ai/docs/edgetpu/tflite-python/#update-existing-tf-lite-code-for-the-edge-tpu
                 from tflite_runtime.interpreter import Interpreter, load_delegate
             except ImportError:
                 import tensorflow as tf
 
                 Interpreter, load_delegate = tf.lite.Interpreter, tf.lite.experimental.load_delegate
@@ -283,66 +339,75 @@
             input_details = interpreter.get_input_details()  # inputs
             output_details = interpreter.get_output_details()  # outputs
             # Load metadata
             with contextlib.suppress(zipfile.BadZipFile):
                 with zipfile.ZipFile(w, "r") as model:
                     meta_file = model.namelist()[0]
                     metadata = ast.literal_eval(model.read(meta_file).decode("utf-8"))
-        elif tfjs:  # TF.js
+
+        # TF.js
+        elif tfjs:
             raise NotImplementedError("YOLOv8 TF.js inference is not currently supported.")
-        elif paddle:  # PaddlePaddle
+
+        # PaddlePaddle
+        elif paddle:
             LOGGER.info(f"Loading {w} for PaddlePaddle inference...")
             check_requirements("paddlepaddle-gpu" if cuda else "paddlepaddle")
             import paddle.inference as pdi  # noqa
 
             w = Path(w)
             if not w.is_file():  # if not *.pdmodel
                 w = next(w.rglob("*.pdmodel"))  # get *.pdmodel file from *_paddle_model dir
             config = pdi.Config(str(w), str(w.with_suffix(".pdiparams")))
             if cuda:
                 config.enable_use_gpu(memory_pool_init_size_mb=2048, device_id=0)
             predictor = pdi.create_predictor(config)
             input_handle = predictor.get_input_handle(predictor.get_input_names()[0])
             output_names = predictor.get_output_names()
             metadata = w.parents[1] / "metadata.yaml"
-        elif ncnn:  # ncnn
-            LOGGER.info(f"Loading {w} for ncnn inference...")
-            check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires ncnn
+
+        # NCNN
+        elif ncnn:
+            LOGGER.info(f"Loading {w} for NCNN inference...")
+            check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires NCNN
             import ncnn as pyncnn
 
             net = pyncnn.Net()
             net.opt.use_vulkan_compute = cuda
             w = Path(w)
             if not w.is_file():  # if not *.param
                 w = next(w.glob("*.param"))  # get *.param file from *_ncnn_model dir
             net.load_param(str(w))
             net.load_model(str(w.with_suffix(".bin")))
             metadata = w.parent / "metadata.yaml"
-        elif triton:  # NVIDIA Triton Inference Server
+
+        # NVIDIA Triton Inference Server
+        elif triton:
             check_requirements("tritonclient[all]")
             from ultralytics.utils.triton import TritonRemoteModel
 
             model = TritonRemoteModel(w)
+
+        # Any other format (unsupported)
         else:
             from ultralytics.engine.exporter import export_formats
 
             raise TypeError(
                 f"model='{w}' is not a supported model format. "
-                "See https://docs.ultralytics.com/modes/predict for help."
-                f"\n\n{export_formats()}"
+                f"See https://docs.ultralytics.com/modes/predict for help.\n\n{export_formats()}"
             )
 
         # Load external metadata YAML
         if isinstance(metadata, (str, Path)) and Path(metadata).exists():
             metadata = yaml_load(metadata)
         if metadata:
             for k, v in metadata.items():
-                if k in ("stride", "batch"):
+                if k in {"stride", "batch"}:
                     metadata[k] = int(v)
-                elif k in ("imgsz", "names", "kpt_shape") and isinstance(v, str):
+                elif k in {"imgsz", "names", "kpt_shape"} and isinstance(v, str):
                     metadata[k] = eval(v)
             stride = metadata["stride"]
             task = metadata["task"]
             batch = metadata["batch"]
             imgsz = metadata["imgsz"]
             names = metadata["names"]
             kpt_shape = metadata.get("kpt_shape")
@@ -376,42 +441,81 @@
         """
         b, ch, h, w = im.shape  # batch, channel, height, width
         if self.fp16 and im.dtype != torch.float16:
             im = im.half()  # to FP16
         if self.nhwc:
             im = im.permute(0, 2, 3, 1)  # torch BCHW to numpy BHWC shape(1,320,192,3)
 
-        if self.pt or self.nn_module:  # PyTorch
+        # PyTorch
+        if self.pt or self.nn_module:
             y = self.model(im, augment=augment, visualize=visualize, embed=embed)
-        elif self.jit:  # TorchScript
+
+        # TorchScript
+        elif self.jit:
             y = self.model(im)
-        elif self.dnn:  # ONNX OpenCV DNN
+
+        # ONNX OpenCV DNN
+        elif self.dnn:
             im = im.cpu().numpy()  # torch to numpy
             self.net.setInput(im)
             y = self.net.forward()
-        elif self.onnx:  # ONNX Runtime
+
+        # ONNX Runtime
+        elif self.onnx:
             im = im.cpu().numpy()  # torch to numpy
             y = self.session.run(self.output_names, {self.session.get_inputs()[0].name: im})
-        elif self.xml:  # OpenVINO
+
+        # OpenVINO
+        elif self.xml:
             im = im.cpu().numpy()  # FP32
-            y = list(self.ov_compiled_model(im).values())
-        elif self.engine:  # TensorRT
-            if self.dynamic and im.shape != self.bindings["images"].shape:
-                i = self.model.get_binding_index("images")
-                self.context.set_binding_shape(i, im.shape)  # reshape if dynamic
-                self.bindings["images"] = self.bindings["images"]._replace(shape=im.shape)
-                for name in self.output_names:
-                    i = self.model.get_binding_index(name)
-                    self.bindings[name].data.resize_(tuple(self.context.get_binding_shape(i)))
+
+            if self.inference_mode in {"THROUGHPUT", "CUMULATIVE_THROUGHPUT"}:  # optimized for larger batch-sizes
+                n = im.shape[0]  # number of images in batch
+                results = [None] * n  # preallocate list with None to match the number of images
+
+                def callback(request, userdata):
+                    """Places result in preallocated list using userdata index."""
+                    results[userdata] = request.results
+
+                # Create AsyncInferQueue, set the callback and start asynchronous inference for each input image
+                async_queue = self.ov.runtime.AsyncInferQueue(self.ov_compiled_model)
+                async_queue.set_callback(callback)
+                for i in range(n):
+                    # Start async inference with userdata=i to specify the position in results list
+                    async_queue.start_async(inputs={self.input_name: im[i : i + 1]}, userdata=i)  # keep image as BCHW
+                async_queue.wait_all()  # wait for all inference requests to complete
+                y = np.concatenate([list(r.values())[0] for r in results])
+
+            else:  # inference_mode = "LATENCY", optimized for fastest first result at batch-size 1
+                y = list(self.ov_compiled_model(im).values())
+
+        # TensorRT
+        elif self.engine:
+            if self.dynamic or im.shape != self.bindings["images"].shape:
+                if self.is_trt10:
+                    self.context.set_input_shape("images", im.shape)
+                    self.bindings["images"] = self.bindings["images"]._replace(shape=im.shape)
+                    for name in self.output_names:
+                        self.bindings[name].data.resize_(tuple(self.context.get_tensor_shape(name)))
+                else:
+                    i = self.model.get_binding_index("images")
+                    self.context.set_binding_shape(i, im.shape)
+                    self.bindings["images"] = self.bindings["images"]._replace(shape=im.shape)
+                    for name in self.output_names:
+                        i = self.model.get_binding_index(name)
+                        self.bindings[name].data.resize_(tuple(self.context.get_binding_shape(i)))
+
             s = self.bindings["images"].shape
             assert im.shape == s, f"input size {im.shape} {'>' if self.dynamic else 'not equal to'} max model size {s}"
             self.binding_addrs["images"] = int(im.data_ptr())
             self.context.execute_v2(list(self.binding_addrs.values()))
             y = [self.bindings[x].data for x in sorted(self.output_names)]
-        elif self.coreml:  # CoreML
+
+        # CoreML
+        elif self.coreml:
             im = im[0].cpu().numpy()
             im_pil = Image.fromarray((im * 255).astype("uint8"))
             # im = im.resize((192, 320), Image.BILINEAR)
             y = self.model.predict({"image": im_pil})  # coordinates are xywh normalized
             if "confidence" in y:
                 raise TypeError(
                     "Ultralytics only supports inference of non-pipelined CoreML models exported with "
@@ -422,59 +526,63 @@
                 # box = xywh2xyxy(y['coordinates'] * [[w, h, w, h]])  # xyxy pixels
                 # conf, cls = y['confidence'].max(1), y['confidence'].argmax(1).astype(np.float32)
                 # y = np.concatenate((box, conf.reshape(-1, 1), cls.reshape(-1, 1)), 1)
             elif len(y) == 1:  # classification model
                 y = list(y.values())
             elif len(y) == 2:  # segmentation model
                 y = list(reversed(y.values()))  # reversed for segmentation models (pred, proto)
-        elif self.paddle:  # PaddlePaddle
+
+        # PaddlePaddle
+        elif self.paddle:
             im = im.cpu().numpy().astype(np.float32)
             self.input_handle.copy_from_cpu(im)
             self.predictor.run()
             y = [self.predictor.get_output_handle(x).copy_to_cpu() for x in self.output_names]
-        elif self.ncnn:  # ncnn
+
+        # NCNN
+        elif self.ncnn:
             mat_in = self.pyncnn.Mat(im[0].cpu().numpy())
-            ex = self.net.create_extractor()
-            input_names, output_names = self.net.input_names(), self.net.output_names()
-            ex.input(input_names[0], mat_in)
-            y = []
-            for output_name in output_names:
-                mat_out = self.pyncnn.Mat()
-                ex.extract(output_name, mat_out)
-                y.append(np.array(mat_out)[None])
-        elif self.triton:  # NVIDIA Triton Inference Server
+            with self.net.create_extractor() as ex:
+                ex.input(self.net.input_names()[0], mat_in)
+                # WARNING: 'output_names' sorted as a temporary fix for https://github.com/pnnx/pnnx/issues/130
+                y = [np.array(ex.extract(x)[1])[None] for x in sorted(self.net.output_names())]
+
+        # NVIDIA Triton Inference Server
+        elif self.triton:
             im = im.cpu().numpy()  # torch to numpy
             y = self.model(im)
-        else:  # TensorFlow (SavedModel, GraphDef, Lite, Edge TPU)
+
+        # TensorFlow (SavedModel, GraphDef, Lite, Edge TPU)
+        else:
             im = im.cpu().numpy()
             if self.saved_model:  # SavedModel
                 y = self.model(im, training=False) if self.keras else self.model(im)
                 if not isinstance(y, list):
                     y = [y]
             elif self.pb:  # GraphDef
                 y = self.frozen_func(x=self.tf.constant(im))
                 if len(y) == 2 and len(self.names) == 999:  # segments and names not defined
                     ip, ib = (0, 1) if len(y[0].shape) == 4 else (1, 0)  # index of protos, boxes
                     nc = y[ib].shape[1] - y[ip].shape[3] - 4  # y = (1, 160, 160, 32), (1, 116, 8400)
                     self.names = {i: f"class{i}" for i in range(nc)}
             else:  # Lite or Edge TPU
                 details = self.input_details[0]
-                integer = details["dtype"] in (np.int8, np.int16)  # is TFLite quantized int8 or int16 model
-                if integer:
+                is_int = details["dtype"] in {np.int8, np.int16}  # is TFLite quantized int8 or int16 model
+                if is_int:
                     scale, zero_point = details["quantization"]
                     im = (im / scale + zero_point).astype(details["dtype"])  # de-scale
                 self.interpreter.set_tensor(details["index"], im)
                 self.interpreter.invoke()
                 y = []
                 for output in self.output_details:
                     x = self.interpreter.get_tensor(output["index"])
-                    if integer:
+                    if is_int:
                         scale, zero_point = output["quantization"]
                         x = (x.astype(np.float32) - zero_point) * scale  # re-scale
-                    if x.ndim > 2:  # if task is not classification
+                    if x.ndim == 3:  # if task is not classification, excluding masks (ndim=4) as well
                         # Denormalize xywh by image size. See https://github.com/ultralytics/ultralytics/pull/1695
                         # xywh are normalized in TFLite/EdgeTPU to mitigate quantization error of integer models
                         x[:, [0, 2]] *= w
                         x[:, [1, 3]] *= h
                     y.append(x)
             # TF segment fixes: export is reversed vs ONNX export and protos are transposed
             if len(y) == 2:  # segment with (det, proto) output order reversed
@@ -527,22 +635,22 @@
         Examples:
             >>> model = AutoBackend(weights="path/to/model.onnx")
             >>> model_type = model._model_type()  # returns "onnx"
         """
         from ultralytics.engine.exporter import export_formats
 
         sf = list(export_formats().Suffix)  # export suffixes
-        if not is_url(p, check=False) and not isinstance(p, str):
+        if not is_url(p) and not isinstance(p, str):
             check_suffix(p, sf)  # checks
         name = Path(p).name
         types = [s in name for s in sf]
         types[5] |= name.endswith(".mlmodel")  # retain support for older Apple CoreML *.mlmodel formats
         types[8] &= not types[9]  # tflite &= not edgetpu
         if any(types):
             triton = False
         else:
             from urllib.parse import urlsplit
 
             url = urlsplit(p)
-            triton = url.netloc and url.path and url.scheme in {"http", "grpc"}
+            triton = bool(url.netloc) and bool(url.path) and url.scheme in {"http", "grpc"}
 
         return types + [triton]
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.0/ultralytics/nn/modules/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,26 +20,36 @@
 from .block import (
     C1,
     C2,
     C3,
     C3TR,
     DFL,
     SPP,
+    SPPELAN,
     SPPF,
+    ADown,
+    BNContrastiveHead,
     Bottleneck,
     BottleneckCSP,
     C2f,
+    C2fAttn,
     C3Ghost,
     C3x,
+    CBFuse,
+    CBLinear,
+    ContrastiveHead,
     GhostBottleneck,
     HGBlock,
     HGStem,
+    ImagePoolingAttn,
     Proto,
     RepC3,
+    RepNCSPELAN4,
     ResNetLayer,
+    Silence,
 )
 from .conv import (
     CBAM,
     ChannelAttention,
     Concat,
     Conv,
     Conv2,
@@ -48,15 +58,15 @@
     DWConvTranspose2d,
     Focus,
     GhostConv,
     LightConv,
     RepConv,
     SpatialAttention,
 )
-from .head import OBB, Classify, Detect, Pose, RTDETRDecoder, Segment
+from .head import OBB, Classify, Detect, Pose, RTDETRDecoder, Segment, WorldDetect
 from .transformer import (
     AIFI,
     MLP,
     DeformableTransformerDecoder,
     DeformableTransformerDecoderLayer,
     LayerNorm2d,
     MLPBlock,
@@ -89,14 +99,15 @@
     "HGStem",
     "SPP",
     "SPPF",
     "C1",
     "C2",
     "C3",
     "C2f",
+    "C2fAttn",
     "C3x",
     "C3TR",
     "C3Ghost",
     "GhostBottleneck",
     "Bottleneck",
     "BottleneckCSP",
     "Proto",
@@ -110,8 +121,18 @@
     "AIFI",
     "DeformableTransformerDecoder",
     "DeformableTransformerDecoderLayer",
     "MSDeformAttn",
     "MLP",
     "ResNetLayer",
     "OBB",
+    "WorldDetect",
+    "ImagePoolingAttn",
+    "ContrastiveHead",
+    "BNContrastiveHead",
+    "RepNCSPELAN4",
+    "ADown",
+    "SPPELAN",
+    "CBFuse",
+    "CBLinear",
+    "Silence",
 )
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.0/ultralytics/nn/modules/conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
 class SpatialAttention(nn.Module):
     """Spatial-attention module."""
 
     def __init__(self, kernel_size=7):
         """Initialize Spatial-attention module with kernel size argument."""
         super().__init__()
-        assert kernel_size in (3, 7), "kernel size must be 3 or 7"
+        assert kernel_size in {3, 7}, "kernel size must be 3 or 7"
         padding = 3 if kernel_size == 7 else 1
         self.cv1 = nn.Conv2d(2, 1, kernel_size, padding=padding, bias=False)
         self.act = nn.Sigmoid()
 
     def forward(self, x):
         """Apply channel and spatial attention on input for feature recalibration."""
         return x * self.act(self.cv1(torch.cat([torch.mean(x, 1, keepdim=True), torch.max(x, 1, keepdim=True)[0]], 1)))
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/modules/head.py` & `ultralytics-8.2.0/ultralytics/nn/modules/head.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import math
 
 import torch
 import torch.nn as nn
 from torch.nn.init import constant_, xavier_uniform_
 
 from ultralytics.utils.tal import TORCH_1_10, dist2bbox, dist2rbox, make_anchors
-from .block import DFL, Proto
+
+from .block import DFL, BNContrastiveHead, ContrastiveHead, Proto
 from .conv import Conv
 from .transformer import MLP, DeformableTransformerDecoder, DeformableTransformerDecoderLayer
 from .utils import bias_init_with_prob, linear_init
 
 __all__ = "Detect", "Segment", "Pose", "Classify", "OBB", "RTDETRDecoder"
 
 
@@ -50,45 +51,46 @@
         # Inference path
         shape = x[0].shape  # BCHW
         x_cat = torch.cat([xi.view(shape[0], self.no, -1) for xi in x], 2)
         if self.dynamic or self.shape != shape:
             self.anchors, self.strides = (x.transpose(0, 1) for x in make_anchors(x, self.stride, 0.5))
             self.shape = shape
 
-        if self.export and self.format in ("saved_model", "pb", "tflite", "edgetpu", "tfjs"):  # avoid TF FlexSplitV ops
+        if self.export and self.format in {"saved_model", "pb", "tflite", "edgetpu", "tfjs"}:  # avoid TF FlexSplitV ops
             box = x_cat[:, : self.reg_max * 4]
             cls = x_cat[:, self.reg_max * 4 :]
         else:
             box, cls = x_cat.split((self.reg_max * 4, self.nc), 1)
-        dbox = self.decode_bboxes(box)
 
-        if self.export and self.format in ("tflite", "edgetpu"):
+        if self.export and self.format in {"tflite", "edgetpu"}:
             # Precompute normalization factor to increase numerical stability
             # See https://github.com/ultralytics/ultralytics/issues/7371
-            img_h = shape[2]
-            img_w = shape[3]
-            img_size = torch.tensor([img_w, img_h, img_w, img_h], device=box.device).reshape(1, 4, 1)
-            norm = self.strides / (self.stride[0] * img_size)
-            dbox = dist2bbox(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2], xywh=True, dim=1)
+            grid_h = shape[2]
+            grid_w = shape[3]
+            grid_size = torch.tensor([grid_w, grid_h, grid_w, grid_h], device=box.device).reshape(1, 4, 1)
+            norm = self.strides / (self.stride[0] * grid_size)
+            dbox = self.decode_bboxes(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2])
+        else:
+            dbox = self.decode_bboxes(self.dfl(box), self.anchors.unsqueeze(0)) * self.strides
 
         y = torch.cat((dbox, cls.sigmoid()), 1)
         return y if self.export else (y, x)
 
     def bias_init(self):
         """Initialize Detect() biases, WARNING: requires stride availability."""
         m = self  # self.model[-1]  # Detect() module
         # cf = torch.bincount(torch.tensor(np.concatenate(dataset.labels, 0)[:, 0]).long(), minlength=nc) + 1
         # ncf = math.log(0.6 / (m.nc - 0.999999)) if cf is None else torch.log(cf / cf.sum())  # nominal class frequency
         for a, b, s in zip(m.cv2, m.cv3, m.stride):  # from
             a[-1].bias.data[:] = 1.0  # box
             b[-1].bias.data[: m.nc] = math.log(5 / m.nc / (640 / s) ** 2)  # cls (.01 objects, 80 classes, 640 img)
 
-    def decode_bboxes(self, bboxes):
+    def decode_bboxes(self, bboxes, anchors):
         """Decode bounding boxes."""
-        return dist2bbox(self.dfl(bboxes), self.anchors.unsqueeze(0), xywh=True, dim=1) * self.strides
+        return dist2bbox(bboxes, anchors, xywh=True, dim=1)
 
 
 class Segment(Detect):
     """YOLOv8 Segment head for segmentation models."""
 
     def __init__(self, nc=80, nm=32, npr=256, ch=()):
         """Initialize the YOLO model attributes such as the number of masks, prototypes, and the convolution layers."""
@@ -135,17 +137,17 @@
         if not self.training:
             self.angle = angle
         x = self.detect(self, x)
         if self.training:
             return x, angle
         return torch.cat([x, angle], 1) if self.export else (torch.cat([x[0], angle], 1), (x[1], angle))
 
-    def decode_bboxes(self, bboxes):
+    def decode_bboxes(self, bboxes, anchors):
         """Decode rotated bounding boxes."""
-        return dist2rbox(self.dfl(bboxes), self.angle, self.anchors.unsqueeze(0), dim=1) * self.strides
+        return dist2rbox(bboxes, self.angle, anchors, dim=1)
 
 
 class Pose(Detect):
     """YOLOv8 Pose head for keypoints models."""
 
     def __init__(self, nc=80, kpt_shape=(17, 3), ch=()):
         """Initialize YOLO network with default parameters and Convolutional Layers."""
@@ -203,14 +205,66 @@
         """Performs a forward pass of the YOLO model on input image data."""
         if isinstance(x, list):
             x = torch.cat(x, 1)
         x = self.linear(self.drop(self.pool(self.conv(x)).flatten(1)))
         return x if self.training else x.softmax(1)
 
 
+class WorldDetect(Detect):
+    def __init__(self, nc=80, embed=512, with_bn=False, ch=()):
+        """Initialize YOLOv8 detection layer with nc classes and layer channels ch."""
+        super().__init__(nc, ch)
+        c3 = max(ch[0], min(self.nc, 100))
+        self.cv3 = nn.ModuleList(nn.Sequential(Conv(x, c3, 3), Conv(c3, c3, 3), nn.Conv2d(c3, embed, 1)) for x in ch)
+        self.cv4 = nn.ModuleList(BNContrastiveHead(embed) if with_bn else ContrastiveHead() for _ in ch)
+
+    def forward(self, x, text):
+        """Concatenates and returns predicted bounding boxes and class probabilities."""
+        for i in range(self.nl):
+            x[i] = torch.cat((self.cv2[i](x[i]), self.cv4[i](self.cv3[i](x[i]), text)), 1)
+        if self.training:
+            return x
+
+        # Inference path
+        shape = x[0].shape  # BCHW
+        x_cat = torch.cat([xi.view(shape[0], self.nc + self.reg_max * 4, -1) for xi in x], 2)
+        if self.dynamic or self.shape != shape:
+            self.anchors, self.strides = (x.transpose(0, 1) for x in make_anchors(x, self.stride, 0.5))
+            self.shape = shape
+
+        if self.export and self.format in {"saved_model", "pb", "tflite", "edgetpu", "tfjs"}:  # avoid TF FlexSplitV ops
+            box = x_cat[:, : self.reg_max * 4]
+            cls = x_cat[:, self.reg_max * 4 :]
+        else:
+            box, cls = x_cat.split((self.reg_max * 4, self.nc), 1)
+
+        if self.export and self.format in {"tflite", "edgetpu"}:
+            # Precompute normalization factor to increase numerical stability
+            # See https://github.com/ultralytics/ultralytics/issues/7371
+            grid_h = shape[2]
+            grid_w = shape[3]
+            grid_size = torch.tensor([grid_w, grid_h, grid_w, grid_h], device=box.device).reshape(1, 4, 1)
+            norm = self.strides / (self.stride[0] * grid_size)
+            dbox = self.decode_bboxes(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2])
+        else:
+            dbox = self.decode_bboxes(self.dfl(box), self.anchors.unsqueeze(0)) * self.strides
+
+        y = torch.cat((dbox, cls.sigmoid()), 1)
+        return y if self.export else (y, x)
+
+    def bias_init(self):
+        """Initialize Detect() biases, WARNING: requires stride availability."""
+        m = self  # self.model[-1]  # Detect() module
+        # cf = torch.bincount(torch.tensor(np.concatenate(dataset.labels, 0)[:, 0]).long(), minlength=nc) + 1
+        # ncf = math.log(0.6 / (m.nc - 0.999999)) if cf is None else torch.log(cf / cf.sum())  # nominal class frequency
+        for a, b, s in zip(m.cv2, m.cv3, m.stride):  # from
+            a[-1].bias.data[:] = 1.0  # box
+            # b[-1].bias.data[:] = math.log(5 / m.nc / (640 / s) ** 2)  # cls (.01 objects, 80 classes, 640 img)
+
+
 class RTDETRDecoder(nn.Module):
     """
     Real-Time Deformable Transformer Decoder (RTDETRDecoder) module for object detection.
 
     This decoder module utilizes Transformer architecture along with deformable convolutions to predict bounding boxes
     and class labels for objects in an image. It integrates features from multiple layers and runs through a series of
     Transformer decoder layers to output the final predictions.
@@ -347,15 +401,15 @@
 
             valid_WH = torch.tensor([w, h], dtype=dtype, device=device)
             grid_xy = (grid_xy.unsqueeze(0) + 0.5) / valid_WH  # (1, h, w, 2)
             wh = torch.ones_like(grid_xy, dtype=dtype, device=device) * grid_size * (2.0**i)
             anchors.append(torch.cat([grid_xy, wh], -1).view(-1, h * w, 4))  # (1, h*w, 4)
 
         anchors = torch.cat(anchors, 1)  # (1, h*w*nl, 4)
-        valid_mask = ((anchors > eps) * (anchors < 1 - eps)).all(-1, keepdim=True)  # 1, h*w*nl, 1
+        valid_mask = ((anchors > eps) & (anchors < 1 - eps)).all(-1, keepdim=True)  # 1, h*w*nl, 1
         anchors = torch.log(anchors / (1 - anchors))
         anchors = anchors.masked_fill(~valid_mask, float("inf"))
         return anchors, valid_mask
 
     def _get_encoder_input(self, x):
         """Processes and returns encoder inputs by getting projection features from input and concatenating them."""
         # Get projection features
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.0/ultralytics/nn/modules/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         s = (x - u).pow(2).mean(1, keepdim=True)
         x = (x - u) / torch.sqrt(s + self.eps)
         return self.weight[:, None, None] * x + self.bias[:, None, None]
 
 
 class MSDeformAttn(nn.Module):
     """
-    Multi-Scale Deformable Attention Module based on Deformable-DETR and PaddleDetection implementations.
+    Multiscale Deformable Attention Module based on Deformable-DETR and PaddleDetection implementations.
 
     https://github.com/fundamentalvision/Deformable-DETR/blob/main/models/ops/modules/ms_deform_attn.py
     """
 
     def __init__(self, d_model=256, n_levels=4, n_heads=8, n_points=4):
         """Initialize MSDeformAttn with the given parameters."""
         super().__init__()
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.0/ultralytics/nn/modules/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def multi_scale_deformable_attn_pytorch(
     value: torch.Tensor,
     value_spatial_shapes: torch.Tensor,
     sampling_locations: torch.Tensor,
     attention_weights: torch.Tensor,
 ) -> torch.Tensor:
     """
-    Multi-scale deformable attention.
+    Multiscale deformable attention.
 
     https://github.com/IDEA-Research/detrex/blob/main/detrex/layers/multi_scale_deform_attn.py
     """
 
     bs, _, num_heads, embed_dims = value.shape
     _, num_queries, num_heads, num_levels, num_points, _ = sampling_locations.shape
     value_list = value.split([H_ * W_ for H_, W_ in value_spatial_shapes], dim=1)
```

### Comparing `ultralytics-8.1.9/ultralytics/nn/tasks.py` & `ultralytics-8.2.0/ultralytics/nn/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,48 @@
     AIFI,
     C1,
     C2,
     C3,
     C3TR,
     OBB,
     SPP,
+    SPPELAN,
     SPPF,
+    ADown,
     Bottleneck,
     BottleneckCSP,
     C2f,
+    C2fAttn,
     C3Ghost,
     C3x,
+    CBFuse,
+    CBLinear,
     Classify,
     Concat,
     Conv,
     Conv2,
     ConvTranspose,
     Detect,
     DWConv,
     DWConvTranspose2d,
     Focus,
     GhostBottleneck,
     GhostConv,
     HGBlock,
     HGStem,
+    ImagePoolingAttn,
     Pose,
     RepC3,
     RepConv,
+    RepNCSPELAN4,
     ResNetLayer,
     RTDETRDecoder,
     Segment,
+    Silence,
+    WorldDetect,
 )
 from ultralytics.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, emojis, yaml_load
 from ultralytics.utils.checks import check_requirements, check_suffix, check_yaml
 from ultralytics.utils.loss import v8ClassificationLoss, v8DetectionLoss, v8OBBLoss, v8PoseLoss, v8SegmentationLoss
 from ultralytics.utils.plotting import feature_visualization
 from ultralytics.utils.torch_utils import (
     fuse_conv_and_bn,
@@ -218,15 +227,15 @@
             fn (function): the function to apply to the model
 
         Returns:
             (BaseModel): An updated BaseModel object.
         """
         self = super()._apply(fn)
         m = self.model[-1]  # Detect()
-        if isinstance(m, (Detect, Segment)):
+        if isinstance(m, Detect):  # includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
             m.stride = fn(m.stride)
             m.anchors = fn(m.anchors)
             m.strides = fn(m.strides)
         return self
 
     def load(self, weights, verbose=True):
         """
@@ -277,15 +286,15 @@
             self.yaml["nc"] = nc  # override YAML value
         self.model, self.save = parse_model(deepcopy(self.yaml), ch=ch, verbose=verbose)  # model, savelist
         self.names = {i: f"{i}" for i in range(self.yaml["nc"])}  # default names dict
         self.inplace = self.yaml.get("inplace", True)
 
         # Build strides
         m = self.model[-1]  # Detect()
-        if isinstance(m, (Detect, Segment, Pose, OBB)):
+        if isinstance(m, Detect):  # includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
             s = 256  # 2x min stride
             m.inplace = self.inplace
             forward = lambda x: self.forward(x)[0] if isinstance(m, (Segment, Pose, OBB)) else self.forward(x)
             m.stride = torch.tensor([s / x.shape[-2] for x in forward(torch.zeros(1, ch, s, s))])  # forward
             self.stride = m.stride
             m.bias_init()  # only run once
         else:
@@ -542,14 +551,103 @@
                 if m.i == max(embed):
                     return torch.unbind(torch.cat(embeddings, 1), dim=0)
         head = self.model[-1]
         x = head([y[j] for j in head.f], batch)  # head inference
         return x
 
 
+class WorldModel(DetectionModel):
+    """YOLOv8 World Model."""
+
+    def __init__(self, cfg="yolov8s-world.yaml", ch=3, nc=None, verbose=True):
+        """Initialize YOLOv8 world model with given config and parameters."""
+        self.txt_feats = torch.randn(1, nc or 80, 512)  # features placeholder
+        self.clip_model = None  # CLIP model placeholder
+        super().__init__(cfg=cfg, ch=ch, nc=nc, verbose=verbose)
+
+    def set_classes(self, text, batch=80, cache_clip_model=True):
+        """Set classes in advance so that model could do offline-inference without clip model."""
+        try:
+            import clip
+        except ImportError:
+            check_requirements("git+https://github.com/ultralytics/CLIP.git")
+            import clip
+
+        if (
+            not getattr(self, "clip_model", None) and cache_clip_model
+        ):  # for backwards compatibility of models lacking clip_model attribute
+            self.clip_model = clip.load("ViT-B/32")[0]
+        model = self.clip_model if cache_clip_model else clip.load("ViT-B/32")[0]
+        device = next(model.parameters()).device
+        text_token = clip.tokenize(text).to(device)
+        txt_feats = [model.encode_text(token).detach() for token in text_token.split(batch)]
+        txt_feats = txt_feats[0] if len(txt_feats) == 1 else torch.cat(txt_feats, dim=0)
+        txt_feats = txt_feats / txt_feats.norm(p=2, dim=-1, keepdim=True)
+        self.txt_feats = txt_feats.reshape(-1, len(text), txt_feats.shape[-1])
+        self.model[-1].nc = len(text)
+
+    def predict(self, x, profile=False, visualize=False, txt_feats=None, augment=False, embed=None):
+        """
+        Perform a forward pass through the model.
+
+        Args:
+            x (torch.Tensor): The input tensor.
+            profile (bool, optional): If True, profile the computation time for each layer. Defaults to False.
+            visualize (bool, optional): If True, save feature maps for visualization. Defaults to False.
+            txt_feats (torch.Tensor): The text features, use it if it's given. Defaults to None.
+            augment (bool, optional): If True, perform data augmentation during inference. Defaults to False.
+            embed (list, optional): A list of feature vectors/embeddings to return.
+
+        Returns:
+            (torch.Tensor): Model's output tensor.
+        """
+        txt_feats = (self.txt_feats if txt_feats is None else txt_feats).to(device=x.device, dtype=x.dtype)
+        if len(txt_feats) != len(x):
+            txt_feats = txt_feats.repeat(len(x), 1, 1)
+        ori_txt_feats = txt_feats.clone()
+        y, dt, embeddings = [], [], []  # outputs
+        for m in self.model:  # except the head part
+            if m.f != -1:  # if not from previous layer
+                x = y[m.f] if isinstance(m.f, int) else [x if j == -1 else y[j] for j in m.f]  # from earlier layers
+            if profile:
+                self._profile_one_layer(m, x, dt)
+            if isinstance(m, C2fAttn):
+                x = m(x, txt_feats)
+            elif isinstance(m, WorldDetect):
+                x = m(x, ori_txt_feats)
+            elif isinstance(m, ImagePoolingAttn):
+                txt_feats = m(x, txt_feats)
+            else:
+                x = m(x)  # run
+
+            y.append(x if m.i in self.save else None)  # save output
+            if visualize:
+                feature_visualization(x, m.type, m.i, save_dir=visualize)
+            if embed and m.i in embed:
+                embeddings.append(nn.functional.adaptive_avg_pool2d(x, (1, 1)).squeeze(-1).squeeze(-1))  # flatten
+                if m.i == max(embed):
+                    return torch.unbind(torch.cat(embeddings, 1), dim=0)
+        return x
+
+    def loss(self, batch, preds=None):
+        """
+        Compute loss.
+
+        Args:
+            batch (dict): Batch to compute loss on.
+            preds (torch.Tensor | List[torch.Tensor]): Predictions.
+        """
+        if not hasattr(self, "criterion"):
+            self.criterion = self.init_criterion()
+
+        if preds is None:
+            preds = self.forward(batch["img"], txt_feats=batch["txt_feats"])
+        return self.criterion(preds, batch)
+
+
 class Ensemble(nn.ModuleList):
     """Ensemble of models."""
 
     def __init__(self):
         """Initialize an ensemble of models."""
         super().__init__()
 
@@ -681,29 +779,28 @@
             model.stride = torch.tensor([32.0])
 
         # Append
         ensemble.append(model.fuse().eval() if fuse and hasattr(model, "fuse") else model.eval())  # model in eval mode
 
     # Module updates
     for m in ensemble.modules():
-        t = type(m)
-        if t in (nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Segment, Pose, OBB):
+        if hasattr(m, "inplace"):
             m.inplace = inplace
-        elif t is nn.Upsample and not hasattr(m, "recompute_scale_factor"):
+        elif isinstance(m, nn.Upsample) and not hasattr(m, "recompute_scale_factor"):
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model
     if len(ensemble) == 1:
         return ensemble[-1]
 
     # Return ensemble
     LOGGER.info(f"Ensemble created with {weights}\n")
     for k in "names", "nc", "yaml":
         setattr(ensemble, k, getattr(ensemble[0], k))
-    ensemble.stride = ensemble[torch.argmax(torch.tensor([m.stride.max() for m in ensemble])).int()].stride
+    ensemble.stride = ensemble[int(torch.argmax(torch.tensor([m.stride.max() for m in ensemble])))].stride
     assert all(ensemble[0].nc == m.nc for m in ensemble), f"Models differ in class counts {[m.nc for m in ensemble]}"
     return ensemble
 
 
 def attempt_load_one_weight(weight, device=None, inplace=True, fuse=False):
     """Loads a single model weights."""
     ckpt, weight = torch_safe_load(weight)  # load ckpt
@@ -717,18 +814,17 @@
     if not hasattr(model, "stride"):
         model.stride = torch.tensor([32.0])
 
     model = model.fuse().eval() if fuse and hasattr(model, "fuse") else model.eval()  # model in eval mode
 
     # Module updates
     for m in model.modules():
-        t = type(m)
-        if t in (nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Segment, Pose, OBB):
+        if hasattr(m, "inplace"):
             m.inplace = inplace
-        elif t is nn.Upsample and not hasattr(m, "recompute_scale_factor"):
+        elif isinstance(m, nn.Upsample) and not hasattr(m, "recompute_scale_factor"):
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model and ckpt
     return model, ckpt
 
 
 def parse_model(d, ch, verbose=True):  # model_dict, input_channels(3)
@@ -759,65 +855,80 @@
         m = getattr(torch.nn, m[3:]) if "nn." in m else globals()[m]  # get module
         for j, a in enumerate(args):
             if isinstance(a, str):
                 with contextlib.suppress(ValueError):
                     args[j] = locals()[a] if a in locals() else ast.literal_eval(a)
 
         n = n_ = max(round(n * depth), 1) if n > 1 else n  # depth gain
-        if m in (
+        if m in {
             Classify,
             Conv,
             ConvTranspose,
             GhostConv,
             Bottleneck,
             GhostBottleneck,
             SPP,
             SPPF,
             DWConv,
             Focus,
             BottleneckCSP,
             C1,
             C2,
             C2f,
+            RepNCSPELAN4,
+            ADown,
+            SPPELAN,
+            C2fAttn,
             C3,
             C3TR,
             C3Ghost,
             nn.ConvTranspose2d,
             DWConvTranspose2d,
             C3x,
             RepC3,
-        ):
+        }:
             c1, c2 = ch[f], args[0]
             if c2 != nc:  # if c2 not equal to number of classes (i.e. for Classify() output)
                 c2 = make_divisible(min(c2, max_channels) * width, 8)
+            if m is C2fAttn:
+                args[1] = make_divisible(min(args[1], max_channels // 2) * width, 8)  # embed channels
+                args[2] = int(
+                    max(round(min(args[2], max_channels // 2 // 32)) * width, 1) if args[2] > 1 else args[2]
+                )  # num heads
 
             args = [c1, c2, *args[1:]]
-            if m in (BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x, RepC3):
+            if m in {BottleneckCSP, C1, C2, C2f, C2fAttn, C3, C3TR, C3Ghost, C3x, RepC3}:
                 args.insert(2, n)  # number of repeats
                 n = 1
         elif m is AIFI:
             args = [ch[f], *args]
-        elif m in (HGStem, HGBlock):
+        elif m in {HGStem, HGBlock}:
             c1, cm, c2 = ch[f], args[0], args[1]
             args = [c1, cm, c2, *args[2:]]
             if m is HGBlock:
                 args.insert(4, n)  # number of repeats
                 n = 1
         elif m is ResNetLayer:
             c2 = args[1] if args[3] else args[1] * 4
         elif m is nn.BatchNorm2d:
             args = [ch[f]]
         elif m is Concat:
             c2 = sum(ch[x] for x in f)
-        elif m in (Detect, Segment, Pose, OBB):
+        elif m in {Detect, WorldDetect, Segment, Pose, OBB, ImagePoolingAttn}:
             args.append([ch[x] for x in f])
             if m is Segment:
                 args[2] = make_divisible(min(args[2], max_channels) * width, 8)
         elif m is RTDETRDecoder:  # special case, channels arg must be passed in index 1
             args.insert(1, [ch[x] for x in f])
+        elif m is CBLinear:
+            c2 = args[0]
+            c1 = ch[f]
+            args = [c1, c2, *args[1:]]
+        elif m is CBFuse:
+            c2 = ch[f[-1]]
         else:
             c2 = ch[f]
 
         m_ = nn.Sequential(*(m(*args) for _ in range(n))) if n > 1 else m(*args)  # module
         t = str(m)[8:-2].replace("__main__.", "")  # module type
         m.np = sum(x.numel() for x in m_.parameters())  # number params
         m_.i, m_.f, m_.type = i, f, t  # attach index, 'from' index, type
@@ -881,15 +992,15 @@
     Raises:
         SyntaxError: If the task of the model could not be determined.
     """
 
     def cfg2task(cfg):
         """Guess from YAML dictionary."""
         m = cfg["head"][-1][-2].lower()  # output module name
-        if m in ("classify", "classifier", "cls", "fc"):
+        if m in {"classify", "classifier", "cls", "fc"}:
             return "classify"
         if m == "detect":
             return "detect"
         if m == "segment":
             return "segment"
         if m == "pose":
             return "pose"
@@ -907,24 +1018,24 @@
             with contextlib.suppress(Exception):
                 return eval(x)["task"]
         for x in "model.yaml", "model.model.yaml", "model.model.model.yaml":
             with contextlib.suppress(Exception):
                 return cfg2task(eval(x))
 
         for m in model.modules():
-            if isinstance(m, Detect):
-                return "detect"
-            elif isinstance(m, Segment):
+            if isinstance(m, Segment):
                 return "segment"
             elif isinstance(m, Classify):
                 return "classify"
             elif isinstance(m, Pose):
                 return "pose"
             elif isinstance(m, OBB):
                 return "obb"
+            elif isinstance(m, (Detect, WorldDetect)):
+                return "detect"
 
     # Guess from model filename
     if isinstance(model, (str, Path)):
         model = Path(model)
         if "-seg" in model.stem or "segment" in model.parts:
             return "segment"
         elif "-cls" in model.stem or "classify" in model.parts:
```

### Comparing `ultralytics-8.1.9/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.0/ultralytics/solutions/ai_gym.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,56 +42,50 @@
         line_thickness=2,
         view_img=False,
         pose_up_angle=145.0,
         pose_down_angle=90.0,
         pose_type="pullup",
     ):
         """
-        Configures the AIGym line_thickness, save image and view image parameters
+        Configures the AIGym line_thickness, save image and view image parameters.
+
         Args:
             kpts_to_check (list): 3 keypoints for counting
             line_thickness (int): Line thickness for bounding boxes.
             view_img (bool): display the im0
             pose_up_angle (float): Angle to set pose position up
             pose_down_angle (float): Angle to set pose position down
-            pose_type: "pushup", "pullup" or "abworkout"
+            pose_type (str): "pushup", "pullup" or "abworkout"
         """
         self.kpts_to_check = kpts_to_check
         self.tf = line_thickness
         self.view_img = view_img
         self.poseup_angle = pose_up_angle
         self.posedown_angle = pose_down_angle
         self.pose_type = pose_type
 
     def start_counting(self, im0, results, frame_count):
         """
-        Function used to count the gym steps
+        Function used to count the gym steps.
+
         Args:
             im0 (ndarray): Current frame from the video stream.
-            results: Pose estimation data
-            frame_count: store current frame count
+            results (list): Pose estimation data
+            frame_count (int): store current frame count
         """
         self.im0 = im0
         if frame_count == 1:
             self.count = [0] * len(results[0])
             self.angle = [0] * len(results[0])
             self.stage = ["-" for _ in results[0]]
         self.keypoints = results[0].keypoints.data
         self.annotator = Annotator(im0, line_width=2)
 
-        num_keypoints = len(results[0])
-
-        # Resize self.angle, self.count, and self.stage if the number of keypoints has changed
-        if len(self.angle) != num_keypoints:
-            self.angle = [0] * num_keypoints
-            self.count = [0] * num_keypoints
-            self.stage = ["-" for _ in range(num_keypoints)]
-
         for ind, k in enumerate(reversed(self.keypoints)):
-            if self.pose_type in ["pushup", "pullup"]:
+            if self.pose_type in {"pushup", "pullup"}:
                 self.angle[ind] = self.annotator.estimate_pose_angle(
                     k[int(self.kpts_to_check[0])].cpu(),
                     k[int(self.kpts_to_check[1])].cpu(),
                     k[int(self.kpts_to_check[2])].cpu(),
                 )
                 self.im0 = self.annotator.draw_specific_points(k, self.kpts_to_check, shape=(640, 640), radius=10)
```

### Comparing `ultralytics-8.1.9/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.0/ultralytics/solutions/distance_calculation.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,33 +103,36 @@
         """
         self.boxes = tracks[0].boxes.xyxy.cpu()
         self.clss = tracks[0].boxes.cls.cpu().tolist()
         self.trk_ids = tracks[0].boxes.id.int().cpu().tolist()
 
     def calculate_centroid(self, box):
         """
-        Calculate the centroid of bounding box
+        Calculate the centroid of bounding box.
+
         Args:
             box (list): Bounding box data
         """
         return int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2)
 
     def calculate_distance(self, centroid1, centroid2):
         """
-        Calculate distance between two centroids
+        Calculate distance between two centroids.
+
         Args:
             centroid1 (point): First bounding box data
             centroid2 (point): Second bounding box data
         """
         pixel_distance = math.sqrt((centroid1[0] - centroid2[0]) ** 2 + (centroid1[1] - centroid2[1]) ** 2)
         return pixel_distance / self.pixel_per_meter, (pixel_distance / self.pixel_per_meter) * 1000
 
     def start_process(self, im0, tracks):
         """
-        Calculate distance between two bounding boxes based on tracking data
+        Calculate distance between two bounding boxes based on tracking data.
+
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img:
```

### Comparing `ultralytics-8.1.9/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.0/ultralytics/solutions/heatmap.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,18 +20,21 @@
         """Initializes the heatmap class with default values for Visual, Image, track, count and heatmap parameters."""
 
         # Visual information
         self.annotator = None
         self.view_img = False
         self.shape = "circle"
 
+        self.names = None  # Classes names
+
         # Image information
         self.imw = None
         self.imh = None
         self.im0 = None
+        self.tf = 2
         self.view_in_counts = True
         self.view_out_counts = True
 
         # Heatmap colormap and heatmap np array
         self.colormap = None
         self.heatmap = None
         self.heatmap_alpha = 0.5
@@ -48,104 +51,106 @@
         self.line_dist_thresh = 15
         self.region_thickness = 5
         self.region_color = (255, 0, 255)
 
         # Object Counting Information
         self.in_counts = 0
         self.out_counts = 0
-        self.counting_list = []
-        self.count_txt_thickness = 0
+        self.count_ids = []
+        self.class_wise_count = {}
         self.count_txt_color = (0, 0, 0)
-        self.count_color = (255, 255, 255)
+        self.count_bg_color = (255, 255, 255)
+        self.cls_txtdisplay_gap = 50
 
         # Decay factor
         self.decay_factor = 0.99
 
         # Check if environment support imshow
         self.env_check = check_imshow(warn=True)
 
     def set_args(
         self,
         imw,
         imh,
+        classes_names=None,
         colormap=cv2.COLORMAP_JET,
         heatmap_alpha=0.5,
         view_img=False,
         view_in_counts=True,
         view_out_counts=True,
         count_reg_pts=None,
-        count_txt_thickness=2,
         count_txt_color=(0, 0, 0),
-        count_color=(255, 255, 255),
+        count_bg_color=(255, 255, 255),
         count_reg_color=(255, 0, 255),
         region_thickness=5,
         line_dist_thresh=15,
+        line_thickness=2,
         decay_factor=0.99,
         shape="circle",
     ):
         """
         Configures the heatmap colormap, width, height and display parameters.
 
         Args:
             colormap (cv2.COLORMAP): The colormap to be set.
             imw (int): The width of the frame.
             imh (int): The height of the frame.
+            classes_names (dict): Classes names
+            line_thickness (int): Line thickness for bounding boxes.
             heatmap_alpha (float): alpha value for heatmap display
             view_img (bool): Flag indicating frame display
             view_in_counts (bool): Flag to control whether to display the incounts on video stream.
             view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
             count_reg_pts (list): Object counting region points
-            count_txt_thickness (int): Text thickness for object counting display
             count_txt_color (RGB color): count text color value
-            count_color (RGB color): count text background color value
+            count_bg_color (RGB color): count highlighter line color
             count_reg_color (RGB color): Color of object counting region
             region_thickness (int): Object counting Region thickness
             line_dist_thresh (int): Euclidean Distance threshold for line counter
             decay_factor (float): value for removing heatmap area after object passed
             shape (str): Heatmap shape, rect or circle shape supported
         """
+        self.tf = line_thickness
+        self.names = classes_names
         self.imw = imw
         self.imh = imh
         self.heatmap_alpha = heatmap_alpha
         self.view_img = view_img
         self.view_in_counts = view_in_counts
         self.view_out_counts = view_out_counts
         self.colormap = colormap
 
         # Region and line selection
         if count_reg_pts is not None:
             if len(count_reg_pts) == 2:
                 print("Line Counter Initiated.")
                 self.count_reg_pts = count_reg_pts
-                self.counting_region = LineString(count_reg_pts)
-
-            elif len(count_reg_pts) == 4:
-                print("Region Counter Initiated.")
+                self.counting_region = LineString(self.count_reg_pts)
+            elif len(count_reg_pts) >= 3:
+                print("Polygon Counter Initiated.")
                 self.count_reg_pts = count_reg_pts
                 self.counting_region = Polygon(self.count_reg_pts)
-
             else:
-                print("Region or line points Invalid, 2 or 4 points supported")
+                print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
                 print("Using Line Counter Now")
-                self.counting_region = Polygon([(20, 400), (1260, 400)])  # dummy points
+                self.counting_region = LineString(self.count_reg_pts)
 
         # Heatmap new frame
         self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
 
-        self.count_txt_thickness = count_txt_thickness
         self.count_txt_color = count_txt_color
-        self.count_color = count_color
+        self.count_bg_color = count_bg_color
         self.region_color = count_reg_color
         self.region_thickness = region_thickness
         self.decay_factor = decay_factor
         self.line_dist_thresh = line_dist_thresh
         self.shape = shape
 
         # shape of heatmap, if not selected
-        if self.shape not in ["circle", "rect"]:
+        if self.shape not in {"circle", "rect"}:
             print("Unknown shape value provided, 'circle' & 'rect' supported")
             print("Using Circular shape now")
             self.shape = "circle"
 
     def extract_results(self, tracks):
         """
         Extracts results from the provided data.
@@ -169,24 +174,30 @@
         if tracks[0].boxes.id is None:
             self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
             if self.view_img and self.env_check:
                 self.display_frames()
             return im0
         self.heatmap *= self.decay_factor  # decay factor
         self.extract_results(tracks)
-        self.annotator = Annotator(self.im0, self.count_txt_thickness, None)
+        self.annotator = Annotator(self.im0, self.tf, None)
 
         if self.count_reg_pts is not None:
             # Draw counting region
             if self.view_in_counts or self.view_out_counts:
                 self.annotator.draw_region(
                     reg_pts=self.count_reg_pts, color=self.region_color, thickness=self.region_thickness
                 )
 
             for box, cls, track_id in zip(self.boxes, self.clss, self.track_ids):
+                # Store class info
+                if self.names[cls] not in self.class_wise_count:
+                    if len(self.names[cls]) > 5:
+                        self.names[cls] = self.names[cls][:5]
+                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
                     mask = (x - center[0]) ** 2 + (y - center[1]) ** 2 <= radius**2
 
@@ -199,31 +210,44 @@
 
                 # Store tracking hist
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
-                # Count objects
-                if len(self.count_reg_pts) == 4:
-                    if self.counting_region.contains(Point(track_line[-1])) and track_id not in self.counting_list:
-                        self.counting_list.append(track_id)
-                        if box[0] < self.counting_region.centroid.x:
-                            self.out_counts += 1
-                        else:
+                prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
+
+                # Count objects in any polygon
+                if len(self.count_reg_pts) >= 3:
+                    is_inside = self.counting_region.contains(Point(track_line[-1]))
+
+                    if prev_position is not None and is_inside and track_id not in self.count_ids:
+                        self.count_ids.append(track_id)
+
+                        if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
+                            self.class_wise_count[self.names[cls]]["in"] += 1
+                        else:
+                            self.out_counts += 1
+                            self.class_wise_count[self.names[cls]]["out"] += 1
 
+                # Count objects using line
                 elif len(self.count_reg_pts) == 2:
-                    distance = Point(track_line[-1]).distance(self.counting_region)
-                    if distance < self.line_dist_thresh and track_id not in self.counting_list:
-                        self.counting_list.append(track_id)
-                        if box[0] < self.counting_region.centroid.x:
-                            self.out_counts += 1
-                        else:
-                            self.in_counts += 1
+                    if prev_position is not None and track_id not in self.count_ids:
+                        distance = Point(track_line[-1]).distance(self.counting_region)
+                        if distance < self.line_dist_thresh and track_id not in self.count_ids:
+                            self.count_ids.append(track_id)
+
+                            if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
+                                self.in_counts += 1
+                                self.class_wise_count[self.names[cls]]["in"] += 1
+                            else:
+                                self.out_counts += 1
+                                self.class_wise_count[self.names[cls]]["out"] += 1
+
         else:
             for box, cls in zip(self.boxes, self.clss):
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
@@ -236,34 +260,35 @@
                 else:
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += 2
 
         # Normalize, apply colormap to heatmap and combine with original image
         heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
         heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
 
-        incount_label = f"In Count : {self.in_counts}"
-        outcount_label = f"OutCount : {self.out_counts}"
+        label = "Ultralytics Analytics \t"
 
-        # Display counts based on user choice
-        counts_label = None
-        if not self.view_in_counts and not self.view_out_counts:
-            counts_label = None
-        elif not self.view_in_counts:
-            counts_label = outcount_label
-        elif not self.view_out_counts:
-            counts_label = incount_label
-        else:
-            counts_label = f"{incount_label} {outcount_label}"
+        for key, value in self.class_wise_count.items():
+            if value["in"] != 0 or value["out"] != 0:
+                if not self.view_in_counts and not self.view_out_counts:
+                    label = None
+                elif not self.view_in_counts:
+                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                elif not self.view_out_counts:
+                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                else:
+                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+
+        label = label.rstrip()
+        label = label.split("\t")
 
-        if self.count_reg_pts is not None and counts_label is not None:
-            self.annotator.count_labels(
-                counts=counts_label,
-                count_txt_size=self.count_txt_thickness,
-                txt_color=self.count_txt_color,
-                color=self.count_color,
+        if self.count_reg_pts is not None and label is not None:
+            self.annotator.display_counts(
+                counts=label,
+                count_txt_color=self.count_txt_color,
+                count_bg_color=self.count_bg_color,
             )
 
         self.im0 = cv2.addWeighted(self.im0, 1 - self.heatmap_alpha, heatmap_colored, self.heatmap_alpha, 0)
 
         if self.env_check and self.view_img:
             self.display_frames()
```

### Comparing `ultralytics-8.1.9/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.0/ultralytics/solutions/object_counter.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,99 +34,103 @@
         self.tf = None
         self.view_img = False
         self.view_in_counts = True
         self.view_out_counts = True
 
         self.names = None  # Classes names
         self.annotator = None  # Annotator
+        self.window_name = "Ultralytics YOLOv8 Object Counter"
 
         # Object counting Information
         self.in_counts = 0
         self.out_counts = 0
-        self.counting_list = []
+        self.count_ids = []
+        self.class_wise_count = {}
         self.count_txt_thickness = 0
-        self.count_txt_color = (0, 0, 0)
-        self.count_color = (255, 255, 255)
+        self.count_txt_color = (255, 255, 255)
+        self.count_bg_color = (255, 255, 255)
+        self.cls_txtdisplay_gap = 50
+        self.fontsize = 0.6
 
         # Tracks info
         self.track_history = defaultdict(list)
         self.track_thickness = 2
         self.draw_tracks = False
-        self.track_color = (0, 255, 0)
+        self.track_color = None
 
         # Check if environment support imshow
         self.env_check = check_imshow(warn=True)
 
     def set_args(
         self,
         classes_names,
         reg_pts,
         count_reg_color=(255, 0, 255),
+        count_txt_color=(0, 0, 0),
+        count_bg_color=(255, 255, 255),
         line_thickness=2,
         track_thickness=2,
         view_img=False,
         view_in_counts=True,
         view_out_counts=True,
         draw_tracks=False,
-        count_txt_thickness=2,
-        count_txt_color=(0, 0, 0),
-        count_color=(255, 255, 255),
-        track_color=(0, 255, 0),
+        track_color=None,
         region_thickness=5,
         line_dist_thresh=15,
+        cls_txtdisplay_gap=50,
     ):
         """
         Configures the Counter's image, bounding box line thickness, and counting region points.
 
         Args:
             line_thickness (int): Line thickness for bounding boxes.
             view_img (bool): Flag to control whether to display the video stream.
             view_in_counts (bool): Flag to control whether to display the incounts on video stream.
             view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
             reg_pts (list): Initial list of points defining the counting region.
             classes_names (dict): Classes names
             track_thickness (int): Track thickness
             draw_tracks (Bool): draw tracks
-            count_txt_thickness (int): Text thickness for object counting display
             count_txt_color (RGB color): count text color value
-            count_color (RGB color): count text background color value
+            count_bg_color (RGB color): count highlighter line color
             count_reg_color (RGB color): Color of object counting region
             track_color (RGB color): color for tracks
             region_thickness (int): Object counting Region thickness
             line_dist_thresh (int): Euclidean Distance threshold for line counter
+            cls_txtdisplay_gap (int): Display gap between each class count
         """
         self.tf = line_thickness
         self.view_img = view_img
         self.view_in_counts = view_in_counts
         self.view_out_counts = view_out_counts
         self.track_thickness = track_thickness
         self.draw_tracks = draw_tracks
 
         # Region and line selection
         if len(reg_pts) == 2:
             print("Line Counter Initiated.")
             self.reg_pts = reg_pts
             self.counting_region = LineString(self.reg_pts)
-        elif len(reg_pts) == 4:
-            print("Region Counter Initiated.")
+        elif len(reg_pts) >= 3:
+            print("Polygon Counter Initiated.")
             self.reg_pts = reg_pts
             self.counting_region = Polygon(self.reg_pts)
         else:
-            print("Invalid Region points provided, region_points can be 2 or 4")
+            print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
             print("Using Line Counter Now")
             self.counting_region = LineString(self.reg_pts)
 
         self.names = classes_names
         self.track_color = track_color
-        self.count_txt_thickness = count_txt_thickness
         self.count_txt_color = count_txt_color
-        self.count_color = count_color
+        self.count_bg_color = count_bg_color
         self.region_color = count_reg_color
         self.region_thickness = region_thickness
         self.line_dist_thresh = line_dist_thresh
+        self.cls_txtdisplay_gap = cls_txtdisplay_gap
 
     def mouse_event_for_region(self, event, x, y, flags, params):
         """
         This function is designed to move region with mouse events in a real-time video stream.
 
         Args:
             event (int): The type of mouse event (e.g., cv2.EVENT_MOUSEMOVE, cv2.EVENT_LBUTTONDOWN, etc.).
@@ -154,114 +158,125 @@
 
         elif event == cv2.EVENT_LBUTTONUP:
             self.is_drawing = False
             self.selected_point = None
 
     def extract_and_process_tracks(self, tracks):
         """Extracts and processes tracks for object counting in a video stream."""
-        boxes = tracks[0].boxes.xyxy.cpu()
-        clss = tracks[0].boxes.cls.cpu().tolist()
-        track_ids = tracks[0].boxes.id.int().cpu().tolist()
 
         # Annotator Init and region drawing
         self.annotator = Annotator(self.im0, self.tf, self.names)
+
+        # Draw region or line
         self.annotator.draw_region(reg_pts=self.reg_pts, color=self.region_color, thickness=self.region_thickness)
 
-        # Extract tracks
-        for box, track_id, cls in zip(boxes, track_ids, clss):
-            # Draw bounding box
-            self.annotator.box_label(box, label=f"{track_id}:{self.names[cls]}", color=colors(int(cls), True))
-
-            # Draw Tracks
-            track_line = self.track_history[track_id]
-            track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
-            if len(track_line) > 30:
-                track_line.pop(0)
-
-            # Draw track trails
-            if self.draw_tracks:
-                self.annotator.draw_centroid_and_tracks(
-                    track_line, color=self.track_color, track_thickness=self.track_thickness
-                )
+        if tracks[0].boxes.id is not None:
+            boxes = tracks[0].boxes.xyxy.cpu()
+            clss = tracks[0].boxes.cls.cpu().tolist()
+            track_ids = tracks[0].boxes.id.int().cpu().tolist()
+
+            # Extract tracks
+            for box, track_id, cls in zip(boxes, track_ids, clss):
+                # Draw bounding box
+                self.annotator.box_label(box, label=f"{self.names[cls]}#{track_id}", color=colors(int(track_id), True))
+
+                # Store class info
+                if self.names[cls] not in self.class_wise_count:
+                    if len(self.names[cls]) > 5:
+                        self.names[cls] = self.names[cls][:5]
+                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+
+                # Draw Tracks
+                track_line = self.track_history[track_id]
+                track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
+                if len(track_line) > 30:
+                    track_line.pop(0)
+
+                # Draw track trails
+                if self.draw_tracks:
+                    self.annotator.draw_centroid_and_tracks(
+                        track_line,
+                        color=self.track_color if self.track_color else colors(int(track_id), True),
+                        track_thickness=self.track_thickness,
+                    )
+
+                prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
+
+                # Count objects in any polygon
+                if len(self.reg_pts) >= 3:
+                    is_inside = self.counting_region.contains(Point(track_line[-1]))
 
-            prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
+                    if prev_position is not None and is_inside and track_id not in self.count_ids:
+                        self.count_ids.append(track_id)
 
-            # Count objects
-            if len(self.reg_pts) == 4:
-                if (
-                    prev_position is not None
-                    and self.counting_region.contains(Point(track_line[-1]))
-                    and track_id not in self.counting_list
-                ):
-                    self.counting_list.append(track_id)
-                    if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
-                        self.in_counts += 1
-                    else:
-                        self.out_counts += 1
-
-            elif len(self.reg_pts) == 2:
-                if prev_position is not None:
-                    distance = Point(track_line[-1]).distance(self.counting_region)
-                    if distance < self.line_dist_thresh and track_id not in self.counting_list:
-                        self.counting_list.append(track_id)
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
+                            self.class_wise_count[self.names[cls]]["in"] += 1
                         else:
                             self.out_counts += 1
+                            self.class_wise_count[self.names[cls]]["out"] += 1
 
-        incount_label = f"In Count : {self.in_counts}"
-        outcount_label = f"OutCount : {self.out_counts}"
-
-        # Display counts based on user choice
-        counts_label = None
-        if not self.view_in_counts and not self.view_out_counts:
-            counts_label = None
-        elif not self.view_in_counts:
-            counts_label = outcount_label
-        elif not self.view_out_counts:
-            counts_label = incount_label
-        else:
-            counts_label = f"{incount_label} {outcount_label}"
-
-        if counts_label is not None:
-            self.annotator.count_labels(
-                counts=counts_label,
-                count_txt_size=self.count_txt_thickness,
-                txt_color=self.count_txt_color,
-                color=self.count_color,
+                # Count objects using line
+                elif len(self.reg_pts) == 2:
+                    if prev_position is not None and track_id not in self.count_ids:
+                        distance = Point(track_line[-1]).distance(self.counting_region)
+                        if distance < self.line_dist_thresh and track_id not in self.count_ids:
+                            self.count_ids.append(track_id)
+
+                            if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
+                                self.in_counts += 1
+                                self.class_wise_count[self.names[cls]]["in"] += 1
+                            else:
+                                self.out_counts += 1
+                                self.class_wise_count[self.names[cls]]["out"] += 1
+
+        label = "Ultralytics Analytics \t"
+
+        for key, value in self.class_wise_count.items():
+            if value["in"] != 0 or value["out"] != 0:
+                if not self.view_in_counts and not self.view_out_counts:
+                    label = None
+                elif not self.view_in_counts:
+                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                elif not self.view_out_counts:
+                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                else:
+                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+
+        label = label.rstrip()
+        label = label.split("\t")
+
+        if label is not None:
+            self.annotator.display_counts(
+                counts=label,
+                count_txt_color=self.count_txt_color,
+                count_bg_color=self.count_bg_color,
             )
 
     def display_frames(self):
         """Display frame."""
         if self.env_check:
-            cv2.namedWindow("Ultralytics YOLOv8 Object Counter")
+            cv2.namedWindow(self.window_name)
             if len(self.reg_pts) == 4:  # only add mouse event If user drawn region
-                cv2.setMouseCallback(
-                    "Ultralytics YOLOv8 Object Counter", self.mouse_event_for_region, {"region_points": self.reg_pts}
-                )
-            cv2.imshow("Ultralytics YOLOv8 Object Counter", self.im0)
+                cv2.setMouseCallback(self.window_name, self.mouse_event_for_region, {"region_points": self.reg_pts})
+            cv2.imshow(self.window_name, self.im0)
             # Break Window
             if cv2.waitKey(1) & 0xFF == ord("q"):
                 return
 
     def start_counting(self, im0, tracks):
         """
         Main function to start the object counting process.
 
         Args:
             im0 (ndarray): Current frame from the video stream.
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0  # store image
-
-        if tracks[0].boxes.id is None:
-            if self.view_img:
-                self.display_frames()
-            return im0
-        self.extract_and_process_tracks(tracks)
+        self.extract_and_process_tracks(tracks)  # draw region even if no objects
 
         if self.view_img:
             self.display_frames()
         return self.im0
 
 
 if __name__ == "__main__":
```

### Comparing `ultralytics-8.1.9/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.0/ultralytics/solutions/speed_estimation.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,16 @@
         self.annotator.box_label(box, speed_label, bbox_color)
 
         cv2.polylines(self.im0, [self.trk_pts], isClosed=False, color=(0, 255, 0), thickness=1)
         cv2.circle(self.im0, (int(track[-1][0]), int(track[-1][1])), 5, bbox_color, -1)
 
     def calculate_speed(self, trk_id, track):
         """
-        Calculation of object speed
+        Calculation of object speed.
+
         Args:
             trk_id (int): object track id.
             track (list): tracking history for tracks path drawing
         """
 
         if not self.reg_pts[0][0] < track[-1][0] < self.reg_pts[1][0]:
             return
@@ -149,30 +150,32 @@
                 dist_difference = np.abs(track[-1][1] - self.trk_previous_points[trk_id][1])
                 speed = dist_difference / time_difference
                 self.dist_data[trk_id] = speed
 
         self.trk_previous_times[trk_id] = time()
         self.trk_previous_points[trk_id] = track[-1]
 
-    def estimate_speed(self, im0, tracks):
+    def estimate_speed(self, im0, tracks, region_color=(255, 0, 0)):
         """
-        Calculate object based on tracking data
+        Calculate object based on tracking data.
+
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
+            region_color (tuple): Color to use when drawing regions.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img and self.env_check:
                 self.display_frames()
             return im0
         self.extract_tracks(tracks)
 
         self.annotator = Annotator(self.im0, line_width=2)
-        self.annotator.draw_region(reg_pts=self.reg_pts, color=(255, 0, 0), thickness=self.region_thickness)
+        self.annotator.draw_region(reg_pts=self.reg_pts, color=region_color, thickness=self.region_thickness)
 
         for box, trk_id, cls in zip(self.boxes, self.trk_ids, self.clss):
             track = self.store_track_info(trk_id, box)
 
             if trk_id not in self.trk_previous_times:
                 self.trk_previous_times[trk_id] = 0
```

### Comparing `ultralytics-8.1.9/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.0/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.0/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.0/ultralytics/trackers/byte_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import numpy as np
 
+from ..utils import LOGGER
+from ..utils.ops import xywh2ltwh
 from .basetrack import BaseTrack, TrackState
 from .utils import matching
 from .utils.kalman_filter import KalmanFilterXYAH
-from ..utils.ops import xywh2ltwh
-from ..utils import LOGGER
 
 
 class STrack(BaseTrack):
     """
     Single object tracking representation that uses Kalman filtering for state estimation.
 
     This class is responsible for storing all the information regarding individual tracklets and performs state updates
@@ -43,15 +43,15 @@
 
     shared_kalman = KalmanFilterXYAH()
 
     def __init__(self, xywh, score, cls):
         """Initialize new STrack instance."""
         super().__init__()
         # xywh+idx or xywha+idx
-        assert len(xywh) in [5, 6], f"expected 5 or 6 values but got {len(xywh)}"
+        assert len(xywh) in {5, 6}, f"expected 5 or 6 values but got {len(xywh)}"
         self._tlwh = np.asarray(xywh2ltwh(xywh[:4]), dtype=np.float32)
         self.kalman_filter = None
         self.mean, self.covariance = None, None
         self.is_activated = False
 
         self.score = score
         self.tracklet_len = 0
@@ -231,15 +231,15 @@
         get_kalmanfilter(): Returns a Kalman filter object for tracking bounding boxes.
         init_track(dets, scores, cls, img=None): Initialize object tracking with detections.
         get_dists(tracks, detections): Calculates the distance between tracks and detections.
         multi_predict(tracks): Predicts the location of tracks.
         reset_id(): Resets the ID counter of STrack.
         joint_stracks(tlista, tlistb): Combines two lists of stracks.
         sub_stracks(tlista, tlistb): Filters out the stracks present in the second list from the first list.
-        remove_duplicate_stracks(stracksa, stracksb): Removes duplicate stracks based on IOU.
+        remove_duplicate_stracks(stracksa, stracksb): Removes duplicate stracks based on IoU.
     """
 
     def __init__(self, args, frame_rate=30):
         """Initialize a YOLOv8 object to track objects with given arguments and frame rate."""
         self.tracked_stracks = []  # type: list[STrack]
         self.lost_stracks = []  # type: list[STrack]
         self.removed_stracks = []  # type: list[STrack]
@@ -369,15 +369,15 @@
         return KalmanFilterXYAH()
 
     def init_track(self, dets, scores, cls, img=None):
         """Initialize object tracking with detections and scores using STrack algorithm."""
         return [STrack(xyxy, s, c) for (xyxy, s, c) in zip(dets, scores, cls)] if len(dets) else []  # detections
 
     def get_dists(self, tracks, detections):
-        """Calculates the distance between tracks and detections using IOU and fuses scores."""
+        """Calculates the distance between tracks and detections using IoU and fuses scores."""
         dists = matching.iou_distance(tracks, detections)
         # TODO: mot20
         # if not self.args.mot20:
         dists = matching.fuse_score(dists, detections)
         return dists
 
     def multi_predict(self, tracks):
@@ -424,15 +424,15 @@
         return list(stracks.values())
         """
         track_ids_b = {t.track_id for t in tlistb}
         return [t for t in tlista if t.track_id not in track_ids_b]
 
     @staticmethod
     def remove_duplicate_stracks(stracksa, stracksb):
-        """Remove duplicate stracks with non-maximum IOU distance."""
+        """Remove duplicate stracks with non-maximum IoU distance."""
         pdist = matching.iou_distance(stracksa, stracksb)
         pairs = np.where(pdist < 0.15)
         dupa, dupb = [], []
         for p, q in zip(*pairs):
             timep = stracksa[p].frame_id - stracksa[p].start_frame
             timeq = stracksb[q].frame_id - stracksb[q].start_frame
             if timep > timeq:
```

### Comparing `ultralytics-8.1.9/ultralytics/trackers/track.py` & `ultralytics-8.2.0/ultralytics/trackers/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import partial
 from pathlib import Path
 
 import torch
 
 from ultralytics.utils import IterableSimpleNamespace, yaml_load
 from ultralytics.utils.checks import check_yaml
+
 from .bot_sort import BOTSORT
 from .byte_tracker import BYTETracker
 
 # A mapping of tracker types to corresponding tracker classes
 TRACKER_MAP = {"bytetrack": BYTETracker, "botsort": BOTSORT}
 
 
@@ -27,44 +28,50 @@
     """
     if hasattr(predictor, "trackers") and persist:
         return
 
     tracker = check_yaml(predictor.args.tracker)
     cfg = IterableSimpleNamespace(**yaml_load(tracker))
 
-    if cfg.tracker_type not in ["bytetrack", "botsort"]:
+    if cfg.tracker_type not in {"bytetrack", "botsort"}:
         raise AssertionError(f"Only 'bytetrack' and 'botsort' are supported for now, but got '{cfg.tracker_type}'")
 
     trackers = []
     for _ in range(predictor.dataset.bs):
         tracker = TRACKER_MAP[cfg.tracker_type](args=cfg, frame_rate=30)
         trackers.append(tracker)
+        if predictor.dataset.mode != "stream":  # only need one tracker for other modes.
+            break
     predictor.trackers = trackers
+    predictor.vid_path = [None] * predictor.dataset.bs  # for determining when to reset tracker on new video
 
 
 def on_predict_postprocess_end(predictor: object, persist: bool = False) -> None:
     """
     Postprocess detected boxes and update with object tracking.
 
     Args:
         predictor (object): The predictor object containing the predictions.
         persist (bool, optional): Whether to persist the trackers if they already exist. Defaults to False.
     """
-    bs = predictor.dataset.bs
     path, im0s = predictor.batch[:2]
 
     is_obb = predictor.args.task == "obb"
-    for i in range(bs):
-        if not persist and predictor.vid_path[i] != str(predictor.save_dir / Path(path[i]).name):  # new video
-            predictor.trackers[i].reset()
+    is_stream = predictor.dataset.mode == "stream"
+    for i in range(len(im0s)):
+        tracker = predictor.trackers[i if is_stream else 0]
+        vid_path = predictor.save_dir / Path(path[i]).name
+        if not persist and predictor.vid_path[i if is_stream else 0] != vid_path:
+            tracker.reset()
+            predictor.vid_path[i if is_stream else 0] = vid_path
 
         det = (predictor.results[i].obb if is_obb else predictor.results[i].boxes).cpu().numpy()
         if len(det) == 0:
             continue
-        tracks = predictor.trackers[i].update(det, im0s[i])
+        tracks = tracker.update(det, im0s[i])
         if len(tracks) == 0:
             continue
         idx = tracks[:, -1].astype(int)
         predictor.results[i] = predictor.results[i][idx]
 
         update_args = dict()
         update_args["obb" if is_obb else "boxes"] = torch.as_tensor(tracks[:, :-1])
```

### Comparing `ultralytics-8.1.9/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.0/ultralytics/trackers/utils/gmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     This class provides methods for tracking and detecting objects based on several tracking algorithms including ORB,
     SIFT, ECC, and Sparse Optical Flow. It also supports downscaling of frames for computational efficiency.
 
     Attributes:
         method (str): The method used for tracking. Options include 'orb', 'sift', 'ecc', 'sparseOptFlow', 'none'.
         downscale (int): Factor by which to downscale the frames for processing.
-        prevFrame (np.array): Stores the previous frame for tracking.
+        prevFrame (np.ndarray): Stores the previous frame for tracking.
         prevKeyPoints (list): Stores the keypoints from the previous frame.
-        prevDescriptors (np.array): Stores the descriptors from the previous frame.
+        prevDescriptors (np.ndarray): Stores the descriptors from the previous frame.
         initializedFirstFrame (bool): Flag to indicate if the first frame has been processed.
 
     Methods:
         __init__(self, method='sparseOptFlow', downscale=2): Initializes a GMC object with the specified method
                                                               and downscale factor.
         apply(self, raw_frame, detections=None): Applies the chosen method to a raw frame and optionally uses
                                                  provided detections.
@@ -78,45 +78,44 @@
         self.initializedFirstFrame = False
 
     def apply(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply object detection on a raw frame using specified method.
 
         Args:
-            raw_frame (np.array): The raw frame to be processed.
+            raw_frame (np.ndarray): The raw frame to be processed.
             detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.array): Processed frame.
+            (np.ndarray): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.apply(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
-        if self.method in ["orb", "sift"]:
+        if self.method in {"orb", "sift"}:
             return self.applyFeatures(raw_frame, detections)
         elif self.method == "ecc":
-            return self.applyEcc(raw_frame, detections)
+            return self.applyEcc(raw_frame)
         elif self.method == "sparseOptFlow":
-            return self.applySparseOptFlow(raw_frame, detections)
+            return self.applySparseOptFlow(raw_frame)
         else:
             return np.eye(2, 3)
 
-    def applyEcc(self, raw_frame: np.array, detections: list = None) -> np.array:
+    def applyEcc(self, raw_frame: np.array) -> np.array:
         """
         Apply ECC algorithm to a raw frame.
 
         Args:
-            raw_frame (np.array): The raw frame to be processed.
-            detections (list): List of detections to be used in the processing.
+            raw_frame (np.ndarray): The raw frame to be processed.
 
         Returns:
-            (np.array): Processed frame.
+            (np.ndarray): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applyEcc(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -140,30 +139,30 @@
             self.initializedFirstFrame = True
 
             return H
 
         # Run the ECC algorithm. The results are stored in warp_matrix.
         # (cc, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria)
         try:
-            (cc, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria, None, 1)
+            (_, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria, None, 1)
         except Exception as e:
             LOGGER.warning(f"WARNING: find transform failed. Set warp as identity {e}")
 
         return H
 
     def applyFeatures(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply feature-based methods like ORB or SIFT to a raw frame.
 
         Args:
-            raw_frame (np.array): The raw frame to be processed.
+            raw_frame (np.ndarray): The raw frame to be processed.
             detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.array): Processed frame.
+            (np.ndarray): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applyFeatures(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -271,15 +270,15 @@
         #         matches_img = cv2.circle(matches_img, curr_pt, 2, tuple(color), -1)
         #
         #     plt.figure()
         #     plt.imshow(matches_img)
         #     plt.show()
 
         # Find rigid matrix
-        if (prevPoints.shape[0] > 4) and (prevPoints.shape[0] == prevPoints.shape[0]):
+        if prevPoints.shape[0] > 4:
             H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             # Handle downscale
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
@@ -288,24 +287,23 @@
         # Store to next iteration
         self.prevFrame = frame.copy()
         self.prevKeyPoints = copy.copy(keypoints)
         self.prevDescriptors = copy.copy(descriptors)
 
         return H
 
-    def applySparseOptFlow(self, raw_frame: np.array, detections: list = None) -> np.array:
+    def applySparseOptFlow(self, raw_frame: np.array) -> np.array:
         """
         Apply Sparse Optical Flow method to a raw frame.
 
         Args:
-            raw_frame (np.array): The raw frame to be processed.
-            detections (list): List of detections to be used in the processing.
+            raw_frame (np.ndarray): The raw frame to be processed.
 
         Returns:
-            (np.array): Processed frame.
+            (np.ndarray): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applySparseOptFlow(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -317,22 +315,22 @@
         if self.downscale > 1.0:
             frame = cv2.resize(frame, (width // self.downscale, height // self.downscale))
 
         # Find the keypoints
         keypoints = cv2.goodFeaturesToTrack(frame, mask=None, **self.feature_params)
 
         # Handle first frame
-        if not self.initializedFirstFrame:
+        if not self.initializedFirstFrame or self.prevKeyPoints is None:
             self.prevFrame = frame.copy()
             self.prevKeyPoints = copy.copy(keypoints)
             self.initializedFirstFrame = True
             return H
 
         # Find correspondences
-        matchedKeypoints, status, err = cv2.calcOpticalFlowPyrLK(self.prevFrame, frame, self.prevKeyPoints, None)
+        matchedKeypoints, status, _ = cv2.calcOpticalFlowPyrLK(self.prevFrame, frame, self.prevKeyPoints, None)
 
         # Leave good correspondences only
         prevPoints = []
         currPoints = []
 
         for i in range(len(status)):
             if status[i]:
@@ -340,15 +338,15 @@
                 currPoints.append(matchedKeypoints[i])
 
         prevPoints = np.array(prevPoints)
         currPoints = np.array(currPoints)
 
         # Find rigid matrix
         if (prevPoints.shape[0] > 4) and (prevPoints.shape[0] == prevPoints.shape[0]):
-            H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
+            H, _ = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
             LOGGER.warning("WARNING: not enough matching points")
```

### Comparing `ultralytics-8.1.9/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.0/ultralytics/trackers/utils/kalman_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         Create track from unassociated measurement.
 
         Args:
             measurement (ndarray): Bounding box coordinates (x, y, a, h) with center position (x, y), aspect ratio a,
                 and height h.
 
         Returns:
-            (tuple[ndarray, ndarray]): Returns the mean vector (8 dimensional) and covariance matrix (8x8 dimensional) of
-                the new track. Unobserved velocities are initialized to 0 mean.
+            (tuple[ndarray, ndarray]): Returns the mean vector (8 dimensional) and covariance matrix (8x8 dimensional)
+                of the new track. Unobserved velocities are initialized to 0 mean.
         """
         mean_pos = measurement
         mean_vel = np.zeros_like(mean_pos)
         mean = np.r_[mean_pos, mean_vel]
 
         std = [
             2 * self._std_weight_position * measurement[3],
@@ -231,16 +231,16 @@
         """
         Create track from unassociated measurement.
 
         Args:
             measurement (ndarray): Bounding box coordinates (x, y, w, h) with center position (x, y), width, and height.
 
         Returns:
-            (tuple[ndarray, ndarray]): Returns the mean vector (8 dimensional) and covariance matrix (8x8 dimensional) of
-                the new track. Unobserved velocities are initialized to 0 mean.
+            (tuple[ndarray, ndarray]): Returns the mean vector (8 dimensional) and covariance matrix (8x8 dimensional)
+                of the new track. Unobserved velocities are initialized to 0 mean.
         """
         mean_pos = measurement
         mean_vel = np.zeros_like(mean_pos)
         mean = np.r_[mean_pos, mean_vel]
 
         std = [
             2 * self._std_weight_position * measurement[2],
```

### Comparing `ultralytics-8.1.9/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.0/ultralytics/trackers/utils/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import numpy as np
 import scipy
 from scipy.spatial.distance import cdist
 
-from ultralytics.utils.metrics import bbox_ioa, batch_probiou
+from ultralytics.utils.metrics import batch_probiou, bbox_ioa
 
 try:
     import lap  # for linear_assignment
 
     assert lap.__version__  # verify package is not directory
 except (ImportError, AssertionError, AttributeError):
     from ultralytics.utils.checks import check_requirements
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/__init__.py` & `ultralytics-8.2.0/ultralytics/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
+import importlib.metadata
 import inspect
 import logging.config
 import os
 import platform
 import re
 import subprocess
 import sys
@@ -26,25 +27,28 @@
 from ultralytics import __version__
 
 # PyTorch Multi-GPU DDP Constants
 RANK = int(os.getenv("RANK", -1))
 LOCAL_RANK = int(os.getenv("LOCAL_RANK", -1))  # https://pytorch.org/docs/stable/elastic/run.html
 
 # Other Constants
+ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[1]  # YOLO
 ASSETS = ROOT / "assets"  # default images
 DEFAULT_CFG_PATH = ROOT / "cfg/default.yaml"
 NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLOv5 multiprocessing threads
 AUTOINSTALL = str(os.getenv("YOLO_AUTOINSTALL", True)).lower() == "true"  # global auto-install mode
 VERBOSE = str(os.getenv("YOLO_VERBOSE", True)).lower() == "true"  # global verbose mode
 TQDM_BAR_FORMAT = "{l_bar}{bar:10}{r_bar}" if VERBOSE else None  # tqdm bar format
 LOGGING_NAME = "ultralytics"
 MACOS, LINUX, WINDOWS = (platform.system() == x for x in ["Darwin", "Linux", "Windows"])  # environment booleans
-ARM64 = platform.machine() in ("arm64", "aarch64")  # ARM64 booleans
+ARM64 = platform.machine() in {"arm64", "aarch64"}  # ARM64 booleans
+PYTHON_VERSION = platform.python_version()
+TORCHVISION_VERSION = importlib.metadata.version("torchvision")  # faster than importing torchvision
 HELP_MSG = """
     Usage examples for running YOLOv8:
 
     1. Install the ultralytics package:
 
         pip install ultralytics
 
@@ -109,15 +113,15 @@
 
 class TQDM(tqdm_original):
     """
     Custom Ultralytics tqdm class with different default arguments.
 
     Args:
         *args (list): Positional arguments passed to original tqdm.
-        **kwargs (dict): Keyword arguments, with custom defaults applied.
+        **kwargs (any): Keyword arguments, with custom defaults applied.
     """
 
     def __init__(self, *args, **kwargs):
         """
         Initialize custom Ultralytics tqdm class with different default arguments.
 
         Note these can still be overridden when calling TQDM.
@@ -208,15 +212,15 @@
 
     def decorator(func):
         """Decorator to apply temporary rc parameters and backend to a function."""
 
         def wrapper(*args, **kwargs):
             """Sets rc parameters and backend, calls the original function, and restores the settings."""
             original_backend = plt.get_backend()
-            if backend != original_backend:
+            if backend.lower() != original_backend.lower():
                 plt.close("all")  # auto-close()ing of figures upon backend switching is deprecated since 3.8
                 plt.switch_backend(backend)
 
             with plt.rc_context(rcparams):
                 result = func(*args, **kwargs)
 
             if backend != original_backend:
@@ -225,45 +229,50 @@
             return result
 
         return wrapper
 
     return decorator
 
 
-def set_logging(name=LOGGING_NAME, verbose=True):
-    """Sets up logging for the given name with UTF-8 encoding support."""
+def set_logging(name="LOGGING_NAME", verbose=True):
+    """Sets up logging for the given name with UTF-8 encoding support, ensuring compatibility across different
+    environments.
+    """
     level = logging.INFO if verbose and RANK in {-1, 0} else logging.ERROR  # rank in world for Multi-GPU trainings
 
-    # Configure the console (stdout) encoding to UTF-8
+    # Configure the console (stdout) encoding to UTF-8, with checks for compatibility
     formatter = logging.Formatter("%(message)s")  # Default formatter
-    if WINDOWS and sys.stdout.encoding != "utf-8":
+    if WINDOWS and hasattr(sys.stdout, "encoding") and sys.stdout.encoding != "utf-8":
+
+        class CustomFormatter(logging.Formatter):
+            def format(self, record):
+                """Sets up logging with UTF-8 encoding and configurable verbosity."""
+                return emojis(super().format(record))
+
         try:
+            # Attempt to reconfigure stdout to use UTF-8 encoding if possible
             if hasattr(sys.stdout, "reconfigure"):
                 sys.stdout.reconfigure(encoding="utf-8")
+            # For environments where reconfigure is not available, wrap stdout in a TextIOWrapper
             elif hasattr(sys.stdout, "buffer"):
                 import io
 
                 sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
             else:
-                sys.stdout.encoding = "utf-8"
+                formatter = CustomFormatter("%(message)s")
         except Exception as e:
             print(f"Creating custom formatter for non UTF-8 environments due to {e}")
+            formatter = CustomFormatter("%(message)s")
 
-            class CustomFormatter(logging.Formatter):
-                def format(self, record):
-                    """Sets up logging with UTF-8 encoding and configurable verbosity."""
-                    return emojis(super().format(record))
-
-            formatter = CustomFormatter("%(message)s")  # Use CustomFormatter to eliminate UTF-8 output as last recourse
-
-    # Create and configure the StreamHandler
+    # Create and configure the StreamHandler with the appropriate formatter and level
     stream_handler = logging.StreamHandler(sys.stdout)
     stream_handler.setFormatter(formatter)
     stream_handler.setLevel(level)
 
+    # Set up the logger
     logger = logging.getLogger(name)
     logger.setLevel(level)
     logger.addHandler(stream_handler)
     logger.propagate = False
     return logger
 
 
@@ -354,15 +363,15 @@
     Args:
         file (str, optional): File name. Default is 'data.yaml'.
         append_filename (bool): Add the YAML filename to the YAML dictionary. Default is False.
 
     Returns:
         (dict): YAML data and file name.
     """
-    assert Path(file).suffix in (".yaml", ".yml"), f"Attempting to load non-YAML file {file} with yaml_load()"
+    assert Path(file).suffix in {".yaml", ".yml"}, f"Attempting to load non-YAML file {file} with yaml_load()"
     with open(file, errors="ignore", encoding="utf-8") as f:
         s = f.read()  # string
 
         # Remove special characters
         if not s.isprintable():
             s = re.sub(r"[^\x09\x0A\x0D\x20-\x7E\x85\xA0-\uD7FF\uE000-\uFFFD\U00010000-\U0010ffff]+", "", s)
 
@@ -393,14 +402,28 @@
 for k, v in DEFAULT_CFG_DICT.items():
     if isinstance(v, str) and v.lower() == "none":
         DEFAULT_CFG_DICT[k] = None
 DEFAULT_CFG_KEYS = DEFAULT_CFG_DICT.keys()
 DEFAULT_CFG = IterableSimpleNamespace(**DEFAULT_CFG_DICT)
 
 
+def read_device_model() -> str:
+    """
+    Reads the device model information from the system and caches it for quick access. Used by is_jetson() and
+    is_raspberrypi().
+
+    Returns:
+        (str): Model file contents if read successfully or empty string otherwise.
+    """
+    with contextlib.suppress(Exception):
+        with open("/proc/device-tree/model") as f:
+            return f.read()
+    return ""
+
+
 def is_ubuntu() -> bool:
     """
     Check if the OS is Ubuntu.
 
     Returns:
         (bool): True if OS is Ubuntu, False otherwise.
     """
@@ -447,46 +470,58 @@
 def is_docker() -> bool:
     """
     Determine if the script is running inside a Docker container.
 
     Returns:
         (bool): True if the script is running inside a Docker container, False otherwise.
     """
-    file = Path("/proc/self/cgroup")
-    if file.exists():
-        with open(file) as f:
+    with contextlib.suppress(Exception):
+        with open("/proc/self/cgroup") as f:
             return "docker" in f.read()
-    else:
-        return False
+    return False
+
+
+def is_raspberrypi() -> bool:
+    """
+    Determines if the Python environment is running on a Raspberry Pi by checking the device model information.
+
+    Returns:
+        (bool): True if running on a Raspberry Pi, False otherwise.
+    """
+    return "Raspberry Pi" in PROC_DEVICE_MODEL
+
+
+def is_jetson() -> bool:
+    """
+    Determines if the Python environment is running on a Jetson Nano or Jetson Orin device by checking the device model
+    information.
+
+    Returns:
+        (bool): True if running on a Jetson Nano or Jetson Orin, False otherwise.
+    """
+    return "NVIDIA" in PROC_DEVICE_MODEL  # i.e. "NVIDIA Jetson Nano" or "NVIDIA Orin NX"
 
 
 def is_online() -> bool:
     """
     Check internet connectivity by attempting to connect to a known online host.
 
     Returns:
         (bool): True if connection is successful, False otherwise.
     """
-    import socket
+    with contextlib.suppress(Exception):
+        assert str(os.getenv("YOLO_OFFLINE", "")).lower() != "true"  # check if ENV var YOLO_OFFLINE="True"
+        import socket
 
-    for host in "1.1.1.1", "8.8.8.8", "223.5.5.5":  # Cloudflare, Google, AliDNS:
-        try:
-            test_connection = socket.create_connection(address=(host, 53), timeout=2)
-        except (socket.timeout, socket.gaierror, OSError):
-            continue
-        else:
-            # If the connection was successful, close it to avoid a ResourceWarning
-            test_connection.close()
+        for dns in ("1.1.1.1", "8.8.8.8"):  # check Cloudflare and Google DNS
+            socket.create_connection(address=(dns, 80), timeout=1.0).close()
             return True
     return False
 
 
-ONLINE = is_online()
-
-
 def is_pip_package(filepath: str = __name__) -> bool:
     """
     Determines if the file at the given filepath is part of a pip package.
 
     Args:
         filepath (str): The filepath to check.
 
@@ -518,72 +553,72 @@
 def is_pytest_running():
     """
     Determines whether pytest is currently running or not.
 
     Returns:
         (bool): True if pytest is running, False otherwise.
     """
-    return ("PYTEST_CURRENT_TEST" in os.environ) or ("pytest" in sys.modules) or ("pytest" in Path(sys.argv[0]).stem)
+    return ("PYTEST_CURRENT_TEST" in os.environ) or ("pytest" in sys.modules) or ("pytest" in Path(ARGV[0]).stem)
 
 
 def is_github_action_running() -> bool:
     """
     Determine if the current environment is a GitHub Actions runner.
 
     Returns:
         (bool): True if the current environment is a GitHub Actions runner, False otherwise.
     """
     return "GITHUB_ACTIONS" in os.environ and "GITHUB_WORKFLOW" in os.environ and "RUNNER_OS" in os.environ
 
 
-def is_git_dir():
-    """
-    Determines whether the current file is part of a git repository. If the current file is not part of a git
-    repository, returns None.
-
-    Returns:
-        (bool): True if current file is part of a git repository.
-    """
-    return get_git_dir() is not None
-
-
 def get_git_dir():
     """
     Determines whether the current file is part of a git repository and if so, returns the repository root directory. If
     the current file is not part of a git repository, returns None.
 
     Returns:
         (Path | None): Git root directory if found or None if not found.
     """
     for d in Path(__file__).parents:
         if (d / ".git").is_dir():
             return d
 
 
+def is_git_dir():
+    """
+    Determines whether the current file is part of a git repository. If the current file is not part of a git
+    repository, returns None.
+
+    Returns:
+        (bool): True if current file is part of a git repository.
+    """
+    return GIT_DIR is not None
+
+
 def get_git_origin_url():
     """
     Retrieves the origin URL of a git repository.
 
     Returns:
         (str | None): The origin URL of the git repository or None if not git directory.
     """
-    if is_git_dir():
+    if IS_GIT_DIR:
         with contextlib.suppress(subprocess.CalledProcessError):
             origin = subprocess.check_output(["git", "config", "--get", "remote.origin.url"])
             return origin.decode().strip()
 
 
 def get_git_branch():
     """
     Returns the current git branch name. If not in a git repository, returns None.
 
     Returns:
         (str | None): The current git branch name or None if not a git directory.
     """
-    if is_git_dir():
+    if IS_GIT_DIR:
         with contextlib.suppress(subprocess.CalledProcessError):
             origin = subprocess.check_output(["git", "rev-parse", "--abbrev-ref", "HEAD"])
             return origin.decode().strip()
 
 
 def get_default_args(func):
     """
@@ -641,14 +676,26 @@
 
     # Create the subdirectory if it does not exist
     path.mkdir(parents=True, exist_ok=True)
 
     return path
 
 
+# Define constants (required below)
+PROC_DEVICE_MODEL = read_device_model()  # is_jetson() and is_raspberrypi() depend on this constant
+ONLINE = is_online()
+IS_COLAB = is_colab()
+IS_DOCKER = is_docker()
+IS_JETSON = is_jetson()
+IS_JUPYTER = is_jupyter()
+IS_KAGGLE = is_kaggle()
+IS_PIP_PACKAGE = is_pip_package()
+IS_RASPBERRYPI = is_raspberrypi()
+GIT_DIR = get_git_dir()
+IS_GIT_DIR = is_git_dir()
 USER_CONFIG_DIR = Path(os.getenv("YOLO_CONFIG_DIR") or get_user_config_dir())  # Ultralytics settings dir
 SETTINGS_YAML = USER_CONFIG_DIR / "settings.yaml"
 
 
 def colorstr(*input):
     """
     Colors a string based on the provided color and style arguments. Utilizes ANSI escape codes.
@@ -670,16 +717,16 @@
                        'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white'
         Misc: 'end', 'bold', 'underline'
 
     Returns:
         (str): The input string wrapped with ANSI escape codes for the specified color and style.
 
     Examples:
-        >>> colorstr('blue', 'bold', 'hello world')
-        >>> '\033[34m\033[1mhello world\033[0m'
+        >>> colorstr("blue", "bold", "hello world")
+        >>> "\033[34m\033[1mhello world\033[0m"
     """
     *args, string = input if len(input) > 1 else ("blue", "bold", input[0])  # color arguments, string
     colors = {
         "black": "\033[30m",  # basic colors
         "red": "\033[31m",
         "green": "\033[32m",
         "yellow": "\033[33m",
@@ -779,14 +826,15 @@
         self.delay = delay
         self._attempts = 0
 
     def __call__(self, func):
         """Decorator implementation for Retry with exponential backoff."""
 
         def wrapped_func(*args, **kwargs):
+            """Applies retries to the decorated function or method."""
             self._attempts = 0
             while self._attempts < self.times:
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     self._attempts += 1
                     print(f"Retry {self._attempts}/{self.times} failed: {e}")
@@ -860,33 +908,33 @@
             hint (dict): A dictionary containing additional information about the error.
 
         Returns:
             dict: The modified event or None if the event should not be sent to Sentry.
         """
         if "exc_info" in hint:
             exc_type, exc_value, tb = hint["exc_info"]
-            if exc_type in (KeyboardInterrupt, FileNotFoundError) or "out of memory" in str(exc_value):
+            if exc_type in {KeyboardInterrupt, FileNotFoundError} or "out of memory" in str(exc_value):
                 return None  # do not send event
 
         event["tags"] = {
-            "sys_argv": sys.argv[0],
-            "sys_argv_name": Path(sys.argv[0]).name,
-            "install": "git" if is_git_dir() else "pip" if is_pip_package() else "other",
+            "sys_argv": ARGV[0],
+            "sys_argv_name": Path(ARGV[0]).name,
+            "install": "git" if IS_GIT_DIR else "pip" if IS_PIP_PACKAGE else "other",
             "os": ENVIRONMENT,
         }
         return event
 
     if (
         SETTINGS["sync"]
-        and RANK in (-1, 0)
-        and Path(sys.argv[0]).name == "yolo"
+        and RANK in {-1, 0}
+        and Path(ARGV[0]).name == "yolo"
         and not TESTS_RUNNING
         and ONLINE
-        and is_pip_package()
-        and not is_git_dir()
+        and IS_PIP_PACKAGE
+        and not IS_GIT_DIR
     ):
         # If sentry_sdk package is not installed then return and do not use Sentry
         try:
             import sentry_sdk  # noqa
         except ImportError:
             return
 
@@ -917,17 +965,16 @@
         """
         import copy
         import hashlib
 
         from ultralytics.utils.checks import check_version
         from ultralytics.utils.torch_utils import torch_distributed_zero_first
 
-        git_dir = get_git_dir()
-        root = git_dir or Path()
-        datasets_root = (root.parent if git_dir and is_dir_writeable(root.parent) else root).resolve()
+        root = GIT_DIR or Path()
+        datasets_root = (root.parent if GIT_DIR and is_dir_writeable(root.parent) else root).resolve()
 
         self.file = Path(file)
         self.version = version
         self.defaults = {
             "settings_version": version,
             "datasets_dir": str(datasets_root / "datasets"),
             "weights_dir": str(root / "weights"),
@@ -953,23 +1000,33 @@
             if not self.file.exists():
                 self.save()
 
             self.load()
             correct_keys = self.keys() == self.defaults.keys()
             correct_types = all(type(a) is type(b) for a, b in zip(self.values(), self.defaults.values()))
             correct_version = check_version(self["settings_version"], self.version)
+            help_msg = (
+                f"\nView settings with 'yolo settings' or at '{self.file}'"
+                "\nUpdate settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'. "
+                "For help see https://docs.ultralytics.com/quickstart/#ultralytics-settings."
+            )
             if not (correct_keys and correct_types and correct_version):
                 LOGGER.warning(
                     "WARNING ⚠️ Ultralytics settings reset to default values. This may be due to a possible problem "
-                    "with your settings or a recent ultralytics package update. "
-                    f"\nView settings with 'yolo settings' or at '{self.file}'"
-                    "\nUpdate settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'."
+                    f"with your settings or a recent ultralytics package update. {help_msg}"
                 )
                 self.reset()
 
+            if self.get("datasets_dir") == self.get("runs_dir"):
+                LOGGER.warning(
+                    f"WARNING ⚠️ Ultralytics setting 'datasets_dir: {self.get('datasets_dir')}' "
+                    f"must be different than 'runs_dir: {self.get('runs_dir')}'. "
+                    f"Please change one to avoid possible issues during training. {help_msg}"
+                )
+
     def load(self):
         """Loads settings from the YAML file."""
         super().update(yaml_load(self.file))
 
     def save(self):
         """Saves the current settings to the YAML file."""
         yaml_save(self.file, dict(self))
@@ -1013,21 +1070,21 @@
 PREFIX = colorstr("Ultralytics: ")
 SETTINGS = SettingsManager()  # initialize settings
 DATASETS_DIR = Path(SETTINGS["datasets_dir"])  # global datasets directory
 WEIGHTS_DIR = Path(SETTINGS["weights_dir"])  # global weights directory
 RUNS_DIR = Path(SETTINGS["runs_dir"])  # global runs directory
 ENVIRONMENT = (
     "Colab"
-    if is_colab()
+    if IS_COLAB
     else "Kaggle"
-    if is_kaggle()
+    if IS_KAGGLE
     else "Jupyter"
-    if is_jupyter()
+    if IS_JUPYTER
     else "Docker"
-    if is_docker()
+    if IS_DOCKER
     else platform.system()
 )
 TESTS_RUNNING = is_pytest_running() or is_github_action_running()
 set_sentry()
 
 # Apply monkey patches
 from .patches import imread, imshow, imwrite, torch_save
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/autobatch.py` & `ultralytics-8.2.0/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.0/ultralytics/utils/benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 CoreML                  | `coreml`                  | yolov8n.mlpackage
 TensorFlow SavedModel   | `saved_model`             | yolov8n_saved_model/
 TensorFlow GraphDef     | `pb`                      | yolov8n.pb
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
-ncnn                    | `ncnn`                    | yolov8n_ncnn_model/
+NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
 """
 
 import glob
 import platform
 import time
 from pathlib import Path
 
 import numpy as np
 import torch.cuda
 
-from ultralytics import YOLO
+from ultralytics import YOLO, YOLOWorld
 from ultralytics.cfg import TASK2DATA, TASK2METRIC
 from ultralytics.engine.exporter import export_formats
-from ultralytics.utils import ASSETS, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
-from ultralytics.utils.checks import check_requirements, check_yolo
+from ultralytics.utils import ARM64, ASSETS, IS_JETSON, IS_RASPBERRYPI, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
+from ultralytics.utils.checks import IS_PYTHON_3_12, check_requirements, check_yolo
 from ultralytics.utils.files import file_size
 from ultralytics.utils.torch_utils import select_device
 
 
 def benchmark(
     model=WEIGHTS_DIR / "yolov8n.pt", data=None, imgsz=160, half=False, int8=False, device="cpu", verbose=False
 ):
@@ -65,35 +65,44 @@
     Example:
         ```python
         from ultralytics.utils.benchmarks import benchmark
 
         benchmark(model='yolov8n.pt', imgsz=640)
         ```
     """
-
-    import pandas as pd
+    import pandas as pd  # scope for faster 'import ultralytics'
 
     pd.options.display.max_columns = 10
     pd.options.display.width = 120
     device = select_device(device, verbose=False)
     if isinstance(model, (str, Path)):
         model = YOLO(model)
 
     y = []
     t0 = time.time()
     for i, (name, format, suffix, cpu, gpu) in export_formats().iterrows():  # index, (name, format, suffix, CPU, GPU)
         emoji, filename = "❌", None  # export defaults
         try:
             # Checks
-            if i == 9:
-                assert LINUX, "Edge TPU export only supported on Linux"
-            elif i == 7:
+            if i == 5:  # CoreML
+                assert not (IS_RASPBERRYPI or IS_JETSON), "CoreML export not supported on Raspberry Pi or NVIDIA Jetson"
+            if i == 9:  # Edge TPU
+                assert LINUX and not ARM64, "Edge TPU export only supported on non-aarch64 Linux"
+            elif i == 7:  # TF GraphDef
                 assert model.task != "obb", "TensorFlow GraphDef not supported for OBB task"
             elif i in {5, 10}:  # CoreML and TF.js
                 assert MACOS or LINUX, "export only supported on macOS and Linux"
+            if i in {3, 5}:  # CoreML and OpenVINO
+                assert not IS_PYTHON_3_12, "CoreML and OpenVINO not supported on Python 3.12"
+            if i in {6, 7, 8, 9, 10}:  # All TF formats
+                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 TensorFlow exports not supported by onnx2tf yet"
+            if i in {11}:  # Paddle
+                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 Paddle exports not supported yet"
+            if i in {12}:  # NCNN
+                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 NCNN exports not supported yet"
             if "cpu" in device.type:
                 assert cpu, "inference not supported on CPU"
             if "cuda" in device.type:
                 assert gpu, "inference not supported on GPU"
 
             # Export
             if format == "-":
@@ -103,15 +112,15 @@
                 filename = model.export(imgsz=imgsz, format=format, half=half, int8=int8, device=device, verbose=False)
                 exported_model = YOLO(filename, task=model.task)
                 assert suffix in str(filename), "export failed"
             emoji = "❎"  # indicates export succeeded
 
             # Predict
             assert model.task != "pose" or i != 7, "GraphDef Pose inference is not supported"
-            assert i not in (9, 10), "inference not supported"  # Edge TPU and TF.js are unsupported
+            assert i not in {9, 10}, "inference not supported"  # Edge TPU and TF.js are unsupported
             assert i != 5 or platform.system() == "Darwin", "inference only supported on macOS>=10.13"  # CoreML
             exported_model.predict(ASSETS / "bus.jpg", imgsz=imgsz, device=device, half=half)
 
             # Validate
             data = data or TASK2DATA[model.task]  # task to dataset, i.e. coco8.yaml for task=detect
             key = TASK2METRIC[model.task]  # task to metric, i.e. metrics/mAP50-95(B) for task=detect
             results = exported_model.val(
@@ -143,16 +152,15 @@
     return df
 
 
 class ProfileModels:
     """
     ProfileModels class for profiling different models on ONNX and TensorRT.
 
-    This class profiles the performance of different models, provided their paths. The profiling includes parameters such as
-    model speed and FLOPs.
+    This class profiles the performance of different models, returning results such as model speed and FLOPs.
 
     Attributes:
         paths (list): Paths of the models to profile.
         num_timed_runs (int): Number of timed runs for the profiling. Default is 100.
         num_warmup_runs (int): Number of warmup runs before profiling. Default is 10.
         min_time (float): Minimum number of seconds to profile for. Default is 60.
         imgsz (int): Image size used in the models. Default is 640.
@@ -184,17 +192,17 @@
 
         Args:
             paths (list): List of paths of the models to be profiled.
             num_timed_runs (int, optional): Number of timed runs for the profiling. Default is 100.
             num_warmup_runs (int, optional): Number of warmup runs before the actual profiling starts. Default is 10.
             min_time (float, optional): Minimum time in seconds for profiling a model. Default is 60.
             imgsz (int, optional): Size of the image used during profiling. Default is 640.
-            half (bool, optional): Flag to indicate whether to use half-precision floating point for profiling. Default is True.
+            half (bool, optional): Flag to indicate whether to use half-precision floating point for profiling.
             trt (bool, optional): Flag to indicate whether to profile using TensorRT. Default is True.
-            device (torch.device, optional): Device used for profiling. If None, it is determined automatically. Default is None.
+            device (torch.device, optional): Device used for profiling. If None, it is determined automatically.
         """
         self.paths = paths
         self.num_timed_runs = num_timed_runs
         self.num_warmup_runs = num_warmup_runs
         self.min_time = min_time
         self.imgsz = imgsz
         self.half = half
@@ -209,15 +217,15 @@
             print("No matching *.pt or *.onnx files found.")
             return
 
         table_rows = []
         output = []
         for file in files:
             engine_file = file.with_suffix(".engine")
-            if file.suffix in (".pt", ".yaml", ".yml"):
+            if file.suffix in {".pt", ".yaml", ".yml"}:
                 model = YOLO(str(file))
                 model.fuse()  # to report correct params and GFLOPs in model.info()
                 model_info = model.info()
                 if self.trt and self.device.type != "cpu" and not engine_file.is_file():
                     engine_file = model.export(
                         format="engine", half=self.half, imgsz=self.imgsz, device=self.device, verbose=False
                     )
@@ -256,15 +264,16 @@
 
     def get_onnx_model_info(self, onnx_file: str):
         """Retrieves the information including number of layers, parameters, gradients and FLOPs for an ONNX model
         file.
         """
         return 0.0, 0.0, 0.0, 0.0  # return (num_layers, num_params, num_gradients, num_flops)
 
-    def iterative_sigma_clipping(self, data, sigma=2, max_iters=3):
+    @staticmethod
+    def iterative_sigma_clipping(data, sigma=2, max_iters=3):
         """Applies an iterative sigma clipping algorithm to the given data times number of iterations."""
         data = np.array(data)
         for _ in range(max_iters):
             mean, std = np.mean(data), np.std(data)
             clipped_data = data[(data > mean - sigma * std) & (data < mean + sigma * std)]
             if len(clipped_data) == len(data):
                 break
@@ -354,30 +363,41 @@
 
         run_times = self.iterative_sigma_clipping(np.array(run_times), sigma=2, max_iters=5)  # sigma clipping
         return np.mean(run_times), np.std(run_times)
 
     def generate_table_row(self, model_name, t_onnx, t_engine, model_info):
         """Generates a formatted string for a table row that includes model performance and metric details."""
         layers, params, gradients, flops = model_info
-        return f"| {model_name:18s} | {self.imgsz} | - | {t_onnx[0]:.2f} ± {t_onnx[1]:.2f} ms | {t_engine[0]:.2f} ± {t_engine[1]:.2f} ms | {params / 1e6:.1f} | {flops:.1f} |"
+        return (
+            f"| {model_name:18s} | {self.imgsz} | - | {t_onnx[0]:.2f} ± {t_onnx[1]:.2f} ms | {t_engine[0]:.2f} ± "
+            f"{t_engine[1]:.2f} ms | {params / 1e6:.1f} | {flops:.1f} |"
+        )
 
-    def generate_results_dict(self, model_name, t_onnx, t_engine, model_info):
+    @staticmethod
+    def generate_results_dict(model_name, t_onnx, t_engine, model_info):
         """Generates a dictionary of model details including name, parameters, GFLOPS and speed metrics."""
         layers, params, gradients, flops = model_info
         return {
             "model/name": model_name,
             "model/parameters": params,
             "model/GFLOPs": round(flops, 3),
             "model/speed_ONNX(ms)": round(t_onnx[0], 3),
             "model/speed_TensorRT(ms)": round(t_engine[0], 3),
         }
 
-    def print_table(self, table_rows):
+    @staticmethod
+    def print_table(table_rows):
         """Formats and prints a comparison table for different models with given statistics and performance data."""
         gpu = torch.cuda.get_device_name(0) if torch.cuda.is_available() else "GPU"
-        header = f"| Model | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>{gpu} TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |"
-        separator = "|-------------|---------------------|--------------------|------------------------------|-----------------------------------|------------------|-----------------|"
+        header = (
+            f"| Model | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | "
+            f"Speed<br><sup>{gpu} TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |"
+        )
+        separator = (
+            "|-------------|---------------------|--------------------|------------------------------|"
+            "-----------------------------------|------------------|-----------------|"
+        )
 
         print(f"\n\n{header}")
         print(separator)
         for row in table_rows:
             print(row)
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 """Base callbacks."""
 
 from collections import defaultdict
 from copy import deepcopy
 
-
 # Trainer callbacks ----------------------------------------------------------------------------------------------------
 
 
 def on_pretrain_routine_start(trainer):
     """Called before the pretraining routine starts."""
     pass
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/clearml.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from ultralytics.utils import LOGGER, SETTINGS, TESTS_RUNNING
 
 try:
     assert not TESTS_RUNNING  # do not log pytest
     assert SETTINGS["clearml"] is True  # verify integration is enabled
     import clearml
     from clearml import Task
-    from clearml.binding.frameworks.pytorch_bind import PatchPyTorchModelIO
-    from clearml.binding.matplotlib_bind import PatchedMatplotlib
 
     assert hasattr(clearml, "__version__")  # verify package is not directory
 
 except (ImportError, AssertionError):
     clearml = None
 
 
@@ -57,16 +55,19 @@
     )
 
 
 def on_pretrain_routine_start(trainer):
     """Runs at start of pretraining routine; initializes and connects/ logs task to ClearML."""
     try:
         if task := Task.current_task():
-            # Make sure the automatic pytorch and matplotlib bindings are disabled!
+            # WARNING: make sure the automatic pytorch and matplotlib bindings are disabled!
             # We are logging these plots and model files manually in the integration
+            from clearml.binding.frameworks.pytorch_bind import PatchPyTorchModelIO
+            from clearml.binding.matplotlib_bind import PatchedMatplotlib
+
             PatchPyTorchModelIO.update_current_task(None)
             PatchedMatplotlib.update_current_task(None)
         else:
             task = Task.init(
                 project_name=trainer.args.project or "YOLOv8",
                 task_name=trainer.args.name,
                 tags=["YOLOv8"],
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/comet.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return comet_ml.OfflineExperiment(project_name=project_name)
 
     return comet_ml.Experiment(project_name=project_name)
 
 
 def _create_experiment(args):
     """Ensures that the experiment object is only created in a single process during distributed training."""
-    if RANK not in (-1, 0):
+    if RANK not in {-1, 0}:
         return
     try:
         comet_mode = _get_comet_mode()
         _project_name = os.getenv("COMET_PROJECT_NAME", args.project)
         experiment = _get_experiment_type(comet_mode, _project_name)
         experiment.log_parameters(vars(args))
         experiment.log_others(
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 
 
 def on_pretrain_routine_end(trainer):
     """Logs info before starting timer for upload rate limit."""
     session = getattr(trainer, "hub_session", None)
     if session:
         # Start timer for upload rate limit
-        session.timers = {
-            "metrics": time(),
-            "ckpt": time(),
-        }  # start timer on session.rate_limit
+        session.timers = {"metrics": time(), "ckpt": time()}  # start timer on session.rate_limit
 
 
 def on_fit_epoch_end(trainer):
     """Uploads training progress metrics at the end of each epoch."""
     session = getattr(trainer, "hub_session", None)
     if session:
         # Upload metrics after val end
@@ -29,28 +26,33 @@
         }
         if trainer.epoch == 0:
             from ultralytics.utils.torch_utils import model_info_for_loggers
 
             all_plots = {**all_plots, **model_info_for_loggers(trainer)}
 
         session.metrics_queue[trainer.epoch] = json.dumps(all_plots)
+
+        # If any metrics fail to upload, add them to the queue to attempt uploading again.
+        if session.metrics_upload_failed_queue:
+            session.metrics_queue.update(session.metrics_upload_failed_queue)
+
         if time() - session.timers["metrics"] > session.rate_limits["metrics"]:
             session.upload_metrics()
             session.timers["metrics"] = time()  # reset timer
             session.metrics_queue = {}  # reset queue
 
 
 def on_model_save(trainer):
     """Saves checkpoints to Ultralytics HUB with rate limiting."""
     session = getattr(trainer, "hub_session", None)
     if session:
         # Upload checkpoints with rate limiting
         is_best = trainer.best_fitness == trainer.fitness
         if time() - session.timers["ckpt"] > session.rate_limits["ckpt"]:
-            LOGGER.info(f"{PREFIX}Uploading checkpoint {HUB_WEB_ROOT}/models/{session.model_id}")
+            LOGGER.info(f"{PREFIX}Uploading checkpoint {HUB_WEB_ROOT}/models/{session.model.id}")
             session.upload_model(trainer.epoch, trainer.last, is_best)
             session.timers["ckpt"] = time()  # reset timer
 
 
 def on_train_end(trainer):
     """Upload final model and metrics to Ultralytics HUB at the end of training."""
     session = getattr(trainer, "hub_session", None)
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/mlflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     Global:
         mlflow: The imported mlflow module to use for logging.
 
     Environment Variables:
         MLFLOW_TRACKING_URI: The URI for MLflow tracking. If not set, defaults to 'runs/mlflow'.
         MLFLOW_EXPERIMENT_NAME: The name of the MLflow experiment. If not set, defaults to trainer.args.project.
         MLFLOW_RUN: The name of the MLflow run. If not set, defaults to trainer.args.name.
+        MLFLOW_KEEP_RUN_ACTIVE: Boolean indicating whether to keep the MLflow run active after the end of training.
     """
     global mlflow
 
     uri = os.environ.get("MLFLOW_TRACKING_URI") or str(RUNS_DIR / "mlflow")
     LOGGER.debug(f"{PREFIX} tracking uri: {uri}")
     mlflow.set_tracking_uri(uri)
 
@@ -82,17 +83,20 @@
         LOGGER.warning(f"{PREFIX}WARNING ⚠️ Failed to initialize: {e}\n" f"{PREFIX}WARNING ⚠️ Not tracking this run")
 
 
 def on_train_epoch_end(trainer):
     """Log training metrics at the end of each train epoch to MLflow."""
     if mlflow:
         mlflow.log_metrics(
-            metrics=SANITIZE(trainer.label_loss_items(trainer.tloss, prefix="train")), step=trainer.epoch
+            metrics={
+                **SANITIZE(trainer.lr),
+                **SANITIZE(trainer.label_loss_items(trainer.tloss, prefix="train")),
+            },
+            step=trainer.epoch,
         )
-        mlflow.log_metrics(metrics=SANITIZE(trainer.lr), step=trainer.epoch)
 
 
 def on_fit_epoch_end(trainer):
     """Log training metrics at the end of each fit epoch to MLflow."""
     if mlflow:
         mlflow.log_metrics(metrics=SANITIZE(trainer.metrics), step=trainer.epoch)
 
@@ -100,24 +104,30 @@
 def on_train_end(trainer):
     """Log model artifacts at the end of the training."""
     if mlflow:
         mlflow.log_artifact(str(trainer.best.parent))  # log save_dir/weights directory with best.pt and last.pt
         for f in trainer.save_dir.glob("*"):  # log all other files in save_dir
             if f.suffix in {".png", ".jpg", ".csv", ".pt", ".yaml"}:
                 mlflow.log_artifact(str(f))
+        keep_run_active = os.environ.get("MLFLOW_KEEP_RUN_ACTIVE", "False").lower() == "true"
+        if keep_run_active:
+            LOGGER.info(f"{PREFIX}mlflow run still alive, remember to close it using mlflow.end_run()")
+        else:
+            mlflow.end_run()
+            LOGGER.debug(f"{PREFIX}mlflow run ended")
 
-        mlflow.end_run()
         LOGGER.info(
             f"{PREFIX}results logged to {mlflow.get_tracking_uri()}\n"
             f"{PREFIX}disable with 'yolo settings mlflow=False'"
         )
 
 
 callbacks = (
     {
         "on_pretrain_routine_end": on_pretrain_routine_end,
+        "on_train_epoch_end": on_train_epoch_end,
         "on_fit_epoch_end": on_fit_epoch_end,
         "on_train_end": on_train_end,
     }
     if mlflow
     else {}
 )
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/raytune.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 except (ImportError, AssertionError):
     tune = None
 
 
 def on_fit_epoch_end(trainer):
     """Sends training metrics to Ray Tune at end of each epoch."""
-    if ray.tune.is_session_enabled():
+    if ray.train._internal.session._get_session():  # replacement for deprecated ray.tune.is_session_enabled()
         metrics = trainer.metrics
         metrics["epoch"] = trainer.epoch
         session.report(metrics)
 
 
 callbacks = (
     {
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     assert SETTINGS["tensorboard"] is True  # verify integration is enabled
     WRITER = None  # TensorBoard SummaryWriter instance
     PREFIX = colorstr("TensorBoard: ")
 
     # Imports below only required if TensorBoard enabled
     import warnings
     from copy import deepcopy
+
     from ultralytics.utils.torch_utils import de_parallel, torch
 
 except (ImportError, AssertionError, TypeError, AttributeError):
     # TypeError for handling 'Descriptors cannot not be created directly.' protobuf errors in Windows
     # AttributeError: module 'tensorflow' has no attribute 'io' if 'tensorflow' not installed
     SummaryWriter = None
 
@@ -41,14 +42,15 @@
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)  # suppress jit trace warning
         warnings.simplefilter("ignore", category=torch.jit.TracerWarning)  # suppress jit trace warning
 
         # Try simple method first (YOLO)
         with contextlib.suppress(Exception):
+            trainer.model.eval()  # place in .eval() mode to avoid BatchNorm statistics changes
             WRITER.add_graph(torch.jit.trace(de_parallel(trainer.model), im, strict=False), [])
             LOGGER.info(f"{PREFIX}model graph visualization added ✅")
             return
 
         # Fallback to TorchScript export steps (RTDETR)
         try:
             model = deepcopy(de_parallel(trainer.model))
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.0/ultralytics/utils/callbacks/wb.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 
 try:
     assert not TESTS_RUNNING  # do not log pytest
     assert SETTINGS["wandb"] is True  # verify integration is enabled
     import wandb as wb
 
     assert hasattr(wb, "__version__")  # verify package is not directory
-
-    import numpy as np
-    import pandas as pd
-
     _processed_plots = {}
 
 except (ImportError, AssertionError):
     wb = None
 
 
 def _custom_table(x, y, classes, title="Precision Recall Curve", x_title="Recall", y_title="Precision"):
     """
     Create and log a custom metric visualization to wandb.plot.pr_curve.
 
-    This function crafts a custom metric visualization that mimics the behavior of wandb's default precision-recall curve
-    while allowing for enhanced customization. The visual metric is useful for monitoring model performance across different classes.
+    This function crafts a custom metric visualization that mimics the behavior of wandb's default precision-recall
+    curve while allowing for enhanced customization. The visual metric is useful for monitoring model performance across
+    different classes.
 
     Args:
         x (List): Values for the x-axis; expected to have length N.
         y (List): Corresponding values for the y-axis; also expected to have length N.
         classes (List): Labels identifying the class of each point; length N.
         title (str, optional): Title for the plot; defaults to 'Precision Recall Curve'.
         x_title (str, optional): Label for the x-axis; defaults to 'Recall'.
         y_title (str, optional): Label for the y-axis; defaults to 'Precision'.
 
     Returns:
         (wandb.Object): A wandb object suitable for logging, showcasing the crafted metric visualization.
     """
-    df = pd.DataFrame({"class": classes, "y": y, "x": x}).round(3)
+    import pandas  # scope for faster 'import ultralytics'
+
+    df = pandas.DataFrame({"class": classes, "y": y, "x": x}).round(3)
     fields = {"x": "x", "y": "y", "class": "class"}
     string_fields = {"title": title, "x-axis-title": x_title, "y-axis-title": y_title}
     return wb.plot_table(
         "wandb/area-under-curve/v0", wb.Table(dataframe=df), fields=fields, string_fields=string_fields
     )
 
 
@@ -60,26 +59,28 @@
     Log a metric curve visualization.
 
     This function generates a metric curve based on input data and logs the visualization to wandb.
     The curve can represent aggregated data (mean) or individual class data, depending on the 'only_mean' flag.
 
     Args:
         x (np.ndarray): Data points for the x-axis with length N.
-        y (np.ndarray): Corresponding data points for the y-axis with shape CxN, where C represents the number of classes.
-        names (list, optional): Names of the classes corresponding to the y-axis data; length C. Defaults to an empty list.
+        y (np.ndarray): Corresponding data points for the y-axis with shape CxN, where C is the number of classes.
+        names (list, optional): Names of the classes corresponding to the y-axis data; length C. Defaults to [].
         id (str, optional): Unique identifier for the logged data in wandb. Defaults to 'precision-recall'.
         title (str, optional): Title for the visualization plot. Defaults to 'Precision Recall Curve'.
         x_title (str, optional): Label for the x-axis. Defaults to 'Recall'.
         y_title (str, optional): Label for the y-axis. Defaults to 'Precision'.
         num_x (int, optional): Number of interpolated data points for visualization. Defaults to 100.
         only_mean (bool, optional): Flag to indicate if only the mean curve should be plotted. Defaults to True.
 
     Note:
         The function leverages the '_custom_table' function to generate the actual visualization.
     """
+    import numpy as np
+
     # Create new x
     if names is None:
         names = []
     x_new = np.linspace(x[0], x[-1], num_x).round(5)
 
     # Create arrays for logging
     x_log = x_new.tolist()
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/checks.py` & `ultralytics-8.2.0/ultralytics/utils/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 import inspect
 import math
 import os
 import platform
 import re
 import shutil
 import subprocess
-import sys
 import time
 from importlib import metadata
 from pathlib import Path
 from typing import Optional
 
 import cv2
 import numpy as np
 import requests
 import torch
-from matplotlib import font_manager
 
 from ultralytics.utils import (
     ASSETS,
     AUTOINSTALL,
+    IS_COLAB,
+    IS_DOCKER,
+    IS_JUPYTER,
+    IS_KAGGLE,
+    IS_PIP_PACKAGE,
     LINUX,
     LOGGER,
     ONLINE,
+    PYTHON_VERSION,
     ROOT,
+    TORCHVISION_VERSION,
     USER_CONFIG_DIR,
+    Retry,
     SimpleNamespace,
     ThreadingLocked,
     TryExcept,
     clean_url,
     colorstr,
     downloads,
     emojis,
-    is_colab,
-    is_docker,
     is_github_action_running,
-    is_jupyter,
-    is_kaggle,
-    is_online,
-    is_pip_package,
     url2file,
 )
 
 
 def parse_requirements(file_path=ROOT.parent / "requirements.txt", package=""):
     """
     Parse a requirements.txt file, ignoring lines that start with '#' and any text after '#'.
@@ -137,14 +137,16 @@
     stride = int(stride.max() if isinstance(stride, torch.Tensor) else stride)
 
     # Convert image size to list if it is an integer
     if isinstance(imgsz, int):
         imgsz = [imgsz]
     elif isinstance(imgsz, (list, tuple)):
         imgsz = list(imgsz)
+    elif isinstance(imgsz, str):  # i.e. '640' or '[640,640]'
+        imgsz = [int(imgsz)] if imgsz.isnumeric() else eval(imgsz)
     else:
         raise TypeError(
             f"'imgsz={imgsz}' is of invalid type {type(imgsz).__name__}. "
             f"Valid imgsz types are int i.e. 'imgsz=640' or list i.e. 'imgsz=[640,640]'"
         )
 
     # Apply max_dim
@@ -230,15 +232,15 @@
     for r in required.strip(",").split(","):
         op, version = re.match(r"([^0-9]*)([\d.]+)", r).groups()  # split '>=22.04' -> ('>=', '22.04')
         v = parse_version(version)  # '1.2.3' -> (1, 2, 3)
         if op == "==" and c != v:
             result = False
         elif op == "!=" and c == v:
             result = False
-        elif op in (">=", "") and not (c >= v):  # if no constraint passed assume '>=required'
+        elif op in {">=", ""} and not (c >= v):  # if no constraint passed assume '>=required'
             result = False
         elif op == "<=" and not (c <= v):
             result = False
         elif op == ">" and not (c > v):
             result = False
         elif op == "<" and not (c < v):
             result = False
@@ -271,15 +273,15 @@
 def check_pip_update_available():
     """
     Checks if a new version of the ultralytics package is available on PyPI.
 
     Returns:
         (bool): True if an update is available, False otherwise.
     """
-    if ONLINE and is_pip_package():
+    if ONLINE and IS_PIP_PACKAGE:
         with contextlib.suppress(Exception):
             from ultralytics import __version__
 
             latest = check_latest_pypi_version()
             if check_version(__version__, f"<{latest}"):  # check if current version is < latest version
                 LOGGER.info(
                     f"New https://pypi.org/project/ultralytics/{latest} available 😃 "
@@ -296,44 +298,45 @@
 
     Args:
         font (str): Path or name of font.
 
     Returns:
         file (Path): Resolved font file path.
     """
-    name = Path(font).name
+    from matplotlib import font_manager
 
     # Check USER_CONFIG_DIR
+    name = Path(font).name
     file = USER_CONFIG_DIR / name
     if file.exists():
         return file
 
     # Check system fonts
     matches = [s for s in font_manager.findSystemFonts() if font in s]
     if any(matches):
         return matches[0]
 
     # Download to USER_CONFIG_DIR if missing
     url = f"https://ultralytics.com/assets/{name}"
-    if downloads.is_url(url):
+    if downloads.is_url(url, check=True):
         downloads.safe_download(url=url, file=file)
         return file
 
 
 def check_python(minimum: str = "3.8.0") -> bool:
     """
     Check current python version against the required minimum version.
 
     Args:
         minimum (str): Required minimum version of python.
 
     Returns:
         (bool): Whether the installed Python version meets the minimum constraints.
     """
-    return check_version(platform.python_version(), minimum, name="Python ", hard=True)
+    return check_version(PYTHON_VERSION, minimum, name="Python ", hard=True)
 
 
 @TryExcept()
 def check_requirements(requirements=ROOT.parent / "requirements.txt", exclude=(), install=True, cmds=""):
     """
     Check if installed dependencies meet YOLOv8 requirements and attempt to auto-update if needed.
 
@@ -382,16 +385,17 @@
     s = " ".join(f'"{x}"' for x in pkgs)  # console string
     if s:
         if install and AUTOINSTALL:  # check environment variable
             n = len(pkgs)  # number of packages updates
             LOGGER.info(f"{prefix} Ultralytics requirement{'s' * (n > 1)} {pkgs} not found, attempting AutoUpdate...")
             try:
                 t = time.time()
-                assert is_online(), "AutoUpdate skipped (offline)"
-                LOGGER.info(subprocess.check_output(f"pip install --no-cache {s} {cmds}", shell=True).decode())
+                assert ONLINE, "AutoUpdate skipped (offline)"
+                with Retry(times=2, delay=1):  # run up to 2 times with 1-second retry delay
+                    LOGGER.info(subprocess.check_output(f"pip install --no-cache {s} {cmds}", shell=True).decode())
                 dt = time.time() - t
                 LOGGER.info(
                     f"{prefix} AutoUpdate success ✅ {dt:.1f}s, installed {n} package{'s' * (n > 1)}: {pkgs}\n"
                     f"{prefix} ⚠️ {colorstr('bold', 'Restart runtime or rerun command for updates to take effect')}\n"
                 )
             except Exception as e:
                 LOGGER.warning(f"{prefix} ❌ {e}")
@@ -410,22 +414,20 @@
     to the provided compatibility table based on:
     https://github.com/pytorch/vision#installation.
 
     The compatibility table is a dictionary where the keys are PyTorch versions and the values are lists of compatible
     Torchvision versions.
     """
 
-    import torchvision
-
     # Compatibility table
     compatibility_table = {"2.0": ["0.15"], "1.13": ["0.14"], "1.12": ["0.13"]}
 
     # Extract only the major and minor versions
     v_torch = ".".join(torch.__version__.split("+")[0].split(".")[:2])
-    v_torchvision = ".".join(torchvision.__version__.split("+")[0].split(".")[:2])
+    v_torchvision = ".".join(TORCHVISION_VERSION.split("+")[0].split(".")[:2])
 
     if v_torch in compatibility_table:
         compatible_versions = compatibility_table[v_torch]
         if all(v_torchvision != v for v in compatible_versions):
             print(
                 f"WARNING ⚠️ torchvision=={v_torchvision} is incompatible with torch=={v_torch}.\n"
                 f"Run 'pip install torchvision=={compatible_versions[0]}' to fix torchvision or "
@@ -488,15 +490,15 @@
         file = url2file(file)  # '%2F' to '/', split https://url.com/file.txt?auth
         if Path(file).exists():
             LOGGER.info(f"Found {clean_url(url)} locally at {file}")  # file already exists
         else:
             downloads.safe_download(url=url, file=file, unzip=False)
         return file
     else:  # search
-        files = glob.glob(str(ROOT / "cfg" / "**" / file), recursive=True)  # find file
+        files = glob.glob(str(ROOT / "**" / file), recursive=True) or glob.glob(str(ROOT.parent / file))  # find file
         if not files and hard:
             raise FileNotFoundError(f"'{file}' does not exist")
         elif len(files) > 1 and hard:
             raise FileNotFoundError(f"Multiple files match '{file}', specify exact path: {files}")
         return files[0] if len(files) else []  # return file
 
 
@@ -522,15 +524,15 @@
     return path_resolved.is_file() and path_resolved.parts[: len(base_dir_resolved.parts)] == base_dir_resolved.parts
 
 
 def check_imshow(warn=False):
     """Check if environment supports image displays."""
     try:
         if LINUX:
-            assert "DISPLAY" in os.environ and not is_docker() and not is_colab() and not is_kaggle()
+            assert "DISPLAY" in os.environ and not IS_DOCKER and not IS_COLAB and not IS_KAGGLE
         cv2.imshow("test", np.zeros((8, 8, 3), dtype=np.uint8))  # show a small 8-pixel image
         cv2.waitKey(1)
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         return True
     except Exception as e:
         if warn:
@@ -540,18 +542,18 @@
 
 def check_yolo(verbose=True, device=""):
     """Return a human-readable YOLO software and hardware summary."""
     import psutil
 
     from ultralytics.utils.torch_utils import select_device
 
-    if is_jupyter():
+    if IS_JUPYTER:
         if check_requirements("wandb", install=False):
             os.system("pip uninstall -y wandb")  # uninstall wandb: unwanted account creation prompt with infinite hang
-        if is_colab():
+        if IS_COLAB:
             shutil.rmtree("sample_data", ignore_errors=True)  # remove colab /sample_data directory
 
     if verbose:
         # System info
         gib = 1 << 30  # bytes per GiB
         ram = psutil.virtual_memory().total
         total, used, free = shutil.disk_usage("/")
@@ -568,24 +570,24 @@
 
 
 def collect_system_info():
     """Collect and print relevant system information including OS, Python, RAM, CPU, and CUDA."""
 
     import psutil
 
-    from ultralytics.utils import ENVIRONMENT, is_git_dir
+    from ultralytics.utils import ENVIRONMENT, IS_GIT_DIR
     from ultralytics.utils.torch_utils import get_cpu_info
 
     ram_info = psutil.virtual_memory().total / (1024**3)  # Convert bytes to GB
     check_yolo()
     LOGGER.info(
         f"\n{'OS':<20}{platform.platform()}\n"
         f"{'Environment':<20}{ENVIRONMENT}\n"
-        f"{'Python':<20}{sys.version.split()[0]}\n"
-        f"{'Install':<20}{'git' if is_git_dir() else 'pip' if is_pip_package() else 'other'}\n"
+        f"{'Python':<20}{PYTHON_VERSION}\n"
+        f"{'Install':<20}{'git' if IS_GIT_DIR else 'pip' if IS_PIP_PACKAGE else 'other'}\n"
         f"{'RAM':<20}{ram_info:.2f} GB\n"
         f"{'CPU':<20}{get_cpu_info()}\n"
         f"{'CUDA':<20}{torch.version.cuda if torch and torch.cuda.is_available() else None}\n"
     )
 
     for r in parse_requirements(package="ultralytics"):
         try:
@@ -625,15 +627,15 @@
         check_amp(model)
         ```
 
     Returns:
         (bool): Returns True if the AMP functionality works correctly with YOLOv8 model, else False.
     """
     device = next(model.parameters()).device  # get model device
-    if device.type in ("cpu", "mps"):
+    if device.type in {"cpu", "mps"}:
         return False  # AMP only used on CUDA devices
 
     def amp_allclose(m, im):
         """All close FP32 vs AMP results."""
         a = m(im, device=device, verbose=False)[0].boxes.data  # FP32 inference
         with torch.cuda.amp.autocast(True):
             b = m(im, device=device, verbose=False)[0].boxes.data  # AMP inference
@@ -718,7 +720,11 @@
     """
     Check if CUDA is available in the environment.
 
     Returns:
         (bool): True if one or more NVIDIA GPUs are available, False otherwise.
     """
     return cuda_device_count() > 0
+
+
+# Define constants
+IS_PYTHON_3_12 = PYTHON_VERSION.startswith("3.12")
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/dist.py` & `ultralytics-8.2.0/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/downloads.py` & `ultralytics-8.2.0/ultralytics/utils/downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,34 +16,38 @@
 
 # Define Ultralytics GitHub assets maintained at https://github.com/ultralytics/assets
 GITHUB_ASSETS_REPO = "ultralytics/assets"
 GITHUB_ASSETS_NAMES = (
     [f"yolov8{k}{suffix}.pt" for k in "nsmlx" for suffix in ("", "-cls", "-seg", "-pose", "-obb")]
     + [f"yolov5{k}{resolution}u.pt" for k in "nsmlx" for resolution in ("", "6")]
     + [f"yolov3{k}u.pt" for k in ("", "-spp", "-tiny")]
+    + [f"yolov8{k}-world.pt" for k in "smlx"]
+    + [f"yolov8{k}-worldv2.pt" for k in "smlx"]
+    + [f"yolov9{k}.pt" for k in "ce"]
     + [f"yolo_nas_{k}.pt" for k in "sml"]
     + [f"sam_{k}.pt" for k in "bl"]
     + [f"FastSAM-{k}.pt" for k in "sx"]
     + [f"rtdetr-{k}.pt" for k in "lx"]
     + ["mobile_sam.pt"]
+    + ["calibration_image_sample_data_20x128x128x3_float32.npy.zip"]
 )
 GITHUB_ASSETS_STEMS = [Path(k).stem for k in GITHUB_ASSETS_NAMES]
 
 
-def is_url(url, check=True):
+def is_url(url, check=False):
     """
     Validates if the given string is a URL and optionally checks if the URL exists online.
 
     Args:
         url (str): The string to be validated as a URL.
         check (bool, optional): If True, performs an additional check to see if the URL exists online.
             Defaults to True.
 
     Returns:
-        (bool): Returns True if the string is a valid URL. If 'check' is True, also returns True if the URL exists online.
+        (bool): Returns True for a valid URL. If 'check' is True, also returns True if the URL exists online.
             Returns False otherwise.
 
     Example:
         ```python
         valid = is_url("https://www.example.com")
         ```
     """
@@ -183,20 +187,21 @@
                 LOGGER.warning(f"Potentially insecure file path: {f}, skipping extraction.")
                 continue
             zipObj.extract(f, extract_path)
 
     return path  # return unzip dir
 
 
-def check_disk_space(url="https://ultralytics.com/assets/coco128.zip", sf=1.5, hard=True):
+def check_disk_space(url="https://ultralytics.com/assets/coco128.zip", path=Path.cwd(), sf=1.5, hard=True):
     """
     Check if there is sufficient disk space to download and store a file.
 
     Args:
         url (str, optional): The URL to the file. Defaults to 'https://ultralytics.com/assets/coco128.zip'.
+        path (str | Path, optional): The path or drive to check the available free space on.
         sf (float, optional): Safety factor, the multiplier for the required free space. Defaults to 2.0.
         hard (bool, optional): Whether to throw an error or not on insufficient disk space. Defaults to True.
 
     Returns:
         (bool): True if there is sufficient disk space, False otherwise.
     """
     try:
@@ -204,15 +209,15 @@
         assert r.status_code < 400, f"URL error for {url}: {r.status_code} {r.reason}"  # check response
     except Exception:
         return True  # requests issue, default to True
 
     # Check file size
     gib = 1 << 30  # bytes per GiB
     data = int(r.headers.get("Content-Length", 0)) / gib  # file size (GB)
-    total, used, free = (x / gib for x in shutil.disk_usage(Path.cwd()))  # bytes
+    total, used, free = (x / gib for x in shutil.disk_usage(path))  # bytes
 
     if data * sf < free:
         return True  # sufficient space
 
     # Insufficient space
     text = (
         f"WARNING ⚠️ Insufficient free disk space {free:.1f} GB < {data * sf:.3f} GB required, "
@@ -311,15 +316,15 @@
     f = Path(dir or ".") / (file or url2file(url))  # URL converted to filename
     if "://" not in str(url) and Path(url).is_file():  # URL exists ('://' check required in Windows Python<3.10)
         f = Path(url)  # filename
     elif not f.is_file():  # URL and file do not exist
         desc = f"Downloading {url if gdrive else clean_url(url)} to '{f}'"
         LOGGER.info(f"{desc}...")
         f.parent.mkdir(parents=True, exist_ok=True)  # make directory if missing
-        check_disk_space(url)
+        check_disk_space(url, path=f.parent)
         for i in range(retry + 1):
             try:
                 if curl or i > 0:  # curl download with retry, continue
                     s = "sS" * (not progress)  # silent
                     r = subprocess.run(["curl", "-#", f"-{s}L", url, "-o", f, "--retry", "3", "-C", "-"]).returncode
                     assert r == 0, f"Curl return value {r}"
                 else:  # urllib download
@@ -347,21 +352,21 @@
             except Exception as e:
                 if i == 0 and not is_online():
                     raise ConnectionError(emojis(f"❌  Download failure for {url}. Environment is not online.")) from e
                 elif i >= retry:
                     raise ConnectionError(emojis(f"❌  Download failure for {url}. Retry limit reached.")) from e
                 LOGGER.warning(f"⚠️ Download failure, retrying {i + 1}/{retry} {url}...")
 
-    if unzip and f.exists() and f.suffix in ("", ".zip", ".tar", ".gz"):
+    if unzip and f.exists() and f.suffix in {"", ".zip", ".tar", ".gz"}:
         from zipfile import is_zipfile
 
         unzip_dir = (dir or f.parent).resolve()  # unzip to dir if provided else unzip in place
         if is_zipfile(f):
             unzip_dir = unzip_file(file=f, path=unzip_dir, exist_ok=exist_ok, progress=progress)  # unzip
-        elif f.suffix in (".tar", ".gz"):
+        elif f.suffix in {".tar", ".gz"}:
             LOGGER.info(f"Unzipping {f} to {unzip_dir}...")
             subprocess.run(["tar", "xf" if f.suffix == ".tar" else "xfz", f, "--directory", unzip_dir], check=True)
         if delete:
             f.unlink()  # remove zip
         return unzip_dir
 
 
@@ -402,15 +407,15 @@
     Attempt to download a file from GitHub release assets if it is not found locally. The function checks for the file
     locally first, then tries to download it from the specified GitHub repository release.
 
     Args:
         file (str | Path): The filename or file path to be downloaded.
         repo (str, optional): The GitHub repository in the format 'owner/repo'. Defaults to 'ultralytics/assets'.
         release (str, optional): The specific release version to be downloaded. Defaults to 'v8.1.0'.
-        **kwargs (dict): Additional keyword arguments for the download process.
+        **kwargs (any): Additional keyword arguments for the download process.
 
     Returns:
         (str): The path to the downloaded file.
 
     Example:
         ```python
         file_path = attempt_download_asset('yolov5s.pt', repo='ultralytics/assets', release='latest')
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/errors.py` & `ultralytics-8.2.0/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/files.py` & `ultralytics-8.2.0/ultralytics/utils/files.py`

 * *Files 15% similar despite different names*

```diff
@@ -141,7 +141,48 @@
     return 0.0
 
 
 def get_latest_run(search_dir="."):
     """Return path to most recent 'last.pt' in /runs (i.e. to --resume from)."""
     last_list = glob.glob(f"{search_dir}/**/last*.pt", recursive=True)
     return max(last_list, key=os.path.getctime) if last_list else ""
+
+
+def update_models(model_names=("yolov8n.pt",), source_dir=Path("."), update_names=False):
+    """
+    Updates and re-saves specified YOLO models in an 'updated_models' subdirectory.
+
+    Args:
+        model_names (tuple, optional): Model filenames to update, defaults to ("yolov8n.pt").
+        source_dir (Path, optional): Directory containing models and target subdirectory, defaults to current directory.
+        update_names (bool, optional): Update model names from a data YAML.
+
+    Example:
+        ```python
+        from ultralytics.utils.files import update_models
+
+        model_names = (f"rtdetr-{size}.pt" for size in "lx")
+        update_models(model_names)
+        ```
+    """
+    from ultralytics import YOLO
+    from ultralytics.nn.autobackend import default_class_names
+
+    target_dir = source_dir / "updated_models"
+    target_dir.mkdir(parents=True, exist_ok=True)  # Ensure target directory exists
+
+    for model_name in model_names:
+        model_path = source_dir / model_name
+        print(f"Loading model from {model_path}")
+
+        # Load model
+        model = YOLO(model_path)
+        model.half()
+        if update_names:  # update model names from a dataset YAML
+            model.model.names = default_class_names("coco8.yaml")
+
+        # Define new save path
+        save_path = target_dir / model_name
+
+        # Save model using model.save()
+        print(f"Re-saving {model_name} model to {save_path}")
+        model.save(save_path, use_dill=False)
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/instance.py` & `ultralytics-8.2.0/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/loss.py` & `ultralytics-8.2.0/ultralytics/utils/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ultralytics.utils.metrics import OKS_SIGMA
 from ultralytics.utils.ops import crop_mask, xywh2xyxy, xyxy2xywh
 from ultralytics.utils.tal import RotatedTaskAlignedAssigner, TaskAlignedAssigner, dist2bbox, dist2rbox, make_anchors
+
 from .metrics import bbox_iou, probiou
 from .tal import bbox2dist
 
 
 class VarifocalLoss(nn.Module):
     """
     Varifocal loss by Zhang et al.
@@ -133,18 +134,18 @@
     def __init__(self, sigmas) -> None:
         """Initialize the KeypointLoss class."""
         super().__init__()
         self.sigmas = sigmas
 
     def forward(self, pred_kpts, gt_kpts, kpt_mask, area):
         """Calculates keypoint loss factor and Euclidean distance loss for predicted and actual keypoints."""
-        d = (pred_kpts[..., 0] - gt_kpts[..., 0]) ** 2 + (pred_kpts[..., 1] - gt_kpts[..., 1]) ** 2
+        d = (pred_kpts[..., 0] - gt_kpts[..., 0]).pow(2) + (pred_kpts[..., 1] - gt_kpts[..., 1]).pow(2)
         kpt_loss_factor = kpt_mask.shape[1] / (torch.sum(kpt_mask != 0, dim=1) + 1e-9)
         # e = d / (2 * (area * self.sigmas) ** 2 + 1e-9)  # from formula
-        e = d / (2 * self.sigmas) ** 2 / (area + 1e-9) / 2  # from cocoeval
+        e = d / ((2 * self.sigmas).pow(2) * (area + 1e-9) * 2)  # from cocoeval
         return (kpt_loss_factor.view(-1, 1) * ((1 - torch.exp(-e)) * kpt_mask)).mean()
 
 
 class v8DetectionLoss:
     """Criterion class for computing training losses."""
 
     def __init__(self, model):  # model must be de-paralleled
@@ -153,15 +154,15 @@
         h = model.args  # hyperparameters
 
         m = model.model[-1]  # Detect() module
         self.bce = nn.BCEWithLogitsLoss(reduction="none")
         self.hyp = h
         self.stride = m.stride  # model strides
         self.nc = m.nc  # number of classes
-        self.no = m.no
+        self.no = m.nc + m.reg_max * 4
         self.reg_max = m.reg_max
         self.device = device
 
         self.use_dfl = m.reg_max > 1
 
         self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = BboxLoss(m.reg_max - 1, use_dfl=self.use_dfl).to(device)
@@ -593,15 +594,20 @@
         """Compute the classification loss between predictions and true labels."""
         loss = torch.nn.functional.cross_entropy(preds, batch["cls"], reduction="mean")
         loss_items = loss.detach()
         return loss, loss_items
 
 
 class v8OBBLoss(v8DetectionLoss):
-    def __init__(self, model):  # model must be de-paralleled
+    def __init__(self, model):
+        """
+        Initializes v8OBBLoss with model, assigner, and rotated bbox loss.
+
+        Note model must be de-paralleled.
+        """
         super().__init__(model)
         self.assigner = RotatedTaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = RotatedBboxLoss(self.reg_max - 1, use_dfl=self.use_dfl).to(self.device)
 
     def preprocess(self, targets, batch_size, scale_tensor):
         """Preprocesses the target counts and matches with the input batch size to output a tensor."""
         if targets.shape[0] == 0:
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/metrics.py` & `ultralytics-8.2.0/ultralytics/utils/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 
 def bbox_ioa(box1, box2, iou=False, eps=1e-7):
     """
     Calculate the intersection over box2 area given box1 and box2. Boxes are in x1y1x2y2 format.
 
     Args:
-        box1 (np.array): A numpy array of shape (n, 4) representing n bounding boxes.
-        box2 (np.array): A numpy array of shape (m, 4) representing m bounding boxes.
-        iou (bool): Calculate the standard iou if True else return inter_area/box2_area.
+        box1 (np.ndarray): A numpy array of shape (n, 4) representing n bounding boxes.
+        box2 (np.ndarray): A numpy array of shape (m, 4) representing m bounding boxes.
+        iou (bool): Calculate the standard IoU if True else return inter_area/box2_area.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
-        (np.array): A numpy array of shape (n, m) representing the intersection over box2 area.
+        (np.ndarray): A numpy array of shape (n, m) representing the intersection over box2 area.
     """
 
     # Get the coordinates of bounding boxes
     b1_x1, b1_y1, b1_x2, b1_y2 = box1.T
     b2_x1, b2_y1, b2_x2, b2_y2 = box2.T
 
     # Intersection area
@@ -112,18 +112,20 @@
 
     # IoU
     iou = inter / union
     if CIoU or DIoU or GIoU:
         cw = b1_x2.maximum(b2_x2) - b1_x1.minimum(b2_x1)  # convex (smallest enclosing box) width
         ch = b1_y2.maximum(b2_y2) - b1_y1.minimum(b2_y1)  # convex height
         if CIoU or DIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
-            c2 = cw**2 + ch**2 + eps  # convex diagonal squared
-            rho2 = ((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4  # center dist ** 2
+            c2 = cw.pow(2) + ch.pow(2) + eps  # convex diagonal squared
+            rho2 = (
+                (b2_x1 + b2_x2 - b1_x1 - b1_x2).pow(2) + (b2_y1 + b2_y2 - b1_y1 - b1_y2).pow(2)
+            ) / 4  # center dist**2
             if CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
-                v = (4 / math.pi**2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
+                v = (4 / math.pi**2) * ((w2 / h2).atan() - (w1 / h1).atan()).pow(2)
                 with torch.no_grad():
                     alpha = v / (v - iou + (1 + eps))
                 return iou - (rho2 / c2 + v * alpha)  # CIoU
             return iou - rho2 / c2  # DIoU
         c_area = cw * ch + eps  # convex area
         return iou - (c_area - union) / c_area  # GIoU https://arxiv.org/pdf/1902.09630.pdf
     return iou  # IoU
@@ -158,45 +160,45 @@
         area (torch.Tensor): A tensor of shape (N,) representing areas from ground truth.
         sigma (list): A list containing 17 values representing keypoint scales.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
         (torch.Tensor): A tensor of shape (N, M) representing keypoint similarities.
     """
-    d = (kpt1[:, None, :, 0] - kpt2[..., 0]) ** 2 + (kpt1[:, None, :, 1] - kpt2[..., 1]) ** 2  # (N, M, 17)
+    d = (kpt1[:, None, :, 0] - kpt2[..., 0]).pow(2) + (kpt1[:, None, :, 1] - kpt2[..., 1]).pow(2)  # (N, M, 17)
     sigma = torch.tensor(sigma, device=kpt1.device, dtype=kpt1.dtype)  # (17, )
     kpt_mask = kpt1[..., 2] != 0  # (N, 17)
-    e = d / (2 * sigma) ** 2 / (area[:, None, None] + eps) / 2  # from cocoeval
+    e = d / ((2 * sigma).pow(2) * (area[:, None, None] + eps) * 2)  # from cocoeval
     # e = d / ((area[None, :, None] + eps) * sigma) ** 2 / 2  # from formula
-    return (torch.exp(-e) * kpt_mask[:, None]).sum(-1) / (kpt_mask.sum(-1)[:, None] + eps)
+    return ((-e).exp() * kpt_mask[:, None]).sum(-1) / (kpt_mask.sum(-1)[:, None] + eps)
 
 
 def _get_covariance_matrix(boxes):
     """
     Generating covariance matrix from obbs.
 
     Args:
         boxes (torch.Tensor): A tensor of shape (N, 5) representing rotated bounding boxes, with xywhr format.
 
     Returns:
         (torch.Tensor): Covariance metrixs corresponding to original rotated bounding boxes.
     """
     # Gaussian bounding boxes, ignore the center points (the first two columns) because they are not needed here.
-    gbbs = torch.cat((torch.pow(boxes[:, 2:4], 2) / 12, boxes[:, 4:]), dim=-1)
+    gbbs = torch.cat((boxes[:, 2:4].pow(2) / 12, boxes[:, 4:]), dim=-1)
     a, b, c = gbbs.split(1, dim=-1)
-    return (
-        a * torch.cos(c) ** 2 + b * torch.sin(c) ** 2,
-        a * torch.sin(c) ** 2 + b * torch.cos(c) ** 2,
-        a * torch.cos(c) * torch.sin(c) - b * torch.sin(c) * torch.cos(c),
-    )
+    cos = c.cos()
+    sin = c.sin()
+    cos2 = cos.pow(2)
+    sin2 = sin.pow(2)
+    return a * cos2 + b * sin2, a * sin2 + b * cos2, (a - b) * cos * sin
 
 
 def probiou(obb1, obb2, CIoU=False, eps=1e-7):
     """
-    Calculate the prob iou between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
+    Calculate the prob IoU between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
 
     Args:
         obb1 (torch.Tensor): A tensor of shape (N, 5) representing ground truth obbs, with xywhr format.
         obb2 (torch.Tensor): A tensor of shape (N, 5) representing predicted obbs, with xywhr format.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
@@ -204,43 +206,38 @@
     """
     x1, y1 = obb1[..., :2].split(1, dim=-1)
     x2, y2 = obb2[..., :2].split(1, dim=-1)
     a1, b1, c1 = _get_covariance_matrix(obb1)
     a2, b2, c2 = _get_covariance_matrix(obb2)
 
     t1 = (
-        ((a1 + a2) * (torch.pow(y1 - y2, 2)) + (b1 + b2) * (torch.pow(x1 - x2, 2)))
-        / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)
+        ((a1 + a2) * (y1 - y2).pow(2) + (b1 + b2) * (x1 - x2).pow(2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)
     ) * 0.25
-    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)) * 0.5
+    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)) * 0.5
     t3 = (
-        torch.log(
-            ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)))
-            / (4 * torch.sqrt((a1 * b1 - torch.pow(c1, 2)).clamp_(0) * (a2 * b2 - torch.pow(c2, 2)).clamp_(0)) + eps)
-            + eps
-        )
-        * 0.5
-    )
-    bd = t1 + t2 + t3
-    bd = torch.clamp(bd, eps, 100.0)
-    hd = torch.sqrt(1.0 - torch.exp(-bd) + eps)
+        ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2))
+        / (4 * ((a1 * b1 - c1.pow(2)).clamp_(0) * (a2 * b2 - c2.pow(2)).clamp_(0)).sqrt() + eps)
+        + eps
+    ).log() * 0.5
+    bd = (t1 + t2 + t3).clamp(eps, 100.0)
+    hd = (1.0 - (-bd).exp() + eps).sqrt()
     iou = 1 - hd
     if CIoU:  # only include the wh aspect ratio part
         w1, h1 = obb1[..., 2:4].split(1, dim=-1)
         w2, h2 = obb2[..., 2:4].split(1, dim=-1)
-        v = (4 / math.pi**2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
+        v = (4 / math.pi**2) * ((w2 / h2).atan() - (w1 / h1).atan()).pow(2)
         with torch.no_grad():
             alpha = v / (v - iou + (1 + eps))
         return iou - v * alpha  # CIoU
     return iou
 
 
 def batch_probiou(obb1, obb2, eps=1e-7):
     """
-    Calculate the prob iou between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
+    Calculate the prob IoU between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
 
     Args:
         obb1 (torch.Tensor | np.ndarray): A tensor of shape (N, 5) representing ground truth obbs, with xywhr format.
         obb2 (torch.Tensor | np.ndarray): A tensor of shape (M, 5) representing predicted obbs, with xywhr format.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
@@ -251,29 +248,24 @@
 
     x1, y1 = obb1[..., :2].split(1, dim=-1)
     x2, y2 = (x.squeeze(-1)[None] for x in obb2[..., :2].split(1, dim=-1))
     a1, b1, c1 = _get_covariance_matrix(obb1)
     a2, b2, c2 = (x.squeeze(-1)[None] for x in _get_covariance_matrix(obb2))
 
     t1 = (
-        ((a1 + a2) * (torch.pow(y1 - y2, 2)) + (b1 + b2) * (torch.pow(x1 - x2, 2)))
-        / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)
+        ((a1 + a2) * (y1 - y2).pow(2) + (b1 + b2) * (x1 - x2).pow(2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)
     ) * 0.25
-    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)) * 0.5
+    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)) * 0.5
     t3 = (
-        torch.log(
-            ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)))
-            / (4 * torch.sqrt((a1 * b1 - torch.pow(c1, 2)).clamp_(0) * (a2 * b2 - torch.pow(c2, 2)).clamp_(0)) + eps)
-            + eps
-        )
-        * 0.5
-    )
-    bd = t1 + t2 + t3
-    bd = torch.clamp(bd, eps, 100.0)
-    hd = torch.sqrt(1.0 - torch.exp(-bd) + eps)
+        ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2))
+        / (4 * ((a1 * b1 - c1.pow(2)).clamp_(0) * (a2 * b2 - c2.pow(2)).clamp_(0)).sqrt() + eps)
+        + eps
+    ).log() * 0.5
+    bd = (t1 + t2 + t3).clamp(eps, 100.0)
+    hd = (1.0 - (-bd).exp() + eps).sqrt()
     return 1 - hd
 
 
 def smooth_BCE(eps=0.1):
     """
     Computes smoothed positive and negative Binary Cross-Entropy targets.
 
@@ -291,26 +283,26 @@
 
 class ConfusionMatrix:
     """
     A class for calculating and updating a confusion matrix for object detection and classification tasks.
 
     Attributes:
         task (str): The type of task, either 'detect' or 'classify'.
-        matrix (np.array): The confusion matrix, with dimensions depending on the task.
+        matrix (np.ndarray): The confusion matrix, with dimensions depending on the task.
         nc (int): The number of classes.
         conf (float): The confidence threshold for detections.
         iou_thres (float): The Intersection over Union threshold.
     """
 
     def __init__(self, nc, conf=0.25, iou_thres=0.45, task="detect"):
         """Initialize attributes for the YOLO model."""
         self.task = task
         self.matrix = np.zeros((nc + 1, nc + 1)) if self.task == "detect" else np.zeros((nc, nc))
         self.nc = nc  # number of classes
-        self.conf = 0.25 if conf in (None, 0.001) else conf  # apply 0.25 if default val conf is passed
+        self.conf = 0.25 if conf in {None, 0.001} else conf  # apply 0.25 if default val conf is passed
         self.iou_thres = iou_thres
 
     def process_cls_preds(self, preds, targets):
         """
         Update confusion matrix for classification task.
 
         Args:
@@ -322,17 +314,18 @@
             self.matrix[p][t] += 1
 
     def process_batch(self, detections, gt_bboxes, gt_cls):
         """
         Update confusion matrix for object detection task.
 
         Args:
-            detections (Array[N, 6]): Detected bounding boxes and their associated information.
-                                      Each row should contain (x1, y1, x2, y2, conf, class).
-            gt_bboxes (Array[M, 4]): Ground truth bounding boxes with xyxy format.
+            detections (Array[N, 6] | Array[N, 7]): Detected bounding boxes and their associated information.
+                                      Each row should contain (x1, y1, x2, y2, conf, class)
+                                      or with an additional element `angle` when it's obb.
+            gt_bboxes (Array[M, 4]| Array[N, 5]): Ground truth bounding boxes with xyxy/xyxyr format.
             gt_cls (Array[M]): The class labels.
         """
         if gt_cls.shape[0] == 0:  # Check if labels is empty
             if detections is not None:
                 detections = detections[detections[:, 4] > self.conf]
                 detection_classes = detections[:, 5].int()
                 for dc in detection_classes:
@@ -343,15 +336,20 @@
             for gc in gt_classes:
                 self.matrix[self.nc, gc] += 1  # background FN
             return
 
         detections = detections[detections[:, 4] > self.conf]
         gt_classes = gt_cls.int()
         detection_classes = detections[:, 5].int()
-        iou = box_iou(gt_bboxes, detections[:, :4])
+        is_obb = detections.shape[1] == 7 and gt_bboxes.shape[1] == 5  # with additional `angle` dimension
+        iou = (
+            batch_probiou(gt_bboxes, torch.cat([detections[:, :4], detections[:, -1:]], dim=-1))
+            if is_obb
+            else box_iou(gt_bboxes, detections[:, :4])
+        )
 
         x = torch.where(iou > self.iou_thres)
         if x[0].shape[0]:
             matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]), 1).cpu().numpy()
             if x[0].shape[0] > 1:
                 matches = matches[matches[:, 2].argsort()[::-1]]
                 matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
@@ -393,27 +391,27 @@
 
         Args:
             normalize (bool): Whether to normalize the confusion matrix.
             save_dir (str): Directory where the plot will be saved.
             names (tuple): Names of classes, used as labels on the plot.
             on_plot (func): An optional callback to pass plots path and data when they are rendered.
         """
-        import seaborn as sn
+        import seaborn  # scope for faster 'import ultralytics'
 
         array = self.matrix / ((self.matrix.sum(0).reshape(1, -1) + 1e-9) if normalize else 1)  # normalize columns
         array[array < 0.005] = np.nan  # don't annotate (would appear as 0.00)
 
         fig, ax = plt.subplots(1, 1, figsize=(12, 9), tight_layout=True)
         nc, nn = self.nc, len(names)  # number of classes, names
-        sn.set(font_scale=1.0 if nc < 50 else 0.8)  # for label size
+        seaborn.set_theme(font_scale=1.0 if nc < 50 else 0.8)  # for label size
         labels = (0 < nn < 99) and (nn == nc)  # apply names to ticklabels
         ticklabels = (list(names) + ["background"]) if labels else "auto"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")  # suppress empty matrix RuntimeWarning: All-NaN slice encountered
-            sn.heatmap(
+            seaborn.heatmap(
                 array,
                 ax=ax,
                 annot=nc < 30,
                 annot_kws={"size": 8},
                 cmap="Blues",
                 fmt=".2f" if normalize else ".0f",
                 square=True,
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/ops.py` & `ultralytics-8.2.0/ultralytics/utils/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 import time
 
 import cv2
 import numpy as np
 import torch
 import torch.nn.functional as F
-import torchvision
 
 from ultralytics.utils import LOGGER
 from ultralytics.utils.metrics import batch_probiou
 
 
 class Profile(contextlib.ContextDecorator):
     """
@@ -143,15 +142,15 @@
 def nms_rotated(boxes, scores, threshold=0.45):
     """
     NMS for obbs, powered by probiou and fast-nms.
 
     Args:
         boxes (torch.Tensor): (N, 5), xywhr.
         scores (torch.Tensor): (N, ).
-        threshold (float): Iou threshold.
+        threshold (float): IoU threshold.
 
     Returns:
     """
     if len(boxes) == 0:
         return np.empty((0,), dtype=np.int8)
     sorted_idx = torch.argsort(scores, descending=True)
     boxes = boxes[sorted_idx]
@@ -169,14 +168,15 @@
     multi_label=False,
     labels=(),
     max_det=300,
     nc=0,  # number of classes (optional)
     max_time_img=0.05,
     max_nms=30000,
     max_wh=7680,
+    in_place=True,
     rotated=False,
 ):
     """
     Perform non-maximum suppression (NMS) on a set of boxes, with support for masks and multiple labels per box.
 
     Args:
         prediction (torch.Tensor): A tensor of shape (batch_size, num_classes + 4 + num_masks, num_boxes)
@@ -193,21 +193,23 @@
         labels (List[List[Union[int, float, torch.Tensor]]]): A list of lists, where each inner
             list contains the apriori labels for a given image. The list should be in the format
             output by a dataloader, with each label being a tuple of (class_index, x1, y1, x2, y2).
         max_det (int): The maximum number of boxes to keep after NMS.
         nc (int, optional): The number of classes output by the model. Any indices after this will be considered masks.
         max_time_img (float): The maximum time (seconds) for processing one image.
         max_nms (int): The maximum number of boxes into torchvision.ops.nms().
-        max_wh (int): The maximum box width and height in pixels
+        max_wh (int): The maximum box width and height in pixels.
+        in_place (bool): If True, the input prediction tensor will be modified in place.
 
     Returns:
         (List[torch.Tensor]): A list of length batch_size, where each element is a tensor of
             shape (num_boxes, 6 + num_masks) containing the kept boxes, with columns
             (x1, y1, x2, y2, confidence, class, mask1, mask2, ...).
     """
+    import torchvision  # scope for faster 'import ultralytics'
 
     # Checks
     assert 0 <= conf_thres <= 1, f"Invalid Confidence threshold {conf_thres}, valid values are between 0.0 and 1.0"
     assert 0 <= iou_thres <= 1, f"Invalid IoU {iou_thres}, valid values are between 0.0 and 1.0"
     if isinstance(prediction, (list, tuple)):  # YOLOv8 model in validation model, output = (inference_out, loss_out)
         prediction = prediction[0]  # select only inference output
 
@@ -220,15 +222,18 @@
     # Settings
     # min_wh = 2  # (pixels) minimum box width and height
     time_limit = 2.0 + max_time_img * bs  # seconds to quit after
     multi_label &= nc > 1  # multiple labels per box (adds 0.5ms/img)
 
     prediction = prediction.transpose(-1, -2)  # shape(1,84,6300) to shape(1,6300,84)
     if not rotated:
-        prediction[..., :4] = xywh2xyxy(prediction[..., :4])  # xywh to xyxy
+        if in_place:
+            prediction[..., :4] = xywh2xyxy(prediction[..., :4])  # xywh to xyxy
+        else:
+            prediction = torch.cat((xywh2xyxy(prediction[..., :4]), prediction[..., 4:]), dim=-1)  # xywh to xyxy
 
     t = time.time()
     output = [torch.zeros((0, 6 + nm), device=prediction.device)] * bs
     for xi, x in enumerate(prediction):  # image index, image inference
         # Apply constraints
         # x[((x[:, 2:4] < min_wh) | (x[:, 2:4] > max_wh)).any(1), 4] = 0  # width-height
         x = x[xc[xi]]  # confidence
@@ -278,15 +283,15 @@
         i = i[:max_det]  # limit detections
 
         # # Experimental
         # merge = False  # use merge-NMS
         # if merge and (1 < n < 3E3):  # Merge NMS (boxes merged using weighted mean)
         #     # Update boxes as boxes(i,4) = weights(i,n) * boxes(n,4)
         #     from .metrics import box_iou
-        #     iou = box_iou(boxes[i], boxes) > iou_thres  # iou matrix
+        #     iou = box_iou(boxes[i], boxes) > iou_thres  # IoU matrix
         #     weights = iou * scores[None]  # box weights
         #     x[i, :4] = torch.mm(weights, x[:, :4]).float() / weights.sum(1, keepdim=True)  # merged boxes
         #     redundant = True  # require redundant detections
         #     if redundant:
         #         i = i[iou.sum(1) > 1]  # require redundancy
 
         output[xi] = x[i]
@@ -542,15 +547,15 @@
 
 def xywhr2xyxyxyxy(rboxes):
     """
     Convert batched Oriented Bounding Boxes (OBB) from [xywh, rotation] to [xy1, xy2, xy3, xy4]. Rotation values should
     be in degrees from 0 to 90.
 
     Args:
-        rboxes (numpy.ndarray | torch.Tensor): Input data in [cx, cy, w, h, rotation] format of shape (n, 5) or (b, n, 5).
+        rboxes (numpy.ndarray | torch.Tensor): Boxes in [cx, cy, w, h, rotation] format of shape (n, 5) or (b, n, 5).
 
     Returns:
         (numpy.ndarray | torch.Tensor): Converted corner points of shape (n, 4, 2) or (b, n, 4, 2).
     """
     is_numpy = isinstance(rboxes, np.ndarray)
     cos, sin = (np.cos, np.sin) if is_numpy else (torch.cos, torch.sin)
 
@@ -629,15 +634,15 @@
     Args:
         masks (torch.Tensor): [n, h, w] tensor of masks
         boxes (torch.Tensor): [n, 4] tensor of bbox coordinates in relative point form
 
     Returns:
         (torch.Tensor): The masks are being cropped to the bounding box.
     """
-    n, h, w = masks.shape
+    _, h, w = masks.shape
     x1, y1, x2, y2 = torch.chunk(boxes[:, :, None], 4, 1)  # x1 shape(n,1,1)
     r = torch.arange(w, device=masks.device, dtype=x1.dtype)[None, None, :]  # rows shape(1,1,w)
     c = torch.arange(h, device=masks.device, dtype=x1.dtype)[None, :, None]  # cols shape(1,h,1)
 
     return masks * ((r >= x1) * (r < x2) * (c >= y1) * (c < y2))
 
 
@@ -677,20 +682,22 @@
         (torch.Tensor): A binary mask tensor of shape [n, h, w], where n is the number of masks after NMS, and h and w
             are the height and width of the input image. The mask is applied to the bounding boxes.
     """
 
     c, mh, mw = protos.shape  # CHW
     ih, iw = shape
     masks = (masks_in @ protos.float().view(c, -1)).sigmoid().view(-1, mh, mw)  # CHW
+    width_ratio = mw / iw
+    height_ratio = mh / ih
 
     downsampled_bboxes = bboxes.clone()
-    downsampled_bboxes[:, 0] *= mw / iw
-    downsampled_bboxes[:, 2] *= mw / iw
-    downsampled_bboxes[:, 3] *= mh / ih
-    downsampled_bboxes[:, 1] *= mh / ih
+    downsampled_bboxes[:, 0] *= width_ratio
+    downsampled_bboxes[:, 2] *= width_ratio
+    downsampled_bboxes[:, 3] *= height_ratio
+    downsampled_bboxes[:, 1] *= height_ratio
 
     masks = crop_mask(masks, downsampled_bboxes)  # CHW
     if upsample:
         masks = F.interpolate(masks[None], shape, mode="bilinear", align_corners=False)[0]  # CHW
     return masks.gt_(0.5)
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/patches.py` & `ultralytics-8.2.0/ultralytics/utils/patches.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,31 +56,33 @@
     _imshow(winname.encode("unicode_escape").decode(), mat)
 
 
 # PyTorch functions ----------------------------------------------------------------------------------------------------
 _torch_save = torch.save  # copy to avoid recursion errors
 
 
-def torch_save(*args, **kwargs):
+def torch_save(*args, use_dill=True, **kwargs):
     """
-    Use dill (if exists) to serialize the lambda functions where pickle does not do this. Also adds 3 retries with
-    exponential standoff in case of save failure to improve robustness to transient issues.
+    Optionally use dill to serialize lambda functions where pickle does not, adding robustness with 3 retries and
+    exponential standoff in case of save failure.
 
     Args:
         *args (tuple): Positional arguments to pass to torch.save.
-        **kwargs (dict): Keyword arguments to pass to torch.save.
+        use_dill (bool): Whether to try using dill for serialization if available. Defaults to True.
+        **kwargs (any): Keyword arguments to pass to torch.save.
     """
     try:
-        import dill as pickle  # noqa
-    except ImportError:
+        assert use_dill
+        import dill as pickle
+    except (AssertionError, ImportError):
         import pickle
 
     if "pickle_module" not in kwargs:
-        kwargs["pickle_module"] = pickle  # noqa
+        kwargs["pickle_module"] = pickle
 
     for i in range(4):  # 3 retries
         try:
             return _torch_save(*args, **kwargs)
-        except RuntimeError:  # unable to save, possibly waiting for device to flush or anti-virus to finish scanning
+        except RuntimeError as e:  # unable to save, possibly waiting for device to flush or antivirus scan
             if i == 3:
-                raise
-            time.sleep((2**i) / 2)  # exponential standoff 0.5s, 1.0s, 2.0s
+                raise e
+            time.sleep((2**i) / 2)  # exponential standoff: 0.5s, 1.0s, 2.0s
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/plotting.py` & `ultralytics-8.2.0/ultralytics/utils/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image, ImageDraw, ImageFont
 from PIL import __version__ as pil_version
 
 from ultralytics.utils import LOGGER, TryExcept, ops, plt_settings, threaded
-from .checks import check_font, check_version, is_ascii
-from .files import increment_path
+from ultralytics.utils.checks import check_font, check_version, is_ascii
+from ultralytics.utils.files import increment_path
 
 
 class Colors:
     """
     Ultralytics default color palette https://ultralytics.com/.
 
     This class provides methods to work with the Ultralytics color palette, including converting hex color codes to
     RGB values.
 
     Attributes:
         palette (list of tuple): List of RGB color values.
         n (int): The number of colors in the palette.
-        pose_palette (np.array): A specific color palette array with dtype np.uint8.
+        pose_palette (np.ndarray): A specific color palette array with dtype np.uint8.
     """
 
     def __init__(self):
         """Initialize colors as hex = matplotlib.colors.TABLEAU_COLORS.values()."""
         hexs = (
             "FF3838",
             "FF9D97",
@@ -108,31 +108,32 @@
         skeleton (List[List[int]]): Skeleton structure for keypoints.
         limb_color (List[int]): Color palette for limbs.
         kpt_color (List[int]): Color palette for keypoints.
     """
 
     def __init__(self, im, line_width=None, font_size=None, font="Arial.ttf", pil=False, example="abc"):
         """Initialize the Annotator class with image and line width along with color palette for keypoints and limbs."""
-        assert im.data.contiguous, "Image not contiguous. Apply np.ascontiguousarray(im) to Annotator() input images."
         non_ascii = not is_ascii(example)  # non-latin labels, i.e. asian, arabic, cyrillic
-        self.pil = pil or non_ascii
-        self.lw = line_width or max(round(sum(im.shape) / 2 * 0.003), 2)  # line width
+        input_is_pil = isinstance(im, Image.Image)
+        self.pil = pil or non_ascii or input_is_pil
+        self.lw = line_width or max(round(sum(im.size if input_is_pil else im.shape) / 2 * 0.003), 2)
         if self.pil:  # use PIL
-            self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
+            self.im = im if input_is_pil else Image.fromarray(im)
             self.draw = ImageDraw.Draw(self.im)
             try:
                 font = check_font("Arial.Unicode.ttf" if non_ascii else font)
                 size = font_size or max(round(sum(self.im.size) / 2 * 0.035), 12)
                 self.font = ImageFont.truetype(str(font), size)
             except Exception:
                 self.font = ImageFont.load_default()
             # Deprecation fix for w, h = getsize(string) -> _, _, w, h = getbox(string)
             if check_version(pil_version, "9.2.0"):
                 self.font.getsize = lambda x: self.font.getbbox(x)[2:4]  # text width, height
         else:  # use cv2
+            assert im.data.contiguous, "Image not contiguous. Apply np.ascontiguousarray(im) to Annotator input images."
             self.im = im if im.flags.writeable else im.copy()
             self.tf = max(self.lw - 1, 1)  # font thickness
             self.sf = self.lw / 3  # font scale
         # Pose
         self.skeleton = [
             [16, 14],
             [14, 12],
@@ -235,52 +236,53 @@
         im_mask = im_gpu * 255
         im_mask_np = im_mask.byte().cpu().numpy()
         self.im[:] = im_mask_np if retina_masks else ops.scale_image(im_mask_np, self.im.shape)
         if self.pil:
             # Convert im back to PIL and update draw
             self.fromarray(self.im)
 
-    def kpts(self, kpts, shape=(640, 640), radius=5, kpt_line=True):
+    def kpts(self, kpts, shape=(640, 640), radius=5, kpt_line=True, conf_thres=0.25):
         """
         Plot keypoints on the image.
 
         Args:
             kpts (tensor): Predicted keypoints with shape [17, 3]. Each keypoint has (x, y, confidence).
             shape (tuple): Image shape as a tuple (h, w), where h is the height and w is the width.
             radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool, optional): If True, the function will draw lines connecting keypoints
                                        for human pose. Default is True.
 
-        Note: `kpt_line=True` currently only supports human pose plotting.
+        Note:
+            `kpt_line=True` currently only supports human pose plotting.
         """
         if self.pil:
             # Convert to numpy first
             self.im = np.asarray(self.im).copy()
         nkpt, ndim = kpts.shape
         is_pose = nkpt == 17 and ndim in {2, 3}
         kpt_line &= is_pose  # `kpt_line=True` for now only supports human pose plotting
         for i, k in enumerate(kpts):
             color_k = [int(x) for x in self.kpt_color[i]] if is_pose else colors(i)
             x_coord, y_coord = k[0], k[1]
             if x_coord % shape[1] != 0 and y_coord % shape[0] != 0:
                 if len(k) == 3:
                     conf = k[2]
-                    if conf < 0.5:
+                    if conf < conf_thres:
                         continue
                 cv2.circle(self.im, (int(x_coord), int(y_coord)), radius, color_k, -1, lineType=cv2.LINE_AA)
 
         if kpt_line:
             ndim = kpts.shape[-1]
             for i, sk in enumerate(self.skeleton):
                 pos1 = (int(kpts[(sk[0] - 1), 0]), int(kpts[(sk[0] - 1), 1]))
                 pos2 = (int(kpts[(sk[1] - 1), 0]), int(kpts[(sk[1] - 1), 1]))
                 if ndim == 3:
                     conf1 = kpts[(sk[0] - 1), 2]
                     conf2 = kpts[(sk[1] - 1), 2]
-                    if conf1 < 0.5 or conf2 < 0.5:
+                    if conf1 < conf_thres or conf2 < conf_thres:
                         continue
                 if pos1[0] % shape[1] == 0 or pos1[1] % shape[0] == 0 or pos1[0] < 0 or pos1[1] < 0:
                     continue
                 if pos2[0] % shape[1] == 0 or pos2[1] % shape[0] == 0 or pos2[0] < 0 or pos2[1] < 0:
                     continue
                 cv2.line(self.im, pos1, pos2, [int(x) for x in self.limb_color[i]], thickness=2, lineType=cv2.LINE_AA)
         if self.pil:
@@ -325,69 +327,158 @@
         self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
         self.draw = ImageDraw.Draw(self.im)
 
     def result(self):
         """Return annotated image as array."""
         return np.asarray(self.im)
 
-    # Object Counting Annotator
+    def show(self, title=None):
+        """Show the annotated image."""
+        Image.fromarray(np.asarray(self.im)[..., ::-1]).show(title)
+
+    def save(self, filename="image.jpg"):
+        """Save the annotated image to 'filename'."""
+        cv2.imwrite(filename, np.asarray(self.im))
+
+    def get_bbox_dimension(self, bbox=None):
+        """
+        Calculate the area of a bounding box.
+
+        Args:
+            bbox (tuple): Bounding box coordinates in the format (x_min, y_min, x_max, y_max).
+
+        Returns:
+            angle (degree): Degree value of angle between three points
+        """
+        x_min, y_min, x_max, y_max = bbox
+        width = x_max - x_min
+        height = y_max - y_min
+        return width, height, width * height
+
     def draw_region(self, reg_pts=None, color=(0, 255, 0), thickness=5):
         """
-        Draw region line
+        Draw region line.
+
         Args:
             reg_pts (list): Region Points (for line 2 points, for region 4 points)
             color (tuple): Region Color value
             thickness (int): Region area thickness value
         """
         cv2.polylines(self.im, [np.array(reg_pts, dtype=np.int32)], isClosed=True, color=color, thickness=thickness)
 
     def draw_centroid_and_tracks(self, track, color=(255, 0, 255), track_thickness=2):
         """
-        Draw centroid point and track trails
+        Draw centroid point and track trails.
+
         Args:
             track (list): object tracking points for trails display
             color (tuple): tracks line color
             track_thickness (int): track line thickness value
         """
         points = np.hstack(track).astype(np.int32).reshape((-1, 1, 2))
         cv2.polylines(self.im, [points], isClosed=False, color=color, thickness=track_thickness)
         cv2.circle(self.im, (int(track[-1][0]), int(track[-1][1])), track_thickness * 2, color, -1)
 
-    def count_labels(self, counts=0, count_txt_size=2, color=(255, 255, 255), txt_color=(0, 0, 0)):
+    def queue_counts_display(self, label, points=None, region_color=(255, 255, 255), txt_color=(0, 0, 0), fontsize=0.7):
         """
-        Plot counts for object counter
+        Displays queue counts on an image centered at the points with customizable font size and colors.
+
         Args:
-            counts (int): objects counts value
-            count_txt_size (int): text size for counts display
-            color (tuple): background color of counts display
-            txt_color (tuple): text color of counts display
+            label (str): queue counts label
+            points (tuple): region points for center point calculation to display text
+            region_color (RGB): queue region color
+            txt_color (RGB): text display color
+            fontsize (float): text fontsize
+        """
+        x_values = [point[0] for point in points]
+        y_values = [point[1] for point in points]
+        center_x = sum(x_values) // len(points)
+        center_y = sum(y_values) // len(points)
+
+        text_size = cv2.getTextSize(label, 0, fontScale=fontsize, thickness=self.tf)[0]
+        text_width = text_size[0]
+        text_height = text_size[1]
+
+        rect_width = text_width + 20
+        rect_height = text_height + 20
+        rect_top_left = (center_x - rect_width // 2, center_y - rect_height // 2)
+        rect_bottom_right = (center_x + rect_width // 2, center_y + rect_height // 2)
+        cv2.rectangle(self.im, rect_top_left, rect_bottom_right, region_color, -1)
+
+        text_x = center_x - text_width // 2
+        text_y = center_y + text_height // 2
+
+        # Draw text
+        cv2.putText(
+            self.im,
+            label,
+            (text_x, text_y),
+            0,
+            fontScale=fontsize,
+            color=txt_color,
+            thickness=self.tf,
+            lineType=cv2.LINE_AA,
+        )
+
+    def display_counts(self, counts=None, count_bg_color=(0, 0, 0), count_txt_color=(255, 255, 255)):
         """
-        self.tf = count_txt_size
+        Display counts on im0 with text background and border.
+
+        Args:
+            counts (str): objects count data
+            count_bg_color (RGB Color): counts highlighter color
+            count_txt_color (RGB Color): counts display color
+        """
+
         tl = self.tf or round(0.002 * (self.im.shape[0] + self.im.shape[1]) / 2) + 1
         tf = max(tl - 1, 1)
 
-        # Get text size for in_count and out_count
-        t_size_in = cv2.getTextSize(str(counts), 0, fontScale=tl / 2, thickness=tf)[0]
+        t_sizes = [cv2.getTextSize(str(count), 0, fontScale=self.sf, thickness=self.tf)[0] for count in counts]
 
-        # Calculate positions for counts label
-        text_width = t_size_in[0]
-        text_x = (self.im.shape[1] - text_width) // 2  # Center x-coordinate
-        text_y = t_size_in[1]
+        max_text_width = max([size[0] for size in t_sizes])
+        max_text_height = max([size[1] for size in t_sizes])
 
-        # Create a rounded rectangle for in_count
-        cv2.rectangle(
-            self.im, (text_x - 5, text_y - 5), (text_x + text_width + 7, text_y + t_size_in[1] + 7), color, -1
-        )
-        cv2.putText(
-            self.im, str(counts), (text_x, text_y + t_size_in[1]), 0, tl / 2, txt_color, self.tf, lineType=cv2.LINE_AA
-        )
+        text_x = self.im.shape[1] - int(self.im.shape[1] * 0.025 + max_text_width)
+        text_y = int(self.im.shape[0] * 0.025)
+
+        # Calculate dynamic gap between each count value based on the width of the image
+        dynamic_gap = max(1, self.im.shape[1] // 100) * tf
+
+        for i, count in enumerate(counts):
+            text_x_pos = text_x
+            text_y_pos = text_y + i * dynamic_gap  # Adjust vertical position with dynamic gap
+
+            # Draw the border
+            cv2.rectangle(
+                self.im,
+                (text_x_pos - (10 * tf), text_y_pos - (10 * tf)),
+                (text_x_pos + max_text_width + (10 * tf), text_y_pos + max_text_height + (10 * tf)),
+                count_bg_color,
+                -1,
+            )
+
+            # Draw the count text
+            cv2.putText(
+                self.im,
+                str(count),
+                (text_x_pos, text_y_pos + max_text_height),
+                0,
+                fontScale=self.sf,
+                color=count_txt_color,
+                thickness=self.tf,
+                lineType=cv2.LINE_AA,
+            )
+
+            text_y_pos += tf * max_text_height
 
     @staticmethod
     def estimate_pose_angle(a, b, c):
-        """Calculate the pose angle for object
+        """
+        Calculate the pose angle for object.
+
         Args:
             a (float) : The value of pose point a
             b (float): The value of pose point b
             c (float): The value o pose point c
 
         Returns:
             angle (degree): Degree value of angle between three points
@@ -395,33 +486,31 @@
         a, b, c = np.array(a), np.array(b), np.array(c)
         radians = np.arctan2(c[1] - b[1], c[0] - b[0]) - np.arctan2(a[1] - b[1], a[0] - b[0])
         angle = np.abs(radians * 180.0 / np.pi)
         if angle > 180.0:
             angle = 360 - angle
         return angle
 
-    def draw_specific_points(self, keypoints, indices=[2, 5, 7], shape=(640, 640), radius=2):
+    def draw_specific_points(self, keypoints, indices=[2, 5, 7], shape=(640, 640), radius=2, conf_thres=0.25):
         """
         Draw specific keypoints for gym steps counting.
 
         Args:
             keypoints (list): list of keypoints data to be plotted
             indices (list): keypoints ids list to be plotted
             shape (tuple): imgsz for model inference
             radius (int): Keypoint radius value
         """
-        nkpts, ndim = keypoints.shape
-        nkpts == 17 and ndim == 3
         for i, k in enumerate(keypoints):
             if i in indices:
                 x_coord, y_coord = k[0], k[1]
                 if x_coord % shape[1] != 0 and y_coord % shape[0] != 0:
                     if len(k) == 3:
                         conf = k[2]
-                        if conf < 0.5:
+                        if conf < conf_thres:
                             continue
                     cv2.circle(self.im, (int(x_coord), int(y_coord)), radius, (0, 255, 0), -1, lineType=cv2.LINE_AA)
         return self.im
 
     def plot_angle_and_count_and_stage(self, angle_text, count_text, stage_text, center_kpt, line_thickness=2):
         """
         Plot the pose angle, count value and step stage.
@@ -526,38 +615,34 @@
         Args:
             distance_m (float): Distance between two bbox centroids in meters.
             distance_mm (float): Distance between two bbox centroids in millimeters.
             centroids (list): Bounding box centroids data.
             line_color (RGB): Distance line color.
             centroid_color (RGB): Bounding box centroid color.
         """
-        (text_width_m, text_height_m), _ = cv2.getTextSize(
-            f"Distance M: {distance_m:.2f}m", cv2.FONT_HERSHEY_SIMPLEX, 0.8, 2
-        )
+        (text_width_m, text_height_m), _ = cv2.getTextSize(f"Distance M: {distance_m:.2f}m", 0, 0.8, 2)
         cv2.rectangle(self.im, (15, 25), (15 + text_width_m + 10, 25 + text_height_m + 20), (255, 255, 255), -1)
         cv2.putText(
             self.im,
             f"Distance M: {distance_m:.2f}m",
             (20, 50),
-            cv2.FONT_HERSHEY_SIMPLEX,
+            0,
             0.8,
             (0, 0, 0),
             2,
             cv2.LINE_AA,
         )
 
-        (text_width_mm, text_height_mm), _ = cv2.getTextSize(
-            f"Distance MM: {distance_mm:.2f}mm", cv2.FONT_HERSHEY_SIMPLEX, 0.8, 2
-        )
+        (text_width_mm, text_height_mm), _ = cv2.getTextSize(f"Distance MM: {distance_mm:.2f}mm", 0, 0.8, 2)
         cv2.rectangle(self.im, (15, 75), (15 + text_width_mm + 10, 75 + text_height_mm + 20), (255, 255, 255), -1)
         cv2.putText(
             self.im,
             f"Distance MM: {distance_mm:.2f}mm",
             (20, 100),
-            cv2.FONT_HERSHEY_SIMPLEX,
+            0,
             0.8,
             (0, 0, 0),
             2,
             cv2.LINE_AA,
         )
 
         cv2.line(self.im, centroids[0], centroids[1], line_color, 3)
@@ -582,45 +667,45 @@
         cv2.line(self.im, center_point, center_bbox, color, thickness)
 
 
 @TryExcept()  # known issue https://github.com/ultralytics/yolov5/issues/5395
 @plt_settings()
 def plot_labels(boxes, cls, names=(), save_dir=Path(""), on_plot=None):
     """Plot training labels including class histograms and box statistics."""
-    import pandas as pd
-    import seaborn as sn
+    import pandas  # scope for faster 'import ultralytics'
+    import seaborn  # scope for faster 'import ultralytics'
 
     # Filter matplotlib>=3.7.2 warning and Seaborn use_inf and is_categorical FutureWarnings
     warnings.filterwarnings("ignore", category=UserWarning, message="The figure layout has changed to tight")
     warnings.filterwarnings("ignore", category=FutureWarning)
 
     # Plot dataset labels
     LOGGER.info(f"Plotting labels to {save_dir / 'labels.jpg'}... ")
     nc = int(cls.max() + 1)  # number of classes
     boxes = boxes[:1000000]  # limit to 1M boxes
-    x = pd.DataFrame(boxes, columns=["x", "y", "width", "height"])
+    x = pandas.DataFrame(boxes, columns=["x", "y", "width", "height"])
 
     # Seaborn correlogram
-    sn.pairplot(x, corner=True, diag_kind="auto", kind="hist", diag_kws=dict(bins=50), plot_kws=dict(pmax=0.9))
+    seaborn.pairplot(x, corner=True, diag_kind="auto", kind="hist", diag_kws=dict(bins=50), plot_kws=dict(pmax=0.9))
     plt.savefig(save_dir / "labels_correlogram.jpg", dpi=200)
     plt.close()
 
     # Matplotlib labels
     ax = plt.subplots(2, 2, figsize=(8, 8), tight_layout=True)[1].ravel()
     y = ax[0].hist(cls, bins=np.linspace(0, nc, nc + 1) - 0.5, rwidth=0.8)
     for i in range(nc):
         y[2].patches[i].set_color([x / 255 for x in colors(i)])
     ax[0].set_ylabel("instances")
     if 0 < len(names) < 30:
         ax[0].set_xticks(range(len(names)))
         ax[0].set_xticklabels(list(names.values()), rotation=90, fontsize=10)
     else:
         ax[0].set_xlabel("classes")
-    sn.histplot(x, x="x", y="y", ax=ax[2], bins=50, pmax=0.9)
-    sn.histplot(x, x="width", y="height", ax=ax[3], bins=50, pmax=0.9)
+    seaborn.histplot(x, x="x", y="y", ax=ax[2], bins=50, pmax=0.9)
+    seaborn.histplot(x, x="width", y="height", ax=ax[3], bins=50, pmax=0.9)
 
     # Rectangles
     boxes[:, 0:2] = 0.5  # center
     boxes = ops.xywh2xyxy(boxes) * 1000
     img = Image.fromarray(np.ones((1000, 1000, 3), dtype=np.uint8) * 255)
     for cls, box in zip(cls[:500], boxes[:500]):
         ImageDraw.Draw(img).rectangle(box, width=1, outline=colors(cls))  # plot
@@ -697,14 +782,15 @@
     kpts=np.zeros((0, 51), dtype=np.float32),
     paths=None,
     fname="images.jpg",
     names=None,
     on_plot=None,
     max_subplots=16,
     save=True,
+    conf_thres=0.25,
 ):
     """Plot image grid with labels."""
     if isinstance(images, torch.Tensor):
         images = images.cpu().float().numpy()
     if isinstance(cls, torch.Tensor):
         cls = cls.cpu().numpy()
     if isinstance(bboxes, torch.Tensor):
@@ -748,29 +834,29 @@
             idx = batch_idx == i
             classes = cls[idx].astype("int")
             labels = confs is None
 
             if len(bboxes):
                 boxes = bboxes[idx]
                 conf = confs[idx] if confs is not None else None  # check for confidence presence (label vs pred)
-                is_obb = boxes.shape[-1] == 5  # xywhr
-                boxes = ops.xywhr2xyxyxyxy(boxes) if is_obb else ops.xywh2xyxy(boxes)
                 if len(boxes):
                     if boxes[:, :4].max() <= 1.1:  # if normalized with tolerance 0.1
-                        boxes[..., 0::2] *= w  # scale to pixels
-                        boxes[..., 1::2] *= h
+                        boxes[..., [0, 2]] *= w  # scale to pixels
+                        boxes[..., [1, 3]] *= h
                     elif scale < 1:  # absolute coords need scale if image scales
                         boxes[..., :4] *= scale
-                boxes[..., 0::2] += x
-                boxes[..., 1::2] += y
+                boxes[..., 0] += x
+                boxes[..., 1] += y
+                is_obb = boxes.shape[-1] == 5  # xywhr
+                boxes = ops.xywhr2xyxyxyxy(boxes) if is_obb else ops.xywh2xyxy(boxes)
                 for j, box in enumerate(boxes.astype(np.int64).tolist()):
                     c = classes[j]
                     color = colors(c)
                     c = names.get(c, c) if names else c
-                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
+                    if labels or conf[j] > conf_thres:
                         label = f"{c}" if labels else f"{c} {conf[j]:.1f}"
                         annotator.box_label(box, label, color=color, rotated=is_obb)
 
             elif len(classes):
                 for c in classes:
                     color = colors(c)
                     c = names.get(c, c) if names else c
@@ -784,31 +870,31 @@
                         kpts_[..., 0] *= w  # scale to pixels
                         kpts_[..., 1] *= h
                     elif scale < 1:  # absolute coords need scale if image scales
                         kpts_ *= scale
                 kpts_[..., 0] += x
                 kpts_[..., 1] += y
                 for j in range(len(kpts_)):
-                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
-                        annotator.kpts(kpts_[j])
+                    if labels or conf[j] > conf_thres:
+                        annotator.kpts(kpts_[j], conf_thres=conf_thres)
 
             # Plot masks
             if len(masks):
                 if idx.shape[0] == masks.shape[0]:  # overlap_masks=False
                     image_masks = masks[idx]
                 else:  # overlap_masks=True
                     image_masks = masks[[i]]  # (1, 640, 640)
                     nl = idx.sum()
                     index = np.arange(nl).reshape((nl, 1, 1)) + 1
                     image_masks = np.repeat(image_masks, nl, axis=0)
                     image_masks = np.where(image_masks == index, 1.0, 0.0)
 
                 im = np.asarray(annotator.im).copy()
                 for j in range(len(image_masks)):
-                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
+                    if labels or conf[j] > conf_thres:
                         color = colors(classes[j])
                         mh, mw = image_masks[j].shape
                         if mh != h or mw != w:
                             mask = image_masks[j].astype(np.uint8)
                             mask = cv2.resize(mask, (w, h))
                             mask = mask.astype(bool)
                         else:
@@ -843,15 +929,15 @@
     Example:
         ```python
         from ultralytics.utils.plotting import plot_results
 
         plot_results('path/to/results.csv', segment=True)
         ```
     """
-    import pandas as pd
+    import pandas as pd  # scope for faster 'import ultralytics'
     from scipy.ndimage import gaussian_filter1d
 
     save_dir = Path(file).parent if file else Path(dir)
     if classify:
         fig, ax = plt.subplots(2, 2, figsize=(6, 6), tight_layout=True)
         index = [1, 4, 2, 3]
     elif segment:
@@ -873,15 +959,15 @@
             x = data.values[:, 0]
             for i, j in enumerate(index):
                 y = data.values[:, j].astype("float")
                 # y[y == 0] = np.nan  # don't show zero values
                 ax[i].plot(x, y, marker=".", label=f.stem, linewidth=2, markersize=8)  # actual results
                 ax[i].plot(x, gaussian_filter1d(y, sigma=3), ":", label="smooth", linewidth=2)  # smoothing line
                 ax[i].set_title(s[j], fontsize=12)
-                # if j in [8, 9, 10]:  # share train and val loss y axes
+                # if j in {8, 9, 10}:  # share train and val loss y axes
                 #     ax[i].get_shared_y_axes().join(ax[i], ax[i - 5])
         except Exception as e:
             LOGGER.warning(f"WARNING: Plotting error for {f}: {e}")
     ax[1].legend()
     fname = save_dir / "results.png"
     fig.savefig(fname, dpi=200)
     plt.close()
@@ -929,15 +1015,15 @@
     Args:
         csv_file (str, optional): Path to the CSV file containing the tuning results. Defaults to 'tune_results.csv'.
 
     Examples:
         >>> plot_tune_results('path/to/tune_results.csv')
     """
 
-    import pandas as pd
+    import pandas as pd  # scope for faster 'import ultralytics'
     from scipy.ndimage import gaussian_filter1d
 
     # Scatter plots for each hyperparameter
     csv_file = Path(csv_file)
     data = pd.read_csv(csv_file)
     num_metrics_columns = 1
     keys = [x.strip() for x in data.columns][num_metrics_columns:]
@@ -1011,21 +1097,21 @@
         stage (int): Module stage within the model.
         n (int, optional): Maximum number of feature maps to plot. Defaults to 32.
         save_dir (Path, optional): Directory to save results. Defaults to Path('runs/detect/exp').
     """
     for m in ["Detect", "Pose", "Segment"]:
         if m in module_type:
             return
-    batch, channels, height, width = x.shape  # batch, channels, height, width
+    _, channels, height, width = x.shape  # batch, channels, height, width
     if height > 1 and width > 1:
         f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
 
         blocks = torch.chunk(x[0].cpu(), channels, dim=0)  # select batch index 0, block by channels
         n = min(n, channels)  # number of plots
-        fig, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
+        _, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
         ax = ax.ravel()
         plt.subplots_adjust(wspace=0.05, hspace=0.05)
         for i in range(n):
             ax[i].imshow(blocks[i].squeeze())  # cmap='gray'
             ax[i].axis("off")
 
         LOGGER.info(f"Saving {f}... ({n}/{channels})")
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/tal.py` & `ultralytics-8.2.0/ultralytics/utils/tal.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         gt_boxes = gt_bboxes.unsqueeze(2).expand(-1, -1, na, -1)[mask_gt]
         overlaps[mask_gt] = self.iou_calculation(gt_boxes, pd_boxes)
 
         align_metric = bbox_scores.pow(self.alpha) * overlaps.pow(self.beta)
         return align_metric, overlaps
 
     def iou_calculation(self, gt_bboxes, pd_bboxes):
-        """Iou calculation for horizontal bounding boxes."""
+        """IoU calculation for horizontal bounding boxes."""
         return bbox_iou(gt_bboxes, pd_bboxes, xywh=False, CIoU=True).squeeze(-1).clamp_(0)
 
     def select_topk_candidates(self, metrics, largest=True, topk_mask=None):
         """
         Select the top-k candidates based on the given metrics.
 
         Args:
@@ -227,15 +227,15 @@
         bbox_deltas = torch.cat((xy_centers[None] - lt, rb - xy_centers[None]), dim=2).view(bs, n_boxes, n_anchors, -1)
         # return (bbox_deltas.min(3)[0] > eps).to(gt_bboxes.dtype)
         return bbox_deltas.amin(3).gt_(eps)
 
     @staticmethod
     def select_highest_overlaps(mask_pos, overlaps, n_max_boxes):
         """
-        If an anchor box is assigned to multiple gts, the one with the highest IoI will be selected.
+        If an anchor box is assigned to multiple gts, the one with the highest IoU will be selected.
 
         Args:
             mask_pos (Tensor): shape(b, n_max_boxes, h*w)
             overlaps (Tensor): shape(b, n_max_boxes, h*w)
 
         Returns:
             target_gt_idx (Tensor): shape(b, h*w)
@@ -256,15 +256,15 @@
         # Find each grid serve which gt(index)
         target_gt_idx = mask_pos.argmax(-2)  # (b, h*w)
         return target_gt_idx, fg_mask, mask_pos
 
 
 class RotatedTaskAlignedAssigner(TaskAlignedAssigner):
     def iou_calculation(self, gt_bboxes, pd_bboxes):
-        """Iou calculation for rotated bounding boxes."""
+        """IoU calculation for rotated bounding boxes."""
         return probiou(gt_bboxes, pd_bboxes).squeeze(-1).clamp_(0)
 
     @staticmethod
     def select_candidates_in_gts(xy_centers, gt_bboxes):
         """
         Select the positive anchor center in gt for rotated bounding boxes.
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.0/ultralytics/utils/torch_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import os
-import platform
 import random
 import time
 from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
-import torchvision
 
-from ultralytics.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, __version__
+from ultralytics.utils import (
+    DEFAULT_CFG_DICT,
+    DEFAULT_CFG_KEYS,
+    LOGGER,
+    PYTHON_VERSION,
+    TORCHVISION_VERSION,
+    __version__,
+    colorstr,
+)
 from ultralytics.utils.checks import check_version
 
 try:
     import thop
 except ImportError:
     thop = None
 
+# Version checks (all default to version>=min_version)
 TORCH_1_9 = check_version(torch.__version__, "1.9.0")
+TORCH_1_13 = check_version(torch.__version__, "1.13.0")
 TORCH_2_0 = check_version(torch.__version__, "2.0.0")
-TORCHVISION_0_10 = check_version(torchvision.__version__, "0.10.0")
-TORCHVISION_0_11 = check_version(torchvision.__version__, "0.11.0")
-TORCHVISION_0_13 = check_version(torchvision.__version__, "0.13.0")
+TORCHVISION_0_10 = check_version(TORCHVISION_VERSION, "0.10.0")
+TORCHVISION_0_11 = check_version(TORCHVISION_VERSION, "0.11.0")
+TORCHVISION_0_13 = check_version(TORCHVISION_VERSION, "0.13.0")
 
 
 @contextmanager
 def torch_distributed_zero_first(local_rank: int):
     """Decorator to make all processes in distributed training wait for each local_master to do something."""
     initialized = torch.distributed.is_available() and torch.distributed.is_initialized()
-    if initialized and local_rank not in (-1, 0):
+    if initialized and local_rank not in {-1, 0}:
         dist.barrier(device_ids=[local_rank])
     yield
     if initialized and local_rank == 0:
         dist.barrier(device_ids=[0])
 
 
 def smart_inference_mode():
@@ -99,28 +107,28 @@
     Note:
         Sets the 'CUDA_VISIBLE_DEVICES' environment variable for specifying which GPUs to use.
     """
 
     if isinstance(device, torch.device):
         return device
 
-    s = f"Ultralytics YOLOv{__version__} 🚀 Python-{platform.python_version()} torch-{torch.__version__} "
+    s = f"Ultralytics YOLOv{__version__} 🚀 Python-{PYTHON_VERSION} torch-{torch.__version__} "
     device = str(device).lower()
     for remove in "cuda:", "none", "(", ")", "[", "]", "'", " ":
         device = device.replace(remove, "")  # to string, 'cuda:0' -> '0' and '(0, 1)' -> '0,1'
     cpu = device == "cpu"
-    mps = device in ("mps", "mps:0")  # Apple Metal Performance Shaders (MPS)
+    mps = device in {"mps", "mps:0"}  # Apple Metal Performance Shaders (MPS)
     if cpu or mps:
         os.environ["CUDA_VISIBLE_DEVICES"] = "-1"  # force torch.cuda.is_available() = False
     elif device:  # non-cpu device requested
         if device == "cuda":
             device = "0"
         visible = os.environ.get("CUDA_VISIBLE_DEVICES", None)
         os.environ["CUDA_VISIBLE_DEVICES"] = device  # set environment variable - must be before assert is_available()
-        if not (torch.cuda.is_available() and torch.cuda.device_count() >= len(device.replace(",", ""))):
+        if not (torch.cuda.is_available() and torch.cuda.device_count() >= len(device.split(","))):
             LOGGER.info(s)
             install = (
                 "See https://pytorch.org/get-started/locally/ for up-to-date torch install instructions if no "
                 "CUDA devices are seen by torch.\n"
                 if torch.cuda.device_count() == 0
                 else ""
             )
@@ -342,15 +350,15 @@
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
             pass  # nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
         elif t is nn.BatchNorm2d:
             m.eps = 1e-3
             m.momentum = 0.03
-        elif t in [nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU]:
+        elif t in {nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU}:
             m.inplace = True
 
 
 def scale_img(img, ratio=1.0, same_shape=False, gs=32):
     """Scales and pads an image tensor of shape img(bs,3,y,x) based on given ratio and grid size gs, optionally
     retaining the original shape.
     """
@@ -500,14 +508,28 @@
     x["train_args"] = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}  # strip non-default keys
     # x['model'].args = x['train_args']
     torch.save(x, s or f)
     mb = os.path.getsize(s or f) / 1e6  # file size
     LOGGER.info(f"Optimizer stripped from {f},{f' saved as {s},' if s else ''} {mb:.1f}MB")
 
 
+def convert_optimizer_state_dict_to_fp16(state_dict):
+    """
+    Converts the state_dict of a given optimizer to FP16, focusing on the 'state' key for tensor conversions.
+
+    This method aims to reduce storage size without altering 'param_groups' as they contain non-tensor data.
+    """
+    for state in state_dict["state"].values():
+        for k, v in state.items():
+            if k != "step" and isinstance(v, torch.Tensor) and v.dtype is torch.float32:
+                state[k] = v.half()
+
+    return state_dict
+
+
 def profile(input, ops, n=10, device=None):
     """
     Ultralytics speed, memory and FLOPs profiler.
 
     Example:
         ```python
         from ultralytics.utils.torch_utils import profile
@@ -595,14 +617,15 @@
         if fitness >= self.best_fitness:  # >= 0 to allow for early zero-fitness stage of training
             self.best_epoch = epoch
             self.best_fitness = fitness
         delta = epoch - self.best_epoch  # epochs without improvement
         self.possible_stop = delta >= (self.patience - 1)  # possible stop may occur next epoch
         stop = delta >= self.patience  # stop training if patience exceeded
         if stop:
+            prefix = colorstr("EarlyStopping: ")
             LOGGER.info(
-                f"Stopping training early as no improvement observed in last {self.patience} epochs. "
+                f"{prefix}Training stopped early as no improvement observed in last {self.patience} epochs. "
                 f"Best results observed at epoch {self.best_epoch}, best model saved as best.pt.\n"
                 f"To update EarlyStopping(patience={self.patience}) pass a new patience value, "
                 f"i.e. `patience=300` or use `patience=0` to disable EarlyStopping."
             )
         return stop
```

### Comparing `ultralytics-8.1.9/ultralytics/utils/triton.py` & `ultralytics-8.2.0/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.9/ultralytics/utils/tuner.py` & `ultralytics-8.2.0/ultralytics/utils/tuner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 from ultralytics.cfg import TASK2DATA, TASK2METRIC, get_save_dir
-from ultralytics.utils import DEFAULT_CFG, DEFAULT_CFG_DICT, LOGGER, NUM_THREADS
+from ultralytics.utils import DEFAULT_CFG, DEFAULT_CFG_DICT, LOGGER, NUM_THREADS, checks
 
 
 def run_ray_tune(
     model, space: dict = None, grace_period: int = 10, gpu_per_trial: int = None, max_samples: int = 10, **train_args
 ):
     """
     Runs hyperparameter tuning using Ray Tune.
@@ -36,31 +36,32 @@
     """
 
     LOGGER.info("💡 Learn about RayTune at https://docs.ultralytics.com/integrations/ray-tune")
     if train_args is None:
         train_args = {}
 
     try:
-        subprocess.run("pip install ray[tune]".split(), check=True)
+        subprocess.run("pip install ray[tune]".split(), check=True)  # do not add single quotes here
 
         import ray
         from ray import tune
         from ray.air import RunConfig
         from ray.air.integrations.wandb import WandbLoggerCallback
         from ray.tune.schedulers import ASHAScheduler
     except ImportError:
-        raise ModuleNotFoundError('Tuning hyperparameters requires Ray Tune. Install with: pip install "ray[tune]"')
+        raise ModuleNotFoundError('Ray Tune required but not found. To install run: pip install "ray[tune]"')
 
     try:
         import wandb
 
         assert hasattr(wandb, "__version__")
     except (ImportError, AssertionError):
         wandb = False
 
+    checks.check_version(ray.__version__, "<=2.9.3", "ray")
     default_space = {
         # 'optimizer': tune.choice(['SGD', 'Adam', 'AdamW', 'NAdam', 'RAdam', 'RMSProp']),
         "lr0": tune.uniform(1e-5, 1e-1),
         "lrf": tune.uniform(0.01, 1.0),  # final OneCycleLR learning rate (lr0 * lrf)
         "momentum": tune.uniform(0.6, 0.98),  # SGD momentum/Adam beta1
         "weight_decay": tune.uniform(0.0, 0.001),  # optimizer weight decay 5e-4
         "warmup_epochs": tune.uniform(0.0, 5.0),  # warmup epochs (fractions ok)
@@ -73,14 +74,15 @@
         "degrees": tune.uniform(0.0, 45.0),  # image rotation (+/- deg)
         "translate": tune.uniform(0.0, 0.9),  # image translation (+/- fraction)
         "scale": tune.uniform(0.0, 0.9),  # image scale (+/- gain)
         "shear": tune.uniform(0.0, 10.0),  # image shear (+/- deg)
         "perspective": tune.uniform(0.0, 0.001),  # image perspective (+/- fraction), range 0-0.001
         "flipud": tune.uniform(0.0, 1.0),  # image flip up-down (probability)
         "fliplr": tune.uniform(0.0, 1.0),  # image flip left-right (probability)
+        "bgr": tune.uniform(0.0, 1.0),  # image channel BGR (probability)
         "mosaic": tune.uniform(0.0, 1.0),  # image mixup (probability)
         "mixup": tune.uniform(0.0, 1.0),  # image mixup (probability)
         "copy_paste": tune.uniform(0.0, 1.0),  # segment copy-paste (probability)
     }
 
     # Put the model in ray store
     task = model.task
```

### Comparing `ultralytics-8.1.9/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.0/ultralytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.1.9
+Version: 8.2.0
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -15,26 +15,26 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: numpy>=1.22.2
 Requires-Dist: opencv-python>=4.6.0
 Requires-Dist: pillow>=7.1.2
 Requires-Dist: pyyaml>=5.3.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchvision>=0.9.0
@@ -47,38 +47,40 @@
 Provides-Extra: dev
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs-material>=9.5.9; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: mkdocs-redirects; extra == "dev"
-Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
+Requires-Dist: mkdocs-ultralytics-plugin>=0.0.44; extra == "dev"
 Provides-Extra: export
 Requires-Dist: onnx>=1.12.0; extra == "export"
-Requires-Dist: coremltools>=7.0; platform_system != "Windows" and extra == "export"
-Requires-Dist: openvino-dev>=2023.0; extra == "export"
-Requires-Dist: tensorflow<=2.13.1; extra == "export"
-Requires-Dist: tensorflowjs>=3.9.0; extra == "export"
+Requires-Dist: coremltools>=7.0; (platform_system != "Windows" and python_version <= "3.11") and extra == "export"
+Requires-Dist: openvino>=2024.0.0; extra == "export"
+Requires-Dist: tensorflow<=2.13.1; python_version <= "3.11" and extra == "export"
+Requires-Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra == "export"
+Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
-Requires-Dist: duckdb; extra == "explorer"
+Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 Provides-Extra: logging
 Requires-Dist: comet; extra == "logging"
 Requires-Dist: tensorboard>=2.13.0; extra == "logging"
 Requires-Dist: dvclive>=2.12.0; extra == "logging"
 Provides-Extra: extra
-Requires-Dist: hub-sdk>=0.0.2; extra == "extra"
+Requires-Dist: hub-sdk>=0.0.5; extra == "extra"
 Requires-Dist: ipython; extra == "extra"
 Requires-Dist: albumentations>=1.0.3; extra == "extra"
-Requires-Dist: pycocotools>=2.0.6; extra == "extra"
+Requires-Dist: pycocotools>=2.0.7; extra == "extra"
 
 <div align="center">
   <p>
     <a href="https://www.ultralytics.com/blog/ultralytics-yolov8-turns-one-a-year-of-breakthroughs-and-innovations" target="_blank">
       <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/im/banner-yolo-vision-2023.png" alt="YOLO Vision banner"></a>
   </p>
 
@@ -274,15 +276,15 @@
 | -------------------------------------------------------------------------------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8n-obb.pt) | 1024                  | 78.0               | 204.77                         | 3.57                                | 3.1                | 23.3              |
 | [YOLOv8s-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8s-obb.pt) | 1024                  | 79.5               | 424.88                         | 4.07                                | 11.4               | 76.3              |
 | [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8m-obb.pt) | 1024                  | 80.5               | 763.48                         | 7.61                                | 26.4               | 208.6             |
 | [YOLOv8l-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt) | 1024                  | 80.7               | 1278.42                        | 11.83                               | 44.5               | 433.8             |
 | [YOLOv8x-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024                  | 81.36              | 1759.10                        | 13.23                               | 69.5               | 676.7             |
 
-- **mAP<sup>test</sup>** values are for single-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
+- **mAP<sup>test</sup>** values are for single-model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html) dataset. <br>Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/evaluation.html).
 - **Speed** averaged over DOTAv1 val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance. <br>Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification (ImageNet)</summary>
 
 See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models trained on [ImageNet](https://docs.ultralytics.com/datasets/classify/imagenet/), which include 1000 pretrained classes.
```

#### html2text {}

```diff
@@ -1,54 +1,57 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.1.9 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.0 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
 vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development Classifier: Topic :: Scientific/Engineering Classifier:
-Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Image Recognition Classifier: Operating System ::
-POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
-System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: matplotlib>=3.3.0 Requires-
-Dist: numpy>=1.22.2 Requires-Dist: opencv-python>=4.6.0 Requires-Dist:
-pillow>=7.1.2 Requires-Dist: pyyaml>=5.3.1 Requires-Dist: requests>=2.23.0
-Requires-Dist: scipy>=1.4.1 Requires-Dist: torch>=1.8.0 Requires-Dist:
-torchvision>=0.9.0 Requires-Dist: tqdm>=4.64.0 Requires-Dist: psutil Requires-
-Dist: py-cpuinfo Requires-Dist: thop>=0.1.1 Requires-Dist: pandas>=1.1.4
-Requires-Dist: seaborn>=0.11.0 Provides-Extra: dev Requires-Dist: ipython;
-extra == "dev" Requires-Dist: check-manifest; extra == "dev" Requires-Dist:
-pre-commit; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-pytest-cov; extra == "dev" Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocstrings
-[python]; extra == "dev" Requires-Dist: mkdocs-jupyter; extra == "dev"
-Requires-Dist: mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-
-ultralytics-plugin>=0.0.42; extra == "dev" Provides-Extra: export Requires-
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
+Engineering :: Image Recognition Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
+:: Windows Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: matplotlib>=3.3.0 Requires-Dist: opencv-
+python>=4.6.0 Requires-Dist: pillow>=7.1.2 Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: requests>=2.23.0 Requires-Dist: scipy>=1.4.1 Requires-Dist:
+torch>=1.8.0 Requires-Dist: torchvision>=0.9.0 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: psutil Requires-Dist: py-cpuinfo Requires-Dist: thop>=0.1.1
+Requires-Dist: pandas>=1.1.4 Requires-Dist: seaborn>=0.11.0 Provides-Extra: dev
+Requires-Dist: ipython; extra == "dev" Requires-Dist: check-manifest; extra ==
+"dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: coverage[toml];
+extra == "dev" Requires-Dist: mkdocs-material>=9.5.9; extra == "dev" Requires-
+Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mkdocs-jupyter; extra
+== "dev" Requires-Dist: mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-
+ultralytics-plugin>=0.0.44; extra == "dev" Provides-Extra: export Requires-
 Dist: onnx>=1.12.0; extra == "export" Requires-Dist: coremltools>=7.0;
-platform_system != "Windows" and extra == "export" Requires-Dist: openvino-
-dev>=2023.0; extra == "export" Requires-Dist: tensorflow<=2.13.1; extra ==
-"export" Requires-Dist: tensorflowjs>=3.9.0; extra == "export" Provides-Extra:
-explorer Requires-Dist: lancedb; extra == "explorer" Requires-Dist: duckdb;
-extra == "explorer" Requires-Dist: streamlit; extra == "explorer" Provides-
-Extra: logging Requires-Dist: comet; extra == "logging" Requires-Dist:
-tensorboard>=2.13.0; extra == "logging" Requires-Dist: dvclive>=2.12.0; extra
-== "logging" Provides-Extra: extra Requires-Dist: hub-sdk>=0.0.2; extra ==
-"extra" Requires-Dist: ipython; extra == "extra" Requires-Dist:
-albumentations>=1.0.3; extra == "extra" Requires-Dist: pycocotools>=2.0.6;
-extra == "extra"
+(platform_system != "Windows" and python_version <= "3.11") and extra ==
+"export" Requires-Dist: openvino>=2024.0.0; extra == "export" Requires-Dist:
+tensorflow<=2.13.1; python_version <= "3.11" and extra == "export" Requires-
+Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra ==
+"export" Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra
+== "export" Provides-Extra: explorer Requires-Dist: lancedb; extra ==
+"explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer" Requires-Dist:
+streamlit; extra == "explorer" Provides-Extra: logging Requires-Dist: comet;
+extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra == "logging"
+Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra: extra
+Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython; extra
+== "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra" Requires-
+Dist: pycocotools>=2.0.7; extra == "extra"
                              _[_Y_O_L_O_ _V_i_s_i_o_n_ _b_a_n_n_e_r_]
        [ä¸­æ](https://docs.ultralytics.com/zh/) | [íêµ­ì´](https://
  docs.ultralytics.com/ko/) | [æ¥æ¬èª](https://docs.ultralytics.com/ja/) |
     [Ð ÑÑÑÐºÐ¸Ð¹](https://docs.ultralytics.com/ru/) | [Deutsch](https://
  docs.ultralytics.com/de/) | [FranÃ§ais](https://docs.ultralytics.com/fr/) |
      [EspaÃ±ol](https://docs.ultralytics.com/es/) | [PortuguÃªs](https://
 docs.ultralytics.com/pt/) | [à¤¹à¤¿à¤¨à¥à¤¦à¥](https://docs.ultralytics.com/
@@ -281,15 +284,15 @@
 v8.1.0/yolov8s-obb.pt) | 1024 | 79.5 | 424.88 | 4.07 | 11.4 | 76.3 | |
 [YOLOv8m-obb](https://github.com/ultralytics/assets/releases/download/v8.1.0/
 yolov8m-obb.pt) | 1024 | 80.5 | 763.48 | 7.61 | 26.4 | 208.6 | | [YOLOv8l-obb]
 (https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8l-obb.pt)
 | 1024 | 80.7 | 1278.42 | 11.83 | 44.5 | 433.8 | | [YOLOv8x-obb](https://
 github.com/ultralytics/assets/releases/download/v8.1.0/yolov8x-obb.pt) | 1024 |
 81.36 | 1759.10 | 13.23 | 69.5 | 676.7 | - **mAPtest** values are for single-
-model multi-scale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
+model multiscale on [DOTAv1](https://captain-whu.github.io/DOTA/index.html)
 dataset.
 Reproduce by `yolo val obb data=DOTAv1.yaml device=0 split=test` and submit
 merged results to [DOTA evaluation](https://captain-whu.github.io/DOTA/
 evaluation.html). - **Speed** averaged over DOTAv1 val images using an [Amazon
 EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
 Reproduce by `yolo val obb data=DOTAv1.yaml batch=1 device=0|cpu`
 Classification (ImageNet) See [Classification Docs](https://
```

### Comparing `ultralytics-8.1.9/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.0/ultralytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 ultralytics/cfg/datasets/DOTAv1.yaml
 ultralytics/cfg/datasets/GlobalWheat2020.yaml
 ultralytics/cfg/datasets/ImageNet.yaml
 ultralytics/cfg/datasets/Objects365.yaml
 ultralytics/cfg/datasets/SKU-110K.yaml
 ultralytics/cfg/datasets/VOC.yaml
 ultralytics/cfg/datasets/VisDrone.yaml
+ultralytics/cfg/datasets/african-wildlife.yaml
+ultralytics/cfg/datasets/brain-tumor.yaml
 ultralytics/cfg/datasets/carparts-seg.yaml
 ultralytics/cfg/datasets/coco-pose.yaml
 ultralytics/cfg/datasets/coco.yaml
 ultralytics/cfg/datasets/coco128-seg.yaml
 ultralytics/cfg/datasets/coco128.yaml
 ultralytics/cfg/datasets/coco8-pose.yaml
 ultralytics/cfg/datasets/coco8-seg.yaml
 ultralytics/cfg/datasets/coco8.yaml
 ultralytics/cfg/datasets/crack-seg.yaml
 ultralytics/cfg/datasets/dota8.yaml
+ultralytics/cfg/datasets/lvis.yaml
 ultralytics/cfg/datasets/open-images-v7.yaml
 ultralytics/cfg/datasets/package-seg.yaml
 ultralytics/cfg/datasets/tiger-pose.yaml
 ultralytics/cfg/datasets/xView.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
@@ -61,15 +64,21 @@
 ultralytics/cfg/models/v8/yolov8-p2.yaml
 ultralytics/cfg/models/v8/yolov8-p6.yaml
 ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
 ultralytics/cfg/models/v8/yolov8-pose.yaml
 ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
 ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
 ultralytics/cfg/models/v8/yolov8-seg.yaml
+ultralytics/cfg/models/v8/yolov8-world.yaml
+ultralytics/cfg/models/v8/yolov8-worldv2.yaml
 ultralytics/cfg/models/v8/yolov8.yaml
+ultralytics/cfg/models/v9/yolov9c-seg.yaml
+ultralytics/cfg/models/v9/yolov9c.yaml
+ultralytics/cfg/models/v9/yolov9e-seg.yaml
+ultralytics/cfg/models/v9/yolov9e.yaml
 ultralytics/cfg/trackers/botsort.yaml
 ultralytics/cfg/trackers/bytetrack.yaml
 ultralytics/data/__init__.py
 ultralytics/data/annotator.py
 ultralytics/data/augment.py
 ultralytics/data/base.py
 ultralytics/data/build.py
@@ -143,28 +152,32 @@
 ultralytics/models/yolo/pose/predict.py
 ultralytics/models/yolo/pose/train.py
 ultralytics/models/yolo/pose/val.py
 ultralytics/models/yolo/segment/__init__.py
 ultralytics/models/yolo/segment/predict.py
 ultralytics/models/yolo/segment/train.py
 ultralytics/models/yolo/segment/val.py
+ultralytics/models/yolo/world/__init__.py
+ultralytics/models/yolo/world/train.py
+ultralytics/models/yolo/world/train_world.py
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
 ultralytics/nn/tasks.py
 ultralytics/nn/modules/__init__.py
 ultralytics/nn/modules/block.py
 ultralytics/nn/modules/conv.py
 ultralytics/nn/modules/head.py
 ultralytics/nn/modules/transformer.py
 ultralytics/nn/modules/utils.py
 ultralytics/solutions/__init__.py
 ultralytics/solutions/ai_gym.py
 ultralytics/solutions/distance_calculation.py
 ultralytics/solutions/heatmap.py
 ultralytics/solutions/object_counter.py
+ultralytics/solutions/queue_management.py
 ultralytics/solutions/speed_estimation.py
 ultralytics/trackers/__init__.py
 ultralytics/trackers/basetrack.py
 ultralytics/trackers/bot_sort.py
 ultralytics/trackers/byte_tracker.py
 ultralytics/trackers/track.py
 ultralytics/trackers/utils/__init__.py
```

