# Comparing `tmp/keras_nightly-3.2.1.dev2024041622.tar.gz` & `tmp/keras_nightly-3.3.0.dev2024041703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.2.1.dev2024041622.tar", last modified: Tue Apr 16 22:17:09 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.0.dev2024041703.tar", last modified: Wed Apr 17 03:20:38 2024, max compression
```

## Comparing `keras_nightly-3.2.1.dev2024041622.tar` & `keras_nightly-3.3.0.dev2024041703.tar`

### file list

```diff
@@ -1,921 +1,921 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.931298 keras_nightly-3.2.1.dev2024041622/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.963298 keras_nightly-3.2.1.dev2024041622/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.967298 keras_nightly-3.2.1.dev2024041622/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/applications_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.967298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.971298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.971298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.975299 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27716 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.979298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67427 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.983298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45948 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.983298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17482 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.987299 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.999299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.999299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.003299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.007299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    42038 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63526 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.007299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.011299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.015299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.023299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.027299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.031299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.035299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.035299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.043299 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.047299 keras_nightly-3.2.1.dev2024041622/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/functional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22761 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.051299 keras_nightly-3.2.1.dev2024041622/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   190182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   278258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    39082 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.063299 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    45028 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    49087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.063299 keras_nightly-3.2.1.dev2024041622/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 22:17:07.000000 keras_nightly-3.2.1.dev2024041622/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-16 22:17:07.000000 keras_nightly-3.2.1.dev2024041622/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.768287 keras_nightly-3.3.0.dev2024041703/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-17 03:20:38.768287 keras_nightly-3.3.0.dev2024041703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.644286 keras_nightly-3.3.0.dev2024041703/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.644286 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.648286 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.652287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.656287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.660287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.664287 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.668287 keras_nightly-3.3.0.dev2024041703/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/activations/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.672287 keras_nightly-3.3.0.dev2024041703/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/applications_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.672287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.676287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.676287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.680287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27716 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.684287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67427 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.684287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45948 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.688287 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.692287 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.692287 keras_nightly-3.3.0.dev2024041703/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.692287 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.696287 keras_nightly-3.3.0.dev2024041703/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.696287 keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.696287 keras_nightly-3.3.0.dev2024041703/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/export/export_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.696287 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.696287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.700287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.700287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.704287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.708287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42038 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63526 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.708287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.712287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.712287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.720287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.724287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.728287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.732287 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.732287 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.732287 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.732287 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.736287 keras_nightly-3.3.0.dev2024041703/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/losses/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/losses/losses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.740287 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.740287 keras_nightly-3.3.0.dev2024041703/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/cloning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/functional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22761 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/sequential_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/variable_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.744287 keras_nightly-3.3.0.dev2024041703/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/linalg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/nn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190182 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278258 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/numpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.748287 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39082 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.748287 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.752287 keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.752287 keras_nightly-3.3.0.dev2024041703/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/random/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/random/seed_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.752287 keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.752287 keras_nightly-3.3.0.dev2024041703/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.752287 keras_nightly-3.3.0.dev2024041703/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.756287 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.756287 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46440 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.760287 keras_nightly-3.3.0.dev2024041703/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/tree/tree_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/tree/tree_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.768287 keras_nightly-3.3.0.dev2024041703/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/naming_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/keras/src/utils/tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 03:20:36.000000 keras_nightly-3.3.0.dev2024041703/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:20:38.768287 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-17 03:20:38.000000 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-17 03:20:38.000000 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:20:38.000000 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 03:20:38.000000 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 03:20:38.000000 keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 03:19:13.000000 keras_nightly-3.3.0.dev2024041703/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 03:20:38.768287 keras_nightly-3.3.0.dev2024041703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-17 03:20:36.000000 keras_nightly-3.3.0.dev2024041703/setup.py
```

### Comparing `keras_nightly-3.2.1.dev2024041622/LICENSE` & `keras_nightly-3.3.0.dev2024041703/LICENSE`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/PKG-INFO` & `keras_nightly-3.3.0.dev2024041703/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041622
+Version: 3.3.0.dev2024041703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -76,14 +76,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras_nightly-3.2.1.dev2024041622/README.md` & `keras_nightly-3.3.0.dev2024041703/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/activation_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/activation_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/attention_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/attention_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/base_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/base_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/conv_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/conv_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/core_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/core_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/merge_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/merge_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/normalization_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/normalization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/pooling_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/pooling_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/regularization_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/regularization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/reshaping_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/reshaping_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/rnn_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/layer_benchmark/rnn_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/bert_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/bert_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/image_classification_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/model_benchmark/image_classification_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py` & `keras_nightly-3.3.0.dev2024041703/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-from keras.api import _tf_keras
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
@@ -34,25 +33,22 @@
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
-from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
-from keras.src.dtype_policies.dtype_policy import QuantizedFloat8DTypePolicy
 from keras.src.initializers.initializer import Initializer
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.losses.loss import Loss
 from keras.src.metrics.metric import Metric
 from keras.src.models.model import Model
 from keras.src.models.sequential import Sequential
 from keras.src.ops.function import Function
 from keras.src.ops.operation import Operation
 from keras.src.optimizers.optimizer import Optimizer
-from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import __version__
 from keras.src.version import version
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
+from keras.api import _tf_keras
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
@@ -33,25 +34,22 @@
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
-from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
-from keras.src.dtype_policies.dtype_policy import QuantizedFloat8DTypePolicy
 from keras.src.initializers.initializer import Initializer
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.losses.loss import Loss
 from keras.src.metrics.metric import Metric
 from keras.src.models.model import Model
 from keras.src.models.sequential import Sequential
 from keras.src.ops.function import Function
 from keras.src.ops.operation import Operation
 from keras.src.optimizers.optimizer import Optimizer
-from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import __version__
 from keras.src.version import version
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/applications/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/config/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/random/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/api/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/activations/activations_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/api_export.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/applications_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/applications_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/convnext.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/densenet.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/imagenet_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/nasnet.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg16.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg19.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/applications/xception.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/backend_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/compute_output_spec_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/compute_output_spec_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/dtypes_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/keras_tensor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/stateless_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/common/variables_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/config.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/exports.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/core.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/math.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/random.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/jax/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,29 +433,30 @@
                     "trainable_variables": trainable_variables,
                     "non_trainable_variables": non_trainable_variables,
                     "optimizer_variables": optimizer_variables,
                     "metrics_variables": metrics_variables,
                 }
 
                 # Callbacks
-                callbacks.on_train_batch_end(step, self._pythonify_logs(logs))
+                logs = self._pythonify_logs(logs)
+                callbacks.on_train_batch_end(step, logs)
                 if self.stop_training:
                     break
 
             # Reattach state to the model (if not already done by a callback).
             # NOTE: doing this after each step would be a big performance
             # bottleneck.
             self.jax_state_sync()
 
-            # Override with model metrics instead of last step logs
+            # Override with model metrics instead of last step logs if needed.
             # The jax spmd_mode is need for multi-process context, since the
             # metrics values are replicated, and we don't want to do a all
             # gather, and only need the local copy of the value.
             with jax.spmd_mode("allow_all"):
-                epoch_logs = self.get_metrics_result()
+                epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
             ):
                 # Create JAXEpochIterator for evaluation and cache it.
                 if getattr(self, "_eval_epoch_iterator", None) is None:
@@ -581,26 +582,27 @@
             self._jax_state = {
                 # I wouldn't recommend modifying non-trainable model state
                 # during evaluate(), but it's allowed.
                 "trainable_variables": trainable_variables,
                 "non_trainable_variables": non_trainable_variables,
                 "metrics_variables": metrics_variables,
             }
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
 
         # Reattach state back to model (if not already done by a callback).
         self.jax_state_sync()
 
         # The jax spmd_mode is need for multi-process context, since the
         # metrics values are replicated, and we don't want to do a all
         # gather, and only need the local copy of the value.
         with jax.spmd_mode("allow_all"):
-            logs = self.get_metrics_result()
+            logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
         self._jax_state = None
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/numpy/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,18 +265,19 @@
         self.stop_evaluating = False
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         for step, data in epoch_iterator.enumerate_epoch():
             callbacks.on_test_batch_begin(step)
             logs = self.test_function(data)
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def train_on_batch(
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribute_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/name_scope_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer_distribute_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/optimizer_distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/saved_model_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/saved_model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/tensorflow/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,22 +308,21 @@
         for epoch in range(initial_epoch, epochs):
             self.reset_metrics()
             callbacks.on_epoch_begin(epoch)
             with epoch_iterator.catch_stop_iteration():
                 for step, iterator in epoch_iterator.enumerate_epoch():
                     callbacks.on_train_batch_begin(step)
                     logs = self.train_function(iterator)
-                    callbacks.on_train_batch_end(
-                        step, self._pythonify_logs(logs)
-                    )
+                    logs = self._pythonify_logs(logs)
+                    callbacks.on_train_batch_end(step, logs)
                     if self.stop_training:
                         break
 
-            # Override with model metrics instead of last step logs
-            epoch_logs = self.get_metrics_result()
+            # Override with model metrics instead of last step logs if needed.
+            epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
             ):
                 # Create EpochIterator for evaluation and cache it.
                 if getattr(self, "_eval_epoch_iterator", None) is None:
@@ -420,18 +419,19 @@
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         with epoch_iterator.catch_stop_iteration():
             for step, iterator in epoch_iterator.enumerate_epoch():
                 callbacks.on_test_batch_begin(step)
                 logs = self.test_function(iterator)
-                callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+                logs = self._pythonify_logs(logs)
+                callbacks.on_test_batch_end(step, logs)
                 if self.stop_evaluating:
                     break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/core.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/math.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/random.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/backend/torch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,22 +248,23 @@
             # when implementing a custom layer with torch layers.
             self.train()
             for step, data in epoch_iterator.enumerate_epoch():
                 # Callbacks
                 callbacks.on_train_batch_begin(step)
 
                 logs = self.train_function(data)
+                logs = self._pythonify_logs(logs)
 
                 # Callbacks
-                callbacks.on_train_batch_end(step, self._pythonify_logs(logs))
+                callbacks.on_train_batch_end(step, logs)
                 if self.stop_training:
                     break
 
-            # Override with model metrics instead of last step logs
-            epoch_logs = self.get_metrics_result()
+            # Override with model metrics instead of last step logs if needed.
+            epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Switch the torch Module back to testing mode.
             self.eval()
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
@@ -364,18 +365,19 @@
         self.stop_evaluating = False
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         for step, data in epoch_iterator.enumerate_epoch():
             callbacks.on_test_batch_begin(step)
             logs = self.test_function(data)
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/backup_and_restore_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/csv_logger_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/early_stopping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/history.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/lambda_callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/learning_rate_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/model_checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/reduce_lr_on_plateau_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/remote_monitor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/swap_ema_weights_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/tensorboard_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/callbacks/terminate_on_nan_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/constraints/constraints_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/imdb.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/mnist.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/reuters.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/distribution/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/dtype_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,15 @@
                 "'float32'."
             )
 
     def __repr__(self):
         return f'<FloatDTypePolicy "{self._name}">'
 
 
-@keras_export(
-    ["keras.QuantizedDTypePolicy", "keras.dtype_policies.QuantizedDTypePolicy"]
-)
+@keras_export("keras.dtype_policies.QuantizedDTypePolicy")
 class QuantizedDTypePolicy(DTypePolicy):
     def __init__(self, name):
         super().__init__(name)
         self._quantization_mode, self._compute_dtype, self._variable_dtype = (
             self._parse_name(name)
         )
 
@@ -254,20 +252,15 @@
         ]
         # Remove invalid policies
         valid_policies.remove("int8_from_float16")
         valid_policies.remove("int8_from_mixed_float16")
         return valid_policies
 
 
-@keras_export(
-    [
-        "keras.QuantizedFloat8DTypePolicy",
-        "keras.dtype_policies.QuantizedFloat8DTypePolicy",
-    ]
-)
+@keras_export("keras.dtype_policies.QuantizedFloat8DTypePolicy")
 class QuantizedFloat8DTypePolicy(QuantizedDTypePolicy):
     def __init__(self, name, amax_history_length=1024):
         super().__init__(name)
         if not isinstance(amax_history_length, int):
             raise TypeError(
                 "`amax_history_length` must be an integer. "
                 f"Received: amax_history_length={amax_history_length}"
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/dtype_policies/dtype_policy_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/export/export_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/constant_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/initializer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/initializers/random_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/activation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/elu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/leaky_relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/prelu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/activations/softmax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/additive_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/grouped_query_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/attention/multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_transpose_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/conv_transpose_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/depthwise_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/convolutional/separable_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/dense_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/einsum_dense_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/input_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/lambda_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/masking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/core/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/input_spec.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/add.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/average.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/merging_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/merging_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/batch_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/group_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/layer_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/spectral_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/normalization/unit_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/global_max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/pooling/max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/audio_preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/category_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/discretization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/feature_space_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashed_crossing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/hashing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/index_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/integer_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_brightness_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_rotation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_translation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/random_zoom_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/rescaling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/resizing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/string_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/text_vectorization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/activity_regularization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/alpha_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/gaussian_noise_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/regularization/spatial_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/cropping3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/flatten_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/permute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/repeat_vector_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/reshape_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/up_sampling3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/reshaping/zero_padding3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/bidirectional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/conv_lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/dropout_rnn_cell_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/gru_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/simple_rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/stacked_rnn_cells_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/layers/rnn/time_distributed_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/backend.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/layers.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/losses.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/legacy_h5_format_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/losses/loss_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/accuracy_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/confusion_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/f_score_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/hinge_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/iou_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metric_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/probabilistic_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/reduction_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/metrics/regression_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/cloning_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/functional.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/functional_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/functional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/model.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/model_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/sequential_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/models/variable_mapping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/core.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/core_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/core_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/function.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/function_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/function_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/image.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/image_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/image_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/linalg_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/math.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/math_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/math_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/nn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/node.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/node_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/node_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/numpy_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/operation_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/ops/symbolic_arguments_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adadelta_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adafactor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adagrad_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/adamw_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/ftrl_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/lion_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/loss_scale_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/nadam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_sparse_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer_sparse_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/rmsprop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/schedules/learning_rate_schedule_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/optimizers/sgd_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/quantizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         Returns:
             Python dictionary.
         """
         raise NotImplementedError(f"{self} does not implement get_config()")
 
 
-@keras_export(["keras.quantizers.abs_max_quantize"])
+@keras_export("keras.quantizers.abs_max_quantize")
 def abs_max_quantize(
     inputs,
     axis,
     value_range=(-127, 127),
     dtype="int8",
     epsilon=backend.epsilon(),
 ):
@@ -71,15 +71,15 @@
     )
     outputs = ops.multiply(inputs, scale)
     outputs = ops.clip(ops.round(outputs), value_range[0], value_range[1])
     outputs = ops.cast(outputs, dtype)
     return outputs, scale
 
 
-@keras_export(["keras.AbsMaxQuantizer", "keras.quantizers.AbsMaxQuantizer"])
+@keras_export("keras.quantizers.AbsMaxQuantizer")
 class AbsMaxQuantizer(Quantizer):
     def __init__(
         self,
         axis,
         value_range=(-127, 127),
         epsilon=backend.epsilon(),
         output_dtype="int8",
@@ -105,39 +105,39 @@
             "output_dtype": self.output_dtype,
         }
 
 
 """Float8-related methods"""
 
 
-@keras_export(["keras.quantizers.compute_float8_scale"])
+@keras_export("keras.quantizers.compute_float8_scale")
 def compute_float8_scale(amax, scale, dtype_max, margin=0):
     # The algorithm for computing the new scale is sourced from
     # https://docs.nvidia.com/deeplearning/transformer-engine/user-guide/api/jax.html#transformer_engine.jax.update_fp8_metas
     # wherein the `original_scale` corresponds to the reciprocal of the
     # `scale` passed in this function.
     scale = ops.reciprocal(scale)
     sf = ops.divide(ops.divide(dtype_max, amax), 2**margin)
     sf = ops.where(amax > 0.0, sf, scale)
     sf = ops.where(ops.isfinite(amax), sf, scale)
     return ops.reciprocal(sf)
 
 
-@keras_export(["keras.quantizers.compute_float8_amax_history"])
+@keras_export("keras.quantizers.compute_float8_amax_history")
 def compute_float8_amax_history(x, amax_history):
     amax_update = ops.cast(ops.max(ops.abs(x)), amax_history.dtype)
     new_amax_history = ops.scatter_update(
         ops.roll(amax_history, shift=-1),
         [[0]],
         ops.reshape(amax_update, [1]),
     )
     return new_amax_history
 
 
-@keras_export(["keras.quantizers.quantize_and_dequantize"])
+@keras_export("keras.quantizers.quantize_and_dequantize")
 def quantize_and_dequantize(inputs, scale, quantized_dtype, compute_dtype):
     # Quantize
     quantized_dtype_max = ops.cast(
         float(ml_dtypes.finfo(quantized_dtype).max), compute_dtype
     )
     x = ops.divide(inputs, ops.cast(scale, compute_dtype))
     x = ops.clip(x, -quantized_dtype_max, quantized_dtype_max)
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/quantizers/quantizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/random/random.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/random/random_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/random/random_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/random/seed_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/regularizers/regularizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/object_registration_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_api_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/saving_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/saving/serialization_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_case.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/testing/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/compile_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/generator_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/py_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/epoch_iterator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -895,14 +895,45 @@
                 try:
                     value = float(value)
                 except:
                     pass
                 result[key] = value
         return result
 
+    def _get_metrics_result_or_logs(self, logs):
+        """Returns model metrics as a dict if the keys match with input logs.
+
+        When the training / evalution is performed with an asynchronous steps,
+        the last scheduled `train / test_step` may not give the latest metrics
+        because it is not guaranteed to be executed the last. This method gets
+        metrics from the model directly instead of relying on the return from
+        last step function.
+
+        When the user has custom train / test step functions, the metrics
+        returned may be different from `Model.metrics`. In those instances,
+        this function will be no-op and return the logs passed in.
+
+        Args:
+            logs: A `dict` of metrics returned by train / test step function.
+
+        Returns:
+            A `dict` containing values of the metrics listed in `self.metrics`
+            when logs and model metrics keys match. Otherwise it returns input
+            `logs`.
+        """
+        metric_logs = self.get_metrics_result()
+        # Verify that train / test step logs passed and metric logs have
+        # matching keys. It could be different when using custom step functions,
+        # in which case we return the logs from the last step.
+        if isinstance(logs, dict) and set(logs.keys()) == set(
+            metric_logs.keys()
+        ):
+            return metric_logs
+        return logs
+
     def _flatten_metrics_in_order(self, logs):
         """Turns `logs` dict into a list as per key order of `metrics_names`."""
         metric_names = []
         for metric in self.metrics:
             if isinstance(metric, CompileMetrics):
                 metric_names += [
                     sub_metric.name for sub_metric in metric.metrics
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/trainers/trainer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,38 @@
             units=units,
             use_bias=False,
             kernel_initializer=initializers.Ones(),
         )
         Trainer.__init__(self)
 
 
+class CustomTrainTestStepModel(ExampleModel):
+    def train_step(self, data):
+        logs = super().train_step(data)
+        logs["my_custom_metric"] = 10.0
+        return logs
+
+    def test_step(self, data):
+        logs = super().test_step(data)
+        logs["my_custom_metric"] = 5.0
+        return logs
+
+
+class JaxCustomTrainTestStepModel(ExampleModel):
+    def train_step(self, state, data):
+        logs, state = super().train_step(state, data)
+        logs["my_custom_metric"] = 10.0
+        return logs, state
+
+    def test_step(self, state, data):
+        logs, state = super().test_step(state, data)
+        logs["my_custom_metric"] = 5.0
+        return logs, state
+
+
 class StructModel(Trainer, layers.Layer):
     def __init__(self, units):
         layers.Layer.__init__(self)
         Trainer.__init__(self)
         self.dense_1 = layers.Dense(
             units,
             use_bias=False,
@@ -304,14 +328,35 @@
             epochs=epochs,
             validation_split=0.2,
         )
         history = history.history
         self.assertIn("loss", history)
         self.assertIn("val_loss", history)
 
+    @pytest.mark.requires_trainable_backend
+    def test_fit_with_custom_train_step(self):
+        if backend.backend() == "jax":
+            model = JaxCustomTrainTestStepModel(units=3)
+        else:
+            model = CustomTrainTestStepModel(units=3)
+        x = np.ones((100, 4))
+        y = np.zeros((100, 3))
+        batch_size = 16
+
+        model.compile(
+            optimizer=optimizers.SGD(),
+            loss=losses.MeanSquaredError(),
+            metrics=[metrics.MeanSquaredError()],
+        )
+        history = model.fit(x, y, batch_size=batch_size)
+        history = history.history
+        self.assertIn("loss", history)
+        self.assertIn("mean_squared_error", history)
+        self.assertAllClose(history["my_custom_metric"], 10.0)
+
     @parameterized.named_parameters(
         named_product(
             generator_type=["tf", "jax", "scipy"], mode=["eager", "graph"]
         )
     )
     @pytest.mark.skipif(
         not backend.SUPPORTS_SPARSE_TENSORS,
@@ -371,14 +416,39 @@
         self.assertAllClose(output, [16.0, 16.0])
         output = model.evaluate(x, y, batch_size=batch_size, return_dict=True)
         self.assertIsInstance(output, dict)
         self.assertIn("loss", output)
         self.assertIn("mean_squared_error", output)
         self.assertAllClose(output["mean_squared_error"], 16.0)
 
+    @parameterized.named_parameters([("flat", False), ("dict", True)])
+    @pytest.mark.requires_trainable_backend
+    def test_evaluate_with_custom_test_step(self, return_dict):
+        if backend.backend() == "jax":
+            model = JaxCustomTrainTestStepModel(units=3)
+        else:
+            model = CustomTrainTestStepModel(units=3)
+        x = np.ones((100, 4))
+        y = np.zeros((100, 3))
+        batch_size = 16
+
+        model.compile(
+            optimizer=optimizers.SGD(),
+            loss=losses.MeanSquaredError(),
+            metrics=[metrics.MeanSquaredError()],
+        )
+        output = model.evaluate(
+            x, y, batch_size=batch_size, return_dict=return_dict
+        )
+        self.assertLen(output, 3)
+        if return_dict:
+            self.assertAllClose(output["my_custom_metric"], 5.0)
+        else:
+            self.assertAllClose(output[-1], 5.0)  # Custom metrics go last.
+
     @parameterized.named_parameters(
         named_product(
             generator_type=["tf", "jax", "scipy"], mode=["eager", "graph"]
         )
     )
     @pytest.mark.skipif(
         not backend.SUPPORTS_SPARSE_TENSORS,
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_api.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/tree/tree_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/audio_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/code_stats_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/dtype_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/file_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/jax_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/module_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/naming_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/numerical_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/progbar.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/rng_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/sequence_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/text_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/timeseries_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/torch_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking_test.py` & `keras_nightly-3.3.0.dev2024041703/keras/src/utils/tracking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041622
+Version: 3.3.0.dev2024041703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -76,14 +76,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.0.dev2024041703/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/pyproject.toml` & `keras_nightly-3.3.0.dev2024041703/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041622/setup.py` & `keras_nightly-3.3.0.dev2024041703/setup.py`

 * *Files identical despite different names*

