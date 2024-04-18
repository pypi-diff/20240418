# Comparing `tmp/haliax-1.4.dev291.tar.gz` & `tmp/haliax-1.4.dev292.tar.gz`

## Comparing `haliax-1.4.dev291.tar` & `haliax-1.4.dev292.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.coveragerc
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.flake8
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.pre-commit-config.yaml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.readthedocs.yaml
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev291/CONTRIBUTING.md
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev291/mkdocs.yml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/publish_dev.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/run_pre_commit.yaml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/run_tests.yaml
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/api.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/broadcasting.md
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/cheatsheet.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/faq.md
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/fp8.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/hof.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/index.md
--rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/indexing.md
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/matmul.md
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/nn.md
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/partitioning.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/rearrange.ipynb
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/rearrange.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/requirements.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/tutorial.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/css/material.css
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/data_parallel_mesh.png
--rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/data_parallel_mesh_replicated.png
--rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_1d.png
--rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_1d_zero.png
--rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_batch_partitioned.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated.png
--rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
--rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
--rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_zero.png
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/__about__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/__init__.py
--rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/axis.py
--rw-r--r--   0        0        0    67867 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/core.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/debug.py
--rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/hof.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/jax_utils.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/ops.py
--rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/partitioning.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/quantization.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/random.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/specialized_fns.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/tree_util.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/types.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/util.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/__init__.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/compile_utils.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/dot.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/einsum.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/fp8.py
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/parsing.py
--rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/rearrange.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/util.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/activations.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/attention.py
--rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/conv.py
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/dropout.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/embedding.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/linear.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/loss.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/mlp.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/normalization.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/pool.py
--rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/scan.py
--rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/core_test.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_attention.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_axis.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_conv.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_debug.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_dot.py
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_einsum.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_fp8.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_hof.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_nn.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_ops.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_parsing.py
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_partitioning.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_pool.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_random.py
--rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_rearrange.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_scan.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_specialized_fns.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_tree_util.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev291/LICENSE
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev291/README.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev291/pyproject.toml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev291/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.coveragerc
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.flake8
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.readthedocs.yaml
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev292/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev292/mkdocs.yml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.github/workflows/publish_dev.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.github/workflows/run_pre_commit.yaml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/api.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/broadcasting.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/cheatsheet.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/faq.md
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/fp8.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/hof.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/index.md
+-rw-r--r--   0        0        0    11288 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/indexing.md
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/matmul.md
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/nn.md
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/partitioning.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/rearrange.ipynb
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/rearrange.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/tutorial.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/css/material.css
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/data_parallel_mesh.png
+-rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/data_parallel_mesh_replicated.png
+-rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_1d.png
+-rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_1d_zero.png
+-rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d_batch_partitioned.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d_data_replicated.png
+-rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
+-rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
+-rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev292/docs/figures/device_mesh_2d_zero.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/__about__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/__init__.py
+-rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/axis.py
+-rw-r--r--   0        0        0    67867 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/core.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/debug.py
+-rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/hof.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/jax_utils.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/ops.py
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/partitioning.py
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/quantization.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/random.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/specialized_fns.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/tree_util.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/types.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/util.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/compile_utils.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/dot.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/einsum.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/fp8.py
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/parsing.py
+-rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/rearrange.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/_src/util.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/activations.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/attention.py
+-rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/conv.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/dropout.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/embedding.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/linear.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/loss.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/mlp.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/normalization.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/pool.py
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev292/src/haliax/nn/scan.py
+-rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/core_test.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_attention.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_axis.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_conv.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_debug.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_dot.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_einsum.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_fp8.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_hof.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_nn.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_ops.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_parsing.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_partitioning.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_pool.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_random.py
+-rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_rearrange.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_scan.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_specialized_fns.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_tree_util.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev292/tests/test_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev292/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev292/LICENSE
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev292/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev292/pyproject.toml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev292/PKG-INFO
```

### Comparing `haliax-1.4.dev291/.pre-commit-config.yaml` & `haliax-1.4.dev292/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/CONTRIBUTING.md` & `haliax-1.4.dev292/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/mkdocs.yml` & `haliax-1.4.dev292/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/.github/workflows/publish_dev.yaml` & `haliax-1.4.dev292/.github/workflows/publish_dev.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/.github/workflows/run_pre_commit.yaml` & `haliax-1.4.dev292/.github/workflows/run_pre_commit.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/.github/workflows/run_tests.yaml` & `haliax-1.4.dev292/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/api.md` & `haliax-1.4.dev292/docs/api.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/broadcasting.md` & `haliax-1.4.dev292/docs/broadcasting.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/cheatsheet.md` & `haliax-1.4.dev292/docs/cheatsheet.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/faq.md` & `haliax-1.4.dev292/docs/faq.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/fp8.md` & `haliax-1.4.dev292/docs/fp8.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/indexing.md` & `haliax-1.4.dev292/docs/indexing.md`

 * *Files 3% similar despite different names*

```diff
@@ -149,17 +149,19 @@
 
 It's not a huge improvement, but it's a bit more convenient.
 
 
 ## Advanced Indexing
 
 NumPy's [Advanced Indexing](https://numpy.org/doc/stable/user/basics.indexing.html#advanced-indexing) is supported, though we use named arrays for the indices instead of normal arrays.
-In NumPy, the indexed arrays much be broadcastable to the same shape.Advanced indexing in Haliax is similar, except that
-they follow Haliax's broadcasting rules, meaning that the axis names determine broadcasting.Axes with the same name must
-have the same size.
+(Though, as noted above, you can use 1-D JAX arrays of integers as well.)
+In NumPy, the indexed arrays must be broadcastable to the same shape. Advanced indexing in Haliax is similar,
+except that it follows Haliax's broadcasting rules, meaning that shared names are broadcasted together,
+while non-shared names are treated as separate axes and are cross-producted.
+In particular, axes with the same name must have the same size.
 
 ```python
 import haliax as hax
 import jax
 
 X = hax.Axis("X", 10)
 Y = hax.Axis("Y", 20)
```

### Comparing `haliax-1.4.dev291/docs/matmul.md` & `haliax-1.4.dev292/docs/matmul.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/nn.md` & `haliax-1.4.dev292/docs/nn.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/partitioning.md` & `haliax-1.4.dev292/docs/partitioning.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/rearrange.ipynb` & `haliax-1.4.dev292/docs/rearrange.ipynb`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/rearrange.md` & `haliax-1.4.dev292/docs/rearrange.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/css/material.css` & `haliax-1.4.dev292/docs/css/material.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/css/mkdocstrings.css` & `haliax-1.4.dev292/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/data_parallel_mesh.png` & `haliax-1.4.dev292/docs/figures/data_parallel_mesh.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/data_parallel_mesh_replicated.png` & `haliax-1.4.dev292/docs/figures/data_parallel_mesh_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_1d.png` & `haliax-1.4.dev292/docs/figures/device_mesh_1d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_1d_zero.png` & `haliax-1.4.dev292/docs/figures/device_mesh_1d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d_batch_partitioned.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d_batch_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d_data_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/docs/figures/device_mesh_2d_zero.png` & `haliax-1.4.dev292/docs/figures/device_mesh_2d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/__init__.py` & `haliax-1.4.dev292/src/haliax/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/axis.py` & `haliax-1.4.dev292/src/haliax/axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/core.py` & `haliax-1.4.dev292/src/haliax/core.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/debug.py` & `haliax-1.4.dev292/src/haliax/debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/hof.py` & `haliax-1.4.dev292/src/haliax/hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/jax_utils.py` & `haliax-1.4.dev292/src/haliax/jax_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/ops.py` & `haliax-1.4.dev292/src/haliax/ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/partitioning.py` & `haliax-1.4.dev292/src/haliax/partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/quantization.py` & `haliax-1.4.dev292/src/haliax/quantization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/random.py` & `haliax-1.4.dev292/src/haliax/random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/specialized_fns.py` & `haliax-1.4.dev292/src/haliax/specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/tree_util.py` & `haliax-1.4.dev292/src/haliax/tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/types.py` & `haliax-1.4.dev292/src/haliax/types.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/util.py` & `haliax-1.4.dev292/src/haliax/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/wrap.py` & `haliax-1.4.dev292/src/haliax/wrap.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/compile_utils.py` & `haliax-1.4.dev292/src/haliax/_src/compile_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/dot.py` & `haliax-1.4.dev292/src/haliax/_src/dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/einsum.py` & `haliax-1.4.dev292/src/haliax/_src/einsum.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/fp8.py` & `haliax-1.4.dev292/src/haliax/_src/fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/parsing.py` & `haliax-1.4.dev292/src/haliax/_src/parsing.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/rearrange.py` & `haliax-1.4.dev292/src/haliax/_src/rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/_src/util.py` & `haliax-1.4.dev292/src/haliax/_src/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/__init__.py` & `haliax-1.4.dev292/src/haliax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/activations.py` & `haliax-1.4.dev292/src/haliax/nn/activations.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/attention.py` & `haliax-1.4.dev292/src/haliax/nn/attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/conv.py` & `haliax-1.4.dev292/src/haliax/nn/conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/dropout.py` & `haliax-1.4.dev292/src/haliax/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/embedding.py` & `haliax-1.4.dev292/src/haliax/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/linear.py` & `haliax-1.4.dev292/src/haliax/nn/linear.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/loss.py` & `haliax-1.4.dev292/src/haliax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/mlp.py` & `haliax-1.4.dev292/src/haliax/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/normalization.py` & `haliax-1.4.dev292/src/haliax/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/pool.py` & `haliax-1.4.dev292/src/haliax/nn/pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/src/haliax/nn/scan.py` & `haliax-1.4.dev292/src/haliax/nn/scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/core_test.py` & `haliax-1.4.dev292/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_attention.py` & `haliax-1.4.dev292/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_axis.py` & `haliax-1.4.dev292/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_conv.py` & `haliax-1.4.dev292/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_debug.py` & `haliax-1.4.dev292/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_dot.py` & `haliax-1.4.dev292/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_einsum.py` & `haliax-1.4.dev292/tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_fp8.py` & `haliax-1.4.dev292/tests/test_fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_hof.py` & `haliax-1.4.dev292/tests/test_hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_nn.py` & `haliax-1.4.dev292/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_ops.py` & `haliax-1.4.dev292/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_parsing.py` & `haliax-1.4.dev292/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_partitioning.py` & `haliax-1.4.dev292/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_pool.py` & `haliax-1.4.dev292/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_random.py` & `haliax-1.4.dev292/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_rearrange.py` & `haliax-1.4.dev292/tests/test_rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_scan.py` & `haliax-1.4.dev292/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_specialized_fns.py` & `haliax-1.4.dev292/tests/test_specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/tests/test_tree_util.py` & `haliax-1.4.dev292/tests/test_tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/.gitignore` & `haliax-1.4.dev292/.gitignore`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/LICENSE` & `haliax-1.4.dev292/LICENSE`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/README.md` & `haliax-1.4.dev292/README.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/pyproject.toml` & `haliax-1.4.dev292/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev291/PKG-INFO` & `haliax-1.4.dev292/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haliax
-Version: 1.4.dev291
+Version: 1.4.dev292
 Summary: Named Tensors for Legible Deep Learning in JAX
 Project-URL: Homepage, https://github.com/stanford-crfm/haliax
 Project-URL: Bug Tracker, https://github.com/stanford-crfm/haliax/issues/
 Author-email: David Hall <dlwh@cs.stanford.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

