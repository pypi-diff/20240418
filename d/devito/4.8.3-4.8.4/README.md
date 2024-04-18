# Comparing `tmp/devito-4.8.3.tar.gz` & `tmp/devito-4.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devito-4.8.3.tar", last modified: Mon Oct 16 12:28:13 2023, max compression
+gzip compressed data, was "devito-4.8.4.tar", last modified: Thu Apr 18 12:32:16 2024, max compression
```

## Comparing `devito-4.8.3.tar` & `devito-4.8.4.tar`

### file list

```diff
@@ -1,254 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-16 12:28:02.000000 devito-4.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-16 12:28:02.000000 devito-4.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-16 12:28:13.684351 devito-4.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-10-16 12:28:02.000000 devito-4.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/benchmarks/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/benchmarks/user/advisor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/advisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/advisor/advisor_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/advisor/roofline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/advisor/run_advisor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-10-16 12:28:02.000000 devito-4.8.3/benchmarks/user/make-pbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/devito/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-10-16 12:28:02.000000 devito-4.8.3/devito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-16 12:28:13.684351 devito-4.8.3/devito/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/devito/arch/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-16 12:28:02.000000 devito-4.8.3/devito/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25042 2023-10-16 12:28:02.000000 devito-4.8.3/devito/arch/archinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    31849 2023-10-16 12:28:02.000000 devito-4.8.3/devito/arch/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/devito/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-16 12:28:02.000000 devito-4.8.3/devito/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2023-10-16 12:28:02.000000 devito-4.8.3/devito/builtins/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2023-10-16 12:28:02.000000 devito-4.8.3/devito/builtins/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2023-10-16 12:28:02.000000 devito-4.8.3/devito/builtins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/devito/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-16 12:28:02.000000 devito-4.8.3/devito/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2023-10-16 12:28:02.000000 devito-4.8.3/devito/checkpointing/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/devito/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/autotuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/intel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-16 12:28:02.000000 devito-4.8.3/devito/core/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/data/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14987 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/allocators.py
--rw-r--r--   0 runner    (1001) docker     (127)    26477 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20653 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2023-10-16 12:28:02.000000 devito-4.8.3/devito/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-16 12:28:02.000000 devito-4.8.3/devito/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/finite_differences/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/derivative.py
--rw-r--r--   0 runner    (1001) docker     (127)    26015 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/differentiable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14838 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/elementary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2023-10-16 12:28:02.000000 devito-4.8.3/devito/finite_differences/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/clusters/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/clusters/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/clusters/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/clusters/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/equations/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/equations/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/equations/equation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/iet/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/efunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39452 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42512 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/iet/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/stree/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/stree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/stree/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/stree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/ir/support/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38423 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/guards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    30280 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/symregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/syncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2023-10-16 12:28:02.000000 devito-4.8.3/devito/ir/support/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-10-16 12:28:02.000000 devito-4.8.3/devito/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.672351 devito-4.8.3/devito/mpatches/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpatches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpatches/rationaltools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23248 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpi/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    24942 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpi/halo_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    45388 2023-10-16 12:28:02.000000 devito-4.8.3/devito/mpi/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/operations/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14741 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operations/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operations/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45297 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operator/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19899 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operator/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-10-16 12:28:02.000000 devito-4.8.3/devito/operator/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2023-10-16 12:28:02.000000 devito-4.8.3/devito/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/passes/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/passes/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51852 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (127)    16665 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)    28743 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/buffering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/cse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/factorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17835 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/unevaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/clusters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/passes/equations/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/equations/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/passes/iet/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (127)    21305 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13974 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/langbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.676351 devito-4.8.3/devito/passes/iet/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/languages/C.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/languages/openacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/languages/openmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/languages/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/linearization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27691 2023-10-16 12:28:02.000000 devito-4.8.3/devito/passes/iet/parpragma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/devito/symbolics/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17323 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/extended_sympy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15326 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-16 12:28:02.000000 devito-4.8.3/devito/symbolics/unevaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/devito/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/dtypes_lowering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/os_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2023-10-16 12:28:02.000000 devito-4.8.3/devito/tools/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/devito/types/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    47686 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    62937 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    50960 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    29251 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)    82404 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    13502 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-10-16 12:28:02.000000 devito-4.8.3/devito/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.668351 devito-4.8.3/devito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-16 12:28:13.000000 devito-4.8.3/devito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-10-16 12:28:13.000000 devito-4.8.3/devito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 12:28:13.000000 devito-4.8.3/devito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-10-16 12:28:13.000000 devito-4.8.3/devito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-16 12:28:13.000000 devito-4.8.3/devito.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.664351 devito-4.8.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/examples/cfd/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-16 12:28:02.000000 devito-4.8.3/examples/cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-10-16 12:28:02.000000 devito-4.8.3/examples/cfd/example_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2023-10-16 12:28:02.000000 devito-4.8.3/examples/cfd/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/examples/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/examples/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/examples/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-10-16 12:28:02.000000 devito-4.8.3/examples/misc/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/examples/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/examples/mpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.680351 devito-4.8.3/examples/performance/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-16 12:28:02.000000 devito-4.8.3/examples/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-10-16 12:28:02.000000 devito-4.8.3/examples/performance/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/acoustic/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/acoustic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/acoustic/acoustic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/acoustic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/acoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/elastic/elastic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/elastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/elastic/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15675 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/preset_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/self_adjoint/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/example_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18618 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/test_wavesolver_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/self_adjoint/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/test_seismic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/tti/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/tti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26009 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/tti/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/tti/tti_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15989 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/tti/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/viscoacoustic/
--rwxr-xr-x   0 runner    (1001) docker     (127)      112 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoacoustic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22768 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoacoustic/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3351 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoacoustic/viscoacoustic_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17366 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoacoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/seismic/viscoelastic/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoelastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoelastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoelastic/viscoelastic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2023-10-16 12:28:02.000000 devito-4.8.3/examples/seismic/viscoelastic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:13.684351 devito-4.8.3/examples/userapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 12:28:02.000000 devito-4.8.3/examples/userapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-16 12:28:02.000000 devito-4.8.3/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-16 12:28:02.000000 devito-4.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-16 12:28:13.684351 devito-4.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-10-16 12:28:02.000000 devito-4.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68635 2023-10-16 12:28:02.000000 devito-4.8.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.531878 devito-4.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 12:32:08.000000 devito-4.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 12:32:08.000000 devito-4.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 12:32:16.531878 devito-4.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 12:32:08.000000 devito-4.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/benchmarks/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/benchmarks/user/advisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/advisor_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/roofline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/run_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/make-pbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-18 12:32:08.000000 devito-4.8.4/devito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 12:32:16.531878 devito-4.8.4/devito/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/archinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34728 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 12:32:08.000000 devito-4.8.4/devito/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-18 12:32:08.000000 devito-4.8.4/devito/checkpointing/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/autotuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/intel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/allocators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 12:32:08.000000 devito-4.8.4/devito/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/finite_differences/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31997 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/differentiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/elementary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/rsfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/equations/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/equation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/iet/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/efunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42683 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/ir/stree/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/ir/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47211 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/guards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32039 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/symregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 12:32:08.000000 devito-4.8.4/devito/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/mpatches/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpatches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpatches/rationaltools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23631 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25197 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/halo_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46775 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-18 12:32:08.000000 devito-4.8.4/devito/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/passes/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50437 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/cse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/factorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/unevaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/equations/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/equations/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/iet/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17777 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/langbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/iet/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/C.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/openacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/parpragma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.503878 devito-4.8.4/devito/symbolics/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/extended_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/unevaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.503878 devito-4.8.4/devito/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23684 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/dtypes_lowering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/os_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.507878 devito-4.8.4/devito/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50787 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53530 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84563 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.527878 devito-4.8.4/devito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/example_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-18 12:32:08.000000 devito-4.8.4/examples/misc/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/mpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 12:32:08.000000 devito-4.8.4/examples/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 12:32:08.000000 devito-4.8.4/examples/performance/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/seismic/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/seismic/acoustic/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/acoustic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/elastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17436 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/preset_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/self_adjoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/example_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/test_wavesolver_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/test_seismic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/tti/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/tti_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/viscoacoustic/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22768 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3351 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/viscoacoustic_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17366 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/viscoelastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/viscoelastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/userapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/userapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 12:32:08.000000 devito-4.8.4/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 12:32:08.000000 devito-4.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 12:32:16.531878 devito-4.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-18 12:32:08.000000 devito-4.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.527878 devito-4.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22230 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_cinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65948 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35428 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_differentiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69440 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55068 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116568 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_error_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_fission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57869 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_openacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_iet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37983 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_lower_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_lower_exprs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101814 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78996 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29848 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_roundoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_skewing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_staggered_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_subdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_symbolic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_symbolics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_timestepping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_unexpansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-18 12:32:08.000000 devito-4.8.4/versioneer.py
```

### Comparing `devito-4.8.3/LICENSE.md` & `devito-4.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/README.md` & `devito-4.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ```
 
 An `Operator` generates low-level code from an ordered collection of `Eq` (the
 example above being for a single equation). This code may also be compiled and
 executed
 
 ```python
->>> op(t=timesteps)
+>>> op(t=timesteps, dt=dt)
 ```
 
 There is virtually no limit to the complexity of an `Operator` -- the Devito
 compiler will automatically analyze the input, detect and apply optimizations
 (including single- and multi-node parallelism), and eventually generate code
 with suitable loops and expressions.
```

### Comparing `devito-4.8.3/benchmarks/user/advisor/advisor_logging.py` & `devito-4.8.4/benchmarks/user/advisor/advisor_logging.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/benchmarks/user/advisor/roofline.py` & `devito-4.8.4/benchmarks/user/advisor/roofline.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/benchmarks/user/advisor/run_advisor.py` & `devito-4.8.4/benchmarks/user/advisor/run_advisor.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/benchmarks/user/benchmark.py` & `devito-4.8.4/benchmarks/user/benchmark.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/benchmarks/user/make-pbs.py` & `devito-4.8.4/benchmarks/user/make-pbs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/__init__.py` & `devito-4.8.4/devito/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from itertools import product
+from . import _version
 
 # Import the global `configuration` dict
 from devito.parameters import *  # noqa
 
 # DSL imports
 from devito.types import NODE, CELL, Buffer  # noqa
 from devito.types.caching import _SymbolCache, CacheManager  # noqa
@@ -18,15 +19,15 @@
 from devito.operations.solve import *
 from devito.operator import Operator  # noqa
 
 # Other stuff exposed to the user
 from devito.builtins import *  # noqa
 from devito.data.allocators import *  # noqa
 from devito.logger import error, warning, info, set_log_level  # noqa
-from devito.mpi import MPI  # noqa
+from devito.mpi import MPI, CustomTopology  # noqa
 try:
     from devito.checkpointing import DevitoCheckpoint, CheckpointOperator  # noqa
     from pyrevolve import Revolver
 except ImportError:
     from devito.checkpointing import NoopCheckpoint as DevitoCheckpoint  # noqa
     from devito.checkpointing import NoopCheckpointOperator as CheckpointOperator  # noqa
     from devito.checkpointing import NoopRevolver as Revolver  # noqa
@@ -117,17 +118,18 @@
 levels = ['off', 'basic', 'aggressive', 'max']
 modes = ['preemptive', 'destructive', 'runtime']
 accepted = levels + [list(i) for i in product(levels, modes)]
 configuration.add('autotuning', 'off', accepted, callback=autotune_callback,
                   impacts_jit=False)
 
 # In develop-mode:
-# - Some optimizations may not be applied to the generated code.
-# - The compiler performs more type and value checking
-configuration.add('develop-mode', True, [False, True])
+# - The ALLOC_GUARD data allocator is used. This will trigger segfaults as soon
+#   as an out-of-bounds memory access is performed
+# - Some autoi-tuning optimizations are disabled
+configuration.add('develop-mode', False, [False, True])
 
 # Setup optimization level
 configuration.add('opt', 'advanced', list(operator_registry._accepted), deprecate='dle')
 configuration.add('opt-options', {}, deprecate='dle-options')
 
 # Setup Operator profiling
 configuration.add('profiling', 'basic', list(profiler_registry), impacts_jit=False)
@@ -151,7 +153,10 @@
     also employs suitable NUMA strategies for memory allocation.
     """
     configuration['develop-mode'] = False
     configuration['autotuning'] = 'aggressive'
     # With the autotuner in `aggressive` mode, a more aggressive blocking strategy
     # which also tiles the innermost loop) is beneficial
     configuration['opt-options']['blockinner'] = True
+
+
+__version__ = _version.get_versions()['version']
```

### Comparing `devito-4.8.3/devito/arch/archinfo.py` & `devito-4.8.4/devito/arch/archinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 import cpuinfo
 import ctypes
 import numpy as np
 import psutil
 import re
 import os
 import sys
+import json
 
 from devito.logger import warning
 from devito.tools import as_tuple, all_equal, memoized_func
 
 __all__ = ['platform_registry', 'get_cpu_info', 'get_gpu_info', 'get_nvidia_cc',
            'get_cuda_path', 'get_hip_path', 'check_cuda_runtime', 'get_m1_llvm_path',
            'Platform', 'Cpu64', 'Intel64', 'IntelSkylake', 'Amd', 'Arm', 'Power',
            'Device', 'NvidiaDevice', 'AmdDevice', 'IntelDevice',
-           # Intel
+           # Intel CPUs
            'INTEL64', 'SNB', 'IVB', 'HSW', 'BDW', 'KNL', 'KNL7210',
            'SKX', 'KLX', 'CLX', 'CLK', 'SPR',
-           # ARM
-           'AMD', 'ARM', 'M1', 'GRAVITON',
-           # Other loosely supported CPU architectures
+           # ARM CPUs
+           'AMD', 'ARM', 'AppleArm', 'M1', 'M2', 'M3', 'GRAVITON',
+           # Other legacy CPUs
            'POWER8', 'POWER9',
-           # GPUs
-           'AMDGPUX', 'NVIDIAX', 'INTELGPUX']
+           # Generic GPUs
+           'AMDGPUX', 'NVIDIAX', 'INTELGPUX',
+           # Intel GPUs
+           'PVC', 'INTELGPUMAX', 'MAX1100', 'MAX1550']
 
 
 @memoized_func
 def get_cpu_info():
     """Attempt CPU info autodetection."""
 
     # Obtain textual cpu info
@@ -243,14 +246,85 @@
             gpu_info['mem.%s' % i] = make_cbk(i)
 
         return gpu_info
 
     except OSError:
         pass
 
+    # *** Second try: `rocm-smi`, clearly only works with AMD cards
+    try:
+        gpu_infos = {}
+
+        # Base gpu info
+        info_cmd = ['rocm-smi', '--showproductname']
+        proc = Popen(info_cmd, stdout=PIPE, stderr=DEVNULL)
+        raw_info = str(proc.stdout.read())
+
+        lines = raw_info.replace('\\n', '\n').replace('b\'', '').replace('\\t', '')
+        lines = lines.splitlines()
+
+        for line in lines:
+            if 'GPU' in line:
+                # Product
+                pattern = r'GPU\[(\d+)\].*?Card series:\s*(.*?)\s*$'
+                match1 = re.match(pattern, line)
+
+                if match1:
+                    gid = match1.group(1)
+                    gpu_infos.setdefault(gid, dict())
+                    gpu_infos[gid]['physicalid'] = gid
+                    gpu_infos[gid]['product'] = match1.group(2)
+
+                # Model
+                pattern = r'GPU\[(\d+)\].*?Card model:\s*(.*?)\s*$'
+                match2 = re.match(pattern, line)
+
+                if match2:
+                    gid = match2.group(1)
+                    gpu_infos.setdefault(gid, dict())
+                    gpu_infos[gid]['physicalid'] = match2.group(1)
+                    gpu_infos[gid]['model'] = match2.group(2)
+
+        gpu_info = homogenise_gpus(list(gpu_infos.values()))
+
+        # Also attach callbacks to retrieve instantaneous memory info
+        info_cmd = ['rocm-smi', '--showmeminfo', 'vram', '--json']
+        proc = Popen(info_cmd, stdout=PIPE, stderr=DEVNULL)
+        raw_info = str(proc.stdout.read())
+        lines = raw_info.replace('\\n', '').replace('b\'', '').replace('\'', '')
+        info = json.loads(lines)
+
+        for i in ['total', 'free', 'used']:
+            def make_cbk(i):
+                def cbk(deviceid=0):
+                    try:
+                        # Should only contain Used and total
+                        assert len(info['card%s' % deviceid]) == 2
+                        used = [int(v) for k, v in info['card%s' % deviceid].items()
+                                if 'Used' in k][0]
+                        total = [int(v) for k, v in info['card%s' % deviceid].items()
+                                 if 'Used' not in k][0]
+                        free = total - used
+                        return {'total': total, 'free': free, 'used': used}[i]
+                    except:
+                        # We shouldn't really end up here, unless nvidia-smi changes
+                        # the output format (though we still have tests in place that
+                        # will catch this)
+                        return None
+
+                return cbk
+
+            gpu_info['mem.%s' % i] = make_cbk(i)
+
+        gpu_infos['architecture'] = 'AMD'
+        return gpu_info
+
+    except OSError:
+        pass
+
     # *** Second try: `lshw`
     try:
         info_cmd = ['lshw', '-C', 'video']
         proc = Popen(info_cmd, stdout=PIPE, stderr=DEVNULL)
         raw_info = str(proc.stdout.read())
 
         def lshw_single_gpu_info(raw_info):
@@ -519,17 +593,35 @@
 
     # Unable to detect platform. Stick to default...
     return CPU64
 
 
 class Platform(object):
 
+    registry = {}
+    """
+    The Platform registry.
+
+    Each new Platform instance is automatically added to the registry.
+    """
+
+    max_mem_trans_nbytes = None
+    """Maximum memory transaction size in bytes."""
+
     def __init__(self, name):
         self.name = name
 
+        self.registry[name] = self
+
+    def __eq__(self, other):
+        return isinstance(other, Platform) and self.name == other.name
+
+    def __hash__(self):
+        return hash(self.name)
+
     @classmethod
     def _mro(cls):
         return [Platform]
 
     def __call__(self):
         return self
 
@@ -543,47 +635,48 @@
         return 'unknown'
 
     @property
     def threads_per_core(self):
         return self.cores_logical // self.cores_physical
 
     @property
-    def simd_reg_size(self):
-        """Size in bytes of a SIMD register."""
-        return isa_registry.get(self.isa, 0)
-
-    def simd_items_per_reg(self, dtype):
-        """Number of items of type ``dtype`` that can fit in a SIMD register."""
-        assert self.simd_reg_size % np.dtype(dtype).itemsize == 0
-        return int(self.simd_reg_size / np.dtype(dtype).itemsize)
-
-    @property
     def memtotal(self):
         """Physical memory size in bytes, or None if unknown."""
         return None
 
     def memavail(self, *args, **kwargs):
         """Available physical memory in bytes, or None if unknown."""
         return None
 
+    def max_mem_trans_size(self, dtype):
+        """
+        Number of items of type `dtype` that can be transferred in a single
+        memory transaction.
+        """
+        assert self.max_mem_trans_nbytes % np.dtype(dtype).itemsize == 0
+        return int(self.max_mem_trans_nbytes / np.dtype(dtype).itemsize)
+
 
 class Cpu64(Platform):
 
+    # The vast majority of CPUs have a 64-byte cache line size
+    max_mem_trans_nbytes = 64
+
+    # The known ISAs are to be provided by the subclasses
+    known_isas = ()
+
     def __init__(self, name, cores_logical=None, cores_physical=None, isa=None):
         super().__init__(name)
 
         cpu_info = get_cpu_info()
 
         self.cores_logical = cores_logical or cpu_info['logical']
         self.cores_physical = cores_physical or cpu_info['physical']
         self.isa = isa or self._detect_isa()
 
-    # The known ISAs are to be provided by the subclasses
-    known_isas = ()
-
     @classmethod
     def _mro(cls):
         # Retain only the CPU Platforms
         retval = []
         for i in cls.mro():
             if issubclass(i, Cpu64):
                 retval.append(i)
@@ -595,14 +688,28 @@
         for i in reversed(self.known_isas):
             if any(j.startswith(i) for j in as_tuple(get_cpu_info()['flags'])):
                 # Using `startswith`, rather than `==`, as a flag such as 'avx512'
                 # appears as 'avx512f, avx512cd, ...'
                 return i
         return 'cpp'
 
+    @property
+    def simd_reg_nbytes(self):
+        """
+        Size in bytes of a SIMD register.
+        """
+        return isa_registry.get(self.isa, 0)
+
+    def simd_items_per_reg(self, dtype):
+        """
+        Number of items of type `dtype` that fit in a SIMD register.
+        """
+        assert self.simd_reg_nbytes % np.dtype(dtype).itemsize == 0
+        return int(self.simd_reg_nbytes / np.dtype(dtype).itemsize)
+
     @cached_property
     def memtotal(self):
         return psutil.virtual_memory().total
 
     def memavail(self, *args, **kwargs):
         return psutil.virtual_memory().available
 
@@ -621,46 +728,64 @@
 
 
 class Arm(Cpu64):
 
     known_isas = ('fp', 'asimd', 'asimdrdm')
 
 
+class AppleArm(Arm):
+
+    @cached_property
+    def march(self):
+        sysinfo = run(["sysctl", "-n", "machdep.cpu.brand_string"],
+                      stdout=PIPE, stderr=DEVNULL).stdout.decode("utf-8")
+        mx = sysinfo.split(' ')[1].lower()
+        # Currently clang only supports up to m2
+        return min(mx, 'm2')
+
+
 class Amd(Cpu64):
 
     known_isas = ('cpp', 'sse', 'avx', 'avx2')
 
 
 class Power(Cpu64):
 
     def _detect_isa(self):
         return 'altivec'
 
 
 class Device(Platform):
 
-    def __init__(self, name, cores_logical=1, cores_physical=1, isa='cpp'):
+    def __init__(self, name, cores_logical=1, cores_physical=1, isa='cpp',
+                 max_threads_per_block=1024, max_threads_dimx=1024,
+                 max_threads_dimy=1024, max_threads_dimz=64):
         super().__init__(name)
 
         self.cores_logical = cores_logical
         self.cores_physical = cores_physical
         self.isa = isa
 
+        self.max_threads_per_block = max_threads_per_block
+        self.max_threads_dimx = max_threads_dimx
+        self.max_threads_dimy = max_threads_dimy
+        self.max_threads_dimz = max_threads_dimz
+
     @classmethod
     def _mro(cls):
         # Retain only the Device Platforms
         retval = []
         for i in cls.mro():
             if issubclass(i, Device):
                 retval.append(i)
             else:
                 break
         return retval
 
-    @cached_property
+    @property
     def march(self):
         return None
 
     @cached_property
     def memtotal(self):
         info = get_gpu_info()
         try:
@@ -677,33 +802,44 @@
             return info['mem.free'](deviceid)
         except (AttributeError, KeyError):
             return None
 
 
 class IntelDevice(Device):
 
-    @cached_property
+    max_mem_trans_nbytes = 64
+
+    def __init__(self, *args, sub_group_size=32, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.sub_group_size = sub_group_size
+
+    @property
     def march(self):
         return ''
 
 
 class NvidiaDevice(Device):
 
+    max_mem_trans_nbytes = 128
+
     @cached_property
     def march(self):
         info = get_gpu_info()
         if info:
             architecture = info['architecture']
             if 'tesla' in architecture.lower():
                 return 'tesla'
         return None
 
 
 class AmdDevice(Device):
 
+    max_mem_trans_nbytes = 256
+
     @cached_property
     def march(cls):
         # TODO: this corresponds to Vega, which acts as the fallback `march`
         # in case we don't manage to detect the actual `march`. Can we improve this?
         fallback = 'gfx900'
 
         # The AMD's AOMP compiler toolkit ships the `mygpu` program to (quoting
@@ -730,72 +866,51 @@
 
 
 # CPUs
 CPU64 = Cpu64('cpu64')
 CPU64_DUMMY = Intel64('cpu64-dummy', cores_logical=2, cores_physical=1, isa='sse')
 
 INTEL64 = Intel64('intel64')
-SNB = Intel64('snb')
-IVB = Intel64('ivb')
-HSW = Intel64('hsw')
-BDW = Intel64('bdw', isa='avx2')
-KNL = Intel64('knl')
-KNL7210 = Intel64('knl', cores_logical=256, cores_physical=64, isa='avx512')
-SKX = IntelSkylake('skx')
-KLX = IntelSkylake('klx')
-CLX = IntelSkylake('clx')
-CLK = IntelSkylake('clk')
-SPR = IntelGoldenCove('spr')
+SNB = Intel64('snb')  # Sandy Bridge
+IVB = Intel64('ivb')  # Ivy Bridge
+HSW = Intel64('hsw')  # Haswell
+BDW = Intel64('bdw', isa='avx2')  # Broadwell
+KNL = Intel64('knl')  # Knights Landing
+KNL7210 = Intel64('knl7210', cores_logical=256, cores_physical=64, isa='avx512')
+SKX = IntelSkylake('skx')  # Skylake
+KLX = IntelSkylake('klx')  # Kaby Lake
+CLX = IntelSkylake('clx')  # Coffee Lake
+CLK = IntelSkylake('clk')  # Cascade Lake
+SPR = IntelGoldenCove('spr')  # Sapphire Rapids
 
 ARM = Arm('arm')
 GRAVITON = Arm('graviton')
-M1 = Arm('m1')
+M1 = AppleArm('m1')
+M2 = AppleArm('m2')
+M3 = AppleArm('m3')
 
 AMD = Amd('amd')
 
 POWER8 = Power('power8')
 POWER9 = Power('power9')
 
 # Devices
 NVIDIAX = NvidiaDevice('nvidiaX')
+
 AMDGPUX = AmdDevice('amdgpuX')
-INTELGPUX = IntelDevice('intelgpuX')
 
+INTELGPUX = IntelDevice('intelgpuX')
+PVC = IntelDevice('pvc')  # Legacy codename for MAX GPUs
+INTELGPUMAX = IntelDevice('intelgpuMAX')
+MAX1100 = IntelDevice('max1100')
+MAX1550 = IntelDevice('max1550')
 
-platform_registry = {
-    'cpu64-dummy': CPU64_DUMMY,
-    'intel64': INTEL64,
-    'snb': SNB,  # Sandy Bridge
-    'ivb': IVB,  # Ivy Bridge
-    'hsw': HSW,  # Haswell
-    'bdw': BDW,  # Broadwell
-    'skx': SKX,  # Skylake
-    'klx': KLX,  # Kaby Lake
-    'clx': CLX,  # Coffee Lake
-    'clk': CLK,  # Cascade Lake
-    'spr': SPR,  # Sapphire Rapids
-    'knl': KNL,
-    'knl7210': KNL7210,
-    'arm': ARM,  # Generic ARM CPU
-    'graviton': GRAVITON,  # AMS arm
-    'm1': M1,
-    'amd': AMD,  # Generic AMD CPU
-    'power8': POWER8,
-    'power9': POWER9,
-    'nvidiaX': NVIDIAX,  # Generic NVidia GPU
-    'amdgpuX': AMDGPUX,   # Generic AMD GPU
-    'intelgpuX': INTELGPUX   # Generic Intel GPU
-}
-"""
-Registry dict for deriving Platform classes according to the environment variable
-DEVITO_PLATFORM. Developers should add new platform classes here.
-"""
+platform_registry = Platform.registry
 platform_registry['cpu64'] = get_platform  # Autodetection
 
-
 isa_registry = {
     'cpp': 16,
     'sse': 16,
     'avx': 32,
     'avx2': 32,
     'avx512': 64,
     'altivec': 16,
```

### Comparing `devito-4.8.3/devito/arch/compiler.py` & `devito-4.8.4/devito/arch/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from functools import partial
 from hashlib import sha1
 from os import environ, path, makedirs
 from packaging.version import Version
-from subprocess import DEVNULL, PIPE, CalledProcessError, check_output, check_call, run
+from subprocess import (DEVNULL, PIPE, CalledProcessError, check_output,
+                        check_call, run)
 import platform
 import warnings
 import sys
 import time
 
 import numpy.ctypeslib as npct
 from codepy.jit import compile_from_string
-from codepy.toolchain import GCCToolchain, call_capture_output as _call_capture_output
+from codepy.toolchain import (GCCToolchain,
+                              call_capture_output as _call_capture_output)
 
-from devito.arch import (AMDGPUX, Cpu64, M1, NVIDIAX, POWER8, POWER9, GRAVITON,
-                         INTELGPUX, get_nvidia_cc, check_cuda_runtime,
+from devito.arch import (AMDGPUX, Cpu64, AppleArm, NVIDIAX, POWER8, POWER9, GRAVITON,
+                         IntelDevice, get_nvidia_cc, check_cuda_runtime,
                          get_m1_llvm_path)
 from devito.exceptions import CompilationError
 from devito.logger import debug, warning, error
 from devito.parameters import configuration
 from devito.tools import (as_list, change_directory, filter_ordered,
                           memoized_func, make_tempdir)
 
 __all__ = ['sniff_mpi_distro', 'compiler_registry']
 
 
 @memoized_func
-def sniff_compiler_version(cc):
+def sniff_compiler_version(cc, allow_fail=False):
     """
     Detect the compiler version.
 
     Adapted from: ::
 
         https://github.com/OP2/PyOP2/
     """
@@ -37,16 +39,19 @@
         res = run([cc, "--version"], stdout=PIPE, stderr=DEVNULL)
         ver = res.stdout.decode("utf-8")
         if not ver:
             return Version("0")
     except UnicodeDecodeError:
         return Version("0")
     except FileNotFoundError:
-        error("The `%s` compiler isn't available on this system" % cc)
-        sys.exit(1)
+        if allow_fail:
+            return Version("0")
+        else:
+            error("The `%s` compiler isn't available on this system" % cc)
+            sys.exit(1)
 
     if ver.startswith("gcc"):
         compiler = "gcc"
     elif ver.startswith("clang"):
         compiler = "clang"
     elif ver.startswith("Apple LLVM"):
         compiler = "clang"
@@ -159,80 +164,91 @@
         * :data:`self.undefines`
 
     Parameters
     ----------
     suffix : str, optional
         The JIT compiler version to be used. For example, assuming ``CC=gcc`` and
         ``suffix='4.9'``, the ``gcc-4.9`` will be used as JIT compiler.
-    cpp : bool, optional
-        If True, JIT compile using a C++ compiler. Defaults to False.
-    mpi : bool, optional
-        If True, JIT compile using an MPI compiler. Defaults to False.
+    cpp : bool, optional, default=False
+        If True, JIT compile using a C++ compiler.
+    mpi : bool, optional, default=False
+        If True, JIT compile using an MPI compiler.
     platform : Platform, optional
         The target Platform on which the JIT compiler will be used.
     """
 
     fields = {'cc', 'ld'}
+    _cpp = False
 
     def __init__(self, **kwargs):
-        super(Compiler, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         self.__lookup_cmds__()
 
         self.suffix = kwargs.get('suffix')
         if not kwargs.get('mpi'):
-            self.cc = self.CC if kwargs.get('cpp', False) is False else self.CXX
+            self.cc = self.CC if self._cpp is False else self.CXX
             self.cc = self.cc if self.suffix is None else ('%s-%s' %
                                                            (self.cc, self.suffix))
         else:
-            self.cc = self.MPICC if kwargs.get('cpp', False) is False else self.MPICXX
+            self.cc = self.MPICC if self._cpp is False else self.MPICXX
         self.ld = self.cc  # Wanted by the superclass
 
         self.cflags = ['-O3', '-g', '-fPIC', '-Wall', '-std=c99']
         self.ldflags = ['-shared']
 
         self.include_dirs = []
         self.libraries = ['m']
         self.library_dirs = []
         self.defines = []
         self.undefines = []
 
-        self.src_ext = 'c' if kwargs.get('cpp', False) is False else 'cpp'
+        self.src_ext = 'c' if self._cpp is False else 'cpp'
 
         if platform.system() == "Linux":
             self.so_ext = '.so'
         elif platform.system() == "Darwin":
             self.so_ext = '.dylib'
         elif platform.system() == "Windows":
             self.so_ext = '.dll'
         else:
             raise NotImplementedError("Unsupported platform %s" % platform)
 
-        if self.suffix is not None:
-            try:
-                self.version = Version(str(float(self.suffix)))
-            except (TypeError, ValueError):
-                self.version = Version(self.suffix)
-        else:
-            # Knowing the version may still be useful to pick supported flags
-            self.version = sniff_compiler_version(self.CC)
+        self.__init_finalize__(**kwargs)
+
+    def __init_finalize__(self, **kwargs):
+        pass
 
     def __new_with__(self, **kwargs):
         """
         Create a new Compiler from an existing one, inherenting from it
         the flags that are not specified via ``kwargs``.
         """
         return self.__class__(suffix=kwargs.pop('suffix', self.suffix),
                               mpi=kwargs.pop('mpi', configuration['mpi']),
                               **kwargs)
 
     @property
     def name(self):
         return self.__class__.__name__
 
+    @property
+    def version(self):
+        if self.suffix is not None:
+            try:
+                version = Version(str(float(self.suffix)))
+            except (TypeError, ValueError):
+                version = Version(self.suffix)
+        else:
+            # Knowing the version may still be useful to pick supported flags
+            allow_fail = isinstance(self, CustomCompiler)
+            version = sniff_compiler_version(self.CC, allow_fail=allow_fail)
+
+        return version
+
     def get_version(self):
         result, stdout, stderr = call_capture_output((self.cc, "--version"))
         if result != 0:
             raise RuntimeError(f"version query failed: {stderr}")
         return stdout
 
     def get_jit_dir(self):
@@ -390,17 +406,15 @@
 
     def add_ldflags(self, flags):
         self.ldflags = filter_ordered(self.ldflags + as_list(flags))
 
 
 class GNUCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
+    def __init_finalize__(self, **kwargs):
         platform = kwargs.pop('platform', configuration['platform'])
 
         self.cflags += ['-Wno-unused-result',
                         '-Wno-unused-variable', '-Wno-unused-but-set-variable']
 
         if configuration['safe-math']:
             self.cflags.append('-fno-unsafe-math-optimizations')
@@ -439,32 +453,31 @@
         self.CXX = 'g++'
         self.MPICC = 'mpicc'
         self.MPICXX = 'mpicxx'
 
 
 class ArmCompiler(GNUCompiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
+    def __init_finalize__(self, **kwargs):
+        GNUCompiler.__init_finalize__(self, **kwargs)
         platform = kwargs.pop('platform', configuration['platform'])
 
         # Graviton flag
         if platform is GRAVITON:
             self.cflags += ['-mcpu=neoverse-n1']
 
 
 class ClangCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init_finalize__(self, **kwargs):
 
         self.cflags += ['-Wno-unused-result', '-Wno-unused-variable']
         if not configuration['safe-math']:
             self.cflags.append('-ffast-math')
+        self.cflags.append('-fdenormal-fp-math=ieee')
 
         language = kwargs.pop('language', configuration['language'])
         platform = kwargs.pop('platform', configuration['platform'])
 
         if platform is NVIDIAX:
             self.cflags.remove('-std=c99')
             # Add flags for OpenMP offloading
@@ -478,22 +491,24 @@
             # Add flags for OpenMP offloading
             if language in ['C', 'openmp']:
                 self.ldflags += ['-target', 'x86_64-pc-linux-gnu']
                 self.ldflags += ['-fopenmp',
                                  '-fopenmp-targets=amdgcn-amd-amdhsa',
                                  '-Xopenmp-target=amdgcn-amd-amdhsa']
                 self.ldflags += ['-march=%s' % platform.march]
-        elif platform is M1:
+        elif isinstance(platform, AppleArm):
             # NOTE:
-            # Apple M1 supports OpenMP through Apple's LLVM compiler.
+            # Apple Mx supports OpenMP through Apple's LLVM compiler.
             # The compiler can be installed with Homebrew or can be built from scratch.
             # Check if installed and set compiler flags accordingly
             llvmm1 = get_m1_llvm_path(language)
             if llvmm1 and language == 'openmp':
-                self.ldflags += ['-mcpu=apple-m1', '-fopenmp', '-L%s' % llvmm1['libs']]
+                mx = platform.march
+                self.ldflags += ['-mcpu=apple-%s' % mx,
+                                 '-fopenmp', '-L%s' % llvmm1['libs']]
                 self.cflags += ['-Xclang', '-I%s' % llvmm1['include']]
         else:
             if platform in [POWER8, POWER9]:
                 # -march isn't supported on power architectures
                 self.cflags += ['-mcpu=native']
             else:
                 self.cflags += ['-march=native']
@@ -518,16 +533,15 @@
         self.MPICXX = 'CC'
 
 
 class AOMPCompiler(Compiler):
 
     """AMD's fork of Clang for OpenMP offloading on both AMD and NVidia cards."""
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init_finalize__(self, **kwargs):
 
         language = kwargs.pop('language', configuration['language'])
         platform = kwargs.pop('platform', configuration['platform'])
 
         self.cflags += ['-Wno-unused-result', '-Wno-unused-variable']
         if not configuration['safe-math']:
             self.cflags.append('-ffast-math')
@@ -552,32 +566,32 @@
         self.CXX = 'amdclang++'
         self.MPICC = 'mpicc'
         self.MPICXX = 'mpicxx'
 
 
 class DPCPPCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init_finalize__(self, **kwargs):
 
         self.cflags += ['-qopenmp', '-fopenmp-targets=spir64']
 
     def __lookup_cmds__(self):
         # OneAPI Base Kit comes with dpcpp/icpx, both are clang++,
         # and icx, which is clang
         self.CC = 'icx'
         self.CXX = 'icpx'
         self.MPICC = 'mpic++'
         self.MPICXX = 'mpicxx'
 
 
 class PGICompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, cpp=True, **kwargs)
+    _cpp = True
+
+    def __init_finalize__(self, **kwargs):
 
         self.cflags.remove('-std=c99')
         self.cflags.remove('-O3')
         self.cflags.remove('-Wall')
 
         self.cflags.append('-std=c++11')
 
@@ -614,16 +628,17 @@
         self.CXX = 'nvc++'
         self.MPICC = 'mpic++'
         self.MPICXX = 'mpicxx'
 
 
 class CudaCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, cpp=True, **kwargs)
+    _cpp = True
+
+    def __init_finalize__(self, **kwargs):
 
         self.cflags.remove('-std=c99')
         self.cflags.remove('-Wall')
         self.cflags.remove('-fPIC')
         self.cflags.extend(['-std=c++14', '-Xcompiler', '-fPIC'])
 
         if configuration['mpi']:
@@ -649,15 +664,19 @@
                     proc_link_flags.extend([
                         '-Xcompiler', '"%s"' % i.replace(',', r'\,')
                     ])
                 else:
                     proc_link_flags.append(i)
             self.ldflags.extend(proc_link_flags)
 
-        self.cflags.append('-arch=native')
+        cc = get_nvidia_cc()
+        if cc:
+            self.cflags.append(f'-arch=sm_{cc}')
+        else:
+            self.cflags.append('-arch=native')
 
         # Disable `warning #1650-D: result of call is not used`
         # See `https://gist.github.com/gavinb/f2320f9eaa0e0a7efca6877a34047a9d` about
         # disabling specific warnings with nvcc
         self.cflags.extend(['-Xcudafe', '--display_error_number',
                             '--diag-suppress', '1650'])
         # Same as above but for the host compiler
@@ -679,16 +698,17 @@
         self.CXX = 'nvcc'
         self.MPICC = 'nvcc'
         self.MPICXX = 'nvcc'
 
 
 class HipCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, cpp=True, **kwargs)
+    _cpp = True
+
+    def __init_finalize__(self, **kwargs):
 
         self.cflags.remove('-std=c99')
         self.cflags.remove('-Wall')
         self.cflags.remove('-fPIC')
         self.cflags.extend(['-std=c++14', '-fPIC'])
 
         if configuration['mpi']:
@@ -708,17 +728,15 @@
         self.CXX = 'hipcc'
         self.MPICC = 'hipcc'
         self.MPICXX = 'hipcc'
 
 
 class IntelCompiler(Compiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
+    def __init_finalize__(self, **kwargs):
         platform = kwargs.pop('platform', configuration['platform'])
         language = kwargs.pop('language', configuration['language'])
 
         self.cflags.append("-xHost")
 
         if configuration['safe-math']:
             self.cflags.append("-fp-model=strict")
@@ -728,21 +746,28 @@
         if platform.isa == 'avx512':
             # Systematically use 512-bit vectors if avx512 is available.
             self.cflags.append("-qopt-zmm-usage=high")
 
         if language == 'openmp':
             self.ldflags.append('-qopenmp')
 
-        # Make sure the MPI compiler uses `icc` underneath -- whatever the MPI distro is
         if kwargs.get('mpi'):
-            mpi_distro = sniff_mpi_distro('mpiexec')
-            if mpi_distro != 'IntelMPI':
-                warning("Expected Intel MPI distribution with `%s`, but found `%s`"
-                        % (self.__class__.__name__, mpi_distro))
-            self.cflags.insert(0, '-cc=%s' % self.CC)
+            self.__init_intel_mpi__()
+            self.__init_intel_mpi_flags__()
+
+    def __init_intel_mpi__(self, **kwargs):
+        # Make sure the MPI compiler uses an Intel compiler underneath,
+        # whatever the MPI distro is
+        mpi_distro = sniff_mpi_distro('mpiexec')
+        if mpi_distro != 'IntelMPI':
+            warning("Expected Intel MPI distribution with `%s`, but found `%s`"
+                    % (self.__class__.__name__, mpi_distro))
+
+    def __init_intel_mpi_flags__(self, **kwargs):
+        self.cflags.insert(0, '-cc=%s' % self.CC)
 
     def get_version(self):
         if configuration['mpi']:
             cmd = (self.cc, "-cc=%s" % self.CC, "--version")
         else:
             cmd = (self.cc, "--version")
         result, stdout, stderr = call_capture_output(cmd)
@@ -767,63 +792,107 @@
         except FileNotFoundError:
             self.MPICC = 'mpicc'
             self.MPICXX = 'mpicxx'
 
 
 class IntelKNLCompiler(IntelCompiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init_finalize__(self, **kwargs):
+        IntelCompiler.__init_finalize__(self, **kwargs)
 
         language = kwargs.pop('language', configuration['language'])
 
         self.cflags.append('-xMIC-AVX512')
 
         if language != 'openmp':
             warning("Running on Intel KNL without OpenMP is highly discouraged")
 
 
 class OneapiCompiler(IntelCompiler):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init_finalize__(self, **kwargs):
+        IntelCompiler.__init_finalize__(self, **kwargs)
 
         platform = kwargs.pop('platform', configuration['platform'])
         language = kwargs.pop('language', configuration['language'])
 
-        # Earlier versions to OneAPI 2023.2.0 (clang17 underneath), have an OpenMP bug
-        if self.version < Version('17.0.0') and language == 'openmp':
-            self.ldflags.remove('-qopenmp')
-            self.ldflags.append('-fopenmp')
-
         if language == 'sycl':
-            self.cflags.append('-fsycl')
-            if platform is NVIDIAX:
-                self.cflags.append('-fsycl-targets=nvptx64-cuda')
-            else:
-                self.cflags.append('-fsycl-targets=spir64')
+            raise ValueError("Use SyclCompiler to jit-compile sycl")
+
+        elif language == 'openmp':
+            # Earlier versions to OneAPI 2023.2.0 (clang17 underneath), have an
+            # OpenMP bug concerning reductions, hence with them we're forced to
+            # use the obsolete -fopenmp
+            if self.version < Version('17.0.0'):
+                self.ldflags.remove('-qopenmp')
+                self.ldflags.append('-fopenmp')
 
             if platform is NVIDIAX:
                 self.cflags.append('-fopenmp-targets=nvptx64-cuda')
-            if platform is INTELGPUX:
+            elif isinstance(platform, IntelDevice):
+                self.cflags.append('-fiopenmp')
                 self.cflags.append('-fopenmp-targets=spir64')
                 self.cflags.append('-fopenmp-target-simd')
 
-        if platform is INTELGPUX:
-            self.cflags.remove('-g')  # -g disables some optimizations in IGC
-            self.cflags.append('-gline-tables-only')
-            self.cflags.append('-fdebug-info-for-profiling')
+                self.cflags.remove('-g')  # -g disables some optimizations in IGC
+                self.cflags.append('-gline-tables-only')
+                self.cflags.append('-fdebug-info-for-profiling')
+
+    def __init_intel_mpi__(self, **kwargs):
+        IntelCompiler.__init_intel_mpi__(self, **kwargs)
+
+        platform = kwargs.pop('platform', configuration['platform'])
+
+        # The Intel toolchain requires the I_MPI_OFFLOAD env var to be set
+        # to enable GPU-aware MPI (that is, passing device pointers to MPI calls)
+        if isinstance(platform, IntelDevice):
+            environ['I_MPI_OFFLOAD'] = '1'
+
+    def __init_intel_mpi_flags__(self, **kwargs):
+        pass
+
+    get_version = Compiler.get_version
 
     def __lookup_cmds__(self):
         # OneAPI HPC ToolKit comes with icpx, which is clang++,
         # and icx, which is clang
         self.CC = 'icx'
         self.CXX = 'icpx'
-        self.MPICC = 'mpicc'
-        self.MPICXX = 'mpicxx'
+        self.MPICC = 'mpiicx'
+        self.MPICXX = 'mpiicpx'
+
+
+class SyclCompiler(OneapiCompiler):
+
+    _cpp = True
+
+    def __init_finalize__(self, **kwargs):
+        IntelCompiler.__init_finalize__(self, **kwargs)
+
+        platform = kwargs.pop('platform', configuration['platform'])
+        language = kwargs.pop('language', configuration['language'])
+
+        if language != 'sycl':
+            raise ValueError("Expected language sycl with SyclCompiler")
+
+        self.cflags.remove('-std=c99')
+        self.cflags.append('-fsycl')
+
+        self.cflags.remove('-g')  # -g disables some optimizations in IGC
+        self.cflags.append('-gline-tables-only')
+        self.cflags.append('-fdebug-info-for-profiling')
+
+        if isinstance(platform, Cpu64):
+            pass
+        elif platform is NVIDIAX:
+            self.cflags.append('-fsycl-targets=nvptx64-cuda')
+        elif isinstance(platform, IntelDevice):
+            self.cflags.append('-fsycl-targets=spir64')
+        else:
+            raise NotImplementedError("Unsupported platform %s" % platform)
 
 
 class CustomCompiler(Compiler):
 
     """
     Custom compiler based on standard environment flags.
 
@@ -835,41 +904,66 @@
     default GNU/gcc settings. If DEVITO_ARCH is enabled and the DEVITO_LANGUAGE
     is set to 'openmp', then the OpenMP linker flags are read from OMP_LDFLAGS
     or otherwise default to ``-fopenmp``.
     """
 
     def __new__(cls, *args, **kwargs):
         platform = kwargs.pop('platform', configuration['platform'])
+        language = kwargs.pop('language', configuration['language'])
 
-        if any(i in environ for i in ['CC', 'CXX', 'CFLAGS', 'LDFLAGS']):
-            obj = super().__new__(cls)
-            obj.__init__(*args, **kwargs)
-            return obj
-        elif platform is M1:
-            return ClangCompiler(*args, **kwargs)
-        else:
-            return GNUCompiler(*args, **kwargs)
-
-    def __init__(self, *args, **kwargs):
-        super(CustomCompiler, self).__init__(*args, **kwargs)
-
-        default = '-O3 -g -march=native -fPIC -Wall -std=c99'
-        self.cflags = environ.get('CFLAGS', default).split(' ')
-        self.ldflags = environ.get('LDFLAGS', '-shared').split(' ')
+        if isinstance(platform, AppleArm):
+            _base = ClangCompiler
+        elif isinstance(platform, IntelDevice):
+            _base = OneapiCompiler
+        elif platform is NVIDIAX:
+            if language == 'cuda':
+                _base = CudaCompiler
+            else:
+                _base = NvidiaCompiler
+        elif platform is AMDGPUX:
+            if language == 'hip':
+                _base = HipCompiler
+            else:
+                _base = AOMPCompiler
+        else:
+            _base = GNUCompiler
 
-        language = kwargs.pop('language', configuration['language'])
+        obj = super().__new__(cls)
+        # Keep base to initialize accordingly
+        obj._base = kwargs.pop('base', _base)
+        obj._cpp = obj._base._cpp
 
-        if language == 'openmp':
-            self.ldflags += environ.get('OMP_LDFLAGS', '-fopenmp').split(' ')
+        return obj
+
+    def __init_finalize__(self, **kwargs):
+        self._base.__init_finalize__(self, **kwargs)
+        # Update cflags
+        try:
+            extrac = environ.get('CFLAGS').split(' ')
+            self.cflags = self.cflags + extrac
+        except AttributeError:
+            pass
+        # Update ldflags
+        try:
+            extrald = environ.get('LDFLAGS').split(' ')
+            self.ldflags = self.ldflags + extrald
+        except AttributeError:
+            pass
 
     def __lookup_cmds__(self):
-        self.CC = environ.get('CC', 'gcc')
-        self.CXX = environ.get('CXX', 'g++')
-        self.MPICC = environ.get('MPICC', 'mpicc')
-        self.MPICXX = environ.get('MPICXX', 'mpicxx')
+        self._base.__lookup_cmds__(self)
+        # TODO: check for conflicts, for example using the nvhpc module file
+        # will set CXX to nvc++ breaking  the cuda backend
+        self.CC = environ.get('CC', self.CC)
+        self.CXX = environ.get('CXX', self.CXX)
+        self.MPICC = environ.get('MPICC', self.MPICC)
+        self.MPICXX = environ.get('MPICXX', self.MPICXX)
+
+    def __new_with__(self, **kwargs):
+        return super().__new_with__(base=self._base, **kwargs)
 
 
 compiler_registry = {
     'custom': CustomCompiler,
     'gnu': GNUCompiler,
     'gcc': GNUCompiler,
     'arm': ArmCompiler,
@@ -884,19 +978,21 @@
     'nvc++': NvidiaCompiler,
     'nvidia': NvidiaCompiler,
     'cuda': CudaCompiler,
     'osx': ClangCompiler,
     'intel': OneapiCompiler,
     'icx': OneapiCompiler,
     'icpx': OneapiCompiler,
+    'sycl': SyclCompiler,
     'icc': IntelCompiler,
     'icpc': IntelCompiler,
     'intel-knl': IntelKNLCompiler,
     'knl': IntelKNLCompiler,
     'dpcpp': DPCPPCompiler,
 }
 """
 Registry dict for deriving Compiler classes according to the environment variable
 DEVITO_ARCH. Developers should add new compiler classes here.
 """
 compiler_registry.update({'gcc-%s' % i: partial(GNUCompiler, suffix=i)
-                          for i in ['4.9', '5', '6', '7', '8', '9', '10', '11', '12']})
+                          for i in ['4.9', '5', '6', '7', '8', '9', '10',
+                                    '11', '12', '13']})
```

### Comparing `devito-4.8.3/devito/builtins/arithmetic.py` & `devito-4.8.4/devito/builtins/arithmetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     """
     Compute the norm of a Function.
 
     Parameters
     ----------
     f : Function
         Input Function.
-    order : int, optional
-        The order of the norm. Defaults to 2.
+    order : int, default=2
+        The order of the norm.
     """
     Pow = dv.finite_differences.differentiable.Pow
     kwargs = {}
     if f.is_TimeFunction and f._time_buffering:
         kwargs[f.time_dim.max_name] = f._time_size - 1
 
     # Protect SparseFunctions from accessing duplicated (out-of-domain) data,
```

### Comparing `devito-4.8.3/devito/builtins/initializers.py` & `devito-4.8.4/devito/builtins/initializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         accepted. Default mode is 'reflect'.
     """
     class ObjectiveDomain(dv.SubDomain):
 
         name = 'objective_domain'
 
         def __init__(self, lw):
-            super(ObjectiveDomain, self).__init__()
+            super().__init__()
             self.lw = lw
 
         def define(self, dimensions):
             return {d: ('middle', l, l) for d, l in zip(dimensions, self.lw)}
 
     def create_gaussian_weights(sigma, lw):
         weights = [w/w.sum() for w in (np.exp(-0.5/s**2*(np.linspace(-l, l, 2*l+1))**2)
```

### Comparing `devito-4.8.3/devito/builtins/utils.py` & `devito-4.8.4/devito/builtins/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
         else:
             raise ValueError("Multiple Grids found")
         if dtype is not None:
             self.dtype = dtype
         else:
             dtype = {f.dtype for f in functions}
             if len(dtype) == 1:
-                self.dtype = dtype.pop()
+                self.dtype = np.result_type(dtype.pop(), np.float32).type
             else:
                 raise ValueError("Illegal mixed data types")
         self.v = None
         self.op = op
 
     def __enter__(self):
         i = dv.Dimension(name='mri',)
         self.n = dv.Function(name='n', shape=(1,), dimensions=(i,),
-                             grid=self.grid, dtype=self.dtype)
-        self.n.data[0] = 0
+                             grid=self.grid, dtype=self.dtype, space='host')
+        self.n.data[:] = 0
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if self.grid is None or not dv.configuration['mpi']:
             assert self.n.data.size == 1
             self.v = self.n.data[0]
         else:
```

### Comparing `devito-4.8.3/devito/checkpointing/checkpoint.py` & `devito-4.8.4/devito/checkpointing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/core/__init__.py` & `devito-4.8.4/devito/core/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/core/autotuning.py` & `devito-4.8.4/devito/core/autotuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     if mode == 'preemptive':
         writes = {i.name: i for i in operator.writes}
         copies = {k: writes[k]._C_as_ndarray(v).copy()
                   for k, v in args.items() if k in writes}
         # WARNING: `copies` keeps references to numpy arrays, which is required
         # to avoid garbage collection to kick in during autotuning and prematurely
         # free the shadow copies handed over to C-land
-        at_args.update({k: writes[k]._C_make_dataobj(v) for k, v in copies.items()})
+        at_args.update({k: writes[k]._C_make_dataobj(alias=writes[k], **copies)
+                        for k in copies})
 
     # Disable halo exchanges through MPI_PROC_NULL
     if mode in ['preemptive', 'destructive']:
         for p in operator.parameters:
             if isinstance(p, MPINeighborhood):
                 at_args.update(
                     MPINeighborhood(p.neighborhood)._arg_values()
```

### Comparing `devito-4.8.3/devito/core/cpu.py` & `devito-4.8.4/devito/core/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from devito.core.operator import CoreOperator, CustomOperator, ParTile
 from devito.exceptions import InvalidOperator
 from devito.passes.equations import collect_derivatives
 from devito.passes.clusters import (Lift, blocking, buffering, cire, cse,
                                     factorize, fission, fuse, optimize_pows,
                                     optimize_hyperplanes)
-from devito.passes.iet import (CTarget, OmpTarget, avoid_denormals, linearize, mpiize,
-                               hoist_prodders, relax_incr_dimensions)
+from devito.passes.iet import (CTarget, OmpTarget, avoid_denormals, linearize,
+                               mpiize, hoist_prodders, relax_incr_dimensions,
+                               check_stability)
 from devito.tools import timed_pass
 
 __all__ = ['Cpu64NoopCOperator', 'Cpu64NoopOmpOperator', 'Cpu64AdvCOperator',
            'Cpu64AdvOmpOperator', 'Cpu64FsgCOperator', 'Cpu64FsgOmpOperator',
            'Cpu64CustomOperator']
 
 
@@ -39,15 +40,17 @@
         # Blocking
         o['blockinner'] = oo.pop('blockinner', False)
         o['blocklevels'] = oo.pop('blocklevels', cls.BLOCK_LEVELS)
         o['blockeager'] = oo.pop('blockeager', cls.BLOCK_EAGER)
         o['blocklazy'] = oo.pop('blocklazy', not o['blockeager'])
         o['blockrelax'] = oo.pop('blockrelax', cls.BLOCK_RELAX)
         o['skewing'] = oo.pop('skewing', False)
-        o['par-tile'] = ParTile(oo.pop('par-tile', False), default=16)
+        o['par-tile'] = ParTile(oo.pop('par-tile', False), default=16,
+                                sparse=oo.pop('par-tile-sparse', None),
+                                reduce=oo.pop('par-tile-reduce', None))
 
         # CIRE
         o['min-storage'] = oo.pop('min-storage', False)
         o['cire-rotate'] = oo.pop('cire-rotate', False)
         o['cire-maxpar'] = oo.pop('cire-maxpar', False)
         o['cire-ftemps'] = oo.pop('cire-ftemps', False)
         o['cire-mingain'] = oo.pop('cire-mingain', cls.CIRE_MINGAIN)
@@ -59,21 +62,26 @@
         o['par-chunk-nonaffine'] = oo.pop('par-chunk-nonaffine', cls.PAR_CHUNK_NONAFFINE)
         o['par-dynamic-work'] = oo.pop('par-dynamic-work', cls.PAR_DYNAMIC_WORK)
         o['par-nested'] = oo.pop('par-nested', cls.PAR_NESTED)
 
         # Distributed parallelism
         o['dist-drop-unwritten'] = oo.pop('dist-drop-unwritten', cls.DIST_DROP_UNWRITTEN)
 
-        # Misc
+        # Code generation options for derivatives
         o['expand'] = oo.pop('expand', cls.EXPAND)
-        o['optcomms'] = oo.pop('optcomms', True)
+        o['deriv-schedule'] = oo.pop('deriv-schedule', cls.DERIV_SCHEDULE)
+        o['deriv-unroll'] = oo.pop('deriv-unroll', False)
+
+        # Misc
+        o['opt-comms'] = oo.pop('opt-comms', True)
         o['linearize'] = oo.pop('linearize', False)
         o['mapify-reduce'] = oo.pop('mapify-reduce', cls.MAPIFY_REDUCE)
         o['index-mode'] = oo.pop('index-mode', cls.INDEX_MODE)
         o['place-transfers'] = oo.pop('place-transfers', True)
+        o['errctl'] = oo.pop('errctl', cls.ERRCTL)
 
         # Recognised but unused by the CPU backend
         oo.pop('par-disabled', None)
         oo.pop('gpu-fit', None)
         oo.pop('gpu-create', None)
 
         if oo:
@@ -162,15 +170,15 @@
     def _specialize_iet(cls, graph, **kwargs):
         options = kwargs['options']
         platform = kwargs['platform']
         compiler = kwargs['compiler']
         sregistry = kwargs['sregistry']
 
         # Flush denormal numbers
-        avoid_denormals(graph, platform=platform)
+        avoid_denormals(graph, **kwargs)
 
         # Distributed-memory parallelism
         mpiize(graph, **kwargs)
 
         # Lower BlockDimensions so that blocks of arbitrary shape may be used
         relax_incr_dimensions(graph, **kwargs)
 
@@ -179,14 +187,17 @@
         parizer.make_simd(graph)
         parizer.make_parallel(graph)
         parizer.initialize(graph, options=options)
 
         # Misc optimizations
         hoist_prodders(graph)
 
+        # Perform error checking
+        check_stability(graph, **kwargs)
+
         # Symbol definitions
         cls._Target.DataManager(**kwargs).process(graph)
 
         # Linearize n-dimensional Indexeds
         linearize(graph, **kwargs)
 
         return graph
@@ -256,15 +267,15 @@
         platform = kwargs['platform']
         compiler = kwargs['compiler']
         sregistry = kwargs['sregistry']
 
         parizer = cls._Target.Parizer(sregistry, options, platform, compiler)
 
         return {
-            'denormals': avoid_denormals,
+            'denormals': partial(avoid_denormals, **kwargs),
             'blocking': partial(relax_incr_dimensions, **kwargs),
             'parallel': parizer.make_parallel,
             'openmp': parizer.make_parallel,
             'mpi': partial(mpiize, **kwargs),
             'linearize': partial(linearize, **kwargs),
             'simd': partial(parizer.make_simd),
             'prodders': hoist_prodders,
```

### Comparing `devito-4.8.3/devito/core/gpu.py` & `devito-4.8.4/devito/core/gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from devito.exceptions import InvalidOperator
 from devito.operator.operator import rcompile
 from devito.passes import is_on_device
 from devito.passes.equations import collect_derivatives
 from devito.passes.clusters import (Lift, Streaming, Tasker, blocking, buffering,
                                     cire, cse, factorize, fission, fuse,
                                     optimize_pows)
-from devito.passes.iet import (DeviceOmpTarget, DeviceAccTarget, mpiize, hoist_prodders,
-                               linearize, pthreadify, relax_incr_dimensions)
+from devito.passes.iet import (DeviceOmpTarget, DeviceAccTarget, mpiize,
+                               hoist_prodders, linearize, pthreadify,
+                               relax_incr_dimensions, check_stability)
 from devito.tools import as_tuple, timed_pass
 
 __all__ = ['DeviceNoopOperator', 'DeviceAdvOperator', 'DeviceCustomOperator',
            'DeviceNoopOmpOperator', 'DeviceAdvOmpOperator', 'DeviceFsgOmpOperator',
            'DeviceCustomOmpOperator', 'DeviceNoopAccOperator', 'DeviceAdvAccOperator',
            'DeviceFsgAccOperator', 'DeviceCustomAccOperator']
 
@@ -61,61 +62,76 @@
         o['cire-rotate'] = False
         o['cire-maxpar'] = oo.pop('cire-maxpar', True)
         o['cire-ftemps'] = oo.pop('cire-ftemps', False)
         o['cire-mingain'] = oo.pop('cire-mingain', cls.CIRE_MINGAIN)
         o['cire-schedule'] = oo.pop('cire-schedule', cls.CIRE_SCHEDULE)
 
         # GPU parallelism
-        o['par-tile'] = ParTile(oo.pop('par-tile', False), default=(32, 4))
+        o['par-tile'] = ParTile(oo.pop('par-tile', False), default=(32, 4, 4),
+                                sparse=oo.pop('par-tile-sparse', None),
+                                reduce=oo.pop('par-tile-reduce', None))
         o['par-collapse-ncores'] = 1  # Always collapse (meaningful if `par-tile=False`)
         o['par-collapse-work'] = 1  # Always collapse (meaningful if `par-tile=False`)
         o['par-chunk-nonaffine'] = oo.pop('par-chunk-nonaffine', cls.PAR_CHUNK_NONAFFINE)
         o['par-dynamic-work'] = np.inf  # Always use static scheduling
         o['par-nested'] = np.inf  # Never use nested parallelism
         o['par-disabled'] = oo.pop('par-disabled', True)  # No host parallelism by default
-        o['gpu-fit'] = as_tuple(oo.pop('gpu-fit', cls._normalize_gpu_fit(**kwargs)))
+        o['gpu-fit'] = cls._normalize_gpu_fit(oo, **kwargs)
         o['gpu-create'] = as_tuple(oo.pop('gpu-create', ()))
 
         # Distributed parallelism
         o['dist-drop-unwritten'] = oo.pop('dist-drop-unwritten', cls.DIST_DROP_UNWRITTEN)
 
-        # Misc
+        # Code generation options for derivatives
         o['expand'] = oo.pop('expand', cls.EXPAND)
-        o['optcomms'] = oo.pop('optcomms', True)
+        o['deriv-schedule'] = oo.pop('deriv-schedule', cls.DERIV_SCHEDULE)
+        o['deriv-unroll'] = oo.pop('deriv-unroll', False)
+
+        # Misc
+        o['opt-comms'] = oo.pop('opt-comms', True)
         o['linearize'] = oo.pop('linearize', False)
         o['mapify-reduce'] = oo.pop('mapify-reduce', cls.MAPIFY_REDUCE)
         o['index-mode'] = oo.pop('index-mode', cls.INDEX_MODE)
         o['place-transfers'] = oo.pop('place-transfers', True)
+        o['errctl'] = oo.pop('errctl', cls.ERRCTL)
 
         if oo:
             raise InvalidOperator("Unsupported optimization options: [%s]"
                                   % ", ".join(list(oo)))
 
         kwargs['options'].update(o)
 
         return kwargs
 
     @classmethod
-    def _normalize_gpu_fit(cls, **kwargs):
-        if any(i in kwargs['mode'] for i in ['tasking', 'streaming']):
-            return None
-        else:
-            return cls.GPU_FIT
+    def _normalize_gpu_fit(cls, oo, **kwargs):
+        try:
+            gfit = as_tuple(oo.pop('gpu-fit'))
+            gfit = set().union(*[f.values() if f.is_AbstractTensor else [f]
+                                 for f in gfit])
+            return tuple(gfit)
+        except KeyError:
+            if any(i in kwargs['mode'] for i in ['tasking', 'streaming']):
+                return (None,)
+            else:
+                return as_tuple(cls.GPU_FIT)
 
     @classmethod
-    def _rcompile_wrapper(cls, **kwargs):
-        options = kwargs['options']
+    def _rcompile_wrapper(cls, **kwargs0):
+        options = kwargs0['options']
 
-        def wrapper(expressions, kwargs=kwargs, mode='default'):
+        def wrapper(expressions, mode='default', **kwargs1):
             if mode == 'host':
-                kwargs = {
+                kwargs = {**{
                     'platform': 'cpu64',
                     'language': 'C' if options['par-disabled'] else 'openmp',
                     'compiler': 'custom',
-                }
+                }, **kwargs1}
+            else:
+                kwargs = {**kwargs0, **kwargs1}
             return rcompile(expressions, kwargs)
 
         return wrapper
 
 # Mode level
 
 
@@ -208,14 +224,17 @@
         parizer = cls._Target.Parizer(sregistry, options, platform, compiler)
         parizer.make_parallel(graph)
         parizer.initialize(graph, options=options)
 
         # Misc optimizations
         hoist_prodders(graph)
 
+        # Perform error checking
+        check_stability(graph, **kwargs)
+
         # Symbol definitions
         cls._Target.DataManager(**kwargs).process(graph)
 
         # Linearize n-dimensional Indexeds
         linearize(graph, **kwargs)
 
         return graph
```

### Comparing `devito-4.8.3/devito/core/operator.py` & `devito-4.8.4/devito/core/operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections.abc import Iterable
 
 from devito.core.autotuning import autotune
-from devito.exceptions import InvalidOperator
+from devito.exceptions import InvalidArgument, InvalidOperator
 from devito.logger import warning
 from devito.mpi.routines import mpi_registry
 from devito.parameters import configuration
 from devito.operator import Operator
-from devito.tools import as_tuple, is_integer, timed_pass
+from devito.tools import (as_tuple, is_integer, timed_pass,
+                          UnboundTuple, UnboundedMultiTuple)
 from devito.types import NThreads
 
 __all__ = ['CoreOperator', 'CustomOperator',
            # Optimization options
            'ParTile']
 
 
@@ -91,14 +92,20 @@
 
     EXPAND = True
     """
     Unroll all loops with short, numeric trip count, such as loops created by
     finite-difference derivatives.
     """
 
+    DERIV_SCHEDULE = 'basic'
+    """
+    The schedule to use for the computation of finite-difference derivatives.
+    Only meaningful when `EXPAND=False`.
+    """
+
     MPI_MODES = tuple(mpi_registry)
     """
     The supported MPI modes.
     """
 
     DIST_DROP_UNWRITTEN = True
     """
@@ -108,14 +115,21 @@
 
     INDEX_MODE = "int64"
     """
     The type of the expression used to compute array indices. Either `int64`
     (default) or `int32`.
     """
 
+    ERRCTL = None
+    """
+    Runtime error checking. If this option is enabled, the generated code will
+    include runtime checks for various things that might go south, such as
+    instability (e.g., NaNs), failed library calls (e.g., kernel launches).
+    """
+
     _Target = None
     """
     The target language constructor, to be specified by subclasses.
     """
 
     @classmethod
     def _normalize_kwargs(cls, **kwargs):
@@ -139,14 +153,22 @@
     @classmethod
     def _check_kwargs(cls, **kwargs):
         oo = kwargs['options']
 
         if oo['mpi'] and oo['mpi'] not in cls.MPI_MODES:
             raise InvalidOperator("Unsupported MPI mode `%s`" % oo['mpi'])
 
+        if oo['deriv-schedule'] not in ('basic', 'smart'):
+            raise InvalidArgument("Illegal `deriv-schedule` value")
+        if oo['deriv-unroll'] not in (False, 'inner', 'full'):
+            raise InvalidArgument("Illegal `deriv-unroll` value")
+
+        if oo['errctl'] not in (None, False, 'basic', 'max'):
+            raise InvalidArgument("Illegal `errctl` value")
+
     def _autotune(self, args, setup):
         if setup in [False, 'off']:
             return args
         elif setup is True:
             level, mode = configuration['autotuning']
             level = level or 'basic'
             args, summary = autotune(self, args, level, mode)
@@ -323,41 +345,43 @@
 # Wrappers for optimization options
 
 
 class OptOption(object):
     pass
 
 
-class ParTileArg(tuple):
+class ParTileArg(UnboundTuple):
 
-    def __new__(cls, items, shm=0, tag=None):
-        obj = super().__new__(cls, items)
-        obj.shm = shm
+    def __new__(cls, items, rule=None, tag=None):
+        if items is None:
+            items = tuple()
+        obj = super().__new__(cls, *items)
+        obj.rule = rule
         obj.tag = tag
         return obj
 
 
-class ParTile(tuple, OptOption):
+class ParTile(UnboundedMultiTuple, OptOption):
 
-    def __new__(cls, items, default=None):
+    def __new__(cls, items, default=None, sparse=None, reduce=None):
         if not items:
-            return None
+            return UnboundedMultiTuple()
         elif isinstance(items, bool):
             if not default:
                 raise ValueError("Expected `default` value, got None")
             items = (ParTileArg(as_tuple(default)),)
         elif isinstance(items, (list, tuple)):
             if not items:
                 raise ValueError("Expected at least one value")
 
             # Normalize to tuple of ParTileArgs
 
             x = items[0]
             if is_integer(x):
-                # E.g., (32, 4, 8)
+                # E.g., 32
                 items = (ParTileArg(items),)
 
             elif x is None:
                 # E.g. (None, None); to define the dimensionality of a block,
                 # while the actual shape values remain parametric
                 items = (ParTileArg(items),)
 
@@ -367,31 +391,34 @@
 
             elif isinstance(x, Iterable):
                 if not x:
                     raise ValueError("Expected at least one value")
 
                 try:
                     y = items[1]
-                    if is_integer(y):
-                        # E.g., ((32, 4, 8), 1)
-                        # E.g., ((32, 4, 8), 1, 'tag')
+                    if is_integer(y) or isinstance(y, str) or y is None:
+                        # E.g., ((32, 4, 8), 'rule')
+                        # E.g., ((32, 4, 8), 'rule', 'tag')
                         items = (ParTileArg(*items),)
                     else:
                         try:
-                            # E.g., (((32, 4, 8), 1), ((32, 4, 4), 2))
-                            # E.g., (((32, 4, 8), 1, 'tag0'), ((32, 4, 4), 2, 'tag1'))
+                            # E.g., (((32, 4, 8), 'rule'), ((32, 4, 4), 'rule'))
+                            # E.g., (((32, 4, 8), 'rule0', 'tag0'),
+                            #        ((32, 4, 4), 'rule1', 'tag1'))
                             items = tuple(ParTileArg(*i) for i in items)
                         except TypeError:
                             # E.g., ((32, 4, 8), (32, 4, 4))
                             items = tuple(ParTileArg(i) for i in items)
                 except IndexError:
                     # E.g., ((32, 4, 8),)
                     items = (ParTileArg(x),)
             else:
                 raise ValueError("Expected int or tuple, got %s instead" % type(x))
         else:
             raise ValueError("Expected bool or iterable, got %s instead" % type(items))
 
-        obj = super().__new__(cls, items)
+        obj = super().__new__(cls, *items)
         obj.default = as_tuple(default)
+        obj.sparse = as_tuple(sparse)
+        obj.reduce = as_tuple(reduce)
 
         return obj
```

### Comparing `devito-4.8.3/devito/data/allocators.py` & `devito-4.8.4/devito/data/allocators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import abc
 from functools import reduce
 from operator import mul
+import ctypes
+from ctypes.util import find_library
 import mmap
 import os
 import sys
 
 import numpy as np
-import ctypes
-from ctypes.util import find_library
 
 from devito.logger import logger
 from devito.parameters import configuration
-from devito.tools import dtype_to_ctype
+from devito.tools import dtype_to_ctype, is_integer
 
-__all__ = ['ALLOC_FLAT', 'ALLOC_NUMA_LOCAL', 'ALLOC_NUMA_ANY',
+__all__ = ['ALLOC_ALIGNED', 'ALLOC_NUMA_LOCAL', 'ALLOC_NUMA_ANY',
            'ALLOC_KNL_MCDRAM', 'ALLOC_KNL_DRAM', 'ALLOC_GUARD',
            'default_allocator']
 
 
 class MemoryAllocator(object):
 
     """Abstract class defining the interface to memory allocators."""
 
     __metaclass__ = abc.ABCMeta
 
-    is_Posix = False
-    is_Numa = False
-
     _attempted_init = False
     lib = None
 
     guaranteed_alignment = 64
     """Guaranteed data alignment."""
 
     @classmethod
@@ -47,51 +44,69 @@
 
         Notes
         -----
         This method must be implemented by all subclasses of MemoryAllocator.
         """
         return
 
-    def alloc(self, shape, dtype):
+    def alloc(self, shape, dtype, padding=0):
         """
         Allocate memory.
 
         Parameters
         ----------
         shape : tuple of ints
             Shape of the allocated array.
         dtype : numpy.dtype
             The data type of the raw data.
+        padding : int or 2-tuple of ints, optional
+            The number of points that are allocated before and after the data,
+            that is in addition to the requested shape. Defaults to 0.
 
         Returns
         -------
         pointer, memfree_args
             The first element of the tuple is the reference that can be used to
             access the data as a ctypes object. The second element is an opaque
             object that is needed only for the "memfree" call.
         """
-        size = int(reduce(mul, shape))
+        datasize = int(reduce(mul, shape))
         ctype = dtype_to_ctype(dtype)
 
-        c_pointer, memfree_args = self._alloc_C_libcall(size, ctype)
-        if c_pointer is None:
-            raise RuntimeError("Unable to allocate %d elements in memory", str(size))
+        # Add padding, if any
+        try:
+            padleft, padright = padding
+        except TypeError:
+            padleft, padright = padding, padding
+        if not is_integer(padleft) and not is_integer(padright):
+            raise TypeError("padding must be an int or a 2-tuple of ints")
+        size = datasize + padleft + padright
+
+        padleft_pointer, memfree_args = self._alloc_C_libcall(size, ctype)
+        if padleft_pointer is None:
+            raise RuntimeError("Unable to allocate %d elements in memory" % size)
+
+        # Compute the pointer to the user data
+        padleft_bytes = padleft * ctypes.sizeof(ctype)
+        c_pointer = ctypes.c_void_p(padleft_pointer.value + padleft_bytes)
 
-        # cast to 1D array of the specified size
-        ctype_1d = ctype * size
+        # Cast to 1D array of the specified `datasize`
+        ctype_1d = ctype * datasize
         buf = ctypes.cast(c_pointer, ctypes.POINTER(ctype_1d)).contents
-        pointer = np.frombuffer(buf, dtype=dtype)
-        # pointer.reshape should not be used here because it may introduce a copy
-        # From https://docs.scipy.org/doc/numpy/reference/generated/numpy.reshape.html:
-        # It is not always possible to change the shape of an array without copying the
-        # data. If you want an error to be raised when the data is copied, you should
-        # assign the new shape to the shape attribute of the array:
-        pointer.shape = shape
+        array = np.frombuffer(buf, dtype=dtype)
 
-        return (pointer, memfree_args)
+        # `array.reshape` should not be used here because it may introduce
+        # a copy. From `docs.scipy.org/doc/numpy/reference/generated/numpy.reshape`:
+        #   It is not always possible to change the shape of an array without
+        #   copying the data. If you want an error to be raised when the data
+        #   is copied, you should assign the new shape to the shape attribute
+        #   of the array:
+        array.shape = shape
+
+        return (array, memfree_args)
 
     @abc.abstractmethod
     def _alloc_C_libcall(self, size, ctype):
         """
         Perform the actual memory allocation by calling a C function.  Should
         return a 2-tuple (c_pointer, memfree_args), where the free args are
         what is handed back to free() later to deallocate.
@@ -120,16 +135,14 @@
 class PosixAllocator(MemoryAllocator):
 
     """
     Memory allocator based on ``posix`` functions. The allocated memory is
     aligned to page boundaries.
     """
 
-    is_Posix = True
-
     @classmethod
     def initialize(cls):
         handle = find_library('c')
 
         # Special case: on MacOS Big Sur any code that attempts to check
         # for dynamic library presence by looking for a file at a path
         # will fail. For this case, a static path is provided.
@@ -158,15 +171,15 @@
     def free(self, c_pointer):
         self.lib.free(c_pointer)
 
 
 class GuardAllocator(PosixAllocator):
 
     """
-    Memory allocator based on ``posix`` functions. The allocated memory is
+    Memory allocator based on `posix` functions. The allocated memory is
     aligned to page boundaries.  Additionally, it allocates extra memory
     before and after the data, and configures it so that an SEGV is thrown
     immediately if an out-of-bounds access occurs.
 
     Further, the remainder region of the last page (which cannot be
     protected), is poisoned with NaNs.
     """
@@ -191,45 +204,45 @@
         c_bytesize = ctypes.c_ulong(npages_alloc * pagesize)
         c_pointer = ctypes.cast(ctypes.c_void_p(), ctypes.c_void_p)
         alignment = self.lib.getpagesize()
         ret = self.lib.posix_memalign(ctypes.byref(c_pointer), alignment, c_bytesize)
         if ret != 0:
             return None, None
 
-        # generate pointers to the left padding, the user data, and the right pad
+        # Generate pointers to the left padding, the user data, and the right pad
         padleft_pointer = c_pointer
         c_pointer = ctypes.c_void_p(c_pointer.value + self.padding_bytes)
         padright_pointer = ctypes.c_void_p(c_pointer.value + npages_user * pagesize)
 
-        # and set the permissions on the pad memory to 0 (no access)
-        # if these fail, don't worry about failing the entire allocation
+        # And set the permissions on the pad memory to 0 (no access)
+        # If these fail, don't worry about failing the entire allocation
         c_padsize = ctypes.c_ulong(self.padding_bytes)
         if self.lib.mprotect(padleft_pointer, c_padsize, ctypes.c_int(0)):
             logger.warning("couldn't protect memory")
         if self.lib.mprotect(padright_pointer, c_padsize, ctypes.c_int(0)):
             logger.warning("couldn't protect memory")
 
-        # if there is a multiple of 4 bytes left, use the code below to poison
+        # If there is a multiple of 4 bytes left, use the code below to poison
         # the memory
         if nbytes_user % 4 == 0:
             poison_size = npages_user*pagesize - nbytes_user
             intp_type = ctypes.POINTER(ctypes.c_int)
             poison_ptr = ctypes.cast(ctypes.c_void_p(c_pointer.value + nbytes_user),
                                      intp_type)
 
-            # for both float32 and float64, a sequence of -100 int32s represents NaNs,
-            # at least on little-endian architectures.  It shouldn't matter what we
-            # put in there, anyway
+            # For both float32 and float64, a sequence of -100 int32s
+            # represents NaNs, at least on little-endian architectures;
+            # it shouldn't matter what we put in there, anyway
             for i in range(poison_size // 4):
                 poison_ptr[i] = -100
 
         return c_pointer, (padleft_pointer, c_bytesize)
 
     def free(self, c_pointer, total_size):
-        # unprotect it, since free() accesses it, I think...
+        # Unprotect it, since free() accesses it, I think...
         self.lib.mprotect(c_pointer, total_size,
                           ctypes.c_int(mmap.PROT_READ | mmap.PROT_WRITE))
         self.lib.free(c_pointer)
 
 
 class NumaAllocator(MemoryAllocator):
 
@@ -243,16 +256,14 @@
     ----------
     node : int or str
         If an integer, it indicates a specific NUMA node. Otherwise, the two
         keywords ``local`` ("allocate on the local NUMA node") and ``any``
         ("allocate on any NUMA node with sufficient free memory") are accepted.
     """
 
-    is_Numa = True
-
     @classmethod
     def initialize(cls):
         handle = find_library('numa')
         if handle is None:
             return
         lib = ctypes.CDLL(handle)
         if lib.numa_available() == -1:
@@ -264,15 +275,15 @@
         # Required because numa_alloc* functions return pointers
         lib.numa_alloc_onnode.restype = ctypes.c_void_p
         lib.numa_alloc_local.restype = ctypes.c_void_p
         lib.numa_alloc.restype = ctypes.c_void_p
         cls.lib = lib
 
     def __init__(self, node):
-        super(NumaAllocator, self).__init__()
+        super().__init__()
         self._node = node
 
     def _alloc_C_libcall(self, size, ctype):
         if not self.available():
             raise RuntimeError("Couldn't find `libnuma`'s `numa_alloc_*` to "
                                "allocate memory")
 
@@ -352,27 +363,27 @@
     array([[1., 2.],
            [1., 1.]], dtype=float32)
     """
 
     def __init__(self, numpy_array):
         self.numpy_array = numpy_array
 
-    def alloc(self, shape, dtype):
+    def alloc(self, shape, dtype, padding=0):
         assert shape == self.numpy_array.shape, \
             "Provided array has shape %s. Expected %s" %\
             (str(self.numpy_array.shape), str(shape))
         assert dtype == self.numpy_array.dtype, \
             "Provided array has dtype %s. Expected %s" %\
             (str(self.numpy_array.dtype), str(dtype))
 
         return (self.numpy_array, None)
 
 
 ALLOC_GUARD = GuardAllocator(1048576)
-ALLOC_FLAT = PosixAllocator()
+ALLOC_ALIGNED = PosixAllocator()
 ALLOC_KNL_DRAM = NumaAllocator(0)
 ALLOC_KNL_MCDRAM = NumaAllocator(1)
 ALLOC_NUMA_ANY = NumaAllocator('any')
 ALLOC_NUMA_LOCAL = NumaAllocator('local')
 
 custom_allocators = {}
 """User-defined allocators."""
@@ -399,16 +410,16 @@
 
 def default_allocator(name=None):
     """
     Return a MemoryAllocator for the underlying architecture.
 
         * ALLOC_GUARD: Only used in so-called "develop mode", to trigger SIGSEGV as
                        soon as OOB accesses are performed.
-        * ALLOC_FLAT: Align memory to page boundaries using the posix function
-                      `posix_memalign`.
+        * ALLOC_ALIGNED: Align memory to page boundaries using the function
+                         `posix_memalign`.
         * ALLOC_NUMA_LOCAL: Allocate memory in the "closest" NUMA node. This only
                             makes sense on a NUMA architecture. Falls back to
                             allocation in an arbitrary NUMA node if there isn't
                             enough space.
         * ALLOC_NUMA_ANY: Allocate memory in an arbitrary NUMA node.
         * ALLOC_KNL_MCDRAM: On a Knights Landing platform, allocate memory in MCDRAM.
                             Falls back to DRAM if there isn't enough space.
@@ -420,14 +431,13 @@
         try:
             return custom_allocators[name]
         except KeyError:
             pass
 
     if configuration['develop-mode']:
         return ALLOC_GUARD
-    elif NumaAllocator.available():
-        if configuration['platform'].name == 'knl' and infer_knl_mode() == 'flat':
-            return ALLOC_KNL_MCDRAM
-        else:
-            return ALLOC_NUMA_LOCAL
+    elif (NumaAllocator.available() and
+          configuration['platform'].name == 'knl' and
+          infer_knl_mode() == 'flat'):
+        return ALLOC_KNL_MCDRAM
     else:
-        return ALLOC_FLAT
+        return custom_allocators.get('default', ALLOC_ALIGNED)
```

### Comparing `devito-4.8.3/devito/data/data.py` & `devito-4.8.4/devito/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable
 from functools import wraps
 
 import numpy as np
 
-from devito.data.allocators import ALLOC_FLAT
+from devito.data.allocators import ALLOC_ALIGNED
 from devito.data.utils import *
 from devito.logger import warning
 from devito.parameters import configuration
 from devito.tools import Tag, as_tuple, as_list, is_integer
 
 __all__ = ['Data']
 
@@ -22,36 +22,40 @@
     shape : tuple of ints
         Shape of created array.
     dtype : numpy.dtype
         The data type of the raw data.
     decomposition : tuple of Decomposition, optional
         The data decomposition, for each dimension.
     modulo : tuple of bool, optional
-        If the i-th entry is True, then the i-th array dimension uses modulo indexing.
+        If the i-th entry is True, then the i-th array dimension uses modulo
+        indexing.
     allocator : MemoryAllocator, optional
-        Used to allocate memory. Defaults to ``ALLOC_FLAT``.
+        Used to allocate memory. Defaults to `ALLOC_ALIGNED`.
     distributor : Distributor, optional
-        The distributor from which the original decomposition was produced. Note that
-        the decomposition Parameter above may be different to distributor.decomposition.
+        The distributor from which the original decomposition was produced.
+        Note that `decomposition` may differ from `distributor.decomposition`.
+    padding : int or 2-tuple of ints, optional
+        The number of points that are allocated before and after the data,
+        that is in addition to the requested shape. Defaults to 0.
 
     Notes
     -----
     NumPy array subclassing is described at: ::
 
         https://numpy.org/doc/stable/user/basics.subclassing.html
 
     Any view or copy created from ``self``, for instance via a slice operation
     or a universal function ("ufunc" in NumPy jargon), will still be of type
     `Data`.
     """
 
-    def __new__(cls, shape, dtype, decomposition=None, modulo=None, allocator=ALLOC_FLAT,
-                distributor=None):
+    def __new__(cls, shape, dtype, decomposition=None, modulo=None,
+                allocator=ALLOC_ALIGNED, distributor=None, padding=0):
         assert len(shape) == len(modulo)
-        ndarray, memfree_args = allocator.alloc(shape, dtype)
+        ndarray, memfree_args = allocator.alloc(shape, dtype, padding=padding)
         obj = ndarray.view(cls)
         obj._allocator = allocator
         obj._memfree_args = memfree_args
         obj._decomposition = decomposition or (None,)*len(shape)
         obj._modulo = modulo or (False,)*len(shape)
         obj._distributor = distributor
 
@@ -105,14 +109,15 @@
         self._memfree_args = None
 
         if not issubclass(type(obj), Data):
             # Definitely from view casting
             self._is_distributed = False
             self._modulo = tuple(False for i in range(self.ndim))
             self._decomposition = (None,)*self.ndim
+            self._allocator = ALLOC_ALIGNED
         elif obj._index_stash is not None:
             # From `__getitem__`
             self._is_distributed = obj._is_distributed
             self._distributor = obj._distributor
             glb_idx = obj._normalize_index(obj._index_stash)
             self._modulo = tuple(m for i, m in zip(glb_idx, obj._modulo)
                                  if not is_integer(i))
@@ -121,17 +126,19 @@
                 if is_integer(i):
                     continue
                 elif dec is None:
                     decomposition.append(None)
                 else:
                     decomposition.append(dec.reshape(i))
             self._decomposition = tuple(decomposition)
+            self._allocator = obj._allocator
         else:
             self._is_distributed = obj._is_distributed
             self._distributor = obj._distributor
+            self._allocator = obj._allocator
             if self.ndim == obj.ndim:
                 # E.g., from a ufunc, such as `np.add`
                 self._modulo = obj._modulo
                 self._decomposition = obj._decomposition
             else:
                 # E.g., from a reduction operation such as `np.mean` or `np.all`
                 self._modulo = tuple(False for i in range(self.ndim))
@@ -239,15 +246,15 @@
                 return retval
             else:
                 return None
         elif comm_type is index_by_index or is_gather:
             # Retrieve the pertinent local data prior to MPI send/receive operations
             data_idx = loc_data_idx(loc_idx)
             self._index_stash = flip_idx(glb_idx, self._decomposition)
-            local_val = super(Data, self).__getitem__(data_idx)
+            local_val = super().__getitem__(data_idx)
             self._index_stash = None
 
             comm = self._distributor.comm
             rank = comm.Get_rank()
 
             owners, send, global_si, local_si = \
                 mpi_index_maps(loc_idx, local_val.shape, self._distributor.topology,
@@ -310,31 +317,31 @@
                 return retval
         elif loc_idx is NONLOCAL:
             # Caller expects a scalar. However, `glb_idx` doesn't belong to
             # self's data partition, so None is returned
             return None
         else:
             self._index_stash = glb_idx
-            retval = super(Data, self).__getitem__(loc_idx)
+            retval = super().__getitem__(loc_idx)
             self._index_stash = None
             return retval
 
     @_check_idx
     def __setitem__(self, glb_idx, val, comm_type):
         loc_idx = self._index_glb_to_loc(glb_idx)
         if loc_idx is NONLOCAL:
             # no-op
             return
         elif np.isscalar(val):
             if index_is_basic(loc_idx):
                 # Won't go through `__getitem__` as it's basic indexing mode,
                 # so we should just propage `loc_idx`
-                super(Data, self).__setitem__(loc_idx, val)
+                super().__setitem__(loc_idx, val)
             else:
-                super(Data, self).__setitem__(glb_idx, val)
+                super().__setitem__(glb_idx, val)
         elif isinstance(val, Data) and val._is_distributed:
             if comm_type is index_by_index:
                 glb_idx, val = self._process_args(glb_idx, val)
                 val_idx = as_tuple([slice(i.glb_min, i.glb_max+1, 1) for
                                     i in val._decomposition])
                 idx = self._set_global_idx(val, glb_idx, val_idx)
                 comm = self._distributor.comm
@@ -349,15 +356,15 @@
                 for j in range(nprocs):
                     skip = any(i is None for i in idx_global[j]) \
                         or data_global[j].size == 0
                     if not skip:
                         self.__setitem__(idx_global[j], data_global[j])
             elif self._is_distributed:
                 # `val` is decomposed, `self` is decomposed -> local set
-                super(Data, self).__setitem__(glb_idx, val)
+                super().__setitem__(glb_idx, val)
             else:
                 # `val` is decomposed, `self` is replicated -> gatherall-like
                 raise NotImplementedError
         elif isinstance(val, np.ndarray):
             if self._is_distributed:
                 # `val` is replicated, `self` is decomposed -> `val` gets decomposed
                 glb_idx = self._normalize_index(glb_idx)
@@ -385,21 +392,21 @@
                     else:
                         processed.append(j)
                 val_idx = as_tuple(processed)
                 val = val[val_idx]
             else:
                 # `val` is replicated`, `self` is replicated -> plain ndarray.__setitem__
                 pass
-            super(Data, self).__setitem__(glb_idx, val)
+            super().__setitem__(glb_idx, val)
         elif isinstance(val, Iterable):
             if self._is_mpi_distributed:
                 raise NotImplementedError("With MPI, data can only be set "
                                           "via scalars, numpy arrays or "
                                           "other data ")
-            super(Data, self).__setitem__(glb_idx, val)
+            super().__setitem__(glb_idx, val)
         else:
             raise ValueError("Cannot insert obj of type `%s` into a Data" % type(val))
 
     def _normalize_index(self, idx):
         if isinstance(idx, np.ndarray):
             # Advanced indexing mode
             return (idx,)
```

### Comparing `devito-4.8.3/devito/data/decomposition.py` & `devito-4.8.4/devito/data/decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def __new__(cls, items, local):
         if len(items) == 0:
             raise ValueError("The decomposition must contain at least one subdomain")
         if not all(isinstance(i, Iterable) for i in items):
             raise TypeError("Illegal Decomposition element type")
         if not is_integer(local) and (0 <= local < len(items)):
             raise ValueError("`local` must be an index in ``items``.")
-        obj = super(Decomposition, cls).__new__(cls, [np.array(i) for i in items])
+        obj = super().__new__(cls, [np.array(i) for i in items])
         obj._local = local
         return obj
 
     @property
     def local(self):
         return self._local
 
@@ -320,20 +320,24 @@
             if self.loc_empty:
                 return None
             abs_ofs, side = args
             if side is LEFT:
                 rel_ofs = self.glb_min + abs_ofs - base
                 if abs_ofs >= base and abs_ofs <= top:
                     return rel_ofs
+                elif abs_ofs > top:
+                    return top + 1
                 else:
                     return None
             else:
                 rel_ofs = abs_ofs - (self.glb_max - top)
                 if abs_ofs >= self.glb_max - top and abs_ofs <= self.glb_max - base:
                     return rel_ofs
+                elif abs_ofs > self.glb_max - base:
+                    return self.glb_max - base + 1
                 else:
                     return None
         else:
             raise TypeError("Expected 1 or 2 arguments, found %d" % len(args))
 
     def index_loc_to_glb(self, *args):
         """
```

### Comparing `devito-4.8.3/devito/data/meta.py` & `devito-4.8.4/devito/data/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 NOPAD = DataRegion('nopad', 4)  # == DOMAIN+HALO
 FULL = DataRegion('full', 5)  # == DOMAIN+HALO+PADDING
 
 
 class DataSide(Tag):
 
     def __init__(self, name, val, flipto=None):
-        super(DataSide, self).__init__(name, val)
+        super().__init__(name, val)
         self.flipto = flipto
         if flipto is not None:
             flipto.flipto = self
 
     def flip(self):
         if self.flipto is not None:
             return self.flipto
```

### Comparing `devito-4.8.3/devito/data/utils.py` & `devito-4.8.4/devito/data/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/finite_differences/coefficients.py` & `devito-4.8.4/devito/finite_differences/coefficients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from cached_property import cached_property
 
-from devito.finite_differences import generate_indices
+from devito.finite_differences import Weights, generate_indices
 from devito.finite_differences.tools import numeric_weights, symbolic_weights
 from devito.tools import filter_ordered, as_tuple
 
 __all__ = ['Coefficient', 'Substitutions', 'default_rules']
 
 
 class Coefficient(object):
@@ -85,15 +85,15 @@
 
     @property
     def index(self):
         """
         The dimension to which the coefficients will be applied plus the offset
         in that dimension if the function is staggered.
         """
-        return self._function.indices_ref[self._dimension]
+        return self._dimension
 
     @property
     def weights(self):
         """The set of weights."""
         return self._weights
 
     def _check_input(self, deriv_order, function, dimension, weights):
@@ -253,42 +253,72 @@
         # Actual FD used indices and weights
         if deriv_order == 1 and fd_order == 2:
             fd_order = 1
 
         indices, x0 = generate_indices(function, dim,
                                        fd_order, side=None, x0=mapper)
 
-        coeffs = numeric_weights(deriv_order, indices, x0)
+        coeffs = numeric_weights(function, deriv_order, indices, x0)
 
         for (c, i) in zip(coeffs, indices):
             subs.update({function._coeff_symbol(i, deriv_order, function, index): c})
 
         # Set all unused weights to zero
         subs.update({w: 0 for w in sweights if w not in subs})
 
         return subs
 
     # Determine which 'rules' are missing
     sym = get_sym(functions)
     terms = obj.find(sym)
+    for i in obj.find(Weights):
+        for w in i.weights:
+            terms.update(w.find(sym))
+
     args_present = filter_ordered(term.args[1:] for term in terms)
 
     subs = obj.substitutions
     if subs:
         args_provided = [(i.deriv_order, i.function, i.index)
                          for i in subs.coefficients]
     else:
         args_provided = []
 
     # NOTE: Do we want to throw a warning if the same arg has
     # been provided twice?
     args_provided = list(set(args_provided))
-    not_provided = [i for i in args_present if i not in frozenset(args_provided)]
 
     rules = {}
+    not_provided = []
+    for i0 in args_present:
+        if any(i0 == i1 for i1 in args_provided):
+            # Perfect match, as expected by the legacy custom coeffs API
+            continue
+
+        # TODO: to make cross-derivs work, we must relax `not_provided` by
+        # checking not for equality, but rather for inclusion. This is ugly,
+        # but basically a major revamp is the only alternative... and for now,
+        # it does the trick
+        mapper = {}
+        deriv_order, expr, dim = i0
+        try:
+            for k, v in subs.rules.items():
+                ofs, do, f, d = k.args
+                is_dim = dim == expr.indices_ref[d]
+                if deriv_order == do and is_dim and f in expr._functions:
+                    mapper[k.func(ofs, do, expr, expr.indices_ref[d])] = v
+        except AttributeError:
+            # assert subs is None
+            pass
+
+        if mapper:
+            rules.update(mapper)
+        else:
+            not_provided.append(i0)
+
     for i in not_provided:
         rules = {**rules, **generate_subs(*i)}
 
     return rules
 
 
 def get_sym(functions):
```

### Comparing `devito-4.8.3/devito/finite_differences/derivative.py` & `devito-4.8.4/devito/finite_differences/derivative.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from cached_property import cached_property
 import sympy
 
 from .finite_difference import generic_derivative, first_derivative, cross_derivative
 from .differentiable import Differentiable
 from .tools import direct, transpose
+from .rsfd import d45
 from devito.tools import as_mapper, as_tuple, filter_ordered, frozendict
 from devito.types.utils import DimensionTuple
 
 __all__ = ['Derivative']
 
 
 class Derivative(sympy.Derivative, Differentiable):
@@ -21,26 +22,26 @@
     upon evaluation.
 
     Parameters
     ----------
     expr : expr-like
         Expression for which the Derivative is produced.
     dims : Dimension or tuple of Dimension
-        Dimenions w.r.t. which to differentiate.
-    fd_order : int or tuple of int, optional
+        Dimensions w.r.t. which to differentiate.
+    fd_order : int or tuple of int, optional, default=1
         Coefficient discretization order. Note: this impacts the width of
-        the resulting stencil. Defaults to 1.
-    deriv_order: int or tuple of int, optional
-        Derivative order. Defaults to 1.
-    side : Side or tuple of Side, optional
+        the resulting stencil.
+    deriv_order: int or tuple of int, optional, default=1
+        Derivative order.
+    side : Side or tuple of Side, optional, default=centered
         Side of the finite difference location, centered (at x), left (at x - 1)
-        or right (at x +1). Defaults to ``centered``.
-    transpose : Transpose, optional
+        or right (at x +1).
+    transpose : Transpose, optional, default=direct
         Forward (matvec=direct) or transpose (matvec=transpose) mode of the
-        finite difference. Defaults to ``direct``.
+        finite difference.
     subs : dict, optional
         Substitutions to apply to the finite-difference expression after evaluation.
     x0 : dict, optional
         Origin (where the finite-difference is evaluated at) for the finite-difference
         scheme, e.g. {x: x, y: y + h_y/2}.
 
     Examples
@@ -82,15 +83,16 @@
     will create the second derivative at x=x + x.spacing. Accepted arguments for dynamic
     evaluation are `x0`, `fd_order` and `side`.
     """
 
     _fd_priority = 3
 
     __rargs__ = ('expr', 'dims')
-    __rkwargs__ = ('side', 'deriv_order', 'fd_order', 'transpose', '_ppsubs', 'x0')
+    __rkwargs__ = ('side', 'deriv_order', 'fd_order', 'transpose', '_ppsubs',
+                   'x0', 'method')
 
     def __new__(cls, expr, *dims, **kwargs):
         if type(expr) is sympy.Derivative:
             raise ValueError("Cannot nest sympy.Derivative with devito.Derivative")
         if not isinstance(expr, Differentiable):
             raise ValueError("`expr` must be a Differentiable object")
 
@@ -102,14 +104,15 @@
 
         skip = kwargs.get('preprocessed', False) or obj.ndims == 1
 
         obj._fd_order = fd_o if skip else DimensionTuple(*fd_o, getters=obj._dims)
         obj._deriv_order = orders if skip else DimensionTuple(*orders, getters=obj._dims)
         obj._side = kwargs.get("side")
         obj._transpose = kwargs.get("transpose", direct)
+        obj._method = kwargs.get("method", 'FD')
 
         ppsubs = kwargs.get("subs", kwargs.get("_ppsubs", []))
         processed = []
         if ppsubs:
             for i in ppsubs:
                 try:
                     processed.append(frozendict(i))
@@ -179,20 +182,22 @@
         # SymPy expects the list of variable w.r.t. which we differentiate to be a list
         # of 2-tuple `(s, count)` where s is the entity to diff wrt and count is the order
         # of the derivative
         variable_count = [sympy.Tuple(s, new_dims.count(s))
                           for s in filter_ordered(new_dims)]
         return new_dims, orders, fd_orders, variable_count
 
-    def __call__(self, x0=None, fd_order=None, side=None):
+    def __call__(self, x0=None, fd_order=None, side=None, method=None):
         if self.ndims == 1:
-            _fd_order = fd_order or self._fd_order
-            _side = side or self._side
-            new_x0 = {self.dims[0]: x0} if x0 is not None else self.x0
-            return self._new_from_self(fd_order=_fd_order, side=_side, x0=new_x0)
+            fd_order = fd_order or self._fd_order
+            side = side or self._side
+            method = method or self._method
+            x0 = {self.dims[0]: x0} if x0 is not None else self.x0
+            return self._new_from_self(fd_order=fd_order, side=side, x0=x0,
+                                       method=method)
 
         if side is not None:
             raise TypeError("Side only supported for first order single"
                             "Dimension derivative such as `.dxl` or .dx(side=left)")
         # Cross derivative
         _x0 = dict(self._x0)
         _fd_order = dict(self.fd_order._getters)
@@ -206,15 +211,15 @@
 
         return self._new_from_self(fd_order=_fd_order, x0=_x0)
 
     def _new_from_self(self, **kwargs):
         expr = kwargs.pop('expr', self.expr)
         _kwargs = {'deriv_order': self.deriv_order, 'fd_order': self.fd_order,
                    'side': self.side, 'transpose': self.transpose, 'subs': self._ppsubs,
-                   'x0': self.x0, 'preprocessed': True}
+                   'x0': self.x0, 'preprocessed': True, 'method': self.method}
         _kwargs.update(**kwargs)
         return Derivative(expr, *self.dims, **_kwargs)
 
     def func(self, expr, *args, **kwargs):
         return self._new_from_self(expr=expr, **kwargs)
 
     def _subs(self, old, new, **hints):
@@ -302,14 +307,18 @@
         return self._transpose
 
     @property
     def is_TimeDependent(self):
         return self.expr.is_TimeDependent
 
     @property
+    def method(self):
+        return self._method
+
+    @property
     def T(self):
         """Transpose of the Derivative.
 
         FD derivatives can be represented as matrices and have adjoint/transpose.
         This is really useful for more advanced FD definitions. For example
         the conventional Laplacian is `.dxl.T * .dxl`
         """
@@ -380,22 +389,29 @@
             pass
 
         # If True, the derivative will be fully expanded as a sum of products,
         # otherwise an IndexSum will returned
         expand = kwargs.get('expand', True)
 
         # Step 2: Evaluate FD of the new expression
-        if self.side is not None and self.deriv_order == 1:
+        if self.method == 'RSFD':
+            assert len(self.dims) == 1
+            assert self.deriv_order == 1
+            res = d45(expr, self.dims[0], x0=self.x0, expand=expand)
+        elif self.side is not None and self.deriv_order == 1:
+            assert self.method == 'FD'
             res = first_derivative(expr, self.dims[0], self.fd_order,
                                    side=self.side, matvec=self.transpose,
                                    x0=self.x0, expand=expand)
         elif len(self.dims) > 1:
+            assert self.method == 'FD'
             res = cross_derivative(expr, self.dims, self.fd_order, self.deriv_order,
                                    matvec=self.transpose, x0=self.x0, expand=expand)
         else:
+            assert self.method == 'FD'
             res = generic_derivative(expr, *self.dims, self.fd_order, self.deriv_order,
                                      matvec=self.transpose, x0=self.x0, expand=expand)
 
         # Step 3: Apply substitutions
         for e in self._ppsubs:
             res = res.xreplace(e)
```

### Comparing `devito-4.8.3/devito/finite_differences/differentiable.py` & `devito-4.8.4/devito/finite_differences/differentiable.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from functools import singledispatch
 
 from cached_property import cached_property
 import numpy as np
 import sympy
 from sympy.core.add import _addsort
 from sympy.core.mul import _keep_coeff, _mulsort
+from sympy.core.core import ordering_of_classes
 from sympy.core.decorators import call_highest_priority
 from sympy.core.evalf import evalf_table
 
-from devito.finite_differences.tools import make_shift_x0
+from devito.finite_differences.tools import make_shift_x0, coeff_priority
 from devito.logger import warning
 from devito.tools import (as_tuple, filter_ordered, flatten, frozendict,
                           infer_dtype, is_integer, split)
-from devito.types import (Array, DimensionTuple, Evaluable, Indexed, Spacing,
+from devito.types import (Array, DimensionTuple, Evaluable, Indexed,
                           StencilDimension)
 
-__all__ = ['Differentiable', 'IndexDerivative', 'EvalDerivative', 'Weights']
+__all__ = ['Differentiable', 'DiffDerivative', 'IndexDerivative', 'EvalDerivative',
+           'Weights']
 
 
 class Differentiable(sympy.Expr, Evaluable):
 
     """
     A Differentiable is an algebric expression involving Functions, which can
     be derived w.r.t. one or more Dimensions.
@@ -100,24 +102,48 @@
 
     @cached_property
     def is_TimeDependent(self):
         return any(i.is_Time for i in self.dimensions)
 
     @cached_property
     def _fd(self):
-        return dict(ChainMap(*[getattr(i, '_fd', {}) for i in self._args_diff]))
+        # Filter out all args with fd order too high
+        fd_args = []
+        for f in self._args_diff:
+            try:
+                if f.space_order <= self.space_order and \
+                        (not f.is_TimeDependent or f.time_order <= self.time_order):
+                    fd_args.append(f)
+            except AttributeError:
+                pass
+        return dict(ChainMap(*[getattr(i, '_fd', {}) for i in fd_args]))
 
     @cached_property
     def _symbolic_functions(self):
         return frozenset([i for i in self._functions if i.coefficients == 'symbolic'])
 
     @cached_property
     def _uses_symbolic_coefficients(self):
         return bool(self._symbolic_functions)
 
+    @cached_property
+    def coefficients(self):
+        coefficients = {f.coefficients for f in self._functions}
+        # If there is multiple ones, we have to revert to the highest priority
+        # i.e we have to remove symbolic
+        key = lambda x: coeff_priority[x]
+        return sorted(coefficients, key=key, reverse=True)[0]
+
+    @cached_property
+    def _coeff_symbol(self, *args, **kwargs):
+        if self._uses_symbolic_coefficients:
+            return W
+        else:
+            raise ValueError("Couldn't find any symbolic coefficients")
+
     def _eval_at(self, func):
         if not func.is_Staggered:
             # Cartesian grid, do no waste time
             return self
         return self.func(*[getattr(a, '_eval_at', lambda x: a)(func) for a in self.args])
 
     def _subs(self, old, new, **hints):
@@ -138,15 +164,15 @@
         return self.func(*[getattr(a, '_eval_deriv', a) for a in self.args])
 
     @property
     def _fd_priority(self):
         return .75 if self.is_TimeDependent else .5
 
     def __hash__(self):
-        return super(Differentiable, self).__hash__()
+        return super().__hash__()
 
     def __getattr__(self, name):
         """
         Try calling a dynamically created FD shortcut.
 
         Notes
         -----
@@ -224,21 +250,29 @@
     def __rmod__(self, other):
         return Mod(other, self)
 
     def __neg__(self):
         return Mul(sympy.S.NegativeOne, self)
 
     def __eq__(self, other):
-        ret = super(Differentiable, self).__eq__(other)
+        ret = super().__eq__(other)
         if ret is NotImplemented or not ret:
             # Non comparable or not equal as sympy objects
             return False
         return all(getattr(self, i, None) == getattr(other, i, None)
                    for i in self.__rkwargs__)
 
+    def _hashable_content(self):
+        # SymPy computes the hash of all Basic objects as:
+        # `hash((type(self).__name__,) + self._hashable_content())`
+        # However, our subclasses will be named after the main SymPy classes,
+        # for example sympy.Add -> differentiable.Add, so we need to override
+        # the hashable content to specify it's our own subclasses
+        return super()._hashable_content() + ('differentiable',)
+
     @property
     def name(self):
         return "".join(f.name for f in self._functions)
 
     def shift(self, dim, shift):
         """
         Shift  expression by `shift` along the Dimension `dim`.
@@ -248,29 +282,88 @@
 
     @property
     def laplace(self):
         """
         Generates a symbolic expression for the Laplacian, the second
         derivative w.r.t all spatial Dimensions.
         """
+        return self.laplacian()
+
+    def laplacian(self, shift=None, order=None):
+        """
+        Laplacian of the Differentiable with shifted derivatives and custom
+        FD order.
+
+        Each second derivative is left-right (i.e D^T D with D the first derivative ):
+        `(self.dx(x0=dim+shift*dim.spacing,
+                  fd_order=order)).dx(x0=dim-shift*dim.spacing, fd_order=order)`
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        """
+        order = order or self.space_order
         space_dims = [d for d in self.dimensions if d.is_Space]
+        shift_x0 = make_shift_x0(shift, (len(space_dims),))
         derivs = tuple('d%s2' % d.name for d in space_dims)
-        return Add(*[getattr(self, d) for d in derivs])
-
-    def div(self, shift=None):
+        return Add(*[getattr(self, d)(x0=shift_x0(shift, space_dims[i], None, i),
+                                      fd_order=order)
+                     for i, d in enumerate(derivs)])
+
+    def div(self, shift=None, order=None, method='FD'):
+        """
+        Divergence of the input Function.
+
+        Parameters
+        ----------
+        func : Function or TensorFunction
+            Function to take the divergence of
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
+        """
         space_dims = [d for d in self.dimensions if d.is_Space]
         shift_x0 = make_shift_x0(shift, (len(space_dims),))
-        return Add(*[getattr(self, 'd%s' % d.name)(x0=shift_x0(shift, d, None, i))
+        order = order or self.space_order
+        return Add(*[getattr(self, 'd%s' % d.name)(x0=shift_x0(shift, d, None, i),
+                                                   fd_order=order, method=method)
                      for i, d in enumerate(space_dims)])
 
-    def grad(self, shift=None):
+    def grad(self, shift=None, order=None, method='FD'):
+        """
+        Gradient of the input Function.
+
+        Parameters
+        ----------
+        func : Function or TensorFunction
+            Function to take the gradient of
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
+        """
         from devito.types.tensor import VectorFunction, VectorTimeFunction
         space_dims = [d for d in self.dimensions if d.is_Space]
         shift_x0 = make_shift_x0(shift, (len(space_dims),))
-        comps = [getattr(self, 'd%s' % d.name)(x0=shift_x0(shift, d, None, i))
+        order = order or self.space_order
+        comps = [getattr(self, 'd%s' % d.name)(x0=shift_x0(shift, d, None, i),
+                                               fd_order=order, method=method)
                  for i, d in enumerate(space_dims)]
         vec_func = VectorTimeFunction if self.is_TimeDependent else VectorFunction
         return vec_func(name='grad_%s' % self.name, time_order=self.time_order,
                         space_order=self.space_order, components=comps, grid=self.grid)
 
     def biharmonic(self, weight=1):
         """
@@ -322,14 +415,18 @@
 
 
 def highest_priority(DiffOp):
     prio = lambda x: getattr(x, '_fd_priority', 0)
     return sorted(DiffOp._args_diff, key=prio, reverse=True)[0]
 
 
+# Abstract symbol representing a symbolic coefficient
+W = sympy.Function('W')
+
+
 class DifferentiableOp(Differentiable):
 
     __sympy_class__ = None
 
     def __new__(cls, *args, **kwargs):
         # Do not re-evaluate if any of the args is an EvalDerivative,
         # since the integrity of these objects must be preserved
@@ -503,15 +600,15 @@
     __sympy_class__ = sympy.Pow
 
 
 class Mod(DifferentiableOp, sympy.Mod):
     __sympy_class__ = sympy.Mod
 
 
-class IndexSum(DifferentiableOp):
+class IndexSum(sympy.Expr, Evaluable):
 
     """
     Represent the summation over a multiindex, that is a collection of
     Dimensions, of an indexed expression.
     """
 
     __rargs__ = ('expr', 'dimensions')
@@ -552,14 +649,17 @@
 
     def __repr__(self):
         return "%s(%s, (%s))" % (self.__class__.__name__, self.expr,
                                  ', '.join(d.name for d in self.dimensions))
 
     __str__ = __repr__
 
+    def _sympystr(self, printer):
+        return str(self)
+
     def _hashable_content(self):
         return super()._hashable_content() + (self.dimensions,)
 
     @property
     def expr(self):
         return self._expr
 
@@ -567,15 +667,15 @@
     def dimensions(self):
         return self._dimensions
 
     def _evaluate(self, **kwargs):
         expr = self.expr._evaluate(**kwargs)
 
         if not kwargs.get('expand', True):
-            return self.func(expr, self.dimensions)
+            return self._rebuild(expr)
 
         values = product(*[list(d.range) for d in self.dimensions])
         terms = []
         for i in values:
             mapper = dict(zip(self.dimensions, i))
             terms.append(expr.xreplace(mapper))
         return sum(terms)
@@ -598,52 +698,81 @@
         weights = kwargs.get('initvalue')
 
         assert len(dimensions) == 1
         d = dimensions[0]
         assert isinstance(d, StencilDimension) and d.symbolic_size == len(weights)
         assert isinstance(weights, (list, tuple, np.ndarray))
 
-        try:
-            self._spacings = set().union(*[i.find(Spacing) for i in weights])
-        except AttributeError:
-            self._spacing = set()
+        # Normalize `weights`
+        from devito.symbolics import pow_to_mul  # noqa, sigh
+        weights = tuple(pow_to_mul(sympy.sympify(i)) for i in weights)
 
-        kwargs['scope'] = 'constant'
+        kwargs['scope'] = kwargs.get('scope', 'stack')
+        kwargs['initvalue'] = weights
 
         super().__init_finalize__(*args, **kwargs)
 
     def __eq__(self, other):
         return (isinstance(other, Weights) and
                 self.name == other.name and
                 self.dimension == other.dimension and
                 self.indices == other.indices and
                 self.weights == other.weights)
 
     __hash__ = sympy.Basic.__hash__
 
     def _hashable_content(self):
-        return (self.name, self.dimension, hash(tuple(self.weights)))
+        return (self.name, self.dimension, str(self.weights), self.scope)
 
     @property
     def dimension(self):
         return self.dimensions[0]
 
-    @property
-    def spacings(self):
-        return self._spacings
-
     weights = Array.initvalue
 
+    def _xreplace(self, rule):
+        if self in rule:
+            return rule[self], True
+        elif not rule:
+            return self, False
+        else:
+            try:
+                weights, flags = zip(*[i._xreplace(rule) for i in self.weights])
+                if any(flags):
+                    return self.func(initvalue=weights, function=None), True
+            except AttributeError:
+                # `float` weights
+                pass
+            return super()._xreplace(rule)
+
+    @cached_property
+    def _npweights(self):
+        # NOTE: `self.weights` cannot just be an array or SymPy will fail
+        # internally at `__eq__` since numpy arrays requite .all, not ==,
+        # for equality comparison
+        return np.array(self.weights)
+
+    def value(self, idx):
+        try:
+            v = self.weights[idx]
+        except TypeError:
+            # E.g., `idx` is a tuple
+            v = self._npweights[idx]
+        if v.is_Number or v.is_Indexed:
+            return sympy.sympify(v)
+        else:
+            return self[idx]
+
 
 class IndexDerivative(IndexSum):
 
     __rargs__ = ('expr', 'mapper')
 
     def __new__(cls, expr, mapper, **kwargs):
-        dimensions = as_tuple(mapper.values())
+        dimensions = as_tuple(set(mapper.values()))
 
         # Detect the Weights among the arguments
         weightss = []
         for a in expr.args:
             try:
                 f = a.function
             except AttributeError:
@@ -661,14 +790,28 @@
         obj._mapper = frozendict(mapper)
 
         return obj
 
     def _hashable_content(self):
         return super()._hashable_content() + (self.mapper,)
 
+    def compare(self, other):
+        if self is other:
+            return 0
+        n1 = self.__class__
+        n2 = other.__class__
+        if n1.__name__ == n2.__name__:
+            return self.base.compare(other.base)
+        else:
+            return super().compare(other)
+
+    @cached_property
+    def base(self):
+        return self.expr.func(*[a for a in self.expr.args if a is not self.weights])
+
     @property
     def weights(self):
         return self._weights
 
     @property
     def mapper(self):
         return self._mapper
@@ -686,15 +829,24 @@
 
         w = self.weights
         f = w.function
         d = w.dimension
         mapper = {w.subs(d, i): f.weights[n] for n, i in enumerate(d.range)}
         expr = expr.xreplace(mapper)
 
-        return expr
+        return EvalDerivative(*expr.args, base=self.base)
+
+
+class DiffDerivative(IndexDerivative, DifferentiableOp):
+    pass
+
+
+# SymPy args ordering is the same for Derivatives and IndexDerivatives
+for i in ('DiffDerivative', 'IndexDerivative'):
+    ordering_of_classes.insert(ordering_of_classes.index('Derivative') + 1, i)
 
 
 class EvalDerivative(DifferentiableOp, sympy.Add):
 
     is_commutative = True
 
     __rkwargs__ = ('base',)
@@ -724,17 +876,14 @@
 
     func = DifferentiableOp._rebuild
 
     def _new_rawargs(self, *args, **kwargs):
         kwargs.pop('is_commutative', None)
         return self.func(*args, **kwargs)
 
-    def _coeff_symbol(self, *args, **kwargs):
-        return self.base._coeff_symbol(*args, **kwargs)
-
 
 class diffify(object):
 
     """
     Helper class based on single dispatch to reconstruct all nodes in a sympy
     tree such they are all of type Differentiable.
 
@@ -801,14 +950,20 @@
     def _diff2sympy(obj):
         flag = False
         args = []
         for a in obj.args:
             ax, af = _diff2sympy(a)
             args.append(ax)
             flag |= af
+
+        # Handle special objects
+        if isinstance(obj, DiffDerivative):
+            return IndexDerivative(*args, obj.mapper), True
+
+        # Handle generic objects such as arithmetic operations
         try:
             return obj.__sympy_class__(*args, evaluate=False), True
         except AttributeError:
             # Not of type DifferentiableOp
             pass
         except TypeError:
             # Won't lower (e.g., EvalDerivative)
```

### Comparing `devito-4.8.3/devito/finite_differences/elementary.py` & `devito-4.8.4/devito/finite_differences/elementary.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/finite_differences/finite_difference.py` & `devito-4.8.4/devito/finite_differences/finite_difference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from sympy import sympify
 
-from .differentiable import EvalDerivative, IndexDerivative, Weights
-from .tools import (numeric_weights, symbolic_weights, left, right,
-                    generate_indices, centered, direct, transpose,
-                    check_input, check_symbolic)
+from .differentiable import EvalDerivative, DiffDerivative, Weights
+from .tools import (left, right, generate_indices, centered, direct, transpose,
+                    check_input, check_symbolic, fd_weights_registry)
 
 __all__ = ['first_derivative', 'cross_derivative', 'generic_derivative',
            'left', 'right', 'centered', 'transpose', 'generate_indices']
 
 # Number of digits for FD coefficients to avoid roundup errors and non-deterministic
 # code generation
 _PRECISION = 9
 
 
 @check_input
 @check_symbolic
 def first_derivative(expr, dim, fd_order=None, side=centered, matvec=direct, x0=None,
-                     symbolic=False, expand=True):
+                     coefficients='taylor', expand=True):
     """
     First-order derivative of a given expression.
 
     Parameters
     ----------
     expr : expr-like
         Expression for which the first-order derivative is produced.
     dim : Dimension
         The Dimension w.r.t. which to differentiate.
-    fd_order : int, optional
+    fd_order : int, optional, default=expr.space_order
         Coefficient discretization order. Note: this impacts the width of
-        the resulting stencil. Defaults to `expr.space_order`.
-    side : Side, optional
+        the resulting stencil.
+    side : Side, optional, default=centered
         Side of the finite difference location, centered (at x), left (at x - 1)
-        or right (at x +1). Defaults to `centered`.
-    matvec : Transpose, optional
+        or right (at x +1).
+    matvec : Transpose, optional, default=direct
         Forward (matvec=direct) or transpose (matvec=transpose) mode of the
-        finite difference. Defaults to `direct`.
-    x0 : dict, optional
+        finite difference.
+    x0 : dict, optional, default=None
         Origin of the finite-difference scheme as a map dim: origin_dim.
-    symbolic : bool, optional
-        Use default or custom coefficients (weights). Defaults to False.
-    expand : bool, optional
+    coefficients : string, optional, default='taylor'
+        Use taylor or custom coefficients (weights).
+    expand : bool, optional, default=True
         If True, the derivative is fully expanded as a sum of products,
-        otherwise an IndexSum is returned. Defaults to True.
+        otherwise an IndexSum is returned.
 
     Returns
     -------
     expr-like
         First-order derivative of ``expr``.
 
     Examples
@@ -84,45 +83,50 @@
 
     >>> first_derivative(f, dim=x, x0={x: 1})
     -f(1, y)/h_x + f(h_x + 1, y)/h_x
     """
     fd_order = fd_order or expr.space_order
     deriv_order = 1
 
+    # Enforce stable time coefficients
+    if dim.is_Time and coefficients != 'symbolic':
+        coefficients = 'taylor'
+
     return make_derivative(expr, dim, fd_order, deriv_order, side,
-                           matvec, x0, symbolic, expand)
+                           matvec, x0, coefficients, expand)
 
 
 @check_input
 @check_symbolic
 def cross_derivative(expr, dims, fd_order, deriv_order, x0=None, **kwargs):
     """
     Arbitrary-order cross derivative of a given expression.
 
     Parameters
     ----------
     expr : expr-like
         Expression for which the cross derivative is produced.
     dims : tuple of Dimension
         Dimensions w.r.t. which to differentiate.
-    fd_order : tuple of ints
+    fd_order : int, optional, default=expr.space_order
         Coefficient discretization order. Note: this impacts the width of
         the resulting stencil.
-    deriv_order : tuple of ints
-        Derivative order, e.g. 2 for a second-order derivative.
-    matvec : Transpose, optional
+    side : Side, optional, default=centered
+        Side of the finite difference location, centered (at x), left (at x - 1)
+        or right (at x +1).
+    matvec : Transpose, optional, default=direct
         Forward (matvec=direct) or transpose (matvec=transpose) mode of the
-        finite difference. Defaults to `direct`.
-    x0 : dict, optional
+        finite difference.
+    x0 : dict, optional, default=None
         Origin of the finite-difference scheme as a map dim: origin_dim.
-    symbolic : bool, optional
-        Use default or custom coefficients (weights). Defaults to False.
-    expand : bool, optional
+    coefficients : string, optional, default='taylor'
+        Use taylor or custom coefficients (weights).
+    expand : bool, optional, default=True
         If True, the derivative is fully expanded as a sum of products,
-        otherwise an IndexSum is returned. Defaults to True.
+        otherwise an IndexSum is returned.
 
     Returns
     -------
     expr-like
         Cross-derivative of ``expr``.
 
     Examples
@@ -162,90 +166,99 @@
 
     return expr
 
 
 @check_input
 @check_symbolic
 def generic_derivative(expr, dim, fd_order, deriv_order, matvec=direct, x0=None,
-                       symbolic=False, expand=True):
+                       coefficients='taylor', expand=True):
     """
     Arbitrary-order derivative of a given expression.
 
     Parameters
     ----------
     expr : expr-like
         Expression for which the derivative is produced.
     dim : Dimension
         The Dimension w.r.t. which to differentiate.
-    fd_order : int
+    fd_order : int, optional, default=expr.space_order
         Coefficient discretization order. Note: this impacts the width of
         the resulting stencil.
-    deriv_order : int
-        Derivative order, e.g. 2 for a second-order derivative.
-    matvec : Transpose, optional
+    side : Side, optional, default=centered
+        Side of the finite difference location, centered (at x), left (at x - 1)
+        or right (at x +1).
+    matvec : Transpose, optional, default=direct
         Forward (matvec=direct) or transpose (matvec=transpose) mode of the
-        finite difference. Defaults to `direct`.
-    x0 : dict, optional
+        finite difference.
+    x0 : dict, optional, default=None
         Origin of the finite-difference scheme as a map dim: origin_dim.
-    symbolic : bool, optional
-        Use default or custom coefficients (weights). Defaults to False.
-    expand : bool, optional
+    coefficients : string, optional, default='taylor'
+        Use taylor or custom coefficients (weights).
+    expand : bool, optional, default=True
         If True, the derivative is fully expanded as a sum of products,
-        otherwise an IndexSum is returned. Defaults to True.
+        otherwise an IndexSum is returned.
 
     Returns
     -------
     expr-like
         ``deriv-order`` derivative of ``expr``.
     """
     side = None
-    # First order derivative with 2nd order FD is highly non-recommended so taking
+    # First order derivative with 2nd order FD is strongly discouraged so taking
     # first order fd that is a lot better
-    if deriv_order == 1 and fd_order == 2 and not symbolic:
+    if deriv_order == 1 and fd_order == 2 and coefficients != 'symbolic':
         fd_order = 1
 
+    # Enforce stable time coefficients
+    if dim.is_Time and coefficients != 'symbolic':
+        coefficients = 'taylor'
+
     return make_derivative(expr, dim, fd_order, deriv_order, side,
-                           matvec, x0, symbolic, expand)
+                           matvec, x0, coefficients, expand)
 
 
-def make_derivative(expr, dim, fd_order, deriv_order, side, matvec, x0, symbolic, expand):
+def make_derivative(expr, dim, fd_order, deriv_order, side, matvec, x0, coefficients,
+                    expand):
     # The stencil indices
-    indices, x0 = generate_indices(expr, dim, fd_order, side=side, matvec=matvec, x0=x0)
-
-    # Finite difference weights from Taylor approximation given these positions
-    if symbolic:
-        weights = symbolic_weights(expr, deriv_order, indices, x0)
-    else:
-        weights = numeric_weights(deriv_order, indices, x0)
+    indices, x0 = generate_indices(expr, dim, fd_order, side=side, matvec=matvec,
+                                   x0=x0)
+    # Finite difference weights corresponding to the indices. Computed via the
+    # `coefficients` method (`taylor` or `symbolic`)
+    weights = fd_weights_registry[coefficients](expr, deriv_order, indices, x0)
 
     # Enforce fixed precision FD coefficients to avoid variations in results
     weights = [sympify(w).evalf(_PRECISION) for w in weights]
 
     # Transpose the FD, if necessary
-    if matvec:
-        indices = indices.scale(matvec.val)
+    if matvec == transpose:
+        weights = weights[::-1]
+        indices = indices.transpose()
 
     # Shift index due to staggering, if any
     indices = indices.shift(-(expr.indices_ref[dim] - dim))
 
+    # The user may wish to restrict expansion to selected derivatives
+    if callable(expand):
+        expand = expand(dim)
+
     if not expand and indices.expr is not None:
         weights = Weights(name='w', dimensions=indices.free_dim, initvalue=weights)
 
         # Inject the StencilDimension
         # E.g. `x + i*h_x` into `f(x)` s.t. `f(x + i*h_x)`
         expr = expr._subs(dim, indices.expr)
 
         # Re-evaluate any off-the-grid Functions potentially impacted by the FD
         try:
             expr = expr._evaluate(expand=False)
         except AttributeError:
             # Pure number
             pass
 
-        deriv = IndexDerivative(expr*weights, {dim: indices.free_dim})
+        deriv = DiffDerivative(expr*weights, {dim: indices.free_dim})
     else:
         terms = []
         for i, c in zip(indices, weights):
             # The FD term
             term = expr._subs(dim, i) * c
 
             # Re-evaluate any off-the-grid Functions potentially impacted by the FD
```

### Comparing `devito-4.8.3/devito/finite_differences/tools.py` & `devito-4.8.4/devito/finite_differences/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,15 +60,17 @@
     def wrapper(expr, *args, **kwargs):
         if expr._uses_symbolic_coefficients:
             expr_dict = expr.as_coefficients_dict()
             if any(v > 1 for k, v in expr_dict.items()):
                 raise NotImplementedError("Applying the chain rule to functions "
                                           "with symbolic coefficients is not currently "
                                           "supported")
-        kwargs['symbolic'] = expr._uses_symbolic_coefficients
+            kwargs['coefficients'] = 'symbolic'
+        else:
+            kwargs['coefficients'] = expr.coefficients
         return func(expr, *args, **kwargs)
     return wrapper
 
 
 def dim_with_order(dims, orders):
     """
     Create all possible derivative order for each dims
@@ -133,14 +135,23 @@
         derivatives[name_fd] = (deriv, desciption)
         # Right
         deriv = partial(diff_f, deriv_order=1, dims=d, fd_order=o, side=right)
         name_fd = 'd%sr' % name
         desciption = 'right first order derivative w.r.t dimension %s' % d.name
         derivatives[name_fd] = (deriv, desciption)
 
+    # Add RSFD for first order derivatives
+    for d, o in zip(dims, orders):
+        if not d.is_Time:
+            name = d.root.name
+            deriv = partial(diff_f, deriv_order=1, dims=d, fd_order=o, method='RSFD')
+            name_fd = 'd%s45' % name
+            desciption = 'Derivative w.r.t %s with rotated 45 degree FD' % d.name
+            derivatives[name_fd] = (deriv, desciption)
+
     return derivatives
 
 
 class IndexSet(tuple):
 
     """
     The points of a finite-difference expansion.
@@ -171,35 +182,41 @@
     def __repr__(self):
         return "IndexSet(%s)" % ", ".join(str(i) for i in self)
 
     @property
     def spacing(self):
         return self.dim.spacing
 
-    def scale(self, v):
+    def transpose(self):
         """
-        Construct a new IndexSet with all indices scaled by `v`.
+        Transpose the IndexSet.
         """
-        mapper = {self.spacing: v*self.spacing}
+        mapper = {self.spacing: -self.spacing}
 
         indices = []
-        for i in self:
+        for i in reversed(self):
             try:
                 iloc = i.xreplace(mapper)
             except AttributeError:
                 # Pure number -> sympify
                 iloc = sympify(i).xreplace(mapper)
             indices.append(iloc)
 
         try:
+            free_dim = self.free_dim.transpose()
+            mapper.update({self.free_dim: -free_dim})
+        except AttributeError:
+            free_dim = self.free_dim
+
+        try:
             expr = self.expr.xreplace(mapper)
         except AttributeError:
             expr = None
 
-        return IndexSet(self.dim, indices, expr=expr, fd=self.free_dim)
+        return IndexSet(self.dim, indices, expr=expr, fd=free_dim)
 
     def shift(self, v):
         """
         Construct a new IndexSet with all indices shifted by `v`.
         """
         indices = [i + v for i in self]
 
@@ -215,24 +232,29 @@
     """
     Create a StencilDimension for `expr` with unique name.
     """
     n = len(expr.find(StencilDimension))
     return StencilDimension(name='i%d' % n, _min=_min, _max=_max)
 
 
-def symbolic_weights(function, deriv_order, indices, dim):
-    return [function._coeff_symbol(indices[j], deriv_order, function, dim)
+def symbolic_weights(function, deriv_order, indices, x0):
+    return [function._coeff_symbol(indices[j], deriv_order, function, x0)
             for j in range(0, len(indices))]
 
 
 @cacheit
-def numeric_weights(deriv_order, indices, x0):
+def numeric_weights(function, deriv_order, indices, x0):
     return finite_diff_weights(deriv_order, indices, x0)[-1][-1]
 
 
+fd_weights_registry = {'taylor': numeric_weights, 'standard': numeric_weights,
+                       'symbolic': symbolic_weights}
+coeff_priority = {'taylor': 1, 'standard': 1, 'symbolic': 0}
+
+
 def generate_indices(expr, dim, order, side=None, matvec=None, x0=None):
     """
     Indices for the finite-difference scheme.
 
     Parameters
     ----------
     expr : expr-like
@@ -249,15 +271,15 @@
     x0 : dict of {Dimension: Dimension or Expr or Number}, optional
         Origin of the scheme, ie. `x`, `x + .5 * x.spacing`, ...
 
     Returns
     -------
     An IndexSet, representing an ordered list of indices.
     """
-    if expr.is_Staggered and not dim.is_Time:
+    if expr.is_Staggered and not dim.is_Time and side is None:
         x0, indices = generate_indices_staggered(expr, dim, order, side=side, x0=x0)
     else:
         x0 = (x0 or {dim: dim}).get(dim, dim)
         # Check if called from first_derivative()
         indices = generate_indices_cartesian(expr, dim, order, side, x0)
 
     assert isinstance(indices, IndexSet)
@@ -339,30 +361,43 @@
         ind0 = start
 
     if start != ind0:
         if order < 2:
             indices = [start - diff/2, start + diff/2]
             indices = IndexSet(dim, indices)
         else:
-            o_min = -order//2+1
+            o_min = -order//2 + 1
             o_max = order//2
 
             d = make_stencil_dimension(expr, o_min, o_max)
             iexpr = start - diff/2 + d * diff
             indices = IndexSet(dim, expr=iexpr)
     else:
         if order < 2:
             indices = [start, start - diff]
             indices = IndexSet(dim, indices)
         else:
-            o_min = -order//2
-            o_max = order//2
+            if x0 is None or order % 2 == 0:
+                # No _eval_at or even order derivatives
+                # keep the centered indices
+                o_min = -order//2
+                o_max = order//2
+            elif start is dim:
+                # Staggered FD requires half cell shift
+                # for stability
+                o_min = -order//2 + 1
+                o_max = order//2
+                start = dim + diff/2
+            else:
+                o_min = -order//2
+                o_max = order//2 - 1
+                start = dim
 
             d = make_stencil_dimension(expr, o_min, o_max)
-            iexpr = start + d * diff
+            iexpr = ind0 + d * diff
             indices = IndexSet(dim, expr=iexpr)
 
     return start, indices
 
 
 def make_shift_x0(shift, ndim):
     """
```

### Comparing `devito-4.8.3/devito/ir/clusters/algorithms.py` & `devito-4.8.4/devito/ir/clusters/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,84 @@
 from functools import partial
 from itertools import groupby
 
 import numpy as np
 import sympy
 
 from devito.exceptions import InvalidOperator
-from devito.ir.support import (Any, Backward, Forward, IterationSpace,
+from devito.finite_differences.elementary import Max, Min
+from devito.ir.support import (Any, Backward, Forward, IterationSpace, erange,
                                pull_dims)
+from devito.ir.equations import OpMin, OpMax
 from devito.ir.clusters.analysis import analyze
 from devito.ir.clusters.cluster import Cluster, ClusterGroup
 from devito.ir.clusters.visitors import Queue, QueueStateful, cluster_pass
 from devito.mpi.halo_scheme import HaloScheme, HaloTouch
-from devito.symbolics import retrieve_indexed, uxreplace, xreplace_indices
+from devito.symbolics import (limits_mapper, retrieve_indexed, uxreplace,
+                              xreplace_indices)
 from devito.tools import (DefaultOrderedDict, Stamp, as_mapper, flatten,
-                          is_integer, timed_pass)
+                          is_integer, timed_pass, toposort)
 from devito.types import Array, Eq, Symbol
 from devito.types.dimension import BOTTOM, ModuloDimension
 
 __all__ = ['clusterize']
 
 
 def clusterize(exprs, **kwargs):
     """
     Turn a sequence of LoweredEqs into a sequence of Clusters.
     """
     # Initialization
     clusters = [Cluster(e, e.ispace) for e in exprs]
 
     # Setup the IterationSpaces based on data dependence analysis
+    clusters = impose_total_ordering(clusters)
     clusters = Schedule().process(clusters)
 
     # Handle SteppingDimensions
     clusters = Stepper().process(clusters)
 
     # Handle ConditionalDimensions
     clusters = guard(clusters)
 
     # Determine relevant computational properties (e.g., parallelism)
     clusters = analyze(clusters)
 
-    # Input normalization (e.g., SSA)
+    # Input normalization
     clusters = normalize(clusters, **kwargs)
 
     # Derive the necessary communications for distributed-memory parallelism
     clusters = Communications().process(clusters)
 
     return ClusterGroup(clusters)
 
 
+def impose_total_ordering(clusters):
+    """
+    Create a new sequence of Clusters whose IterationSpaces are totally ordered
+    according to a global set of relations.
+    """
+    global_relations = set().union(*[c.ispace.relations for c in clusters])
+    ordering = toposort(global_relations)
+
+    processed = []
+    for c in clusters:
+        key = lambda d: ordering.index(d)
+        try:
+            relations = {tuple(sorted(c.ispace.itdims, key=key))}
+        except ValueError:
+            # See issue #2204
+            relations = c.ispace.relations
+        ispace = c.ispace.reorder(relations=relations, mode='total')
+
+        processed.append(c.rebuild(ispace=ispace))
+
+    return processed
+
+
 class Schedule(QueueStateful):
 
     """
     This special Queue produces a new sequence of "scheduled" Clusters, which
     means that:
 
         * The iteration direction along each Dimension of each Cluster is such
@@ -117,18 +144,20 @@
         # in any Dimension. We exploit this observation so that we only compute
         # `d_flow`, which instead may be expensive, when strictly necessary
         maybe_break = scope.d_anti.cause & candidates
         if len(clusters) > 1 and maybe_break:
             require_break = scope.d_flow.cause & maybe_break
             if require_break:
                 backlog = [clusters[-1]] + backlog
-                # Try with increasingly smaller ClusterGroups until the ambiguity is gone
+                # Try with increasingly smaller ClusterGroups until the
+                # ambiguity is gone
                 return self.callback(clusters[:-1], prefix, backlog, require_break)
 
-        # Schedule Clusters over different IterationSpaces if this increases parallelism
+        # Schedule Clusters over different IterationSpaces if this increases
+        # parallelism
         for i in range(1, len(clusters)):
             if self._break_for_parallelism(scope, candidates, i):
                 return self.callback(clusters[:i], prefix, clusters[i:] + backlog,
                                      candidates | known_break)
 
         # Compute iteration direction
         idir = {d: Backward for d in candidates if d.root in scope.d_anti.cause}
@@ -142,16 +171,16 @@
             ispace = IterationSpace(c.ispace.intervals, c.ispace.sub_iterators,
                                     {**c.ispace.directions, **idir})
             processed.append(c.rebuild(ispace=ispace))
 
         if not backlog:
             return processed
 
-        # Handle the backlog -- the Clusters characterized by flow- and anti-dependences
-        # along one or more Dimensions
+        # Handle the backlog -- the Clusters characterized by flow- and
+        # anti-dependences along one or more Dimensions
         idir = {d: Any for d in known_break}
         stamp = Stamp()
         for i, c in enumerate(list(backlog)):
             ispace = IterationSpace(c.ispace.intervals.lift(known_break, stamp),
                                     c.ispace.sub_iterators,
                                     {**c.ispace.directions, **idir})
             backlog[i] = c.rebuild(ispace=ispace)
@@ -274,25 +303,30 @@
                     si = sis.pop()
                 else:
                     raise InvalidOperator("Cannot use multiple SteppingDimensions "
                                           "to index into a Function")
                 size = i.function.shape_allocated[d]
                 assert is_integer(size)
 
-                mapper[size][si].add(iaf)
+                # Resolve StencilDimensions in case of unexpanded expressions
+                # E.g. `i0 + t` -> `(t - 1, t, t + 1)`
+                iafs = erange(iaf)
+
+                mapper[size][si].update(iafs)
 
         # Construct the ModuloDimensions
         mds = []
         for size, v in mapper.items():
             for si, iafs in list(v.items()):
                 # Offsets are sorted so that the semantic order (t0, t1, t2) follows
                 # SymPy's index ordering (t, t-1, t+1) afer modulo replacement so
                 # that associativity errors are consistent. This corresponds to
                 # sorting offsets {-1, 0, 1} as {0, -1, 1} assigning -inf to 0
-                siafs = sorted(iafs, key=lambda i: -np.inf if i - si == 0 else (i - si))
+                key = lambda i: -np.inf if i - si == 0 else (i - si)
+                siafs = sorted(iafs, key=key)
 
                 for iaf in siafs:
                     name = '%s%d' % (si.name, len(mds))
                     offset = uxreplace(iaf, {si: d.root})
                     mds.append(ModuloDimension(name, si, offset, size, origin=iaf))
 
         # Replacement rule for ModuloDimensions
@@ -339,75 +373,77 @@
     """
 
     _q_guards_in_key = True
     _q_properties_in_key = True
 
     B = Symbol(name='⊥')
 
-    @timed_pass(name='schedule')
+    @timed_pass(name='communications')
     def process(self, clusters):
         return self._process_fatd(clusters, 1, seen=set())
 
     def callback(self, clusters, prefix, seen=None):
-        if seen.issuperset(clusters):
+        if not prefix:
             return clusters
 
         d = prefix[-1].dim
 
-        # Construct the mock exprs representing the halo accesses
-        exprs = []
+        # Construct a representation of the halo accesses
+        processed = []
         for c in clusters:
-            if c.properties.is_sequential(d):
+            if c.properties.is_sequential(d) or \
+               c in seen:
                 continue
 
-            halo_scheme = HaloScheme(c.exprs, c.ispace)
+            hs = HaloScheme(c.exprs, c.ispace)
+            if hs.is_void or \
+               not d._defines & hs.distributed_aindices:
+                continue
 
-            if not halo_scheme.is_void and \
-               c.properties.is_parallel_relaxed(d):
-                points = set()
-                for f in halo_scheme.fmapper:
-                    for a in c.scope.getreads(f):
-                        points.add(a.access)
-
-                # We also add all written symbols to ultimately create mock WARs
-                # with `c`, which will prevent the newly created HaloTouch to ever
-                # be rescheduled after `c` upon topological sorting
-                points.update(a.access for a in c.scope.accesses if a.is_write)
-
-                # Sort for determinism
-                # NOTE: not sorting might impact code generation. The order of
-                # the args is important because that's what search functions honor!
-                points = sorted(points, key=str)
-
-                rhs = HaloTouch(*points, halo_scheme=halo_scheme)
-
-                # Insert only if not redundant, to avoid useless pollution
-                if not any(rhs == e.rhs for e in exprs):
-                    exprs.append(Eq(self.B, rhs))
+            points = set()
+            for f in hs.fmapper:
+                for a in c.scope.getreads(f):
+                    points.add(a.access)
+
+            # We also add all written symbols to ultimately create mock WARs
+            # with `c`, which will prevent the newly created HaloTouch to ever
+            # be rescheduled after `c` upon topological sorting
+            points.update(a.access for a in c.scope.accesses if a.is_write)
+
+            # Sort for determinism
+            # NOTE: not sorting might impact code generation. The order of
+            # the args is important because that's what search functions honor!
+            points = sorted(points, key=str)
+
+            # Construct the HaloTouch Cluster
+            expr = Eq(self.B, HaloTouch(*points, halo_scheme=hs))
 
-        processed = []
-        if exprs:
-            ispace = prefix[:prefix.index(d)]
-            properties = prefix.properties.drop(d)
+            key = lambda i: i in prefix[:-1] or i in hs.loc_indices
+            ispace = c.ispace.project(key)
 
-            processed.append(Cluster(exprs, ispace, c.guards, properties))
-            seen.update(clusters)
+            halo_touch = c.rebuild(exprs=expr, ispace=ispace)
+
+            processed.append(halo_touch)
+            seen.update({halo_touch, c})
 
         processed.extend(clusters)
 
         return processed
 
 
 def normalize(clusters, **kwargs):
     options = kwargs['options']
     sregistry = kwargs['sregistry']
 
     clusters = normalize_nested_indexeds(clusters, sregistry)
-    clusters = normalize_reductions_dense(clusters, sregistry, options)
-    clusters = normalize_reductions_sparse(clusters, sregistry, options)
+    if options['mapify-reduce']:
+        clusters = normalize_reductions_dense(clusters, sregistry)
+    else:
+        clusters = normalize_reductions_minmax(clusters)
+    clusters = normalize_reductions_sparse(clusters, sregistry)
 
     return clusters
 
 
 @cluster_pass(mode='all')
 def normalize_nested_indexeds(cluster, sregistry):
     """
@@ -442,49 +478,104 @@
             e = e.xreplace({k: v})
         processed.append(e)
 
     return cluster.rebuild(processed)
 
 
 @cluster_pass(mode='dense')
-def normalize_reductions_dense(cluster, sregistry, options):
+def normalize_reductions_minmax(cluster):
+    """
+    Initialize the reduction variables to their neutral element and use them
+    to compute the reduction.
+    """
+    dims = [d for d in cluster.ispace.itdims
+            if cluster.properties.is_parallel_atomic(d)]
+    if not dims:
+        return cluster
+
+    init = []
+    processed = []
+    for e in cluster.exprs:
+        lhs, rhs = e.args
+        f = lhs.function
+
+        if e.operation is OpMin:
+            if not f.is_Input:
+                expr = Eq(lhs, limits_mapper[lhs.dtype].max)
+                ispace = cluster.ispace.project(lambda i: i not in dims)
+                init.append(cluster.rebuild(exprs=expr, ispace=ispace))
+
+            processed.append(e.func(lhs, Min(lhs, rhs)))
+
+        elif e.operation is OpMax:
+            if not f.is_Input:
+                expr = Eq(lhs, limits_mapper[lhs.dtype].min)
+                ispce = cluster.ispace.project(lambda i: i not in dims)
+                init.append(cluster.rebuild(exprs=expr, ispace=ispce))
+
+            processed.append(e.func(lhs, Max(lhs, rhs)))
+
+        else:
+            processed.append(e)
+
+    return init + [cluster.rebuild(processed)]
+
+
+def normalize_reductions_dense(cluster, sregistry):
     """
     Extract the right-hand sides of reduction Eq's in to temporaries.
     """
-    opt_mapify_reduce = options['mapify-reduce']
+    return _normalize_reductions_dense(cluster, sregistry, {})
 
-    dims = [d for d in cluster.properties.dimensions
-            if cluster.properties.is_parallel_atomic(d)]
 
+@cluster_pass(mode='dense')
+def _normalize_reductions_dense(cluster, sregistry, mapper):
+    dims = [d for d in cluster.ispace.itdims
+            if cluster.properties.is_parallel_atomic(d)]
     if not dims:
         return cluster
 
     processed = []
     for e in cluster.exprs:
-        if e.is_Reduction and e.lhs.is_Symbol and opt_mapify_reduce:
+        if e.is_Reduction:
             # Transform `e` into what is in essence an explicit map-reduce
             # For example, turn:
             # `s += f(u[x], v[x], ...)`
             # into
             # `r[x] = f(u[x], v[x], ...)`
             # `s += r[x]`
             # This makes it much easier to parallelize the map part regardless
             # of the target backend
-            name = sregistry.make_name()
-            a = Array(name=name, dtype=e.dtype, dimensions=dims)
-            processed.extend([Eq(a.indexify(), e.rhs),
-                              e.func(e.lhs, a.indexify())])
+            lhs, rhs = e.args
+
+            if lhs.function.is_Array:
+                # Probably a compiler-generated reduction, e.g. via
+                # recursive compilation; it's an Array already, so nothing to do
+                processed.append(e)
+            elif rhs in mapper:
+                # Seen this RHS already, so reuse the Array that was created for it
+                processed.append(e.func(lhs, mapper[rhs].indexify()))
+            else:
+                # Here the LHS could be a Symbol or a user-level Function
+                # In the latter case we copy the data into a temporary Array
+                # because the Function might be padded, and reduction operations
+                # require, in general, the data values to be contiguous
+                name = sregistry.make_name()
+                a = mapper[rhs] = Array(name=name, dtype=e.dtype, dimensions=dims)
+
+                processed.extend([Eq(a.indexify(), rhs),
+                                  e.func(lhs, a.indexify())])
         else:
             processed.append(e)
 
     return cluster.rebuild(processed)
 
 
 @cluster_pass(mode='sparse')
-def normalize_reductions_sparse(cluster, sregistry, options):
+def normalize_reductions_sparse(cluster, sregistry):
     """
     Extract the right-hand sides of reduction Eq's in to temporaries.
     """
     processed = []
     for e in cluster.exprs:
         if e.is_Reduction and e.lhs.is_Indexed:
             # Transform `e` such that we reduce into a scalar (ultimately via
```

### Comparing `devito-4.8.3/devito/ir/clusters/cluster.py` & `devito-4.8.4/devito/ir/clusters/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 import numpy as np
 from cached_property import cached_property
 
 from devito.ir.equations import ClusterizedEq
 from devito.ir.support import (PARALLEL, PARALLEL_IF_PVT, BaseGuardBoundNext,
                                Forward, Interval, IntervalGroup, IterationSpace,
-                               DataSpace, Guards, Properties, Scope, detect_accesses,
-                               detect_io, normalize_properties, normalize_syncs,
-                               sdims_min, sdims_max)
+                               DataSpace, Guards, Properties, Scope, WithLock,
+                               PrefetchUpdate, detect_accesses, detect_io,
+                               normalize_properties, normalize_syncs, minimum,
+                               maximum, null_ispace)
 from devito.mpi.halo_scheme import HaloScheme, HaloTouch
 from devito.symbolics import estimate_cost
 from devito.tools import as_tuple, flatten, frozendict, infer_dtype
+from devito.types import WeakFence, CriticalRegion
 
 __all__ = ["Cluster", "ClusterGroup"]
 
 
 class Cluster(object):
 
     """
@@ -37,32 +39,24 @@
         Mapper from Dimensions to lists of SyncOps, that is ordered sequences of
         synchronization operations that must be performed in order to compute the
         Cluster asynchronously.
     halo_scheme : HaloScheme, optional
         The halo exchanges required by the Cluster.
     """
 
-    def __init__(self, exprs, ispace=None, guards=None, properties=None, syncs=None,
-                 halo_scheme=None):
-        ispace = ispace or IterationSpace([])
-
+    def __init__(self, exprs, ispace=null_ispace, guards=None, properties=None,
+                 syncs=None, halo_scheme=None):
         self._exprs = tuple(ClusterizedEq(e, ispace=ispace) for e in as_tuple(exprs))
         self._ispace = ispace
         self._guards = Guards(guards or {})
         self._syncs = frozendict(syncs or {})
 
         # Normalize properties
         properties = Properties(properties or {})
-        for d in ispace.itdimensions:
-            properties = properties.add(d)
-        for i in properties:
-            for d in as_tuple(i):
-                if d not in ispace.itdimensions:
-                    properties = properties.drop(d)
-        self._properties = properties
+        self._properties = tailor_properties(properties, ispace)
 
         self._halo_scheme = halo_scheme
 
     def __repr__(self):
         return "Cluster([%s])" % ('\n' + ' '*9).join('%s' % i for i in self.exprs)
 
     @classmethod
@@ -81,18 +75,15 @@
                              "non-homogeneous guards")
 
         exprs = chain(*[c.exprs for c in clusters])
         ispace = IterationSpace.union(*[c.ispace for c in clusters])
 
         guards = root.guards
 
-        properties = {}
-        for c in clusters:
-            for d, v in c.properties.items():
-                properties[d] = normalize_properties(properties.get(d, v), v)
+        properties = reduce_properties(clusters)
 
         try:
             syncs = normalize_syncs(*[c.syncs for c in clusters])
         except ValueError:
             raise ValueError("Cannot build a Cluster from Clusters with "
                              "non-compatible synchronization operations")
 
@@ -184,66 +175,92 @@
         return self.scope.functions
 
     @cached_property
     def has_increments(self):
         return any(e.is_Increment for e in self.exprs)
 
     @cached_property
-    def is_scalar(self):
-        return not any(f.is_Function for f in self.scope.writes)
-
-    @cached_property
     def grid(self):
         grids = set(f.grid for f in self.functions if f.is_DiscreteFunction) - {None}
         if len(grids) == 1:
             return grids.pop()
         else:
             raise ValueError("Cluster has no unique Grid")
 
     @cached_property
+    def is_scalar(self):
+        return not any(f.is_Function for f in self.scope.writes)
+
+    @cached_property
     def is_dense(self):
         """
-        A Cluster is dense if at least one of the following conditions is True:
+        True if at least one of the following conditions are True:
 
             * It is defined over a unique Grid and all of the Grid Dimensions
               are PARALLEL.
             * Only DiscreteFunctions are written and only affine index functions
               are used (e.g., `a[x+1, y-2]` is OK, while `a[b[x], y-2]` is not)
+
+        False in all other cases.
         """
         # Hopefully it's got a unique Grid and all Dimensions are PARALLEL (or
         # at most PARALLEL_IF_PVT). This is a quick and easy check so we try it first
         try:
             pset = {PARALLEL, PARALLEL_IF_PVT}
-            grid = self.grid
-            for d in grid.dimensions:
-                if not any(pset & v for k, v in self.properties.items()
-                           if d in k._defines):
-                    raise ValueError
-            return True
+            target = set(self.grid.dimensions)
+            dims = {d for d in self.properties if d._defines & target}
+            if any(pset & self.properties[d] for d in dims):
+                return True
         except ValueError:
             pass
 
         # Fallback to legacy is_dense checks
         return (not any(e.conditionals for e in self.exprs) and
                 not any(f.is_SparseFunction for f in self.functions) and
-                not self.is_halo_touch and
+                not self.is_wild and
                 all(a.is_regular for a in self.scope.accesses))
 
     @cached_property
     def is_sparse(self):
         """
-        A Cluster is sparse if it represents a sparse operation, i.e iff
-        There's at least one irregular access.
+        True if it represents a sparse operation, i.e iff there's at least
+        one irregular access, False otherwise.
         """
         return any(a.is_irregular for a in self.scope.accesses)
 
     @property
+    def is_wild(self):
+        """
+        True if encoding a non-mathematical operation, False otherwise.
+        """
+        return self.is_halo_touch or self.is_fence
+
+    @property
     def is_halo_touch(self):
-        return (len(self.exprs) > 0 and
-                all(isinstance(e.rhs, HaloTouch) for e in self.exprs))
+        return self.exprs and all(isinstance(e.rhs, HaloTouch) for e in self.exprs)
+
+    @property
+    def is_fence(self):
+        return self.is_weak_fence or self.is_critical_region
+
+    @property
+    def is_weak_fence(self):
+        return self.exprs and all(isinstance(e.rhs, WeakFence) for e in self.exprs)
+
+    @property
+    def is_critical_region(self):
+        return self.exprs and all(isinstance(e.rhs, CriticalRegion) for e in self.exprs)
+
+    @property
+    def is_async(self):
+        """
+        True if an asynchronous Cluster, False otherwise.
+        """
+        return any(isinstance(s, (WithLock, PrefetchUpdate))
+                   for s in flatten(self.syncs.values()))
 
     @cached_property
     def dtype(self):
         """
         The arithmetic data type of the Cluster.
 
         If the Cluster performs floating point arithmetic, then the expressions
@@ -276,17 +293,17 @@
         # space for each Function appearing in `self.exprs`
         parts = {}
         for f, v in accesses.items():
             if f is None:
                 continue
 
             intervals = [Interval(d,
-                                  min([sdims_min(i) for i in offs]),
-                                  max([sdims_max(i) for i in offs]))
-                         for d, offs in v.items()]
+                                  min([minimum(i, ispace=self.ispace) for i in o]),
+                                  max([maximum(i, ispace=self.ispace) for i in o]))
+                         for d, o in v.items()]
             intervals = IntervalGroup(intervals)
 
             # Factor in the IterationSpace -- if the min/max points aren't zero,
             # then the data intervals need to shrink/expand accordingly
             intervals = intervals.promote(lambda d: d.is_Block)
             shift = self.ispace.intervals.promote(lambda d: d.is_Block)
             intervals = intervals.add(shift)
@@ -308,15 +325,16 @@
                     intervals = intervals.translate(d, 1)
             for d in self.properties:
                 if self.properties.is_inbound(d):
                     intervals = intervals.zero(d._defines)
 
             # Special case: if the factor of a ConditionalDimension has value 1,
             # then we can safely resort to the parent's Interval
-            intervals = intervals.promote(lambda d: d.is_Conditional and d.factor == 1)
+            key = lambda d: d.is_Conditional and d.condition is None and d.factor == 1
+            intervals = intervals.promote(key)
 
             parts[f] = intervals
 
         # Determine the Dimensions requiring shifted min/max points to avoid
         # OOB accesses
         oobs = set()
         for f, v in parts.items():
@@ -335,14 +353,15 @@
                     # Unable to detect presence of OOB accesses (e.g., `d` not in
                     # `f._size_halo`, that is typical of indirect accesses `A[B[i]]`)
                     pass
 
         # Construct the `intervals` of the DataSpace, that is a global,
         # Dimension-centric view of the data space
         intervals = IntervalGroup.generate('union', *parts.values())
+
         # E.g., `db0 -> time`, but `xi NOT-> x`
         intervals = intervals.promote(lambda d: not d.is_Sub)
         intervals = intervals.zero(set(intervals.dimensions) - oobs)
 
         return DataSpace(intervals, parts)
 
     @cached_property
@@ -359,36 +378,42 @@
         Notes
         -----
         If a Function is both read and written, then it is counted twice.
         """
         reads, writes = detect_io(self.exprs, relax=True)
         accesses = [(i, 'r') for i in reads] + [(i, 'w') for i in writes]
 
+        # Ordering isn't important at this point, so returning an unordered
+        # collection makes the caller's life easier
+        uispace = self.ispace.reorder(mode='unordered')
+
         ret = {}
         for i, mode in accesses:
             if not i.is_AbstractFunction:
                 continue
             elif i in self.dspace.parts:
                 # Stencils extend the data spaces beyond the iteration spaces
                 intervals = self.dspace.parts[i]
 
                 # Assume that invariant dimensions always cause new loads/stores
-                invariants = self.ispace.intervals.drop(intervals.dimensions)
+                invariants = uispace.intervals.drop(intervals.dimensions)
+
                 intervals = intervals.generate('union', invariants, intervals)
 
                 # Bundles impact depends on the number of components
                 try:
                     v = len(i.components)
                 except AttributeError:
                     v = 1
 
                 for n in range(v):
                     ret[(i, mode, n)] = intervals
             else:
-                ret[(i, mode, 0)] = self.ispace.intervals
+                ret[(i, mode, 0)] = uispace.intervals
+
         return ret
 
 
 class ClusterGroup(tuple):
 
     """
     An immutable, totally-ordered sequence of Clusters.
@@ -398,15 +423,15 @@
     clusters : tuple of Clusters
         Input elements.
     ispace : IterationSpace, optional
         The IterationSpace section shared by all `clusters`.
     """
 
     def __new__(cls, clusters, ispace=None):
-        obj = super(ClusterGroup, cls).__new__(cls, flatten(as_tuple(clusters)))
+        obj = super().__new__(cls, flatten(as_tuple(clusters)))
         obj._ispace = ispace
         return obj
 
     @classmethod
     def concatenate(cls, *cgroups):
         return list(chain(*cgroups))
 
@@ -419,22 +444,28 @@
         return Scope(exprs=self.exprs)
 
     @cached_property
     def ispace(self):
         return self._ispace
 
     @cached_property
+    def properties(self):
+        return tailor_properties(reduce_properties(self), self.ispace)
+
+    @cached_property
     def guards(self):
         """The guards of each Cluster in self."""
         return tuple(i.guards for i in self)
 
     @cached_property
     def syncs(self):
-        """The synchronization operations of each Cluster in self."""
-        return tuple(i.syncs for i in self)
+        """
+        A view of the ClusterGroup's synchronization operations.
+        """
+        return normalize_syncs(*[c.syncs for c in self])
 
     @cached_property
     def dspace(self):
         """Return the DataSpace of this ClusterGroup."""
         return DataSpace.union(*[i.dspace.reset() for i in self])
 
     @property
@@ -448,20 +479,51 @@
 
         If at least one Cluster performs floating point arithmetic, then the
         Clusters performing integer arithmetic are ignored.
 
         If two Clusters perform calculations with different precision, the
         data type with highest precision is returned.
         """
-        dtypes = {i.dtype for i in self}
+        dtypes = {i.dtype for i in self} - {None}
 
         return infer_dtype(dtypes)
 
     @cached_property
     def meta(self):
         """
         Returns
         -------
         dtype, DSpace
             The data type and the data space of the ClusterGroup.
         """
         return (self.dtype, self.dspace)
+
+
+# *** Utils
+
+def reduce_properties(clusters):
+    """
+    The normalized intersection (basically, a reduction) of the Properties in
+    `clusters`.
+    """
+    properties = {}
+    for c in clusters:
+        for d, v in c.properties.items():
+            properties[d] = normalize_properties(properties.get(d, v), v)
+
+    return Properties(properties)
+
+
+def tailor_properties(properties, ispace):
+    """
+    Create a new Properties object off `properties` that retains all and only
+    the iteration dimensions in `ispace`.
+    """
+    for i in properties:
+        for d in as_tuple(i):
+            if d not in ispace.itdims:
+                properties = properties.drop(d)
+
+    for d in ispace.itdims:
+        properties = properties.add(d)
+
+    return properties
```

### Comparing `devito-4.8.3/devito/ir/clusters/visitors.py` & `devito-4.8.4/devito/ir/clusters/visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 from collections.abc import Iterable
 
 from itertools import groupby
 
-from devito.ir.support import IterationSpace, Scope
+from devito.ir.support import IterationSpace, Scope, null_ispace
 from devito.tools import as_tuple, flatten, timed_pass
 
 __all__ = ['Queue', 'QueueStateful', 'cluster_pass']
 
 
 class Queue(object):
 
@@ -46,15 +46,15 @@
                 # `cluster` is actually a ClusterGroup
                 assert len(cluster.guards) == 1
                 guards = tuple(cluster.guards[0].get(i.dim) for i in ispace)
         else:
             guards = None
 
         if self._q_properties_in_key:
-            properties = cluster.properties.drop(cluster.ispace[level:].itdimensions)
+            properties = cluster.properties.drop(cluster.ispace[level:].itdims)
         else:
             properties = None
 
         if self._q_syncs_in_key:
             try:
                 syncs = tuple(cluster.syncs.get(i.dim) for i in ispace)
             except AttributeError:
@@ -69,20 +69,18 @@
         subkey = self._make_key_hook(cluster, level)
 
         return (prefix,) + subkey
 
     def _make_key_hook(self, cluster, level):
         return ()
 
-    def _process_fdta(self, clusters, level, prefix=None, **kwargs):
+    def _process_fdta(self, clusters, level, prefix=null_ispace, **kwargs):
         """
         fdta -> First Divide Then Apply
         """
-        prefix = prefix or IterationSpace([])
-
         # Divide part
         processed = []
         for k, g in groupby(clusters, key=lambda i: self._make_key(i, level)):
             pfx = k[0]
             if level > len(pfx):
                 # Base case
                 processed.extend(list(g))
@@ -125,15 +123,15 @@
     class State(object):
 
         def __init__(self):
             self.properties = {}
             self.scopes = {}
 
     def __init__(self, state=None):
-        super(QueueStateful, self).__init__()
+        super().__init__()
         self.state = state or QueueStateful.State()
 
     def _fetch_scope(self, clusters):
         exprs = flatten(c.exprs for c in as_tuple(clusters))
         key = tuple(exprs)
         if key not in self.state.scopes:
             self.state.scopes[key] = Scope(exprs)
@@ -196,17 +194,17 @@
                 return cluster_pass(func, mode)
             return wrapper
 
     def __init__(self, func, mode='dense'):
         self.func = func
 
         if mode == 'dense':
-            self.cond = lambda c: c.is_dense or not c.is_sparse
+            self.cond = lambda c: (c.is_dense or not c.is_sparse) and not c.is_wild
         elif mode == 'sparse':
-            self.cond = lambda c: c.is_sparse
+            self.cond = lambda c: c.is_sparse and not c.is_wild
         else:
             self.cond = lambda c: True
 
     def __call__(self, *args):
         if timed_pass.is_enabled():
             maybe_timed = lambda *_args: timed_pass(self.func, self.func.__name__)(*_args)
         else:
```

### Comparing `devito-4.8.3/devito/ir/equations/algorithms.py` & `devito-4.8.4/devito/ir/equations/algorithms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from collections.abc import Iterable
 
-from sympy import sympify
-
 from devito.symbolics import retrieve_indexed, uxreplace, retrieve_dimensions
-from devito.tools import (PartialOrderTuple, as_tuple, flatten,
-                          filter_sorted, filter_ordered)
+from devito.tools import Ordering, as_tuple, flatten, filter_sorted, filter_ordered
 from devito.types import Dimension, IgnoreDimSort
 from devito.types.basic import AbstractFunction
 
 __all__ = ['dimension_sort', 'lower_exprs']
 
 
 def dimension_sort(expr):
@@ -81,52 +78,53 @@
             if d.index.name == d.name:
                 dims.append(d)
             else:
                 dims.extend([d.index, d])
 
         implicit_relations.update({tuple(filter_ordered(dims))})
 
-    ordering = PartialOrderTuple(extra, relations=implicit_relations)
+    ordering = Ordering(extra, relations=implicit_relations, mode='partial')
 
     return ordering
 
 
-def lower_exprs(expressions, **kwargs):
+def lower_exprs(expressions, subs=None, **kwargs):
     """
     Lowering an expression consists of the following passes:
 
         * Indexify functions;
         * Align Indexeds with the computational domain;
         * Apply user-provided substitution;
 
     Examples
     --------
     f(x - 2*h_x, y) -> f[xi + 2, yi + 4]  (assuming halo_size=4)
     """
-    # Normalize subs
-    subs = {k: sympify(v) for k, v in kwargs.get('subs', {}).items()}
+    return _lower_exprs(expressions, subs or {})
+
 
+def _lower_exprs(expressions, subs):
     processed = []
     for expr in as_tuple(expressions):
         try:
             dimension_map = expr.subdomain.dimension_map
         except AttributeError:
             # Some Relationals may be pure SymPy objects, thus lacking the subdomain
             dimension_map = {}
 
         # Handle Functions (typical case)
-        mapper = {f: lower_exprs(f.indexify(subs=dimension_map), **kwargs)
+        mapper = {f: _lower_exprs(f.indexify(subs=dimension_map), subs)
                   for f in expr.find(AbstractFunction)}
 
         # Handle Indexeds (from index notation)
         for i in retrieve_indexed(expr):
             f = i.function
 
             # Introduce shifting to align with the computational domain
-            indices = [(lower_exprs(a) + o) for a, o in
+            indices = [_lower_exprs(a, subs) + o for a, o in
                        zip(i.indices, f._size_nodomain.left)]
 
             # Substitute spacing (spacing only used in own dimension)
             indices = [i.xreplace({d.spacing: 1, -d.spacing: -1})
                        for i, d in zip(indices, f.dimensions)]
 
             # Apply substitutions, if necessary
```

### Comparing `devito-4.8.3/devito/ir/equations/equation.py` & `devito-4.8.4/devito/ir/equations/equation.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def __repr__(self):
         if not self.is_Reduction:
             return super().__repr__()
         elif self.operation is OpInc:
             return '%s += %s' % (self.lhs, self.rhs)
         else:
-            return '%s = %s(%s, %s)' % (self.lhs, self.operation, self.lhs, self.rhs)
+            return '%s = %s(%s)' % (self.lhs, self.operation, self.rhs)
 
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
 class Operation(Tag):
 
@@ -174,16 +174,16 @@
                 # Use `parent`, and `root`, because a ConditionalDimension may
                 # have a SubDimension as parent
                 iterators.setdefault(d.parent, set())
             elif not d.is_Stencil:
                 iterators.setdefault(d, set())
 
         # Construct the IterationSpace
-        intervals = IntervalGroup([Interval(d, 0, 0) for d in iterators],
-                                  relations=ordering.relations)
+        intervals = IntervalGroup([Interval(d) for d in iterators],
+                                  relations=ordering.relations, mode='partial')
         ispace = IterationSpace(intervals, iterators)
 
         # Construct the conditionals and replace the ConditionalDimensions in `expr`
         conditionals = {}
         for d in ordering:
             if not d.is_Conditional:
                 continue
@@ -195,15 +195,15 @@
                 expr = uxreplace(expr, {d: IntDiv(d.index, d.factor)})
         conditionals = frozendict(conditionals)
 
         # Lower all Differentiable operations into SymPy operations
         rhs = diff2sympy(expr.rhs)
 
         # Finally create the LoweredEq with all metadata attached
-        expr = super(LoweredEq, cls).__new__(cls, expr.lhs, rhs, evaluate=False)
+        expr = super().__new__(cls, expr.lhs, rhs, evaluate=False)
 
         expr._ispace = ispace
         expr._conditionals = conditionals
         expr._reads, expr._writes = detect_io(expr)
         expr._implicit_dims = input_expr.implicit_dims
         expr._operation = Operation.detect(input_expr)
```

### Comparing `devito-4.8.3/devito/ir/iet/algorithms.py` & `devito-4.8.4/devito/ir/iet/algorithms.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,18 @@
                              properties=i.properties, uindices=i.sub_iterators)
 
         elif i.is_Section:
             body = Section('section%d' % nsections, body=queues.pop(i))
             nsections += 1
 
         elif i.is_Halo:
-            body = HaloSpot(queues.pop(i), i.halo_scheme)
+            try:
+                body = HaloSpot(queues.pop(i), i.halo_scheme)
+            except KeyError:
+                body = HaloSpot(None, i.halo_scheme)
 
         elif i.is_Sync:
             body = SyncSpot(i.sync_ops, body=queues.pop(i, None))
 
         queues.setdefault(i.parent, []).append(body)
 
     assert False
```

### Comparing `devito-4.8.3/devito/ir/iet/efunc.py` & `devito-4.8.4/devito/ir/iet/efunc.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from devito.ir.iet.nodes import Call, Callable
 from devito.ir.iet.utils import derive_parameters
 from devito.symbolics import uxreplace
 from devito.tools import as_tuple
 
 __all__ = ['ElementalFunction', 'ElementalCall', 'make_efunc', 'make_callable',
            'EntryFunction', 'AsyncCallable', 'AsyncCall', 'ThreadCallable',
-           'DeviceFunction', 'DeviceCall']
+           'DeviceFunction', 'DeviceCall', 'KernelLaunch', 'CommCallable']
 
 
 # ElementalFunction machinery
 
 class ElementalCall(Call):
 
     def __init__(self, name, arguments=None, mapper=None, dynamic_args_mapper=None,
@@ -29,20 +29,20 @@
             if len(self._mapper[k]) != len(tv):
                 raise ValueError("Expected %d values for dynamic parameter `%s`, given %d"
                                  % (len(self._mapper[k]), k, len(tv)))
             # Create the argument list
             for i, j in zip(self._mapper[k], tv):
                 arguments[i] = j if incr is False else (arguments[i] + j)
 
-        super(ElementalCall, self).__init__(name, arguments, retobj, is_indirect)
+        super().__init__(name, arguments, retobj, is_indirect)
 
     def _rebuild(self, *args, dynamic_args_mapper=None, incr=False,
                  retobj=None, **kwargs):
         # This guarantees that `ec._rebuild(arguments=ec.arguments) == ec`
-        return super(ElementalCall, self)._rebuild(
+        return super()._rebuild(
             *args, dynamic_args_mapper=dynamic_args_mapper, incr=incr,
             retobj=retobj, **kwargs
         )
 
     @cached_property
     def dynamic_defaults(self):
         return {k: tuple(self.arguments[i] for i in v) for k, v in self._mapper.items()}
@@ -59,15 +59,15 @@
     """
     _Call_cls = ElementalCall
 
     is_ElementalFunction = True
 
     def __init__(self, name, body, retval='void', parameters=None, prefix=('static',),
                  dynamic_parameters=None):
-        super(ElementalFunction, self).__init__(name, body, retval, parameters, prefix)
+        super().__init__(name, body, retval, parameters, prefix)
 
         self._mapper = {}
         for i in as_tuple(dynamic_parameters):
             if i.is_Dimension:
                 self._mapper[i] = (parameters.index(i.symbolic_min),
                                    parameters.index(i.symbolic_max))
             else:
@@ -101,15 +101,15 @@
 # Callable machinery
 
 
 def make_callable(name, iet, retval='void', prefix='static'):
     """
     Utility function to create a Callable from an IET.
     """
-    parameters = derive_parameters(iet)
+    parameters = derive_parameters(iet, ordering='canonical')
     return Callable(name, iet, retval, parameters=parameters, prefix=prefix)
 
 
 # EntryFunction machinery
 
 class EntryFunction(Callable):
     pass
@@ -133,45 +133,90 @@
 
 class ThreadCallable(Callable):
 
     """
     A Callable executed asynchronously by a thread.
     """
 
-    def __init__(self, name, body, parameters=None, prefix='static'):
-        super().__init__(name, body, 'void*', parameters=parameters, prefix=prefix)
+    def __init__(self, name, body, parameters):
+        super().__init__(name, body, 'void*', parameters=parameters, prefix='static')
+
+        # Sanity checks
+        # By construction, the first unpack statement of a ThreadCallable must
+        # be the PointerCast that makes `sdata` available in the local scope
+        assert len(body.unpacks) > 0
+        v = body.unpacks[0]
+        assert v.is_PointerCast
+        self.sdata = v.function
 
 
 # DeviceFunction machinery
 
 
 class DeviceFunction(Callable):
 
     """
     A Callable executed asynchronously on a device.
     """
 
-    def __init__(self, name, body, retval='void', parameters=None, prefix='__global__'):
-        super().__init__(name, body, retval, parameters=parameters, prefix=prefix)
+    def __init__(self, name, body, retval='void', parameters=None,
+                 prefix='__global__', templates=None):
+        super().__init__(name, body, retval, parameters=parameters, prefix=prefix,
+                         templates=templates)
 
 
 class DeviceCall(Call):
 
     """
-    A call to an external function executed asynchronously on a device.
+    A call to a function executed asynchronously on a device.
     """
 
     def __init__(self, name, arguments=None, **kwargs):
         # Explicitly convert host pointers into device pointers
         processed = []
-        for a in arguments:
+        for a in as_tuple(arguments):
             try:
                 f = a.function
             except AttributeError:
                 processed.append(a)
                 continue
             if f._mem_mapped:
                 processed.append(uxreplace(a, {f.indexed: f.dmap}))
             else:
                 processed.append(a)
 
         super().__init__(name, arguments=processed, **kwargs)
+
+
+class KernelLaunch(DeviceCall):
+
+    """
+    A call to an asynchronous device kernel.
+    """
+
+    def __init__(self, name, grid, block, shm=0, stream=None,
+                 arguments=None, writes=None, templates=None):
+        super().__init__(name, arguments=arguments, writes=writes,
+                         templates=templates)
+
+        # Kernel launch arguments
+        self.grid = grid
+        self.block = block
+        self.shm = shm
+        self.stream = stream
+
+    def __repr__(self):
+        return 'Launch[%s]<<<(%s)>>>' % (self.name,
+                                         ','.join(str(i.name) for i in self.writes))
+
+    @cached_property
+    def functions(self):
+        launch_args = (self.grid, self.block,)
+        if self.stream is not None:
+            launch_args += (self.stream.function,)
+        return super().functions + launch_args
+
+
+# Other relevant Callable subclasses
+
+class CommCallable(Callable):
+    pass
```

### Comparing `devito-4.8.3/devito/ir/iet/nodes.py` & `devito-4.8.4/devito/ir/iet/nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 from devito.symbolics import ListInitializer, CallFromPointer, ccode
 from devito.tools import (Signer, as_tuple, filter_ordered, filter_sorted, flatten,
                           ctypes_to_cstr)
 from devito.types.basic import (AbstractFunction, AbstractSymbol, Basic, Indexed,
                                 Symbol)
 from devito.types.object import AbstractObject, LocalObject
 
-__all__ = ['Node', 'Block', 'Expression', 'Callable', 'Call',
-           'Conditional', 'Iteration', 'List', 'Section', 'TimedList', 'Prodder',
-           'MetaCall', 'PointerCast', 'HaloSpot', 'Definition', 'ExpressionBundle',
-           'AugmentedExpression', 'Increment', 'Return', 'While',
-           'ParallelIteration', 'ParallelBlock', 'Dereference', 'Lambda',
-           'SyncSpot', 'Pragma', 'DummyExpr', 'BlankLine', 'ParallelTree',
-           'BusyWait', 'CallableBody', 'Transfer']
+__all__ = ['Node', 'MultiTraversable', 'Block', 'Expression', 'Callable',
+           'Call', 'ExprStmt', 'Conditional', 'Iteration', 'List', 'Section',
+           'TimedList', 'Prodder', 'MetaCall', 'PointerCast', 'HaloSpot',
+           'Definition', 'ExpressionBundle', 'AugmentedExpression', 'Break',
+           'Increment', 'Return', 'While', 'ListMajor', 'ParallelIteration',
+           'ParallelBlock', 'Dereference', 'Lambda', 'SyncSpot', 'Pragma',
+           'DummyExpr', 'BlankLine', 'ParallelTree', 'BusyWait', 'UsingNamespace',
+           'CallableBody', 'Transfer']
 
 # First-class IET nodes
 
 
 class Node(Signer):
 
     __metaclass__ = abc.ABCMeta
@@ -64,15 +65,15 @@
     _ccode_handler = None
     """
     Customizable by subclasses, in particular Operator subclasses which define
     backend-specific nodes and, as such, require node-specific handlers.
     """
 
     def __new__(cls, *args, **kwargs):
-        obj = super(Node, cls).__new__(cls)
+        obj = super().__new__(cls)
         argnames, _, _, defaultvalues, _, _, _ = inspect.getfullargspec(cls.__init__)
         try:
             defaults = dict(zip(argnames[-len(defaultvalues):], defaultvalues))
         except TypeError:
             # No default kwarg values
             defaults = {}
         obj._args = {k: v for k, v in zip(argnames[1:], args)}
@@ -128,20 +129,20 @@
         return str(self.ccode)
 
     def __repr__(self):
         return self.__class__.__name__
 
     @property
     def functions(self):
-        """All AbstractFunction objects used by this node."""
+        """All AbstractFunctions and AbstractObjects used by this node."""
         return ()
 
     @property
     def expr_symbols(self):
-        """All symbols appearing in an expression within this node."""
+        """All symbols appearing within this node."""
         return ()
 
     @property
     def defines(self):
         """All Basic objects defined by this node."""
         return ()
 
@@ -171,14 +172,23 @@
     -----
     An ExprStmt does *not* have children Nodes.
     """
 
     pass
 
 
+class MultiTraversable(Node):
+
+    """
+    An abstract base class for Nodes comprising more than one traversable children.
+    """
+
+    pass
+
+
 class List(Node):
 
     """A sequence of Nodes."""
 
     is_List = True
 
     _traversable = ['body']
@@ -236,38 +246,51 @@
         code will be `name, arg1, ..., argN` rather than `name(arg1, ..., argN)`.
         Defaults to False.
     cast : bool, optional
         If True, the Call return value is explicitly casted to the `retobj` type.
         Defaults to False.
     writes : list, optional
         The AbstractFunctions that will be written to by the called function.
-        Explicitly tagging these AbstractFunctions is useful in the case of external
-        calls, that is whenever the compiler would be unable to retrieve that
-        information by analysis of the IET graph.
+        Explicitly tagging these AbstractFunctions is useful in the case of
+        external calls, that is whenever the compiler would be unable to
+        retrieve that information by analysis of the IET graph.
+    templates : list of Basic, optional
+        The template arguments of the Call.
     """
 
     is_Call = True
 
     def __init__(self, name, arguments=None, retobj=None, is_indirect=False,
-                 cast=False, writes=None):
+                 cast=False, writes=None, templates=None):
         if isinstance(name, CallFromPointer):
             self.base = name.base
         else:
             self.base = None
         self.name = str(name)
         self.arguments = as_tuple(arguments)
         self.retobj = retobj
         self.is_indirect = is_indirect
         self.cast = cast
         self._writes = as_tuple(writes)
+        self.templates = as_tuple(templates)
 
     def __repr__(self):
         ret = "" if self.retobj is None else "%s = " % self.retobj
         return "%sCall::\n\t%s(...)" % (ret, self.name)
 
+    def _rebuild(self, *args, **kwargs):
+        if args:
+            # Not elegant, but basically it handles the fact that a Call might
+            # have nested Calls/Lambdas among its `arguments`, and these might
+            # change, and we are in such a case *if and only if* we have `args`
+            assert len(args) == len(self.children)
+            mapper = dict(zip(self.children, args))
+            kwargs['arguments'] = [mapper.get(i, i) for i in self.arguments]
+        return super()._rebuild(**kwargs)
+
     @property
     def children(self):
         return tuple(i for i in self.arguments if isinstance(i, (Call, Lambda)))
 
     @cached_property
     def functions(self):
         retval = []
@@ -322,16 +345,14 @@
             retval.append(self.retobj)
 
         return tuple(filter_ordered(retval))
 
     @property
     def defines(self):
         ret = ()
-        if self.base is not None:
-            ret += (self.base,)
         if isinstance(self.retobj, Basic):
             ret += (self.retobj,)
         return ret
 
     @property
     def writes(self):
         return self._writes
@@ -359,16 +380,17 @@
     def __init__(self, expr, pragmas=None, init=False, operation=None):
         self.expr = expr
         self.pragmas = as_tuple(pragmas)
         self.init = init
         self.operation = operation
 
     def __repr__(self):
-        return "<%s::%s>" % (self.__class__.__name__,
-                             filter_ordered([f.func for f in self.functions]))
+        return "<%s::%s=%s>" % (self.__class__.__name__,
+                                type(self.write),
+                                ','.join('%s' % type(f) for f in self.functions))
 
     @property
     def dtype(self):
         return self.expr.dtype
 
     @property
     def output(self):
@@ -406,16 +428,16 @@
         return self.operation in (OpInc, OpMin, OpMax)
 
     @property
     def is_initializable(self):
         """
         True if it can be an initializing assignment, False otherwise.
         """
-        return ((self.is_scalar and not self.is_reduction) or
-                (self.is_tensor and isinstance(self.expr.rhs, ListInitializer)))
+        return (((self.is_scalar and not self.is_reduction) or
+                 (self.is_tensor and isinstance(self.expr.rhs, ListInitializer))))
 
     @property
     def defines(self):
         return (self.output.base,) if self.is_initializable else ()
 
     @property
     def expr_symbols(self):
@@ -717,80 +739,100 @@
     @property
     def all_parameters(self):
         return self.parameters + self.templates
 
     @property
     def functions(self):
         return tuple(i.function for i in self.all_parameters
-                     if isinstance(i.function, AbstractFunction))
+                     if isinstance(i.function, (AbstractFunction, AbstractObject)))
 
     @property
     def defines(self):
         return self.all_parameters
 
 
-class CallableBody(Node):
+class CallableBody(MultiTraversable):
 
     """
     The immediate child of a Callable.
 
     Parameters
     ----------
     body : Node or list of Node
         The actual body.
     unpacks : list of Nodes, optional
         Statements unpacking data from composite types.
     init : Node, optional
         A piece of IET to perform some initialization relevant for `body`
         (e.g., to initialize the target language runtime).
+    standalones : list of Definitions, optional
+        Object definitions for `body`. Instantiating these objects does not
+        require passing any arguments to their constructors, so these
+        Definitions can be scheduled safely right after `init`. They may or may
+        not be required by some of the subsequent nodes (e.g., `allocs`,
+        `maps`).
     allocs : list of Nodes, optional
         Data definitions and allocations for `body`.
+    stacks : list of Definitions, optional
+        Definitions for the stack-scoped objects appearing in `body`.
     casts : list of PointerCasts, optional
         Sequence of PointerCasts required by the `body`.
     bundles : list of Nodes, optional
         Data bundling for `body`. Used to initialize data subjected to layout
         transformation (w.r.t. how it arrives from Python), such as vector types.
     maps : Transfer or list of Transfer, optional
         Data maps for `body` (a data map may e.g. trigger a data transfer from
         host to device).
     strides : list of Nodes, optional
         Statements defining symbols used to access linearized arrays.
     objs : list of Definitions, optional
-        Object definitions for `body`.
+        Object definitions for `body`. Instantiating these objects may or may
+        not require some of the symbols defined in the previous nodes (e.g.,
+        `allocs`, `maps`).
     unmaps : Transfer or list of Transfer, optional
         Data unmaps for `body`.
     unbundles : list of Nodes, optional
         Data unbundling for `body`.
     frees : list of Calls, optional
         Data deallocations for `body`.
+    errors : list of Nodes, optional
+        Error handling for `body`.
+    retstmt : Node, optional
+        The return statement for `body`.
     """
 
     is_CallableBody = True
 
-    _traversable = ['unpacks', 'init', 'allocs', 'casts', 'bundles', 'maps',
-                    'strides', 'objs', 'body', 'unmaps', 'unbundles', 'frees']
-
-    def __init__(self, body, init=(), unpacks=(), strides=(), allocs=(), casts=(),
-                 bundles=(), objs=(), maps=(), unmaps=(), unbundles=(), frees=()):
+    _traversable = ['unpacks', 'init', 'standalones', 'allocs', 'stacks',
+                    'casts', 'bundles', 'maps', 'strides', 'objs', 'body',
+                    'unmaps', 'unbundles', 'frees', 'errors', 'retstmt']
+
+    def __init__(self, body, init=(), standalones=(), unpacks=(), strides=(),
+                 allocs=(), stacks=(), casts=(), bundles=(), objs=(), maps=(),
+                 unmaps=(), unbundles=(), frees=(), errors=(), retstmt=()):
         # Sanity check
         assert not isinstance(body, CallableBody), "CallableBody's cannot be nested"
 
         self.body = as_tuple(body)
 
         self.unpacks = as_tuple(unpacks)
         self.init = as_tuple(init)
+        self.standalones = as_tuple(standalones)
         self.allocs = as_tuple(allocs)
+        self.stacks = as_tuple(stacks)
         self.casts = as_tuple(casts)
         self.strides = as_tuple(strides)
         self.bundles = as_tuple(bundles)
         self.maps = as_tuple(maps)
         self.objs = as_tuple(objs)
         self.unmaps = as_tuple(unmaps)
         self.unbundles = as_tuple(unbundles)
         self.frees = as_tuple(frees)
+        self.errors = as_tuple(errors)
+        self.retstmt = as_tuple(retstmt)
 
     def __repr__(self):
         return ("<CallableBody <unpacks=%d, allocs=%d, casts=%d, maps=%d, "
                 "objs=%d> <unmaps=%d, frees=%d>>" %
                 (len(self.unpacks), len(self.allocs), len(self.casts),
                  len(self.maps), len(self.objs), len(self.unmaps),
                  len(self.frees)))
@@ -845,28 +887,28 @@
         The TimedList body.
     """
 
     def __init__(self, timer, lname, body):
         self._name = lname
         self._timer = timer
 
-        super().__init__(header=c.Line('START_TIMER(%s)' % lname),
+        super().__init__(header=c.Line('START(%s)' % lname),
                          body=body,
-                         footer=c.Line('STOP_TIMER(%s,%s)' % (lname, timer.name)))
+                         footer=c.Line('STOP(%s,%s)' % (lname, timer.name)))
 
     @classmethod
     def _start_timer_header(cls):
-        return ('START_TIMER(S)', ('struct timeval start_ ## S , end_ ## S ; '
-                                   'gettimeofday(&start_ ## S , NULL);'))
+        return ('START(S)', ('struct timeval start_ ## S , end_ ## S ; '
+                             'gettimeofday(&start_ ## S , NULL);'))
 
     @classmethod
     def _stop_timer_header(cls):
-        return ('STOP_TIMER(S,T)', ('gettimeofday(&end_ ## S, NULL); T->S += (double)'
-                                    '(end_ ## S .tv_sec-start_ ## S.tv_sec)+(double)'
-                                    '(end_ ## S .tv_usec-start_ ## S .tv_usec)/1000000;'))
+        return ('STOP(S,T)', ('gettimeofday(&end_ ## S, NULL); T->S += (double)'
+                              '(end_ ## S .tv_sec-start_ ## S.tv_sec)+(double)'
+                              '(end_ ## S .tv_usec-start_ ## S .tv_usec)/1000000;'))
 
     @property
     def name(self):
         return self._name
 
     @property
     def timer(self):
@@ -889,35 +931,49 @@
         self.function = function
 
     def __repr__(self):
         return "<Def(%s)>" % self.function
 
     @property
     def functions(self):
-        return (self.function,)
+        ret = [self.function]
+        for i in self.expr_symbols:
+            f = i.function
+            if f.is_AbstractFunction or f.is_AbstractObject:
+                ret.append(i.function)
+        return tuple(ret)
 
     @property
     def defines(self):
         if self.function._mem_stack:
             return (self.function.indexed,)
         else:
             return (self.function,)
 
     @property
     def expr_symbols(self):
-        if not self.function.is_Array or self.function.initvalue is None:
-            return ()
-        # These are just a handful of values so it's OK to iterate them over
-        ret = set()
-        for i in self.function.initvalue:
+        f = self.function
+        if f.is_LocalObject:
+            ret = set(flatten(i.free_symbols for i in f.cargs))
             try:
-                ret.update(i.free_symbols)
+                ret.update(f.initvalue.free_symbols)
             except AttributeError:
                 pass
-        return tuple(ret)
+            return tuple(ret)
+        elif f.is_Array and f.initvalue is not None:
+            # These are just a handful of values so it's OK to iterate them over
+            ret = set()
+            for i in f.initvalue:
+                try:
+                    ret.update(i.free_symbols)
+                except AttributeError:
+                    pass
+            return tuple(ret)
+        else:
+            return ()
 
 
 class PointerCast(ExprStmt, Node):
 
     """
     A node encapsulating a cast of a raw void pointer to a non-void,
     potentially multi-dimensional array.
@@ -1013,44 +1069,60 @@
 
 class Lambda(Node):
 
     """
     A callable C++ lambda function. Several syntaxes are possible; here we
     implement one of the common ones:
 
-        [captures](parameters){body}
+        [captures](parameters){body} SPECIAL [[attributes]]
 
     For more info about C++ lambda functions:
 
         https://en.cppreference.com/w/cpp/language/lambda
 
     Parameters
     ----------
     body : Node or list of Node
         The lambda function body.
     captures : list of str or expr-like, optional
         The captures of the lambda function.
     parameters : list of Basic or expr-like, optional
         The objects in input to the lambda function.
+    special : list of Basic, optional
+        Placeholder for custom lambdas, to add in e.g. macros.
+    attributes : list of str, optional
+        The attributes of the lambda function.
     """
 
     _traversable = ['body']
 
-    def __init__(self, body, captures=None, parameters=None):
+    def __init__(self, body, captures=None, parameters=None, special=None,
+                 attributes=None):
         self.body = as_tuple(body)
         self.captures = as_tuple(captures)
         self.parameters = as_tuple(parameters)
+        self.special = as_tuple(special)
+        self.attributes = as_tuple(attributes)
 
     def __repr__(self):
         return "Lambda[%s](%s)" % (self.captures, self.parameters)
 
+    @property
+    def functions(self):
+        return tuple(i.function for i in self.parameters
+                     if isinstance(i.function, AbstractFunction))
+
     @cached_property
     def expr_symbols(self):
         return tuple(self.parameters)
 
+    @property
+    def defines(self):
+        return tuple(self.parameters)
+
 
 class Section(List):
 
     """
     A sequence of nodes.
 
     Functionally, a Section is identical to a List; that is,
@@ -1059,15 +1131,15 @@
     the IET (e.g., groups of statements that logically represent the same
     computation unit).
     """
 
     is_Section = True
 
     def __init__(self, name, body=None, is_subsection=False):
-        super(Section, self).__init__(body=body)
+        super().__init__(body=body)
         self.name = name
         self.is_subsection = is_subsection
 
     def __repr__(self):
         return "<Section (%s)>" % self.name
 
     @property
@@ -1080,15 +1152,15 @@
     """
     A sequence of Expressions.
     """
 
     is_ExpressionBundle = True
 
     def __init__(self, ispace, ops, traffic, body=None):
-        super(ExpressionBundle, self).__init__(body=body)
+        super().__init__(body=body)
         self.ispace = ispace
         self.ops = ops
         self.traffic = traffic
 
     def __repr__(self):
         return "<ExpressionBundle (%d)>" % len(self.exprs)
 
@@ -1125,14 +1197,27 @@
         return self._single_thread
 
     @property
     def periodic(self):
         return self._periodic
 
 
+class UsingNamespace(Node):
+
+    """
+    A C++ using namespace directive.
+    """
+
+    def __init__(self, namespace):
+        self.namespace = namespace
+
+    def __repr__(self):
+        return "<UsingNamespace(%s)>" % self.namespace
+
+
 class Pragma(Node):
 
     """
     One or more pragmas floating in the IET constructed through a callback.
     """
 
     def __init__(self, callback, arguments=None):
@@ -1299,20 +1384,28 @@
     def __init__(self, **kwargs):
         super().__init__(header=c.Line())
 
     def __repr__(self):
         return ""
 
 
+class Break(Node):
+    pass
+
+
 class Return(Node):
 
     def __init__(self, value=None):
         self.value = value
 
 
+class ListMajor(List):
+    pass
+
+
 def DummyExpr(*args, init=False):
     return Expression(DummyEq(*args), init=init)
 
 
 BlankLine = CBlankLine()
 
 
@@ -1327,15 +1420,15 @@
     """
 
     is_HaloSpot = True
 
     _traversable = ['body']
 
     def __init__(self, body, halo_scheme):
-        super(HaloSpot, self).__init__()
+        super().__init__()
 
         if isinstance(body, Node):
             self._body = body
         elif isinstance(body, (list, tuple)) and len(body) == 1:
             self._body = body[0]
         elif body is None:
             self._body = List()
```

### Comparing `devito-4.8.3/devito/ir/iet/utils.py` & `devito-4.8.4/devito/ir/iet/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
         return self[-1] if self else None
 
     @property
     def dimensions(self):
         return [i.dim for i in self]
 
     def __repr__(self):
-        return "IterationTree%s" % super(IterationTree, self).__repr__()
+        return "IterationTree%s" % super().__repr__()
 
     def __getitem__(self, key):
-        ret = super(IterationTree, self).__getitem__(key)
+        ret = super().__getitem__(key)
         return IterationTree(ret) if isinstance(key, slice) else ret
 
 
 def retrieve_iteration_tree(node, mode='normal'):
     """
     A list with all Iteration sub-trees within an IET.
 
@@ -88,19 +88,21 @@
         if key(i):
             filtered.append(i)
         elif len(filtered) > 0:
             break
     return filtered
 
 
-def derive_parameters(iet, drop_locals=False):
+def derive_parameters(iet, drop_locals=False, ordering='default'):
     """
     Derive all input parameters (function call arguments) from an IET
     by collecting all symbols not defined in the tree itself.
     """
+    assert ordering in ('default', 'canonical')
+
     # Extract all candidate parameters
     candidates = FindSymbols().visit(iet)
 
     # Symbols, Objects, etc, become input parameters as well
     basics = FindSymbols('basics').visit(iet)
     candidates.extend(i.function for i in basics)
 
@@ -118,14 +120,23 @@
     parameters = [p for p in parameters
                   if not (p._mem_internal_eager or p._mem_constant)]
 
     # Maybe filter out all other compiler-generated objects
     if drop_locals:
         parameters = [p for p in parameters if not (p.is_ArrayBasic or p.is_LocalObject)]
 
+    # NOTE: This is requested by the caller when the parameters are used to
+    # construct Callables whose signature only depends on the object types,
+    # rather than on their name
+    # TODO: It should maybe be done systematically... but it's gonna change a huge
+    # amount of tests and examples; plus, it might break compatibility those
+    # using devito as a library-generator to be embedded within legacy codes
+    if ordering == 'canonical':
+        parameters = sorted(parameters, key=lambda p: str(type(p)))
+
     return parameters
 
 
 def maybe_alias(obj, candidate):
     """
     True if `candidate` can act as an alias for `obj`, False otherwise.
     """
```

### Comparing `devito-4.8.3/devito/ir/iet/visitors.py` & `devito-4.8.4/devito/ir/iet/visitors.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 
 import cgen as c
 from sympy import IndexedBase
 from sympy.core.function import Application
 
 from devito.exceptions import VisitorException
 from devito.ir.iet.nodes import (Node, Iteration, Expression, ExpressionBundle,
-                                 Call, Lambda, BlankLine, Section)
+                                 Call, Lambda, BlankLine, Section, ListMajor)
 from devito.ir.support.space import Backward
-from devito.symbolics import ListInitializer, ccode, uxreplace
+from devito.symbolics import (FieldFromComposite, FieldFromPointer,
+                              ListInitializer, ccode, uxreplace)
 from devito.tools import (GenericVisitor, as_tuple, ctypes_to_cstr, filter_ordered,
-                          filter_sorted, flatten, is_external_ctype, c_restrict_void_p)
+                          filter_sorted, flatten, is_external_ctype,
+                          c_restrict_void_p, sorted_priority)
 from devito.types.basic import AbstractFunction, Basic
 from devito.types import (ArrayObject, CompositeObject, Dimension, Pointer,
                           IndexedData, DeviceMap)
 
 
 __all__ = ['FindApplications', 'FindNodes', 'FindSections', 'FindSymbols',
            'MapExprStmts', 'MapHaloSpots', 'MapNodes', 'IsPerfectIteration',
@@ -61,15 +63,15 @@
     """
     Return a representation of the Iteration/Expression tree as a string,
     highlighting tree structure and node properties while dropping non-essential
     information.
     """
 
     def __init__(self, verbose=True):
-        super(PrintAST, self).__init__()
+        super().__init__()
         self.verbose = verbose
 
     @classmethod
     def default_retval(cls):
         return "<>"
 
     @property
@@ -187,18 +189,22 @@
     _restrict_keyword = 'restrict'
 
     def _gen_struct_decl(self, obj, masked=()):
         """
         Convert ctypes.Struct -> cgen.Structure.
         """
         ctype = obj._C_ctype
-        while issubclass(ctype, ctypes._Pointer):
-            ctype = ctype._type_
+        try:
+            while issubclass(ctype, ctypes._Pointer):
+                ctype = ctype._type_
 
-        if not issubclass(ctype, ctypes.Structure):
+            if not issubclass(ctype, ctypes.Structure):
+                return None
+        except TypeError:
+            # E.g., `ctype` is of type `dtypes_lowering.CustomDtype`
             return None
 
         try:
             return obj._C_typedecl
         except AttributeError:
             pass
 
@@ -218,65 +224,81 @@
                 cstr = ctypes_to_cstr(ct)
                 if ct is c_restrict_void_p:
                     cstr = '%srestrict' % cstr
                 entries.append(c.Value(cstr, n))
 
         return c.Struct(ctype.__name__, entries)
 
-    def _gen_value(self, obj, level=2, masked=()):
+    def _gen_value(self, obj, mode=1, masked=()):
+        """
+        Convert a devito.types.Basic object into a cgen declaration/definition.
+
+        A Basic object may need to be declared and optionally defined in three
+        different ways, which correspond to the three possible values of `mode`:
+
+            * 0: Simple. E.g., `int a = 1`;
+            * 1: Comprehensive. E.g., `const int *restrict a`, `int a[10]`;
+            * 2: Declaration suitable for a function parameter list.
+        """
         qualifiers = [v for k, v in self._qualifiers_mapper.items()
-                      if getattr(obj, k, False) and v not in masked]
+                      if getattr(obj.function, k, False) and v not in masked]
 
-        if (obj._mem_stack or obj._mem_constant) and level == 2:
+        if (obj._mem_stack or obj._mem_constant) and mode == 1:
             strtype = obj._C_typedata
             strshape = ''.join('[%s]' % ccode(i) for i in obj.symbolic_shape)
         else:
             strtype = ctypes_to_cstr(obj._C_ctype)
             strshape = ''
-            if isinstance(obj, (AbstractFunction, IndexedData)) and level >= 1:
-                strtype = '%s%s' % (strtype, self._restrict_keyword)
+            if isinstance(obj, (AbstractFunction, IndexedData)) and mode >= 1:
+                if not obj._mem_stack:
+                    strtype = '%s%s' % (strtype, self._restrict_keyword)
         strtype = ' '.join(qualifiers + [strtype])
 
+        if obj.is_LocalObject and obj._C_modifier is not None and mode == 2:
+            strtype += obj._C_modifier
+
         strname = obj._C_name
         strobj = '%s%s' % (strname, strshape)
 
-        try:
-            if obj.cargs:
-                strobj = MultilineCall(strobj, obj.cargs, True)
-        except AttributeError:
-            pass
+        if obj.is_LocalObject and obj.cargs and mode == 1:
+            arguments = [ccode(i) for i in obj.cargs]
+            strobj = MultilineCall(strobj, arguments, True)
 
         value = c.Value(strtype, strobj)
 
         try:
-            if obj.is_AbstractFunction and obj._data_alignment and level == 2:
+            if obj.is_AbstractFunction and obj._data_alignment and mode == 1:
                 value = c.AlignedAttribute(obj._data_alignment, value)
         except AttributeError:
             pass
 
-        try:
-            if obj.initvalue is not None and level == 2:
-                init = ListInitializer(obj.initvalue)
-                if not obj._mem_constant or init.is_numeric:
-                    value = c.Initializer(value, ccode(init))
-        except AttributeError:
-            pass
+        if obj.is_Array and obj.initvalue is not None and mode == 1:
+            init = ListInitializer(obj.initvalue)
+            if not obj._mem_constant or init.is_numeric:
+                value = c.Initializer(value, ccode(init))
+        elif obj.is_LocalObject and obj.initvalue is not None and mode == 1:
+            value = c.Initializer(value, ccode(obj.initvalue))
 
         return value
 
     def _gen_rettype(self, obj):
         try:
             return self._gen_value(obj, 0).typename
         except AttributeError:
-            assert isinstance(obj, str)
+            pass
+        if isinstance(obj, str):
             return obj
+        elif isinstance(obj, (FieldFromComposite, FieldFromPointer)):
+            return self._gen_value(obj.function.base, 0).typename
+        else:
+            return None
 
     def _args_decl(self, args):
         """Generate cgen declarations from an iterable of symbols and expressions."""
-        return [self._gen_value(i, 1) for i in args]
+        return [self._gen_value(i, 2) for i in args]
 
     def _args_call(self, args):
         """
         Generate cgen function call arguments from an iterable of symbols and expressions.
         """
         ret = []
         for i in args:
@@ -287,28 +309,32 @@
                     ret.append(self._visit(i))
                 else:
                     ret.append(i._C_name)
             except AttributeError:
                 ret.append(ccode(i))
         return ret
 
-    def _gen_signature(self, o):
+    def _gen_signature(self, o, is_declaration=False):
         decls = self._args_decl(o.parameters)
         prefix = ' '.join(o.prefix + (self._gen_rettype(o.retval),))
         signature = c.FunctionDeclaration(c.Value(prefix, o.name), decls)
         if o.templates:
             tparams = ', '.join([i.inline() for i in self._args_decl(o.templates)])
-            signature = c.Template(tparams, signature)
+            if is_declaration:
+                signature = TemplateDecl(tparams, signature)
+            else:
+                signature = c.Template(tparams, signature)
         return signature
 
     def _blankline_logic(self, children):
         """
         Generate cgen blank lines in between logical units.
         """
-        candidates = (Expression, ExpressionBundle, Iteration, Section)
+        candidates = (Expression, ExpressionBundle, Iteration, Section,
+                      ListMajor)
 
         processed = []
         for child in children:
             prev = None
             rebuilt = []
             for k, group in groupby(child, key=type):
                 g = list(group)
@@ -320,15 +346,17 @@
                         rebuilt.append(i)
                         rebuilt.append(BlankLine)
                     rebuilt.append(g[-1])
                 elif (k is Iteration and
                       prev is ExpressionBundle and
                       all(i.dim.is_Stencil for i in g)):
                     rebuilt.extend(g)
-                elif prev in candidates and k in candidates:
+                elif (prev in candidates and k in candidates) or \
+                     (prev is not None and k in (ListMajor, Section)) or \
+                     (prev in (ListMajor, Section)):
                     rebuilt.append(BlankLine)
                     rebuilt.extend(g)
                 else:
                     rebuilt.extend(g)
 
                 prev = k
 
@@ -371,15 +399,15 @@
             if o.flat is None:
                 shape = ''.join("[%s]" % ccode(i) for i in o.castshape)
                 rshape = '(*)%s' % shape
                 lvalue = c.Value(i._C_typedata, '(*restrict %s)%s' % (v, shape))
             else:
                 rshape = '*'
                 lvalue = c.Value(i._C_typedata, '*%s' % v)
-            if o.alignment:
+            if o.alignment and f._data_alignment:
                 lvalue = c.AlignedAttribute(f._data_alignment, lvalue)
 
             # rvalue
             if f.is_DiscreteFunction or (f.is_Array and f._mem_mapped):
                 if isinstance(o.obj, IndexedData):
                     v = f._C_field_data
                 elif isinstance(o.obj, DeviceMap):
@@ -402,23 +430,21 @@
         a0, a1 = o.functions
         if a1.is_PointerArray or a1.is_TempFunction:
             i = a1.indexed
             if o.flat is None:
                 shape = ''.join("[%s]" % ccode(i) for i in a0.symbolic_shape[1:])
                 rvalue = '(%s (*)%s) %s[%s]' % (i._C_typedata, shape, a1.name,
                                                 a1.dim.name)
-                lvalue = c.AlignedAttribute(
-                    a0._data_alignment,
-                    c.Value(i._C_typedata, '(*restrict %s)%s' % (a0.name, shape))
-                )
+                lvalue = c.Value(i._C_typedata,
+                                 '(*restrict %s)%s' % (a0.name, shape))
             else:
                 rvalue = '(%s *) %s[%s]' % (i._C_typedata, a1.name, a1.dim.name)
-                lvalue = c.AlignedAttribute(
-                    a0._data_alignment, c.Value(i._C_typedata, '*restrict %s' % a0.name)
-                )
+                lvalue = c.Value(i._C_typedata, '*restrict %s' % a0.name)
+            if a0._data_alignment:
+                lvalue = c.AlignedAttribute(a0._data_alignment, lvalue)
         else:
             rvalue = '%s->%s' % (a1.name, a0._C_name)
             lvalue = self._gen_value(a0, 0)
         return c.Initializer(lvalue, rvalue)
 
     def visit_Block(self, o):
         body = flatten(self._visit(i) for i in self._blankline_logic(o.children))
@@ -426,21 +452,18 @@
 
     def visit_List(self, o):
         body = flatten(self._visit(i) for i in self._blankline_logic(o.children))
         return c.Module(o.header + (c.Collection(body),) + o.footer)
 
     def visit_Section(self, o):
         body = flatten(self._visit(i) for i in o.children)
-        if o.is_subsection:
-            header = []
-            footer = []
-        else:
-            header = [c.Comment("Begin %s" % o.name)]
-            footer = [c.Comment("End %s" % o.name)]
-        return c.Module(header + body + footer)
+        return c.Module(body)
+
+    def visit_Break(self, o):
+        return c.Statement('break')
 
     def visit_Return(self, o):
         v = 'return'
         if o.value is not None:
             v += ' %s' % o.value
         return c.Statement(v)
 
@@ -467,24 +490,27 @@
         code = c.Statement("%s %s= %s" % (c_lhs, o.op, c_rhs))
         if o.pragmas:
             code = c.Module(list(o.pragmas) + [code])
         return code
 
     def visit_Call(self, o, nested_call=False):
         retobj = o.retobj
-        cast = o.cast and self._gen_rettype(retobj)
+        rettype = self._gen_rettype(retobj)
+        cast = o.cast and rettype
         arguments = self._args_call(o.arguments)
         if retobj is None:
-            return MultilineCall(o.name, arguments, nested_call, o.is_indirect, cast)
+            return MultilineCall(o.name, arguments, nested_call, o.is_indirect,
+                                 cast, o.templates)
         else:
-            call = MultilineCall(o.name, arguments, True, o.is_indirect, cast)
-            if retobj.is_Indexed:
+            call = MultilineCall(o.name, arguments, True, o.is_indirect, cast,
+                                 o.templates)
+            if retobj.is_Indexed or \
+               isinstance(retobj, (FieldFromComposite, FieldFromPointer)):
                 return c.Assign(ccode(retobj), call)
             else:
-                rettype = self._gen_rettype(retobj)
                 return c.Initializer(c.Value(rettype, retobj._C_name), call)
 
     def visit_Conditional(self, o):
         try:
             then_body, else_body = self._blankline_logic(o.children)
         except ValueError:
             # Some special subclasses of Conditional such as ThreadedProdder
@@ -549,37 +575,73 @@
             return c.Statement('while(%s)' % condition)
 
     def visit_Callable(self, o):
         body = flatten(self._visit(i) for i in o.children)
         signature = self._gen_signature(o)
         return c.FunctionBody(signature, c.Block(body))
 
-    def visit_CallableBody(self, o):
+    def visit_MultiTraversable(self, o):
         body = []
         prev = None
         for i in o.children:
             v = self._visit(i)
             if v:
                 if prev:
                     body.append(c.Line())
                 prev = v
                 body.extend(as_tuple(v))
         return c.Collection(body)
 
+    def visit_UsingNamespace(self, o):
+        return c.Statement('using namespace %s' % ccode(o.namespace))
+
     def visit_Lambda(self, o):
-        body = flatten(self._visit(i) for i in o.children)
+        body = []
+        for i in o.children:
+            v = self._visit(i)
+            if v:
+                if body:
+                    body.append(c.Line())
+                body.extend(as_tuple(v))
         captures = [str(i) for i in o.captures]
         decls = [i.inline() for i in self._args_decl(o.parameters)]
-        top = c.Line('[%s](%s)' % (', '.join(captures), ', '.join(decls)))
+        extra = []
+        if o.special:
+            extra.append(' ')
+            extra.append(' '.join(str(i) for i in o.special))
+        if o.attributes:
+            extra.append(' ')
+            extra.append(' '.join('[[%s]]' % i for i in o.attributes))
+        top = c.Line('[%s](%s)%s' %
+                     (', '.join(captures), ', '.join(decls), ''.join(extra)))
         return LambdaCollection([top, c.Block(body)])
 
     def visit_HaloSpot(self, o):
         body = flatten(self._visit(i) for i in o.children)
         return c.Collection(body)
 
+    def visit_KernelLaunch(self, o):
+        if o.templates:
+            templates = '<%s>' % ','.join([str(i) for i in o.templates])
+        else:
+            templates = ''
+
+        launch_args = [o.grid, o.block]
+        if o.shm is not None:
+            launch_args.append(o.shm)
+        if o.stream is not None:
+            launch_args.append(o.stream)
+        launch_config = ','.join(str(i) for i in launch_args)
+
+        arguments = self._args_call(o.arguments)
+        arguments = ','.join(arguments)
+
+        return c.Statement('%s%s<<<%s>>>(%s)'
+                           % (o.name, templates, launch_config, arguments))
+
     # Operator-handle machinery
 
     def _operator_includes(self, o):
         return [c.Include(i, system=(False if i.endswith('.h') else True))
                 for i in o._includes]
 
     def _operator_typedecls(self, o, mode='all'):
@@ -592,15 +654,16 @@
             if mode == 'public':
                 xfilter1 = lambda i: xfilter0(i) and isinstance(i, public_types)
             else:
                 xfilter1 = lambda i: xfilter0(i) and not isinstance(i, public_types)
 
         # This is essentially to rule out vector types which are declared already
         # in some external headers
-        xfilter = lambda i: xfilter1(i) and not is_external_ctype(i._C_ctype, o._includes)
+        xfilter = lambda i: (xfilter1(i) and
+                             not is_external_ctype(i._C_ctype, o._includes))
 
         candidates = o.parameters + tuple(o._dspace.parts)
         typedecls = [self._gen_struct_decl(i) for i in candidates if xfilter(i)]
         for i in o._func_table.values():
             if not i.local:
                 continue
             typedecls.extend([self._gen_struct_decl(j) for j in i.root.parameters
@@ -615,43 +678,54 @@
 
         return [self._gen_value(i) for i in v]
 
     def visit_Operator(self, o, mode='all'):
         # Kernel signature and body
         body = flatten(self._visit(i) for i in o.children)
         signature = self._gen_signature(o)
-        retval = [c.Line(), c.Statement("return 0")]
+
+        # Honor the `retstmt` flag if set
+        if o.body.retstmt:
+            retval = []
+        else:
+            retval = [c.Line(), c.Statement("return 0")]
+
         kernel = c.FunctionBody(signature, c.Block(body + retval))
 
         # Elemental functions
         esigns = []
         efuncs = [blankline]
-        for i in o._func_table.values():
-            if i.local:
-                esigns.append(self._gen_signature(i.root))
-                efuncs.extend([self._visit(i.root), blankline])
+        items = [i.root for i in o._func_table.values() if i.local]
+        for i in sorted_efuncs(items):
+            esigns.append(self._gen_signature(i, is_declaration=True))
+            efuncs.extend([self._visit(i), blankline])
 
         # Definitions
         headers = [c.Define(*i) for i in o._headers] + [blankline]
 
         # Header files
         includes = self._operator_includes(o) + [blankline]
 
+        # Namespaces
+        namespaces = [self._visit(i) for i in o._namespaces]
+        if namespaces:
+            namespaces.append(blankline)
+
         # Type declarations
         typedecls = self._operator_typedecls(o, mode)
         if mode in ('all', 'public') and o._compiler.src_ext in ('cpp', 'cu'):
             typedecls.append(c.Extern('C', signature))
         typedecls = [i for j in typedecls for i in (j, blankline)]
 
         # Global variables
         globs = self._operator_globals(o, mode)
         if globs:
             globs.append(blankline)
 
-        return c.Module(headers + includes + typedecls + globs +
+        return c.Module(headers + includes + namespaces + typedecls + globs +
                         esigns + [blankline, kernel] + efuncs)
 
 
 class CInterface(CGen):
 
     def _operator_includes(self, o):
         includes = super()._operator_includes(o)
@@ -732,14 +806,16 @@
             ret = self.default_retval()
         if queue is not None:
             ret.setdefault(tuple(queue), []).append(o)
         for i in o.children:
             ret = self._visit(i, ret=ret, queue=queue)
         return ret
 
+    visit_Call = visit_Conditional
+
 
 class MapKind(FindSections):
 
     """
     Base class to construct mappers from Nodes of given type to their enclosing
     scope of Nodes.
     """
@@ -751,19 +827,29 @@
         if ret is None:
             ret = self.default_retval()
         ret[o] = as_tuple(queue)
         return ret
 
     visit_Conditional = FindSections.visit_Iteration
     visit_Block = FindSections.visit_Iteration
+    visit_Lambda = FindSections.visit_Iteration
 
 
 class MapExprStmts(MapKind):
+
     visit_ExprStmt = MapKind.visit_dummy
 
+    def visit_Call(self, o, ret=None, queue=None):
+        if ret is None:
+            ret = self.default_retval()
+        ret[o] = as_tuple(queue)
+        for i in o.children:
+            ret = self._visit(i, ret=ret, queue=queue)
+        return ret
+
 
 class MapHaloSpots(MapKind):
     visit_HaloSpot = MapKind.visit_dummy
 
 
 class MapNodes(Visitor):
 
@@ -789,15 +875,15 @@
         the nodes of type ``child_types`` retrieved by the search. This behaviour
         can be changed through this parameter. Accepted values are:
         - 'immediate': only the closest matching ancestor is mapped.
         - 'groupby': the matching ancestors are grouped together as a single key.
     """
 
     def __init__(self, parent_type=None, child_types=None, mode=None):
-        super(MapNodes, self).__init__()
+        super().__init__()
         if parent_type is None:
             self.parent_type = Iteration
         elif parent_type == 'any':
             self.parent_type = Node
         else:
             assert issubclass(parent_type, Node)
             self.parent_type = parent_type
@@ -883,15 +969,15 @@
         'basics': lambda n: [i for i in n.expr_symbols if isinstance(i, Basic)],
         'dimensions': lambda n: [i for i in n.expr_symbols if isinstance(i, Dimension)],
         'indexeds': lambda n: [i for i in n.expr_symbols if i.is_Indexed],
         'indexedbases': lambda n: [i for i in n.expr_symbols
                                    if isinstance(i, IndexedBase)],
         'writes': lambda n: as_tuple(n.writes),
         'defines': lambda n: as_tuple(n.defines),
-        'globals': lambda n: [f.indexed for f in n.functions if f._mem_constant],
+        'globals': lambda n: [f.base for f in n.functions if f._mem_global],
         'defines-aliases': _defines_aliases
     }
 
     def __init__(self, mode='symbolics'):
         super().__init__()
 
         modes = mode.split('|')
@@ -945,15 +1031,15 @@
 
     rules = {
         'type': lambda match, o: isinstance(o, match),
         'scope': lambda match, o: match in flatten(o.children)
     }
 
     def __init__(self, match, mode='type'):
-        super(FindNodes, self).__init__()
+        super().__init__()
         self.match = match
         self.rule = self.rules[mode]
 
     def visit_object(self, o, ret=None):
         return ret
 
     def visit_tuple(self, o, ret=None):
@@ -1025,15 +1111,15 @@
 class IsPerfectIteration(Visitor):
 
     """
     Return True if an Iteration defines a perfect loop nest, False otherwise.
     """
 
     def __init__(self, depth=None):
-        super(IsPerfectIteration, self).__init__()
+        super().__init__()
 
         assert depth is None or isinstance(depth, Iteration)
         self.depth = depth
 
     def visit_object(self, o, **kwargs):
         return False
 
@@ -1078,15 +1164,15 @@
     In the special case in which ``M[n]`` is None, ``n`` is dropped from T'.
 
     In the special case in which ``M[n]`` is an iterable of nodes, ``n`` is
     "extended" by pre-pending to its body the nodes in ``M[n]``.
     """
 
     def __init__(self, mapper, nested=False):
-        super(Transformer, self).__init__()
+        super().__init__()
         self.mapper = mapper
         self.nested = nested
 
     def visit_object(self, o, **kwargs):
         return o
 
     def visit_tuple(self, o, **kwargs):
@@ -1162,32 +1248,48 @@
 
     def visit_Callable(self, o):
         body = self._visit(o.body)
         parameters = [self.mapper.get(i, i) for i in o.parameters]
         return o._rebuild(body=body, parameters=parameters)
 
     def visit_Call(self, o):
-        arguments = [uxreplace(i, self.mapper) for i in o.arguments]
+        arguments = []
+        for i in o.arguments:
+            if i in o.children:
+                arguments.append(self._visit(i))
+            else:
+                arguments.append(uxreplace(i, self.mapper))
         if o.retobj is not None:
             retobj = uxreplace(o.retobj, self.mapper)
             return o._rebuild(arguments=arguments, retobj=retobj)
         else:
             return o._rebuild(arguments=arguments)
 
+    def visit_Lambda(self, o):
+        body = self._visit(o.body)
+        parameters = [self.mapper.get(i, i) for i in o.parameters]
+        return o._rebuild(body=body, parameters=parameters)
+
     def visit_Conditional(self, o):
         condition = uxreplace(o.condition, self.mapper)
         then_body = self._visit(o.then_body)
         else_body = self._visit(o.else_body)
-        return o._rebuild(condition=condition, then_body=then_body, else_body=else_body)
+        return o._rebuild(condition=condition, then_body=then_body,
+                          else_body=else_body)
 
     def visit_PointerCast(self, o):
         function = self.mapper.get(o.function, o.function)
         obj = self.mapper.get(o.obj, o.obj)
         return o._rebuild(function=function, obj=obj)
 
+    def visit_Dereference(self, o):
+        pointee = self.mapper.get(o.pointee, o.pointee)
+        pointer = self.mapper.get(o.pointer, o.pointer)
+        return o._rebuild(pointee=pointee, pointer=pointer)
+
     def visit_Pragma(self, o):
         arguments = [uxreplace(i, self.mapper) for i in o.arguments]
         return o._rebuild(arguments=arguments)
 
     def visit_PragmaTransfer(self, o):
         function = uxreplace(o.function, self.mapper)
         arguments = [uxreplace(i, self.mapper) for i in o.arguments]
@@ -1196,16 +1298,29 @@
     def visit_HaloSpot(self, o):
         hs = o.halo_scheme
         fmapper = {self.mapper.get(k, k): v for k, v in hs.fmapper.items()}
         halo_scheme = hs.build(fmapper, hs.honored)
         body = self._visit(o.body)
         return o._rebuild(halo_scheme=halo_scheme, body=body)
 
+    def visit_While(self, o, **kwargs):
+        condition = uxreplace(o.condition, self.mapper)
+        body = self._visit(o.body)
+        return o._rebuild(condition=condition, body=body)
+
     visit_ThreadedProdder = visit_Call
 
+    def visit_KernelLaunch(self, o):
+        arguments = [uxreplace(i, self.mapper) for i in o.arguments]
+        grid = self.mapper.get(o.grid, o.grid)
+        block = self.mapper.get(o.block, o.block)
+        stream = self.mapper.get(o.stream, o.stream)
+        return o._rebuild(grid=grid, block=block, stream=stream,
+                          arguments=arguments)
+
 
 # Utils
 
 blankline = c.Line("")
 
 
 def printAST(node, verbose=True):
@@ -1214,26 +1329,32 @@
 
 class LambdaCollection(c.Collection):
     pass
 
 
 class MultilineCall(c.Generable):
 
-    def __init__(self, name, arguments, is_expr=False, is_indirect=False, cast=None):
+    def __init__(self, name, arguments, is_expr=False, is_indirect=False,
+                 cast=None, templates=None):
         self.name = name
         self.arguments = as_tuple(arguments)
         self.is_expr = is_expr
         self.is_indirect = is_indirect
         self.cast = cast
+        self.templates = templates
 
     def generate(self):
+        if self.templates:
+            tip = "%s<%s>" % (self.name, ", ".join(str(i) for i in self.templates))
+        else:
+            tip = self.name
         if not self.is_indirect:
-            tip = "%s(" % self.name
+            tip = "%s(" % tip
         else:
-            tip = "%s%s" % (self.name, ',' if self.arguments else '')
+            tip = "%s%s" % (tip, ',' if self.arguments else '')
         processed = []
         for i in self.arguments:
             if isinstance(i, (MultilineCall, LambdaCollection)):
                 lines = list(i.generate())
                 if len(lines) > 1:
                     yield tip + ",".join(processed + [lines[0]])
                     for line in lines[1:-1]:
@@ -1249,7 +1370,28 @@
         if not self.is_indirect:
             tip += ")"
         if not self.is_expr:
             tip += ";"
         if self.cast:
             tip = '(%s)%s' % (self.cast, tip)
         yield tip
+
+
+class TemplateDecl(c.Template):
+
+    # Workaround to generate ';' at the end
+
+    def generate(self):
+        return super().generate(with_semicolon=True)
+
+
+def sorted_efuncs(efuncs):
+    from devito.ir.iet.efunc import (CommCallable, DeviceFunction,
+                                     ThreadCallable, ElementalFunction)
+
+    priority = {
+        DeviceFunction: 3,
+        ThreadCallable: 2,
+        ElementalFunction: 1,
+        CommCallable: 1
+    }
+    return sorted_priority(efuncs, priority)
```

### Comparing `devito-4.8.3/devito/ir/stree/algorithms.py` & `devito-4.8.4/devito/ir/stree/algorithms.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from devito.ir.clusters import Cluster
 from devito.ir.stree.tree import (ScheduleTree, NodeIteration, NodeConditional,
                                   NodeSync, NodeExprs, NodeSection, NodeHalo)
 from devito.ir.support import (SEQUENTIAL, Any, Interval, IterationInterval,
                                IterationSpace, normalize_properties, normalize_syncs)
 from devito.mpi.halo_scheme import HaloScheme
-from devito.tools import Bunch, DefaultOrderedDict
+from devito.tools import Bunch, DefaultOrderedDict, as_mapper
 
 __all__ = ['stree_build']
 
 
 def stree_build(clusters, profiler=None, **kwargs):
     """
     Create a ScheduleTree from a ClusterGroup.
@@ -81,14 +81,18 @@
             tip = augment_whole_subtree(c, tip, mapper, it)
 
         # Attach NodeHalo if necessary
         for it, v in mapper.items():
             if needs_nodehalo(it.dim, c.halo_scheme):
                 v.bottom.parent = NodeHalo(c.halo_scheme, v.bottom.parent)
                 break
+        else:
+            if c.halo_scheme:
+                assert not c.exprs  # See preprocess() -- we rarely end up here!
+                tip = NodeHalo(c.halo_scheme, v.bottom)
 
         # Add in NodeExprs
         exprs = []
         for conditionals, g in groupby(c.exprs, key=lambda e: e.conditionals):
             exprs = list(g)
 
             # Indirect ConditionalDimensions induce expression-level guards
@@ -128,25 +132,42 @@
 # *** Utilities to construct the ScheduleTree
 
 base = IterationInterval(Interval(None), [], Any)
 
 
 def preprocess(clusters, options=None, **kwargs):
     """
-    Remove the HaloTouch's from `clusters` and create a mapping associating
-    each removed HaloTouch to the first Cluster necessitating it.
+    Lower the so-called "wild" Clusters, that is objects not representing a set
+    of mathematical operations. This boils down to:
+
+        * Moving the HaloTouch's from `clusters` into a mapper `M: {HT -> C}`.
+          `c = M(ht)` is the first Cluster of the sequence requiring the halo
+          exchange `ht` to have terminated before the execution can proceed.
+        * Lower the CriticalRegions:
+            * If they encode an asynchronous operation (e.g., a WaitLock), attach
+              it to a Nop Cluster for future lowering;
+            * Otherwise, simply remove them, as they have served their purpose
+              at this point.
+        * Remove the WeakFences, as they have served their purpose at this point.
     """
     queue = []
     processed = []
     for c in clusters:
         if c.is_halo_touch:
             hs = HaloScheme.union(e.rhs.halo_scheme for e in c.exprs)
-            queue.append(c.rebuild(halo_scheme=hs))
+            queue.append(c.rebuild(exprs=[], halo_scheme=hs))
+
+        elif c.is_critical_region and c.syncs:
+            processed.append(c.rebuild(exprs=None, guards=c.guards, syncs=c.syncs))
+
+        elif c.is_wild:
+            continue
+
         else:
-            dims = set(c.ispace.promote(lambda d: d.is_Block).itdimensions)
+            dims = set(c.ispace.promote(lambda d: d.is_Block).itdims)
 
             found = []
             for c1 in list(queue):
                 distributed_aindices = c1.halo_scheme.distributed_aindices
                 h_indices = set().union(*[d._defines for d in c1.halo_scheme.loc_indices])
 
                 # Skip if the halo exchange would end up outside
@@ -163,16 +184,31 @@
                     queue.remove(c1)
 
             syncs = normalize_syncs(*[c1.syncs for c1 in found])
             if syncs:
                 ispace = c.ispace.project(syncs)
                 processed.append(c.rebuild(exprs=[], ispace=ispace, syncs=syncs))
 
-            halo_scheme = HaloScheme.union([c1.halo_scheme for c1 in found])
-            processed.append(c.rebuild(halo_scheme=halo_scheme))
+            if all(c1.ispace.is_subset(c.ispace) for c1 in found):
+                # 99% of the cases we end up here
+                hs = HaloScheme.union([c1.halo_scheme for c1 in found])
+                processed.append(c.rebuild(halo_scheme=hs))
+            elif options['mpi']:
+                # We end up here with e.g. `t,x,y,z,f` where `f` is a sequential
+                # dimension requiring a loc-index in the HaloScheme. The compiler
+                # will generate the non-perfect loop nest `t,f ; t,x,y,z,f`, with
+                # the first nest triggering all necessary halo exchanges along `f`
+                mapper = as_mapper(found, lambda c1: c1.ispace)
+                for k, v in mapper.items():
+                    hs = HaloScheme.union([c1.halo_scheme for c1 in v])
+                    processed.append(c.rebuild(exprs=[], ispace=k, halo_scheme=hs))
+                processed.append(c)
+            else:
+                # Avoid ugly empty loops
+                processed.append(c)
 
     # Sanity check!
     try:
         assert not queue
     except AssertionError:
         if options['mpi']:
             raise RuntimeError("Unsupported MPI for the given equations")
```

### Comparing `devito-4.8.3/devito/ir/stree/tree.py` & `devito-4.8.4/devito/ir/stree/tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class NodeIteration(ScheduleTree):
 
     is_Iteration = True
 
     def __init__(self, ispace, parent=None, properties=None):
-        super(NodeIteration, self).__init__(parent)
+        super().__init__(parent)
         self.ispace = ispace
         self.properties = properties
 
     @property
     def interval(self):
         return self.ispace.intervals[0]
 
@@ -74,41 +74,41 @@
 
 
 class NodeConditional(ScheduleTree):
 
     is_Conditional = True
 
     def __init__(self, guard, parent=None):
-        super(NodeConditional, self).__init__(parent)
+        super().__init__(parent)
         self.guard = guard
 
     @property
     def __repr_render__(self):
         return "If"
 
 
 class NodeSync(ScheduleTree):
 
     is_Sync = True
 
     def __init__(self, sync_ops, parent=None):
-        super(NodeSync, self).__init__(parent)
+        super().__init__(parent)
         self.sync_ops = sync_ops
 
     @property
     def __repr_render__(self):
         return "Sync[%s]" % ",".join(i.__class__.__name__ for i in self.sync_ops)
 
 
 class NodeExprs(ScheduleTree):
 
     is_Exprs = True
 
     def __init__(self, exprs, ispace, dspace, ops, traffic, parent=None):
-        super(NodeExprs, self).__init__(parent)
+        super().__init__(parent)
         self.exprs = exprs
         self.ispace = ispace
         self.dspace = dspace
         self.ops = ops
         self.traffic = traffic
 
     @property
```

### Comparing `devito-4.8.3/devito/ir/support/basic.py` & `devito-4.8.4/devito/ir/support/basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from itertools import chain, product
 
 from cached_property import cached_property
 from sympy import S
 
-from devito.ir.support.space import Backward, IterationSpace
-from devito.ir.support.utils import AccessMode
+from devito.ir.support.space import Backward, null_ispace
+from devito.ir.support.utils import AccessMode, extrema
 from devito.ir.support.vector import LabeledVector, Vector
-from devito.symbolics import (retrieve_terminals, q_constant, q_affine, q_routine,
-                              q_terminal)
-from devito.tools import (Tag, as_tuple, is_integer, filter_sorted, flatten,
-                          memoized_meth, memoized_generator)
-from devito.types import Barrier, Dimension, DimensionTuple, Jump, Symbol
+from devito.symbolics import (compare_ops, retrieve_indexed, retrieve_terminals,
+                              q_constant, q_affine, q_routine, search, uxreplace)
+from devito.tools import (Tag, as_mapper, as_tuple, is_integer, filter_sorted,
+                          flatten, memoized_meth, memoized_generator)
+from devito.types import (ComponentAccess, Dimension, DimensionTuple, Fence,
+                          CriticalRegion, Function, Symbol, Temp, TempArray,
+                          TBArray)
 
-__all__ = ['IterationInstance', 'TimedAccess', 'Scope']
+__all__ = ['IterationInstance', 'TimedAccess', 'Scope', 'ExprGeometry']
 
 
 class IndexMode(Tag):
     """Tag for access functions."""
     pass
 AFFINE = IndexMode('affine')  # noqa
 REGULAR = IndexMode('regular')
 IRREGULAR = IndexMode('irregular')
 
-mocksym = Symbol(name='⋈')
-"""
-A Symbol to create mock data depdendencies.
-"""
+# Symbols to create mock data depdendencies
+mocksym0 = Symbol(name='__⋈_0__')
+mocksym1 = Symbol(name='__⋈_1__')
 
 
 class IterationInstance(LabeledVector):
 
     """
     A representation of the iteration and data points accessed by an
     Indexed object. Three different concepts are distinguished:
@@ -213,35 +214,36 @@
     """
 
     def __new__(cls, access, mode, timestamp, ispace=None):
         obj = super().__new__(cls, access)
         AccessMode.__init__(obj, mode=mode)
         return obj
 
-    def __init__(self, access, mode, timestamp, ispace=None):
+    def __init__(self, access, mode, timestamp, ispace=null_ispace):
         assert is_integer(timestamp)
 
         self.access = access
         self.timestamp = timestamp
-        self.ispace = ispace or IterationSpace([])
+        self.ispace = ispace
 
     def __repr__(self):
         mode = '\033[1;37;31mW\033[0m' if self.is_write else '\033[1;37;32mR\033[0m'
         return "%s<%s,[%s]>" % (mode, self.name, ', '.join(str(i) for i in self))
 
     def __eq__(self, other):
         if not isinstance(other, TimedAccess):
             return False
 
         # At this point no need to go through the class hierarchy's __eq__,
         # which might require expensive comparisons of Vector entries (i.e.,
         # SymPy expressions)
 
-        return (self.access is other.access and  # => self.function is other.function
-                self.mode == other.mode and
+        return (self.mode == other.mode and
+                self.timestamp == other.timestamp and
+                self.access == other.access and
                 self.ispace == other.ispace)
 
     def __hash__(self):
         return super().__hash__()
 
     @property
     def function(self):
@@ -318,14 +320,20 @@
         Compute the distance from ``self`` to ``other``.
 
         Parameters
         ----------
         other : TimedAccess
             The TimedAccess w.r.t. which the distance is computed.
         """
+        if isinstance(self.access, ComponentAccess) and \
+           isinstance(other.access, ComponentAccess) and \
+           self.access.index != other.access.index:
+            # E.g., `uv(x).x` and `uv(x).y` -- not a real dependence!
+            return Vector(S.ImaginaryUnit)
+
         ret = []
         for sit, oit in zip(self.itintervals, other.itintervals):
             n = len(ret)
 
             try:
                 sai = self.aindices[n]
                 oai = other.aindices[n]
@@ -787,19 +795,19 @@
 
     def inplace(self, dim=None):
         """Return the in-place dependences."""
         return DependenceGroup(i for i in self if i.is_inplace(dim))
 
     def __add__(self, other):
         assert isinstance(other, DependenceGroup)
-        return DependenceGroup(super(DependenceGroup, self).__or__(other))
+        return DependenceGroup(super().__or__(other))
 
     def __sub__(self, other):
         assert isinstance(other, DependenceGroup)
-        return DependenceGroup(super(DependenceGroup, self).__sub__(other))
+        return DependenceGroup(super().__sub__(other))
 
     def project(self, function):
         """
         Return a new DependenceGroup retaining only the dependences due to
         the provided function.
         """
         return DependenceGroup(i for i in self if i.function is function)
@@ -808,97 +816,201 @@
 class Scope(object):
 
     def __init__(self, exprs, rules=None):
         """
         A Scope enables data dependence analysis on a totally ordered sequence
         of expressions.
         """
-        exprs = as_tuple(exprs)
-
-        self.reads = {}
-        self.writes = {}
+        self.exprs = as_tuple(exprs)
 
-        self.initialized = set()
+        # A set of rules to drive the collection of dependencies
+        self.rules = as_tuple(rules)
+        assert all(callable(i) for i in self.rules)
 
-        for i, e in enumerate(exprs):
-            # Reads
-            terminals = retrieve_terminals(e.rhs, deep=True, mode='unique')
-            try:
-                terminals.update(retrieve_terminals(e.lhs.indices))
-            except AttributeError:
-                pass
-            for j in terminals:
-                v = self.reads.setdefault(j.function, [])
-                mode = 'RR' if e.is_Reduction and j.function is e.lhs.function else 'R'
-                v.append(TimedAccess(j, mode, i, e.ispace))
-
-            # Write
-            terminals = []
-            if q_terminal(e.lhs):
-                terminals.append(e.lhs)
+    @memoized_generator
+    def writes_gen(self):
+        """
+        Generate all write accesses.
+        """
+        for i, e in enumerate(self.exprs):
+            terminals = retrieve_accesses(e.lhs)
             if q_routine(e.rhs):
                 try:
-                    terminals.extend(e.rhs.writes)
+                    terminals.update(e.rhs.writes)
                 except AttributeError:
                     # E.g., foreign routines, such as `cos` or `sin`
                     pass
             for j in terminals:
-                v = self.writes.setdefault(j.function, [])
-                mode = 'WR' if e.is_Reduction else 'W'
-                v.append(TimedAccess(j, mode, i, e.ispace))
+                if e.is_Reduction:
+                    mode = 'WR'
+                else:
+                    mode = 'W'
+                yield TimedAccess(j, mode, i, e.ispace)
+
+        # Objects altering the control flow (e.g., synchronization barriers,
+        # break statements, ...) are converted into mock dependences
+
+        # Fences (any sort) cannot float around upon topological sorting
+        for i, e in enumerate(self.exprs):
+            if isinstance(e.rhs, Fence):
+                yield TimedAccess(mocksym0, 'W', i, e.ispace)
+
+        # CriticalRegions are stronger than plain Fences.
+        # We must also ensure that none of the Eqs within an opening-closing
+        # CriticalRegion pair floats outside upon topological sorting
+        for i, e in enumerate(self.exprs):
+            if isinstance(e.rhs, CriticalRegion) and e.rhs.opening:
+                for j, e1 in enumerate(self.exprs[i+1:], 1):
+                    if isinstance(e1.rhs, CriticalRegion) and e1.rhs.closing:
+                        break
+                    yield TimedAccess(mocksym1, 'W', i+j, e1.ispace)
+
+    @cached_property
+    def writes(self):
+        """
+        Create a mapper from functions to write accesses.
+        """
+        return as_mapper(self.writes_gen(), key=lambda i: i.function)
+
+    @memoized_generator
+    def reads_explicit_gen(self):
+        """
+        Generate all explicit reads. These are the read accesses to the
+        AbstractFunctions and Symbols appearing in the Scope's symbolic
+        expressions.
+        """
+        for i, e in enumerate(self.exprs):
+            # Reads
+            terminals = retrieve_accesses(e.rhs, deep=True)
+            try:
+                terminals.update(retrieve_accesses(e.lhs.indices))
+            except AttributeError:
+                pass
+            for j in terminals:
+                if j.function is e.lhs.function and e.is_Reduction:
+                    mode = 'RR'
+                else:
+                    mode = 'R'
+                yield TimedAccess(j, mode, i, e.ispace)
 
             # If a reduction, we got one implicit read
             if e.is_Reduction:
-                v = self.reads.setdefault(e.lhs.function, [])
-                v.append(TimedAccess(e.lhs, 'RR', i, e.ispace))
-
-            # If writing to a scalar, we have an initialization
-            if not e.is_Reduction and e.is_scalar:
-                self.initialized.add(e.lhs.function)
+                yield TimedAccess(e.lhs, 'RR', i, e.ispace)
 
             # Look up ConditionalDimensions
             for v in e.conditionals.values():
-                for j in retrieve_terminals(v):
-                    v = self.reads.setdefault(j.function, [])
-                    v.append(TimedAccess(j, 'R', -1, e.ispace))
+                for j in retrieve_accesses(v):
+                    yield TimedAccess(j, 'R', -1, e.ispace)
 
-        # The iteration symbols too
-        dimensions = set().union(*[e.dimensions for e in exprs])
+    @memoized_generator
+    def reads_implicit_gen(self):
+        """
+        Generate all implicit reads. These are for examples the reads accesses
+        to the iteration symbols bounded to the Dimensions used in the Scope's
+        symbolic expressions.
+        """
+        # The iteration symbols
+        dimensions = set().union(*[e.dimensions for e in self.exprs])
+        symbols = set()
         for d in dimensions:
-            for i in d.free_symbols | d.bound_symbols:
-                v = self.reads.setdefault(i.function, [])
-                v.append(TimedAccess(i, 'R', -1))
+            symbols.update(d.free_symbols | d.bound_symbols)
+        for i in symbols:
+            yield TimedAccess(i, 'R', -1)
 
+    @memoized_generator
+    def reads_synchro_gen(self):
+        """
+        Generate all reads due to syncronization operations. These may be explicit
+        or implicit.
+        """
         # Objects altering the control flow (e.g., synchronization barriers,
         # break statements, ...) are converted into mock dependences
-        for i, e in enumerate(exprs):
-            if e.find(Barrier) | e.find(Jump):
-                self.writes.setdefault(mocksym, []).append(
-                    TimedAccess(mocksym, 'W', i, e.ispace)
-                )
-                self.reads.setdefault(mocksym, []).extend([
-                    TimedAccess(mocksym, 'R', max(i, 0), e.ispace),
-                    TimedAccess(mocksym, 'R', i+1, e.ispace),
-                ])
 
-        # A set of rules to drive the collection of dependencies
-        self.rules = as_tuple(rules)
-        assert all(callable(i) for i in self.rules)
+        # Fences (any sort) cannot float around upon topological sorting
+        for i, e in enumerate(self.exprs):
+            if isinstance(e.rhs, Fence):
+                if i > 0:
+                    yield TimedAccess(mocksym0, 'R', i-1, e.ispace)
+                if i < len(self.exprs)-1:
+                    yield TimedAccess(mocksym0, 'R', i+1, e.ispace)
+
+        # CriticalRegions are stronger than plain Fences.
+        # We must also ensure that none of the Eqs within an opening-closing
+        # CriticalRegion pair floats outside upon topological sorting
+        for i, e in enumerate(self.exprs):
+            if isinstance(e.rhs, CriticalRegion):
+                if e.rhs.opening and i > 0:
+                    yield TimedAccess(mocksym1, 'R', i-1, self.exprs[i-1].ispace)
+                elif e.rhs.closing and i < len(self.exprs)-1:
+                    yield TimedAccess(mocksym1, 'R', i+1, self.exprs[i+1].ispace)
+
+    @memoized_generator
+    def reads_gen(self):
+        """
+        Generate all read accesses.
+        """
+        # NOTE: The reason to keep the explicit and implict reads separated
+        # is efficiency. Sometimes we wish to extract all reads to a given
+        # AbstractFunction, and we know that by construction these can't
+        # appear among the implicit reads
+        return chain(self.reads_explicit_gen(),
+                     self.reads_synchro_gen(),
+                     self.reads_implicit_gen())
+
+    @memoized_generator
+    def reads_smart_gen(self, f):
+        """
+        Generate all read access to a given function.
+
+        StencilDimensions, if any, are replaced with their extrema.
+
+        Notes
+        -----
+        The implementation is smart, in the sense that, depending on the
+        given function type, it will not necessarily look everywhere inside
+        the scope to retrieve the corresponding read accesses. Instead, it
+        will only look in the places where the given type is expected to
+        be found. For example, a DiscreteFunction would never appear among
+        the iteration symbols.
+        """
+        if isinstance(f, (Function, Temp, TempArray, TBArray)):
+            for i in chain(self.reads_explicit_gen(), self.reads_synchro_gen()):
+                if f is i.function:
+                    for j in extrema(i.access):
+                        yield TimedAccess(j, i.mode, i.timestamp, i.ispace)
+
+        else:
+            for i in self.reads_gen():
+                if f is i.function:
+                    yield i
+
+    @cached_property
+    def reads(self):
+        """
+        Create a mapper from functions to read accesses.
+        """
+        return as_mapper(self.reads_gen(), key=lambda i: i.function)
+
+    @cached_property
+    def initialized(self):
+        return frozenset(e.lhs.function for e in self.exprs
+                         if not e.is_Reduction and e.is_scalar)
 
     def getreads(self, function):
         return as_tuple(self.reads.get(function))
 
     def getwrites(self, function):
         return as_tuple(self.writes.get(function))
 
     def __getitem__(self, function):
         return self.getwrites(function) + self.getreads(function)
 
     def __repr__(self):
-        tracked = filter_sorted(set(self.reads) | set(self.writes), key=lambda i: i.name)
+        tracked = filter_sorted(set(self.reads) | set(self.writes),
+                                key=lambda i: i.name)
         maxlen = max(1, max([len(i.name) for i in tracked]))
         out = "{:>%d} =>  W : {}\n{:>%d}     R : {}" % (maxlen, maxlen)
         pad = " "*(maxlen + 9)
         reads = [self.getreads(i) for i in tracked]
         for i, r in enumerate(list(reads)):
             if not r:
                 reads[i] = ''
@@ -940,83 +1052,90 @@
                      if a.timestamp in timestamps and a.mode in modes)
 
     @memoized_generator
     def d_flow_gen(self):
         """Generate the flow (or "read-after-write") dependences."""
         for k, v in self.writes.items():
             for w in v:
-                for r in self.reads.get(k, []):
+                for r in self.reads_smart_gen(k):
+                    if any(not rule(w, r) for rule in self.rules):
+                        continue
+
                     dependence = Dependence(w, r)
 
-                    if any(not rule(dependence) for rule in self.rules):
+                    if dependence.is_imaginary:
                         continue
 
                     distance = dependence.distance
                     try:
                         is_flow = distance > 0 or (r.lex_ge(w) and distance == 0)
                     except TypeError:
                         # Non-integer vectors are not comparable.
                         # Conservatively, we assume it is a dependence, unless
                         # it's a read-for-reduction
-                        is_flow = (not dependence.is_imaginary and
-                                   not r.is_read_reduction)
+                        is_flow = not r.is_read_reduction
                     if is_flow:
                         yield dependence
 
     @cached_property
     def d_flow(self):
         """Flow (or "read-after-write") dependences."""
         return DependenceGroup(self.d_flow_gen())
 
     @memoized_generator
     def d_anti_gen(self):
         """Generate the anti (or "write-after-read") dependences."""
         for k, v in self.writes.items():
             for w in v:
-                for r in self.reads.get(k, []):
+                for r in self.reads_smart_gen(k):
+                    if any(not rule(r, w) for rule in self.rules):
+                        continue
+
                     dependence = Dependence(r, w)
 
-                    if any(not rule(dependence) for rule in self.rules):
+                    if dependence.is_imaginary:
                         continue
 
                     distance = dependence.distance
                     try:
                         is_anti = distance > 0 or (r.lex_lt(w) and distance == 0)
                     except TypeError:
                         # Non-integer vectors are not comparable.
                         # Conservatively, we assume it is a dependence, unless
                         # it's a read-for-reduction
-                        is_anti = (not dependence.is_imaginary and
-                                   not r.is_read_reduction)
+                        is_anti = not r.is_read_reduction
                     if is_anti:
                         yield dependence
 
     @cached_property
     def d_anti(self):
         """Anti (or "write-after-read") dependences."""
         return DependenceGroup(self.d_anti_gen())
 
     @memoized_generator
     def d_output_gen(self):
         """Generate the output (or "write-after-write") dependences."""
         for k, v in self.writes.items():
             for w1 in v:
                 for w2 in self.writes.get(k, []):
+                    if any(not rule(w2, w1) for rule in self.rules):
+                        continue
+
                     dependence = Dependence(w2, w1)
 
-                    if any(not rule(dependence) for rule in self.rules):
+                    if dependence.is_imaginary:
                         continue
 
                     distance = dependence.distance
                     try:
                         is_output = distance > 0 or (w2.lex_gt(w1) and distance == 0)
                     except TypeError:
                         # Non-integer vectors are not comparable.
                         # Conservatively, we assume it is a dependence
-                        is_output = not dependence.is_imaginary
+                        is_output = True
                     if is_output:
                         yield dependence
 
     @cached_property
     def d_output(self):
         """Output (or "write-after-write") dependences."""
         return DependenceGroup(self.d_output_gen())
@@ -1035,15 +1154,15 @@
         """
         Generate all flow, anti, and output dependences involving any of
         the given TimedAccess objects.
         """
         accesses = as_tuple(accesses)
         for d in self.d_all_gen():
             for i in accesses:
-                if d.source is i or d.sink is i:
+                if d.source == i or d.sink == i:
                     yield d
                     break
 
     @memoized_meth
     def d_from_access(self, accesses):
         """
         All flow, anti, and output dependences involving any of the given
@@ -1071,7 +1190,151 @@
 
     @cached_property
     def r_all(self):
         """
         All Relations of the Scope.
         """
         return list(self.r_gen())
+
+
+class ExprGeometry(object):
+
+    """
+    Geometric representation of an expression by abstracting Indexeds as
+    LabeledVectors.
+    """
+
+    def __init__(self, expr, indexeds=None, bases=None, offsets=None):
+        self.expr = expr
+
+        if indexeds is not None:
+            self.indexeds = indexeds
+            self.bases = bases
+            self.offsets = offsets
+            return
+
+        self.indexeds = retrieve_indexed(expr)
+
+        bases = []
+        offsets = []
+        for ii in self.iinstances:
+            base = []
+            offset = []
+            for e, fi, ai in zip(ii, ii.findices, ii.aindices):
+                if ai is None:
+                    base.append((fi, e))
+                else:
+                    base.append((fi, ai))
+                    offset.append((ai, e - ai))
+            bases.append(LabeledVector(base))
+            offsets.append(LabeledVector(offset))
+
+        self.bases = bases
+        self.offsets = offsets
+
+    def __repr__(self):
+        return "ExprGeometry(expr=%s)" % self.expr
+
+    def translated(self, other, dims=None):
+        """
+        True if `self` is translated w.r.t. `other`, False otherwise.
+
+        Examples
+        --------
+        Two expressions are translated if they perform the same operations,
+        their bases are the same and their offsets are pairwise translated.
+
+        c := A[i,j] op A[i,j+1]     -> Toffsets = {i: [0,0], j: [0,1]}
+        u := A[i+1,j] op A[i+1,j+1] -> Toffsets = {i: [1,1], j: [0,1]}
+
+        Then `c` is translated w.r.t. `u` with distance `{i: 1, j: 0}`
+
+        The test may be strengthen by imposing that a translation occurs
+        only along a specific set of Dimensions through the kwarg `dims`.
+        """
+        # Check mathematical structure
+        if not compare_ops(self.expr, other.expr):
+            return False
+
+        # Use a suitable value for `dims` if not provided by user
+        if dims is None:
+            if self.aindices != other.aindices:
+                return False
+            dims = self.aindices
+        dims = set(as_tuple(dims))
+
+        # Check bases and offsets
+        for i in ['Tbases', 'Toffsets']:
+            Ti0 = getattr(self, i)
+            Ti1 = getattr(other, i)
+
+            m0 = dict(Ti0)
+            m1 = dict(Ti1)
+
+            # The only hope in presence of Dimensions appearing only in either
+            # `self` or `other` is that they have been projected away by the caller
+            for d in set(m0).symmetric_difference(set(m1)):
+                if not d._defines & dims:
+                    return False
+
+            for d in set(m0).union(set(m1)):
+                try:
+                    o0 = m0[d]
+                    o1 = m1[d]
+                except KeyError:
+                    continue
+
+                distance = set(o0 - o1)
+                if len(distance) != 1:
+                    return False
+
+                if not d._defines & dims:
+                    if distance.pop() != 0:
+                        return False
+
+        return True
+
+    @cached_property
+    def iinstances(self):
+        return tuple(IterationInstance(i) for i in self.indexeds)
+
+    @cached_property
+    def Tbases(self):
+        return LabeledVector.transpose(*self.bases)
+
+    @cached_property
+    def Toffsets(self):
+        return LabeledVector.transpose(*self.offsets)
+
+    @cached_property
+    def dimensions(self):
+        return frozenset(i for i, _ in self.Toffsets)
+
+    @cached_property
+    def aindices(self):
+        try:
+            return tuple(zip(*self.Toffsets))[0]
+        except IndexError:
+            return ()
+
+    @property
+    def is_regular(self):
+        return all(i.is_regular for i in self.iinstances)
+
+
+# *** Utils
+
+def retrieve_accesses(exprs, **kwargs):
+    """
+    Like retrieve_terminals, but ensure that if a ComponentAccess is found,
+    the ComponentAccess itself is returned, while the wrapped Indexed is discarded.
+    """
+    kwargs['mode'] = 'unique'
+
+    compaccs = search(exprs, ComponentAccess)
+    if not compaccs:
+        return retrieve_terminals(exprs, **kwargs)
+
+    subs = {i: Symbol('dummy%d' % n) for n, i in enumerate(compaccs)}
+    exprs1 = uxreplace(exprs, subs)
+
+    return compaccs | retrieve_terminals(exprs1, **kwargs) - set(subs.values())
```

### Comparing `devito-4.8.3/devito/ir/support/guards.py` & `devito-4.8.4/devito/ir/support/guards.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 (e.g., Eq, Cluster, ...) should be evaluated at runtime.
 """
 
 from sympy import And, Ge, Gt, Le, Lt, Mul, true
 
 from devito.ir.support.space import Forward, IterationDirection
 from devito.symbolics import CondEq, CondNe
-from devito.tools import Pickable, as_tuple, frozendict
+from devito.tools import Pickable, as_tuple, frozendict, split
 from devito.types import Dimension
 
 __all__ = ['GuardFactor', 'GuardBound', 'GuardBoundNext', 'BaseGuardBound',
            'BaseGuardBoundNext', 'GuardOverflow', 'Guards']
 
 
 class Guard(object):
@@ -99,34 +99,36 @@
 
 GuardBound = GuardBoundLe
 
 
 # *** GuardBoundNext
 
 
-class BaseGuardBoundNext(Guard):
+class BaseGuardBoundNext(Guard, Pickable):
 
     """
     A guard to avoid out-of-bounds iteration.
 
     Given a Dimension `d` and an IterationDirection `direction`, create a
     symbolic relation that at runtime evaluates to true if
 
         * `next(d) <= d.root.symbolic_max`, with `direction=Forward`
         * `d.root.symbolic_min <= next(d)`, with `direction=Backward`
 
     where `next(d)` represents the next iteration along `d` for the
     given `direction`.
     """
 
+    __rargs__ = ('d', 'direction')
+
     def __new__(cls, d, direction, **kwargs):
         assert isinstance(d, Dimension)
         assert isinstance(direction, IterationDirection)
 
-        if direction is Forward:
+        if direction == Forward:
             p0 = d.root
             p1 = d.root.symbolic_max
 
             if d.is_Conditional:
                 v = d.factor
                 # Round `p0 + 1` up to the nearest multiple of `v`
                 p0 = Mul((((p0 + 1) + v - 1) / v), v, evaluate=False)
@@ -224,15 +226,15 @@
     def andg(self, d, guard):
         m = dict(self)
 
         if guard == true:
             return Guards(m)
 
         try:
-            m[d] = And(m[d], guard)
+            m[d] = simplify_and(m[d], guard)
         except KeyError:
             m[d] = guard
 
         return Guards(m)
 
     def xandg(self, d, guard):
         m = dict(self)
@@ -265,7 +267,49 @@
 
         return Guards(m)
 
     def filter(self, key):
         m = {d: v for d, v in self.items() if key(d)}
 
         return Guards(m)
+
+
+# *** Utils
+
+def simplify_and(relation, v):
+    """
+    Given `x = And(*relation.args, v)`, return `relation` if `x ≡ relation`,
+    `x` otherwise.
+
+    SymPy doesn't have a builtin function to simplify boolean inequalities; here,
+    we run a set of simple checks to at least discard the most obvious (and thus
+    annoying to see in the generated code) redundancies.
+    """
+    if isinstance(relation, And):
+        candidates, other = split(list(relation.args), lambda a: type(a) is type(v))
+    elif type(relation) is type(v):
+        candidates, other = [relation], []
+    else:
+        candidates, other = [], [relation, v]
+
+    covered = False
+    new_args = []
+    for a in candidates:
+        if a.lhs is v.lhs:
+            covered = True
+            try:
+                if type(a) in (Gt, Ge) and v.rhs > a.rhs:
+                    new_args.append(v)
+                elif type(a) in (Lt, Le) and v.rhs < a.rhs:
+                    new_args.append(v)
+                else:
+                    new_args.append(a)
+            except TypeError:
+                # E.g., `v.rhs = const + z_M` and `a.rhs = z_M`, so the inequalities
+                # above are not evaluable to True/False
+                new_args.append(a)
+        else:
+            new_args.append(a)
+    if not covered:
+        new_args.append(v)
+
+    return And(*(new_args + other))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devito-4.8.3/devito/ir/support/properties.py` & `devito-4.8.4/devito/ir/support/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class Property(Tag):
 
     _KNOWN = []
 
     def __init__(self, name, val=None):
-        super(Property, self).__init__(name, val)
+        super().__init__(name, val)
         Property._KNOWN.append(self)
 
 
 SEQUENTIAL = Property('sequential')
 """A sequential Dimension."""
 
 PARALLEL = Property('parallel')
@@ -44,20 +44,14 @@
 Like TILABLE, but it would benefit from relatively small block, since the
 iteration space is likely to be very small.
 """
 
 SKEWABLE = Property('skewable')
 """A fully parallel Dimension that would benefit from wavefront/skewed tiling."""
 
-ROUNDABLE = Property('roundable')
-"""
-A Dimension whose upper limit may be rounded up to a multiple of the SIMD
-vector length thanks to the presence of enough padding.
-"""
-
 AFFINE = Property('affine')
 """
 A Dimension used to index into tensor objects only through affine and regular
 accesses functions. See :mod:`basic.py` for rigorous definitions of "affine"
 and "regular".
 """
 
@@ -126,15 +120,15 @@
     for p in args:
         properties.update(p - drop)
 
     return properties
 
 
 def relax_properties(properties):
-    return frozenset(properties - {PARALLEL_INDEP, ROUNDABLE})
+    return frozenset(properties - {PARALLEL_INDEP})
 
 
 class Properties(frozendict):
 
     """
     A mapper {Dimension -> {properties}}.
     """
@@ -205,20 +199,20 @@
             m[d] = set(m.get(d, [])) | {INBOUND}
         return Properties(m)
 
     def is_parallel(self, dims):
         return any(len(self[d] & {PARALLEL, PARALLEL_INDEP}) > 0
                    for d in as_tuple(dims))
 
-    def is_parallel_atomic(self, dims):
-        return any(len(self[d] & {PARALLEL_IF_ATOMIC}) > 0 for d in as_tuple(dims))
-
     def is_parallel_relaxed(self, dims):
         return any(len(self[d] & PARALLELS) > 0 for d in as_tuple(dims))
 
+    def is_parallel_atomic(self, dims):
+        return any(PARALLEL_IF_ATOMIC in self.get(d, ()) for d in as_tuple(dims))
+
     def is_affine(self, dims):
         return any(AFFINE in self.get(d, ()) for d in as_tuple(dims))
 
     def is_inbound(self, dims):
         return any(INBOUND in self.get(d, ()) for d in as_tuple(dims))
 
     def is_sequential(self, dims):
```

### Comparing `devito-4.8.3/devito/ir/support/space.py` & `devito-4.8.4/devito/ir/support/space.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from collections import OrderedDict
 from functools import reduce
 from operator import mul
 
 from cached_property import cached_property
 from sympy import Expr
 
-from devito.ir.support.utils import sdims_min, sdims_max
+from devito.ir.support.utils import minimum, maximum
 from devito.ir.support.vector import Vector, vmin, vmax
-from devito.tools import (PartialOrderTuple, Stamp, as_list, as_tuple, filter_ordered,
+from devito.tools import (Ordering, Stamp, as_list, as_tuple, filter_ordered,
                           flatten, frozendict, is_integer, toposort)
 from devito.types import Dimension, ModuloDimension
 
 __all__ = ['NullInterval', 'Interval', 'IntervalGroup', 'IterationSpace',
-           'IterationInterval', 'DataSpace', 'Forward', 'Backward', 'Any']
+           'IterationInterval', 'DataSpace', 'Forward', 'Backward', 'Any',
+           'null_ispace']
 
 
 # The default Stamp, used by all new Intervals
 S0 = Stamp()
 
 
 class AbstractInterval(object):
@@ -119,15 +120,15 @@
 
         [dim.symbolic_min + lower, dim.symbolic_max + upper]
     """
 
     is_Defined = True
 
     def __init__(self, dim, lower=0, upper=0, stamp=S0):
-        super(Interval, self).__init__(dim, stamp)
+        super().__init__(dim, stamp)
 
         try:
             self.lower = int(lower)
         except TypeError:
             assert isinstance(lower, Expr)
             self.lower = lower
         try:
@@ -142,15 +143,15 @@
     def __hash__(self):
         return hash((self.dim, self.offsets))
 
     def __eq__(self, o):
         if self is o:
             return True
 
-        return (super(Interval, self).__eq__(o) and
+        return (super().__eq__(o) and
                 self.lower == o.lower and
                 self.upper == o.upper)
 
     def _rebuild(self):
         return Interval(self.dim, self.lower, self.upper, self.stamp)
 
     @property
@@ -282,38 +283,48 @@
             try:
                 return self.switch(self.dim.parent).promote(cond)
             except AttributeError:
                 pass
         return self
 
     def expand(self):
-        return Interval(self.dim, sdims_min(self.lower), sdims_max(self.upper),
-                        self.stamp)
+        return Interval(
+            self.dim, minimum(self.lower), maximum(self.upper), self.stamp
+        )
 
 
-class IntervalGroup(PartialOrderTuple):
+class IntervalGroup(Ordering):
 
     """
-    A partially-ordered sequence of Intervals equipped with set-like
-    operations.
+    A sequence of Intervals equipped with set-like operations.
     """
 
     @classmethod
     def reorder(cls, items, relations):
         if not all(isinstance(i, AbstractInterval) for i in items):
-            raise ValueError("Cannot create an IntervalGroup from objects of type [%s]" %
+            raise ValueError("Cannot create IntervalGroup from objs of type [%s]" %
                              ', '.join(str(type(i)) for i in items))
-        # The relations are between dimensions, not intervals. So we take
-        # care of that here
-        ordering = filter_ordered(toposort(relations) + [i.dim for i in items])
+
+        if len(relations) == 1:
+            # Special case: avoid expensive topological sorting if possible
+            relation, = relations
+            ordering = filter_ordered(list(relation) + [i.dim for i in items])
+        else:
+            ordering = filter_ordered(toposort(relations) + [i.dim for i in items])
+
         return sorted(items, key=lambda i: ordering.index(i.dim))
 
+    @classmethod
+    def simplify_relations(cls, relations, items, mode):
+        if mode == 'total':
+            return [tuple(i.dim for i in items)]
+        else:
+            return super().simplify_relations(relations, items, mode)
+
     def __eq__(self, o):
-        # No need to look at the relations -- if the partial ordering is the same,
-        # then the IntervalGroups are considered equal
         return len(self) == len(o) and all(i == j for i, j in zip(self, o))
 
     def __contains__(self, d):
         return any(i.dim is d for i in self)
 
     def __hash__(self):
         return hash(tuple(self))
@@ -337,29 +348,28 @@
         """
         True if all Intervals are over different Dimensions,
         False otherwise.
         """
         return len(self.dimensions) == len(set(self.dimensions))
 
     @classmethod
-    def generate(self, op, *interval_groups, relations=None):
+    def generate(cls, op, *interval_groups, relations=None):
         """
         Create a new IntervalGroup from the iterative application of an
         operation to some IntervalGroups.
 
         Parameters
         ----------
         op : str
             Any legal Interval operation, such as 'intersection' or
             or 'union'.
         *interval_groups
             Input IntervalGroups.
         relations : tuple, optional
-            Relations to be used in the newly constructed IntervalGroup, in addition
-            to the ones inherited via each element in `interval_groups`.
+            Additional relations to build the new IntervalGroup.
 
         Examples
         --------
         >>> from devito import dimensions
         >>> x, y, z = dimensions('x y z')
         >>> ig0 = IntervalGroup([Interval(x, 1, -1)])
         >>> ig1 = IntervalGroup([Interval(x, 2, -2), Interval(y, 3, -3)])
@@ -379,73 +389,84 @@
             for i in v[1:]:
                 interval = getattr(interval, op)(i)
             intervals.append(interval)
 
         relations = set(as_tuple(relations))
         relations.update(set().union(*[ig.relations for ig in interval_groups]))
 
-        return IntervalGroup(intervals, relations=relations)
+        modes = set(ig.mode for ig in interval_groups)
+        assert len(modes) <= 1
+        try:
+            mode = modes.pop()
+        except KeyError:
+            mode = 'total'
+
+        return IntervalGroup(intervals, relations=relations, mode=mode)
 
     def is_compatible(self, o):
         """
-        Two IntervalGroups are compatible iff they can be ordered according
-        to some common partial ordering.
+        Two IntervalGroups are compatible iff their elements are not subjected
+        to sets of relations that would prevent a reordering.
         """
         if set(self) != set(o):
             return False
         if all(i == j for i, j in zip(self, o)):
             # Same input ordering, definitely compatible
             return True
         try:
             self.add(o)
             return True
         except ValueError:
-            # Cyclic dependence detected, there is no common partial ordering
+            # Cyclic dependence detected
             return False
 
     def _normalize(func):
         """
         A simple decorator to normalize the input of operator methods that
         expect an IntervalGroup as an operand.
         """
         def wrapper(self, o):
             if not isinstance(o, IntervalGroup):
                 o = IntervalGroup(as_tuple(o))
-            return func(self, o)
+            if self.mode != o.mode:
+                raise ValueError("Incompatible ordering modes")
+            relations = self.relations | o.relations
+            return func(self, o, relations, self.mode)
         return wrapper
 
     @_normalize
-    def intersection(self, o):
+    def intersection(self, o, relations, mode):
         mapper = OrderedDict([(i.dim, i) for i in o])
         intervals = [i.intersection(mapper.get(i.dim, i)) for i in self]
-        return IntervalGroup(intervals, relations=(self.relations | o.relations))
+        return IntervalGroup(intervals, relations=relations, mode=mode)
 
     @_normalize
-    def add(self, o):
+    def add(self, o, relations, mode):
         mapper = OrderedDict([(i.dim, i) for i in o])
         intervals = [i.add(mapper.get(i.dim, NullInterval(i.dim))) for i in self]
-        return IntervalGroup(intervals, relations=(self.relations | o.relations))
+        return IntervalGroup(intervals, relations=relations, mode=mode)
 
     @_normalize
-    def subtract(self, o):
+    def subtract(self, o, relations, mode):
         mapper = OrderedDict([(i.dim, i) for i in o])
         intervals = [i.subtract(mapper.get(i.dim, NullInterval(i.dim))) for i in self]
-        return IntervalGroup(intervals, relations=(self.relations | o.relations))
+        return IntervalGroup(intervals, relations=relations, mode=mode)
 
     def relaxed(self, d=None):
         d = set(self.dimensions if d is None else as_tuple(d))
         intervals = [i.relaxed if i.dim in d else i for i in self]
-        return IntervalGroup(intervals, relations=self.relations)
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def promote(self, cond):
-        intervals = IntervalGroup([i.promote(cond) for i in self],
-                                  relations=self.relations)
+        intervals = [i.promote(cond) for i in self]
+        intervals = IntervalGroup(intervals, relations=None, mode='unordered')
 
-        # There could be duplicate Dimensions at this point, so we sum up the Intervals
-        # defined over the same Dimension to produce a well-defined IntervalGroup
+        # There could be duplicate Dimensions at this point, so we sum up the
+        # Intervals defined over the same Dimension to produce a well-defined
+        # IntervalGroup
         intervals = IntervalGroup.generate('add', intervals)
 
         return intervals
 
     def drop(self, d, strict=False):
         # Dropping
         if strict:
@@ -454,63 +475,72 @@
         else:
             dims = set().union(*[i._defines for i in as_tuple(d)])
             intervals = [i._rebuild() for i in self if not i.dim._defines & dims]
 
         # Clean up relations
         relations = [tuple(i for i in r if i not in dims) for r in self.relations]
 
-        return IntervalGroup(intervals, relations=relations)
+        return IntervalGroup(intervals, relations=relations, mode=self.mode)
 
     def negate(self):
-        return IntervalGroup([i.negate() for i in self], relations=self.relations)
+        intervals = [i.negate() for i in self]
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def zero(self, d=None):
         d = self.dimensions if d is None else as_tuple(d)
-        return IntervalGroup([i.zero() if i.dim in d else i for i in self],
-                             relations=self.relations)
+        intervals = [i.zero() if i.dim in d else i for i in self]
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def lift(self, d=None, v=None):
         d = set(self.dimensions if d is None else as_tuple(d))
-        return IntervalGroup([i.lift(v) if i.dim._defines & d else i for i in self],
-                             relations=self.relations)
+        intervals = [i.lift(v) if i.dim._defines & d else i for i in self]
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def reset(self):
-        return IntervalGroup([i.reset() for i in self], relations=self.relations)
+        intervals = [i.reset() for i in self]
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def switch(self, d0, d1):
         intervals = [i.switch(d1) if i.dim is d0 else i for i in self]
 
         # Update relations too
         relations = {tuple(d1 if i is d0 else i for i in r) for r in self.relations}
 
-        return IntervalGroup(intervals, relations=relations)
+        return IntervalGroup(intervals, relations=relations, mode=self.mode)
 
     def translate(self, d, v0=0, v1=None):
-        intervals = [i.translate(v0, v1) if i.dim in as_tuple(d) else i for i in self]
-        return IntervalGroup(intervals, relations=self.relations)
+        dims = as_tuple(d)
+        intervals = [i.translate(v0, v1) if i.dim in dims else i for i in self]
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def expand(self, d=None):
         if d is None:
             d = self.dimensions
         intervals = [i.expand() if i.dim in as_tuple(d) else i for i in self]
-        return IntervalGroup(intervals, relations=self.relations)
+
+        return IntervalGroup(intervals, relations=self.relations, mode=self.mode)
 
     def index(self, key):
         if isinstance(key, Interval):
-            return super(IntervalGroup, self).index(key)
+            return super().index(key)
         elif isinstance(key, Dimension):
-            return super(IntervalGroup, self).index(self[key])
+            return super().index(self[key])
         raise ValueError("Expected Interval or Dimension, got `%s`" % type(key))
 
     def __getitem__(self, key):
         if is_integer(key):
-            return super(IntervalGroup, self).__getitem__(key)
+            return super().__getitem__(key)
         elif isinstance(key, slice):
-            retval = super(IntervalGroup, self).__getitem__(key)
-            return IntervalGroup(retval, relations=self.relations)
+            retval = super().__getitem__(key)
+            return IntervalGroup(retval, relations=self.relations, mode=self.mode)
 
         if not self.is_well_defined:
             raise ValueError("Cannot fetch Interval from ill defined Space")
 
         if not isinstance(key, Dimension):
             return NullInterval(key)
 
@@ -624,14 +654,22 @@
         return tuple(filter_ordered(self.intervals.dimensions))
 
     @property
     def size(self):
         return self.intervals.size
 
     @property
+    def mode(self):
+        return self.intervals.mode
+
+    @property
+    def relations(self):
+        return self.intervals.relations
+
+    @property
     def dimension_map(self):
         """
         Map between the Space Dimensions and the size of their Interval.
         """
         return OrderedDict([(i.dim, i.size) for i in self.intervals])
 
 
@@ -646,25 +684,26 @@
         Data space description.
     parts : dict, optional
         A mapper from Functions to IntervalGroup, describing the individual
         components of the data space.
     """
 
     def __init__(self, intervals, parts=None):
-        super(DataSpace, self).__init__(intervals)
+        super().__init__(intervals)
 
         parts = {k: v.expand() for k, v in (parts or {}).items()}
         self._parts = frozendict(parts)
 
     def __eq__(self, other):
-        return isinstance(other, DataSpace) and\
-            self.intervals == other.intervals and self.parts == other.parts
+        return (isinstance(other, DataSpace) and
+                self.intervals == other.intervals and
+                self.parts == other.parts)
 
     def __hash__(self):
-        return hash((super(DataSpace, self).__hash__(), self.parts))
+        return hash((super().__hash__(), self.parts))
 
     @classmethod
     def union(cls, *others):
         if not others:
             return DataSpace(IntervalGroup(), {})
 
         intervals = IntervalGroup.generate('union', *[i.intervals for i in others])
@@ -710,15 +749,15 @@
         A mapper from Dimensions in ``intervals`` to iterables of
         DerivedDimensions defining sub-regions of iteration.
     directions : dict, optional
         A mapper from Dimensions in ``intervals`` to IterationDirections.
     """
 
     def __init__(self, intervals, sub_iterators=None, directions=None):
-        super(IterationSpace, self).__init__(intervals)
+        super().__init__(intervals)
 
         # Normalize sub-iterators
         sub_iterators = dict([(k, tuple(filter_ordered(as_tuple(v))))
                               for k, v in (sub_iterators or {}).items()])
         sub_iterators.update({i.dim: () for i in self.intervals
                               if i.dim not in sub_iterators})
         self._sub_iterators = frozendict(sub_iterators)
@@ -745,15 +784,15 @@
     def __lt__(self, other):
         """
         A rudimentary less-then comparison between two IterationSpaces.
         """
         return len(self.itintervals) < len(other.itintervals)
 
     def __hash__(self):
-        return hash((super(IterationSpace, self).__hash__(), self.sub_iterators,
+        return hash((super().__hash__(), self.sub_iterators,
                      self.directions))
 
     def __contains__(self, d):
         try:
             self[d]
             return True
         except KeyError:
@@ -767,15 +806,15 @@
             d = v.dim
             return IterationInterval(v, self.sub_iterators[d], self.directions[d])
 
     @classmethod
     def generate(self, op, *others, relations=None):
         if not others:
             return IterationSpace(IntervalGroup())
-        elif len(others) == 1:
+        elif len(others) == 1 and not relations:
             return others[0]
 
         intervals = [i.intervals for i in others]
         intervals = IntervalGroup.generate(op, *intervals, relations=relations)
 
         directions = {}
         for i in others:
@@ -854,16 +893,20 @@
             func = cond
         else:
             func = lambda i: i in cond
 
         dims = [i.dim for i in self if not func(i.dim)]
         intervals = self.intervals.drop(dims, strict=strict)
 
-        sub_iterators = {k: v for k, v in self.sub_iterators.items() if func(k)}
-        directions = {k: v for k, v in self.directions.items() if func(k)}
+        sub_iterators = {}
+        directions = {}
+        for i in intervals:
+            d = i.dim
+            sub_iterators[d] = self.sub_iterators[d]
+            directions[d] = self.directions[d]
 
         return IterationSpace(intervals, sub_iterators, directions)
 
     def zero(self, d=None):
         intervals = self.intervals.zero(d)
 
         return IterationSpace(intervals, self.sub_iterators, self.directions)
@@ -900,43 +943,75 @@
         sub_iterators = {i.promote(cond).dim: self.sub_iterators[i.dim]
                          for i in self.intervals}
         directions = {i.promote(cond).dim: self.directions[i.dim]
                       for i in self.intervals}
 
         return IterationSpace(intervals, sub_iterators, directions)
 
+    def prefix(self, key):
+        """
+        Return the IterationSpace up to and including the last Interval
+        such that `key(interval)` is True.
+        """
+        try:
+            i = self.project(key)[-1]
+        except IndexError:
+            return None
+
+        return self[:self.index(i.dim) + 1]
+
+    def reorder(self, relations=None, mode=None):
+        relations = relations or self.relations
+        mode = mode or self.mode
+        intervals = IntervalGroup(self.intervals, relations=relations, mode=mode)
+
+        return IterationSpace(intervals, self.sub_iterators, self.directions)
+
+    def is_subset(self, other):
+        """
+        True if `self` is included within `other`, False otherwise.
+        """
+        if not self:
+            return True
+
+        d = self[-1].dim
+        try:
+            return self == other[:other.index(d) + 1]
+        except ValueError:
+            return False
+
     def is_compatible(self, other):
         """
         A relaxed version of ``__eq__``, in which only non-derived dimensions
         are compared for equality.
         """
         return (self.intervals.is_compatible(other.intervals) and
                 self.nonderived_directions == other.nonderived_directions)
 
     @property
-    def itdimensions(self):
+    def itdims(self):
         return self.intervals.dimensions
 
     @property
-    def relations(self):
-        return self.intervals.relations
-
-    @property
     def sub_iterators(self):
         return self._sub_iterators
 
     @property
     def directions(self):
         return self._directions
 
     @cached_property
     def itintervals(self):
-        return tuple(self[d] for d in self.itdimensions)
+        return tuple(self[d] for d in self.itdims)
 
     @cached_property
     def dimensions(self):
         sub_dims = flatten(i._defines for v in self.sub_iterators.values() for i in v)
-        return tuple(filter_ordered(self.itdimensions + tuple(sub_dims)))
+        r_dims = flatten(i._defines for v in self.relations for i in v)
+        return tuple(filter_ordered(self.itdims + tuple(sub_dims) + tuple(r_dims)))
 
     @cached_property
     def nonderived_directions(self):
         return {k: v for k, v in self.directions.items() if not k.is_Derived}
+
+
+null_ispace = IterationSpace([])
```

### Comparing `devito-4.8.3/devito/ir/support/symregistry.py` & `devito-4.8.4/devito/ir/support/symregistry.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/ir/support/syncs.py` & `devito-4.8.4/devito/ir/support/syncs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/ir/support/utils.py` & `devito-4.8.4/devito/ir/support/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from collections import defaultdict
+from collections import defaultdict, namedtuple
+from itertools import product
 
-from devito.symbolics import CallFromPointer, retrieve_indexed, retrieve_terminals
+from devito.finite_differences import IndexDerivative
+from devito.symbolics import (CallFromPointer, retrieve_indexed, retrieve_terminals,
+                              search)
 from devito.tools import DefaultOrderedDict, as_tuple, flatten, filter_sorted, split
 from devito.types import (Dimension, DimensionTuple, Indirection, ModuloDimension,
                           StencilDimension)
 
 __all__ = ['AccessMode', 'Stencil', 'IMask', 'detect_accesses', 'detect_io',
-           'pull_dims', 'sdims_min', 'sdims_max']
+           'pull_dims', 'unbounded', 'minimum', 'maximum', 'minmax_index',
+           'extrema', 'erange']
 
 
 class AccessMode(object):
 
     """
     A descriptor for access modes (read, write, ...).
     """
@@ -259,38 +263,116 @@
     """
     Extract all Dimensions from one or more expressions. If `flag=True`
     (default), all of the ancestor and descendant Dimensions are extracted
     as well.
     """
     dims = set()
     for e in as_tuple(exprs):
-        dims.update({i for i in e.free_symbols if i.is_Dimension})
+        dims.update({i for i in e.free_symbols if isinstance(i, Dimension)})
     if flag:
         return set().union(*[d._defines for d in dims])
     else:
         return dims
 
 
 # *** Utility functions for expressions that potentially contain StencilDimensions
 
-def sdims_min(expr):
+def unbounded(expr):
     """
-    Replace all StencilDimensions in `expr` with their minimum point.
+    Retrieve all unbounded Dimensions in `expr`.
     """
-    try:
-        sdims = expr.find(StencilDimension)
-    except AttributeError:
-        return expr
-    mapper = {e: e._min for e in sdims}
-    return expr.subs(mapper)
+    # At the moment we only have logic to retrieve unbounded StencilDimensions,
+    # but in the future this might change
+    bound = set().union(*[i.dimensions for i in search(expr, IndexDerivative)])
+    sdims = search(expr, StencilDimension, mode='unique', deep=True)
+
+    return sdims - bound
+
+
+Extrema = namedtuple('Extrema', 'm M')
 
 
-def sdims_max(expr):
+def _relational(expr, callback, udims=None):
     """
-    Replace all StencilDimensions in `expr` with their maximum point.
+    Helper for `minimum`, `maximum`, and potential future utilities that share
+    a significant chunk of logic.
     """
-    try:
-        sdims = expr.find(StencilDimension)
-    except AttributeError:
+    if not udims:
+        udims = unbounded(expr)
+
+    # Resolution rule 1: StencilDimensions
+    sdims = [d for d in udims if d.is_Stencil]
+    if not sdims:
         return expr
-    mapper = {e: e._max for e in sdims}
+    mapper = {e: callback(e) for e in sdims}
+
     return expr.subs(mapper)
+
+
+def minimum(expr, udims=None, ispace=None):
+    """
+    Substitute the unbounded Dimensions in `expr` with their minimum point.
+
+    Unbounded Dimensions whose possible minimum value is not known are ignored.
+    """
+    def callback(sd):
+        try:
+            return sd._min + ispace[sd].lower
+        except (TypeError, KeyError):
+            return sd._min
+
+    return _relational(expr, callback, udims)
+
+
+def maximum(expr, udims=None, ispace=None):
+    """
+    Substitute the unbounded Dimensions in `expr` with their maximum point.
+
+    Unbounded Dimensions whose possible maximum value is not known are ignored.
+    """
+    def callback(sd):
+        try:
+            return sd._max + ispace[sd].upper
+        except (TypeError, KeyError):
+            return sd._max
+
+    return _relational(expr, callback, udims)
+
+
+def extrema(expr, ispace=None):
+    """
+    The minimum and maximum extrema assumed by `expr` once the unbounded
+    Dimensions are resolved.
+    """
+    return Extrema(minimum(expr, ispace=ispace), maximum(expr, ispace=ispace))
+
+
+def minmax_index(expr, d):
+    """
+    Return the minimum and maximum indices along the `d` Dimension
+    among all Indexeds in `expr`.
+    """
+    indices = set()
+    for i in retrieve_indexed(expr):
+        try:
+            indices.add(i.indices[d])
+        except KeyError:
+            pass
+
+    return Extrema(min(minimum(i) for i in indices),
+                   max(maximum(i) for i in indices))
+
+
+def erange(expr):
+    """
+    All possible values that `expr` can assume once its unbounded Dimensions
+    are resolved.
+    """
+    udims = unbounded(expr)
+    if not udims:
+        return (expr,)
+
+    sdims = [d for d in udims if d.is_Stencil]
+    ranges = [i.range for i in sdims]
+    mappers = [dict(zip(sdims, i)) for i in product(*ranges)]
+
+    return tuple(expr.subs(m) for m in mappers)
```

### Comparing `devito-4.8.3/devito/ir/support/vector.py` & `devito-4.8.4/devito/ir/support/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Raises
     ------
     TypeError
         If two Vectors cannot be compared, e.g. due to incomparable symbolic entries.
     """
 
     def __new__(cls, *items, smart=False):
-        obj = super(Vector, cls).__new__(cls, items)
+        obj = super().__new__(cls, items)
         obj.smart = smart
         return obj
 
     def _asvector(relax=False):
         def __asvector(func):
             def wrapper(self, other):
                 if not isinstance(other, Vector):
@@ -66,15 +66,15 @@
                 if relax is False and len(self) != len(other):
                     raise TypeError("Cannot operate with Vectors of different rank")
                 return func(self, other)
             return wrapper
         return __asvector
 
     def __hash__(self):
-        return super(Vector, self).__hash__()
+        return super().__hash__()
 
     @_asvector()
     def __add__(self, other):
         return Vector(*[i + j for i, j in zip(self, other)], smart=self.smart)
 
     @_asvector()
     def __radd__(self, other):
@@ -86,19 +86,19 @@
 
     @_asvector()
     def __rsub__(self, other):
         return self - other
 
     @_asvector(relax=True)
     def __eq__(self, other):
-        return super(Vector, self).__eq__(other)
+        return super().__eq__(other)
 
     @_asvector(relax=True)
     def __ne__(self, other):
-        return super(Vector, self).__ne__(other)
+        return super().__ne__(other)
 
     def __lt__(self, other):
         # This might raise an exception if the distance between the i-th entry
         # of `self` and `other` isn't integer, but rather a generic expression
         # not comparable to 0. However, the implementation is "smart", in the
         # sense that it will return as soon as the first two comparable entries
         # (i.e., such that their distance is a non-zero integer) are found
@@ -206,15 +206,15 @@
         return True
 
     @_asvector()
     def __ge__(self, other):
         return other.__le__(self)
 
     def __getitem__(self, key):
-        ret = super(Vector, self).__getitem__(key)
+        ret = super().__getitem__(key)
         return Vector(*ret, smart=self.smart) if isinstance(key, slice) else ret
 
     def __repr__(self):
         return "(%s)" % ','.join(str(i) for i in self)
 
     @property
     def rank(self):
@@ -273,15 +273,15 @@
         try:
             labels, values = zip(*items)
         except (ValueError, TypeError):
             labels, values = (), ()
         if not all(isinstance(i, Dimension) for i in labels):
             raise ValueError("All labels must be of type Dimension, got [%s]"
                              % ','.join(i.__class__.__name__ for i in labels))
-        obj = super(LabeledVector, cls).__new__(cls, *values)
+        obj = super().__new__(cls, *values)
         obj.labels = labels
         return obj
 
     @classmethod
     def transpose(cls, *vectors):
         """
         Transpose a matrix represented as an iterable of homogeneous LabeledVectors.
@@ -302,41 +302,41 @@
 
     def __hash__(self):
         return hash((tuple(self), self.labels))
 
     def __eq__(self, other):
         if isinstance(other, LabeledVector) and self.labels != other.labels:
             raise TypeError("Cannot compare due to mismatching `labels`")
-        return super(LabeledVector, self).__eq__(other)
+        return super().__eq__(other)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __lt__(self, other):
         if isinstance(other, LabeledVector) and self.labels != other.labels:
             raise TypeError("Cannot compare due to mismatching `labels`")
-        return super(LabeledVector, self).__lt__(other)
+        return super().__lt__(other)
 
     def __gt__(self, other):
         return other.__lt__(self)
 
     def __ge__(self, other):
         return self.__eq__(other) or self.__gt__(other)
 
     def __le__(self, other):
         return self.__eq__(other) or self.__lt__(other)
 
     def __getitem__(self, index):
         if isinstance(index, (slice, int)):
-            return super(LabeledVector, self).__getitem__(index)
+            return super().__getitem__(index)
         elif isinstance(index, Dimension):
             for d in self.labels:
                 if d._defines & index._defines:
                     i = self.labels.index(d)
-                    return super(LabeledVector, self).__getitem__(i)
+                    return super().__getitem__(i)
             return None
         else:
             raise TypeError("Indices must be integers, slices, or Dimensions, not %s"
                             % type(index))
 
     def fromlabel(self, label, v=None):
         return self[label] if label in self.labels else v
```

### Comparing `devito-4.8.3/devito/logger.py` & `devito-4.8.4/devito/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The Devito logger."""
 
 import logging
 import sys
 from contextlib import contextmanager
 
-__all__ = ('set_log_level', 'set_log_noperf', 'is_log_enabled_for',
-           'log', 'warning', 'error', 'perf', 'perf_adv',
+__all__ = ('set_log_level', 'set_log_noperf', 'is_log_enabled_for', 'switch_log_level',
+           'log', 'warning', 'error', 'perf', 'hint',
            'RED', 'GREEN', 'BLUE')
 
 
 logger = logging.getLogger('Devito')
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
@@ -67,29 +67,50 @@
     ----------
     level : int
         The logging level. Accepted values are: ``DEBUG, PERF, INFO, WARNING,
         ERROR, CRITICAL``.
     comm : MPI communicator, optional
         An MPI communicator the logger should be collective over. If provided, only
         rank-0 on that communicator will write to the registered handlers, other
-        ranks will use a `logging.NullHandler`.  By default, ``comm`` is set
-        to ``None``, so all ranks will use the default handlers.  This could be
+        ranks will use a `logging.NullHandler`. By default, ``comm`` is set
+        to ``None``, so all ranks will use the default handlers. This could be
         used, for example, if one wants to log to one file per rank.
     """
     from devito import configuration
 
-    if comm is not None:
+    if comm is not None and configuration['mpi']:
         if comm.rank != 0:
             logger.removeHandler(stream_handler)
             logger.addHandler(logging.NullHandler())
+    else:
+        logger.addHandler(stream_handler)
 
     # Triggers a callback to `_set_log_level`
     configuration['log-level'] = level
 
 
+class switch_log_level(object):
+    """
+    A context manager to temporarily change MPI logging.
+    """
+
+    def __init__(self, comm):
+
+        from devito import configuration
+        self.level = configuration['log-level']
+        self.comm = comm
+
+    def __enter__(self):
+        # Limit logging to rank 0
+        set_log_level(self.level, self.comm)
+
+    def __exit__(self, *args):
+        set_log_level(self.level)
+
+
 def set_log_noperf():
     """Do not print performance-related messages."""
     logger.setLevel(WARNING)
 
 
 def is_log_enabled_for(level):
     """
@@ -120,16 +141,16 @@
     log(msg, INFO, *args, **kwargs)
 
 
 def perf(msg, *args, **kwargs):
     log(msg, PERF, *args, **kwargs)
 
 
-def perf_adv(msg, *args, **kwargs):
-    log("Potential optimisation missed: %s" % msg, PERF, *args, **kwargs)
+def hint(msg, *args, **kwargs):
+    log("Hint: %s" % msg, PERF, *args, **kwargs)
 
 
 def warning(msg, *args, **kwargs):
     log(msg, WARNING, *args, **kwargs)
 
 
 def error(msg, *args, **kwargs):
```

### Comparing `devito-4.8.3/devito/mpatches/rationaltools.py` & `devito-4.8.4/devito/mpatches/rationaltools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/mpi/distributed.py` & `devito-4.8.4/devito/mpi/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 import numpy as np
 from cgen import Struct, Value
 
 from devito.data import LEFT, CENTER, RIGHT, Decomposition
 from devito.parameters import configuration
 from devito.tools import EnrichedTuple, as_tuple, ctypes_to_cstr, filter_ordered
 from devito.types import CompositeObject, Object
+from devito.types.utils import DimensionTuple
 
 
+__all__ = ['CustomTopology']
+
 # Do not prematurely initialize MPI
 # This allows launching a Devito program from within another Python program
 # that has *already* initialized MPI
 try:
     import mpi4py
     mpi4py.rc(initialize=False, finalize=False)
     from mpi4py import MPI  # noqa
@@ -53,15 +56,15 @@
         def _sizeof(obj):
             return None
 
         def __getattr__(self, name):
             return None
 
 
-__all__ = ['Distributor', 'SparseDistributor', 'MPI']
+__all__ = ['Distributor', 'SparseDistributor', 'MPI', 'CustomTopology']
 
 
 class AbstractDistributor(ABC):
 
     """
     Decompose a set of Dimensions over a set of MPI processes.
 
@@ -122,15 +125,16 @@
     def glb_shape(self):
         """Shape of the decomposed domain."""
         return EnrichedTuple(*self._glb_shape, getters=self.dimensions)
 
     @property
     def shape(self):
         """The calling MPI rank's local shape."""
-        return tuple(len(i) for i in self.glb_numb)
+        return DimensionTuple(*[len(i) for i in self.glb_numb],
+                              getters=self.dimensions)
 
     @property
     def dimensions(self):
         """The decomposed Dimensions."""
         return self._dimensions
 
     @cached_property
@@ -179,15 +183,15 @@
         The domain Dimensions.
     comm : MPI communicator, optional
         The set of processes over which the domain is distributed. Defaults to
         MPI.COMM_WORLD.
     """
 
     def __init__(self, shape, dimensions, input_comm=None, topology=None):
-        super(Distributor, self).__init__(shape, dimensions)
+        super().__init__(shape, dimensions)
 
         if configuration['mpi']:
             # First time we enter here, we make sure MPI is initialized
             if not MPI.Is_initialized():
                 MPI.Init()
                 global init_by_devito
                 init_by_devito = True
@@ -251,14 +255,24 @@
     def nprocs(self):
         if self.comm is not MPI.COMM_NULL:
             return self.comm.size
         else:
             return 1
 
     @property
+    def nprocs_local(self):
+        if self.comm is not MPI.COMM_NULL:
+            local_comm = MPI.Comm.Split_type(self.comm, MPI.COMM_TYPE_SHARED)
+            node_size = local_comm.Get_size()
+            local_comm.Free()
+            return node_size
+        else:
+            return 1
+
+    @property
     def topology(self):
         return self._topology
 
     @property
     def topology_logical(self):
         if isinstance(self.topology, CustomTopology):
             return self.topology.logical
@@ -420,15 +434,15 @@
     dimensions : tuple of Dimensions
         The decomposed Dimensions.
     distributor : Distributor
         The domain decomposition the SparseDistributor depends on.
     """
 
     def __init__(self, npoint, dimension, distributor):
-        super(SparseDistributor, self).__init__(npoint, dimension)
+        super().__init__(npoint, dimension)
         self._distributor = distributor
 
         # The dimension decomposition
         decomposition = SparseDistributor.decompose(npoint, distributor)
         offs = np.concatenate([[0], np.cumsum(decomposition)])
         self._decomposition = [Decomposition([np.arange(offs[i], offs[i+1])
                                               for i in range(self.nprocs)], self.myrank)]
@@ -517,15 +531,15 @@
 
     def __init__(self, neighborhood):
         self._neighborhood = neighborhood
 
         self._entries = [i for i in neighborhood if isinstance(i, tuple)]
 
         fields = [(''.join(j.name[0] for j in i), c_int) for i in self.entries]
-        super(MPINeighborhood, self).__init__('nb', 'neighborhood', fields)
+        super().__init__('nb', 'neighborhood', fields)
 
     @property
     def entries(self):
         return self._entries
 
     @property
     def neighborhood(self):
@@ -546,15 +560,15 @@
         # With this override, we generate the one on the right
         groups = [list(g) for k, g in groupby(self.pfields, key=lambda x: x[0][0])]
         groups = [(j[0], i) for i, j in [zip(*g) for g in groups]]
         return Struct(self.pname, [Value(ctypes_to_cstr(i), ', '.join(j))
                                    for i, j in groups])
 
     def _arg_defaults(self):
-        values = super(MPINeighborhood, self)._arg_defaults()
+        values = super()._arg_defaults()
         for name, i in zip(self.fields, self.entries):
             setattr(values[self.name]._obj, name, self.neighborhood[i])
         return values
 
     def _arg_values(self, *args, **kwargs):
         grid = kwargs.get('grid', None)
         # Update `nb` based on object attached to `grid`
```

### Comparing `devito-4.8.3/devito/mpi/halo_scheme.py` & `devito-4.8.4/devito/mpi/halo_scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sympy
 
 from devito import configuration
 from devito.data import CORE, OWNED, LEFT, CENTER, RIGHT
 from devito.ir.support import Forward, Scope
 from devito.symbolics.manipulation import _uxreplace_registry
 from devito.tools import (Reconstructable, Tag, as_tuple, filter_ordered, flatten,
-                          frozendict, is_integer)
+                          frozendict, is_integer, filter_sorted)
 from devito.types import Grid
 
 __all__ = ['HaloScheme', 'HaloSchemeEntry', 'HaloSchemeException', 'HaloTouch']
 
 
 class HaloSchemeException(Exception):
     pass
@@ -103,15 +103,15 @@
                 self._mapper == other._mapper and
                 self._honored == other._honored)
 
     def __len__(self):
         return len(self._mapper)
 
     def __hash__(self):
-        return (self._mapper.__hash__(), self.honored.__hash__())
+        return hash((self._mapper.__hash__(), self.honored.__hash__()))
 
     @classmethod
     def build(cls, fmapper, honored):
         obj = object.__new__(HaloScheme)
         obj._mapper = frozendict(fmapper)
         obj._honored = frozendict(honored)
         return obj
@@ -283,15 +283,16 @@
 
         Notes
         -----
         For each Function, the '^' and 'o' are exactly the same on *all MPI
         ranks*, so the output of this method is guaranteed to be consistent
         across *all MPI ranks*.
         """
-        items = [((d, CENTER), (d, LEFT), (d, RIGHT)) for d in self.dimensions]
+        items = [((d, CENTER), (d, LEFT), (d, RIGHT))
+                 for d in filter_sorted(self.dimensions)]
 
         processed = []
         for item in product(*items):
             where = []
             mapper = {}
             for d, s in item:
                 osl, osr = self.owned_size[d]
@@ -578,21 +579,29 @@
 
     __str__ = __repr__
 
     def _sympystr(self, printer):
         return str(self)
 
     def __hash__(self):
-        return id(self)
+        return hash(self.halo_scheme)
 
     def __eq__(self, other):
         return isinstance(other, HaloTouch) and self.halo_scheme == other.halo_scheme
 
     func = Reconstructable._rebuild
 
+    @property
+    def fmapper(self):
+        return self.halo_scheme.fmapper
+
+    @property
+    def dims(self):
+        return frozenset().union(*[v.dims for v in self.fmapper.values()])
+
 
 def _uxreplace_dispatch_haloscheme(hs0, rule):
     changed = False
     hs = hs0
     for f, hse0 in hs0.fmapper.items():
         # Is it an attempt to replace `f`?
         for i, v in rule.items():
```

### Comparing `devito-4.8.3/devito/mpi/routines.py` & `devito-4.8.4/devito/mpi/routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from sympy import Integer
 
 from devito.data import OWNED, HALO, NOPAD, LEFT, CENTER, RIGHT
 from devito.ir.equations import DummyEq
 from devito.ir.iet import (Call, Callable, Conditional, ElementalFunction,
                            Expression, ExpressionBundle, AugmentedExpression,
                            Iteration, List, Prodder, Return, make_efunc, FindNodes,
-                           Transformer, ElementalCall)
+                           Transformer, ElementalCall, CommCallable)
 from devito.mpi import MPI
 from devito.symbolics import (Byref, CondNe, FieldFromPointer, FieldFromComposite,
                               IndexedPointer, Macro, cast_mapper, subs_op_args)
 from devito.tools import (as_mapper, dtype_to_mpitype, dtype_len, dtype_to_ctype,
                           flatten, generator, is_integer, split)
-from devito.types import (Array, Bundle, Dimension, Eq, Symbol, LocalObject,
+from devito.types import (Array, Bag, Dimension, Eq, Symbol, LocalObject,
                           CompositeObject, CustomDimension)
 
 __all__ = ['HaloExchangeBuilder', 'mpi_registry']
 
 
 class HaloExchangeBuilder(object):
 
@@ -287,30 +287,30 @@
     """
 
     def _make_bundles(self, hs):
         halo_scheme = hs.halo_scheme
 
         mapper = as_mapper(halo_scheme.fmapper, lambda i: halo_scheme.fmapper[i])
         for hse, components in mapper.items():
-            # We recast everything as Bundles for simplicity -- worst case scenario
-            # all Bundles only have one component. Existing Bundles are preserved
+            # We recast everything as Bags for simplicity -- worst case scenario
+            # all Bags only have one component. Existing Bundles are preserved
             halo_scheme = halo_scheme.drop(components)
             bundles, candidates = split(tuple(components), lambda i: i.is_Bundle)
             for b in bundles:
                 halo_scheme = halo_scheme.add(b, hse)
 
             try:
-                name = "bundle_%s" % "".join(f.name for f in candidates)
-                bundle = Bundle(name=name, components=candidates)
-                halo_scheme = halo_scheme.add(bundle, hse)
+                name = "bag_%s" % "".join(f.name for f in candidates)
+                bag = Bag(name=name, components=candidates)
+                halo_scheme = halo_scheme.add(bag, hse)
             except ValueError:
                 for i in candidates:
-                    name = "bundle_%s" % i.name
-                    bundle = Bundle(name=name, components=i)
-                    halo_scheme = halo_scheme.add(bundle, hse)
+                    name = "bag_%s" % i.name
+                    bag = Bag(name=name, components=i)
+                    halo_scheme = halo_scheme.add(bag, hse)
 
         hs = hs._rebuild(halo_scheme=halo_scheme)
 
         return hs
 
     def _make_msg(self, f, hse, key):
         return
@@ -358,21 +358,25 @@
 
         if swap is False:
             swap = lambda i, j: (i, j)
             name = 'gather%s' % key
         else:
             swap = lambda i, j: (j, i)
             name = 'scatter%s' % key
-        for i, c in enumerate(f.components):
-            eqns.append(Eq(*swap(buf[[i] + bdims], c[findices])))
+        if isinstance(f, Bag):
+            for i, c in enumerate(f.components):
+                eqns.append(Eq(*swap(buf[[i] + bdims], c[findices])))
+        else:
+            for i in range(f.ncomp):
+                eqns.append(Eq(*swap(buf[[i] + bdims], f[[i] + findices])))
 
         # Compile `eqns` into an IET via recursive compilation
         irs, _ = self.rcompile(eqns)
 
-        parameters = [buf] + bshape + list(f.components) + ofs
+        parameters = [buf] + bshape + list(f.handles) + ofs
 
         return CopyBuffer(name, irs.uiet, parameters)
 
     def _make_sendrecv(self, f, hse, key, **kwargs):
         comm = f.grid.distributor._obj_comm
 
         dims = [d.root for d in f.dimensions if d not in hse.loc_indices]
@@ -387,17 +391,17 @@
         ofss = [Symbol(name='os%s' % d.root) for d in f.dimensions]
 
         fromrank = Symbol(name='fromrank')
         torank = Symbol(name='torank')
 
         shape = [d.symbolic_size for d in dims]
 
-        arguments = [bufg] + shape + list(f.components) + ofsg
+        arguments = [bufg] + shape + list(f.handles) + ofsg
         gather = Gather('gather%s' % key, arguments)
-        arguments = [bufs] + shape + list(f.components) + ofss
+        arguments = [bufs] + shape + list(f.handles) + ofss
         scatter = Scatter('scatter%s' % key, arguments)
 
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
@@ -411,21 +415,21 @@
                          torank, Integer(13), comm, Byref(rsend)])
 
         waitrecv = Call('MPI_Wait', [Byref(rrecv), Macro('MPI_STATUS_IGNORE')])
         waitsend = Call('MPI_Wait', [Byref(rsend), Macro('MPI_STATUS_IGNORE')])
 
         iet = List(body=[recv, gather, send, waitsend, waitrecv, scatter])
 
-        parameters = (list(f.components) + shape + ofsg + ofss +
+        parameters = (list(f.handles) + shape + ofsg + ofss +
                       [fromrank, torank, comm])
 
         return SendRecv('sendrecv%s' % key, iet, parameters, bufg, bufs)
 
     def _call_sendrecv(self, name, *args, **kwargs):
-        args = list(args[0].components) + flatten(args[1:])
+        args = list(args[0].handles) + flatten(args[1:])
         return Call(name, args)
 
     def _make_haloupdate(self, f, hse, key, sendrecv, **kwargs):
         distributor = f.grid.distributor
         nb = distributor._obj_neighborhood
         comm = distributor._obj_comm
 
@@ -471,22 +475,22 @@
                 rsizes, rofs = mapper[(d, RIGHT, OWNED)]
                 lsizes, lofs = mapper[(d, LEFT, HALO)]
                 args = [f, rsizes, rofs, lofs, lpeer, rpeer, comm]
                 body.append(self._call_sendrecv(sendrecv.name, *args, **kwargs))
 
         iet = List(body=body)
 
-        parameters = list(f.components) + [comm, nb] + list(fixed.values())
+        parameters = list(f.handles) + [comm, nb] + list(fixed.values())
 
         return HaloUpdate('haloupdate%s' % key, iet, parameters)
 
     def _call_haloupdate(self, name, f, hse, *args):
         comm = f.grid.distributor._obj_comm
         nb = f.grid.distributor._obj_neighborhood
-        args = list(f.components) + [comm, nb] + list(hse.loc_indices.values())
+        args = list(f.handles) + [comm, nb] + list(hse.loc_indices.values())
         return HaloUpdateCall(name, flatten(args))
 
     def _make_compute(self, *args):
         return
 
     def _make_poke(self, *args):
         return
@@ -563,15 +567,15 @@
             kwargs['haloid'] = len(body)
 
             body.append(self._call_sendrecv(sendrecv.name, f, sizes, ofsg, ofss,
                                             fromrank, torank, comm, **kwargs))
 
         iet = List(body=body)
 
-        parameters = list(f.components) + [comm, nb] + list(fixed.values())
+        parameters = list(f.handles) + [comm, nb] + list(fixed.values())
 
         return HaloUpdate('haloupdate%s' % key, iet, parameters)
 
 
 class ComputeCall(ElementalCall):
     pass
 
@@ -610,40 +614,40 @@
 
         fromrank = Symbol(name='fromrank')
         torank = Symbol(name='torank')
 
         sizes = [FieldFromPointer('%s[%d]' % (msg._C_field_sizes, i), msg)
                  for i in range(len(f._dist_dimensions))]
 
-        arguments = [cast(bufg)] + sizes + list(f.components) + ofsg
+        arguments = [cast(bufg)] + sizes + list(f.handles) + ofsg
         gather = Gather('gather%s' % key, arguments)
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
 
         count = reduce(mul, sizes, 1)*dtype_len(f.dtype)
         rrecv = Byref(FieldFromPointer(msg._C_field_rrecv, msg))
         rsend = Byref(FieldFromPointer(msg._C_field_rsend, msg))
         recv = IrecvCall([bufs, count, Macro(dtype_to_mpitype(f.dtype)),
                          fromrank, Integer(13), comm, rrecv])
         send = IsendCall([bufg, count, Macro(dtype_to_mpitype(f.dtype)),
                          torank, Integer(13), comm, rsend])
 
         iet = List(body=[recv, gather, send])
 
-        parameters = list(f.components) + ofsg + [fromrank, torank, comm, msg]
+        parameters = list(f.handles) + ofsg + [fromrank, torank, comm, msg]
 
         return SendRecv('sendrecv%s' % key, iet, parameters, bufg, bufs)
 
     def _call_sendrecv(self, name, *args, msg=None, haloid=None):
         # Drop `sizes` as this HaloExchangeBuilder conveys them through `msg`
         # Drop `ofss` as this HaloExchangeBuilder only needs them in `wait()`,
         # to collect and scatter the result of an MPI_Irecv
         f, _, ofsg, _, fromrank, torank, comm = args
         msg = Byref(IndexedPointer(msg, haloid))
-        return Call(name, list(f.components) + ofsg + [fromrank, torank, comm, msg])
+        return Call(name, list(f.handles) + ofsg + [fromrank, torank, comm, msg])
 
     def _make_haloupdate(self, f, hse, key, sendrecv, msg=None):
         iet = super()._make_haloupdate(f, hse, key, sendrecv, msg=msg)
         iet = iet._rebuild(parameters=iet.parameters + (msg,))
         return iet
 
     def _call_haloupdate(self, name, f, hse, msg):
@@ -672,29 +676,29 @@
 
         ofss = [Symbol(name='os%s' % d.root) for d in f.dimensions]
 
         fromrank = Symbol(name='fromrank')
 
         sizes = [FieldFromPointer('%s[%d]' % (msg._C_field_sizes, i), msg)
                  for i in range(len(f._dist_dimensions))]
-        arguments = [cast(bufs)] + sizes + list(f.components) + ofss
+        arguments = [cast(bufs)] + sizes + list(f.handles) + ofss
         scatter = Scatter('scatter%s' % key, arguments)
 
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
 
         rrecv = Byref(FieldFromPointer(msg._C_field_rrecv, msg))
         waitrecv = Call('MPI_Wait', [rrecv, Macro('MPI_STATUS_IGNORE')])
         rsend = Byref(FieldFromPointer(msg._C_field_rsend, msg))
         waitsend = Call('MPI_Wait', [rsend, Macro('MPI_STATUS_IGNORE')])
 
         iet = List(body=[waitsend, waitrecv, scatter])
 
-        parameters = (list(f.components) + ofss + [fromrank, msg])
+        parameters = (list(f.handles) + ofss + [fromrank, msg])
 
         return Callable('wait_%s' % key, iet, 'void', parameters, ('static',))
 
     def _make_halowait(self, f, hse, key, wait, msg=None):
         nb = f.grid.distributor._obj_neighborhood
 
         fixed = {d: Symbol(name="o%s" % d.root) for d in hse.loc_indices}
@@ -708,26 +712,26 @@
             mapper = OrderedDict(zip(dims, [i.flip() for i in tosides]))
             fromrank = FieldFromPointer(''.join(i.name[0] for i in mapper.values()), nb)
             ofss = [fixed.get(d, f._C_get_field(HALO, d, mapper.get(d)).offset)
                     for d in f.dimensions]
 
             msgi = Byref(IndexedPointer(msg, len(body)))
 
-            arguments = list(f.components) + ofss + [fromrank, msgi]
+            arguments = list(f.handles) + ofss + [fromrank, msgi]
             body.append(Call(wait.name, arguments))
 
         iet = List(body=body)
 
-        parameters = list(f.components) + list(fixed.values()) + [nb, msg]
+        parameters = list(f.handles) + list(fixed.values()) + [nb, msg]
 
         return Callable('halowait%d' % key, iet, 'void', parameters, ('static',))
 
     def _call_halowait(self, name, f, hse, msg):
         nb = f.grid.distributor._obj_neighborhood
-        arguments = list(f.components) + list(hse.loc_indices.values()) + [nb, msg]
+        arguments = list(f.handles) + list(hse.loc_indices.values()) + [nb, msg]
         return HaloWaitCall(name, arguments)
 
     def _make_remainder(self, hs, key, callcompute, *args):
         assert callcompute.is_Call
         body = [callcompute._rebuild(dynamic_args_mapper=i) for _, i in hs.omapper.owned]
         return Remainder.make('remainder%d' % key, body)
 
@@ -785,15 +789,15 @@
         sizes = [FieldFromComposite('%s[%d]' % (msg._C_field_sizes, i), msgi)
                  for i in range(len(f._dist_dimensions))]
         ofsg = [FieldFromComposite('%s[%d]' % (msg._C_field_ofsg, i), msgi)
                 for i in range(len(f._dist_dimensions))]
         ofsg = [fixed.get(d) or ofsg.pop(0) for d in f.dimensions]
 
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
-        arguments = [cast(bufg)] + sizes + list(f.components) + ofsg
+        arguments = [cast(bufg)] + sizes + list(f.handles) + ofsg
         gather = Gather('gather%s' % key, arguments)
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
 
         # Make Irecv/Isend
         count = reduce(mul, sizes, 1)*dtype_len(f.dtype)
         rrecv = Byref(FieldFromComposite(msg._C_field_rrecv, msgi))
         rsend = Byref(FieldFromComposite(msg._C_field_rsend, msgi))
@@ -801,20 +805,20 @@
                           fromrank, Integer(13), comm, rrecv])
         send = IsendCall([bufg, count, Macro(dtype_to_mpitype(f.dtype)),
                          torank, Integer(13), comm, rsend])
 
         # The -1 below is because an Iteration, by default, generates <=
         ncomms = Symbol(name='ncomms')
         iet = Iteration([recv, gather, send], dim, ncomms - 1)
-        parameters = f.components + (comm, msg, ncomms) + tuple(fixed.values())
+        parameters = f.handles + (comm, msg, ncomms) + tuple(fixed.values())
         return HaloUpdate('haloupdate%s' % key, iet, parameters)
 
     def _call_haloupdate(self, name, f, hse, msg):
         comm = f.grid.distributor._obj_comm
-        args = f.components + (comm, msg, msg.npeers) + tuple(hse.loc_indices.values())
+        args = f.handles + (comm, msg, msg.npeers) + tuple(hse.loc_indices.values())
         return HaloUpdateCall(name, args)
 
     def _make_halowait(self, f, hse, key, *args, msg=None):
         cast = cast_mapper[(f.c0.dtype, '*')]
 
         fixed = {d: Symbol(name="o%s" % d.root) for d in hse.loc_indices}
 
@@ -830,31 +834,31 @@
                  for i in range(len(f._dist_dimensions))]
         ofss = [FieldFromComposite('%s[%d]' % (msg._C_field_ofss, i), msgi)
                 for i in range(len(f._dist_dimensions))]
         ofss = [fixed.get(d) or ofss.pop(0) for d in f.dimensions]
 
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
-        arguments = [cast(bufs)] + sizes + list(f.components) + ofss
+        arguments = [cast(bufs)] + sizes + list(f.handles) + ofss
         scatter = Scatter('scatter%s' % key, arguments)
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
 
         rrecv = Byref(FieldFromComposite(msg._C_field_rrecv, msgi))
         waitrecv = Call('MPI_Wait', [rrecv, Macro('MPI_STATUS_IGNORE')])
         rsend = Byref(FieldFromComposite(msg._C_field_rsend, msgi))
         waitsend = Call('MPI_Wait', [rsend, Macro('MPI_STATUS_IGNORE')])
 
         # The -1 below is because an Iteration, by default, generates <=
         ncomms = Symbol(name='ncomms')
         iet = Iteration([waitsend, waitrecv, scatter], dim, ncomms - 1)
-        parameters = f.components + tuple(fixed.values()) + (msg, ncomms)
+        parameters = f.handles + tuple(fixed.values()) + (msg, ncomms)
         return Callable('halowait%d' % key, iet, 'void', parameters, ('static',))
 
     def _call_halowait(self, name, f, hse, msg):
-        args = f.components + tuple(hse.loc_indices.values()) + (msg, msg.npeers)
+        args = f.handles + tuple(hse.loc_indices.values()) + (msg, msg.npeers)
         return HaloWaitCall(name, args)
 
     def _make_wait(self, *args, **kwargs):
         return
 
     def _call_wait(self, *args):
         return
@@ -1007,36 +1011,36 @@
     'dual': DualHaloExchangeBuilder
 }
 
 
 # Callable sub-hierarchy
 
 
-class MPICallable(Callable):
+class MPICallable(CommCallable):
 
     def __init__(self, name, body, parameters):
-        super(MPICallable, self).__init__(name, body, 'void', parameters, ('static',))
+        super().__init__(name, body, 'void', parameters, ('static',))
 
 
 class CopyBuffer(MPICallable):
     pass
 
 
 class SendRecv(MPICallable):
 
     def __init__(self, name, body, parameters, bufg, bufs):
-        super(SendRecv, self).__init__(name, body, parameters)
+        super().__init__(name, body, parameters)
         self.bufg = bufg
         self.bufs = bufs
 
 
 class HaloUpdate(MPICallable):
 
     def __init__(self, name, body, parameters):
-        super(HaloUpdate, self).__init__(name, body, parameters)
+        super().__init__(name, body, parameters)
 
 
 class Remainder(ElementalFunction):
     pass
 
 
 # Call sub-hierarchy
@@ -1062,15 +1066,15 @@
 
 
 class MPICall(Call):
 
     @property
     def ncomps(self):
         """
-        The number of Bundle components this MPICall was constructed for.
+        The number of components this MPICall was constructed for.
         """
         return len([f for f in self.functions if f.is_DiscreteFunction])
 
 
 class HaloUpdateCall(MPICall):
     pass
 
@@ -1209,15 +1213,15 @@
             # returning from C-land
             self._memfree_args.extend([bufg_memfree_args, bufs_memfree_args])
 
         return {self.name: self.value}
 
     def _arg_values(self, args=None, **kwargs):
         # Any will do
-        for f in self.target.components:
+        for f in self.target.handles:
             try:
                 alias = kwargs[f.name]
                 break
             except KeyError:
                 pass
         else:
             alias = f
@@ -1300,15 +1304,15 @@
         for i in self.arguments:
             if i.is_Dimension:
                 fields.append((i.min_name, c_int))
                 fields.append((i.max_name, c_int))
             else:
                 fields.append((i.name, c_int))
 
-        super(MPIRegion, self).__init__(name, pname, fields)
+        super().__init__(name, pname, fields)
 
     def __value_setup__(self, dtype, value):
         # We eventually produce an array of `struct region` that is as big as
         # the number of OWNED sub-regions we have to compute to complete a
         # halo update
         return (dtype._type_*self.nregions)()
```

### Comparing `devito-4.8.3/devito/operations/interpolators.py` & `devito-4.8.4/devito/operations/interpolators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 from abc import ABC, abstractmethod
 from functools import wraps
 
 import sympy
+import numpy as np
 from cached_property import cached_property
 
+try:
+    from scipy.special import i0
+except ImportError:
+    from numpy import i0
+
 from devito.finite_differences.differentiable import Mul
 from devito.finite_differences.elementary import floor
+from devito.logger import warning
 from devito.symbolics import retrieve_function_carriers, retrieve_functions, INT
-from devito.tools import as_tuple, flatten
+from devito.tools import as_tuple, flatten, filter_ordered
 from devito.types import (ConditionalDimension, Eq, Inc, Evaluable, Symbol,
-                          CustomDimension)
+                          CustomDimension, SubFunction)
 from devito.types.utils import DimensionTuple
 
-__all__ = ['LinearInterpolator', 'PrecomputedInterpolator']
+__all__ = ['LinearInterpolator', 'PrecomputedInterpolator', 'SincInterpolator']
 
 
 def check_radius(func):
     @wraps(func)
     def wrapper(interp, *args, **kwargs):
         r = interp.sfunction.r
         funcs = set().union(*[retrieve_functions(a) for a in args])
         so = min({f.space_order for f in funcs if not f.is_SparseFunction} or {r})
         if so < r:
-            raise ValueError("Space order %d smaller than interpolation r %d" % (so, r))
+            raise ValueError("Space order %d too small for interpolation r %d" % (so, r))
         return func(interp, *args, **kwargs)
     return wrapper
 
 
 class UnevaluatedSparseOperation(sympy.Expr, Evaluable):
 
     """
@@ -121,31 +128,42 @@
 
 class GenericInterpolator(ABC):
 
     """
     Abstract base class defining the interface for an interpolator.
     """
 
+    _name = "generic"
+
     @abstractmethod
     def inject(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def interpolate(self, *args, **kwargs):
         pass
 
+    @property
+    def name(self):
+        return self._name
+
+    def _arg_defaults(self, **args):
+        return {}
+
 
 class WeightedInterpolator(GenericInterpolator):
 
     """
     Represent an Interpolation operation on a SparseFunction that is separable
     in space, meaning the coefficients are defined for each Dimension separately
     and multiplied at a given point: `w[x, y] = wx[x] * wy[y]`
     """
 
+    _name = 'weighted'
+
     def __init__(self, sfunction):
         self.sfunction = sfunction
 
     @property
     def grid(self):
         return self.sfunction.grid
 
@@ -159,15 +177,15 @@
 
     @property
     def r(self):
         return self.sfunction.r
 
     @cached_property
     def _rdim(self):
-        parent = self.sfunction.dimensions[-1]
+        parent = self.sfunction._sparse_dim
         dims = [CustomDimension("r%s%s" % (self.sfunction.name, d.name),
                                 -self.r+1, self.r, 2*self.r, parent)
                 for d in self._gdims]
 
         # Make radius dimension conditional to avoid OOB
         rdims = []
         pos = self.sfunction._position_map.values()
@@ -180,32 +198,35 @@
             rdims.append(ConditionalDimension(rd.name, rd, condition=cond,
                                               indirect=True))
 
         return DimensionTuple(*rdims, getters=self._gdims)
 
     def _augment_implicit_dims(self, implicit_dims, extras=None):
         if extras is not None:
-            extra = set([i for v in extras for i in v.dimensions]) - set(self._gdims)
+            extra = filter_ordered([i for v in extras for i in v.dimensions
+                                    if i not in self._gdims and
+                                    i not in self.sfunction.dimensions])
             extra = tuple(extra)
         else:
             extra = tuple()
 
         if self.sfunction._sparse_position == -1:
-            return self.sfunction.dimensions + as_tuple(implicit_dims) + extra
+            idims = self.sfunction.dimensions + as_tuple(implicit_dims) + extra
         else:
-            return as_tuple(implicit_dims) + self.sfunction.dimensions + extra
+            idims = extra + as_tuple(implicit_dims) + self.sfunction.dimensions
+        return tuple(idims)
 
     def _coeff_temps(self, implicit_dims):
         return []
 
     def _positions(self, implicit_dims):
         return [Eq(v, INT(floor(k)), implicit_dims=implicit_dims)
                 for k, v in self.sfunction._position_map.items()]
 
-    def _interp_idx(self, variables, implicit_dims=None):
+    def _interp_idx(self, variables, implicit_dims=None, pos_only=()):
         """
         Generate interpolation indices for the DiscreteFunctions in ``variables``.
         """
         mapper = {}
         pos = self.sfunction._position_map.values()
 
         # Temporaries for the position
@@ -216,14 +237,20 @@
 
         # Substitution mapper for variables
         mapper = self._rdim._getters
         idx_subs = {v: v.subs({k: c + p
                     for ((k, c), p) in zip(mapper.items(), pos)})
                     for v in variables}
 
+        # Position only replacement, not radius dependent.
+        # E.g src.inject(vp(x)*src) needs to use vp[posx] at all points
+        # not vp[posx + rx]
+        idx_subs.update({v: v.subs({k: p for (k, p) in zip(mapper, pos)})
+                         for v in pos_only})
+
         return idx_subs, temps
 
     @check_radius
     def interpolate(self, expr, increment=False, self_subs={}, implicit_dims=None):
         """
         Generate equations interpolating an arbitrary expression into ``self``.
 
@@ -279,24 +306,24 @@
         except AttributeError:
             # E.g., a generic SymPy expression or a number
             _expr = expr
 
         variables = list(retrieve_function_carriers(_expr))
 
         # Implicit dimensions
-        implicit_dims = self._augment_implicit_dims(implicit_dims)
+        implicit_dims = self._augment_implicit_dims(implicit_dims, variables)
 
         # List of indirection indices for all adjacent grid points
         idx_subs, temps = self._interp_idx(variables, implicit_dims=implicit_dims)
 
         # Accumulate point-wise contributions into a temporary
         rhs = Symbol(name='sum', dtype=self.sfunction.dtype)
         summands = [Eq(rhs, 0., implicit_dims=implicit_dims)]
         # Substitute coordinate base symbols into the interpolation coefficients
-        summands.extend([Inc(rhs, (_expr * self._weights).xreplace(idx_subs),
+        summands.extend([Inc(rhs, (self._weights * _expr).xreplace(idx_subs),
                              implicit_dims=implicit_dims)])
 
         # Write/Incr `self`
         lhs = self.sfunction.subs(self_subs)
         ecls = Inc if increment else Eq
         last = [ecls(lhs, rhs, implicit_dims=implicit_dims)]
 
@@ -340,22 +367,21 @@
         # Implicit dimensions
         implicit_dims = self._augment_implicit_dims(implicit_dims, variables)
         # Move all temporaries inside inner loop to improve parallelism
         # Can only be done for inject as interpolation need a temporary
         # summing temp that wouldn't allow collapsing
         implicit_dims = implicit_dims + tuple(r.parent for r in self._rdim)
 
-        variables = variables + list(fields)
-
         # List of indirection indices for all adjacent grid points
-        idx_subs, temps = self._interp_idx(variables, implicit_dims=implicit_dims)
+        idx_subs, temps = self._interp_idx(fields, implicit_dims=implicit_dims,
+                                           pos_only=variables)
 
         # Substitute coordinate base symbols into the interpolation coefficients
         eqns = [Inc(_field.xreplace(idx_subs),
-                    (_expr * self._weights).xreplace(idx_subs),
+                    (self._weights * _expr).xreplace(idx_subs),
                     implicit_dims=implicit_dims)
                 for (_field, _expr) in zip(fields, _exprs)]
 
         return temps + eqns
 
 
 class LinearInterpolator(WeightedInterpolator):
@@ -363,14 +389,17 @@
     Concrete implementation of WeightedInterpolator implementing a Linear interpolation
     scheme, i.e. Bilinear for 2D and Trilinear for 3D problems.
 
     Parameters
     ----------
     sfunction: The SparseFunction that this Interpolator operates on.
     """
+
+    _name = 'linear'
+
     @property
     def _weights(self):
         c = [(1 - p) * (1 - r) + p * r
              for (p, d, r) in zip(self._point_symbols, self._gdims, self._rdim)]
         return Mul(*c)
 
     @cached_property
@@ -396,25 +425,95 @@
     weigths/coefficients.
 
     Parameters
     ----------
     sfunction: The SparseFunction that this Interpolator operates on.
     """
 
+    _name = 'precomp'
+
     def _positions(self, implicit_dims):
-        if self.sfunction.gridpoints is None:
+        if self.sfunction.gridpoints_data is None:
             return super()._positions(implicit_dims)
-        # No position temp as we have directly the gridpoints
-        return [Eq(p, k, implicit_dims=implicit_dims)
-                for (k, p) in self.sfunction._position_map.items()]
+        else:
+            # No position temp as we have directly the gridpoints
+            return[Eq(p, k, implicit_dims=implicit_dims)
+                   for (k, p) in self.sfunction._position_map.items()]
 
     @property
     def interpolation_coeffs(self):
         return self.sfunction.interpolation_coeffs
 
     @property
     def _weights(self):
         ddim, cdim = self.interpolation_coeffs.dimensions[1:]
         mappers = [{ddim: ri, cdim: rd-rd.parent.symbolic_min}
                    for (ri, rd) in enumerate(self._rdim)]
         return Mul(*[self.interpolation_coeffs.subs(mapper)
                      for mapper in mappers])
+
+
+class SincInterpolator(PrecomputedInterpolator):
+    """
+    Hicks windowed sinc interpolation scheme.
+
+    Arbitrary source and receiver positioning in finite‐difference schemes
+    using Kaiser windowed sinc functions
+
+    https://library.seg.org/doi/10.1190/1.1451454
+
+    """
+
+    _name = 'sinc'
+
+    # Table 1
+    _b_table = {2: 2.94, 3: 4.53,
+                4: 4.14, 5: 5.26, 6: 6.40,
+                7: 7.51, 8: 8.56, 9: 9.56, 10: 10.64}
+
+    def __init__(self, sfunction):
+        if i0 is np.i0:
+            warning("""
+Using `numpy.i0`. We (and numpy) recommend to install scipy to improve the performance
+of the SincInterpolator that uses i0 (Bessel function).
+""")
+        super().__init__(sfunction)
+
+    @cached_property
+    def interpolation_coeffs(self):
+        coeffs = {}
+        shape = (self.sfunction.npoint, 2 * self.r)
+        for r in self._rdim:
+            dimensions = (self.sfunction._sparse_dim, r.parent)
+            sf = SubFunction(name="wsinc%s" % r.name, dtype=self.sfunction.dtype,
+                             shape=shape, dimensions=dimensions,
+                             space_order=0, alias=self.sfunction.alias,
+                             distributor=self.sfunction._distributor,
+                             parent=self.sfunction)
+            coeffs[r] = sf
+        return coeffs
+
+    @property
+    def _weights(self):
+        return Mul(*[w._subs(rd, rd-rd.parent.symbolic_min)
+                     for (rd, w) in self.interpolation_coeffs.items()])
+
+    def _arg_defaults(self, coords=None, sfunc=None):
+        args = {}
+        b = self._b_table[self.r]
+        b0 = i0(b)
+        if coords is None or sfunc is None:
+            raise ValueError("No coordinates or sparse function provided")
+        # Coords to indices
+        coords = coords / np.array(sfunc.grid.spacing)
+        coords = coords - np.floor(coords)
+
+        # Precompute sinc
+        for j, r in enumerate(self._rdim):
+            data = np.zeros((coords.shape[0], 2*self.r), dtype=sfunc.dtype)
+            for ri in range(2*self.r):
+                rpos = ri - self.r + 1 - coords[:, j]
+                num = i0(b*np.sqrt(1 - (rpos/self.r)**2))
+                data[:, ri] = num / b0 * np.sinc(rpos)
+            args[self.interpolation_coeffs[r].name] = data
+
+        return args
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devito-4.8.3/devito/operations/solve.py` & `devito-4.8.4/devito/operations/solve.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/operator/operator.py` & `devito-4.8.4/devito/operator/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from collections import OrderedDict, namedtuple
+import ctypes
 from operator import attrgetter
 from math import ceil
 
 from cached_property import cached_property
-import ctypes
+from sympy import sympify
 
 from devito.arch import compiler_registry, platform_registry
 from devito.data import default_allocator
-from devito.exceptions import InvalidOperator
-from devito.logger import debug, info, perf, warning, is_log_enabled_for
+from devito.exceptions import InvalidOperator, ExecutionError
+from devito.logger import debug, info, perf, warning, is_log_enabled_for, switch_log_level
 from devito.ir.equations import LoweredEq, lower_exprs
 from devito.ir.clusters import ClusterGroup, clusterize
 from devito.ir.iet import (Callable, CInterface, EntryFunction, FindSymbols, MetaCall,
                            derive_parameters, iet_build)
 from devito.ir.support import AccessMode, SymbolRegistry
 from devito.ir.stree import stree_build
 from devito.operator.profiling import AdvancedProfilerVerbose, create_profile
 from devito.operator.registry import operator_selector
 from devito.mpi import MPI
 from devito.parameters import configuration
 from devito.passes import (Graph, lower_index_derivatives, generate_implicit,
-                           generate_macros, minimize_symbols, unevaluate)
+                           generate_macros, minimize_symbols, unevaluate,
+                           error_mapper)
 from devito.symbolics import estimate_cost
 from devito.tools import (DAG, OrderedSet, Signer, ReducerMap, as_tuple, flatten,
                           filter_sorted, frozendict, is_integer, split, timed_pass,
                           timed_region, contains_val)
-from devito.types import Grid, Evaluable
+from devito.types import Grid, Evaluable, SubFunction
 
 __all__ = ['Operator']
 
 
 class Operator(Callable):
 
     """
@@ -132,20 +134,21 @@
     automatically discovered and handled by the Devito compiler. For more information,
     refer to the relevant documentation.
     """
 
     _default_headers = [('_POSIX_C_SOURCE', '200809L')]
     _default_includes = ['stdlib.h', 'math.h', 'sys/time.h']
     _default_globals = []
+    _default_namespaces = []
 
     def __new__(cls, expressions, **kwargs):
         if expressions is None:
             # Return a dummy Callable. This is exploited by unpickling. Users
             # can't do anything useful with it
-            return super(Operator, cls).__new__(cls, **kwargs)
+            return super().__new__(cls, **kwargs)
 
         # Parse input arguments
         kwargs = parse_kwargs(**kwargs)
 
         # The Operator type for the given target
         cls = operator_selector(**kwargs)
 
@@ -187,14 +190,16 @@
         op._headers = OrderedSet(*cls._default_headers)
         op._headers.update(byproduct.headers)
         op._globals = OrderedSet(*cls._default_globals)
         op._globals.update(byproduct.globals)
         op._includes = OrderedSet(*cls._default_includes)
         op._includes.update(profiler._default_includes)
         op._includes.update(byproduct.includes)
+        op._namespaces = OrderedSet(*cls._default_namespaces)
+        op._namespaces.update(byproduct.namespaces)
 
         # Required for the jit-compilation
         op._compiler = kwargs['compiler']
         op._language = kwargs['language']
         op._lib = None
         op._cfunction = None
 
@@ -262,17 +267,17 @@
 
         # unbounded IET -> IET
         iet, byproduct = cls._lower_iet(uiet, **kwargs)
 
         return IRs(expressions, clusters, stree, uiet, iet), byproduct
 
     @classmethod
-    def _rcompile_wrapper(cls, **kwargs):
-        def wrapper(expressions, kwargs=kwargs):
-            return rcompile(expressions, kwargs)
+    def _rcompile_wrapper(cls, **kwargs0):
+        def wrapper(expressions, **kwargs1):
+            return rcompile(expressions, {**kwargs0, **kwargs1})
         return wrapper
 
     @classmethod
     def _initialize_state(cls, **kwargs):
         return {}
 
     @classmethod
@@ -307,16 +312,23 @@
             * Shift indices for domain alignment.
         """
         expand = kwargs['options'].get('expand', True)
 
         # Specialization is performed on unevaluated expressions
         expressions = cls._specialize_dsl(expressions, **kwargs)
 
-        # Lower functional DSL
+        # Lower FD derivatives
+        # NOTE: we force expansion of derivatives along SteppingDimensions
+        # because it drastically simplifies the subsequent lowering into
+        # ModuloDimensions
+        if not expand:
+            expand = lambda d: d.is_Stepping
         expressions = flatten([i._evaluate(expand=expand) for i in expressions])
+
+        # Scalarize the tensor equations, if any
         expressions = [j for i in expressions for j in i._flatten]
 
         # A second round of specialization is performed on evaluated expressions
         expressions = cls._specialize_exprs(expressions, **kwargs)
 
         # "True" lowering (indexification, shifting, ...)
         expressions = lower_exprs(expressions, **kwargs)
@@ -436,23 +448,22 @@
         Iteration/Expression tree lowering:
 
             * Introduce distributed-memory, shared-memory, and SIMD parallelism;
             * Introduce optimizations for data locality;
             * Finalize (e.g., symbol definitions, array casts)
         """
         name = kwargs.get("name", "Kernel")
-        sregistry = kwargs['sregistry']
 
         # Wrap the IET with an EntryFunction (a special Callable representing
         # the entry point of the generated library)
         parameters = derive_parameters(uiet, True)
         iet = EntryFunction(name, uiet, 'int', parameters, ())
 
         # Lower IET to a target-specific IET
-        graph = Graph(iet, sregistry=sregistry)
+        graph = Graph(iet, **kwargs)
         graph = cls._specialize_iet(graph, **kwargs)
 
         # Instrument the IET for C-level profiling
         # Note: this is postponed until after _specialize_iet because during
         # specialization further Sections may be introduced
         cls._Target.instrument(graph, profiler=profiler, **kwargs)
 
@@ -611,15 +622,16 @@
         # one or more calls to third-party library functions, there could still be
         # at this point unprocessed arguments (e.g., scalars)
         kwargs.pop('args')
         args.update({k: v for k, v in kwargs.items() if k not in args})
 
         # Sanity check
         for p in self.parameters:
-            p._arg_check(args, self._dspace[p], am=self._access_modes.get(p))
+            p._arg_check(args, self._dspace[p], am=self._access_modes.get(p),
+                         **kwargs)
         for d in self.dimensions:
             if d.is_Derived:
                 d._arg_check(args, self._dspace[p])
 
         # Turn arguments into a format suitable for the generated code
         # E.g., instead of NumPy arrays for Functions, the generated code expects
         # pointers to ctypes.Struct
@@ -631,22 +643,33 @@
                 args.update(p._arg_finalize(args, alias=p))
 
         # Execute autotuning and adjust arguments accordingly
         args.update(self._autotune(args, autotune or configuration['autotuning']))
 
         return args
 
+    def _postprocess_errors(self, retval):
+        if retval == 0:
+            return
+        elif retval == error_mapper['Stability']:
+            raise ExecutionError("Detected nan/inf in some output Functions")
+        elif retval == error_mapper['KernelLaunch']:
+            raise ExecutionError("Kernel launch failed")
+        else:
+            raise ExecutionError("An error occurred during execution")
+
     def _postprocess_arguments(self, args, **kwargs):
         """Process runtime arguments upon returning from ``.apply()``."""
         for p in self.parameters:
             try:
                 subfuncs = (args[getattr(p, s).name] for s in p._sub_functions)
                 p._arg_apply(args[p.name], *subfuncs, alias=kwargs.get(p.name))
             except AttributeError:
-                p._arg_apply(args[p.name], alias=kwargs.get(p.name))
+                if not (isinstance(p, SubFunction) and p.parent in self.parameters):
+                    p._arg_apply(args[p.name], alias=kwargs.get(p.name))
 
     @cached_property
     def _known_arguments(self):
         """The arguments that can be passed to ``apply`` when running the Operator."""
         ret = set()
         for i in self.input:
             ret.update(i._arg_names)
@@ -692,16 +715,15 @@
         JIT-compile the C code generated by the Operator.
 
         It is ensured that JIT compilation will only be performed once per
         Operator, reagardless of how many times this method is invoked.
         """
         if self._lib is None:
             with self._profiler.timer_on('jit-compile'):
-                recompiled, src_file = self._compiler.jit_compile(self._soname,
-                                                                  str(self.ccode))
+                recompiled, src_file = self._compiler.jit_compile(self._soname, str(self))
 
             elapsed = self._profiler.py_timers['jit-compile']
             if recompiled:
                 perf("Operator `%s` jit-compiled `%s` in %.2f s with `%s`" %
                      (self.name, src_file, elapsed, self._compiler))
             else:
                 perf("Operator `%s` fetched `%s` in %.2f s from jit-cache" %
@@ -827,31 +849,35 @@
             args = self.arguments(**kwargs)
 
         # Invoke kernel function with args
         arg_values = [args[p.name] for p in self.parameters]
         try:
             cfunction = self.cfunction
             with self._profiler.timer_on('apply', comm=args.comm):
-                cfunction(*arg_values)
+                retval = cfunction(*arg_values)
         except ctypes.ArgumentError as e:
             if e.args[0].startswith("argument "):
                 argnum = int(e.args[0][9:].split(':')[0]) - 1
                 newmsg = "error in argument '%s' with value '%s': %s" % (
                     self.parameters[argnum].name,
                     arg_values[argnum],
                     e.args[0])
                 raise ctypes.ArgumentError(newmsg) from e
             else:
                 raise
 
+        # Perform error checking
+        self._postprocess_errors(retval)
+
         # Post-process runtime arguments
         self._postprocess_arguments(args, **kwargs)
 
-        # Output summary of performance achieved
-        return self._emit_apply_profiling(args)
+        # In case MPI is used restrict result logging to one rank only
+        with switch_log_level(comm=args.comm):
+            return self._emit_apply_profiling(args)
 
     # Performance profiling
 
     def _emit_build_profiling(self):
         if not is_log_enabled_for('PERF'):
             return
 
@@ -926,37 +952,47 @@
                     metrics.append("%.2f GPts/s" % fround(v.gpointss))
 
                 if metrics:
                     perf("Global performance <w/o setup>: [%s]" % ', '.join(metrics))
 
         # Emit local, i.e. "per-rank" performance. Without MPI, this is the only
         # thing that will be emitted
-        for k, v in summary.items():
-            rank = "[rank%d]" % k.rank if k.rank is not None else ""
+        def lower_perfentry(v):
             if v.gflopss:
                 oi = "OI=%.2f" % fround(v.oi)
                 gflopss = "%.2f GFlops/s" % fround(v.gflopss)
                 gpointss = "%.2f GPts/s" % fround(v.gpointss)
-                metrics = "[%s]" % ", ".join([oi, gflopss, gpointss])
+                return "[%s]" % ", ".join([oi, gflopss, gpointss])
+            elif v.gpointss:
+                gpointss = "%.2f GPts/s" % fround(v.gpointss)
+                return "[%s]" % gpointss
             else:
-                metrics = ""
+                return ""
+
+        for k, v in summary.items():
+            rank = "[rank%d]" % k.rank if k.rank is not None else ""
+
+            metrics = lower_perfentry(v)
 
             itershapes = [",".join(str(i) for i in its) for its in v.itershapes]
             if len(itershapes) > 1:
                 itershapes = ",".join("<%s>" % i for i in itershapes)
             elif len(itershapes) == 1:
                 itershapes = itershapes[0]
             else:
                 itershapes = ""
             name = "%s%s<%s>" % (k.name, rank, itershapes)
 
             perf("%s* %s ran in %.2f s %s" % (indent, name, fround(v.time), metrics))
-            for n, time in summary.subsections.get(k.name, {}).items():
-                perf("%s+ %s ran in %.2f s [%.2f%%]" %
-                     (indent*2, n, time, fround(time/v.time*100)))
+            for n, v1 in summary.subsections.get(k.name, {}).items():
+                metrics = lower_perfentry(v1)
+
+                perf("%s+ %s ran in %.2f s [%.2f%%] %s" %
+                     (indent*2, n, fround(v1.time), fround(v1.time/v.time*100),
+                      metrics))
 
         # Emit performance mode and arguments
         perf_args = {}
         for i in self.input + self.dimensions:
             if not i.is_PerfKnob:
                 continue
             try:
@@ -1013,14 +1049,15 @@
 # Default action (perform or bypass) for selected compilation passes upon
 # recursive compilation
 # NOTE: it may not only be pointless to apply the following passes recursively
 # (because once, during the main compilation phase, is simply enough), but also
 # dangerous as some of them (the minority) might break in some circumstances
 # if applied in cascade (e.g., `linearization` on top of `linearization`)
 rcompile_registry = {
+    'avoid_denormals': False,
     'mpi': False,
     'linearize': False,
     'place-transfers': False
 }
 
 
 def rcompile(expressions, kwargs=None):
@@ -1067,21 +1104,20 @@
     @property
     def comm(self):
         """The MPI communicator the arguments are collective over."""
         return self.grid.comm if self.grid is not None else MPI.COMM_NULL
 
     @property
     def opkwargs(self):
-        temp_registry = {v: k for k, v in platform_registry.items()}
-        platform = temp_registry[self.platform]
-
         temp_registry = {v: k for k, v in compiler_registry.items()}
         compiler = temp_registry[self.compiler.__class__]
 
-        return {'platform': platform, 'compiler': compiler, 'language': self.language}
+        return {'platform': self.platform.name,
+                'compiler': compiler,
+                'language': self.language}
 
 
 def parse_kwargs(**kwargs):
     """
     Parse keyword arguments provided to an Operator.
     """
     # `dse` -- deprecated, dropped
@@ -1195,8 +1231,11 @@
     # `allocator`
     kwargs['allocator'] = default_allocator(
         '%s.%s.%s' % (kwargs['compiler'].name,
                       kwargs['language'],
                       kwargs['platform'])
     )
 
+    # Normalize `subs`, if any
+    kwargs['subs'] = {k: sympify(v) for k, v in kwargs.get('subs', {}).items()}
+
     return kwargs
```

### Comparing `devito-4.8.3/devito/operator/profiling.py` & `devito-4.8.4/devito/operator/profiling.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,33 @@
 
             self._sections[s.name] = SectionData(ops, sops, points, traffic, itermaps)
 
     def track_subsection(self, sname, name):
         v = self._subsections.setdefault(sname, OrderedDict())
         v[name] = SectionData(S.Zero, S.Zero, S.Zero, S.Zero, [])
 
+    def group_as_subsections(self, sname, sections):
+        ops = sum(self._sections[i].ops for i in sections)
+        points = sum(self._sections[i].points for i in sections)
+        traffic = sum(self._sections[i].traffic for i in sections)
+        sectiondata = SectionData(ops, S.Zero, points, traffic, [])
+
+        v = self._subsections.setdefault(sname, OrderedDict())
+        v.update({i: self._sections[i] for i in sections})
+
+        new_sections = OrderedDict()
+        for k, v in self._sections.items():
+            try:
+                if sections.index(k) == len(sections) - 1:
+                    new_sections[sname] = sectiondata
+            except ValueError:
+                new_sections[k] = v
+        self._sections.clear()
+        self._sections.update(new_sections)
+
     def instrument(self, iet, timer):
         """
         Instrument the given IET for C-level performance profiling.
         """
         sections = FindNodes(Section).visit(iet)
         if sections:
             mapper = {}
@@ -207,87 +226,98 @@
         return (MPICall, BusyWait)
 
 
 class AdvancedProfiler(Profiler):
 
     _supports_async_sections = True
 
+    def _evaluate_section(self, name, data, args, dtype):
+        # Time to run the section
+        time = max(getattr(args[self.name]._obj, name), 10e-7)
+
+        # Number of FLOPs performed
+        try:
+            ops = int(subs_op_args(data.ops, args))
+        except (AttributeError, TypeError):
+            # E.g., a section comprising just function calls, or at least
+            # a sequence of unrecognized or non-conventional expr statements
+            ops = np.nan
+
+        try:
+            # Number of grid points computed
+            points = int(subs_op_args(data.points, args))
+
+            # Compulsory traffic
+            traffic = float(subs_op_args(data.traffic, args)*dtype().itemsize)
+        except (AttributeError, TypeError):
+            # E.g., the section has a dynamic loop size
+            points = np.nan
+
+            traffic = np.nan
+
+        # Nmber of FLOPs performed at each iteration
+        sops = data.sops
+
+        # Runtime itermaps/itershapes
+        try:
+            itermaps = [OrderedDict([(k, int(subs_op_args(v, args)))
+                                     for k, v in i.items()])
+                        for i in data.itermaps]
+            itershapes = tuple(tuple(i.values()) for i in itermaps)
+        except TypeError:
+            # E.g., a section comprising just function calls, or at least
+            # a sequence of unrecognized or non-conventional expr statements
+            itershapes = ()
+
+        return time, ops, points, traffic, sops, itershapes
+
+    def _allgather_from_comm(self, comm, time, ops, points, traffic, sops, itershapes):
+        times = comm.allgather(time)
+        assert comm.size == len(times)
+
+        opss = comm.allgather(ops)
+        pointss = comm.allgather(points)
+        traffics = comm.allgather(traffic)
+        sops = [sops]*comm.size
+        itershapess = comm.allgather(itershapes)
+
+        return list(zip(times, opss, pointss, traffics, sops, itershapess))
+
     # Override basic summary so that arguments other than runtime are computed.
     def summary(self, args, dtype, reduce_over=None):
         grid = args.grid
         comm = args.comm
 
         # Produce sections summary
         summary = PerformanceSummary()
         for name, data in self._sections.items():
-            # Time to run the section
-            time = max(getattr(args[self.name]._obj, name), 10e-7)
-
-            # Number of FLOPs performed
-            try:
-                ops = int(subs_op_args(data.ops, args))
-            except (AttributeError, TypeError):
-                # E.g., a section comprising just function calls, or at least
-                # a sequence of unrecognized or non-conventional expr statements
-                ops = np.nan
-
-            try:
-                # Number of grid points computed
-                points = int(subs_op_args(data.points, args))
-
-                # Compulsory traffic
-                traffic = float(subs_op_args(data.traffic, args)*dtype().itemsize)
-            except (AttributeError, TypeError):
-                # E.g., the section has a dynamic loop size
-                points = np.nan
-
-                traffic = np.nan
-
-            # Runtime itermaps/itershapes
-            try:
-                itermaps = [OrderedDict([(k, int(subs_op_args(v, args)))
-                                         for k, v in i.items()])
-                            for i in data.itermaps]
-                itershapes = tuple(tuple(i.values()) for i in itermaps)
-            except TypeError:
-                # E.g., a section comprising just function calls, or at least
-                # a sequence of unrecognized or non-conventional expr statements
-                itershapes = ()
+            items = self._evaluate_section(name, data, args, dtype)
 
             # Add local performance data
             if comm is not MPI.COMM_NULL:
                 # With MPI enabled, we add one entry per section per rank
-                times = comm.allgather(time)
-                assert comm.size == len(times)
-                opss = comm.allgather(ops)
-                pointss = comm.allgather(points)
-                traffics = comm.allgather(traffic)
-                sops = [data.sops]*comm.size
-                itershapess = comm.allgather(itershapes)
-                items = list(zip(times, opss, pointss, traffics, sops, itershapess))
+                items = self._allgather_from_comm(comm, *items)
                 for rank in range(comm.size):
                     summary.add(name, rank, *items[rank])
             else:
-                summary.add(name, None, time, ops, points, traffic, data.sops, itershapes)
+                summary.add(name, None, *items)
 
         # Enrich summary with subsections data
         for sname, v in self._subsections.items():
             for name, data in v.items():
-                # Time to run the section
-                time = max(getattr(args[self.name]._obj, name), 10e-7)
+                items = self._evaluate_section(name, data, args, dtype)
 
                 # Add local performance data
                 if comm is not MPI.COMM_NULL:
                     # With MPI enabled, we add one entry per section per rank
-                    times = comm.allgather(time)
-                    assert comm.size == len(times)
+                    items = self._allgather_from_comm(comm, *items)
                     for rank in range(comm.size):
-                        summary.add_subsection(sname, name, rank, time)
+                        summary.add_subsection(sname, name, rank, *items[rank])
                 else:
-                    summary.add_subsection(sname, name, None, time)
+                    summary.add_subsection(sname, name, None, *items)
 
         # Add global performance data
         if reduce_over is not None:
             # Vanilla metrics
             summary.add_glb_vanilla('vanilla', reduce_over)
 
             # Same as above but without setup overheads (e.g., host-device
@@ -352,15 +382,15 @@
     _ext_calls = [_api_resume, _api_pause]
 
     def __init__(self, name):
         self.path = locate_intel_advisor()
         if self.path is None:
             self.initialized = False
         else:
-            super(AdvisorProfiler, self).__init__(name)
+            super().__init__(name)
             # Make sure future compilations will get the proper header and
             # shared object files
             compiler = configuration['compiler']
             compiler.add_include_dirs(self.path.joinpath('include').as_posix())
             compiler.add_libraries(self._default_libs)
             libdir = self.path.joinpath('lib64').as_posix()
             compiler.add_library_dirs(libdir)
@@ -384,15 +414,15 @@
         # Return the IET intact if no time loop is found
         return iet
 
 
 class PerformanceSummary(OrderedDict):
 
     def __init__(self, *args, **kwargs):
-        super(PerformanceSummary, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.subsections = DefaultOrderedDict(lambda: OrderedDict())
         self.input = OrderedDict()
         self.globals = {}
 
     def add(self, name, rank, time,
             ops=None, points=None, traffic=None, sops=None, itershapes=None):
         """
@@ -418,19 +448,19 @@
             gpointss = gpoints/time
             oi = float(ops/traffic)
 
             self[k] = PerfEntry(time, gflopss, gpointss, oi, sops, itershapes)
 
         self.input[k] = PerfInput(time, ops, points, traffic, sops, itershapes)
 
-    def add_subsection(self, sname, name, rank, time):
+    def add_subsection(self, sname, name, rank, time, *args):
         k0 = PerfKey(sname, rank)
         assert k0 in self
 
-        self.subsections[sname][name] = time
+        self.subsections[sname][name] = PerfEntry(time, None, None, None, None, [])
 
     def add_glb_vanilla(self, key, time):
         """
         Reduce the following performance data:
 
             * ops
             * traffic
@@ -439,15 +469,15 @@
         """
         if not self.input:
             return
 
         ops = sum(v.ops for v in self.input.values())
         traffic = sum(v.traffic for v in self.input.values())
 
-        if np.isnan(traffic):
+        if np.isnan(traffic) or traffic == 0:
             return
 
         gflops = float(ops)/10**9
         gflopss = gflops/time
         oi = float(ops/traffic)
 
         self.globals[key] = PerfEntry(time, gflopss, None, oi, None, None)
```

### Comparing `devito-4.8.3/devito/operator/registry.py` & `devito-4.8.4/devito/operator/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         * `mode` is the optimization level (e.g., `advanced`).
         * `language` is the target language for shared-memory parallelism
           (e.g., 'C', 'openmp').
         * `operator` is an object of type Operator.
     """
 
     _modes = ('noop', 'advanced', 'advanced-fsg')
-    _languages = ('C', 'openmp', 'openacc', 'cuda', 'hip')
+    _languages = ('C', 'openmp', 'openacc', 'cuda', 'hip', 'sycl')
     _accepted = _modes + tuple(product(_modes, _languages))
 
     def add(self, operator, platform, mode, language='C'):
         assert issubclass(platform, Platform)
         assert mode in OperatorRegistry._modes or mode == 'custom'
 
         self[(platform, mode, language)] = operator
```

### Comparing `devito-4.8.3/devito/parameters.py` & `devito-4.8.4/devito/parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     A dictionary-like class to hold global configuration parameters for devito
     On top of a normal dict, this provides the option to provide callback functions
     so that any interested module can be informed when the configuration changes.
     """
 
     def __init__(self, name=None, **kwargs):
-        super(Parameters, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self._name = name
 
         self._accepted = {}
         self._deprecated = {}
         self._defaults = {}
         self._impact_jit = {}
 
@@ -70,34 +70,34 @@
         if key in self._preprocess_functions:
             return self._preprocess_functions[key](value)
         else:
             return value
 
     @_check_key_deprecation
     def __getitem__(self, key, *args):
-        return super(Parameters, self).__getitem__(key)
+        return super().__getitem__(key)
 
     @_check_key_deprecation
     @_check_key_value
     def __setitem__(self, key, value):
         value = self._preprocess(key, value)
         if key in self._update_functions:
             value = self._update_functions[key](value)
         if value is not None:
-            super(Parameters, self).__setitem__(key, value)
+            super().__setitem__(key, value)
 
     @_check_key_deprecation
     @_check_key_value
     def update(self, key, value):
         """
         Update the parameter ``key`` to ``value``. This is different from
         ``self[key] = value`` as both preprocessor and callback, if any,
         are bypassed.
         """
-        super(Parameters, self).__setitem__(key, value)
+        super().__setitem__(key, value)
 
     def add(self, key, value, accepted=None, preprocessor=None, callback=None,
             impacts_jit=True, deprecate=None):
         """
         Add a new parameter ``key`` with default value ``value``.
 
         Associate ``key`` with a list of ``accepted`` values.
@@ -105,15 +105,15 @@
         If provided, make sure ``callback`` is executed when the value of ``key``
         changes.
 
         If ``impacts_jit`` is False (defaults to True), then it can be assumed
         that the parameter doesn't affect code generation, so it can be excluded
         from the construction of the hash key.
         """
-        super(Parameters, self).__setitem__(key, value)
+        super().__setitem__(key, value)
         self._accepted[key] = accepted
         self._defaults[key] = value
         self._impact_jit[key] = impacts_jit
         if callable(preprocessor):
             self._preprocess_functions[key] = preprocessor
         if callable(callback):
             self._update_functions[key] = callback
```

### Comparing `devito-4.8.3/devito/passes/__init__.py` & `devito-4.8.4/devito/passes/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,24 +19,44 @@
         `gpu-fit` and is propagated down here through the various stages of lowering.
     """
     try:
         functions = (obj.function,)
     except AttributeError:
         functions = as_tuple(obj)
 
+    if any(f._mem_host for f in functions):
+        return False
+
     fsave = [f for f in functions
              if isinstance(f, TimeFunction) and is_integer(f.save)]
 
     if 'all-fallback' in gpu_fit and fsave:
         warning("TimeFunction %s assumed to fit the GPU memory" % fsave)
         return True
 
     return all(f in gpu_fit for f in fsave)
 
 
+def needs_transfer(f, gpu_fit):
+    """
+    True if the given object triggers a transfer from/to device memory,
+    False otherwise.
+
+    Parameters
+    ----------
+    f : Function
+        The target object.
+    gpu_fit : list of Function
+        The Function's which are known to definitely fit in the device memory. This
+        information is given directly by the user through the compiler option
+        `gpu-fit` and is propagated down here through the various stages of lowering.
+    """
+    return f._mem_mapped and not f.alias and is_on_device(f, gpu_fit)
+
+
 def is_gpu_create(obj, gpu_create):
     """
     True if the given objects are created and not copied in the device memory,
     False otherwise. Objects created in the device memory are zero-initialised.
 
     Parameters
     ----------
```

### Comparing `devito-4.8.3/devito/passes/clusters/aliases.py` & `devito-4.8.4/devito/passes/clusters/aliases.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 from functools import singledispatch
 from itertools import groupby
 
 from cached_property import cached_property
 import numpy as np
 import sympy
 
-from devito.finite_differences import EvalDerivative
-from devito.ir import (SEQUENTIAL, PARALLEL_IF_PVT, ROUNDABLE, SEPARABLE, Forward,
-                       IterationInstance, IterationSpace, Interval, Cluster,
-                       Queue, IntervalGroup, LabeledVector, normalize_properties,
-                       relax_properties, sdims_min, sdims_max)
-from devito.symbolics import (Uxmapper, compare_ops, estimate_cost, q_constant,
-                              reuse_if_untouched, retrieve_indexed, search, uxreplace,
-                              sympy_dtype)
-from devito.tools import (Stamp, as_mapper, as_tuple, flatten, frozendict, generator,
-                          split, timed_pass)
-from devito.types import (Array, TempFunction, Eq, Symbol, Temp, ModuloDimension,
-                          CustomDimension, IncrDimension, StencilDimension, Indexed,
-                          Hyperplane)
+from devito.finite_differences import EvalDerivative, IndexDerivative, Weights
+from devito.ir import (SEQUENTIAL, PARALLEL_IF_PVT, SEPARABLE, Forward,
+                       IterationSpace, Interval, Cluster, ExprGeometry, Queue,
+                       IntervalGroup, LabeledVector, Vector, normalize_properties,
+                       relax_properties, unbounded, minimum, maximum, extrema,
+                       vmax, vmin)
+from devito.passes.clusters.cse import _cse
+from devito.symbolics import (Uxmapper, estimate_cost, search, reuse_if_untouched,
+                              uxreplace, sympy_dtype)
+from devito.tools import (Stamp, as_mapper, as_tuple, flatten, frozendict,
+                          is_integer, generator, split, timed_pass)
+from devito.types import (Eq, Symbol, Temp, TempArray, TempFunction,
+                          ModuloDimension, CustomDimension, IncrDimension,
+                          StencilDimension, Indexed, Hyperplane)
 from devito.types.grid import MultiSubDimension
 
 __all__ = ['cire']
 
 
 @timed_pass(name='cire')
 def cire(clusters, mode, sregistry, options, platform):
@@ -79,18 +80,21 @@
     CIRE detects that these two expressions are actually redundant and rewrites
     them as:
 
     t2[x,y,z] = a[x,y,z]*b[x,y,z]
     t0 = 2.0*t2[x,y,z]
     t1 = 3.0*t2[x,y,z+1]
     """
-    modes = {
-        'invariants': [CireInvariantsElementary, CireInvariantsDivs],
-        'sops': [CireSops],
-    }
+    # NOTE: Handle prematurely expanded derivatives -- current default on
+    # several backends, but soon to become legacy
+    if mode == 'sops':
+        if options['expand']:
+            mode = 'eval-derivs'
+        else:
+            mode = 'index-derivs'
 
     for cls in modes[mode]:
         transformer = cls(sregistry, options, platform)
 
         clusters = transformer.process(clusters)
 
     return clusters
@@ -117,35 +121,33 @@
 
         # [Clusters]_n -> [Schedule]_m
         variants = []
         for mapper in self._generate(exprs, exclude):
             # Clusters -> AliasList
             found = collect(mapper.extracted, meta.ispace, self.opt_minstorage)
             pexprs, aliases = choose(found, exprs, mapper, self.opt_mingain)
-            if not aliases:
-                continue
 
             # AliasList -> Schedule
             schedule = lower_aliases(aliases, meta, self.opt_maxpar)
 
             variants.append(Variant(schedule, pexprs))
 
-        # [Schedule]_m -> Schedule (s.t. best memory/flops trade-off)
         if not variants:
             return []
-        schedule, exprs = pick_best(variants, self.opt_schedule_strategy,
-                                    self._eval_variants_delta)
+
+        # [Schedule]_m -> Schedule (s.t. best memory/flops trade-off)
+        schedule, exprs = self._select(variants)
 
         # Schedule -> Schedule (optimization)
         if self.opt_rotate:
             schedule = optimize_schedule_rotations(schedule, self.sregistry)
-        schedule = optimize_schedule_padding(schedule, meta, self.platform)
 
         # Schedule -> [Clusters]_k
-        processed, subs = lower_schedule(schedule, meta, self.sregistry, self.opt_ftemps)
+        processed, subs = lower_schedule(schedule, meta, self.sregistry,
+                                         self.opt_ftemps)
 
         # [Clusters]_k -> [Clusters]_k (optimization)
         if self.opt_multisubdomain:
             processed = optimize_clusters_msds(processed)
 
         # [Clusters]_k -> [Clusters]_{k+n}
         for c in clusters:
@@ -159,20 +161,52 @@
 
             processed.append(c.rebuild(exprs=cexprs, ispace=ispace))
 
         assert len(exprs) == 0
 
         return processed
 
+    def process(self, clusters):
+        raise NotImplementedError
+
+    def _generate(self, exprs, exclude):
+        """
+        Generate one or more extractions from ``exprs``. An extraction is a
+        set of CIRE candidates which may be turned into aliases. Two different
+        extractions may contain overlapping sub-expressions and, therefore,
+        should be processed and evaluated indipendently. An extraction won't
+        contain any of the symbols appearing in ``exclude``.
+        """
+        raise NotImplementedError
+
+    def _lookup_key(self, c):
+        """
+        Create a key for the given Cluster. Clusters with same key may be
+        processed together in the search for CIRE candidates. Clusters should
+        have a different key if they must not be processed together, e.g.,
+        when this would lead to violation of data dependencies.
+        """
+        raise NotImplementedError
+
+    def _select(self, variants):
+        """
+        Select the best variant out of a set of variants, weighing flops
+        and working set.
+        """
+        raise NotImplementedError
+
+
+class CireTransformerLegacy(CireTransformer):
+
     def _do_generate(self, exprs, exclude, cbk_search, cbk_compose=None):
         """
         Carry out the bulk of the work of ``_generate``.
         """
         counter = generator()
-        make = lambda: Symbol(name='dummy%d' % counter())
+        make = lambda: Symbol(name='dummy%d' % counter(), dtype=np.float32)
 
         if cbk_compose is None:
             cbk_compose = lambda *args: None
 
         mapper = Uxmapper()
         for e in exprs:
             for i in cbk_search(e):
@@ -189,46 +223,16 @@
                 if {a.function for a in free_symbols} & exclude:
                     continue
 
                 mapper.add(i, make, terms)
 
         return mapper
 
-    def _generate(self, exprs, exclude):
-        """
-        Generate one or more extractions from ``exprs``. An extraction is a
-        set of CIRE candidates which may be turned into aliases. Two different
-        extractions may contain overlapping sub-expressions and, therefore,
-        should be processed and evaluated indipendently. An extraction won't
-        contain any of the symbols appearing in ``exclude``.
-        """
-        raise NotImplementedError
 
-    def _lookup_key(self, c):
-        """
-        Create a key for the given Cluster. Clusters with same key may be
-        processed together in the search for CIRE candidates. Clusters should
-        have a different key if they must not be processed together, e.g.,
-        when this would lead to violation of data dependencies.
-        """
-        raise NotImplementedError
-
-    def _eval_variants_delta(self, delta_flops, delta_ws):
-        """
-        Given the deltas in flop reduction and working set size increase of two
-        Variants, return True if the second variant is estimated to deliever
-        better performance, False otherwise.
-        """
-        raise NotImplementedError
-
-    def process(self, clusters):
-        raise NotImplementedError
-
-
-class CireInvariants(CireTransformer, Queue):
+class CireInvariants(CireTransformerLegacy, Queue):
 
     def __init__(self, sregistry, options, platform):
         super().__init__(sregistry, options, platform)
 
         self.opt_maxpar = True
         self.opt_schedule_strategy = None
 
@@ -268,18 +272,16 @@
     def _lookup_key(self, c, d):
         ispace = c.ispace.reset()
         intervals = c.ispace.intervals.drop(d).reset()
         properties = frozendict({d: relax_properties(v) for d, v in c.properties.items()})
 
         return AliasKey(ispace, intervals, c.dtype, c.guards, properties)
 
-    def _eval_variants_delta(self, delta_flops, delta_ws):
-        # Always prefer the Variant with fewer temporaries
-        return ((delta_ws == 0 and delta_flops < 0) or
-                (delta_ws > 0))
+    def _select(self, variants):
+        return pick_best(variants)
 
 
 class CireInvariantsElementary(CireInvariants):
 
     def _generate(self, exprs, exclude):
         # E.g., extract `sin(x)` and `sqrt(x)` from `a*sin(x)*sqrt(x)`
         rule = lambda e: e.is_Function or (e.is_Pow and e.exp.is_Number and 0 < e.exp < 1)
@@ -306,15 +308,15 @@
     def _generate(self, exprs, exclude):
         # E.g., extract `1/h_x`
         rule = lambda e: e.is_Pow and (not e.exp.is_Number or e.exp < 0)
         cbk_search = lambda e: search(e, rule, 'all', 'bfs_first_hit')
         yield self._do_generate(exprs, exclude, cbk_search)
 
 
-class CireSops(CireTransformer):
+class CireDerivatives(CireTransformerLegacy):
 
     def __init__(self, sregistry, options, platform):
         super().__init__(sregistry, options, platform)
 
         self.opt_maxpar = options['cire-maxpar']
         self.opt_schedule_strategy = options['cire-schedule']
         self.opt_multisubdomain = False
@@ -337,63 +339,113 @@
             made = self._aliases_from_clusters([c], exclude, self._lookup_key(c))
 
             processed.extend(flatten(made) or [c])
 
         return processed
 
     def _generate(self, exprs, exclude):
-        # E.g., extract `u.dx*a*b` and `u.dx*a*c` from `[(u.dx*a*b).dy`, `(u.dx*a*c).dy]`
-        def cbk_search(expr):
-            if isinstance(expr, EvalDerivative) and not expr.base.is_Function:
-                return expr.args
-            else:
-                return flatten(e for e in [cbk_search(a) for a in expr.args] if e)
-
-        cbk_compose = lambda e: split_coeff(e)[1]
-        basextr = self._do_generate(exprs, exclude, cbk_search, cbk_compose)
+        # E.g., extract `u.dx*a*b` and `u.dx*a*c` from
+        # `[(u.dx*a*b).dy`, `(u.dx*a*c).dy]`
+        basextr = self._do_generate(exprs, exclude, self._cbk_search,
+                                    self._cbk_compose)
         if not basextr:
             return
         yield basextr
 
         # E.g., extract `u.dx*a` from `[(u.dx*a*b).dy, (u.dx*a*c).dy]`
-        # That is, attempt extracting the largest common derivative-induced subexprs
+        # I.e., attempt extracting the largest common derivative-induced subexprs
         mappers = [deindexify(e) for e in basextr.extracted]
         counter = Counter(flatten(m.keys() for m in mappers))
         groups = as_mapper(counter, key=counter.get)
         grank = {k: sorted(v, key=lambda e: estimate_cost(e), reverse=True)
                  for k, v in groups.items()}
 
-        def cbk_search2(expr, rank):
-            ret = []
-            for e in cbk_search(expr):
-                mapper = deindexify(e)
-                for i in rank:
-                    if i in mapper:
-                        ret.extend(mapper[i])
-                        break
-            return ret
-
         candidates = sorted(grank, reverse=True)[:2]
         for i in candidates:
             lower_pri_elems = flatten([grank[j] for j in candidates if j != i])
-            cbk_search_i = lambda e: cbk_search2(e, grank[i] + lower_pri_elems)
-            yield self._do_generate(exprs, exclude, cbk_search_i, cbk_compose)
+            cbk_search = lambda e: self._cbk_search2(e, grank[i] + lower_pri_elems)
+            yield self._do_generate(exprs, exclude, cbk_search, self._cbk_compose)
 
     def _lookup_key(self, c):
         return AliasKey(c.ispace, None, c.dtype, c.guards, c.properties)
 
-    def _eval_variants_delta(self, delta_flops, delta_ws):
-        # If there's a greater flop reduction using fewer temporaries, no doubts
-        # what's gonna be the best variant. But if the better flop reduction
-        # comes at the price of using more temporaries, then we have to apply
-        # heuristics, in particular we estimate how many flops would a temporary
-        # allow to save
-        return ((delta_flops >= 0 and delta_ws > 0 and delta_flops / delta_ws < 15) or
-                (delta_flops <= 0 and delta_ws < 0 and delta_flops / delta_ws > 15) or
-                (delta_flops <= 0 and delta_ws >= 0))
+    def _select(self, variants):
+        if isinstance(self.opt_schedule_strategy, int):
+            try:
+                return variants[self.opt_schedule_strategy]
+            except IndexError:
+                raise ValueError("Illegal schedule %d; "
+                                 "generated %d schedules in total"
+                                 % (self.opt_schedule_strategy, len(variants)))
+
+        return pick_best(variants)
+
+
+class CireEvalDerivatives(CireDerivatives):
+
+    def _cbk_compose(self, expr):
+        return split_coeff(expr)[1]
+
+    def _cbk_search(self, expr):
+        if isinstance(expr, EvalDerivative) and not expr.base.is_Function:
+            return expr.args
+        else:
+            return flatten(e for e in [self._cbk_search(a) for a in expr.args] if e)
+
+    def _cbk_search2(self, expr, rank):
+        ret = []
+        for e in self._cbk_search(expr):
+            mapper = deindexify(e)
+            for i in rank:
+                if i in mapper:
+                    ret.extend(mapper[i])
+                    break
+        return ret
+
+
+class CireIndexDerivatives(CireDerivatives):
+
+    def _cbk_compose(self, expr):
+        if expr.is_Pow:
+            return (expr,)
+        terms = []
+        for a in expr.args:
+            try:
+                if not isinstance(a.function, Weights):
+                    terms.append(a)
+            except AttributeError:
+                terms.append(a)
+        return tuple(terms)
+
+    def _cbk_search(self, expr):
+        if isinstance(expr, IndexDerivative):
+            return (expr.expr,)
+        else:
+            return flatten(e for e in [self._cbk_search(a) for a in expr.args] if e)
+
+    def _cbk_search2(self, expr, rank):
+        ret = []
+        for e in self._cbk_search(expr):
+            mapper = deindexify(e)
+            for i in rank:
+                found = [v.expr if isinstance(v, IndexDerivative) else v
+                         for v in mapper.get(i, [])]
+                if found:
+                    ret.extend(found)
+                    break
+        return ret
+
+
+# Subpass mapper
+modes = {
+    'invariants': [CireInvariantsElementary,
+                   CireInvariantsDivs],
+    'eval-derivs': [CireEvalDerivatives],   # NOTE: legacy pass
+    'index-derivs': [CireIndexDerivatives],
+}
 
 
 def collect(extracted, ispace, minstorage):
     """
     Find groups of aliasing expressions.
 
     We shall introduce the following (loose) terminology:
@@ -435,55 +487,32 @@
         * a[i+2] + b[i] : because the distances along ``i`` differ (+2 and +0)
     """
     # Find the potential aliases
     found = []
     for expr in extracted:
         assert not expr.is_Equality
 
-        indexeds = retrieve_indexed(expr)
-
-        bases = []
-        offsets = []
-        for i in indexeds:
-            ii = IterationInstance(i)
-            if ii.is_irregular:
-                break
-
-            base = []
-            offset = []
-            for e, ai in zip(ii, ii.aindices):
-                if q_constant(e):
-                    base.append(e)
-                else:
-                    base.append(ai)
-                    offset.append((ai, e - ai))
-            bases.append(tuple(base))
-            offsets.append(LabeledVector(offset))
-
-        if not indexeds or len(bases) == len(indexeds):
-            found.append(Candidate(expr, ispace, indexeds, bases, offsets))
+        eg = ExprGeometry(expr)
+        if eg.is_regular:
+            found.append(eg)
 
     # Create groups of aliasing expressions
     mapper = OrderedDict()
     unseen = list(found)
     while unseen:
         c = unseen.pop(0)
         group = [c]
         for u in list(unseen):
-            # Is the arithmetic structure of `c` and `u` equivalent ?
-            if not compare_ops(c.expr, u.expr):
-                continue
-
             # Is `c` translated w.r.t. `u` ?
             if not c.translated(u):
                 continue
 
             group.append(u)
             unseen.remove(u)
-        group = Group(group)
+        group = Group(group, ispace=ispace)
 
         if minstorage:
             k = group.dimensions_translated
         else:
             k = group.dimensions
         mapper.setdefault(k, []).append(group)
 
@@ -558,37 +587,36 @@
                 distance = [(d, set(v)) for d, v in LabeledVector.transpose(*distance)]
                 distances.append(LabeledVector([(d, v.pop()) for d, v in distance]))
 
             # Compute the alias score
             na = g.naliases
             nr = nredundants(ispace, pivot)
             score = estimate_cost(pivot, True)*((na - 1) + nr)
-            if score > 0:
-                aliases.add(pivot, aliaseds, list(mapper), distances, score)
+            aliases.add(pivot, aliaseds, list(mapper), distances, score)
 
     return aliases
 
 
 def choose(aliases, exprs, mapper, mingain):
     """
     Analyze the detected aliases and, after applying a cost model to rule out
     the aliases with a bad memory/flops trade-off, inject them into the original
     expressions.
     """
     aliases = AliasList(aliases)
 
+    if not aliases:
+        return exprs, aliases
+
     # `score < m` => discarded
     # `score > M` => optimized
-    # `m <= score <= M` => maybe discarded, maybe optimized -- depends on heuristics
+    # `m <= score <= M` => maybe discarded, maybe optimized; depends on heuristics
     m = mingain
     M = mingain*3
 
-    if not aliases:
-        return exprs, aliases
-
     # Filter off the aliases with low score
     key = lambda a: a.score >= m
     aliases.filter(key)
 
     # Project the candidate aliases into `exprs` to derive the final working set
     mapper = {k: v for k, v in mapper.items() if v.free_symbols & set(aliases.aliaseds)}
     templated = [uxreplace(e, mapper) for e in exprs]
@@ -685,30 +713,32 @@
                                                        dd.symbolic_size, 1, dd.step)
                 sub_iterators[i.dim] = d
             else:
                 d = i.dim
 
             # Given the iteration `interval`, lower distances to indices
             for distance, indices in zip(a.distances, indicess):
+                v = distance[interval.dim] or 0
                 try:
-                    indices.append(d - interval.lower + distance[interval.dim])
+                    indices.append(d - interval.lower + v)
                 except TypeError:
                     indices.append(d)
 
         # The alias write-to space
         writeto = IterationSpace(IntervalGroup(writeto), sub_iterators)
 
         # The alias iteration space
         ispace = IterationSpace(IntervalGroup(intervals, meta.ispace.relations),
                                 meta.ispace.sub_iterators,
                                 meta.ispace.directions)
         ispace = ispace.augment(sub_iterators)
 
-        processed.append(ScheduledAlias(a.pivot, writeto, ispace, a.aliaseds,
-                                        indicess, a.score))
+        processed.append(
+            ScheduledAlias(a.pivot, writeto, ispace, a.aliaseds, indicess)
+        )
 
     # The [ScheduledAliases] must be ordered so as to reuse as many of the
     # `ispace`'s IterationIntervals as possible in order to honor the
     # write-to region. Another fundamental reason for ordering is to ensure
     # deterministic code generation
     processed = sorted(processed, key=lambda i: cit(meta.ispace, i.ispace))
 
@@ -746,29 +776,29 @@
 
         n = candidate.min_size
         assert n > 0
 
         iis = candidate.lower
         iib = candidate.upper
 
-        ii = ModuloDimension('%sii' % d, ds, iis, incr=iib)
-        cd = CustomDimension(name='%s%s' % (d, d), symbolic_min=ii, symbolic_max=iib,
-                             symbolic_size=n)
-        dsi = ModuloDimension('%si' % ds, cd, cd + ds - iis, n)
+        ii = ModuloDimension('%sii' % d.root.name, ds, iis, incr=iib)
+        cd = CustomDimension(name='%sc' % d.root.name, symbolic_min=ii,
+                             symbolic_max=iib, symbolic_size=n)
+        dsi = ModuloDimension('%si' % ds.root.name, cd, cd + ds - iis, n)
 
         mapper = OrderedDict()
         for i in g:
             # Update `indicess` to use `xs0`, `xs1`, ...
             mds = []
             for indices in i.indicess:
                 v = indices[ridx]
                 try:
                     md = mapper[v]
                 except KeyError:
-                    name = sregistry.make_name(prefix='%sr' % d.name)
+                    name = sregistry.make_name(prefix='%sr' % d.root.name)
                     md = mapper.setdefault(v, ModuloDimension(name, ds, v, n))
                 mds.append(md)
             indicess = [indices[:ridx] + [md] + indices[ridx + 1:]
                         for md, indices in zip(mds, i.indicess)]
 
             # Update `writeto` by switching `d` to `dsi`
             intervals = k.intervals.switch(d, dsi).zero(dsi)
@@ -777,85 +807,63 @@
             writeto = IterationSpace(intervals, sub_iterators)
 
             # Transform `alias` by adding `i`
             pivot = i.pivot.xreplace({d: d + cd})
 
             # Extend `ispace` to iterate over rotations
             d1 = writeto[ridx+1].dim  # Note: we're by construction in-bounds here
-            intervals = IntervalGroup(Interval(cd, 0, 0), relations={(d, cd, d1)})
+            intervals = IntervalGroup(Interval(cd))
             rispace = IterationSpace(intervals, {cd: dsi}, {cd: Forward})
             aispace = i.ispace.zero(d)
             aispace = aispace.augment({d: mds + [ii]})
-            ispace = IterationSpace.union(rispace, aispace)
+            ispace = IterationSpace.union(rispace, aispace, relations={(d, cd, d1)})
 
-            processed.append(ScheduledAlias(pivot, writeto, ispace, i.aliaseds,
-                                            indicess, i.score))
+            processed.append(ScheduledAlias(
+                pivot, writeto, ispace, i.aliaseds, indicess,
+            ))
 
         # Update the rotations mapper
         rmapper[d].extend(list(mapper.values()))
 
     return schedule.rebuild(*processed, rmapper=rmapper)
 
 
-def optimize_schedule_padding(schedule, meta, platform):
-    """
-    Round up the innermost IterationInterval of the tensor temporaries IterationSpace
-    to a multiple of the SIMD vector length. This is not always possible though (it
-    depends on how much halo is safely accessible in all read Functions).
-    """
-    processed = []
-    for i in schedule:
-        try:
-            it = i.ispace.itintervals[-1]
-            if it.dim is i.writeto[-1].dim and ROUNDABLE in meta.properties[it.dim]:
-                vl = platform.simd_items_per_reg(meta.dtype)
-                ispace = i.ispace.add(Interval(it.dim, 0, it.size % vl))
-            else:
-                ispace = i.ispace
-            processed.append(ScheduledAlias(i.pivot, i.writeto, ispace, i.aliaseds,
-                                            i.indicess, i.score))
-        except (TypeError, KeyError, IndexError):
-            processed.append(i)
-
-    return schedule.rebuild(*processed)
-
-
 def lower_schedule(schedule, meta, sregistry, ftemps):
     """
     Turn a Schedule into a sequence of Clusters.
     """
     if ftemps:
         make = TempFunction
     else:
         # Typical case -- the user does *not* "see" the CIRE-created temporaries
-        make = Array
+        make = TempArray
 
     clusters = []
     subs = {}
-    for pivot, writeto, ispace, aliaseds, indicess, _ in schedule:
+    for pivot, writeto, ispace, aliaseds, indicess in schedule:
         name = sregistry.make_name()
         # Infer the dtype for the pivot
         # This prevents cases such as `floor(a*b)` with `a` and `b` floats
-        # that would creat a temporary `int r = b` leading to erronous numerical results
-        # Such cases happen with the positions for sparse functions for example.
-        dtype = sympy_dtype(pivot, meta.dtype)
+        # that would creat a temporary `int r = b` leading to erronous
+        # numerical results
+        dtype = sympy_dtype(pivot, base=meta.dtype)
 
         if writeto:
             # The Dimensions defining the shape of Array
             # Note: with SubDimensions, we may have the following situation:
             #
             # for zi = z_m + zi_ltkn; zi <= z_M - zi_rtkn; ...
             #   r[zi] = ...
             #
             # Instead of `r[zi - z_m - zi_ltkn]` we have just `r[zi]`, so we'll need
             # as much room as in `zi`'s parent to avoid going OOB
             # Aside from ugly generated code, the reason we do not rather shift the
             # indices is that it prevents future passes to transform the loop bounds
             # (e.g., MPI's comp/comm overlap does that)
-            dimensions = [d.parent if d.is_Sub else d for d in writeto.itdimensions]
+            dimensions = [d.parent if d.is_Sub else d for d in writeto.itdims]
 
             # The halo must be set according to the size of `writeto`
             halo = [(abs(i.lower), abs(i.upper)) for i in writeto]
 
             # The indices used to write into the Array
             indices = []
             for i in writeto:
@@ -885,22 +893,26 @@
         subs.update({aliased: callback(indices)
                      for aliased, indices in zip(aliaseds, indicess)})
 
         properties = dict(meta.properties)
 
         # Drop or weaken parallelism if necessary
         for d, v in meta.properties.items():
-            if any(i.is_Modulo for i in ispace.sub_iterators[d]):
-                properties[d] = normalize_properties(v, {SEQUENTIAL})
-            elif d not in writeto.itdimensions:
-                properties[d] = normalize_properties(v, {PARALLEL_IF_PVT}) - {ROUNDABLE}
+            try:
+                if any(i.is_Modulo for i in ispace.sub_iterators[d]):
+                    properties[d] = normalize_properties(v, {SEQUENTIAL})
+                elif d not in writeto.itdims:
+                    properties[d] = normalize_properties(v, {PARALLEL_IF_PVT})
+            except KeyError:
+                # Non-dimension key such as (x, y) for diagonal stencil u(x+i hx, y+i hy)
+                pass
 
         # Track star-shaped stencils for potential future optimization
         if len(writeto) > 1 and schedule.is_frame:
-            properties[Hyperplane(writeto.itdimensions)] = {SEPARABLE}
+            properties[Hyperplane(writeto.itdims)] = {SEPARABLE}
 
         # Finally, build the alias Cluster
         clusters.append(Cluster(expression, ispace, meta.guards, properties))
 
     return clusters, subs
 
 
@@ -908,15 +920,15 @@
     """
     Relax the clusters by letting the expressions defined over MultiSubDomains to
     rather be computed over the entire domain. This increases the likelihood of
     code lifting by later passes.
     """
     processed = []
     for c in clusters:
-        msds = [d for d in c.ispace.itdimensions if isinstance(d, MultiSubDimension)]
+        msds = [d for d in c.ispace.itdims if isinstance(d, MultiSubDimension)]
 
         if msds:
             mapper = {d: d.root for d in msds}
             exprs = [uxreplace(e, mapper) for e in c.exprs]
 
             ispace = c.ispace.relaxed(msds)
 
@@ -928,142 +940,88 @@
                                        properties=properties, syncs=syncs))
         else:
             processed.append(c)
 
     return processed
 
 
-def pick_best(variants, schedule_strategy, eval_variants_delta):
+def pick_best(variants):
     """
-    Return the variant with the best trade-off between operation count
-    reduction and working set increase. Heuristics may be applied.
+    Return the variant with the best theoretical performance.
     """
-    if type(schedule_strategy) is int:
-        try:
-            return variants[schedule_strategy]
-        except IndexError:
-            raise ValueError("Illegal schedule strategy %d; accepted `[0, %d]`"
-                             % (schedule_strategy, len(variants) - 1))
-
     best = None
-    best_flops_score = None
-    best_ws_score = None
-
     for i in variants:
-        i_flops_score = sum(sa.score for sa in i.schedule)
-
-        # The working set score depends on the number and dimensionality of
-        # temporaries required by the Schedule
-        i_ws_count = Counter([len(sa.writeto) for sa in i.schedule])
-        i_ws_score = tuple(i_ws_count[sa + 1] for sa in reversed(range(max(i_ws_count))))
-        # TODO: For now, we assume the performance impact of an N-dimensional
-        # temporary is always the same regardless of the value N, but this might
-        # change in the future
-        i_ws_score = sum(i_ws_score)
+        # Flops in the two sweeps
+        flops0 = i.schedule.cost
+        flops1 = estimate_cost(i.exprs, True)
 
-        if best is None:
-            best, best_flops_score, best_ws_score = i, i_flops_score, i_ws_score
-            continue
-
-        delta_flops = best_flops_score - i_flops_score
-        delta_ws = best_ws_score - i_ws_score
-        if eval_variants_delta(delta_flops, delta_ws):
-            best, best_flops_score, best_ws_score = i, i_flops_score, i_ws_score
-
-    return best
+        flops = flops0 + flops1
 
+        # Data movement in the two sweeps
+        indexeds0 = search([sa.pivot for sa in i.schedule], Indexed)
+        indexeds1 = search(i.exprs, Indexed)
 
-# Utilities
-
-
-class Candidate(object):
+        ntemps = len(i.schedule)
+        nfunctions0 = len({i.function for i in indexeds0})
+        nfunctions1 = len({i.function for i in indexeds1})
 
-    def __init__(self, expr, ispace, indexeds, bases, offsets):
-        self.expr = expr
-        self.ispace = ispace
-        self.indexeds = indexeds
-        self.bases = bases
-        self.offsets = offsets
-
-    def __repr__(self):
-        return "Candidate(expr=%s)" % self.expr
+        ws = ntemps*2 + nfunctions0 + nfunctions1
 
-    def translated(self, other):
-        """
-        True if ``self`` is translated w.r.t. ``other``, False otherwise.
-
-        Examples
-        --------
-        Two candidates are translated if their bases are the same and
-        their offsets are pairwise translated.
-
-        c := A[i,j] op A[i,j+1]     -> Toffsets = {i: [0,0], j: [0,1]}
-        u := A[i+1,j] op A[i+1,j+1] -> Toffsets = {i: [1,1], j: [0,1]}
-
-        Then `c` is translated w.r.t. `u` with distance `{i: 1, j: 0}`
-        """
-        if len(self.Toffsets) != len(other.Toffsets):
-            return False
-        if len(self.bases) != len(other.bases):
-            return False
-
-        # Check the bases
-        if any(b0 != b1 for b0, b1 in zip(self.bases, other.bases)):
-            return False
+        if best is None:
+            best, best_flops, best_ws = i, flops, ws
+            continue
 
-        # Check the offsets
-        for (d0, o0), (d1, o1) in zip(self.Toffsets, other.Toffsets):
-            if d0 is not d1:
-                return False
+        delta_flops = flops - best_flops
+        delta_ws = ws - best_ws
 
-            distance = set(o0 - o1)
-            if len(distance) != 1:
-                return False
+        # Magic sauce
+        # The coefficients were obtained empirically studying the behaviour
+        # of different variants in several kernels and platforms
+        # Intuitively, it's like trading 70 operations for 1 temporary
+        ws_curve = lambda x: (-1 / 70)*x
 
-        return True
+        if delta_ws <= ws_curve(delta_flops):
+            best, best_flops, best_ws = i, flops, ws
 
-    @cached_property
-    def Toffsets(self):
-        return LabeledVector.transpose(*self.offsets)
+    return best
 
-    @cached_property
-    def dimensions(self):
-        return frozenset(i for i, _ in self.Toffsets)
 
-    @property
-    def shifts(self):
-        return self.ispace.intervals
+# Utilities
 
 
 class Group(tuple):
 
     """
     A collection of aliasing expressions.
     """
 
-    def __new__(cls, items):
+    def __new__(cls, items, ispace=None):
         # Expand out the StencilDimensions, if any
         processed = []
         for c in items:
-            if not c.expr.find(StencilDimension):
+            sdims = [d for d in unbounded(c.expr) if d.is_Stencil]
+            if not sdims:
                 processed.append(c)
                 continue
 
-            for f in (sdims_min, sdims_max):
+            f0 = lambda e: minimum(e, sdims)
+            f1 = lambda e: maximum(e, sdims)
+
+            for f in (f0, f1):
                 expr = f(c.expr)
                 indexeds = [f(i) for i in c.indexeds]
                 offsets = [LabeledVector([(d, f(i)) for d, i in v.items()])
                            for v in c.offsets]
 
-                processed.append(
-                    Candidate(expr, c.ispace, indexeds, c.bases, offsets)
-                )
+                processed.append(ExprGeometry(expr, indexeds, c.bases, offsets))
 
         obj = super().__new__(cls, processed)
         obj._items = items
+        obj._ispace = ispace
+
         return obj
 
     def __repr__(self):
         return "Group(%s)" % ", ".join([str(i) for i in self])
 
     def find_rotation_distance(self, d, interval):
         """
@@ -1095,49 +1053,58 @@
         """
         The size of the iteration space required to evaluate all aliasing
         expressions in this Group, along each Dimension.
         """
         ret = defaultdict(int)
         for i in self.Toffsets:
             for d, v in i:
+                if d not in self._ispace:
+                    continue
                 try:
                     distance = int(max(v) - min(v))
                 except TypeError:
                     # An entry in `v` has symbolic components, e.g. `x_m + 2`
                     if len(set(v)) == 1:
                         continue
                     else:
-                        raise ValueError
+                        # Worst-case scenario, we raraly end up here
+                        # Resort to the fast vector-based comparison machinery
+                        # (rather than the slower sympy.simplify)
+                        items = [Vector(i) for i in v]
+                        distance, = vmax(*items) - vmin(*items)
+                        if not is_integer(distance):
+                            raise ValueError
                 ret[d] = max(ret[d], distance)
 
         return ret
 
     @property
     def pivot(self):
         """
-        A deterministically chosen Candidate for this Group.
+        A deterministically chosen reference for this Group.
         """
         return self[0]
 
     @property
     def dimensions(self):
-        return self.pivot.dimensions
+        return frozenset(self.diameter)
 
     @property
     def dimensions_translated(self):
         return frozenset(d for d, v in self.diameter.items() if v > 0)
 
     @property
     def naliases(self):
         na = len(self._items)
 
-        sdims = set().union(*[c.expr.find(StencilDimension) for c in self._items])
-        implicit = int(np.prod([i._size for i in sdims])) - 1
+        udims = set().union(*[unbounded(c.expr) for c in self._items])
+        sdims = [d for d in udims if d.is_Stencil]
+        implicit = int(np.prod([i._size for i in sdims]))
 
-        return na + implicit
+        return na*max(implicit, 1)
 
     @cached_property
     def _pivot_legal_rotations(self):
         """
         All legal rotations along each Dimension for the Group pivot.
         """
         ret = {}
@@ -1159,15 +1126,15 @@
 
         return ret
 
     @cached_property
     def _pivot_min_intervals(self):
         """
         The minimum Interval along each Dimension such that by evaluating the
-        pivot, all Candidates are evaluated too.
+        pivot, all other items are evaluated too.
         """
         c = self.pivot
 
         ret = defaultdict(lambda: [np.inf, -np.inf])
         for i in self:
             distance = [o.distance(v) for o, v in zip(i.offsets, c.offsets)]
             distance = [(d, set(v)) for d, v in LabeledVector.transpose(*distance)]
@@ -1192,25 +1159,31 @@
         Group pivot does not go OOB.
         """
         c = self.pivot
 
         ret = defaultdict(lambda: (-np.inf, np.inf))
         for i, ofs in zip(c.indexeds, c.offsets):
             f = i.function
+
             for l in ofs.labels:
+                if isinstance(l, StencilDimension):
+                    continue
+
                 # `f`'s cumulative halo size along `l`
                 hsize = sum(f._size_halo[l])
 
                 # Any `ofs`'s shift due to non-[0,0] iteration space
-                lower, upper = c.shifts[l].offsets
+                lower, upper = self._ispace.intervals[l].offsets
+
+                ofs0, ofs1 = extrema(ofs[l])
 
                 try:
                     # Assume `ofs[l]` is a number (typical case)
-                    maxd = min(0, max(ret[l][0], -ofs[l] - lower))
-                    mini = max(0, min(ret[l][1], hsize - ofs[l] - upper))
+                    maxd = min(0, max(ret[l][0], -ofs0 - lower))
+                    mini = max(0, min(ret[l][1], hsize - ofs1 - upper))
 
                     ret[l] = (maxd, mini)
                 except TypeError:
                     # E.g., `ofs[d] = x_m - x + 5`
                     ret[l] = (0, 0)
 
         return ret
@@ -1218,15 +1191,15 @@
 
 AliasKey = namedtuple('AliasKey', 'ispace intervals dtype guards properties')
 Variant = namedtuple('Variant', 'schedule exprs')
 
 
 class Alias(object):
 
-    def __init__(self, pivot, aliaseds, intervals, distances, score=0):
+    def __init__(self, pivot, aliaseds, intervals, distances, score):
         self.pivot = pivot
         self.aliaseds = aliaseds
         self.intervals = intervals
         self.distances = distances
         self.score = score
 
     def __repr__(self):
@@ -1278,15 +1251,15 @@
     def __len__(self):
         return self._list.__len__()
 
     def __iter__(self):
         for i in self._list:
             yield i
 
-    def add(self, pivot, aliaseds, intervals, distances, score=0):
+    def add(self, pivot, aliaseds, intervals, distances, score):
         assert len(aliaseds) == len(distances)
         self._list.append(Alias(pivot, aliaseds, intervals, distances, score))
 
     def update(self, aliases):
         self._list.extend(aliases)
 
     def filter(self, key):
@@ -1302,34 +1275,49 @@
     def is_frame(self):
         """
         An AliasList is said to be a "frame" if all of its Aliases are frames.
         """
         return all(i.is_frame for i in self._list)
 
 
-ScheduledAlias = namedtuple('SchedAlias', 'pivot writeto ispace aliaseds indicess score')
+ScheduledAlias = namedtuple('SchedAlias',
+                            'pivot writeto ispace aliaseds indicess')
 
 
 class Schedule(tuple):
 
     def __new__(cls, *items, dmapper=None, rmapper=None, is_frame=False):
-        obj = super(Schedule, cls).__new__(cls, items)
+        obj = super().__new__(cls, items)
         obj.dmapper = dmapper or {}
         obj.rmapper = rmapper or {}
         obj.is_frame = is_frame
         return obj
 
     def rebuild(self, *items, dmapper=None, rmapper=None, is_frame=False):
         return Schedule(
             *items,
             dmapper=dmapper or self.dmapper,
             rmapper=rmapper or self.rmapper,
             is_frame=is_frame or self.is_frame
         )
 
+    @cached_property
+    def cost(self):
+        # Not just the sum for the individual items' cost! There might be
+        # redundancies, which we factor out here...
+        counter = generator()
+        make = lambda: Symbol(name='dummy%d' % counter(), dtype=np.float32)
+
+        tot = 0
+        for v in as_mapper(self, lambda i: i.ispace).values():
+            exprs = [i.pivot for i in v]
+            tot += estimate_cost(_cse(exprs, make), True)
+
+        return tot
+
 
 def make_rotations_table(d, v):
     """
     All possible rotations of `range(v+1)`.
     """
     m = np.array([[j-i if j > i else 0 for j in range(v+1)] for i in range(v+1)])
     m = (m - m.T)[::-1, :]
```

### Comparing `devito-4.8.3/devito/passes/clusters/asynchrony.py` & `devito-4.8.4/devito/passes/clusters/asynchrony.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import OrderedDict, defaultdict
 
 from sympy import And
 
 from devito.ir import (Forward, GuardBoundNext, Queue, Vector, WaitLock, WithLock,
                        FetchUpdate, PrefetchUpdate, ReleaseLock, normalize_syncs)
-from devito.passes.clusters.utils import is_memcpy
+from devito.passes.clusters.utils import bind_critical_regions, is_memcpy
 from devito.symbolics import IntDiv, uxreplace
 from devito.tools import OrderedSet, is_integer, timed_pass
 from devito.types import CustomDimension, Lock
 
 __all__ = ['Tasker', 'Streaming']
 
 
@@ -135,14 +135,20 @@
                     function = None
                     findex = None
 
                 for i in indices:
                     tasks[c0].append(ReleaseLock(lock[i], target))
                     tasks[c0].append(WithLock(lock[i], target, i, function, findex, d))
 
+        # CriticalRegions preempt WaitLocks, by definition
+        mapper = bind_critical_regions(clusters)
+        for c in clusters:
+            for c1 in mapper.get(c, []):
+                waits[c].update(waits.pop(c1, []))
+
         processed = []
         for c in clusters:
             if waits[c] or tasks[c]:
                 processed.append(c.rebuild(syncs={d: list(waits[c]) + tasks[c]}))
             else:
                 processed.append(c)
```

### Comparing `devito-4.8.3/devito/passes/clusters/blocking.py` & `devito-4.8.4/devito/passes/clusters/blocking.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from sympy import sympify
 
+from devito.finite_differences.differentiable import IndexSum
 from devito.ir.clusters import Queue
 from devito.ir.support import (AFFINE, PARALLEL, PARALLEL_IF_ATOMIC, PARALLEL_IF_PVT,
                                SEQUENTIAL, SKEWABLE, TILABLES, Interval,
                                IntervalGroup, IterationSpace, Scope)
 from devito.passes import is_on_device
-from devito.symbolics import uxreplace, xreplace_indices
-from devito.tools import UnboundedMultiTuple, as_tuple, flatten, is_integer, prod
+from devito.symbolics import search, uxreplace, xreplace_indices
+from devito.tools import (UnboundedMultiTuple, UnboundTuple, as_tuple,
+                          filter_ordered, flatten, is_integer, prod)
 from devito.types import BlockDimension
 
 __all__ = ['blocking']
 
 
 def blocking(clusters, sregistry, options):
     """
@@ -96,14 +98,16 @@
 
     def _has_data_reuse(self, cluster):
         # A sufficient condition for the existance of data reuse in `cluster`
         # is that the same Function is accessed twice at the same memory location,
         # which translates into the existance of any Relation accross Indexeds
         if any(r.function.is_AbstractFunction for r in cluster.scope.r_gen()):
             return True
+        if search(cluster.exprs, IndexSum):
+            return True
 
         # If it's a reduction operation a la matrix-matrix multiply, two Indexeds
         # might be enough
         if any(PARALLEL_IF_ATOMIC in p for p in cluster.properties.values()):
             return True
 
         # If we are going to skew, then we might exploit reuse along an
@@ -152,29 +156,37 @@
         super().__init__(options)
 
         self.gpu_fit = options.get('gpu-fit', ())
 
     def _make_key_hook(self, cluster, level):
         return (is_on_device(cluster.functions, self.gpu_fit),)
 
+    def _has_other_blockable_dim(self, cluster, d):
+        return any(cluster.properties.is_parallel_relaxed(i) and
+                   not self._has_short_trip_count(i)
+                   for i in set(cluster.ispace.itdims) - {d})
+
     def callback(self, clusters, prefix):
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
-        if self._has_short_trip_count(d):
-            return clusters
 
         processed = []
         for c in clusters:
             if not c.properties.is_parallel_relaxed(d):
                 return clusters
 
             if is_on_device(c.functions, self.gpu_fit):
-                if self._has_data_reuse(c):
+                if self._has_short_trip_count(d):
+                    if self._has_other_blockable_dim(c, d):
+                        return clusters
+                    else:
+                        properties = c.properties.block(d, 'small')
+                elif self._has_data_reuse(c):
                     properties = c.properties.block(d)
                 else:
                     properties = c.properties.block(d, 'small')
             elif self._has_data_reuse(c):
                 properties = c.properties.block(d)
             else:
                 return clusters
@@ -310,15 +322,15 @@
         # Create the block Dimensions (in total `self.levels` Dimensions)
         base = self.sregistry.make_name(prefix=d.name)
 
         if blk_size_gen is not None:
             # By passing a suitable key to `next` we ensure that we pull the
             # next par-tile entry iff we're now blocking an unseen TILABLE nest
             try:
-                step = sympify(blk_size_gen.next(clusters, d))
+                step = sympify(blk_size_gen.next(prefix, d, clusters))
             except StopIteration:
                 return clusters
         else:
             # This will result in a parametric step, e.g. `x0_blk0_size`
             step = None
 
         name = self.sregistry.make_name(prefix="%s_blk" % base)
@@ -336,22 +348,24 @@
 
         processed = []
         for c in clusters:
             if c.properties.is_blockable(d):
                 ispace = decompose(c.ispace, d, block_dims)
 
                 # Use the innermost BlockDimension in place of `d`
-                exprs = [uxreplace(e, {d: bd}) for e in c.exprs]
+                subs = {d: bd}
+                exprs = [uxreplace(e, subs) for e in c.exprs]
+                guards = {subs.get(i, i): v for i, v in c.guards.items()}
 
                 # The new Cluster properties -- TILABLE is dropped after blocking
                 properties = c.properties.drop(d)
                 properties = properties.add(block_dims, c.properties[d] - TILABLES)
 
                 processed.append(c.rebuild(exprs=exprs, ispace=ispace,
-                                           properties=properties))
+                                           guards=guards, properties=properties))
             else:
                 processed.append(c)
 
         return processed
 
 
 def decompose(ispace, d, block_dims):
@@ -379,26 +393,36 @@
             continue
 
         for bd in block_dims:
             # Avoid e.g. `x > yb`
             if any(i._depth < bd._depth for i in r if i.is_Block):
                 continue
 
-            relations.append(tuple(bd if i in d._defines else i for i in r))
+            # E.g., `r=(z, i0z)` -> `[i0z0_blk0, i0z0_blk0]`
+            v = [bd if i in d._defines else i for i in r]
+
+            # E.g., `v=[i0z0_blk0, i0z0_blk0]` -> `v=(i0z0_blk0,)`
+            v = tuple(filter_ordered(v))
+
+            relations.append(v)
 
     # 3: Make sure BlockDimensions at same depth stick next to each other
     # E.g., `(t, xbb, ybb, xb, yb, x, y)`, and NOT e.g. `(t, xbb, xb, x, ybb, ...)`
     # NOTE: this is perfectly legal since:
     # TILABLE => (perfect nest & PARALLEL) => interchangeable
-    for i in ispace.itdimensions:
+    for i in ispace.itdims:
         if not i.is_Block:
             continue
         for bd in block_dims:
             if i._depth < bd._depth:
+                # E.g. `(zb, y)`
                 relations.append((i, bd))
+            elif i._depth == bd._depth:
+                # E.g. `(y, z)` (i.e., honour input ordering)
+                relations.append((bd, i))
 
     intervals = IntervalGroup(intervals, relations=relations)
 
     sub_iterators = dict(ispace.sub_iterators)
     sub_iterators.pop(d, None)
     sub_iterators.update({bd: () for bd in block_dims[:-1]})
     sub_iterators.update({block_dims[-1]: ispace.sub_iterators[d]})
@@ -413,36 +437,98 @@
 class BlockSizeGenerator(object):
 
     """
     A wrapper for several UnboundedMultiTuples.
     """
 
     def __init__(self, par_tile):
-        self.umt = UnboundedMultiTuple(*par_tile)
+        self.tip = -1
+
+        # The default par-tile, as an UnboundedMultiTuple. It will be used
+        # for most cases
+        self.umt = par_tile
 
-        # This is for Clusters that need a small par-tile to avoid under-utilizing
-        # computational resources (e.g., kernels running over iteration spaces that
-        # are relatively small for the underlying architecture)
+        # Special case 1: a smaller par-tile to avoid under-utilizing
+        # computational resources when the iteration spaces are too small
         if (len(par_tile) == 1 and
             (len(par_tile[0]) < len(par_tile.default) or
              prod(par_tile[0]) < prod(par_tile.default))):
             # Ignore if, e.g., user supplies a lower dimensional block shape
             self.umt_small = self.umt
         else:
             self.umt_small = UnboundedMultiTuple(par_tile.default)
 
-    def next(self, clusters, d):
-        # TODO: This is for now exceptionally rudimentary
+        # Special case 2: par-tiles for iteration spaces that must be fully
+        # blocked for correctness
+        if par_tile.sparse:
+            self.umt_sparse = UnboundTuple(*par_tile.sparse, 1)
+        elif len(par_tile) == 1:
+            self.umt_sparse = UnboundTuple(*par_tile[0], 1)
+        else:
+            self.umt_sparse = UnboundTuple(*par_tile.default, 1)
+
+        if par_tile.reduce:
+            self.umt_reduce = UnboundTuple(*par_tile.reduce, 1)
+        elif len(par_tile) == 1:
+            self.umt_reduce = UnboundTuple(*par_tile[0], 1)
+        else:
+            self.umt_reduce = UnboundTuple(*par_tile.default, 1)
+
+    def next(self, prefix, d, clusters):
+        # If a whole new set of Dimensions, move the tip -- this means `clusters`
+        # at `d` represents a new loop nest or kernel
+        x = any(i.dim.is_Block for i in flatten(c.ispace for c in clusters))
+        if not x:
+            self.tip += 1
+
+        # Correctness -- enforce blocking where necessary.
+        # See also issue #276:PRO
+        if any(c.properties.is_parallel_atomic(d) for c in clusters):
+            if any(c.is_sparse for c in clusters):
+                if not x:
+                    self.umt_sparse.iter()
+                return self.umt_sparse.next()
+            else:
+                if not x:
+                    self.umt_reduce.iter()
+                return self.umt_reduce.next()
+
+        # Performance heuristics -- use a smaller par-tile
         if all(c.properties.is_blockable_small(d) for c in clusters):
-            umt = self.umt_small
+            if not x:
+                self.umt_small.iter()
+            return self.umt_small.next()
+
+        if x:
+            item = self.umt.curitem()
         else:
+            # We can't `self.umt.iter()` because we might still want to
+            # fallback to `self.umt_small`
+            item = self.umt.nextitem()
+
+        # Handle user-provided rules
+        # TODO: This is also rudimentary
+        if item.rule is None:
             umt = self.umt
+        elif is_integer(item.rule):
+            if item.rule == self.tip:
+                umt = self.umt
+            else:
+                umt = self.umt_small
+                if not x:
+                    umt.iter()
+        else:
+            if item.rule in {d.name for d in prefix.itdims}:
+                umt = self.umt
+            else:
+                # This is like "pattern unmatched" -- fallback to `umt_small`
+                umt = self.umt_small
+                if not x:
+                    umt.iter()
 
-        if not any(i.dim.is_Block for i in flatten(c.ispace for c in clusters)):
-            umt.iter()
         return umt.next()
 
 
 class SynthesizeSkewing(Queue):
 
     """
     Construct a new sequence of clusters with skewed expressions and iteration spaces.
```

### Comparing `devito-4.8.3/devito/passes/clusters/buffering.py` & `devito-4.8.4/devito/passes/clusters/buffering.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 # non-uniform SubDimensions, to avoid uninitialized values to
                 # be copied-back into the buffered Function
                 continue
 
             expr = lower_exprs(Eq(lhs, rhs))
             ispace = b.writeto
             guards[pd] = GuardBound(dim.root.symbolic_min, dim.root.symbolic_max)
-            properties = {d: {AFFINE, PARALLEL} for d in ispace.itdimensions}
+            properties = {d: {AFFINE, PARALLEL} for d in ispace.itdims}
 
             init.append(Cluster(expr, ispace, guards=guards, properties=properties))
 
         if not buffers:
             return clusters
 
         # Substitution rules to replace buffered Functions with buffers
@@ -303,15 +303,15 @@
             else:
                 continue
 
             processed1 = []
             for c in processed:
                 if b.buffer in c.functions:
                     key1 = lambda d: d not in b.dim._defines
-                    dims = c.ispace.project(key1).itdimensions
+                    dims = c.ispace.project(key1).itdims
                     ispace = c.ispace.lift(dims, key0())
                     processed1.append(c.rebuild(ispace=ispace))
                 else:
                     processed1.append(c)
             processed = processed1
 
         return init + processed
@@ -428,15 +428,19 @@
         try:
             expr, = self.accessv.exprs
         except ValueError:
             assert False
 
         lhs, rhs = expr.args
 
-        self.xd = lhs.function.indices[self.dim]
+        maybe_xd = lhs.function.indices[self.dim]
+        if not isinstance(maybe_xd, CustomDimension):
+            maybe_xd = rhs.function.indices[self.dim]
+            assert isinstance(maybe_xd, CustomDimension)
+        self.xd = maybe_xd
 
         idx0 = lhs.indices[self.dim]
         idx1 = rhs.indices[self.dim]
 
         if self.is_read:
             if is_integer(idx0) or isinstance(idx0, ModuloDimension):
                 # This is just for aesthetics of the generated code
@@ -610,15 +614,15 @@
         """
         The `readfrom` IterationSpace, that is the iteration space that must be
         iterated over to update the buffer with the buffered Function values.
         """
         ispace0 = self.written.project(lambda d: d in self.xd._defines)
         ispace1 = self.writeto.project(lambda d: d not in self.xd._defines)
 
-        extra = (ispace0.itdimensions + ispace1.itdimensions,)
+        extra = (ispace0.itdims + ispace1.itdims,)
         ispace = IterationSpace.union(ispace0, ispace1, relations=extra)
 
         return ispace
 
     @cached_property
     def lastidx(self):
         """
```

### Comparing `devito-4.8.3/devito/passes/clusters/cse.py` & `devito-4.8.4/devito/passes/clusters/cse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from collections import Counter, OrderedDict
 from functools import singledispatch
 
 from sympy import Add, Function, Indexed, Mul, Pow
+from sympy.core.core import ordering_of_classes
 
 from devito.finite_differences.differentiable import IndexDerivative
 from devito.ir import Cluster, Scope, cluster_pass
 from devito.passes.clusters.utils import makeit_ssa
 from devito.symbolics import estimate_cost, q_leaf
 from devito.symbolics.manipulation import _uxreplace
-from devito.types import Eq, Temp as Temp0
+from devito.tools import as_list
+from devito.types import Eq, Symbol, Temp
 
 __all__ = ['cse']
 
 
-class Temp(Temp0):
-    pass
+class CTemp(Temp):
+
+    """
+    A cluster-level Temp, similar to Temp, ensured to have different priority
+    """
+    ordering_of_classes.insert(ordering_of_classes.index('Temp') + 1, 'CTemp')
 
 
 @cluster_pass
 def cse(cluster, sregistry, options, *args):
     """
     Common sub-expressions elimination (CSE).
     """
-    make = lambda: Temp(name=sregistry.make_name(), dtype=cluster.dtype)
+    make = lambda: CTemp(name=sregistry.make_name(), dtype=cluster.dtype)
     exprs = _cse(cluster, make, min_cost=options['cse-min-cost'])
 
     return cluster.rebuild(exprs=exprs)
 
 
 def _cse(maybe_exprs, make, min_cost=1, mode='default'):
     """
@@ -48,21 +54,26 @@
     # - it also captures array index access functions (eg, i+1 in A[i+1] and B[i+1]);
     # - it sometimes "captures too much", losing factorization opportunities;
     # - very slow
     # TODO: a second "sympy" mode will be provided, relying on SymPy's CSE() but
     # also ensuring some form of post-processing
     assert mode == 'default'  # Only supported mode ATM
 
-    # Just for flexibility, accept either Clusters or exprs
+    # Accept Clusters, Eqs or even just exprs
     if isinstance(maybe_exprs, Cluster):
         processed = list(maybe_exprs.exprs)
         scope = maybe_exprs.scope
     else:
-        processed = list(maybe_exprs)
-        scope = Scope(maybe_exprs)
+        maybe_exprs = as_list(maybe_exprs)
+        if all(e.is_Equality for e in maybe_exprs):
+            processed = maybe_exprs
+            scope = Scope(maybe_exprs)
+        else:
+            processed = [Eq(make(), e) for e in maybe_exprs]
+            scope = Scope([])
 
     # Some sub-expressions aren't really "common" -- that's the case of Dimension-
     # independent data dependences. For example:
     #
     # ... = ... a[i] + 1 ...
     # a[i] = ...
     # ... = ... a[i] + 1 ...
@@ -120,15 +131,15 @@
     exprs = makeit_ssa(exprs)
 
     # Drop candidates are all exprs in the form `t0 = s` where `s` is a symbol
     # Note: only CSE-captured Temps, which are by construction local objects, may
     # safely be compacted; a generic Symbol could instead be accessed in a subsequent
     # Cluster, for example: `for (i = ...) { a = b; for (j = a ...) ...`
     mapper = {e.lhs: e.rhs for e in exprs
-              if isinstance(e.lhs, Temp) and q_leaf(e.rhs) and e.lhs not in exclude}
+              if isinstance(e.lhs, CTemp) and q_leaf(e.rhs) and e.lhs not in exclude}
 
     processed = []
     for e in exprs:
         if e.lhs not in mapper:
             # The temporary is retained, and substitutions may be applied
             expr, changed = e, True
             while changed:
@@ -154,23 +165,33 @@
 def _(exprs):
     mapper = Counter()
     for e in exprs:
         mapper.update(count(e))
     return mapper
 
 
-@count.register(IndexDerivative)
 @count.register(Indexed)
+@count.register(Symbol)
 def _(expr):
     """
     Handler for objects preventing CSE to propagate through their arguments.
     """
     return Counter()
 
 
+@count.register(IndexDerivative)
+def _(expr):
+    """
+    Handler for symbol-binding objects. There can be many of them and therefore
+    they should be detected as common subexpressions, but it's either pointless
+    or forbidden to look inside them.
+    """
+    return Counter([expr])
+
+
 @count.register(Add)
 @count.register(Mul)
 @count.register(Pow)
 @count.register(Function)
 def _(expr):
     mapper = Counter()
     for a in expr.args:
```

### Comparing `devito-4.8.3/devito/passes/clusters/factorization.py` & `devito-4.8.4/devito/passes/clusters/factorization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
 
 from sympy import Add, Mul, S, collect
 
 from devito.ir import cluster_pass
 from devito.symbolics import BasicWrapperMixin, estimate_cost, retrieve_symbols
 from devito.tools import ReducerMap
+from devito.types.object import AbstractObject
 
 __all__ = ['factorize']
 
 
 MIN_COST_FACTORIZE = 100
 """
 Minimum operation count of an expression so that aggressive factorization
@@ -39,14 +40,79 @@
             cost_handle, handle = cost_prev, handle_prev
 
         processed.append(handle)
 
     return cluster.rebuild(processed)
 
 
+def collect_special(expr):
+    """
+    Factorize elemental functions, pows, and other special symbolic objects,
+    prioritizing the most expensive entities.
+    """
+    args, candidates = zip(*[_collect_nested(arg) for arg in expr.args])
+    candidates = ReducerMap.fromdicts(*candidates)
+
+    funcs = candidates.getall('funcs', [])
+    pows = candidates.getall('pows', [])
+    coeffs = candidates.getall('coeffs', [])
+
+    # Functions/Pows are collected first, coefficients afterwards
+    terms = []
+    w_funcs = []
+    w_pows = []
+    w_coeffs = []
+    for i in args:
+        _args = i.args
+        if any(j in funcs for j in _args):
+            w_funcs.append(i)
+        elif any(j in pows for j in _args):
+            w_pows.append(i)
+        elif any(j in coeffs for j in _args):
+            w_coeffs.append(i)
+        else:
+            terms.append(i)
+
+    # Collect common funcs
+    if len(w_funcs) > 1:
+        w_funcs = Add(*w_funcs, evaluate=False)
+        w_funcs = collect(w_funcs, funcs, evaluate=False)
+        try:
+            terms.extend([Mul(k, collect_const(v), evaluate=False)
+                          for k, v in w_funcs.items()])
+        except AttributeError:
+            assert w_funcs == 0
+    else:
+        terms.extend(w_funcs)
+
+    # Collect common pows
+    w_pows = Add(*w_pows, evaluate=False)
+    w_pows = collect(w_pows, pows, evaluate=False)
+    try:
+        terms.extend([Mul(k, collect_const(v), evaluate=False)
+                      for k, v in w_pows.items()])
+    except AttributeError:
+        assert w_pows == 0
+
+    # Collect common temporaries (r0, r1, ...)
+    w_coeffs = Add(*w_coeffs, evaluate=False)
+    symbols = retrieve_symbols(w_coeffs)
+    if symbols:
+        w_coeffs = collect(w_coeffs, symbols, evaluate=False)
+        try:
+            terms.extend([Mul(k, collect_const(v), evaluate=False)
+                          for k, v in w_coeffs.items()])
+        except AttributeError:
+            assert w_coeffs == 0
+    else:
+        terms.append(w_coeffs)
+
+    return Add(*terms)
+
+
 def collect_const(expr):
     """
     *Much* faster alternative to sympy.collect_const. *Potentially* slightly less
     powerful with complex expressions, but it is equally effective for the
     expressions we have to deal with.
     """
     # Running example: `a*3. + b*2. + c*3.`
@@ -63,17 +129,18 @@
             inverse_mapper[-v].append(-k)
 
     terms = []
     for k, v in inverse_mapper.items():
         if len(v) == 1 and not v[0].is_Add:
             # Special case: avoid e.g. (-2)*a
             mul = Mul(k, *v)
-        elif all(i.is_Mul and len(i.args) == 2 and i.args[0] == -1 for i in v):
+        elif all(i.is_Mul and i.args[0] == -1 for i in v):
             # Other special case: [-a, -b, -c ...]
-            add = Add(*[i.args[1] for i in v], evaluate=False)
+            operands = [Mul(*i.args[1:], evaluate=False) for i in v]
+            add = Add(*operands, evaluate=False)
             mul = Mul(-k, add, evaluate=False)
         elif k == 1:
             # 1 * (a + c)
             mul = Add(*v)
         else:
             # Back to the running example
             # -> (a + c)
@@ -85,109 +152,59 @@
                 mul = Mul(k, add, evaluate=False)
 
         terms.append(mul)
 
     return Add(*terms)
 
 
-def collect_nested(expr):
-    """
-    Collect numeric coefficients, trascendental functions, and symbolic powers,
-    across all levels of the expression tree.
+def strategy0(expr):
+    rebuilt = collect_special(expr)
+    rebuilt = collect_const(rebuilt)
+
+    return rebuilt
+
+
+strategies = {
+    'default': strategy0
+}
+
+
+def _collect_nested(expr):
+    """
+    Recursion helper for `collect_nested`.
+    """
+    # Return semantic (rebuilt expression, factorization candidates)
+
+    if expr.is_Number:
+        return expr, {'coeffs': expr}
+    elif expr.is_Function:
+        return expr, {'funcs': expr}
+    elif expr.is_Pow:
+        return expr, {'pows': expr}
+    elif (expr.is_Symbol or expr.is_Indexed or not expr.args or
+          isinstance(expr, (BasicWrapperMixin, AbstractObject))):
+        return expr, {}
+    elif expr.is_Add:
+        return strategies['default'](expr), {}
+    elif expr.is_Mul:
+        args, candidates = zip(*[_collect_nested(arg) for arg in expr.args])
+        return Mul(*args), ReducerMap.fromdicts(*candidates)
+    elif expr.is_Equality:
+        args, candidates = zip(*[_collect_nested(expr.lhs),
+                                 _collect_nested(expr.rhs)])
+        return expr.func(*args, evaluate=False), ReducerMap.fromdicts(*candidates)
+    else:
+        args, candidates = zip(*[_collect_nested(arg) for arg in expr.args])
+        return expr.func(*args), ReducerMap.fromdicts(*candidates)
 
-    The collection gives precedence to (in order of importance):
 
-        1) Trascendental functions,
-        2) Symbolic powers,
-        3) Numeric coefficients.
+def collect_nested(expr):
+    """
+    Collect numeric coefficients, trascendental functions, pows, and other
+    symbolic objects across all levels of the expression tree.
 
     Parameters
     ----------
     expr : expr-like
         The expression to be factorized.
     """
-
-    def run(expr):
-        # Return semantic (rebuilt expression, factorization candidates)
-
-        if expr.is_Number:
-            return expr, {'coeffs': expr}
-        elif expr.is_Function:
-            return expr, {'funcs': expr}
-        elif expr.is_Pow:
-            return expr, {'pows': expr}
-        elif expr.is_Symbol or expr.is_Indexed or isinstance(expr, BasicWrapperMixin):
-            return expr, {}
-        elif expr.is_Add:
-            args, candidates = zip(*[run(arg) for arg in expr.args])
-            candidates = ReducerMap.fromdicts(*candidates)
-
-            funcs = candidates.getall('funcs', [])
-            pows = candidates.getall('pows', [])
-            coeffs = candidates.getall('coeffs', [])
-
-            # Functions/Pows are collected first, coefficients afterwards
-            terms = []
-            w_funcs = []
-            w_pows = []
-            w_coeffs = []
-            for i in args:
-                _args = i.args
-                if any(j in funcs for j in _args):
-                    w_funcs.append(i)
-                elif any(j in pows for j in _args):
-                    w_pows.append(i)
-                elif any(j in coeffs for j in _args):
-                    w_coeffs.append(i)
-                else:
-                    terms.append(i)
-
-            # Collect common funcs
-            if len(w_funcs) > 1:
-                w_funcs = Add(*w_funcs, evaluate=False)
-                w_funcs = collect(w_funcs, funcs, evaluate=False)
-                try:
-                    terms.extend([Mul(k, collect_const(v), evaluate=False)
-                                  for k, v in w_funcs.items()])
-                except AttributeError:
-                    assert w_funcs == 0
-            else:
-                terms.extend(w_funcs)
-
-            # Collect common pows
-            w_pows = Add(*w_pows, evaluate=False)
-            w_pows = collect(w_pows, pows, evaluate=False)
-            try:
-                terms.extend([Mul(k, collect_const(v), evaluate=False)
-                              for k, v in w_pows.items()])
-            except AttributeError:
-                assert w_pows == 0
-
-            # Collect common temporaries (r0, r1, ...)
-            w_coeffs = Add(*w_coeffs, evaluate=False)
-            symbols = retrieve_symbols(w_coeffs)
-            if symbols:
-                w_coeffs = collect(w_coeffs, symbols, evaluate=False)
-                try:
-                    terms.extend([Mul(k, collect_const(v), evaluate=False)
-                                  for k, v in w_coeffs.items()])
-                except AttributeError:
-                    assert w_coeffs == 0
-            else:
-                terms.append(w_coeffs)
-
-            # Collect common coefficients
-            rebuilt = Add(*terms)
-            rebuilt = collect_const(rebuilt)
-
-            return rebuilt, {}
-        elif expr.is_Mul:
-            args, candidates = zip(*[run(arg) for arg in expr.args])
-            return Mul(*args), ReducerMap.fromdicts(*candidates)
-        elif expr.is_Equality:
-            args, candidates = zip(*[run(expr.lhs), run(expr.rhs)])
-            return expr.func(*args, evaluate=False), ReducerMap.fromdicts(*candidates)
-        else:
-            args, candidates = zip(*[run(arg) for arg in expr.args])
-            return expr.func(*args), ReducerMap.fromdicts(*candidates)
-
-    return run(expr)[0]
+    return _collect_nested(expr)[0]
```

### Comparing `devito-4.8.3/devito/passes/clusters/implicit.py` & `devito-4.8.4/devito/passes/clusters/implicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,18 @@
             if dim not in edims and any(d.dim in edims for d in prefix):
                 processed.append(c)
                 continue
 
             # The IterationSpace induced by the MultiSubDomain
             if dims:
                 intervals = [Interval(i) for i in dims]
-                relations = (ispace0.itdimensions + dims, dims + ispace1.itdimensions)
-                ispaceN = IterationSpace(
-                    IntervalGroup(intervals, relations=relations), sub_iterators
-                )
-                ispace = IterationSpace.union(ispace0, ispaceN)
+                ispaceN = IterationSpace(IntervalGroup(intervals), sub_iterators)
+
+                relations = (ispace0.itdims + dims, dims + ispace1.itdims)
+                ispace = IterationSpace.union(ispace0, ispaceN, relations=relations)
             else:
                 ispaceN = None
                 ispace = ispace0
 
             properties = {i.dim: {SEQUENTIAL} for i in ispace}
 
             if not ispaceN:
@@ -153,15 +152,15 @@
                 if tip is None or tip != nxt:
                     processed.append(
                         c.rebuild(exprs=exprs, ispace=ispace, properties=properties)
                     )
                     tip = nxt
 
             if ispaceN:
-                ispace = IterationSpace.union(c.ispace, ispaceN)
+                ispace = IterationSpace.union(c.ispace, ispaceN, relations=relations)
                 processed.append(c.rebuild(ispace=ispace))
             else:
                 processed.append(c)
             seen.add(d)
 
         return processed
```

### Comparing `devito-4.8.3/devito/passes/clusters/misc.py` & `devito-4.8.4/devito/passes/clusters/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import Counter, defaultdict
 from itertools import groupby, product
 
 from devito.finite_differences import IndexDerivative
 from devito.ir.clusters import Cluster, ClusterGroup, Queue, cluster_pass
 from devito.ir.support import (SEQUENTIAL, SEPARABLE, Scope, ReleaseLock,
                                WaitLock, WithLock, FetchUpdate, PrefetchUpdate)
+from devito.passes.clusters.utils import in_critical_region
 from devito.symbolics import pow_to_mul
 from devito.tools import DAG, Stamp, as_tuple, flatten, frozendict, timed_pass
 from devito.types import Hyperplane
 
 __all__ = ['Lift', 'fuse', 'optimize_pows', 'fission', 'optimize_hyperplanes']
 
 
@@ -21,15 +22,15 @@
     -----
     This is analogous to the compiler transformation known as
     "loop-invariant code motion".
     """
 
     @timed_pass(name='lift')
     def process(self, elements):
-        return super(Lift, self).process(elements)
+        return super().process(elements)
 
     def callback(self, clusters, prefix):
         if not prefix:
             # No iteration space to be lifted from
             return clusters
 
         dim = prefix[-1].dim
@@ -40,16 +41,17 @@
         processed = []
         for n, c in enumerate(clusters):
             # Increments prevent lifting
             if c.has_increments:
                 processed.append(c)
                 continue
 
-            # Synchronization operations prevent lifting
-            if c.syncs.get(dim):
+            # Synchronization prevents lifting
+            if c.syncs.get(dim) or \
+               in_critical_region(c, clusters):
                 processed.append(c)
                 continue
 
             # Is `c` a real candidate -- is there at least one invariant Dimension?
             if any(d._defines & hope_invariant for d in c.used_dimensions):
                 processed.append(c)
                 continue
@@ -182,26 +184,26 @@
         ])
 
         # We allow fusing Clusters/ClusterGroups even in presence of WaitLocks and
         # WithLocks, but not with any other SyncOps
         if isinstance(c, Cluster):
             syncs = (c.syncs,)
         else:
-            syncs = c.syncs
+            syncs = tuple(i.syncs for i in c)
         for i in syncs:
             mapper = defaultdict(set)
             for k, v in i.items():
                 for s in v:
-                    if isinstance(s, (FetchUpdate, PrefetchUpdate)) or \
+                    if isinstance(s, PrefetchUpdate) or \
                        (not self.fusetasks and isinstance(s, WaitLock)):
                         # NOTE: A mix of Clusters w/ and w/o WaitLocks can safely
                         # be fused, as in the worst case scenario the WaitLocks
                         # get "hoisted" above the first Cluster in the sequence
                         continue
-                    elif (isinstance(s, (WaitLock, ReleaseLock)) or
+                    elif (isinstance(s, (FetchUpdate, WaitLock, ReleaseLock)) or
                           (self.fusetasks and isinstance(s, WithLock))):
                         mapper[k].add(type(s))
                     else:
                         mapper[k].add(s)
                 if k in mapper:
                     mapper[k] = frozenset(mapper[k])
             strict.append(frozendict(mapper))
@@ -258,15 +260,15 @@
             group.append(c)
         dump()
 
         # 2) Don't group HaloTouch's
 
         groups, processed = processed, []
         for group in groups:
-            for flag, minigroup in groupby(group, key=lambda c: c.is_halo_touch):
+            for flag, minigroup in groupby(group, key=lambda c: c.is_wild):
                 if flag:
                     processed.extend([(c,) for c in minigroup])
                 else:
                     processed.append(tuple(minigroup))
 
         return processed
 
@@ -303,28 +305,28 @@
                 queue.remove(e)
                 return e
 
             assert False
 
         return ClusterGroup(dag.topological_sort(choose_element), prefix)
 
-    def _build_dag(self, cgroups, prefix, peeking=False):
+    def _build_dag(self, cgroups, prefix):
         """
         A DAG representing the data dependences across the ClusterGroups within
         a given scope.
         """
         prefix = {i.dim for i in as_tuple(prefix)}
 
         dag = DAG(nodes=cgroups)
         for n, cg0 in enumerate(cgroups):
 
-            def is_cross(dep):
+            def is_cross(source, sink):
                 # True if a cross-ClusterGroup dependence, False otherwise
-                t0 = dep.source.timestamp
-                t1 = dep.sink.timestamp
+                t0 = source.timestamp
+                t1 = sink.timestamp
                 v = len(cg0.exprs)
                 return t0 < v <= t1 or t1 < v <= t0
 
             for cg1 in cgroups[n+1:]:
                 # A Scope to compute all cross-ClusterGroup anti-dependences
                 scope = Scope(exprs=cg0.exprs + cg1.exprs, rules=is_cross)
 
@@ -350,17 +352,14 @@
                 elif any(not (i.cause and i.cause & prefix) for i in scope.d_flow_gen()):
                     dag.add_edge(cg0, cg1)
 
                 # Clearly, output dependences must be honored
                 elif any(scope.d_output_gen()):
                     dag.add_edge(cg0, cg1)
 
-            if peeking and dag.edges:
-                return dag
-
         return dag
 
 
 @timed_pass()
 def fuse(clusters, toposort=False, options=None):
     """
     Clusters fusion.
```

### Comparing `devito-4.8.3/devito/passes/clusters/unevaluate.py` & `devito-4.8.4/devito/passes/clusters/unevaluate.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/passes/clusters/utils.py` & `devito-4.8.4/devito/passes/clusters/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+from collections import defaultdict
+
+from devito.ir import Cluster
 from devito.symbolics import uxreplace
-from devito.types import Symbol, Wildcard
+from devito.tools import as_tuple, flatten
+from devito.types import CriticalRegion, Eq, Symbol, Wildcard
 
-__all__ = ['makeit_ssa', 'is_memcpy']
+__all__ = ['makeit_ssa', 'is_memcpy', 'make_critical_sequence',
+           'bind_critical_regions', 'in_critical_region']
 
 
 def makeit_ssa(exprs):
     """
     Convert an iterable of Eqs into Static Single Assignment (SSA) form.
     """
     # Identify recurring LHSs
@@ -44,7 +49,48 @@
     """
     a, b = expr.args
 
     if not (a.is_Indexed and b.is_Indexed):
         return False
 
     return a.function.is_Array or b.function.is_Array
+
+
+def make_critical_sequence(ispace, sequence, **kwargs):
+    sequence = as_tuple(sequence)
+    assert len(sequence) >= 1
+
+    processed = []
+
+    # Opening
+    expr = Eq(Symbol(name='⋈'), CriticalRegion(True))
+    processed.append(Cluster(exprs=expr, ispace=ispace, **kwargs))
+
+    processed.extend(sequence)
+
+    # Closing
+    expr = Eq(Symbol(name='⋈'), CriticalRegion(False))
+    processed.append(Cluster(exprs=expr, ispace=ispace, **kwargs))
+
+    return processed
+
+
+def bind_critical_regions(clusters):
+    """
+    A mapper from CriticalRegions to the critical sequences they open.
+    """
+    critical_region = False
+    mapper = defaultdict(list)
+    for c in clusters:
+        if c.is_critical_region:
+            critical_region = not critical_region and c
+        elif critical_region:
+            mapper[critical_region].append(c)
+    return mapper
+
+
+def in_critical_region(cluster, clusters):
+    """
+    True if `cluster` is part of a critical sequence, False otherwise.
+    """
+    mapper = bind_critical_regions(clusters)
+    return cluster in flatten(mapper.values())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devito-4.8.3/devito/passes/equations/linearity.py` & `devito-4.8.4/devito/passes/equations/linearity.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,24 @@
     """
     processed = []
     for e in expressions:
         # Track type and number of nested Derivatives
         mapper = inspect(e)
 
         # E.g., 0.2*u.dx -> (0.2*u).dx
-        ep = aggregate_coeffs(e, mapper)
+        e1 = aggregate_coeffs(e, mapper)
 
         # E.g., (0.2*u).dx + (0.3*v).dx -> (0.2*u + 0.3*v).dx
-        processed.append(factorize_derivatives(ep))
+        e2 = factorize_derivatives(e1)
+        if e2 == e1:
+            # No luck, stick to `e` to preserve e.g. the original
+            # coefficient factorization
+            processed.append(e)
+        else:
+            processed.append(e2)
 
     return processed
 
 
 # subpass: inspect
 
 @singledispatch
```

### Comparing `devito-4.8.3/devito/passes/iet/asynchrony.py` & `devito-4.8.4/devito/passes/iet/asynchrony.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,102 @@
 from collections import OrderedDict
 from ctypes import c_int
 
 import cgen as c
 
 from devito.ir import (AsyncCall, AsyncCallable, BlankLine, Call, Callable,
-                       Conditional, Dereference, DummyExpr, FindNodes, FindSymbols,
+                       Conditional, DummyExpr, FindNodes, FindSymbols,
                        Iteration, List, PointerCast, Return, ThreadCallable,
-                       Transformer, While, maybe_alias)
+                       Transformer, While, make_callable, maybe_alias)
 from devito.passes.iet.definitions import DataManager
 from devito.passes.iet.engine import iet_pass
 from devito.symbolics import (CondEq, CondNe, FieldFromComposite, FieldFromPointer,
                               Null)
-from devito.tools import DefaultOrderedDict, Bunch, split
-from devito.types import (Lock, Pointer, PThreadArray, QueueID, SharedData, Symbol,
+from devito.tools import split
+from devito.types import (Lock, Pointer, PThreadArray, QueueID, SharedData, Temp,
                           VolatileInt)
 
 __all__ = ['pthreadify']
 
 
 def pthreadify(graph, **kwargs):
-    track = DefaultOrderedDict(lambda: Bunch(threads=None, sdata=None))
+    lower_async_callables(graph, root=graph.root, **kwargs)
 
-    lower_async_callables(graph, track=track, root=graph.root, **kwargs)
+    track = {i.name: i.sdata for i in graph.efuncs.values()
+             if isinstance(i, ThreadCallable)}
     lower_async_calls(graph, track=track, **kwargs)
+
     DataManager(**kwargs).place_definitions(graph)
 
 
 @iet_pass
-def lower_async_callables(iet, track=None, root=None, sregistry=None):
+def lower_async_callables(iet, root=None, sregistry=None):
     if not isinstance(iet, AsyncCallable):
         return iet, {}
 
-    n = len(track)
-
     # Determine the max number of threads that can run this `iet` in parallel
     locks = [i for i in iet.parameters if isinstance(i, Lock)]
     npthreads = min([i.size for i in locks], default=1)
     if npthreads > 1:
         npthreads = sregistry.make_npthreads(npthreads)
 
-    # PthreadArray -- the symbol representing an array of pthreads, which will
-    # execute the AsyncCallable asynchronously
-    threads = track[iet.name].threads = PThreadArray(name='threads',
-                                                     npthreads=npthreads)
-
     # The `cfields` are the constant fields, that is the fields whose value
     # definitely never changes across different executions of `ìet`; the
     # `ncfields` are instead the non-constant fields, that is the fields whose
     # value may or may not change across different calls to `iet`. Clearly objects
     # passed by pointer don't really matter
     fields = iet.parameters
     defines = FindSymbols('defines').visit(root.body)
     ncfields, cfields = split(fields, lambda i: i in defines and i.is_Symbol)
 
     # Postprocess `ncfields`
     ncfields = sanitize_ncfields(ncfields)
 
     # SharedData -- that is the data structure that will be used by the
     # main thread to pass information down to the child thread(s)
-    sdata = track[iet.name].sdata = SharedData(name='sdata',
-                                               npthreads=threads.size,
-                                               cfields=cfields,
-                                               ncfields=ncfields,
-                                               pname='tsdata%d' % n)
-    sbase = sdata.symbolic_base
+    sdata = SharedData(
+        name='sdata',
+        npthreads=npthreads,
+        cfields=cfields,
+        ncfields=ncfields,
+        pname=sregistry.make_name(prefix='tsdata')
+    )
+    sbase = sdata.indexed
 
     # Prepend the SharedData fields available upon thread activation
-    preactions = [DummyExpr(i, FieldFromPointer(i.name, sbase)) for i in ncfields]
+    preactions = [DummyExpr(i, FieldFromPointer(i.base, sbase)) for i in ncfields]
     preactions.append(BlankLine)
 
     # Append the flag reset
     postactions = [List(body=[
         BlankLine,
-        DummyExpr(FieldFromPointer(sdata._field_flag, sbase), 1)
+        DummyExpr(FieldFromPointer(sdata.symbolic_flag, sbase), 1)
     ])]
 
     wrap = List(body=preactions + list(iet.body.body) + postactions)
 
     # The thread has work to do when it receives the signal that all locks have
     # been set to 0 by the main thread
-    wrap = Conditional(CondEq(FieldFromPointer(sdata._field_flag, sbase), 2), wrap)
+    wrap = Conditional(CondEq(FieldFromPointer(sdata.symbolic_flag, sbase), 2), wrap)
 
     # The thread keeps spinning until the alive flag is set to 0 by the main thread
-    wrap = While(CondNe(FieldFromPointer(sdata._field_flag, sbase), 0), wrap)
+    wrap = While(CondNe(FieldFromPointer(sdata.symbolic_flag, sbase), 0), wrap)
 
     # pthread functions expect exactly one argument of type void*
     tparameter = Pointer(name='_%s' % sdata.name)
 
     # Unpack `sdata`
     unpacks = [PointerCast(sdata, tparameter), BlankLine]
     for i in cfields:
         if i.is_AbstractFunction:
-            unpacks.append(Dereference(i, sdata))
+            unpacks.append(
+                DummyExpr(i._C_symbol, FieldFromPointer(i._C_symbol, sbase))
+            )
         else:
-            unpacks.append(DummyExpr(i, FieldFromPointer(i.name, sbase)))
+            unpacks.append(DummyExpr(i, FieldFromPointer(i.base, sbase)))
 
     body = iet.body._rebuild(body=[wrap, Return(Null)], unpacks=unpacks)
     iet = ThreadCallable(iet.name, body, tparameter)
 
     return iet, {'includes': ['pthread.h']}
 
 
@@ -110,40 +109,48 @@
     # Create efuncs to initialize the SharedData objects
     efuncs = OrderedDict()
     for n in FindNodes(AsyncCall).visit(iet):
         if n.name in efuncs:
             continue
 
         assert n.name in track
-        b = track[n.name]
-
-        sdata = b.sdata
-        sbase = sdata.symbolic_base
+        sdata = track[n.name]
+        sbase = sdata.indexed
         name = sregistry.make_name(prefix='init_%s' % sdata.name)
-        body = [DummyExpr(FieldFromPointer(i._C_name, sbase), i._C_symbol)
-                for i in sdata.cfields]
-        body.extend([BlankLine, DummyExpr(FieldFromPointer(sdata._field_flag, sbase), 1)])
+        body = []
+        for i in sdata.cfields:
+            if i.is_AbstractFunction:
+                body.append(
+                    DummyExpr(FieldFromPointer(i._C_symbol, sbase), i._C_symbol)
+                )
+            else:
+                body.append(DummyExpr(FieldFromPointer(i.base, sbase), i.base))
+        body.extend([
+            BlankLine,
+            DummyExpr(FieldFromPointer(sdata.symbolic_flag, sbase), 1)
+        ])
         parameters = sdata.cfields + (sdata,)
         efuncs[n.name] = Callable(name, body, 'void', parameters, 'static')
 
     # Transform AsyncCalls
     nqueues = 1  # Number of allocated asynchronous queues so far
     initialization = []
     finalization = []
     mapper = {}
     for n in FindNodes(AsyncCall).visit(iet):
-        # Create `sdata` and `threads` objects for `n`
-        b = track[n.name]
+        # Bind the abstract `sdata` to `n`
         name = sregistry.make_name(prefix='sdata')
-        sdata = b.sdata._rebuild(name=name)
+        sdata = track[n.name]._rebuild(name=name)
+
+        # The pthreads that will execute the AsyncCallable asynchronously
         name = sregistry.make_name(prefix='threads')
-        threads = b.threads._rebuild(name=name)
+        threads = PThreadArray(name=name, npthreads=sdata.npthreads)
 
         # Call to `sdata` initialization Callable
-        sbase = sdata.symbolic_base
+        sbase = sdata.indexed
         d = threads.index
         arguments = []
         for a in n.arguments:
             if any(maybe_alias(a, i) for i in sdata.ncfields):
                 continue
             elif isinstance(a, QueueID):
                 # Different pthreads use different queues
@@ -152,68 +159,76 @@
                 arguments.append(a)
         # Each pthread has its own SharedData copy
         arguments.append(sbase + d)
         assert len(efuncs[n.name].parameters) == len(arguments)
         call0 = Call(efuncs[n.name].name, arguments)
 
         # Create pthreads
-        tbase = threads.symbolic_base
+        tbase = threads.indexed
         call1 = Call('pthread_create', (
             tbase + d, Null, Call(n.name, [], is_indirect=True), sbase + d
         ))
         nqueues += threads.size
 
         # Glue together the initialization pieces
         if threads.size == 1:
             callback = lambda body: body
         else:
             callback = lambda body: Iteration(body, d, threads.size - 1)
         initialization.append(List(
-            header=c.Comment("Fire up and initialize `%s`" % threads.name),
             body=callback([call0, call1])
         ))
 
         # Finalization
-        finalization.append(List(
-            header=c.Comment("Wait for completion of `%s`" % threads.name),
-            body=callback([
-                While(CondEq(FieldFromComposite(sdata._field_flag, sdata[d]), 2)),
-                DummyExpr(FieldFromComposite(sdata._field_flag, sdata[d]), 0),
-                Call('pthread_join', (threads[d], Null))
-            ])
-        ))
+        name = sregistry.make_name(prefix='shutdown')
+        body = List(body=callback([
+            While(CondEq(FieldFromComposite(sdata.symbolic_flag, sdata[d]), 2)),
+            DummyExpr(FieldFromComposite(sdata.symbolic_flag, sdata[d]), 0),
+            Call('pthread_join', (threads[d], Null))
+        ]))
+        efunc = efuncs[name] = make_callable(name, body)
+        finalization.append(Call(name, efunc.parameters))
 
         # Activation
         if threads.size == 1:
             d = threads.index
-            condition = CondNe(FieldFromComposite(sdata._field_flag, sdata[d]), 1)
+            condition = CondNe(FieldFromComposite(sdata.symbolic_flag, sdata[d]), 1)
             activation = [While(condition)]
         else:
-            d = Symbol(name=sregistry.make_name(prefix=threads.index.name))
-            condition = CondNe(FieldFromComposite(sdata._field_flag, sdata[d]), 1)
+            d = Temp(name=sregistry.make_name(prefix=threads.index.name))
+            condition = CondNe(FieldFromComposite(sdata.symbolic_flag, sdata[d]), 1)
             activation = [DummyExpr(d, 0),
                           While(condition, DummyExpr(d, (d + 1) % threads.size))]
-        activation.extend([DummyExpr(FieldFromComposite(i.name, sdata[d]), i)
+        activation.extend([DummyExpr(FieldFromComposite(i.base, sdata[d]), i)
                            for i in sdata.ncfields])
-        activation.append(DummyExpr(FieldFromComposite(sdata._field_flag, sdata[d]), 2))
-        activation = List(
-            header=[c.Line(), c.Comment("Activate `%s`" % threads.name)],
-            body=activation,
-            footer=c.Line()
+        activation.append(
+            DummyExpr(FieldFromComposite(sdata.symbolic_flag, sdata[d]), 2)
         )
-        mapper[n] = activation
+        name = sregistry.make_name(prefix='activate')
+        efunc = efuncs[name] = make_callable(name, activation)
+        mapper[n] = Call(name, efunc.parameters)
 
     if mapper:
         # Inject activation
         iet = Transformer(mapper).visit(iet)
 
         # Inject initialization and finalization
-        initialization.append(BlankLine)
-        finalization.insert(0, BlankLine)
-        body = iet.body._rebuild(body=initialization + list(iet.body.body) + finalization)
+        initialization = List(
+            header=c.Comment("Fire up and initialize pthreads"),
+            body=initialization + [BlankLine]
+        )
+
+        finalization = List(
+            header=c.Comment("Wait for completion of pthreads"),
+            body=finalization
+        )
+
+        body = iet.body._rebuild(
+            body=[initialization] + list(iet.body.body) + [BlankLine, finalization]
+        )
         iet = iet._rebuild(body=body)
     else:
         assert not initialization
         assert not finalization
 
     return iet, {'efuncs': tuple(efuncs.values())}
```

### Comparing `devito-4.8.3/devito/passes/iet/definitions.py` & `devito-4.8.4/devito/passes/iet/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 
 from collections import OrderedDict
 from functools import singledispatch
 from operator import itemgetter
 
 import numpy as np
 
-from devito.ir import (Block, Call, Definition, DeviceCall, DeviceFunction,
-                       DummyExpr, Return, EntryFunction, FindSymbols, MapExprStmts,
-                       Transformer, make_callable)
-from devito.passes import is_on_device, is_gpu_create
-from devito.passes.iet.engine import iet_pass, iet_visit
+from devito.ir import (Block, Call, Definition, DummyExpr, Return, EntryFunction,
+                       FindSymbols, MapExprStmts, Transformer, make_callable)
+from devito.passes import is_gpu_create
+from devito.passes.iet.engine import iet_pass
 from devito.passes.iet.langbase import LangBB
 from devito.symbolics import (Byref, DefFunction, FieldFromPointer, IndexedPointer,
                               SizeOf, VOID, Keyword, pow_to_mul)
 from devito.tools import as_mapper, as_list, as_tuple, filter_sorted, flatten
 from devito.types import Array, CustomDimension, DeviceMap, DeviceRM, Eq, Symbol
 
 __all__ = ['DataManager', 'DeviceAwareDataManager', 'Storage']
 
 
 class MetaSite(object):
 
-    _items = ('allocs', 'objs', 'frees', 'pallocs', 'pfrees',
-              'maps', 'unmaps', 'efuncs')
+    _items = ('standalones', 'allocs', 'stacks', 'objs', 'frees', 'pallocs',
+              'pfrees', 'maps', 'unmaps', 'efuncs')
 
     def __init__(self):
         for i in self._items:
             setattr(self, i, [])
 
 
 class Storage(OrderedDict):
@@ -70,40 +69,44 @@
 class DataManager(object):
 
     lang = LangBB
     """
     The language used to express data allocations, deletions, and host-device transfers.
     """
 
-    def __init__(self, rcompile=None, sregistry=None, **kwargs):
+    def __init__(self, rcompile=None, sregistry=None, platform=None, **kwargs):
         self.rcompile = rcompile
         self.sregistry = sregistry
+        self.platform = platform
 
     def _alloc_object_on_low_lat_mem(self, site, obj, storage):
         """
         Allocate a LocalObject in the low latency memory.
         """
         decl = Definition(obj)
 
         if obj._C_init:
             definition = (decl, obj._C_init)
         else:
             definition = (decl)
 
         frees = obj._C_free
 
-        storage.update(obj, site, objs=definition, frees=frees)
+        if obj.free_symbols - {obj}:
+            storage.update(obj, site, objs=definition, frees=frees)
+        else:
+            storage.update(obj, site, standalones=definition, frees=frees)
 
     def _alloc_array_on_low_lat_mem(self, site, obj, storage):
         """
         Allocate an Array in the low latency memory.
         """
         alloc = Definition(obj)
 
-        storage.update(obj, site, allocs=alloc)
+        storage.update(obj, site, stacks=alloc)
 
     def _alloc_array_on_global_mem(self, site, obj, storage):
         """
         Allocate an Array in the global memory.
         """
         # Is dynamic initialization required?
         try:
@@ -195,21 +198,21 @@
         frees = as_tuple(free) + as_tuple(frees)
 
         ret = Return(obj._C_symbol)
 
         name = self.sregistry.make_name(prefix='alloc')
         body = (decl, *allocs, init, ret)
         efunc0 = make_callable(name, body, retval=obj)
-        assert len(efunc0.parameters) == 1  # `nbytes_param`
-        alloc = Call(name, nbytes_arg, retobj=obj)
+        args = list(efunc0.parameters)
+        args[args.index(nbytes_param)] = nbytes_arg
+        alloc = Call(name, args, retobj=obj)
 
         name = self.sregistry.make_name(prefix='free')
         efunc1 = make_callable(name, frees)
-        assert len(efunc1.parameters) == 1  # `obj`
-        free = Call(name, obj)
+        free = Call(name, efunc1.parameters)
 
         storage.update(obj, site, allocs=alloc, frees=free, efuncs=(efunc0, efunc1))
 
     def _alloc_object_array_on_low_lat_mem(self, site, obj, storage):
         """
         Allocate an Array of Objects in the low latency memory.
         """
@@ -268,18 +271,20 @@
                 mapper[k] = v
                 continue
 
             assert k.is_Callable
             cbody = k.body
 
             # objects
+            standalones = as_list(cbody.standalones) + flatten(v.standalones)
             objs = as_list(cbody.objs) + flatten(v.objs)
 
             # allocs/pallocs
             allocs = as_list(cbody.allocs) + flatten(v.allocs)
+            stacks = as_list(cbody.stacks) + flatten(v.stacks)
             for tid, body in as_mapper(v.pallocs, itemgetter(0), itemgetter(1)).items():
                 header = self.lang.Region._make_header(tid.symbolic_size)
                 init = self.lang['thread-num'](retobj=tid)
                 allocs.append(Block(header=header, body=[init] + body))
 
             # frees/pfrees
             frees = []
@@ -292,16 +297,18 @@
             # maps/unmaps
             maps = as_list(cbody.maps) + flatten(v.maps)
             unmaps = as_list(cbody.unmaps) + flatten(v.unmaps)
 
             # efuncs
             efuncs.extend(v.efuncs)
 
-            mapper[cbody] = cbody._rebuild(allocs=allocs, maps=maps, objs=objs,
-                                           unmaps=unmaps, frees=frees)
+            mapper[cbody] = cbody._rebuild(
+                standalones=standalones, allocs=allocs, stacks=stacks,
+                maps=maps, objs=objs, unmaps=unmaps, frees=frees
+            )
 
         processed = Transformer(mapper, nested=True).visit(iet)
 
         return processed, flatten(efuncs)
 
     @iet_pass
     def place_definitions(self, iet, globs=None, **kwargs):
@@ -351,15 +358,17 @@
             elif i.is_PointerArray:
                 self._alloc_pointed_array_on_high_bw_mem(iet, i, storage)
 
         # Handle postponed global objects
         includes = set()
         if isinstance(iet, EntryFunction) and globs:
             for i in sorted(globs, key=lambda f: f.name):
-                includes.add(self._alloc_array_on_global_mem(iet, i, storage))
+                v = self._alloc_array_on_global_mem(iet, i, storage)
+                if v:
+                    includes.add(v)
 
         iet, efuncs = self._inject_definitions(iet, storage)
 
         return iet, {'efuncs': efuncs,
                      'globals': as_tuple(globs),
                      'includes': as_tuple(includes)}
 
@@ -480,60 +489,30 @@
         else:
             mmap = self.lang._map_to(obj)
             efunc = ()
             unmap = self.lang._map_delete(obj, devicerm=devicerm)
 
         storage.update(obj, site, maps=mmap, unmaps=unmap, efuncs=efunc)
 
-    @iet_visit
-    def derive_transfers(self, iet):
-        """
-        Collect all symbols that cause host-device data transfer, distinguishing
-        between reads and writes.
-        """
-
-        def needs_transfer(f):
-            return f._mem_mapped and not f.alias and is_on_device(f, self.gpu_fit)
-
-        writes = set()
-        reads = set()
-        for i, v in MapExprStmts().visit(iet).items():
-            if not any(isinstance(j, self.lang.DeviceIteration) for j in v) and \
-               not isinstance(i, DeviceCall) and \
-               not isinstance(iet, DeviceFunction):
-                # Not an offloaded Iteration tree
-                continue
-
-            writes.update({w for w in i.writes if needs_transfer(w)})
-            reads.update({f for f in i.functions
-                          if needs_transfer(f) and f not in writes})
-
-        return (reads, writes)
-
     @iet_pass
-    def place_transfers(self, iet, **kwargs):
+    def place_transfers(self, iet, data_movs=None, **kwargs):
         """
         Create a new IET with host-device data transfers. This requires mapping
         symbols to the suitable memory spaces.
         """
         if not self.pmode:
             return iet, {}
 
         @singledispatch
-        def _place_transfers(iet, mapper):
+        def _place_transfers(iet, data_movs):
             return iet, {}
 
         @_place_transfers.register(EntryFunction)
-        def _(iet, mapper):
-            try:
-                reads, writes = list(zip(*mapper.values()))
-            except ValueError:
-                return iet, {}
-            reads = set(flatten(reads))
-            writes = set(flatten(writes))
+        def _(iet, data_movs):
+            reads, writes = data_movs
 
             # Special symbol which gives user code control over data deallocations
             devicerm = DeviceRM()
 
             storage = Storage()
             for i in filter_sorted(writes):
                 if i.is_Array:
@@ -546,15 +525,15 @@
                 else:
                     self._map_function_on_high_bw_mem(iet, i, storage, devicerm, True)
 
             iet, efuncs = self._inject_definitions(iet, storage)
 
             return iet, {'efuncs': efuncs}
 
-        return _place_transfers(iet, mapper=kwargs['mapper'])
+        return _place_transfers(iet, data_movs=data_movs)
 
     @iet_pass
     def place_devptr(self, iet, **kwargs):
         """
         Transform `iet` such that device pointers are used in DeviceCalls.
         """
         defines = FindSymbols('defines').visit(iet)
@@ -574,19 +553,18 @@
         """
         return iet, {}
 
     def process(self, graph):
         """
         Apply the `place_transfers`, `place_definitions` and `place_casts` passes.
         """
-        mapper = self.derive_transfers(graph)
-        self.place_transfers(graph, mapper=mapper)
+        self.place_transfers(graph, data_movs=graph.data_movs)
         self.place_definitions(graph, globs=set())
         self.place_devptr(graph)
-        self.place_bundling(graph)
+        self.place_bundling(graph, writes_input=graph.writes_input)
         self.place_casts(graph)
 
 
 def make_zero_init(obj):
     cdims = []
     for d, (h0, h1), s in zip(obj.dimensions, obj._size_halo, obj.symbolic_shape):
         if d.is_NonlinearDerived:
```

### Comparing `devito-4.8.3/devito/passes/iet/engine.py` & `devito-4.8.4/devito/passes/iet/engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 from collections import OrderedDict
 from functools import partial, singledispatch, wraps
 
-from devito.ir.iet import (Call, FindNodes, FindSymbols, MetaCall, Transformer,
-                           EntryFunction, ThreadCallable, Uxreplace,
+from devito.ir.iet import (Call, ExprStmt, FindNodes, FindSymbols, MetaCall,
+                           Transformer, EntryFunction, ThreadCallable, Uxreplace,
                            derive_parameters)
 from devito.ir.support import SymbolRegistry
-from devito.tools import DAG, as_tuple, filter_ordered, timed_pass
-from devito.types import (Array, CompositeObject, Lock, IncrDimension, Indirection,
-                          Temp)
+from devito.mpi.distributed import MPINeighborhood
+from devito.passes import needs_transfer
+from devito.symbolics import FieldFromComposite, FieldFromPointer
+from devito.tools import (DAG, as_mapper, as_tuple, filter_ordered,
+                          sorted_priority, timed_pass)
+from devito.types import (Array, Bundle, CompositeObject, Lock, IncrDimension,
+                          Indirection, SharedData, ThreadArray, Temp)
 from devito.types.args import ArgProvider
 from devito.types.dense import DiscreteFunction
 from devito.types.dimension import AbstractIncrDimension, BlockDimension
 
 __all__ = ['Graph', 'iet_pass', 'iet_visit']
 
 
 class Graph(object):
 
     """
-    A special DAG representing call graphs.
+    DAG representation of a call graph.
 
-    The nodes of the graph are IET Callables; an edge from node `a` to node `b`
-    indicates that `b` calls `a`.
+    The nodes of the DAG are IET Callables.
+    An edge from node `a` to node `b` indicates that `b` calls `a`.
 
-    The `apply` method may be used to visit the Graph and apply a transformer `T`
-    to all nodes. This may change the state of the Graph: node `a` gets replaced
-    by `a' = T(a)`; new nodes (Callables), and therefore new edges, may be added.
+    The `apply` method visits the Graph and applies a transformation `T`
+    to all nodes. This may change the state of the Graph:
+
+        * Node `a` gets replaced by `a' = T(a)`.
+        * New nodes (Callables) may be added.
+          * Consequently, edges are added.
+        * New global objects may be introduced:
+          * Global symbols, header files, ...
 
     The `visit` method collects info about the nodes in the Graph.
     """
 
-    def __init__(self, iet, sregistry=None):
+    def __init__(self, iet, options=None, sregistry=None, **kwargs):
         self.efuncs = OrderedDict([(iet.name, iet)])
 
         self.sregistry = sregistry
 
         self.includes = []
         self.headers = []
+        self.namespaces = []
         self.globals = []
 
+        # Stash immutable information useful for one or more compiler passes
+
+        # All written user-level objects
+        writes = FindSymbols('writes').visit(iet)
+        self.writes_input = frozenset(f for f in writes if f.is_Input)
+
+        # All symbols requiring host-device data transfers when running
+        # on device
+        self.data_movs = rmovs, wmovs = set(), set()
+        gpu_fit = (options or {}).get('gpu-fit', ())
+        for i in FindNodes(ExprStmt).visit(iet):
+            wmovs.update({w for w in i.writes
+                          if needs_transfer(w, gpu_fit)})
+        for i in FindNodes(ExprStmt).visit(iet):
+            rmovs.update({f for f in i.functions
+                          if needs_transfer(f, gpu_fit) and f not in wmovs})
+
     @property
     def root(self):
         return self.efuncs[list(self.efuncs).pop(0)]
 
     @property
     def funcs(self):
         return tuple(MetaCall(v, True) for v in self.efuncs.values())[1:]
@@ -50,47 +77,55 @@
     def apply(self, func, **kwargs):
         """
         Apply `func` to all nodes in the Graph. This changes the state of the Graph.
         """
         dag = create_call_graph(self.root.name, self.efuncs)
 
         # Apply `func`
+        efuncs = dict(self.efuncs)
         for i in dag.topological_sort():
-            efunc, metadata = func(self.efuncs[i], **kwargs)
+            efunc, metadata = func(efuncs[i], **kwargs)
 
             self.includes.extend(as_tuple(metadata.get('includes')))
             self.headers.extend(as_tuple(metadata.get('headers')))
+            self.namespaces.extend(as_tuple(metadata.get('namespaces')))
             self.globals.extend(as_tuple(metadata.get('globals')))
 
             # Update jit-compiler if necessary
             try:
                 compiler = kwargs['compiler']
                 compiler.add_include_dirs(as_tuple(metadata.get('include_dirs')))
                 compiler.add_libraries(as_tuple(metadata.get('libs')))
                 compiler.add_library_dirs(as_tuple(metadata.get('lib_dirs')))
             except KeyError:
                 pass
 
-            if efunc is self.efuncs[i]:
+            if efunc is efuncs[i]:
                 continue
 
-            # Minimize code size by abstracting semantically identical efuncs
-            efunc, efuncs = reuse_efuncs(efunc, metadata.get('efuncs', []),
-                                         self.sregistry)
+            new_efuncs = metadata.get('efuncs', [])
 
-            self.efuncs[i] = efunc
-            self.efuncs.update(OrderedDict([(i.name, i) for i in efuncs]))
+            efuncs[i] = efunc
+            efuncs.update(OrderedDict([(i.name, i) for i in new_efuncs]))
 
             # Update the parameters / arguments lists since `func` may have
             # introduced or removed objects
-            self.efuncs = update_args(efunc, self.efuncs, dag)
+            efuncs = update_args(efunc, efuncs, dag)
+
+        # Minimize code size
+        if len(efuncs) > len(self.efuncs):
+            efuncs = reuse_compounds(efuncs, self.sregistry)
+            efuncs = reuse_efuncs(self.root, efuncs, self.sregistry)
+
+        self.efuncs = efuncs
 
         # Uniqueness
         self.includes = filter_ordered(self.includes)
         self.headers = filter_ordered(self.headers, key=str)
+        self.namespaces = filter_ordered(self.namespaces, key=str)
         self.globals = filter_ordered(self.globals)
 
     def visit(self, func, **kwargs):
         """
         Apply `func` to all nodes in the Graph. `func` gathers info about the
         state of each node. The gathered info is returned to the called as a mapper
         from nodes to info. Unlike `apply`, `visit` does not change the state
@@ -115,14 +150,20 @@
     @wraps(func)
     def wrapper(*args, **kwargs):
         if timed_pass.is_enabled():
             maybe_timed = timed_pass
         else:
             maybe_timed = lambda func, name: func
         try:
+            # If the pass has been disabled, skip it
+            if not kwargs['options'][func.__name__]:
+                return
+        except KeyError:
+            pass
+        try:
             # Pure function case
             graph, = args
             return maybe_timed(call(graph), func.__name__)(func, **kwargs)
         except ValueError:
             # Instance method case
             self, graph = args
             return maybe_timed(call(graph), func.__name__)(partial(func, self), **kwargs)
@@ -157,14 +198,90 @@
 
     # Sanity check
     assert dag.size == len(efuncs)
 
     return dag
 
 
+def reuse_compounds(efuncs, sregistry=None):
+    """
+    Generalise `efuncs` so that groups of semantically identical compound types
+    are replaced with a unique compound type, thus maximizing code reuse.
+
+    For example, given two C structs originating from e.g. a CompositeObject
+
+        struct foo {int a, char v}
+        struct bar {int g, char e}
+
+    Reduce them to:
+
+        struct foo {int a, char v}
+
+    Which requires replacing all references to `bar` with the new `foo`. Note that
+    in this case the transformed `foo` is also syntactically identical to the
+    input `foo`, but this isn't necessarily the case.
+    """
+    mapper = {}
+    for efunc in efuncs.values():
+        local_sregistry = SymbolRegistry()
+        for i in FindSymbols().visit(efunc):
+            abstract_compound(i, mapper, local_sregistry)
+
+    key = lambda i: mapper[i]._C_ctype
+    subs = {}
+    for v in as_mapper(mapper, key).values():
+        if len(v) == 1:
+            continue
+
+        # Recreate now using a globally unique type name
+        abstract_compound(v[0], subs, sregistry)
+        base = subs[v[0]]
+
+        subs.update({i: base._rebuild(name=mapper[i].name) for i in v})
+
+    # Replace all occurrences in the form of FieldFrom{Composite,Pointer}
+    mapper = {}
+    for i0, i1 in subs.items():
+        b0, b1 = i0.indexed, i1.indexed
+
+        mapper.update({i0: i1, b0: b1})
+
+        for f0, f1 in zip(i0.fields, i1.fields):
+            for cls in (FieldFromComposite, FieldFromPointer):
+                if f0.is_AbstractFunction:
+                    mapper[cls(f0._C_symbol, b0)] = cls(f1._C_symbol, b1)
+                else:
+                    mapper[cls(f0.base, b0)] = cls(f1.base, b1)
+
+    if mapper:
+        efuncs = {i: Uxreplace(mapper).visit(efunc) for i, efunc in efuncs.items()}
+
+    return efuncs
+
+
+@singledispatch
+def abstract_compound(i, mapper, sregistry):
+    """
+    Singledispatch-based implementation of type abstraction.
+    """
+    return
+
+
+@abstract_compound.register(SharedData)
+def _(i, mapper, sregistry):
+    pname = sregistry.make_name(prefix="tsd")
+
+    m = abstract_objects(i.fields)
+    cfields = [m.get(i, i) for i in i.cfields]
+    ncfields = [m.get(i, i) for i in i.ncfields]
+
+    mapper[i] = i._rebuild(cfields=cfields, ncfields=ncfields, pname=pname,
+                           function=None)
+
+
 def reuse_efuncs(root, efuncs, sregistry=None):
     """
     Generalise `efuncs` so that syntactically identical Callables may be dropped,
     thus maximizing code reuse.
 
     For example, given two Callables
 
@@ -178,16 +295,14 @@
     The call sites in `root` are transformed accordingly.
     """
     # Topological sorting ensures that nested Calls are abstract first.
     # For example, given `[foo0(u(x)): bar0(u), foo1(u(x)): bar1(u)]`,
     # assuming that `bar0` and `bar1` are compatible, we first process the
     # `bar`'s to obtain `[foo0(u(x)): bar0(u), foo1(u(x)): bar0(u)]`,
     # and finally `foo0(u(x)): bar0(u)`
-    efuncs = {i.name: i for i in efuncs}
-    efuncs[root.name] = root
     dag = create_call_graph(root.name, efuncs)
 
     mapper = {}
     for i in dag.topological_sort():
         if i == root.name:
             continue
 
@@ -208,19 +323,20 @@
                         if c.name == efuncs[i].name}
                 efuncs[n] = Transformer(subs).visit(efuncs[n])
 
         except KeyError:
             afunc = afunc._rebuild(name=efunc.name)
             mapper[key] = (afunc, [efunc])
 
-    root = efuncs.pop(root.name)
-    processed = [afunc if len(efuncs) > 1 else efuncs.pop()
-                 for afunc, efuncs in mapper.values()]
+    processed = [afunc if len(v) > 1 else v.pop() for afunc, v in mapper.values()]
 
-    return root, processed
+    retval = {root.name: efuncs[root.name]}
+    retval.update({i.name: i for i in processed})
+
+    return retval
 
 
 def abstract_efunc(efunc):
     """
     Abstract `efunc` applying a set of rules:
 
         * The `efunc` names becomes "foo".
@@ -242,43 +358,34 @@
 def abstract_objects(objects, sregistry=None):
     """
     Proxy for `abstract_object`.
     """
     # Precedence rules make it possible to reconstruct objects that depend on
     # higher priority objects
     priority = {
-        DiscreteFunction: 1,
-        AbstractIncrDimension: 2,
-        BlockDimension: 3,
+        Array: 1,
+        DiscreteFunction: 2,
+        AbstractIncrDimension: 3,
+        BlockDimension: 4,
     }
-
-    def key(i):
-        for cls in sorted(priority, key=priority.get, reverse=True):
-            if isinstance(i, cls):
-                return priority[cls]
-        return 0
-
-    objects = sorted(objects, key=key, reverse=True)
+    objects = sorted_priority(objects, priority)
 
     # Build abstraction mappings
     mapper = {}
     sregistry = sregistry or SymbolRegistry()
     for i in objects:
         abstract_object(i, mapper, sregistry)
 
     return mapper
 
 
 @singledispatch
 def abstract_object(i, mapper, sregistry):
     """
     Singledispatch-based implementation of object abstraction.
-
-    Singledispatch allows foreign modules to specify their own rules for
-    object abstraction.
     """
     return
 
 
 @abstract_object.register(DiscreteFunction)
 def _(i, mapper, sregistry):
     name = sregistry.make_name(prefix='f')
@@ -290,38 +397,62 @@
         i.indexed: v.indexed,
         i.dmap: v.dmap,
         i._C_symbol: v._C_symbol,
     })
 
 
 @abstract_object.register(Array)
+@abstract_object.register(Bundle)
 def _(i, mapper, sregistry):
     if isinstance(i, Lock):
         name = sregistry.make_name(prefix='lock')
     else:
         name = sregistry.make_name(prefix='a')
 
-    v = i._rebuild(name=name)
+    v = i._rebuild(name=name, alias=True)
 
     mapper.update({
         i: v,
         i.indexed: v.indexed,
         i._C_symbol: v._C_symbol,
     })
+    if i.dmap is not None:
+        mapper[i.dmap] = v.dmap
 
 
 @abstract_object.register(CompositeObject)
 def _(i, mapper, sregistry):
     name = sregistry.make_name(prefix='o')
 
     v = i._rebuild(name)
 
     mapper[i] = v
 
 
+@abstract_object.register(ThreadArray)
+def _(i, mapper, sregistry):
+    if isinstance(i, SharedData):
+        name = sregistry.make_name(prefix='sd')
+    else:
+        name = sregistry.make_name(prefix='pta')
+
+    v = i._rebuild(name=name)
+
+    mapper.update({
+        i: v,
+        i.indexed: v.indexed,
+        i._C_symbol: v._C_symbol,
+    })
+
+
+@abstract_object.register(MPINeighborhood)
+def _(i, mapper, sregistry):
+    mapper[i] = i._rebuild()
+
+
 @abstract_object.register(BlockDimension)
 def _(i, mapper, sregistry):
     if i._depth != 2:
         return
 
     p = i.parent
     pp = i.parent.parent
@@ -396,54 +527,57 @@
         foo(..., z) : root(x, z)
     """
     if isinstance(root, ThreadCallable):
         return efuncs
 
     # The parameters/arguments lists may have changed since a pass may have:
     # 1) introduced a new symbol
-    new_args = derive_parameters(root)
+    new_params = derive_parameters(root)
 
     # 2) defined a symbol for which no definition was available yet (e.g.
     # via a malloc, or a Dereference)
     defines = FindSymbols('defines').visit(root.body)
-    drop_args = [a for a in root.parameters if a in defines]
+    drop_params = [a for a in root.parameters if a in defines]
 
     # 3) removed a symbol that was previously necessary (e.g., `x_size` after
     # linearization)
     symbols = FindSymbols('basics').visit(root.body)
-    drop_args.extend(a for a in root.parameters if a.is_Symbol and a not in symbols)
+    drop_params.extend(a for a in root.parameters
+                       if a.is_Symbol and a not in symbols)
 
-    if not (new_args or drop_args):
+    # Must record the index, not the param itself, since a param may be
+    # bound to whatever arg, possibly a generic SymPy expr
+    drop_params = [root.parameters.index(a) for a in drop_params]
+
+    if not (new_params or drop_params):
         return efuncs
 
+    # Create the new parameters and arguments lists
+
     def _filter(v, efunc=None):
-        processed = list(v)
-        for a in new_args:
+        processed = [a for i, a in enumerate(v) if i not in drop_params]
+
+        for a in new_params:
             if a in processed:
                 # A child efunc trying to add a symbol alredy added by a
                 # sibling efunc
                 continue
 
             if isinstance(efunc, EntryFunction) and not isinstance(a, ArgProvider):
                 # Temporaries (e.g., Arrays) *cannot* be arguments of an
                 # EntryFunction. So if we end up here, `a` remains for
                 # now undefined inside `efunc`
                 continue
 
             processed.append(a)
 
-        processed = [a for a in processed if a not in drop_args]
-
         return processed
 
     efuncs = OrderedDict(efuncs)
-
-    # Update to use the new signature
-    parameters = _filter(root.parameters, root)
-    efuncs[root.name] = root._rebuild(parameters=parameters)
+    efuncs[root.name] = root._rebuild(parameters=_filter(root.parameters, root))
 
     # Update all call sites to use the new signature
     for n in dag.downstream(root.name):
         mapper = {c: c._rebuild(arguments=_filter(c.arguments))
                   for c in FindNodes(Call).visit(efuncs[n])
                   if c.name == root.name}
         efuncs[n] = Transformer(mapper).visit(efuncs[n])
```

### Comparing `devito-4.8.3/devito/passes/iet/langbase.py` & `devito-4.8.4/devito/passes/iet/langbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from functools import singledispatch
+from itertools import takewhile
 from abc import ABC
 
 import cgen as c
 
 from devito.data import FULL
 from devito.ir import (DummyExpr, Call, Conditional, Expression, List, Prodder,
                        ParallelIteration, ParallelBlock, PointerCast, EntryFunction,
-                       AsyncCallable, FindNodes, FindSymbols)
+                       AsyncCallable, FindNodes, FindSymbols, IsPerfectIteration)
 from devito.mpi.distributed import MPICommObject
 from devito.passes import is_on_device
 from devito.passes.iet.engine import iet_pass
 from devito.symbolics import Byref, CondNe, SizeOf
-from devito.tools import as_list, prod
+from devito.tools import as_list, is_integer, prod
 from devito.types import Symbol, QueueID, Wildcard
 
 __all__ = ['LangBB', 'LangTransformer']
 
 
 class LangMeta(type):
 
@@ -156,15 +157,16 @@
     """
 
     def __init__(self, key, sregistry, platform, compiler):
         """
         Parameters
         ----------
         key : callable, optional
-            Return True if an Iteration can and should be parallelized, False otherwise.
+            Return True if an Iteration can and should be parallelized,
+            False otherwise.
         sregistry : SymbolRegistry
             The symbol registry, to access the symbols appearing in an IET.
         platform : Platform
             The underlying platform.
         compiler : Compiler
             The underlying JIT compiler.
         """
@@ -211,14 +213,177 @@
         return self.lang.DeviceIteration
 
     @property
     def Prodder(self):
         return self.lang.Prodder
 
 
+class ShmTransformer(LangTransformer):
+
+    """
+    Abstract base class for LangTransformers that want to emit
+    shared-memory-parallel IETs for CPUs.
+    """
+
+    def __init__(self, key, sregistry, options, platform, compiler):
+        """
+        Parameters
+        ----------
+        key : callable, optional
+            Return True if an Iteration can and should be parallelized,
+            False otherwise.
+        sregistry : SymbolRegistry
+            The symbol registry, to access the symbols appearing in an IET.
+        options : dict
+             The optimization options.
+             Accepted: ['par-collapse-ncores', 'par-collapse-work',
+             'par-chunk-nonaffine', 'par-dynamic-work', 'par-nested']
+             * 'par-collapse-ncores': use a collapse clause if the number of
+               available physical cores is greater than this threshold.
+             * 'par-collapse-work': use a collapse clause if the trip count of the
+               collapsable Iterations is statically known to exceed this threshold.
+             * 'par-chunk-nonaffine': coefficient to adjust the chunk size in
+               non-affine parallel Iterations.
+             * 'par-dynamic-work': use dynamic scheduling if the operation count per
+               iteration exceeds this threshold. Otherwise, use static scheduling.
+             * 'par-nested': nested parallelism if the number of hyperthreads
+               per core is greater than this threshold.
+        platform : Platform
+            The underlying platform.
+        compiler : Compiler
+            The underlying JIT compiler.
+        """
+        super().__init__(key, sregistry, platform, compiler)
+
+        self.collapse_ncores = options['par-collapse-ncores']
+        self.collapse_work = options['par-collapse-work']
+        self.chunk_nonaffine = options['par-chunk-nonaffine']
+        self.dynamic_work = options['par-dynamic-work']
+        self.nested = options['par-nested']
+
+    @property
+    def ncores(self):
+        return self.platform.cores_physical
+
+    @property
+    def nhyperthreads(self):
+        return self.platform.threads_per_core
+
+    @property
+    def nthreads(self):
+        return self.sregistry.nthreads
+
+    @property
+    def nthreads_nested(self):
+        return self.sregistry.nthreads_nested
+
+    @property
+    def nthreads_nonaffine(self):
+        return self.sregistry.nthreads_nonaffine
+
+    @property
+    def threadid(self):
+        return self.sregistry.threadid
+
+    def _score_candidate(self, n0, root, collapsable=()):
+        """
+        The score of a collapsable nest depends on the number of fully-parallel
+        Iterations and their position in the nest (the outer, the better).
+        """
+        nest = [root] + list(collapsable)
+        n = len(nest)
+
+        # Number of fully-parallel collapsable Iterations
+        key = lambda i: i.is_ParallelNoAtomic
+        fp_iters = list(takewhile(key, nest))
+        n_fp_iters = len(fp_iters)
+
+        # Number of parallel-if-atomic collapsable Iterations
+        key = lambda i: i.is_ParallelAtomic
+        pia_iters = list(takewhile(key, nest))
+        n_pia_iters = len(pia_iters)
+
+        # Prioritize the Dimensions that are more likely to define larger
+        # iteration spaces
+        key = lambda d: (not d.is_Derived or
+                         (d.is_Custom and not is_integer(d.symbolic_size)) or
+                         (d.is_Block and d._depth == 1))
+
+        fpdims = [i.dim for i in fp_iters]
+        n_fp_iters_large = len([d for d in fpdims if key(d)])
+
+        piadims = [i.dim for i in pia_iters]
+        n_pia_iters_large = len([d for d in piadims if key(d)])
+
+        return (
+            int(n_fp_iters == n),  # Fully-parallel nest
+            n_fp_iters_large,
+            n_fp_iters,
+            n_pia_iters_large,
+            n_pia_iters,
+            -(n0 + 1),  # The outer, the better
+            n,
+        )
+
+    def _select_candidates(self, candidates):
+        assert candidates
+
+        if self.ncores < self.collapse_ncores:
+            return candidates[0], []
+
+        mapper = {}
+        for n0, root in enumerate(candidates):
+
+            # Score `root` in isolation
+            mapper[(root, ())] = self._score_candidate(n0, root)
+
+            collapsable = []
+            for n, i in enumerate(candidates[n0+1:], n0+1):
+                # The Iteration nest [root, ..., i] must be perfect
+                if not IsPerfectIteration(depth=i).visit(root):
+                    break
+
+                # Loops are collapsable only if none of the iteration variables
+                # appear in initializer expressions. For example, the following
+                # two loops cannot be collapsed
+                #
+                # for (i = ... )
+                #   for (j = i ...)
+                #     ...
+                #
+                # Here, we make sure this won't happen
+                if any(j.dim in i.symbolic_min.free_symbols for j in candidates[n0:n]):
+                    break
+
+                # Can't collapse SIMD-vectorized Iterations
+                if i.is_Vectorized:
+                    break
+
+                # Would there be enough work per parallel iteration?
+                nested = candidates[n+1:]
+                if nested:
+                    try:
+                        work = prod([int(j.dim.symbolic_size) for j in nested])
+                        if work < self.collapse_work:
+                            break
+                    except TypeError:
+                        pass
+
+                collapsable.append(i)
+
+                # Score `root + collapsable`
+                v = tuple(collapsable)
+                mapper[(root, v)] = self._score_candidate(n0, root, v)
+
+        # Retrieve the candidates with highest score
+        root, collapsable = max(mapper, key=mapper.get)
+
+        return root, list(collapsable)
+
+
 class DeviceAwareMixin(object):
 
     @property
     def deviceid(self):
         return self.sregistry.deviceid
 
     @iet_pass
```

### Comparing `devito-4.8.3/devito/passes/iet/languages/C.py` & `devito-4.8.4/devito/passes/iet/languages/C.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/passes/iet/languages/openacc.py` & `devito-4.8.4/devito/passes/iet/languages/openacc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import cgen as c
 import numpy as np
 
 from devito.arch import AMDGPUX, NVIDIAX
 from devito.ir import (Call, DeviceCall, DummyExpr, EntryFunction, List, Block,
                        ParallelTree, Pragma, Return, FindSymbols, make_callable)
-from devito.passes import is_on_device
+from devito.passes import needs_transfer, is_on_device
 from devito.passes.iet.definitions import DeviceAwareDataManager
 from devito.passes.iet.engine import iet_pass
 from devito.passes.iet.orchestration import Orchestrator
 from devito.passes.iet.parpragma import (PragmaDeviceAwareTransformer, PragmaLangBB,
                                          PragmaIteration, PragmaTransfer)
 from devito.passes.iet.languages.C import CBB
 from devito.passes.iet.languages.openmp import OmpRegion, OmpIteration
 from devito.symbolics import FieldFromPointer, Macro, cast_mapper
-from devito.tools import filter_ordered
-from devito.types import DeviceMap, Symbol
+from devito.tools import filter_ordered, UnboundTuple
+from devito.types import Symbol
 
 __all__ = ['DeviceAccizer', 'DeviceAccDataManager', 'AccOrchestrator']
 
 
 class DeviceAccIteration(PragmaIteration):
 
     @classmethod
@@ -26,15 +26,16 @@
         return 'acc parallel loop'
 
     @classmethod
     def _make_clauses(cls, ncollapsed=0, reduction=None, tile=None, **kwargs):
         clauses = []
 
         if tile:
-            clauses.append('tile(%s)' % ','.join(str(i) for i in tile))
+            stile = [str(tile[i]) for i in range(ncollapsed)]
+            clauses.append('tile(%s)' % ','.join(stile))
         elif ncollapsed > 1:
             clauses.append('collapse(%d)' % ncollapsed)
 
         if reduction:
             clauses.append(cls._make_clause_reduction_from_imask(reduction))
 
         indexeds = FindSymbols('indexeds').visit(kwargs['nodes'])
@@ -155,26 +156,21 @@
 
     lang = AccBB
 
     def _make_partree(self, candidates, nthreads=None):
         assert candidates
 
         root, collapsable = self._select_candidates(candidates)
-        ncollapsable = len(collapsable)
+        ncollapsable = len(collapsable) + 1
 
         if self._is_offloadable(root) and \
            all(i.is_Affine for i in [root] + collapsable) and \
            self.par_tile:
-            tile = self.par_tile.next()
-            assert isinstance(tile, tuple)
-            nremainder = (ncollapsable + 1) - len(tile)
-            if nremainder >= 0:
-                tile += (tile[-1],)*nremainder
-            else:
-                tile = tile[:ncollapsable + 1]
+            tile = self.par_tile.nextitem()
+            assert isinstance(tile, UnboundTuple)
 
             body = self.DeviceIteration(gpu_fit=self.gpu_fit, tile=tile,
                                         ncollapsed=ncollapsable, **root.args)
             partree = ParallelTree([], body, nthreads=nthreads)
 
             return root, partree
         else:
@@ -214,21 +210,21 @@
             }
 
         This method creates an IET along the lines of the code snippet above.
         """
         if not isinstance(iet, EntryFunction):
             return iet, {}
 
-        dmaps = [i for i in FindSymbols('basics').visit(iet)
-                 if isinstance(i, DeviceMap)]
+        symbols = FindSymbols('basics').visit(iet)
+        functions = [f for f in symbols if needs_transfer(f, self.gpu_fit)]
 
         efuncs = []
         calls = []
-        for dmap in filter_ordered(dmaps):
-            f = dmap.function
+        for f in functions:
+            dmap = f.dmap
             hp = f.indexed
 
             tdp = Symbol(name="dptr", dtype=np.uint64)
             init = DummyExpr(tdp, 0, init=True)
 
             dpf = List(body=[
                 Pragma(self.lang.mapper['map-serial-present'], (hp, tdp)),
@@ -242,15 +238,18 @@
             ret = Return(ctdp)
 
             body = List(body=[init, dpf, cast, ret])
 
             name = self.sregistry.make_name(prefix='map_device_ptr')
             efuncs.append(make_callable(name, body, retval=hp))
 
-            calls.append(Call(name, f, retobj=dmap))
+            if dmap in symbols:
+                calls.append(Call(name, f, retobj=dmap))
+            else:
+                calls.append(Call(name, f))
 
         body = iet.body._rebuild(maps=iet.body.maps + tuple(calls))
         iet = iet._rebuild(body=body)
 
         return iet, {'efuncs': efuncs}
```

### Comparing `devito-4.8.3/devito/passes/iet/languages/openmp.py` & `devito-4.8.4/devito/passes/iet/languages/openmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from packaging.version import Version
 
 import cgen as c
 from sympy import And, Ne, Not
 
-from devito.arch import AMDGPUX, NVIDIAX, INTELGPUX
+from devito.arch import AMDGPUX, NVIDIAX, INTELGPUX, PVC
 from devito.arch.compiler import GNUCompiler
 from devito.ir import (Call, Conditional, DeviceCall, List, Prodder,
                        ParallelBlock, PointerCast, While, FindSymbols)
 from devito.passes.iet.definitions import DataManager, DeviceAwareDataManager
 from devito.passes.iet.langbase import LangBB
 from devito.passes.iet.orchestration import Orchestrator
 from devito.passes.iet.parpragma import (PragmaSimdTransformer, PragmaShmTransformer,
@@ -74,22 +74,14 @@
         indexeds = FindSymbols('indexeds').visit(kwargs['nodes'])
         deviceptrs = filter_ordered(i.name for i in indexeds if i.function._mem_local)
         if deviceptrs:
             clauses.append("is_device_ptr(%s)" % ",".join(deviceptrs))
 
         return clauses
 
-    @classmethod
-    def _process_kwargs(cls, **kwargs):
-        kwargs = super()._process_kwargs(**kwargs)
-
-        kwargs.pop('gpu_fit', None)
-
-        return kwargs
-
 
 class ThreadedProdder(Conditional, Prodder):
 
     _traversable = []
 
     def __init__(self, prodder, arguments=None):
         # Atomic-ize any single-thread Prodders in the parallel tree
@@ -113,14 +105,15 @@
         # Misc
         'name': 'OpenMP',
         'header': 'omp.h',
         # Platform mapping
         AMDGPUX: None,
         NVIDIAX: None,
         INTELGPUX: None,
+        PVC: None,
         # Runtime library
         'init': None,
         'thread-num': lambda retobj=None:
             Call('omp_get_thread_num', retobj=retobj),
         # Pragmas
         'simd-for': c.Pragma('omp simd'),
         'simd-for-aligned': lambda i, j: c.Pragma('omp simd aligned(%s:%d)' % (i, j)),
```

### Comparing `devito-4.8.3/devito/passes/iet/languages/targets.py` & `devito-4.8.4/devito/passes/iet/languages/targets.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/passes/iet/linearization.py` & `devito-4.8.4/devito/passes/iet/linearization.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,193 +8,292 @@
 from devito.data import FULL
 from devito.ir import (BlankLine, Call, DummyExpr, Dereference, List, PointerCast,
                        Transfer, FindNodes, FindSymbols, Transformer, Uxreplace,
                        IMask)
 from devito.passes.iet.engine import iet_pass
 from devito.passes.iet.parpragma import PragmaIteration
 from devito.symbolics import DefFunction, MacroArgument, ccode
-from devito.tools import Bunch, filter_ordered, prod
+from devito.tools import Bunch, filter_ordered, flatten, prod
 from devito.types import Array, Bundle, Symbol, FIndexed, Indexed, Wildcard
-from devito.types.basic import IndexedData
 from devito.types.dense import DiscreteFunction
 
-
 __all__ = ['linearize']
 
 
 def linearize(graph, **kwargs):
     """
     Turn n-dimensional Indexeds into 1-dimensional Indexed with suitable index
     access function, such as `a[i, j] -> a[i*n + j]`. The row-major format
     of the underlying Function objects is honored.
     """
+    sregistry = kwargs.get('sregistry')
     options = kwargs.get('options', {})
-    lmode = kwargs.pop('lmode', options.get('linearize'))
-    if not lmode:
+
+    mode = options.get('linearize')
+    maybe_callback = kwargs.pop('callback', mode)
+
+    if not maybe_callback:
         return
+    elif callable(maybe_callback):
+        key = lambda f: maybe_callback(f) and f.ndim > 1 and not f._mem_stack
+    else:
+        key = lambda f: f.is_AbstractFunction and f.ndim > 1 and not f._mem_stack
+
+    if options['index-mode'] == 'int32':
+        dtype = np.int32
+    else:
+        dtype = np.int64
 
-    # All information that need to be propagated across callables
-    tracker = Bunch(
-        sizes={},
-        strides={},
-        undef=defaultdict(set),
-        subs={},
-        headers={}
-    )
+    # NOTE: Even if `mode=False`, `key` may still want to enforce linearization
+    # of some Functions, so it takes precedence and we then attempt to linearize
+    if not mode or isinstance(mode, bool):
+        mode = 'basic'
 
-    linearization(graph, lmode=lmode, tracker=tracker, **kwargs)
+    tracker = Tracker(mode, dtype, sregistry)
+
+    linearization(graph, key=key, tracker=tracker, **kwargs)
 
     # Sanity check
     assert not tracker.undef
 
 
 @iet_pass
-def linearization(iet, lmode=None, tracker=None, **kwargs):
+def linearization(iet, key=None, tracker=None, **kwargs):
     """
     Carry out the actual work of `linearize`.
     """
-    # `lmode` may be a callback describing what Function types, and under what
-    # conditions, should linearization be applied
-    if callable(lmode):
-        key0 = lambda f: lmode(f) and f.ndim > 1
-    else:
-        # Default
-        key0 = lambda f: f.is_AbstractFunction and f.ndim > 1
-    key = lambda f: key0(f) and not f._mem_stack
-
-    iet = linearize_accesses(iet, key, tracker, **kwargs)
+    iet = linearize_accesses(iet, key, tracker)
     iet = linearize_pointers(iet, key)
     iet = linearize_transfers(iet, **kwargs)
     iet = linearize_clauses(iet, **kwargs)
 
     # Postprocess headers
-    headers = [(ccode(define), ccode(expr)) for define, expr in tracker.headers.values()]
+    headers = sorted((ccode(i), ccode(e)) for i, e in tracker.headers.values())
 
     return iet, {'headers': headers}
 
 
 def key1(f, d):
     """
     A key for Function dimensions. The key is:
 
         * False if not statically linearizable, that is not linearizable via
           constant symbolic sizes and strides;
         * A 3-tuple `(Dimension, halo size, grid)` otherwise.
     """
     if f.is_regular:
-        # TODO: same grid + same halo => same padding, however this is not asserted
-        # during compilation... so maybe we should do it at `prepare_args` time?
-        return (d, f._size_halo[d], getattr(f, 'grid', None))
+        # For paddable objects the following holds:
+        # `same dim + same halo => same (auto-)padding`
+        return (d, f._size_halo[d], f.is_autopaddable)
     else:
         return False
 
 
-def linearize_accesses(iet, key0, tracker=None, sregistry=None, options=None,
-                       **kwargs):
+class Size(Symbol):
+
     """
-    Turn Indexeds into FIndexeds and create the necessary access Macros.
+    Symbol representing the size of a Function dimension.
     """
-    if options['index-mode'] == 'int32':
-        dtype = np.int32
-    else:
-        dtype = np.int64
 
-    # 1) What `iet` *needs*
-    indexeds = FindSymbols('indexeds').visit(iet)
-    needs = filter_ordered(i.function for i in indexeds if key0(i.function))
-    needs = sorted(needs, key=lambda f: len(f.dimensions), reverse=True)
+    pass
 
-    # Update unique sizes table
-    # E.g. `{(x, 8, grid) -> x_fsz0}`
-    for f in needs:
-        # NOTE: the outermost dimension is unnecessary
+
+class Stride(Symbol):
+
+    """
+    Symbol representing the stride of a Function dimension.
+
+    The stride is the the number of elements to skip over in the array's linear
+    memory layout to move one step along that dimension. For example, consider
+    a 2D array with rows and columns. The stride for the row dimension tells
+    you how many elements you need to move forward in memory to get from one
+    row to the next. Similarly, the stride for the column dimension tells you
+    the number of elements you need to skip to move from one column to the next
+    in memory. The stride, therefore, is the product of the size of the
+    dimensions that come after the dimension in question.
+    """
+
+    pass
+
+
+class Dist(Symbol):
+
+    """
+    Symbol representing the distance between a reference point and another point.
+    """
+
+    pass
+
+
+class Tracker(object):
+
+    def __init__(self, mode, dtype, sregistry):
+        self.mode = mode
+        self.dtype = dtype
+        self.sregistry = sregistry
+
+        self.sizes = {}
+        self.strides = {}
+        self.strides_dynamic = {}  # Strides varying regularly across iterations
+        self.dists = {}
+        self.undef = defaultdict(set)
+        self.headers = {}
+
+    def add(self, f):
+        # Update unique sizes table
         for d in f.dimensions[1:]:
             k = key1(f, d)
-            if k and k not in tracker.sizes:
-                name = sregistry.make_name(prefix='%s_fsz' % d.name)
-                fsz = Symbol(name=name, dtype=dtype, is_const=True)
-                tracker.sizes[k] = fsz
-
-    # Update unique strides table
-    # E.g., `{x_stride0 -> (y_fsz0, z_fsz0)}`
-    mapper = defaultdict(dict)
-    for f in needs:
+            if not k or k in self.sizes:
+                continue
+            name = self.sregistry.make_name(prefix='%s_fsz' % d.name)
+            self.sizes[k] = Size(name=name, dtype=self.dtype, is_const=True)
+
+        # Update unique strides table
         for n, d in enumerate(f.dimensions[1:], 1):
             try:
-                k = tuple(tracker.sizes[key1(f, d1)] for d1 in f.dimensions[n:])
+                k = tuple(self.get_size(f, d1) for d1 in f.dimensions[n:])
             except KeyError:
                 continue
-            if k not in tracker.strides:
-                name = sregistry.make_name(prefix='%s_stride' % d.name)
-                stride = Symbol(name=name, dtype=dtype, is_const=True)
-                tracker.strides[k] = stride
-            mapper[f][d] = tracker.strides[k]
+            if k in self.strides:
+                continue
+            name = self.sregistry.make_name(prefix='%s_stride' % d.name)
+            self.strides[k] = Stride(name=name, dtype=self.dtype, is_const=True)
 
-    # Update unique access macros
-    # E.g. `{f(x, y) -> foo}`, `foo(Indexed) -> f[(x)*y_stride0 + (y)]`
-    for f in needs:
-        # All the Indexeds demanding an access macro. For a given `f`, more than
-        # one access macros may be required -- in particular, it will be more
-        # than one if `f` was optimized by the `split_pointers` pass
-        v = [i for i in indexeds if i.function is f]
+    def update(self, functions):
+        for f in functions:
+            self.add(f)
+
+    def add_strides_dynamic(self, f, strides):
+        assert not f.is_regular
+        assert len(strides) == f.ndim - 1
+        self.strides_dynamic[f] = tuple(strides)
+
+    def add_header(self, b, define, expr):
+        # NOTE: the input must be an IndexedBase and not a Function because
+        # we might require either the `.base` or the `.dmap`, or perhaps both
+        v = Bunch(define=define, expr=expr)
+        self.headers[b] = v
+        return v
+
+    def needs_header(self, b):
+        return b.function.ndim > 1 and b not in self.headers
+
+    def get_header(self, b):
+        return self.headers.get(b)
+
+    def get_size(self, f, d):
+        return self.sizes[key1(f, d)]
+
+    def get_sizes(self, f):
+        return tuple(self.get_size(f, d) for d in f.dimensions[1:])
+
+    def map_strides(self, f):
+        dims = list(f.dimensions[1:])
+        if f.is_regular:
+            sizes = self.get_sizes(f)
+            return {d: self.strides[sizes[n:]] for n, d in enumerate(dims)}
+        elif f in self.strides_dynamic:
+            return {d: i for d, i in zip(dims, self.strides_dynamic[f])}
+        else:
+            return {}
 
-        _generate_macro(f, v, tracker, mapper[f], sregistry)
+    def make_dist(self, v):
+        try:
+            dist = self.dists[v]
+        except KeyError:
+            name = self.sregistry.make_name(prefix='dst')
+            dist = self.dists[v] = Dist(name=name, dtype=self.dtype, is_const=True)
+        return dist
+
+
+def linearize_accesses(iet, key0, tracker=None):
+    """
+    Turn Indexeds into FIndexeds and create the necessary access Macros.
+    """
+    # 1) What `iet` *needs*
+    indexeds = FindSymbols('indexeds').visit(iet)
+    needs = filter_ordered(i.function for i in indexeds if key0(i.function))
+    needs = sorted(needs, key=lambda f: len(f.dimensions), reverse=True)
+
+    # Update unique sizes and strides
+    tracker.update(needs)
 
-    # Turn Indexeds into FIndexeds
+    # Pick the chosen linearization mode
+    generate_linearization = linearization_registry[tracker.mode]
+
+    # Generate unique access macros
+    # E.g. `{f(x, y) -> foo}`, `foo(Indexed) -> f[(x)*y_stride0 + (y)]`
+    # And linearize Indexeds
     # E.g. `u[t2, x+8, y+9, z+7] -> uL(t2, x+8, y+9, z+7)`
-    iet = Uxreplace(tracker.subs).visit(iet)
+    subs = {}
+    for i in indexeds:
+        f = i.function
+        if f not in needs:
+            continue
+
+        v = generate_linearization(f, i, tracker)
+        if v is not None:
+            subs[i] = v
+
+    iet = Uxreplace(subs).visit(iet)
 
     # 2) What `iet` *offers*
     # E.g. `{x_fsz0 -> u_vec->size[1]}`
     defines = FindSymbols('defines-aliases').visit(iet)
     offers = filter_ordered(f for f in defines if key0(f))
     instances = {}
     for f in offers:
         for d in f.dimensions[1:]:
-            k = key1(f, d)
             try:
-                fsz = tracker.sizes[k]
+                fsz = tracker.get_size(f, d)
+            except KeyError:
+                continue
+            try:
                 val = _generate_fsz(f, d)
                 if val.free_symbols.issubset(f.bound_symbols):
-                    v = DummyExpr(fsz, val, init=True)
-                else:
-                    v = None
-            except (AttributeError, KeyError):
-                v = None
-            if v is not None:
-                instances[fsz] = v
-
-    # 3) What we need to construct are `iet`'s needs plus the callee delegations
-    candidates = set().union(*[v.values() for v in mapper.values()])
+                    instances[fsz] = DummyExpr(fsz, val, init=True)
+            except AttributeError:
+                pass
+
+    # 3) Which symbols (Strides, Dists) does `iet` need?
+    symbols = flatten(i.free_symbols for i in subs.values())
+    candidates = {i for i in symbols if isinstance(i, (Stride, Dist))}
     for n in FindNodes(Call).visit(iet):
+        # Also consider the strides needed by the callee
         candidates.update(tracker.undef.pop(n.name, []))
 
-    # 4) Construct what needs to *and* can be constructed
-    mapper = dict(zip(tracker.strides.values(), tracker.strides.keys()))
-    stmts0, stmts1 = [], []
+    # 4) What `strides` can indeed be constructed?
+    mapper = {}
+    for sizes, stride in tracker.strides.items():
+        if stride in candidates:
+            if set(sizes).issubset(instances):
+                mapper[stride] = sizes
+            else:
+                tracker.undef[iet.name].add(stride)
+
+    # 5) Construct what needs to *and* can be constructed
+    stmts, stmts1 = [], []
     for stride, sizes in mapper.items():
-        if stride not in candidates:
-            continue
-        try:
-            stmts0.extend([instances[size] for size in sizes])
-        except KeyError:
-            # `stride` would be needed by `iet`, but we don't have the means
-            # to define it, hence we delegate to the caller
-            tracker.undef[iet.name].add(stride)
-            continue
+        stmts.extend([instances[size] for size in sizes])
         stmts1.append(DummyExpr(stride, prod(sizes), init=True))
+    stmts = filter_ordered(stmts)
+
+    stmts2 = []
+    for v, dist in tracker.dists.items():
+        if dist in candidates:
+            stmts2.append(DummyExpr(dist, v, init=True))
+
+    for i in [stmts1, stmts2]:
+        if i and stmts:
+            stmts.append(BlankLine)
+        stmts.extend(i)
 
-    # 5) Attach `stmts0` and `stmts1` to `iet`
-    if stmts0:
-        assert len(stmts1) > 0
-        stmts = filter_ordered(stmts0) + [BlankLine] + stmts1
+    if stmts:
         body = iet.body._rebuild(strides=stmts)
         iet = iet._rebuild(body=body)
-    else:
-        assert len(stmts1) == 0
 
     return iet
 
 
 @singledispatch
 def _generate_fsz(f, d):
     return
@@ -215,58 +314,69 @@
     if f.is_DiscreteFunction:
         return _generate_fsz.registry[DiscreteFunction](f, d)
     else:
         return _generate_fsz.registry[Array](f, d)
 
 
 @singledispatch
-def _generate_macro(f, indexeds, tracker, strides, sregistry):
-    pass
+def _generate_header_basic(f, tracker):
+    return
+
+
+@_generate_header_basic.register(DiscreteFunction)
+@_generate_header_basic.register(Array)
+@_generate_header_basic.register(Bundle)
+def _(f, i, tracker):
+    b = i.base
 
+    if not tracker.needs_header(b):
+        return tracker.get_header(b)
 
-@_generate_macro.register(DiscreteFunction)
-@_generate_macro.register(Array)
-@_generate_macro.register(Bundle)
-def _(f, indexeds, tracker, strides, sregistry):
     # Generate e.g. `usave[(time)*xi_slc0 + (xi)*yi_slc0 + (yi)]`
-    assert len(strides) == len(f.dimensions) - 1
+
+    strides = tracker.map_strides(f)
+
     macroargnames = [d.name for d in f.dimensions]
     macroargs = [MacroArgument(i) for i in macroargnames]
 
     items = [m*strides[d] for m, d in zip(macroargs, f.dimensions[1:])]
     items.append(MacroArgument(f.dimensions[-1].name))
 
-    headers = tracker.headers
-    subs = tracker.subs
-    for i in indexeds:
-        if i in subs:
-            continue
+    pname = tracker.sregistry.make_name(prefix='%sL' % f.name)
+    define = DefFunction(pname, macroargnames)
+    expr = Indexed(b, Add(*items, evaluate=False))
 
-        n = len(i.indices)
-        if n == 1:
-            continue
+    return tracker.add_header(b, define, expr)
 
-        if i.base not in headers:
-            pname = sregistry.make_name(prefix='%sL' % f.name)
 
-            value = Add(*items[-n:], evaluate=False)
-            expr = Indexed(IndexedData(i.base, None, f), value)
-            define = DefFunction(pname, macroargnames[-n:])
+@singledispatch
+def _generate_linearization_basic(f, i, tracker):
+    assert False
 
-            headers[i.base] = (define, expr)
-        else:
-            define, _ = headers[i.base]
-            pname = str(define.name)
 
-        if len(i.indices) == i.function.ndim:
-            v = tuple(strides.values())[-n:]
-            subs[i] = FIndexed.from_indexed(i, pname, strides=v)
-        else:
-            # Honour custom indexing
-            subs[i] = i.base[sum(i.indices)]
+@_generate_linearization_basic.register(DiscreteFunction)
+@_generate_linearization_basic.register(Array)
+@_generate_linearization_basic.register(Bundle)
+def _(f, i, tracker):
+    header = _generate_header_basic(f, i, tracker)
+
+    n = len(i.indices)
+
+    if header and n == i.function.ndim:
+        pname = header.define.name.value
+        strides = tuple(tracker.map_strides(f).values())[-n:]
+        return FIndexed.from_indexed(i, pname, strides=strides)
+    else:
+        # Honour custom indexing
+        return i.base[sum(i.indices)]
+
+
+linearization_registry = {
+    'basic': _generate_linearization_basic,
+}
 
 
 def linearize_pointers(iet, key):
     """
     Flatten n-dimensional PointerCasts/Dereferences.
     """
     candidates = {f for f in FindSymbols().visit(iet) if key(f)}
```

### Comparing `devito-4.8.3/devito/passes/iet/misc.py` & `devito-4.8.4/devito/passes/clusters/derivatives.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,200 +1,247 @@
 from functools import singledispatch
 
-import cgen
-import sympy
+from sympy import S
 
-from devito.finite_differences import Max, Min
-from devito.ir import (Any, Forward, Iteration, List, Prodder, FindApplications,
-                       FindNodes, Transformer, Uxreplace, filter_iterations,
-                       retrieve_iteration_tree)
-from devito.passes.iet.engine import iet_pass
-from devito.symbolics import evalrel, has_integer_args
-from devito.tools import as_mapper, split
+from devito.finite_differences import IndexDerivative
+from devito.ir import Backward, Forward, Interval, IterationSpace, Queue
+from devito.passes.clusters.misc import fuse
+from devito.symbolics import BasicWrapperMixin, reuse_if_untouched, uxreplace
+from devito.tools import infer_dtype, timed_pass
+from devito.types import Eq, Inc, Indexed, Symbol
 
-__all__ = ['avoid_denormals', 'hoist_prodders', 'relax_incr_dimensions',
-           'generate_macros', 'minimize_symbols']
+__all__ = ['lower_index_derivatives']
 
 
-@iet_pass
-def avoid_denormals(iet, platform=None):
-    """
-    Introduce nodes in the Iteration/Expression tree that will expand to C
-    macros telling the CPU to flush denormal numbers in hardware. Denormals
-    are normally flushed when using SSE-based instruction sets, except when
-    compiling shared objects.
-    """
-    # There is unfortunately no known portable way of flushing denormal to zero.
-    # See for example: https://stackoverflow.com/questions/59546406/\
-    #                       a-robust-portable-way-to-set-flush-denormals-to-zero
-    try:
-        if 'sse' not in platform.known_isas:
-            return iet, {}
-    except AttributeError:
-        return iet, {}
+@timed_pass()
+def lower_index_derivatives(clusters, mode=None, **kwargs):
+    clusters, weights, mapper = _lower_index_derivatives(clusters, **kwargs)
 
-    if iet.is_ElementalFunction:
-        return iet, {}
+    if not weights:
+        return clusters
 
-    header = (cgen.Comment('Flush denormal numbers to zero in hardware'),
-              cgen.Statement('_MM_SET_DENORMALS_ZERO_MODE(_MM_DENORMALS_ZERO_ON)'),
-              cgen.Statement('_MM_SET_FLUSH_ZERO_MODE(_MM_FLUSH_ZERO_ON)'),
-              cgen.Line())
+    if mode != 'noop':
+        clusters = fuse(clusters, toposort='maximal')
 
-    body = iet.body._rebuild(body=(List(header=header),) + iet.body.body)
-    iet = iet._rebuild(body=body)
+    # At this point we can detect redundancies induced by inner derivatives that
+    # previously were just not detectable via e.g. plain CSE. For example, if
+    # there were two IndexDerivatives such as `(p.dx + m.dx).dx` and `m.dx.dx`
+    # then it's only after `_lower_index_derivatives` that they're detectable!
+    # TODO: see https://github.com/devitocodes/devito/issues/2306
+    clusters = CDE(mapper).process(clusters)
 
-    return iet, {'includes': ('xmmintrin.h', 'pmmintrin.h')}
+    return clusters
 
 
-@iet_pass
-def hoist_prodders(iet):
-    """
-    Move Prodders within the outer levels of an Iteration tree.
-    """
+def _lower_index_derivatives(clusters, **kwargs):
+    weights = {}
+    processed = []
     mapper = {}
-    for tree in retrieve_iteration_tree(iet):
-        for prodder in FindNodes(Prodder).visit(tree.root):
-            if prodder._periodic:
-                try:
-                    key = lambda i: i.dim.is_Block and i.dim.step != 1
-                    candidate = filter_iterations(tree, key)[-1]
-                except IndexError:
-                    # Fallback: use the outermost Iteration
-                    candidate = tree.root
-                mapper[candidate] = candidate._rebuild(nodes=(candidate.nodes +
-                                                              (prodder._rebuild(),)))
-                mapper[prodder] = None
 
-    iet = Transformer(mapper, nested=True).visit(iet)
+    def dump(exprs, c):
+        if exprs:
+            processed.append(c.rebuild(exprs=exprs))
+            exprs[:] = []
+
+    for c in clusters:
+        exprs = []
+        for e in c.exprs:
+            # Optimization 1: if the LHS is already a Symbol, then surely it's
+            # usable as a temporary for one of the IndexDerivatives inside `e`
+            if e.lhs.is_Symbol and e.operation is None:
+                reusable = {e.lhs}
+            else:
+                reusable = set()
+
+            expr, v = _core(e, c, c.ispace, weights, reusable, mapper, **kwargs)
+
+            if v:
+                dump(exprs, c)
+                processed.extend(v)
+
+            if e.lhs is expr.rhs:
+                # Optimization 2: `e` is of the form
+                # `r = IndexDerivative(...)`
+                # Rather than say
+                # `r = foo(IndexDerivative(...))`
+                # Since `r` is reusable (Optimization 1), we now have `r = r`,
+                # which can safely be discarded
+                pass
+            else:
+                exprs.append(expr)
 
-    return iet, {}
+        dump(exprs, c)
 
+    return processed, weights, mapper
 
-@iet_pass
-def relax_incr_dimensions(iet, options=None, **kwargs):
-    """
-    This pass adjusts the bounds of blocked Iterations in order to include the "remainder
-    regions".  Without the relaxation that occurs in this pass, the only way to iterate
-    over the entire iteration space is to have step increments that are perfect divisors
-    of the iteration space (e.g. in case of an iteration space of size 67 and block size
-    8 only 64 iterations would be computed, as `67 - 67mod8 = 64`.
 
-    A simple 1D example: nested Iterations are transformed from:
+@singledispatch
+def _core(expr, c, ispace, weights, reusables, mapper, **kwargs):
+    """
+    Recursively carry out the core of `lower_index_derivatives` based
+    on single-dispatch.
+    """
+    args = []
+    processed = []
+    for a in expr.args:
+        e, clusters = _core(a, c, ispace, weights, reusables, mapper, **kwargs)
+        args.append(e)
+        processed.extend(clusters)
 
-    <Iteration x0_blk0; (x_m, x_M, x0_blk0_size)>
-        <Iteration x; (x0_blk0, x0_blk0 + x0_blk0_size - 1, 1)>
+    expr = reuse_if_untouched(expr, args)
 
-    to:
+    return expr, processed
 
-    <Iteration x0_blk0; (x_m, x_M, x0_blk0_size)>
-        <Iteration x; (x0_blk0, Min(x_M, x0_blk0 + x0_blk0_size - 1)), 1)>
 
-    """
-    mapper = {}
-    for tree in retrieve_iteration_tree(iet):
-        iterations = [i for i in tree if i.dim.is_Block]
-        if not iterations:
-            continue
-
-        root = iterations[0]
-        if root in mapper:
-            continue
-
-        assert all(i.direction in (Forward, Any) for i in iterations)
-        outer, inner = split(iterations, lambda i: not i.dim.parent.is_Block)
-
-        # Get root's `symbolic_max` out of each outer Dimension
-        roots_max = {i.dim.root: i.symbolic_max for i in outer}
-
-        # Process inner iterations and adjust their bounds
-        for n, i in enumerate(inner):
-            # If definitely in-bounds, as ensured by a prior compiler pass, then
-            # we can skip this step
-            if i.is_Inbound:
-                continue
+@_core.register(Symbol)
+@_core.register(Indexed)
+@_core.register(BasicWrapperMixin)
+def _(expr, c, ispace, weights, reusables, mapper, **kwargs):
+    return expr, []
 
-            # The Iteration's maximum is the Min of (a) the `symbolic_max` of current
-            # Iteration e.g. `x0_blk0 + x0_blk0_size - 1` and (b) the `symbolic_max`
-            # of the current Iteration's root Dimension e.g. `x_M`. The generated
-            # maximum will be `Min(x0_blk0 + x0_blk0_size - 1, x_M)
 
-            # In some corner cases an offset may be added (e.g. after CIRE passes)
-            # E.g. assume `i.symbolic_max = x0_blk0 + x0_blk0_size + 1` and
-            # `i.dim.symbolic_max = x0_blk0 + x0_blk0_size - 1` then the generated
-            # maximum will be `Min(x0_blk0 + x0_blk0_size + 1, x_M + 2)`
+@_core.register(IndexDerivative)
+def _(expr, c, ispace, weights, reusables, mapper, **kwargs):
+    sregistry = kwargs['sregistry']
+    options = kwargs['options']
+    subs_user = kwargs['subs']
 
-            root_max = roots_max[i.dim.root] + i.symbolic_max - i.dim.symbolic_max
-            iter_max = evalrel(min, [i.symbolic_max, root_max])
-            mapper[i] = i._rebuild(limits=(i.symbolic_min, iter_max, i.step))
+    try:
+        cbk0 = deriv_schedule_registry[options['deriv-schedule']]
+        cbk1 = deriv_unroll_registry[options['deriv-unroll']]
+    except KeyError:
+        raise ValueError("Unknown derivative lowering mode")
+
+    # Lower the IndexDerivative
+    init, ideriv = cbk0(expr)
+
+    # Create the concrete Weights array, or reuse an already existing one
+    # if possible
+    name = sregistry.make_name(prefix='w')
+    w0 = ideriv.weights.function
+    dtype = infer_dtype([w0.dtype, c.dtype])  # At least np.float32
+    k = tuple(w0.weights)
+    try:
+        w = weights[k]
+    except KeyError:
+        initvalue = tuple(i.subs(subs_user) for i in k)
+        w = weights[k] = w0._rebuild(name=name, dtype=dtype, initvalue=initvalue)
+
+    # Replace the abstract Weights array with the concrete one
+    subs = {w0.indexed: w.indexed}
+    init = uxreplace(init, subs)
+    ideriv = uxreplace(ideriv, subs)
+
+    # The IterationSpace in which the IndexDerivative will be computed
+    dims = ideriv.dimensions
+
+    intervals = [Interval(d) for d in dims]
+    directions = {d: Backward if d.backward else Forward for d in dims}
+    ispace0 = IterationSpace(intervals, directions=directions)
+
+    # Minimize the amount of integer arithmetic to calculate the various index
+    # access functions by enforcing start at 0, e.g. `r0[x + i0 + 2] -> r0[x + i0]`
+    base = ideriv.base
+    for d in dims:
+        ispace0 = ispace0.translate(d, -d._min)
+        base = base.subs(d, d + d._min)
+    ideriv = ideriv._subs(ideriv.base, base)
+
+    # Should the IndexDerivative be unrolled?
+    init, expr, ispace0 = cbk1(init, ideriv, ispace0)
+
+    # The full IterationSpace
+    extra = (ispace.itdims + ispace0.itdims,)
+    ispace1 = IterationSpace.union(ispace, ispace0, relations=extra)
 
-    if mapper:
-        iet = Transformer(mapper, nested=True).visit(iet)
+    # The Symbol that will hold the result of the IndexDerivative computation
+    # NOTE: created before recurring so that we ultimately get a sound ordering
+    try:
+        s = reusables.pop()
+        assert s.dtype is dtype
+    except KeyError:
+        name = sregistry.make_name(prefix='r')
+        s = Symbol(name=name, dtype=dtype)
+
+    # Go inside `expr` and recursively lower any nested IndexDerivatives
+    expr, processed = _core(expr, c, ispace1, weights, reusables, mapper, **kwargs)
+
+    # Finally inject the lowered IndexDerivative
+    if init is not None:
+        expr0 = Eq(s, init)
+        processed.insert(0, c.rebuild(exprs=expr0, ispace=ispace))
 
-    return iet, {}
+        expr1 = Inc(s, expr)
+        processed.append(c.rebuild(exprs=expr1, ispace=ispace1))
+    else:
+        expr1 = Eq(s, expr)
+        processed.append(c.rebuild(exprs=expr1, ispace=ispace1))
 
+    # Track the lowered IndexDerivative for subsequent optimization by the caller
+    mapper.setdefault(expr, []).append(s)
 
-@iet_pass
-def generate_macros(iet):
-    applications = FindApplications().visit(iet)
-    headers = set().union(*[_generate_macros(i) for i in applications])
+    return s, processed
 
-    return iet, {'headers': headers}
 
+def _lower_index_derivative_base(ideriv):
+    return S.Zero, ideriv
 
-@singledispatch
-def _generate_macros(expr):
-    return set()
 
+deriv_schedule_registry = {
+    'basic': _lower_index_derivative_base,
+}
 
-@_generate_macros.register(Min)
-@_generate_macros.register(sympy.Min)
-def _(expr):
-    if has_integer_args(*expr.args) and len(expr.args) == 2:
-        return {('MIN(a,b)', ('(((a) < (b)) ? (a) : (b))'))}
-    else:
-        return set()
 
+deriv_unroll_registry = {
+    False: lambda init, ideriv, ispace: (init, ideriv.expr, ispace)
+}
 
-@_generate_macros.register(Max)
-@_generate_macros.register(sympy.Max)
-def _(expr):
-    if has_integer_args(*expr.args) and len(expr.args) == 2:
-        return {('MAX(a,b)', ('(((a) > (b)) ? (a) : (b))'))}
-    else:
-        return set()
 
+class CDE(Queue):
 
-@iet_pass
-def minimize_symbols(iet):
     """
-    Remove unneccesary symbols. Currently applied sub-passes:
-
-        * Remove redundant ModuloDimensions (e.g., due to using the
-          `save=Buffer(2)` API)
+    Common derivative elimination.
     """
-    iet = remove_redundant_moddims(iet)
 
-    return iet, {}
+    _q_guards_in_key = True
+    _q_syncs_in_key = True
 
+    def __init__(self, mapper):
+        super().__init__()
 
-def remove_redundant_moddims(iet):
-    subs0 = {}
-    subs1 = {}
-    for n in FindNodes(Iteration).visit(iet):
-        mds = [d for d in n.uindices
-               if d.is_Modulo and d.origin is not None]
-        if not mds:
-            continue
+        self.mapper = {k: v for k, v in mapper.items() if len(v) > 1}
 
-        mapper = as_mapper(mds, key=lambda md: md.origin % md.modulo)
-        for k, v in mapper.items():
-            chosen = v.pop(0)
-            subs0.update({d: chosen for d in v})
+    def process(self, clusters):
+        return self._process_fdta(clusters, 1, subs0={}, seen=set())
+
+    def callback(self, clusters, prefix, subs0=None, seen=None):
+        subs = {}
+        processed = []
+        for c in clusters:
+            if c in seen:
+                processed.append(c)
+                continue
+
+            exprs = []
+            for e in c.exprs:
+                k, v = e.args
+
+                if k in subs0:
+                    continue
+
+                try:
+                    subs0[k] = subs[v]
+                    continue
+                except KeyError:
+                    pass
+
+                if v in self.mapper:
+                    subs[v] = k
+                    exprs.append(e)
+                else:
+                    exprs.append(uxreplace(e, {**subs0, **subs}))
 
-        uindices = [d for d in n.uindices if d not in subs0]
-        subs1[n] = n._rebuild(uindices=uindices)
+            processed.append(c.rebuild(exprs=exprs))
 
-    iet = Transformer(subs1, nested=True).visit(iet)
-    iet = Uxreplace(subs0).visit(iet)
+        seen.update(processed)
 
-    return iet
+        return processed
```

### Comparing `devito-4.8.3/devito/passes/iet/mpi.py` & `devito-4.8.4/devito/passes/iet/mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,17 @@
             hsmapper[hs] = hs.halo_scheme
 
             for f, v in hs.fmapper.items():
                 loc_dims = frozenset().union([q for d in v.loc_indices
                                               for q in d._defines])
 
                 for n, i in enumerate(iters):
+                    if i not in scopes:
+                        continue
+
                     candidates = [i.dim._defines for i in iters[n:]]
 
                     all_candidates = set().union(*candidates)
                     reads = scopes[i].getreads(f)
                     if any(set(a.ispace.dimensions) & all_candidates
                            for a in reads):
                         continue
@@ -247,17 +250,18 @@
     Detect the HaloSpots allowing computation/communication overlap and turn
     them into OverlappableHaloSpots.
     """
     # Analysis
     found = []
     for hs in FindNodes(HaloSpot).visit(iet):
         expressions = FindNodes(Expression).visit(hs)
-        scope = Scope([i.expr for i in expressions])
+        if not expressions:
+            continue
 
-        test = True
+        scope = Scope([i.expr for i in expressions])
 
         # Comp/comm overlaps is legal only if the OWNED regions can grow
         # arbitrarly, which means all of the dependences must be carried
         # along a non-halo Dimension
         for dep in scope.d_all_gen():
             if dep.function in hs.functions:
                 cause = dep.cause & hs.dimensions
@@ -266,14 +270,16 @@
                     # for x
                     #   for y
                     #     ... = ... f[x, y-1] ...
                     #   for y
                     #     f[x, y] = ...
                     test = False
                     break
+        else:
+            test = True
 
         # Heuristic: avoid comp/comm overlap for sparse Iteration nests
         if test:
             for i in FindNodes(Iteration).visit(hs):
                 if i.dim._defines & set(hs.halo_scheme.distributed_aindices) and \
                    not i.is_Affine:
                     test = False
@@ -335,13 +341,13 @@
     The former is implemented by manipulating HaloSpots.
 
     The latter resorts to creating MPI Callables and replacing HaloSpots with Calls
     to MPI Callables.
     """
     options = kwargs['options']
 
-    if options['optcomms']:
+    if options['opt-comms']:
         optimize_halospots(graph, **kwargs)
 
     mpimode = options['mpi']
     if mpimode:
         make_mpi(graph, mpimode=mpimode, **kwargs)
```

### Comparing `devito-4.8.3/devito/passes/iet/orchestration.py` & `devito-4.8.4/devito/passes/iet/orchestration.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,58 +31,58 @@
     """
 
     def __init__(self, sregistry):
         self.sregistry = sregistry
 
     def _make_waitlock(self, iet, sync_ops, *args):
         waitloop = List(
-            header=c.Comment("Wait for `%s` to be copied to the host" %
+            header=c.Comment("Wait for `%s` to be transferred" %
                              ",".join(s.target.name for s in sync_ops)),
             body=BusyWait(Or(*[CondEq(s.handle, 0) for s in sync_ops])),
-            footer=c.Line()
         )
 
         iet = List(body=(waitloop,) + iet.body)
 
         return iet, []
 
     def _make_releaselock(self, iet, sync_ops, *args):
         pre = []
         pre.append(BusyWait(Or(*[CondNe(s.handle, 2) for s in sync_ops])))
         pre.extend(DummyExpr(s.handle, 0) for s in sync_ops)
 
-        iet = List(
-            header=c.Comment("Release lock(s) as soon as possible"),
-            body=pre + [iet]
-        )
+        name = self.sregistry.make_name(prefix="release_lock")
+        parameters = derive_parameters(pre, ordering='canonical')
+        efunc = Callable(name, pre, 'void', parameters, 'static')
 
-        return iet, []
+        iet = List(body=[Call(name, efunc.parameters)] + [iet])
+
+        return iet, [efunc]
 
     def _make_withlock(self, iet, sync_ops, layer):
         body, prefix = withlock(layer, iet, sync_ops, self.lang, self.sregistry)
 
         # Turn `iet` into an AsyncCallable so that subsequent passes know
         # that we're happy for this Callable to be executed asynchronously
         name = self.sregistry.make_name(prefix=prefix)
         body = List(body=body)
-        parameters = derive_parameters(body)
+        parameters = derive_parameters(body, ordering='canonical')
         efunc = AsyncCallable(name, body, parameters=parameters)
 
         # The corresponding AsyncCall
         iet = AsyncCall(name, efunc.parameters)
 
         return iet, [efunc]
 
     def _make_fetchupdate(self, iet, sync_ops, layer):
         body, prefix = fetchupdate(layer, iet, sync_ops, self.lang, self.sregistry)
 
         # Turn init IET into a Callable
         name = self.sregistry.make_name(prefix=prefix)
         body = List(body=body)
-        parameters = derive_parameters(body)
+        parameters = derive_parameters(body, ordering='canonical')
         efunc = Callable(name, body, 'void', parameters, 'static')
 
         # Perform initial fetch by the main thread
         iet = List(
             header=c.Comment("Initialize data stream"),
             body=Call(name, parameters)
         )
@@ -92,15 +92,15 @@
     def _make_prefetchupdate(self, iet, sync_ops, layer):
         body, prefix = prefetchupdate(layer, iet, sync_ops, self.lang, self.sregistry)
 
         # Turn `iet` into an AsyncCallable so that subsequent passes know
         # that we're happy for this Callable to be executed asynchronously
         name = self.sregistry.make_name(prefix=prefix)
         body = List(body=body)
-        parameters = derive_parameters(body)
+        parameters = derive_parameters(body, ordering='canonical')
         efunc = AsyncCallable(name, body, parameters=parameters)
 
         # The corresponding AsyncCall
         iet = AsyncCall(name, efunc.parameters)
 
         return iet, [efunc]
 
@@ -191,17 +191,23 @@
 @singledispatch
 def fetchupdate(layer, iet, sync_ops, lang, sregistry):
     raise NotImplementedError
 
 
 @fetchupdate.register(HostLayer)
 def _(layer, iet, sync_ops, lang, sregistry):
+    try:
+        qid = sregistry.queue0
+    except AttributeError:
+        qid = None
+
     body = list(iet.body)
     try:
-        body.extend([lang._map_update_device(s.target, s.imask) for s in sync_ops])
+        body.extend([lang._map_update_device(s.target, s.imask, qid=qid)
+                     for s in sync_ops])
         name = 'init_from_%s' % layer.suffix
     except NotImplementedError:
         name = 'init_to_%s' % layer.suffix
 
     return body, name
```

### Comparing `devito-4.8.3/devito/passes/iet/parpragma.py` & `devito-4.8.4/devito/passes/iet/parpragma.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from itertools import takewhile
+from collections import defaultdict
 
 import numpy as np
 import cgen as c
 from cached_property import cached_property
 from sympy import And, Max, true
 
 from devito.data import FULL
 from devito.ir import (Conditional, DummyEq, Dereference, Expression,
                        ExpressionBundle, FindSymbols, FindNodes, ParallelIteration,
                        ParallelTree, Pragma, Prodder, Transfer, List, Transformer,
                        IsPerfectIteration, OpInc, filter_iterations,
                        retrieve_iteration_tree, IMask, VECTORIZED)
 from devito.passes.iet.engine import iet_pass
 from devito.passes.iet.langbase import (LangBB, LangTransformer, DeviceAwareMixin,
-                                        make_sections_from_imask)
+                                        ShmTransformer, make_sections_from_imask)
 from devito.symbolics import INT, ccode
 from devito.tools import as_tuple, flatten, is_integer, prod
-from devito.tools.data_structures import UnboundTuple
 from devito.types import Symbol
 
 __all__ = ['PragmaSimdTransformer', 'PragmaShmTransformer',
            'PragmaDeviceAwareTransformer', 'PragmaLangBB', 'PragmaTransfer']
 
 
 class PragmaTransformer(LangTransformer):
@@ -40,19 +39,32 @@
     """
 
     @classmethod
     def _support_array_reduction(cls, compiler):
         return True
 
     @property
-    def simd_reg_size(self):
-        return self.platform.simd_reg_size
+    def simd_reg_nbytes(self):
+        return self.platform.simd_reg_nbytes
 
-    @iet_pass
-    def make_simd(self, iet):
+    def _make_simd_pragma(self, iet):
+        indexeds = FindSymbols('indexeds').visit(iet)
+        aligned = {i.name for i in indexeds if i.function.is_DiscreteFunction}
+        if aligned:
+            simd = self.lang['simd-for-aligned']
+            simd = as_tuple(simd(','.join(sorted(aligned)), self.simd_reg_nbytes))
+        else:
+            simd = as_tuple(self.lang['simd-for'])
+
+        return simd
+
+    def _make_simd(self, iet):
+        """
+        Carry out the bulk of `make_simd`.
+        """
         mapper = {}
         for tree in retrieve_iteration_tree(iet):
             candidates = [i for i in tree if i.is_ParallelRelaxed]
 
             # As long as there's an outer level of parallelism, the innermost
             # PARALLEL Iteration gets vectorized
             if len(candidates) < 2:
@@ -99,40 +111,40 @@
                not self._support_array_reduction(self.compiler):
                 exprs = FindNodes(Expression).visit(candidate)
                 reductions = [i.output for i in exprs if i.is_reduction]
                 if any(i.is_Indexed for i in reductions):
                     continue
 
             # Add SIMD pragma
-            indexeds = FindSymbols('indexeds').visit(candidate)
-            aligned = {i.name for i in indexeds if i.function.is_DiscreteFunction}
-            if aligned:
-                simd = self.lang['simd-for-aligned']
-                simd = as_tuple(simd(','.join(sorted(aligned)), self.simd_reg_size))
-            else:
-                simd = as_tuple(self.lang['simd-for'])
+            simd = self._make_simd_pragma(candidate)
             pragmas = candidate.pragmas + simd
 
             # Add VECTORIZED property
             properties = list(candidate.properties) + [VECTORIZED]
 
             mapper[candidate] = candidate._rebuild(pragmas=pragmas, properties=properties)
 
         iet = Transformer(mapper).visit(iet)
 
         return iet, {}
 
+    @iet_pass
+    def make_simd(self, iet):
+        return self._make_simd(iet)
+
 
 class PragmaIteration(ParallelIteration):
 
     def __init__(self, *args, parallel=None, schedule=None, chunk_size=None,
                  nthreads=None, ncollapsed=None, reduction=None, tile=None,
                  gpu_fit=None, **kwargs):
 
-        construct = self._make_construct(parallel=parallel)
+        construct = self._make_construct(
+            parallel=parallel, ncollapsed=ncollapsed, tile=tile
+        )
         clauses = self._make_clauses(
             ncollapsed=ncollapsed, chunk_size=chunk_size, nthreads=nthreads,
             reduction=reduction, schedule=schedule, tile=tile, gpu_fit=gpu_fit,
             **kwargs
         )
         pragma = c.Pragma(' '.join([construct] + clauses))
         kwargs['pragmas'] = pragma
@@ -159,201 +171,56 @@
 
     @classmethod
     def _make_clause_reduction_from_imask(cls, reductions):
         """
         Build a string representing of a reduction clause given a list of
         2-tuples `(symbol, ir.Operation)`.
         """
-        args = []
+        mapper = defaultdict(list)
         for i, imask, r in reductions:
             if i.is_Indexed:
                 f = i.function
                 bounds = []
                 for k, d in zip(imask, f.dimensions):
                     if is_integer(k):
                         bounds.append('[%s]' % k)
                     elif k is FULL:
                         # Lower FULL Dimensions into a range spanning the entire
                         # Dimension space, e.g. `reduction(+:f[0:f_vec->size[1]])`
                         bounds.append('[0:%s]' % f._C_get_field(FULL, d).size)
                     else:
                         assert isinstance(k, tuple) and len(k) == 2
                         bounds.append('[%s:%s]' % k)
-                args.append('%s%s' % (i.name, ''.join(bounds)))
+                mapper[r.name].append('%s%s' % (i.name, ''.join(bounds)))
             else:
-                args.append(str(i))
-        return 'reduction(%s:%s)' % (r.name, ','.join(args))
+                mapper[r.name].append(str(i))
+
+        args = ['reduction(%s:%s)' % (k, ','.join(v)) for k, v in mapper.items()]
+
+        return ' '.join(args)
 
     @cached_property
     def collapsed(self):
         ret = [self]
         for i in range(self.ncollapsed - 1):
             ret.append(ret[i].nodes[0])
         assert all(i.is_Iteration for i in ret)
         return tuple(ret)
 
 
-class PragmaShmTransformer(PragmaSimdTransformer):
+class PragmaShmTransformer(ShmTransformer, PragmaSimdTransformer):
 
     """
-    Abstract base class for PragmaTransformers capable of emitting SIMD-parallel
-    and shared-memory-parallel IETs.
+    PragmaTransformer capable of emitting SIMD-parallel and shared-memory-parallel
+    IETs for CPUs.
     """
 
     def __init__(self, sregistry, options, platform, compiler):
-        """
-        Parameters
-        ----------
-        sregistry : SymbolRegistry
-            The symbol registry, to access the symbols appearing in an IET.
-        options : dict
-             The optimization options. Accepted: ['par-collapse-ncores',
-             'par-collapse-work', 'par-chunk-nonaffine', 'par-dynamic-work', 'par-nested']
-             * 'par-collapse-ncores': use a collapse clause if the number of
-               available physical cores is greater than this threshold.
-             * 'par-collapse-work': use a collapse clause if the trip count of the
-               collapsable Iterations is statically known to exceed this threshold.
-             * 'par-chunk-nonaffine': coefficient to adjust the chunk size in
-               non-affine parallel Iterations.
-             * 'par-dynamic-work': use dynamic scheduling if the operation count per
-               iteration exceeds this threshold. Otherwise, use static scheduling.
-             * 'par-nested': nested parallelism if the number of hyperthreads per core
-               is greater than this threshold.
-        platform : Platform
-            The underlying platform.
-        compiler : Compiler
-            The underlying JIT compiler.
-        """
         key = lambda i: i.is_ParallelRelaxed and not i.is_Vectorized
-        super().__init__(key, sregistry, platform, compiler)
-
-        self.collapse_ncores = options['par-collapse-ncores']
-        self.collapse_work = options['par-collapse-work']
-        self.chunk_nonaffine = options['par-chunk-nonaffine']
-        self.dynamic_work = options['par-dynamic-work']
-        self.nested = options['par-nested']
-
-    @property
-    def ncores(self):
-        return self.platform.cores_physical
-
-    @property
-    def nhyperthreads(self):
-        return self.platform.threads_per_core
-
-    @property
-    def nthreads(self):
-        return self.sregistry.nthreads
-
-    @property
-    def nthreads_nested(self):
-        return self.sregistry.nthreads_nested
-
-    @property
-    def nthreads_nonaffine(self):
-        return self.sregistry.nthreads_nonaffine
-
-    @property
-    def threadid(self):
-        return self.sregistry.threadid
-
-    def _score_candidate(self, n0, root, collapsable=()):
-        """
-        The score of a collapsable nest depends on the number of fully-parallel
-        Iterations and their position in the nest (the outer, the better).
-        """
-        nest = [root] + list(collapsable)
-        n = len(nest)
-
-        # Number of fully-parallel collapsable Iterations
-        key = lambda i: i.is_ParallelNoAtomic
-        fp_iters = list(takewhile(key, nest))
-        n_fp_iters = len(fp_iters)
-
-        # Number of parallel-if-atomic collapsable Iterations
-        key = lambda i: i.is_ParallelAtomic
-        pia_iters = list(takewhile(key, nest))
-        n_pia_iters = len(pia_iters)
-
-        # Prioritize the Dimensions that are more likely to define larger
-        # iteration spaces
-        key = lambda d: (not d.is_Derived or
-                         (d.is_Custom and not is_integer(d.symbolic_size)) or
-                         (d.is_Block and d._depth == 1))
-
-        fpdims = [i.dim for i in fp_iters]
-        n_fp_iters_large = len([d for d in fpdims if key(d)])
-
-        piadims = [i.dim for i in pia_iters]
-        n_pia_iters_large = len([d for d in piadims if key(d)])
-
-        return (
-            int(n_fp_iters == n),  # Fully-parallel nest
-            n_fp_iters_large,
-            n_fp_iters,
-            n_pia_iters_large,
-            n_pia_iters,
-            -(n0 + 1),  # The outer, the better
-            n,
-        )
-
-    def _select_candidates(self, candidates):
-        assert candidates
-
-        if self.ncores < self.collapse_ncores:
-            return candidates[0], []
-
-        mapper = {}
-        for n0, root in enumerate(candidates):
-
-            # Score `root` in isolation
-            mapper[(root, ())] = self._score_candidate(n0, root)
-
-            collapsable = []
-            for n, i in enumerate(candidates[n0+1:], n0+1):
-                # The Iteration nest [root, ..., i] must be perfect
-                if not IsPerfectIteration(depth=i).visit(root):
-                    break
-
-                # Loops are collapsable only if none of the iteration variables
-                # appear in initializer expressions. For example, the following
-                # two loops cannot be collapsed
-                #
-                # for (i = ... )
-                #   for (j = i ...)
-                #     ...
-                #
-                # Here, we make sure this won't happen
-                if any(j.dim in i.symbolic_min.free_symbols for j in candidates[n0:n]):
-                    break
-
-                # Can't collapse SIMD-vectorized Iterations
-                if i.is_Vectorized:
-                    break
-
-                # Would there be enough work per parallel iteration?
-                nested = candidates[n+1:]
-                if nested:
-                    try:
-                        work = prod([int(j.dim.symbolic_size) for j in nested])
-                        if work < self.collapse_work:
-                            break
-                    except TypeError:
-                        pass
-
-                collapsable.append(i)
-
-                # Score `root + collapsable`
-                v = tuple(collapsable)
-                mapper[(root, v)] = self._score_candidate(n0, root, v)
-
-        # Retrieve the candidates with highest score
-        root, collapsable = max(mapper, key=mapper.get)
-
-        return root, list(collapsable)
+        super().__init__(key, sregistry, options, platform, compiler)
 
     def _make_reductions(self, partree):
         if not any(i.is_ParallelAtomic for i in partree.collapsed):
             return partree
 
         exprs = [i for i in FindNodes(Expression).visit(partree) if i.is_reduction]
 
@@ -606,15 +473,16 @@
     shared-memory-parallel, and device-parallel IETs.
     """
 
     def __init__(self, sregistry, options, platform, compiler):
         super().__init__(sregistry, options, platform, compiler)
 
         self.gpu_fit = options['gpu-fit']
-        self.par_tile = UnboundTuple(options['par-tile'])
+        # Need to reset the tile in case was already used and iter over by blocking
+        self.par_tile = options['par-tile'].reset()
         self.par_disabled = options['par-disabled']
 
     def _score_candidate(self, n0, root, collapsable=()):
         # `ndptrs`, the number of device pointers, part of the score too to
         # ensure the outermost loop is offloaded
         ndptrs = len(self._device_pointers(root))
 
@@ -641,15 +509,16 @@
         """
         assert candidates
 
         root, collapsable = self._select_candidates(candidates)
 
         if self._is_offloadable(root):
             body = self.DeviceIteration(gpu_fit=self.gpu_fit,
-                                        ncollapsed=len(collapsable) + 1,
+                                        ncollapsed=len(collapsable)+1,
+                                        tile=self.par_tile.nextitem(),
                                         **root.args)
             partree = ParallelTree([], body, nthreads=nthreads)
 
             return root, partree
         elif not self.par_disabled:
             # Resort to host parallelism
             return super()._make_partree(candidates, nthreads)
```

### Comparing `devito-4.8.3/devito/symbolics/extended_sympy.py` & `devito-4.8.4/devito/symbolics/extended_sympy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Extended SymPy hierarchy.
 """
 
 import numpy as np
 import sympy
-from sympy import Expr, Integer, Function, Number, Tuple, sympify
+from sympy import Expr, Function, Number, Tuple, sympify
 from sympy.core.decorators import call_highest_priority
 
-from devito.tools import (Pickable, as_tuple, is_integer, float2, float3, float4,  # noqa
-                          double2, double3, double4, int2, int3, int4)
 from devito.finite_differences.elementary import Min, Max
+from devito.tools import (Pickable, Bunch, as_tuple, is_integer, float2,  # noqa
+                          float3, float4, double2, double3, double4, int2, int3,
+                          int4)
 from devito.types import Symbol
+from devito.types.basic import Basic
 
-__all__ = ['CondEq', 'CondNe', 'IntDiv', 'CallFromPointer', 'FieldFromPointer',  # noqa
-           'FieldFromComposite', 'ListInitializer', 'Byref', 'IndexedPointer', 'Cast',
-           'DefFunction', 'InlineIf', 'Keyword', 'String', 'Macro', 'MacroArgument',
-           'CustomType', 'Deref', 'INT', 'FLOAT', 'DOUBLE', 'VOID',
-           'Null', 'SizeOf', 'rfunc', 'cast_mapper', 'BasicWrapperMixin']
+__all__ = ['CondEq', 'CondNe', 'IntDiv', 'CallFromPointer',  # noqa
+           'CallFromComposite', 'FieldFromPointer', 'FieldFromComposite',
+           'ListInitializer', 'Byref', 'IndexedPointer', 'Cast', 'DefFunction',
+           'MathFunction', 'InlineIf', 'ReservedWord', 'Keyword', 'String',
+           'Macro', 'Class', 'MacroArgument', 'CustomType', 'Deref', 'Namespace',
+           'Rvalue', 'INT', 'FLOAT', 'DOUBLE', 'VOID', 'Null', 'SizeOf', 'rfunc',
+           'cast_mapper', 'BasicWrapperMixin', 'ValueLimit', 'limits_mapper']
 
 
 class CondEq(sympy.Eq):
 
     """
     A customized version of sympy.Eq representing a conditional equality.
     It suppresses evaluation.
@@ -159,19 +163,17 @@
     __rkwargs__ = ('params',)
 
     def __new__(cls, call, pointer, params=None, **kwargs):
         if isinstance(pointer, str):
             pointer = Symbol(pointer)
         if isinstance(call, str):
             call = Symbol(call)
-        elif not isinstance(call, (CallFromPointer, DefFunction, sympy.Symbol)):
-            # NOTE: we need `sympy.Symbol`, rather than just (devito) `Symbol`
-            # because otherwise it breaks upon certain reconstructions on SymPy-1.8,
-            # due to the way `bound_symbols` and `canonical_variables` interact
-            raise ValueError("`call` must be CallFromPointer, DefFunction, or Symbol")
+        elif not isinstance(call, Basic):
+            raise ValueError("`call` must be a `devito.Basic` or a type "
+                             "with compatible interface")
         _params = []
         for p in as_tuple(params):
             if isinstance(p, str):
                 _params.append(Symbol(p))
             elif isinstance(p, Expr):
                 _params.append(p)
             else:
@@ -191,16 +193,15 @@
     def __str__(self):
         return '%s->%s(%s)' % (self.pointer, self.call,
                                ", ".join(str(i) for i in as_tuple(self.params)))
 
     __repr__ = __str__
 
     def _hashable_content(self):
-        return super(CallFromPointer, self)._hashable_content() +\
-            (self.call, self.pointer) + self.params
+        return super()._hashable_content() + (self.call, self.pointer) + self.params
 
     @property
     def base(self):
         if isinstance(self.pointer, CallFromPointer):
             # CallFromPointer may be nested
             return self.pointer.base
         else:
@@ -216,14 +217,27 @@
 
     is_commutative = BasicWrapperMixin.is_commutative
 
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
+class CallFromComposite(CallFromPointer, Pickable):
+
+    """
+    Symbolic representation of the C notation ``composite.call(params)``.
+    """
+
+    def __str__(self):
+        return '%s.%s(%s)' % (self.pointer, self.call,
+                              ", ".join(str(i) for i in as_tuple(self.params)))
+
+    __repr__ = __str__
+
+
 class FieldFromPointer(CallFromPointer, Pickable):
 
     """
     Symbolic representation of the C notation ``pointer->field``.
     """
 
     __rkwargs__ = ()
@@ -274,22 +288,18 @@
     """
 
     __rargs__ = ('params',)
 
     def __new__(cls, params):
         args = []
         for p in as_tuple(params):
-            if isinstance(p, str):
-                args.append(Symbol(p))
-            elif is_integer(p):
-                args.append(Integer(p))
-            elif not isinstance(p, Expr):
-                raise ValueError("`params` must be an iterable of Expr or str")
-            else:
-                args.append(p)
+            try:
+                args.append(sympify(p))
+            except sympy.SympifyError:
+                raise ValueError("Illegal param `%s`" % p)
         obj = sympy.Expr.__new__(cls, *args)
         obj.params = tuple(args)
         return obj
 
     def __str__(self):
         return "{%s}" % ", ".join(str(i) for i in self.params)
 
@@ -374,14 +384,25 @@
     """
 
     _base_typ = ''
 
     __rkwargs__ = ('stars',)
 
     def __new__(cls, base, stars=None, **kwargs):
+        # Attempt simplifcation
+        # E.g., `FLOAT(32) -> 32.0` of type `sympy.Float`
+        try:
+            return sympify(eval(cls._base_typ)(base))
+        except (NameError, SyntaxError):
+            # E.g., `_base_typ` is "char" or "unsigned long"
+            pass
+        except TypeError:
+            # `base` ain't a number
+            pass
+
         obj = super().__new__(cls, base)
         obj._stars = stars
         return obj
 
     def _hashable_content(self):
         return super()._hashable_content() + (self._stars,)
 
@@ -473,14 +494,17 @@
         return self.value
 
     __repr__ = __str__
 
     def _hashable_content(self):
         return (self.value,)
 
+    def _sympystr(self, printer):
+        return str(self)
+
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
 class Keyword(ReservedWord):
     pass
 
@@ -493,72 +517,129 @@
     pass
 
 
 class Macro(ReservedWord):
     pass
 
 
+class Class(ReservedWord):
+
+    def __str__(self):
+        return "class %s" % self.value
+
+    __repr__ = __str__
+
+
 class MacroArgument(sympy.Symbol):
 
     def __str__(self):
         return "(%s)" % self.name
 
     __repr__ = __str__
 
 
+class ValueLimit(ReservedWord, sympy.Expr):
+
+    """
+    Symbolic representation of the so called limits macros, which provide the
+    minimum and maximum limits for various types, such as INT_MIN, INT_MAX etc.
+    """
+
+    pass
+
+
+limits_mapper = {
+    np.int32: Bunch(min=ValueLimit('INT_MIN'), max=ValueLimit('INT_MAX')),
+    np.int64: Bunch(min=ValueLimit('LONG_MIN'), max=ValueLimit('LONG_MAX')),
+    np.float32: Bunch(min=-ValueLimit('FLT_MAX'), max=ValueLimit('FLT_MAX')),
+    np.float64: Bunch(min=-ValueLimit('DBL_MAX'), max=ValueLimit('DBL_MAX')),
+}
+
+
 class DefFunction(Function, Pickable):
 
     """
     A definitely-defined sympy.Function, to work around:
 
         https://github.com/sympy/sympy/issues/4297
     """
 
-    __rargs__ = ('name', 'arguments')
+    __rargs__ = ('name', 'arguments', 'template')
+
+    def __new__(cls, name, arguments=None, template=None, **kwargs):
+        if isinstance(name, str):
+            name = Keyword(name)
 
-    def __new__(cls, name, arguments=None, **kwargs):
         _arguments = []
         for i in as_tuple(arguments):
             if isinstance(i, str):
                 # Make sure there's no cast to sympy.Symbol underneath
                 # We don't know what `i` is exactly, because the caller won't
                 # tell us, but we're just better off with ReservedWord
                 _arguments.append(ReservedWord(i))
             else:
                 _arguments.append(i)
-        arguments = tuple(_arguments)
-        if isinstance(name, str):
-            name = Keyword(name)
-        obj = Function.__new__(cls, name, Tuple(*arguments))
+
+        _template = []
+        for i in as_tuple(template):
+            if isinstance(i, str):
+                # Same story as above
+                _template.append(ReservedWord(i))
+            else:
+                _template.append(i)
+
+        args = [name]
+        args.append(Tuple(*_arguments))
+        if _template:
+            args.append(Tuple(*_template))
+
+        obj = Function.__new__(cls, *args)
         obj._name = name
-        obj._arguments = arguments
+        obj._arguments = tuple(_arguments)
+        obj._template = tuple(_template)
+
         return obj
 
     @property
     def name(self):
         return self._name
 
     @property
     def arguments(self):
         return self._arguments
 
+    @property
+    def template(self):
+        return self._template
+
     def __str__(self):
-        return "%s(%s)" % (self.name, ', '.join(str(i) for i in self.arguments))
+        if self.template:
+            template = '<%s>' % ','.join(str(i) for i in self.template)
+        else:
+            template = ''
+        arguments = ', '.join(str(i) for i in self.arguments)
+        return "%s%s(%s)" % (self.name, template, arguments)
 
     __repr__ = __str__
 
     def _sympystr(self, printer):
         return str(self)
 
     func = Pickable._rebuild
 
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
+class MathFunction(DefFunction):
+
+    # Supposed to involve real operands
+    is_commutative = True
+
+
 class InlineIf(sympy.Expr, Pickable):
 
     """
     Symbolic representation of the C notation ``(C) ? a : b``.
     """
 
     __rargs__ = ('cond', 'true_expr', 'false_expr')
@@ -593,14 +674,98 @@
 
     __repr__ = __str__
 
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
+class Namespace(sympy.Expr, Pickable):
+
+    """
+    Symbolic representation of a C++ namespace `ns0::ns1::...`.
+    """
+
+    __rargs__ = ('items',)
+
+    def __new__(cls, items, **kwargs):
+        normalized_items = []
+        for i in as_tuple(items):
+            if isinstance(i, str):
+                normalized_items.append(ReservedWord(i))
+            elif isinstance(i, ReservedWord):
+                normalized_items.append(i)
+            else:
+                raise ValueError("`items` must be iterable of str or ReservedWord")
+
+        obj = sympy.Expr.__new__(cls)
+        obj._items = tuple(items)
+
+        return obj
+
+    def _hashable_content(self):
+        return super()._hashable_content() + self.items
+
+    @property
+    def items(self):
+        return self._items
+
+    def __str__(self):
+        return "::".join(str(i) for i in self.items)
+
+    __repr__ = __str__
+
+
+class Rvalue(sympy.Expr, Pickable):
+
+    """
+    A generic C++ rvalue, that is a value that occupies a temporary location in
+    memory.
+    """
+
+    __rargs__ = ('expr',)
+    __rkwargs__ = ('namespace', 'init')
+
+    def __new__(cls, expr, namespace=None, init=None):
+        args = [expr]
+        if namespace is not None:
+            args.append(namespace)
+        if init is not None:
+            args.append(init)
+
+        obj = sympy.Expr.__new__(cls, *args)
+
+        obj._expr = expr
+        obj._namespace = namespace
+        obj._init = init
+
+        return obj
+
+    @property
+    def expr(self):
+        return self._expr
+
+    @property
+    def namespace(self):
+        return self._namespace
+
+    @property
+    def init(self):
+        return self._init
+
+    def __str__(self):
+        rvalue = str(self.expr)
+        if self.namespace:
+            rvalue = "%s::%s" % (self.namespace, rvalue)
+        if self.init:
+            rvalue = "%s%s" % (rvalue, self.init)
+        return rvalue
+
+    __repr__ = __str__
+
+
 # *** Casting
 
 class CastStar(object):
 
     base = None
 
     def __new__(cls, base=''):
@@ -618,14 +783,26 @@
         globals()[clsp.__name__] = clsp
 
 
 class CHAR(Cast):
     _base_typ = 'char'
 
 
+class SHORT(Cast):
+    _base_typ = 'short'
+
+
+class USHORT(Cast):
+    _base_typ = 'unsigned short'
+
+
+class UCHAR(Cast):
+    _base_typ = 'unsigned char'
+
+
 class LONG(Cast):
     _base_typ = 'long'
 
 
 class ULONG(Cast):
     _base_typ = 'unsigned long'
 
@@ -634,28 +811,44 @@
     _base_typ = 'void'
 
 
 class CHARP(CastStar):
     base = CHAR
 
 
+class UCHARP(CastStar):
+    base = UCHAR
+
+
+class SHORTP(CastStar):
+    base = SHORT
+
+
+class USHORTP(CastStar):
+    base = USHORT
+
+
 cast_mapper = {
     np.int8: CHAR,
-    np.uint8: CHAR,
+    np.uint8: UCHAR,
+    np.int16: SHORT,  # noqa
+    np.uint16: USHORT,  # noqa
     int: INT,  # noqa
     np.int32: INT,  # noqa
     np.int64: LONG,
     np.uint64: ULONG,
     np.float32: FLOAT,  # noqa
     float: DOUBLE,  # noqa
     np.float64: DOUBLE,  # noqa
 
     (np.int8, '*'): CHARP,
-    (np.uint8, '*'): CHARP,
+    (np.uint8, '*'): UCHARP,
     (int, '*'): INTP,  # noqa
+    (np.uint16, '*'): USHORTP,  # noqa
+    (np.int16, '*'): SHORTP,  # noqa
     (np.int32, '*'): INTP,  # noqa
     (np.int64, '*'): INTP,  # noqa
     (np.float32, '*'): FLOATP,  # noqa
     (float, '*'): DOUBLEP,  # noqa
     (np.float64, '*'): DOUBLEP  # noqa
 }
```

### Comparing `devito-4.8.3/devito/symbolics/inspection.py` & `devito-4.8.4/devito/symbolics/inspection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import singledispatch
 
 import numpy as np
 from sympy import (Function, Indexed, Integer, Mul, Number,
                    Pow, S, Symbol, Tuple)
-from sympy.core.operations import AssocOp
 
 from devito.finite_differences import Derivative
 from devito.finite_differences.differentiable import IndexDerivative
 from devito.logger import warning
 from devito.symbolics.extended_sympy import (INT, CallFromPointer, Cast,
                                              DefFunction, ReservedWord)
 from devito.symbolics.queries import q_routine
@@ -44,14 +43,19 @@
     False
     >>> compare_ops(u[x] + u[x+1], u[x] + u[y+10])
     True
     """
     if type(e1) is type(e2) and len(e1.args) == len(e2.args):
         if e1.is_Atom:
             return True if e1 == e2 else False
+        elif isinstance(e1, IndexDerivative) and isinstance(e2, IndexDerivative):
+            if e1.mapper == e2.mapper:
+                return compare_ops(e1.expr, e2.expr)
+            else:
+                return False
         elif e1.is_Indexed and e2.is_Indexed:
             return True if e1.base == e2.base else False
         else:
             for a1, a2 in zip(e1.args, e2.args):
                 if not compare_ops(a1, a2):
                     return False
             return True
@@ -82,111 +86,130 @@
     except AttributeError:
         pass
     try:
         # At this point it must be a list of SymPy objects
         # We don't use SymPy's count_ops because we do not count integer arithmetic
         # (e.g., array index functions such as i+1 in A[i+1])
         # Also, the routine below is *much* faster than count_ops
+        seen = {}
         flops = 0
         for expr in as_tuple(exprs):
             # TODO: this if-then should be part of singledispatch too, but because
             # of the annoying symbolics/ vs types/ structuring, we can't do that
             # because of circular imports...
             if expr.is_Equality:
                 e = expr.rhs
                 if expr.is_Reduction:
                     flops += 1
             else:
                 e = expr
 
-            flops += _estimate_cost(e, estimate)[0]
+            flops += _estimate_cost(e, estimate, seen)[0]
 
         return flops
     except:
         warning("Cannot estimate cost of `%s`" % str(exprs))
         return 0
 
 
 estimate_values = {
     'elementary': 100,
     'pow': 50,
     'div': 5,
     'Abs': 5,
+    'floor': 1,
+    'ceil': 1
 }
 
 
+def dont_count_if_seen(func):
+    """
+    This decorator is used to avoid counting the same expression multiple
+    times. This is necessary because the same expression may appear multiple
+    times in the same expression tree or even across different expressions.
+    """
+    def wrapper(expr, estimate, seen):
+        try:
+            _, flags = seen[expr]
+            flops = 0
+        except KeyError:
+            flops, flags = seen[expr] = func(expr, estimate, seen)
+        return flops, flags
+    return wrapper
+
+
 @singledispatch
-def _estimate_cost(expr, estimate):
+def _estimate_cost(expr, estimate, seen):
     # Retval: flops (int), flag (bool)
     # The flag tells wether it's an integer expression (implying flops==0) or not
-    flops, flags = zip(*[_estimate_cost(a, estimate) for a in expr.args])
+    flops, flags = zip(*[_estimate_cost(a, estimate, seen) for a in expr.args])
     flops = sum(flops)
     if all(flags):
         # `expr` is an operation involving integer operands only
         # NOTE: one of the operands may contain, internally, non-integer
         # operations, e.g. the `a*b` in `2 + INT(a*b)`
         return flops, True
     else:
         return flops + (len(expr.args) - 1), False
 
 
 @_estimate_cost.register(Tuple)
 @_estimate_cost.register(CallFromPointer)
-def _(expr, estimate):
+def _(expr, estimate, seen):
     try:
-        flops, flags = zip(*[_estimate_cost(a, estimate) for a in expr.args])
+        flops, flags = zip(*[_estimate_cost(a, estimate, seen) for a in expr.args])
     except ValueError:
         flops, flags = [], []
     return sum(flops), all(flags)
 
 
 @_estimate_cost.register(Integer)
-def _(expr, estimate):
+def _(expr, estimate, seen):
     return 0, True
 
 
 @_estimate_cost.register(Number)
 @_estimate_cost.register(ReservedWord)
-def _(expr, estimate):
+def _(expr, estimate, seen):
     return 0, False
 
 
 @_estimate_cost.register(Symbol)
 @_estimate_cost.register(Indexed)
-def _(expr, estimate):
+def _(expr, estimate, seen):
     try:
         if issubclass(expr.dtype, np.integer):
             return 0, True
     except:
         pass
     return 0, False
 
 
 @_estimate_cost.register(Mul)
-def _(expr, estimate):
-    flops, flags = _estimate_cost.registry[object](expr, estimate)
+def _(expr, estimate, seen):
+    flops, flags = _estimate_cost.registry[object](expr, estimate, seen)
     if {S.One, S.NegativeOne}.intersection(expr.args):
         flops -= 1
     return flops, flags
 
 
 @_estimate_cost.register(INT)
-def _(expr, estimate):
-    return _estimate_cost(expr.base, estimate)[0], True
+def _(expr, estimate, seen):
+    return _estimate_cost(expr.base, estimate, seen)[0], True
 
 
 @_estimate_cost.register(Cast)
-def _(expr, estimate):
-    return _estimate_cost(expr.base, estimate)[0], False
+def _(expr, estimate, seen):
+    return _estimate_cost(expr.base, estimate, seen)[0], False
 
 
 @_estimate_cost.register(Function)
-def _(expr, estimate):
+def _(expr, estimate, seen):
     if q_routine(expr):
-        flops, _ = zip(*[_estimate_cost(a, estimate) for a in expr.args])
+        flops, _ = zip(*[_estimate_cost(a, estimate, seen) for a in expr.args])
         flops = sum(flops)
         if isinstance(expr, DefFunction):
             # Bypass user-defined or language-specific functions
             flops += 0
         elif estimate:
             try:
                 flops += estimate_values[type(expr).__name__]
@@ -196,16 +219,16 @@
             flops += 1
     else:
         flops = 0
     return flops, False
 
 
 @_estimate_cost.register(Pow)
-def _(expr, estimate):
-    flops, _ = zip(*[_estimate_cost(a, estimate) for a in expr.args])
+def _(expr, estimate, seen):
+    flops, _ = zip(*[_estimate_cost(a, estimate, seen) for a in expr.args])
     flops = sum(flops)
     if estimate:
         if expr.exp.is_Number:
             if expr.exp < 0:
                 flops += estimate_values['div']
             elif expr.exp == 0 or expr.exp == 1:
                 flops += 0
@@ -218,21 +241,23 @@
             flops += estimate_values['pow']
     else:
         flops += 1
     return flops, False
 
 
 @_estimate_cost.register(Derivative)
-def _(expr, estimate):
-    return _estimate_cost(expr._evaluate(expand=False), estimate)
+@dont_count_if_seen
+def _(expr, estimate, seen):
+    return _estimate_cost(expr._evaluate(expand=False), estimate, seen)
 
 
 @_estimate_cost.register(IndexDerivative)
-def _(expr, estimate):
-    flops, _ = _estimate_cost(expr.expr, estimate)
+@dont_count_if_seen
+def _(expr, estimate, seen):
+    flops, _ = _estimate_cost(expr.expr, estimate, seen)
 
     # It's an increment
     flops += 1
 
     # To be multiplied by the number of points this index sum implicitly
     # iterates over
     flops *= prod(i._size for i in expr.dimensions)
@@ -261,25 +286,18 @@
             else:
                 res = res and has_integer_args(a)
         except AttributeError:
             res = res and has_integer_args(a)
     return res
 
 
-def sympy_dtype(expr, default):
+def sympy_dtype(expr, base=None):
     """
-    Infer the dtype of the expression
-    or default if could not be determined.
+    Infer the dtype of the expression.
     """
-    # Symbol/... without argument, check its dtype
-    if len(expr.args) == 0:
+    dtypes = {base} - {None}
+    for i in expr.free_symbols:
         try:
-            return expr.dtype
+            dtypes.add(i.dtype)
         except AttributeError:
-            return default
-    else:
-        if not (isinstance(expr.func, AssocOp) or expr.is_Pow):
-            return default
-        else:
-            # Infer expression dtype from its arguments
-            dtype = infer_dtype([sympy_dtype(a, default) for a in expr.args])
-            return dtype or default
+            pass
+    return infer_dtype(dtypes)
```

### Comparing `devito-4.8.3/devito/symbolics/manipulation.py` & `devito-4.8.4/devito/symbolics/manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from functools import singledispatch
 
-from sympy import Pow, Add, Mul, Min, Max, SympifyError, Tuple, sympify
+from sympy import Pow, Add, Mul, Min, Max, S, SympifyError, Tuple, sympify
 from sympy.core.add import _addsort
 from sympy.core.mul import _mulsort
 
 from devito.symbolics.extended_sympy import DefFunction, rfunc
 from devito.symbolics.queries import q_leaf
 from devito.symbolics.search import retrieve_indexed, retrieve_functions
 from devito.tools import as_list, as_tuple, flatten, split, transitive_closure
@@ -142,14 +142,19 @@
         return expr.func(*args, evaluate=False)
     else:
         return expr._new_rawargs(*args)
 
 
 @_uxreplace_handle.register(Mul)
 def _(expr, args, kwargs):
+    # Perform some basic simplifications at least
+    args = [i for i in args if i != 1]
+    if any(i == 0 for i in args):
+        return S.Zero
+
     if all(i.is_commutative for i in args):
         _mulsort(args)
         _eval_numbers(expr, args)
         return expr.func(*args, evaluate=False)
     else:
         return expr._new_rawargs(*args)
```

### Comparing `devito-4.8.3/devito/symbolics/printer.py` & `devito-4.8.4/devito/symbolics/printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from mpmath.libmp import prec_to_dps, to_str
 from packaging.version import Version
 from sympy.logic.boolalg import BooleanFunction
 from sympy.printing.precedence import PRECEDENCE_VALUES, precedence
 from sympy.printing.c import C99CodePrinter
 
 from devito.arch.compiler import AOMPCompiler
-from devito.symbolics.inspection import has_integer_args
+from devito.symbolics.inspection import has_integer_args, sympy_dtype
 from devito.types.basic import AbstractFunction
 
 __all__ = ['ccode']
 
 
 class CodePrinter(C99CodePrinter):
 
@@ -85,14 +85,33 @@
         # http://en.cppreference.com/w/cpp/language/floating_literal
         p, q = int(expr.p), int(expr.q)
         if self.dtype == np.float64:
             return '%d.0/%d.0' % (p, q)
         else:
             return '%d.0F/%d.0F' % (p, q)
 
+    def _print_math_func(self, expr, nest=False, known=None):
+        cls = type(expr)
+        name = cls.__name__
+        if name not in self._prec_funcs:
+            return super()._print_math_func(expr, nest=nest, known=known)
+
+        try:
+            cname = self.known_functions[name]
+        except KeyError:
+            return super()._print_math_func(expr, nest=nest, known=known)
+
+        dtype = sympy_dtype(expr)
+        if dtype is np.float32:
+            cname += 'f'
+
+        args = ', '.join((self._print(arg) for arg in expr.args))
+
+        return '%s(%s)' % (cname, args)
+
     def _print_Pow(self, expr):
         # Need to override because of issue #1627
         # E.g., (Pow(h_x, -1) AND h_x.dtype == np.float32) => 1.0F/h_x
         try:
             if expr.exp == -1 and self.dtype == np.float32:
                 PREC = precedence(expr)
                 return '1.0F/%s' % self.parenthesize(expr.base, PREC)
@@ -183,14 +202,18 @@
 
     _print_EvalDerivative = C99CodePrinter._print_Add
 
     def _print_CallFromPointer(self, expr):
         indices = [self._print(i) for i in expr.params]
         return "%s->%s(%s)" % (expr.pointer, expr.call, ', '.join(indices))
 
+    def _print_CallFromComposite(self, expr):
+        indices = [self._print(i) for i in expr.params]
+        return "%s.%s(%s)" % (expr.pointer, expr.call, ', '.join(indices))
+
     def _print_FieldFromPointer(self, expr):
         return "%s->%s" % (expr.pointer, expr.field)
 
     def _print_FieldFromComposite(self, expr):
         return "%s.%s" % (expr.pointer, expr.field)
 
     def _print_ListInitializer(self, expr):
@@ -225,25 +248,41 @@
 
     def _print_TrigonometricFunction(self, expr):
         func_name = str(expr.func)
         if self.dtype == np.float32:
             func_name += 'f'
         return '%s(%s)' % (func_name, self._print(*expr.args))
 
+    def _print_DefFunction(self, expr):
+        arguments = [self._print(i) for i in expr.arguments]
+        if expr.template:
+            template = '<%s>' % ','.join([str(i) for i in expr.template])
+        else:
+            template = ''
+        return "%s%s(%s)" % (expr.name, template, ','.join(arguments))
+
+    _print_MathFunction = _print_DefFunction
+
     def _print_Fallback(self, expr):
         return expr.__str__()
 
-    _print_DefFunction = _print_Fallback
+    _print_Namespace = _print_Fallback
+    _print_Rvalue = _print_Fallback
     _print_MacroArgument = _print_Fallback
     _print_IndexedBase = _print_Fallback
     _print_IndexSum = _print_Fallback
-    _print_Keyword = _print_Fallback
+    _print_ReservedWord = _print_Fallback
     _print_Basic = _print_Fallback
 
 
+# Lifted from SymPy so that we go through our own `_print_math_func`
+for k in ('exp log sin cos tan ceiling floor').split():
+    setattr(CodePrinter, '_print_%s' % k, CodePrinter._print_math_func)
+
+
 # Always parenthesize IntDiv and InlineIf within expressions
 PRECEDENCE_VALUES['IntDiv'] = 1
 PRECEDENCE_VALUES['InlineIf'] = 1
 
 
 def ccode(expr, **settings):
     """Generate C++ code from an expression.
```

### Comparing `devito-4.8.3/devito/symbolics/queries.py` & `devito-4.8.4/devito/symbolics/queries.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/symbolics/search.py` & `devito-4.8.4/devito/symbolics/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sympy
+
 from devito.symbolics.queries import (q_indexed, q_function, q_terminal, q_leaf,
                                       q_symbol, q_dimension, q_derivative)
 from devito.tools import as_tuple
 
 __all__ = ['retrieve_indexed', 'retrieve_functions', 'retrieve_function_carriers',
            'retrieve_terminals', 'retrieve_symbols', 'retrieve_dimensions',
            'retrieve_derivatives', 'search']
@@ -44,15 +46,15 @@
             If True, propagate the search within an Indexed's indices. Defaults to False.
         """
         self.query = query
         self.collection = self.modes[mode]
         self.deep = deep
 
     def _next(self, expr):
-        if self.deep is True and expr.is_Indexed:
+        if self.deep and expr.is_Indexed:
             return expr.indices
         elif q_leaf(expr):
             return ()
         else:
             return expr.args
 
     def dfs(self, expr):
@@ -106,18 +108,26 @@
 
 
 def search(exprs, query, mode='unique', visit='dfs', deep=False):
     """Interface to Search."""
 
     assert mode in Search.modes, "Unknown mode"
 
-    searcher = Search(query, mode, deep)
+    if isinstance(query, type):
+        Q = lambda obj: isinstance(obj, query)
+    else:
+        Q = query
+
+    searcher = Search(Q, mode, deep)
 
     found = Search.modes[mode]()
     for e in as_tuple(exprs):
+        if not isinstance(e, sympy.Basic):
+            continue
+
         if visit == 'dfs':
             found.update(searcher.dfs(e))
         elif visit == 'bfs':
             found.update(searcher.bfs(e))
         elif visit == "bfs_first_hit":
             found.update(searcher.bfs_first_hit(e))
         else:
```

### Comparing `devito-4.8.3/devito/tools/abc.py` & `devito-4.8.4/devito/tools/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
             * `a._rebuild(1, c=7) -> x(1, 5, 7)`
         """
         for i in self.__rargs__[len(args):]:
             if i.startswith('*'):
                 args += tuple(getattr(self, i[1:]))
             else:
                 args += (getattr(self, i),)
+
+        args = list(args)
+        for k in list(kwargs):
+            if k in self.__rargs__:
+                args[self.__rargs__.index(k)] = kwargs.pop(k)
+
         kwargs.update({i: getattr(self, i) for i in self.__rkwargs__ if i not in kwargs})
 
         # Should we use a constum reconstructor?
         try:
             cls = self._rcls
         except AttributeError:
             cls = self.__class__
@@ -249,15 +255,15 @@
     Metaclass for singleton classes.
     """
 
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+            cls._instances[cls] = super().__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Stamp(object):
 
     """
     Uniquely identify objects.
```

### Comparing `devito-4.8.3/devito/tools/algorithms.py` & `devito-4.8.4/devito/tools/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/tools/data_structures.py` & `devito-4.8.4/devito/tools/data_structures.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from multidict import MultiDict
 
 from devito.tools import Pickable
 from devito.tools.utils import as_tuple, filter_ordered
 from devito.tools.algorithms import toposort
 
 __all__ = ['Bunch', 'EnrichedTuple', 'ReducerMap', 'DefaultOrderedDict',
-           'OrderedSet', 'PartialOrderTuple', 'DAG', 'frozendict',
-           'UnboundedMultiTuple']
+           'OrderedSet', 'Ordering', 'DAG', 'frozendict',
+           'UnboundTuple', 'UnboundedMultiTuple']
 
 
 class Bunch(object):
 
     """
     Bind together an arbitrary number of generic items. This is a mutable
     alternative to a ``namedtuple``.
@@ -25,23 +25,30 @@
         http://code.activestate.com/recipes/52308-the-simple-but-handy-collector-of\
         -a-bunch-of-named/?in=user-97991
     """
 
     def __init__(self, **kwargs):
         self.__dict__.update(kwargs)
 
+    def __repr__(self):
+        return "Bunch(%s)" % ", ".join(["%s=%s" % i for i in self.__dict__.items()])
+
+    def __iter__(self):
+        for i in self.__dict__.values():
+            yield i
+
 
 class EnrichedTuple(tuple, Pickable):
 
     """
     A tuple with an arbitrary number of additional attributes.
     """
 
     def __new__(cls, *items, getters=None, **kwargs):
-        obj = super(EnrichedTuple, cls).__new__(cls, items)
+        obj = super().__new__(cls, items)
         obj.__dict__.update(kwargs)
         obj._getters = OrderedDict(zip(getters or [], items))
         return obj
 
     def __getitem__(self, key):
         if isinstance(key, int):
             return super().__getitem__(key)
@@ -205,15 +212,15 @@
         return value
 
     def __reduce__(self):
         if self.default_factory is None:
             args = tuple()
         else:
             args = self.default_factory,
-        return type(self), args, None, None, self.items()
+        return type(self), args, None, None, self()
 
     def copy(self):
         return self.__copy__()
 
     def __copy__(self):
         return type(self)(self.default_factory, self)
 
@@ -275,99 +282,139 @@
     issubset = property(lambda self: self.__le__)
     issuperset = property(lambda self: self.__ge__)
     symmetric_difference = property(lambda self: self.__xor__)
     symmetric_difference_update = property(lambda self: self.__ixor__)
     union = property(lambda self: self.__or__)
 
 
-class PartialOrderTuple(tuple):
+class Ordering(tuple):
 
     """
     A tuple whose elements are ordered according to a set of relations.
 
     Parameters
     ----------
     items : object or iterable of objects
         The elements of the tuple.
     relations : iterable of tuples, optional
-        One or more binary relations between elements in ``items``. If not
-        provided, then ``items`` is interpreted as a totally ordered sequence.
+        One or more n-ary relations between the elements in `items`. If not
+        provided, then `items` is interpreted as a totally ordered sequence.
         If provided, then a (partial) ordering is computed and all elements in
-        ``items`` for which a relation is not provided are appended.
+        `items` for which a relation is not provided are appended.
+    mode : str, optional
+        If 'total' (default), the resulting object is interpreted as a totally
+        ordered sequence; the object's relations are simplified away and no
+        subsequent operation involving the Ordering will ever be able to alter
+        the obtained sequence. If 'partial', the outcome is a partially ordered
+        sequence; the relations as provided by the user are preserved, which
+        leaves room for further reordering upon future operations. If 'unordered',
+        the `relations` are ignored and the resulting object degenerates to an
+        unordered collection.
     """
-    def __new__(cls, items=None, relations=None):
+    def __new__(cls, items=None, relations=None, mode='total'):
+        assert mode in ('total', 'partial', 'unordered')
+
         items = as_tuple(items)
         if relations:
             items = cls.reorder(items, relations)
-        obj = super(PartialOrderTuple, cls).__new__(cls, items)
-        obj._relations = set(tuple(i) for i in as_tuple(relations))
+
+        obj = super().__new__(cls, items)
+
+        obj._relations = frozenset(cls.simplify_relations(relations, items, mode))
+        obj._mode = mode
+
         return obj
 
     @classmethod
     def reorder(cls, items, relations):
         return filter_ordered(toposort(relations) + list(items))
 
+    @classmethod
+    def simplify_relations(cls, relations, items, mode):
+        if mode == 'total':
+            return [tuple(items)]
+        elif mode == 'partial':
+            return [tuple(i) for i in as_tuple(relations)]
+        else:
+            return []
+
     def __eq__(self, other):
-        return super(PartialOrderTuple, self).__eq__(other) and\
-            self.relations == other.relations
+        return (super().__eq__(other) and
+                self.relations == other.relations and
+                self.mode == other.mode)
 
     def __hash__(self):
-        return hash(*([i for i in self] + list(self.relations)))
+        return hash(*([i for i in self] + list(self.relations) + [self.mode]))
 
     @property
     def relations(self):
         return self._relations
 
-    def generate_ordering(self):
-        raise NotImplementedError
+    @property
+    def mode(self):
+        return self._mode
 
 
 class DAG(object):
 
     """
     An implementation of a directed acyclic graph (DAG).
 
     Notes
     -----
     Originally extracted from:
 
         https://github.com/thieman/py-dag/
     """
 
-    def __init__(self, nodes=None, edges=None):
+    def __init__(self, nodes=None, edges=None, labels=None):
         self.graph = OrderedDict()
         self.labels = DefaultOrderedDict(dict)
+
         for node in as_tuple(nodes):
             self.add_node(node)
+
         for i in as_tuple(edges):
             try:
                 ind_node, dep_node = i
             except ValueError:
                 ind_node, dep_node, label = i
                 self.labels[ind_node][dep_node] = label
             self.add_edge(ind_node, dep_node)
 
+        for ind_node, i in (labels or {}).items():
+            for dep_node, v in i.items():
+                if dep_node in self.graph.get(ind_node, []):
+                    self.labels[ind_node][dep_node] = v
+
     def __contains__(self, key):
         return key in self.graph
 
     @property
     def nodes(self):
         return tuple(self.graph)
 
     @property
+    def roots(self):
+        return tuple(n for n in self.nodes if not self.predecessors(n))
+
+    @property
     def edges(self):
         ret = []
         for k, v in self.graph.items():
             ret.extend([(k, i) for i in v])
         return tuple(ret)
 
     @property
     def size(self):
         return len(self.graph)
 
+    def clone(self):
+        return self.__class__(self.nodes, self.edges, self.labels)
+
     def add_node(self, node_name, ignore_existing=False):
         """Add a node if it does not exist yet, or error out."""
         if node_name in self.graph:
             if ignore_existing is True:
                 return
             raise KeyError('node %s already exists' % node_name)
         self.graph[node_name] = OrderedSet()
@@ -408,14 +455,32 @@
         except KeyError:
             return default
 
     def predecessors(self, node):
         """Return a list of all predecessors of the given node."""
         return [key for key in self.graph if node in self.graph[key]]
 
+    def all_predecessors(self, node):
+        """
+        Return a list of all nodes ultimately predecessors of the given node
+        in the dependency graph, in topological order.
+        """
+        found = set()
+
+        def _all_predecessors(n):
+            if n in found:
+                return
+            found.add(n)
+            for predecessor in self.predecessors(n):
+                _all_predecessors(predecessor)
+
+        _all_predecessors(node)
+
+        return found
+
     def downstream(self, node):
         """Return a list of all nodes this node has edges towards."""
         if node not in self.graph:
             raise KeyError('node %s is not in graph' % node)
         return list(self.graph[node])
 
     def all_downstreams(self, node):
@@ -503,14 +568,36 @@
             mapper = OrderedDict()
             for n, g in enumerate(groups):
                 mapper.update({i: n for i in g})
             return mapper
         else:
             return tuple(groups)
 
+    def find_paths(self, node):
+        if node not in self.graph:
+            raise KeyError('node %s is not in graph' % node)
+
+        paths = []
+
+        def dfs(node, path):
+            path.append(node)
+
+            if not self.graph[node]:
+                paths.append(tuple(path))
+            else:
+                for child in self.graph[node]:
+                    dfs(child, path)
+
+            # Remove the node from the path to backtrack
+            path.pop()
+
+        dfs(node, [])
+
+        return tuple(paths)
+
 
 class frozendict(Mapping):
     """
     An immutable wrapper around dictionaries that implements the complete
     :py:class:`collections.Mapping` interface. It can be used as a drop-in
     replacement for dictionaries where immutability is desired.
 
@@ -548,87 +635,163 @@
             h = 0
             for key, value in self._dict.items():
                 h ^= hash((key, value))
             self._hash = h
         return self._hash
 
 
-class UnboundedMultiTuple(object):
+class UnboundTuple(tuple):
+    """
+    An UnboundedTuple is a tuple that can be
+    infinitely iterated over.
+
+    Examples
+    --------
+    >>> ub = UnboundTuple((1, 2),(3, 4))
+    >>> ub
+    UnboundTuple(UnboundTuple(1, 2), UnboundTuple(3, 4))
+    >>> ub.next()
+    UnboundTuple(1, 2)
+    >>> ub.next()
+    UnboundTuple(3, 4)
+    >>> ub.next()
+    UnboundTuple(3, 4)
+    """
+
+    def __new__(cls, *items, **kwargs):
+        nitems = []
+        for i in as_tuple(items):
+            if isinstance(i, UnboundTuple):
+                nitems.append(i)
+            elif isinstance(i, Iterable):
+                nitems.append(UnboundTuple(*i))
+            else:
+                nitems.append(i)
+
+        obj = super().__new__(cls, tuple(nitems))
+        obj.last = len(nitems)
+        obj.current = 0
+
+        return obj
+
+    @property
+    def prod(self):
+        return np.prod(self)
+
+    def reset(self):
+        self.iter()
+        return self
+
+    def iter(self):
+        self.current = 0
+
+    def next(self):
+        if not self:
+            return None
+        item = self[self.current]
+        if self.current == self.last-1 or self.current == -1:
+            self.current = self.last
+        else:
+            self.current += 1
+        return item
+
+    def __len__(self):
+        return self.last
+
+    def __repr__(self):
+        sitems = [s.__repr__() for s in self]
+        return "%s(%s)" % (self.__class__.__name__, ", ".join(sitems))
+
+    def __getitem__(self, idx):
+        if not self:
+            return None
+        if isinstance(idx, slice):
+            start = idx.start or 0
+            stop = idx.stop or self.last
+            if stop < 0:
+                stop = self.last + stop
+            step = idx.step or 1
+            return UnboundTuple(*[self[i] for i in range(start, stop, step)])
+        try:
+            if idx >= self.last-1:
+                return super().__getitem__(self.last-1)
+            else:
+                return super().__getitem__(idx)
+        except TypeError:
+            # Slice, ...
+            return UnboundTuple(self[i] for i in idx)
+
+
+class UnboundedMultiTuple(UnboundTuple):
 
     """
     An UnboundedMultiTuple is an ordered collection of tuples that can be
     infinitely iterated over.
 
     Examples
     --------
     >>> ub = UnboundedMultiTuple([1, 2], [3, 4])
     >>> ub
-    UnboundedMultiTuple((1, 2), (3, 4))
+    UnboundedMultiTuple(UnboundTuple(1, 2), UnboundTuple(3, 4))
     >>> ub.iter()
     >>> ub
-    UnboundedMultiTuple(*(1, 2), (3, 4))
+    UnboundedMultiTuple(UnboundTuple(1, 2), UnboundTuple(3, 4))
     >>> ub.next()
     1
     >>> ub.next()
     2
     >>> ub.iter()
     >>> ub.iter()  # No effect, tip has reached the last tuple
     >>> ub.iter()  # No effect, tip has reached the last tuple
     >>> ub
-    UnboundedMultiTuple((1, 2), *(3, 4))
+    UnboundedMultiTuple(UnboundTuple(1, 2), UnboundTuple(3, 4))
     >>> ub.next()
     3
     >>> ub.next()
     4
     >>> ub.iter()  # Reloads the last iterator
     >>> ub.next()
     3
     """
 
-    def __init__(self, *items):
-        # Normalize input
-        nitems = []
-        for i in as_tuple(items):
-            if isinstance(i, Iterable):
-                nitems.append(tuple(i))
-            else:
-                raise ValueError("Expected sequence, got %s" % type(i))
-
-        self.items = tuple(nitems)
-        self.tip = -1
-        self.curiter = None
-
-    def __repr__(self):
-        items = [str(i) for i in self.items]
-        if self.curiter is not None:
-            items[self.tip] = "*%s" % items[self.tip]
-        return "%s(%s)" % (self.__class__.__name__, ", ".join(items))
+    def __new__(cls, *items, **kwargs):
+        obj = super().__new__(cls, *items, **kwargs)
+        # MultiTuple are un-initialized
+        obj.current = None
+        return obj
 
-    def iter(self):
-        if not self.items:
-            raise ValueError("No tuples available")
-        self.tip = min(self.tip + 1, max(len(self.items) - 1, 0))
-        self.curiter = iter(self.items[self.tip])
+    def reset(self):
+        self.current = None
+        return self
 
-    def next(self):
-        if self.curiter is None:
+    def curitem(self):
+        if self.current is None:
             raise StopIteration
-        return next(self.curiter)
+        if not self:
+            return None
+        return self[self.current]
 
+    def nextitem(self):
+        if not self:
+            return None
+        self.iter()
+        return self.curitem()
 
-class UnboundTuple(object):
-    """
-    A simple data structure that returns the last element forever once reached
-    """
+    def index(self, item):
+        return self.index(item)
 
-    def __init__(self, items):
-        self.items = as_tuple(items)
-        self.last = len(self.items)
-        self.current = 0
+    def iter(self):
+        if self.current is None:
+            self.current = 0
+        else:
+            self.current = min(self.current + 1, self.last - 1)
+        self[self.current].reset()
+        return
 
     def next(self):
-        item = self.items[self.current]
-        self.current = min(self.last - 1, self.current+1)
-        return item
-
-    def __len__(self):
-        return self.last
+        if not self:
+            return None
+        if self.current is None:
+            raise StopIteration
+        if self[self.current].current >= self[self.current].last:
+            raise StopIteration
+        return self[self.current].next()
```

### Comparing `devito-4.8.3/devito/tools/dtypes_lowering.py` & `devito-4.8.4/devito/tools/dtypes_lowering.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 """
 
 import ctypes
 
 import numpy as np
 from cgen import dtype_to_ctype as cgen_dtype_to_ctype
 
+from .utils import as_tuple
+
 __all__ = ['int2', 'int3', 'int4', 'float2', 'float3', 'float4', 'double2',  # noqa
            'double3', 'double4', 'dtypes_vector_mapper', 'dtype_to_mpidtype',
            'dtype_to_cstr', 'dtype_to_ctype', 'dtype_to_mpitype', 'dtype_len',
            'ctypes_to_cstr', 'c_restrict_void_p', 'ctypes_vector_mapper',
-           'is_external_ctype', 'infer_dtype']
+           'is_external_ctype', 'infer_dtype', 'CustomDtype']
 
 
 # *** Custom np.dtypes
 
 # NOTE: the following is inspired by pyopencl.cltypes
 
 mapper = {
@@ -71,29 +73,60 @@
         if not isinstance(field_name, str) or field_name in field_names:
             raise ValueError("Expected field name different than x,y,z,w")
         if count <= max(counts):
             raise ValueError("Expected at least 5 fields")
 
         self.update(build_dtypes_vector([field_name], [count]))
 
-    def get_base_dtype(self, v):
+    def get_base_dtype(self, v, default=None):
         for (base_dtype, count), dtype in self.items():
             if dtype is v:
                 return base_dtype
 
-        raise ValueError
+        if default is not None:
+            return default
+        else:
+            raise ValueError
 
 
 dtypes_vector_mapper = DTypesVectorMapper()
 # Standard vector dtypes
 dtypes_vector_mapper.update(build_dtypes_vector(field_names, counts))
 # Fallbacks
 dtypes_vector_mapper.update({(v, 1): v for v in mapper.values()})
 
 
+# *** Custom types escaping both the numpy and ctypes namespaces
+
+
+class CustomDtype(object):
+
+    def __init__(self, name, template=None, modifier=None):
+        self.name = name
+        self.template = as_tuple(template)
+        self.modifier = modifier or ''
+
+    def __eq__(self, other):
+        return (isinstance(other, CustomDtype) and
+                self.name == other.name and
+                self.template == other.template and
+                self.modifier == other.modifier)
+
+    def __hash__(self):
+        return hash((self.name, self.template, self.modifier))
+
+    def __repr__(self):
+        template = '<%s>' % ','.join([str(i) for i in self.template])
+        return "%s%s%s" % (self.name,
+                           template if self.template else '',
+                           self.modifier)
+
+    __str__ = __repr__
+
+
 # *** np.dtypes lowering
 
 
 def dtype_to_cstr(dtype):
     """Translate numpy.dtype into C string."""
     return cgen_dtype_to_ctype(dtype)
 
@@ -173,14 +206,16 @@
 # *** ctypes lowering
 
 
 def ctypes_to_cstr(ctype, toarray=None):
     """Translate ctypes types into C strings."""
     if ctype in ctypes_vector_mapper.values():
         retval = ctype.__name__
+    elif isinstance(ctype, CustomDtype):
+        retval = str(ctype)
     elif issubclass(ctype, ctypes.Structure):
         retval = 'struct %s' % ctype.__name__
     elif issubclass(ctype, ctypes.Union):
         retval = 'union %s' % ctype.__name__
     elif issubclass(ctype, ctypes._Pointer):
         if toarray:
             retval = ctypes_to_cstr(ctype._type_, '(* %s)' % toarray)
@@ -259,16 +294,18 @@
     """
     Given a set of np.dtypes, return the "winning" dtype:
 
         * In the case of multiple floating dtypes, return the dtype with
           highest precision;
         * If there's at least one floating dtype, ignore any integer dtypes.
     """
-    fdtypes = {i for i in dtypes if np.issubdtype(i, np.floating)}
+    # Resolve the vector types, if any
+    dtypes = {dtypes_vector_mapper.get_base_dtype(i, i) for i in dtypes}
 
+    fdtypes = {i for i in dtypes if np.issubdtype(i, np.floating)}
     if len(fdtypes) > 1:
         return max(fdtypes, key=lambda i: np.dtype(i).itemsize)
     elif len(fdtypes) == 1:
         return fdtypes.pop()
     elif len(dtypes) == 1:
         return dtypes.pop()
     else:
```

### Comparing `devito-4.8.3/devito/tools/memoization.py` & `devito-4.8.4/devito/tools/memoization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/tools/os_helper.py` & `devito-4.8.4/devito/tools/os_helper.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/tools/threading.py` & `devito-4.8.4/devito/tools/threading.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/tools/timing.py` & `devito-4.8.4/devito/tools/timing.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/tools/utils.py` & `devito-4.8.4/devito/tools/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from functools import reduce
 from itertools import chain, combinations, groupby, product, zip_longest
 from operator import attrgetter, mul
+import sys
 import types
 
 import numpy as np
 import sympy
 
 __all__ = ['prod', 'as_tuple', 'is_integer', 'generator', 'grouper', 'split',
            'roundm', 'powerset', 'invert', 'flatten', 'single_or', 'filter_ordered',
            'as_mapper', 'filter_sorted', 'pprint', 'sweep', 'all_equal', 'as_list',
            'indices_to_slices', 'indices_to_sections', 'transitive_closure',
-           'humanbytes', 'contains_val']
+           'humanbytes', 'contains_val', 'sorted_priority']
+
+
+# Some utils run faster with Python>=3.7
+vi = sys.version_info
+py_ge_37 = (vi.major, vi.minor) >= (3, 7)
 
 
 def prod(iterable, initial=1):
     return reduce(mul, iterable, initial)
 
 
 def as_list(item, type=None, length=None):
@@ -153,40 +159,57 @@
     Note that this is not a XOR function, according to the truth table of the XOR
     boolean function with n > 2 inputs. Hence the name ``single_or``."""
     # No
     i = iter(l)
     return any(i) and not any(i)
 
 
-def filter_ordered(elements, key=None):
-    """
-    Filter elements in a list while preserving order.
+if py_ge_37:
+    def filter_ordered(elements, key=None):
+        # This method exploits the fact that dictionary keys are unique and ordered
+        # (since Python 3.7). It's concise and often faster for larger lists
 
-    Parameters
-    ----------
-    key : callable, optional
-        Conversion key used during equality comparison.
-    """
-    if isinstance(elements, types.GeneratorType):
-        elements = list(elements)
-    seen = set()
-    if key is None:
-        try:
-            unordered, inds = np.unique(elements, return_index=True)
-            return unordered[np.argsort(inds)].tolist()
-        except:
-            return sorted(list(set(elements)), key=elements.index)
-    else:
-        ret = []
-        for e in elements:
-            k = key(e)
-            if k not in seen:
-                ret.append(e)
-                seen.add(k)
-        return ret
+        if isinstance(elements, types.GeneratorType):
+            elements = list(elements)
+
+        if key is None:
+            return list(dict.fromkeys(elements))
+        else:
+            return list(dict(zip([key(i) for i in elements], elements)).values())
+
+else:
+    def filter_ordered(elements, key=None):
+        if isinstance(elements, types.GeneratorType):
+            elements = list(elements)
+
+        seen = set()
+        if key is None:
+            try:
+                unordered, inds = np.unique(elements, return_index=True)
+                return unordered[np.argsort(inds)].tolist()
+            except:
+                return sorted(list(set(elements)), key=elements.index)
+        else:
+            ret = []
+            for e in elements:
+                k = key(e)
+                if k not in seen:
+                    ret.append(e)
+                    seen.add(k)
+            return ret
+
+
+filter_ordered.__doc__ = """\
+Filter elements in a list while preserving order.
+
+Parameters
+----------
+key : callable, optional
+    Conversion key used during equality comparison.
+"""
 
 
 def filter_sorted(elements, key=None):
     """
     Filter elements in a list and sort them by key. The default key is
     ``operator.attrgetter('name')``.
     """
@@ -305,7 +328,38 @@
         return '%d KB' % round(B / KB)
     elif MB <= B < GB:
         return '%d MB' % round(B / MB)
     elif GB <= B < TB:
         return '%.1f GB' % round(B / GB, 1)
     elif TB <= B:
         return '%.2f TB' % round(B / TB, 1)
+
+
+def sorted_priority(items, priority):
+    """
+    Sort items based on their type priority.
+
+    Rules:
+
+        * Each type has an integer priority.
+        * Types with higher priority precede types with lower priority.
+        * Types with same priority are sorted based on the type name.
+        * Types with unknown priority are given 0-priority.
+
+    Parameters
+    ----------
+    items : iterable
+        The objects to be sorted.
+    priority : dict
+        A dictionary from types to integer values.
+    """
+
+    def key(i):
+        for cls in sorted(priority, key=priority.get, reverse=True):
+            if isinstance(i, cls):
+                v = priority[cls]
+                break
+        else:
+            v = 0
+        return (v, str(type(i)))
+
+    return sorted(items, key=key, reverse=True)
```

### Comparing `devito-4.8.3/devito/tools/visitors.py` & `devito-4.8.4/devito/tools/visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/__init__.py` & `devito-4.8.4/devito/types/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/args.py` & `devito-4.8.4/devito/types/args.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/array.py` & `devito-4.8.4/devito/types/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from ctypes import POINTER, Structure, c_void_p, c_ulong
-from math import ceil
 
 import numpy as np
 from cached_property import cached_property
-from sympy import Expr, Number
+from sympy import Expr
 
-from devito.parameters import configuration
 from devito.tools import (Reconstructable, as_tuple, c_restrict_void_p,
-                          dtype_to_ctype, dtypes_vector_mapper)
+                          dtype_to_ctype, dtypes_vector_mapper, is_integer)
 from devito.types.basic import AbstractFunction
 from devito.types.utils import CtypesFactory, DimensionTuple
 
-__all__ = ['Array', 'ArrayMapped', 'ArrayObject', 'PointerArray', 'Bundle']
+__all__ = ['Array', 'ArrayMapped', 'ArrayObject', 'PointerArray', 'Bundle',
+           'ComponentAccess', 'Bag']
 
 
 class ArrayBasic(AbstractFunction):
 
     is_ArrayBasic = True
 
     @classmethod
@@ -99,86 +98,60 @@
     Arrays are created and managed directly by Devito (IOW, they are not
     expected to be used directly in user code).
     """
 
     is_Array = True
 
     __rkwargs__ = (AbstractFunction.__rkwargs__ +
-                   ('dimensions', 'liveness', 'space', 'scope', 'initvalue'))
+                   ('dimensions', 'liveness', 'scope', 'initvalue'))
 
     def __new__(cls, *args, **kwargs):
         kwargs.update({'options': {'evaluate': False}})
-        space = kwargs.get('space', 'local')
+        space = kwargs.setdefault('space', 'local')
 
         if cls is Array and space == 'mapped':
             return AbstractFunction.__new__(ArrayMapped, *args, **kwargs)
         else:
             return AbstractFunction.__new__(cls, *args, **kwargs)
 
     def __init_finalize__(self, *args, **kwargs):
-        super(Array, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         self._liveness = kwargs.get('liveness', 'lazy')
         assert self._liveness in ['eager', 'lazy']
 
-        self._space = kwargs.get('space', 'local')
-        assert self._space in ['local', 'mapped', 'host']
-
         self._scope = kwargs.get('scope', 'heap')
         assert self._scope in ['heap', 'stack', 'static', 'constant', 'shared']
 
         self._initvalue = kwargs.get('initvalue')
         assert self._initvalue is None or self._scope != 'heap'
 
+    @classmethod
+    def __dtype_setup__(cls, **kwargs):
+        return kwargs.get('dtype', np.float32)
+
     def __padding_setup__(self, **kwargs):
         padding = kwargs.get('padding')
         if padding is None:
-            padding = [(0, 0) for _ in range(self.ndim)]
-            if kwargs.get('autopadding', configuration['autopadding']):
-                # Heuristic 1; Arrays are typically introduced for temporaries
-                # introduced during compilation, and are almost always used together
-                # with loop blocking.  Since the typical block size is a multiple of
-                # the SIMD vector length, `vl`, padding is made such that the
-                # NODOMAIN size is a multiple of `vl` too
-
-                # Heuristic 2: the right-NODOMAIN size is not only a multiple of
-                # `vl`, but also guaranteed to be *at least* greater or equal than
-                # `vl`, so that the compiler can tweak loop trip counts to maximize
-                # the effectiveness of SIMD vectorization
-
-                # Let UB be a function that rounds up a value `x` to the nearest
-                # multiple of the SIMD vector length
-                vl = configuration['platform'].simd_items_per_reg(self.dtype)
-                ub = lambda x: int(ceil(x / vl)) * vl
-
-                fvd_halo_size = sum(self.halo[-1])
-                fvd_pad_size = (ub(fvd_halo_size) - fvd_halo_size) + vl
-
-                padding[-1] = (0, fvd_pad_size)
-            return tuple(padding)
-        elif isinstance(padding, int):
-            return tuple((0, padding) for _ in range(self.ndim))
+            padding = ((0, 0),)*self.ndim
+        elif isinstance(padding, DimensionTuple):
+            padding = tuple(padding[d] for d in self.dimensions)
+        elif is_integer(padding):
+            padding = tuple((0, padding) for _ in range(self.ndim))
         elif isinstance(padding, tuple) and len(padding) == self.ndim:
-            return tuple((0, i) if isinstance(i, int) else i for i in padding)
+            padding = tuple((0, i) if is_integer(i) else i for i in padding)
         else:
             raise TypeError("`padding` must be int or %d-tuple of ints" % self.ndim)
-
-    @classmethod
-    def __dtype_setup__(cls, **kwargs):
-        return kwargs.get('dtype', np.float32)
+        return DimensionTuple(*padding, getters=self.dimensions)
 
     @property
     def liveness(self):
         return self._liveness
 
     @property
-    def space(self):
-        return self._space
-
-    @property
     def scope(self):
         return self._scope
 
     @property
     def _C_ctype(self):
         return POINTER(dtype_to_ctype(self.dtype))
 
@@ -187,26 +160,14 @@
         return self._liveness == 'eager'
 
     @property
     def _mem_internal_lazy(self):
         return self._liveness == 'lazy'
 
     @property
-    def _mem_local(self):
-        return self._space == 'local'
-
-    @property
-    def _mem_mapped(self):
-        return self._space == 'mapped'
-
-    @property
-    def _mem_host(self):
-        return self._space == 'host'
-
-    @property
     def _mem_stack(self):
         return self._scope in ('stack', 'shared')
 
     @property
     def _mem_heap(self):
         return self._scope == 'heap'
 
@@ -342,15 +303,15 @@
     __rkwargs__ = ('name', 'dimensions', 'array')
 
     def __new__(cls, *args, **kwargs):
         kwargs.update({'options': {'evaluate': False}})
         return AbstractFunction.__new__(cls, *args, **kwargs)
 
     def __init_finalize__(self, *args, **kwargs):
-        super(PointerArray, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         self._array = kwargs['array']
         assert self._array.is_Array
 
     @classmethod
     def __dtype_setup__(cls, **kwargs):
         return kwargs['array'].dtype
@@ -446,50 +407,47 @@
         return self.c0.is_DiscreteFunction
 
     @property
     def is_TimeFunction(self):
         return self.c0.is_TimeFunction
 
     @property
-    def grid(self):
-        return self.c0.grid
+    def is_Input(self):
+        return all(i.is_Input for i in self.components)
+
+    @property
+    def is_autopaddable(self):
+        return all(i.is_autopaddable for i in self.components)
 
     # Other properties and methods
 
     @property
+    def handles(self):
+        return (self,)
+
+    @property
     def components(self):
         return self._components
 
     @property
     def ncomp(self):
         return len(self.components)
 
     @property
-    def symbolic_shape(self):
-        # A Bundle may be defined over a SteppingDimension, which is of unknown
-        # size, hence we gotta use the actual numeric size instead
-        ret = []
-        for d, s, v in zip(self.dimensions, super().symbolic_shape, self.c0.shape):
-            if d.is_Stepping:
-                ret.append(Number(v))
-            else:
-                ret.append(s)
-        return DimensionTuple(*ret, getters=self.dimensions)
-
-    @property
     def initvalue(self):
         return None
 
     # CodeSymbol overrides defaulting to self.c0's behaviour
 
     for i in ['_mem_internal_eager', '_mem_internal_lazy', '_mem_local',
               '_mem_mapped', '_mem_host', '_mem_stack', '_mem_constant',
               '_mem_shared', '_size_domain', '_size_halo', '_size_owned',
               '_size_padding', '_size_nopad', '_size_nodomain', '_offset_domain',
-              '_offset_halo', '_offset_owned', '_dist_dimensions', '_C_get_field']:
+              '_offset_halo', '_offset_owned', '_dist_dimensions', '_C_get_field',
+              'grid', 'symbolic_shape']:
         locals()[i] = property(lambda self, v=i: getattr(self.c0, v))
 
     @property
     def _mem_heap(self):
         return not self._mem_stack
 
     @property
@@ -519,24 +477,38 @@
     def _C_ctype(self):
         if self._mem_mapped:
             return ArrayMapped._C_ctype
         else:
             return POINTER(dtype_to_ctype(self.dtype))
 
 
+class Bag(Bundle):
+
+    """
+    A Bag is like a Bundle but it doesn't represent a concrete object
+    in the generated code. It's used by the compiler because, in certain
+    passes, treating groups of Function homogeneously is more practical
+    than keeping them separated.
+    """
+
+    @property
+    def handles(self):
+        return self.components
+
+
 class ComponentAccess(Expr, Reconstructable):
 
     _component_names = ('x', 'y', 'z', 'w')
 
     __rkwargs__ = ('index',)
 
     def __new__(cls, arg, index=0, **kwargs):
         if not arg.is_Indexed:
             raise ValueError("Expected Indexed, got `%s` instead" % type(arg))
-        if not isinstance(index, int) or index > 3:
+        if not is_integer(index) or index > 3:
             raise ValueError("Expected 0 <= index < 4")
 
         obj = Expr.__new__(cls, arg)
         obj._index = index
 
         return obj
```

### Comparing `devito-4.8.3/devito/types/basic.py` & `devito-4.8.4/devito/types/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from functools import reduce
 from operator import mul
 
 import numpy as np
 import sympy
 
 from sympy.core.assumptions import _assume_rules
+from sympy.core.decorators import call_highest_priority
 from cached_property import cached_property
 
 from devito.data import default_allocator
+from devito.parameters import configuration
 from devito.tools import (Pickable, as_tuple, ctypes_to_cstr, dtype_to_ctype,
                           frozendict, memoized_meth, sympy_mutex)
 from devito.types.args import ArgProvider
 from devito.types.caching import Cached, Uncached
 from devito.types.lazy import Evaluable
 from devito.types.utils import DimensionTuple
 
@@ -34,15 +36,16 @@
     its type.
 
     The _mem_* properties describe the object memory allocation strategy. There
     are three axes, with a few possible values each:
 
         * "liveness": `_mem_external`, `_mem_internal_eager`, `_mem_internal_lazy`
         * "space": `_mem_local`, `_mem_mapped`, `_mem_host`
-        * "scope": `_mem_stack`, `_mem_heap`, `_mem_constant`, `_mem_shared`
+        * "scope": `_mem_stack`, `_mem_heap`, `_mem_global`, `_mem_shared`,
+                   `_mem_constant`
 
     For example, an object that is `<_mem_internal_lazy, _mem_local, _mem_heap>`
     is allocated within the Operator entry point, on either the host or device
     memory (but not both), and on the heap. Refer to the __doc__ of the single
     _mem_* properties for more info. Obviously, not all triplets make sense
     for a given architecture.
     """
@@ -169,37 +172,44 @@
         True if the associated data is systematically allocated in the host DRAM.
         """
         return False
 
     @property
     def _mem_stack(self):
         """
-        True if the associated data should be allocated on the stack, False otherwise.
+        True if the associated data is allocated on the stack, False otherwise.
         """
         return False
 
     @property
     def _mem_heap(self):
         """
-        True if the associated data gets allocated on the heap, False otherwise.
+        True if the associated data is allocated on the heap, False otherwise.
         """
         return False
 
     @property
+    def _mem_global(self):
+        """
+        True if the symbol is globally scoped, False otherwise.
+        """
+        return self._mem_constant
+
+    @property
     def _mem_constant(self):
         """
-        True if the associated data gets allocated in global constant memory,
-        False otherwise.
+        True if the associated data is allocated in global constant memory,
+        False otherwise. This is a special case of `_mem_global`.
         """
         return False
 
     @property
     def _mem_shared(self):
         """
-        True if the associated data gets allocated in so called shared memory,
+        True if the associated data is allocated in so called shared memory,
         False otherwise.
         """
         return False
 
 
 class Basic(CodeSymbol):
 
@@ -233,14 +243,15 @@
     -----
     The AbstractFunction sub-hierarchy is implemented in :mod:`dense.py`.
     The AbstractTensor sub-hierarchy is implemented in :mod:`tensor.py`.
     """
 
     # Top hierarchy
     is_AbstractFunction = False
+    is_AbstractTensor = False
     is_AbstractObject = False
 
     # Symbolic objects created internally by Devito
     is_Symbol = False
     is_ArrayBasic = False
     is_Array = False
     is_PointerArray = False
@@ -267,14 +278,18 @@
     # Time dependence
     is_TimeDependent = False
 
     # Some other properties
     is_PerfKnob = False  # Does it impact the Operator performance?
 
     @property
+    def base(self):
+        return self
+
+    @property
     def bound_symbols(self):
         """
         Unlike SymPy, we systematically define `bound_symbols` on all of
         the API and internal objects that may be used to construct an
         Operator.
         """
         return set()
@@ -354,14 +369,25 @@
     def __init__(self, *args, **kwargs):
         # no-op, the true init is performed by __init_finalize__
         pass
 
     def __init_finalize__(self, *args, **kwargs):
         self._is_const = kwargs.get('is_const', False)
 
+    def __eq__(self, other):
+        return (type(self) is type(other) and
+                self.dtype is other.dtype and
+                self.is_const == other.is_const and
+                super().__eq__(other))
+
+    __hash__ = sympy.Symbol.__hash__
+
+    def _hashable_content(self):
+        return super()._hashable_content() + (self.dtype, self.is_const)
+
     @property
     def dtype(self):
         return self._dtype
 
     @property
     def indices(self):
         return ()
@@ -379,18 +405,14 @@
         return 0
 
     @property
     def symbolic_shape(self):
         return ()
 
     @property
-    def base(self):
-        return self
-
-    @property
     def function(self):
         return self
 
     def _evaluate(self, **kwargs):
         return self
 
     def indexify(self, indices=None):
@@ -648,14 +670,30 @@
         except TypeError:
             # We can end up here when `_fromrep` is called through the default _new
             # when input `comps` don't have grid or dimensions. For example
             # `test_non_devito_tens` in `test_tensor.py`.
             pass
         return newobj
 
+    @classmethod
+    def __subfunc_setup__(cls, *args, **kwargs):
+        """Setup each component of the tensor as a Devito type."""
+        return []
+
+    @property
+    def grid(self):
+        """
+        A Tensor is expected to have all its components defined over the same grid
+        """
+        grids = {getattr(c, 'grid', None) for c in self.flat()} - {None}
+        if len(grids) == 0:
+            return None
+        assert len(grids) == 1
+        return grids.pop()
+
     def _infer_dims(self):
         grids = {getattr(c, 'grid', None) for c in self.flat()} - {None}
         dimensions = {d for c in self.flat()
                       for d in getattr(c, 'dimensions', ())} - {None}
         # If none of the components are devito objects, returns a sympy Matrix
         if len(grids) == 0 and len(dimensions) == 0:
             return None, None
@@ -689,14 +727,23 @@
             return new.applyfunc(lambda x: getattr(x, 'T', x))
         return new
 
     def adjoint(self, inner=True):
         # Real valued adjoint is transpose
         return self.transpose(inner=inner)
 
+    @call_highest_priority('__radd__')
+    def __add__(self, other):
+        try:
+            # Most case support sympy add
+            return super().__add__(other)
+        except TypeError:
+            # Sympy doesn't support add with scalars
+            return self.applyfunc(lambda x: x + other)
+
     def _eval_matrix_mul(self, other):
         """
         Copy paste from sympy to avoid explicit call to sympy.Add
         TODO: fix inside sympy
         """
         other_len = other.rows*other.cols
         new_len = self.rows*other.cols
@@ -718,19 +765,14 @@
                 vec = [mat[a]*other_mat[b] for a, b in zip(row_indices, col_indices)]
                 new_mat[i] = sum(vec)
 
         # Get new class and return product
         newcls = self.classof_prod(other, new_mat)
         return newcls._new(self.rows, other.cols, new_mat, copy=False)
 
-    @classmethod
-    def __subfunc_setup__(cls, *args, **kwargs):
-        """Setup each component of the tensor as a Devito type."""
-        return []
-
 
 class AbstractFunction(sympy.Function, Basic, Pickable, Evaluable):
 
     """
     Base class for tensor symbols, cached by both SymPy and Devito. It inherits
     from and mimicks the behaviour of a sympy.Function.
 
@@ -789,20 +831,23 @@
     is_regular = True
     """
     True if data and iteration points are aligned. Cases where they won't be
     aligned (currently unsupported): Functions defined on SubDomains; compressed
     Functions; etc.
     """
 
-    is_compact = True
+    is_autopaddable = False
     """
-    True if data is allocated as a single, contiguous chunk of memory.
+    True if the Function can be padded automatically by the Devito runtime,
+    thus increasing its size, False otherwise. Note that this property has no
+    effect if autopadding is disabled, which is the default behavior.
     """
 
-    __rkwargs__ = ('name', 'dtype', 'grid', 'halo', 'padding', 'alias', 'function')
+    __rkwargs__ = ('name', 'dtype', 'grid', 'halo', 'padding', 'ghost',
+                   'alias', 'space', 'function')
 
     def __new__(cls, *args, **kwargs):
         # Preprocess arguments
         args, kwargs = cls.__args_setup__(*args, **kwargs)
 
         # Extract the `indices`, as perhaps they're explicitly provided
         dimensions, indices = cls.__indices_setup__(*args, **kwargs)
@@ -840,15 +885,14 @@
         newobj._dtype = cls.__dtype_setup__(**kwargs)
 
         # All objects created off an existing AbstractFunction `f` (e.g.,
         # via .func, or .subs, such as `f(x + 1)`) keep a reference to `f`
         # through the `function` field
         newobj.function = function or newobj
 
-        # Initialization
         newobj.__init_finalize__(*args, **kwargs)
 
         return newobj
 
     def __init__(self, *args, **kwargs):
         # no-op, the true init is performed by __init_finalize__
         pass
@@ -885,32 +929,39 @@
         # With the legacy caching framework this wasn't necessary because
         # the function name was already encoded in the class_key
         class_key, args, exp, coeff = super().sort_key(order=order)
         args = (len(args[1]) + 1, (self.name,) + args[1])
         return class_key, args, exp, coeff
 
     def __init_finalize__(self, *args, **kwargs):
-        # Setup halo and padding regions
+        # Setup halo, padding, and ghost regions
         self._is_halo_dirty = False
         self._halo = self.__halo_setup__(**kwargs)
         self._padding = self.__padding_setup__(**kwargs)
+        self._ghost = self.__ghost_setup__(**kwargs)
 
         # There may or may not be a `Grid`
         self._grid = kwargs.get('grid')
 
         # A `Distributor` to handle domain decomposition
         self._distributor = self.__distributor_setup__(**kwargs)
 
         # Symbol properties
-        # "Aliasing" another DiscreteFunction means that `self` logically
+
+        # "Aliasing" another AbstractFunction means that `self` logically
         # represents another object. For example, `self` might be used as the
         # formal parameter of a routine generated by the compiler, where the
         # routines is applied to several actual DiscreteFunctions
         self._alias = kwargs.get('alias', False)
 
+        # The memory space of the AbstractFunction
+        # See `_mem_{local,mapped,host}.__doc__` for more info
+        self._space = kwargs.get('space', 'mapped')
+        assert self._space in ['local', 'mapped', 'host']
+
     @classmethod
     def __args_setup__(cls, *args, **kwargs):
         """
         Preprocess *args and **kwargs before object initialization.
 
         Notes
         -----
@@ -930,39 +981,56 @@
 
     @classmethod
     def __dtype_setup__(cls, **kwargs):
         """Extract the object data type from ``kwargs``."""
         return None
 
     def __halo_setup__(self, **kwargs):
-        halo = tuple(kwargs.get('halo', [(0, 0) for i in range(self.ndim)]))
+        halo = tuple(kwargs.get('halo', ((0, 0),)*self.ndim))
         return DimensionTuple(*halo, getters=self.dimensions)
 
     def __padding_setup__(self, **kwargs):
-        padding = tuple(kwargs.get('padding', [(0, 0) for i in range(self.ndim)]))
+        padding = tuple(kwargs.get('padding', ((0, 0),)*self.ndim))
         return DimensionTuple(*padding, getters=self.dimensions)
 
+    def __padding_setup_smart__(self, **kwargs):
+        nopadding = ((0, 0),)*self.ndim
+
+        if kwargs.get('autopadding', configuration['autopadding']):
+            # The padded Dimension
+            candidates = self.space_dimensions
+            if not candidates:
+                return nopadding
+            d = candidates[-1]
+
+            mmts = configuration['platform'].max_mem_trans_size(self.dtype)
+            remainder = self._size_nopad[d] % mmts
+            if remainder == 0:
+                # Already a multiple of `mmts`, no need to pad
+                return nopadding
+
+            dpadding = (0, (mmts - remainder))
+            padding = [(0, 0)]*self.ndim
+            padding[self.dimensions.index(d)] = dpadding
+
+            return tuple(padding)
+        else:
+            return nopadding
+
+    def __ghost_setup__(self, **kwargs):
+        return (0, 0)
+
     def __distributor_setup__(self, **kwargs):
         # There may or may not be a `Distributor`. In the latter case, the
         # AbstractFunction is to be considered "local" to each MPI rank
         try:
             return kwargs.get('grid').distributor
         except AttributeError:
             return kwargs.get('distributor')
 
-    @cached_property
-    def _honors_autopadding(self):
-        """
-        True if the actual padding is greater or equal than whatever autopadding
-        would produce, False otherwise.
-        """
-        autopadding = self.__padding_setup__(autopadding=True)
-        return all(l0 >= l1 and r0 >= r1
-                   for (l0, r0), (l1, r1) in zip(self.padding, autopadding))
-
     @property
     def name(self):
         """The name of the object."""
         return self._name
 
     @property
     def indices(self):
@@ -985,14 +1053,23 @@
                               getters=self.dimensions)
 
     @property
     def dimensions(self):
         """Tuple of Dimensions representing the object indices."""
         return self._dimensions
 
+    @cached_property
+    def space_dimensions(self):
+        """Tuple of Dimensions defining the physical space."""
+        return tuple(d for d in self.dimensions if d.is_Space)
+
+    @property
+    def base(self):
+        return self.indexed
+
     @property
     def _eval_deriv(self):
         return self
 
     @property
     def _is_on_grid(self):
         """
@@ -1117,32 +1194,48 @@
         return self._halo
 
     @property
     def padding(self):
         return self._padding
 
     @property
+    def ghost(self):
+        return self._ghost
+
+    @property
     def is_const(self):
         return False
 
     @property
     def alias(self):
         return self._alias
 
     @property
+    def space(self):
+        return self._space
+
+    @property
     def _C_name(self):
         return "%s_vec" % self.name
 
     @cached_property
     def _C_symbol(self):
         return BoundSymbol(name=self._C_name, dtype=self.dtype, function=self.function)
 
     @property
+    def _mem_local(self):
+        return self._space == 'local'
+
+    @property
     def _mem_mapped(self):
-        return not self._mem_local
+        return self._space == 'mapped'
+
+    @property
+    def _mem_host(self):
+        return self._space == 'host'
 
     def _make_pointer(self):
         """Generate a symbolic pointer to self."""
         raise NotImplementedError
 
     @cached_property
     def _dist_dimensions(self):
@@ -1200,14 +1293,22 @@
         right = tuple(i for _, i in np.add(self._halo, self._padding))
 
         sizes = tuple(Size(i, j) for i, j in np.add(self._halo, self._padding))
 
         return DimensionTuple(*sizes, getters=self.dimensions, left=left, right=right)
 
     @cached_property
+    def _size_ghost(self):
+        """
+        Number of points in the ghost region, that is the two areas before
+        and after the allocated data.
+        """
+        return Size(*self._ghost)
+
+    @cached_property
     def _offset_domain(self):
         """Number of points before the first domain element."""
         offsets = tuple(np.add(self._size_padding.left, self._size_halo.left))
         return DimensionTuple(*offsets, getters=self.dimensions)
 
     @cached_property
     def _offset_halo(self):
@@ -1416,14 +1517,18 @@
     def _hashable_content(self):
         return super()._hashable_content() + (self.base.function,)
 
     @cached_property
     def indices(self):
         return DimensionTuple(*super().indices, getters=self.function.dimensions)
 
+    @cached_property
+    def dimensions(self):
+        return self.function.dimensions
+
     @property
     def function(self):
         return self.base.function
 
     @property
     def dtype(self):
         return self.function.dtype
```

### Comparing `devito-4.8.3/devito/types/caching.py` & `devito-4.8.4/devito/types/caching.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/constant.py` & `devito-4.8.4/devito/types/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,16 @@
     Symbol representing a constant, scalar value in symbolic equations.
     A Constant carries a scalar value.
 
     Parameters
     ----------
     name : str
         Name of the symbol.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to ``np.float32``.
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
 
     Examples
     --------
     >>> from devito import Constant
     >>> c = Constant(name='c')
     >>> c
     c
```

### Comparing `devito-4.8.3/devito/types/dense.py` & `devito-4.8.4/devito/types/dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import namedtuple
 from ctypes import POINTER, Structure, c_int, c_ulong, c_void_p, cast, byref
 from functools import wraps, reduce
-from math import ceil
 from operator import mul
 
 import numpy as np
 import sympy
 from psutil import virtual_memory
 from cached_property import cached_property
 
@@ -14,14 +13,15 @@
                          Data, default_allocator)
 from devito.exceptions import InvalidArgument
 from devito.logger import debug, warning
 from devito.mpi import MPI
 from devito.parameters import configuration
 from devito.symbolics import FieldFromPointer, normalize_args
 from devito.finite_differences import Differentiable, generate_fd_shortcuts
+from devito.finite_differences.tools import fd_weights_registry
 from devito.tools import (ReducerMap, as_tuple, c_restrict_void_p, flatten, is_integer,
                           memoized_meth, dtype_to_ctype, humanbytes)
 from devito.types.dimension import Dimension
 from devito.types.args import ArgProvider
 from devito.types.caching import CacheManager
 from devito.types.basic import AbstractFunction, Size
 from devito.types.utils import Buffer, DimensionTuple, NODE, CELL
@@ -40,14 +40,17 @@
 
     Notes
     -----
     Users should not instantiate this class directly. Use Function or
     SparseFunction (or their subclasses) instead.
     """
 
+    # Default method for the finite difference approximation weights computation.
+    _default_fd = 'taylor'
+
     # Required by SymPy, otherwise the presence of __getitem__ will make SymPy
     # think that a DiscreteFunction is actually iterable, thus breaking many of
     # its key routines (e.g., solve)
     _iterable = False
 
     is_Input = True
     is_DiscreteFunction = True
@@ -61,20 +64,21 @@
 
     def __init_finalize__(self, *args, function=None, **kwargs):
         # Staggering metadata
         self._staggered = self.__staggered_setup__(**kwargs)
 
         # Now that *all* __X_setup__ hooks have been called, we can let the
         # superclass constructor do its job
-        super(DiscreteFunction, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         # Symbolic (finite difference) coefficients
-        self._coefficients = kwargs.get('coefficients', 'standard')
-        if self._coefficients not in ('standard', 'symbolic'):
-            raise ValueError("coefficients must be `standard` or `symbolic`")
+        self._coefficients = kwargs.get('coefficients', self._default_fd)
+        if self._coefficients not in fd_weights_registry:
+            raise ValueError("coefficients must be one of %s"
+                             " not %s" % (str(fd_weights_registry), self._coefficients))
 
         # Data-related properties
         self._data = None
         self._first_touch = kwargs.get('first_touch', configuration['first-touch'])
         self._allocator = kwargs.get('allocator') or default_allocator()
 
         # Data initialization
@@ -95,15 +99,15 @@
             self._initializer = None
             if len(initializer) > 0:
                 self.data_with_halo[:] = initializer[:]
             else:
                 # This is a corner case -- we might get here, for example, when
                 # running with MPI and some processes get 0-size arrays after
                 # domain decomposition. We touch the data anyway to avoid the
-                # case ``self._data is None``
+                # case `self._data is None`
                 self.data
         else:
             raise ValueError("`initializer` must be callable or buffer, not %s"
                              % type(initializer))
 
     _subs = Differentiable._subs
 
@@ -122,15 +126,16 @@
                 # Clear up both SymPy and Devito caches to drop unreachable data
                 CacheManager.clear(force=False)
 
                 # Allocate the actual data object
                 self._data = self._DataType(self.shape_allocated, self.dtype,
                                             modulo=self._mask_modulo,
                                             allocator=self._allocator,
-                                            distributor=self._distributor)
+                                            distributor=self._distributor,
+                                            padding=self._size_ghost)
 
                 # Initialize data
                 if self._first_touch:
                     assign(self, 0)
                 if callable(self._initializer):
                     if self._first_touch:
                         warning("`first touch` together with `initializer` causing "
@@ -195,22 +200,14 @@
 
     @property
     def coefficients(self):
         """Form of the coefficients of the function."""
         return self._coefficients
 
     @cached_property
-    def _coeff_symbol(self):
-        if self.coefficients == 'symbolic':
-            return sympy.Function('W')
-        else:
-            raise ValueError("Function was not declared with symbolic "
-                             "coefficients.")
-
-    @cached_property
     def shape(self):
         """
         Shape of the domain region. The domain constitutes the area of the
         data written to by an Operator.
 
         Notes
         -----
@@ -223,15 +220,15 @@
         """
         Shape of the domain region. The domain constitutes the area of the
         data written to by an Operator.
 
         Notes
         -----
         In an MPI context, this is the *local* domain region shape.
-        Alias to ``self.shape``.
+        Alias to `self.shape`.
         """
         return self.shape
 
     @cached_property
     def shape_with_halo(self):
         """
         Shape of the domain+outhalo region. The outhalo is the region
@@ -440,15 +437,15 @@
         start : int or tuple of ints
             The `slice` start in each dimension.
         stop : int or tuple of ints
             The final point of the `slice` to include.
 
         Notes
         -----
-        Alias to ``self.data._gather``.
+        Alias to `self.data._gather`.
 
         Note that gathering data from large simulations onto a single rank may
         result in memory blow-up and hence should use this method judiciously.
         """
         return self.data._gather(start=start, stop=stop, step=step, rank=rank)
 
     @property
@@ -457,15 +454,15 @@
         """
         The domain data values.
 
         Elements are stored in row-major format.
 
         Notes
         -----
-        Alias to ``self.data``.
+        Alias to `self.data`.
 
         With this accessor you are claiming that you will modify the values you
         get back. If you only need to look at the values, use
         :meth:`data_ro_domain` instead.
         """
         self._is_halo_dirty = True
         return self._data._global(self._mask_domain, self._decomposition)
@@ -620,30 +617,25 @@
     def local_indices(self):
         """
         Tuple of slices representing the global indices that logically
         belong to the calling MPI rank.
 
         Notes
         -----
-        Given a Function ``f(x, y)`` with shape ``(nx, ny)``, when *not* using
-        MPI this property will return ``(slice(0, nx-1), slice(0, ny-1))``. On
+        Given a Function `f(x, y)` with shape `(nx, ny)`, when *not* using
+        MPI this property will return `(slice(0, nx-1), slice(0, ny-1))`. On
         the other hand, when MPI is used, the local ranges depend on the domain
-        decomposition, which is carried by ``self.grid``.
+        decomposition, which is carried by `self.grid`.
         """
         if self._distributor is None:
             return tuple(slice(0, s) for s in self.shape)
         else:
             return tuple(self._distributor.glb_slices.get(d, slice(0, s))
                          for s, d in zip(self.shape, self.dimensions))
 
-    @cached_property
-    def space_dimensions(self):
-        """Tuple of Dimensions defining the physical space."""
-        return tuple(d for d in self.dimensions if d.is_Space)
-
     @property
     def initializer(self):
         if isinstance(self._data, np.ndarray):
             return self.data_with_halo.view(np.ndarray)
         else:
             return self._initializer
 
@@ -663,19 +655,21 @@
                                           (_C_field_nopad_size, POINTER(c_ulong)),
                                           (_C_field_domain_size, POINTER(c_ulong)),
                                           (_C_field_halo_size, POINTER(c_int)),
                                           (_C_field_halo_ofs, POINTER(c_int)),
                                           (_C_field_owned_ofs, POINTER(c_int)),
                                           (_C_field_dmap, c_void_p)]}))
 
-    def _C_make_dataobj(self, data):
+    def _C_make_dataobj(self, alias=None, **args):
         """
         A ctypes object representing the DiscreteFunction that can be passed to
         an Operator.
         """
+        key = alias or self
+        data = args[key.name]
         dataobj = byref(self._C_ctype._type_())
         dataobj._obj.data = data.ctypes.data_as(c_restrict_void_p)
         dataobj._obj.size = (c_ulong*self.ndim)(*data.shape)
         # MPI-related fields
         dataobj._obj.npsize = (c_ulong*self.ndim)(*[i - sum(j) for i, j in
                                                     zip(data.shape, self._size_padding)])
         dataobj._obj.dsize = (c_ulong*self.ndim)(*self._size_domain)
@@ -745,15 +739,16 @@
         else:
             raise ValueError("Unknown region `%s`" % str(region))
 
         return RegionMeta(offset, size)
 
     def _halo_exchange(self):
         """Perform the halo exchange with the neighboring processes."""
-        if not MPI.Is_initialized() or MPI.COMM_WORLD.size == 1:
+        if not MPI.Is_initialized() or MPI.COMM_WORLD.size == 1 or \
+                not configuration['mpi']:
             # Nothing to do
             return
         if MPI.COMM_WORLD.size > 1 and self._distributor is None:
             raise RuntimeError("`%s` cannot perform a halo exchange as it has "
                                "no Grid attached" % self.name)
 
         neighborhood = self._distributor.neighborhood
@@ -796,16 +791,16 @@
         alias : DiscreteFunction, optional
             To bind the argument values to different names.
         """
         key = alias or self
         args = ReducerMap({key.name: self._data_buffer})
 
         # Collect default dimension arguments from all indices
-        for i, s in zip(self.dimensions, self.shape):
-            args.update(i._arg_defaults(_min=0, size=s))
+        for a, i, s in zip(key.dimensions, self.dimensions, self.shape):
+            args.update(i._arg_defaults(_min=0, size=s, alias=a))
 
         return args
 
     def _arg_values(self, **kwargs):
         """
         A map of argument values after evaluating user input. If no
         user input is provided, return a default value.
@@ -837,44 +832,44 @@
     def _arg_check(self, args, intervals, **kwargs):
         """
         Check that `args` contains legal runtime values bound to `self`.
 
         Raises
         ------
         InvalidArgument
-            If, given the runtime values `args`, an out-of-bounds array
-            access would be performed, or if shape/dtype don't match with
-            self's shape/dtype.
+            If an incompatibility is detected.
         """
         if self.name not in args:
             raise InvalidArgument("No runtime value for `%s`" % self.name)
 
-        key = args[self.name]
-        if len(key.shape) != self.ndim:
+        data = args[self.name]
+
+        if len(data.shape) != self.ndim:
             raise InvalidArgument("Shape %s of runtime value `%s` does not match "
                                   "dimensions %s" %
-                                  (key.shape, self.name, self.dimensions))
-        if key.dtype != self.dtype:
+                                  (data.shape, self.name, self.dimensions))
+        if data.dtype != self.dtype:
             warning("Data type %s of runtime value `%s` does not match the "
-                    "Function data type %s" % (key.dtype, self.name, self.dtype))
+                    "Function data type %s" % (data.dtype, self.name, self.dtype))
 
-        for i, s in zip(self.dimensions, key.shape):
+        # Check each Dimension for potential OOB accesses
+        for i, s in zip(self.dimensions, data.shape):
             i._arg_check(args, s, intervals[i])
 
         if args.options['index-mode'] == 'int32' and \
            args.options['linearize'] and \
-           self.size - 1 >= np.iinfo(np.int32).max:
+           data.size - 1 >= np.iinfo(np.int32).max:
             raise InvalidArgument("`%s`, with its %d elements, may be too big for "
                                   "int32 pointer arithmetic, which might cause an "
                                   "overflow. Use the 'index-mode=int64' option"
-                                  % (self, self.size))
+                                  % (self, data.size))
 
     def _arg_finalize(self, args, alias=None):
         key = alias or self
-        return {key.name: self._C_make_dataobj(args[key.name])}
+        return {key.name: self._C_make_dataobj(alias=key, **args)}
 
     # Pickling support
 
     @property
     def _pickle_rkwargs(self):
         # Picklying carries data over, if available
         return tuple(self.__rkwargs__) + ('initializer',)
@@ -895,41 +890,46 @@
     ----------
     name : str
         Name of the symbol.
     grid : Grid, optional
         Carries shape, dimensions, and dtype of the Function. When grid is not
         provided, shape and dimensions must be given. For MPI execution, a
         Grid is compulsory.
-    space_order : int or 3-tuple of ints, optional
-        Discretisation order for space derivatives. Defaults to 1. ``space_order`` also
-        impacts the number of points available around a generic point of interest.  By
-        default, ``space_order`` points are available on both sides of a generic point of
-        interest, including those nearby the grid boundary. Sometimes, fewer points
-        suffice; in other scenarios, more points are necessary. In such cases, instead of
-        an integer, one can pass a 3-tuple ``(o, lp, rp)`` indicating the discretization
-        order (``o``) as well as the number of points on the left (``lp``) and right
-        (``rp``) sides of a generic point of interest.
+    space_order : int or 3-tuple of ints, optional, default=1
+        Discretisation order for space derivatives.
+        `space_order` also impacts the number of points available around a
+        generic point of interest.  By default, `space_order` points are
+        available on both sides of a generic point of interest, including those
+        nearby the grid boundary. Sometimes, fewer points suffice; in other
+        scenarios, more points are necessary. In such cases, instead of an
+        integer, one can pass:
+          * a 3-tuple `(o, lp, rp)` indicating the discretization order
+            (`o`) as well as the number of points on the left (`lp`) and
+            right (`rp`) sides of a generic point of interest;
+          * a 2-tuple `(o, ((lp0, rp0), (lp1, rp1), ...))` indicating the
+            discretization order (`o`) as well as the number of points on
+            the left/right sides of a generic point of interest for each
+            SpaceDimension.
     shape : tuple of ints, optional
-        Shape of the domain region in grid points. Only necessary if ``grid`` isn't given.
+        Shape of the domain region in grid points. Only necessary if `grid`
+        isn't given.
     dimensions : tuple of Dimension, optional
-        Dimensions associated with the object. Only necessary if ``grid`` isn't given.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to ``np.float32``.
-    staggered : Dimension or tuple of Dimension or Stagger, optional
+        Dimensions associated with the object. Only necessary if `grid` isn't
+        given.
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
+    staggered : Dimension or tuple of Dimension or Stagger, optional, default=None
         Define how the Function is staggered.
-    initializer : callable or any object exposing the buffer interface, optional
+    initializer : callable or any object exposing the buffer interface, default=None
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
     padding : int or tuple of ints, optional
-        .. deprecated:: shouldn't be used; padding is now automatically inserted.
-
         Allocate extra grid points to maximize data access alignment. When a tuple
         of ints, one int per Dimension should be provided.
 
     Examples
     --------
     Creation
 
@@ -970,39 +970,49 @@
 
     >>> g.dx2
     Derivative(g(x, y), (x, 2))
 
     Notes
     -----
     The parameters must always be given as keyword arguments, since SymPy
-    uses ``*args`` to (re-)create the dimension arguments of the symbolic object.
+    uses `*args` to (re-)create the dimension arguments of the symbolic object.
     """
 
     is_Function = True
 
+    is_autopaddable = True
+
     __rkwargs__ = (DiscreteFunction.__rkwargs__ +
                    ('space_order', 'shape_global', 'dimensions'))
 
     def _cache_meta(self):
         # Attach additional metadata to self's cache entry
         return {'nbytes': self.size}
 
     def __init_finalize__(self, *args, **kwargs):
-        super(Function, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         # Space order
         space_order = kwargs.get('space_order', 1)
         if isinstance(space_order, int):
             self._space_order = space_order
-        elif isinstance(space_order, tuple) and len(space_order) == 3:
-            self._space_order, _, _ = space_order
+        elif isinstance(space_order, tuple) and len(space_order) >= 2:
+            self._space_order = space_order[0]
         else:
-            raise TypeError("`space_order` must be int or 3-tuple of ints")
+            raise TypeError("Invalid `space_order`")
+
+        # Acquire derivative shortcuts
+        if self is self.function:
+            self._fd = self.__fd_setup__()
+        else:
+            # E.g., `self is f(x + i0, y)` and `self.function is f(x, y)`
+            # Dynamically genereating derivative shortcuts is expensive; we
+            # can clearly avoid that here though!
+            self._fd = self.function._fd
 
-        self._fd = self.__fd_setup__()
         # Flag whether it is a parameter or a variable.
         # Used at operator evaluation to evaluate the Function at the
         # variable location (i.e. if the variable is staggered in x the
         # parameter has to be computed at x + hx/2)
         self._is_parameter = kwargs.get('parameter', False)
 
     def __fd_setup__(self):
@@ -1101,75 +1111,74 @@
         halo = kwargs.get('halo')
         if halo is not None:
             if isinstance(halo, DimensionTuple):
                 halo = tuple(halo[d] for d in self.dimensions)
         else:
             space_order = kwargs.get('space_order', 1)
             if isinstance(space_order, int):
-                halo = (space_order, space_order)
+                v = (space_order, space_order)
+                halo = [v if i.is_Space else (0, 0) for i in self.dimensions]
+
             elif isinstance(space_order, tuple) and len(space_order) == 3:
-                _, left_points, right_points = space_order
-                halo = (left_points, right_points)
+                _, l, r = space_order
+                halo = [(l, r) if i.is_Space else (0, 0) for i in self.dimensions]
+
+            elif isinstance(space_order, tuple) and len(space_order) == 2:
+                _, space_halo = space_order
+                if not isinstance(space_halo, tuple) or \
+                   not all(isinstance(i, tuple) for i in space_halo) or \
+                   len(space_halo) != len(self.space_dimensions):
+                    raise TypeError("Invalid `space_order`")
+                v = list(space_halo)
+                halo = [v.pop(0) if i.is_Space else (0, 0)
+                        for i in self.dimensions]
+
             else:
-                raise TypeError("`space_order` must be int or 3-tuple of ints")
-            halo = tuple(halo if i.is_Space else (0, 0) for i in self.dimensions)
+                raise TypeError("Invalid `space_order`")
         return DimensionTuple(*halo, getters=self.dimensions)
 
     def __padding_setup__(self, **kwargs):
         padding = kwargs.get('padding')
         if padding is None:
-            if kwargs.get('autopadding', configuration['autopadding']):
-                # Auto-padding
-                # 0-padding in all Dimensions except in the Fastest Varying Dimension,
-                # `fvd`, which is the innermost one
-                padding = [(0, 0) for i in self.dimensions[:-1]]
-                fvd = self.dimensions[-1]
-                # Let UB be a function that rounds up a value `x` to the nearest
-                # multiple of the SIMD vector length, `vl`
-                vl = configuration['platform'].simd_items_per_reg(self.dtype)
-                ub = lambda x: int(ceil(x / vl)) * vl
-                # Given the HALO and DOMAIN sizes, the right-PADDING is such that:
-                # * the `fvd` size is a multiple of `vl`
-                # * it contains *at least* `vl` points
-                # This way:
-                # * all first grid points along the `fvd` will be cache-aligned
-                # * there is enough room to round up the loop trip counts to maximize
-                #   the effectiveness SIMD vectorization
-                fvd_pad_size = (ub(self._size_nopad[fvd]) - self._size_nopad[fvd]) + vl
-                padding.append((0, fvd_pad_size))
+            if self.is_autopaddable:
+                padding = self.__padding_setup_smart__(**kwargs)
             else:
-                padding = tuple((0, 0) for d in self.dimensions)
+                padding = super().__padding_setup__(**kwargs)
+
         elif isinstance(padding, DimensionTuple):
             padding = tuple(padding[d] for d in self.dimensions)
+
         elif isinstance(padding, int):
             padding = tuple((0, padding) if d.is_Space else (0, 0)
                             for d in self.dimensions)
+
         elif isinstance(padding, tuple) and len(padding) == self.ndim:
             padding = tuple((0, i) if isinstance(i, int) else i for i in padding)
+
         else:
             raise TypeError("`padding` must be int or %d-tuple of ints" % self.ndim)
         return DimensionTuple(*padding, getters=self.dimensions)
 
     @property
     def space_order(self):
         """The space order."""
         return self._space_order
 
     def sum(self, p=None, dims=None):
         """
-        Generate a symbolic expression computing the sum of ``p`` points
-        along the spatial dimensions ``dims``.
+        Generate a symbolic expression computing the sum of `p` points
+        along the spatial dimensions `dims`.
 
         Parameters
         ----------
         p : int, optional
             The number of summands. Defaults to the halo size.
         dims : tuple of Dimension, optional
             The Dimensions along which the sum is computed. Defaults to
-            ``self``'s spatial dimensions.
+            `self`'s spatial dimensions.
         """
         points = []
         for d in (as_tuple(dims) or self.space_dimensions):
             if p is None:
                 lp = self._size_inhalo[d].left
                 rp = self._size_inhalo[d].right
             else:
@@ -1178,24 +1187,24 @@
             indices = [d - i for i in range(lp, 0, -1)]
             indices.extend([d + i for i in range(rp)])
             points.extend([self.subs({d: i}) for i in indices])
         return sum(points)
 
     def avg(self, p=None, dims=None):
         """
-        Generate a symbolic expression computing the average of ``p`` points
-        along the spatial dimensions ``dims``.
+        Generate a symbolic expression computing the average of `p` points
+        along the spatial dimensions `dims`.
 
         Parameters
         ----------
         p : int, optional
             The number of summands. Defaults to the halo size.
         dims : tuple of Dimension, optional
             The Dimensions along which the average is computed. Defaults to
-            ``self``'s spatial dimensions.
+            `self`'s spatial dimensions.
         """
         tot = self.sum(p, dims)
         return tot / len(tot.args)
 
 
 class TimeFunction(Function):
 
@@ -1211,56 +1220,62 @@
     ----------
     name : str
         Name of the symbol.
     grid : Grid, optional
         Carries shape, dimensions, and dtype of the Function. When grid is not
         provided, shape and dimensions must be given. For MPI execution, a
         Grid is compulsory.
-    space_order : int or 3-tuple of ints, optional
-        Discretisation order for space derivatives. Defaults to 1. ``space_order`` also
-        impacts the number of points available around a generic point of interest.  By
-        default, ``space_order`` points are available on both sides of a generic point of
-        interest, including those nearby the grid boundary. Sometimes, fewer points
-        suffice; in other scenarios, more points are necessary. In such cases, instead of
-        an integer, one can pass a 3-tuple ``(o, lp, rp)`` indicating the discretization
-        order (``o``) as well as the number of points on the left (``lp``) and right
-        (``rp``) sides of a generic point of interest.
+    space_order : int or 3-tuple of ints, optional, default=1
+        Discretisation order for space derivatives.
+        `space_order` also impacts the number of points available around a
+        generic point of interest.  By default, `space_order` points are
+        available on both sides of a generic point of interest, including those
+        nearby the grid boundary. Sometimes, fewer points suffice; in other
+        scenarios, more points are necessary. In such cases, instead of an
+        integer, one can pass:
+          * a 3-tuple `(o, lp, rp)` indicating the discretization order
+            (`o`) as well as the number of points on the left (`lp`) and
+            right (`rp`) sides of a generic point of interest;
+          * a 2-tuple `(o, ((lp0, rp0), (lp1, rp1), ...))` indicating the
+            discretization order (`o`) as well as the number of points on
+            the left/right sides of a generic point of interest for each
+            SpaceDimension.
     time_order : int, optional
         Discretization order for time derivatives. Defaults to 1.
     shape : tuple of ints, optional
-        Shape of the domain region in grid points. Only necessary if `grid` isn't given.
+        Shape of the domain region in grid points. Only necessary if `grid`
+        isn't given.
     dimensions : tuple of Dimension, optional
-        Dimensions associated with the object. Only necessary if `grid` isn't given.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to `np.float32`.
-    save : int or Buffer, optional
-        By default, ``save=None``, which indicates the use of alternating buffers. This
-        enables cyclic writes to the TimeFunction. For example, if the TimeFunction
-        ``u(t, x)`` has shape (3, 100), then, in an Operator, ``t`` will assume the
-        values ``1, 2, 0, 1, 2, 0, 1, ...`` (note that the very first value depends
-        on the stencil equation in which ``u`` is written.). The default size of the time
-        buffer when ``save=None`` is ``time_order + 1``.  To specify a different size for
-        the time buffer, one should use the syntax ``save=Buffer(mysize)``.
-        Alternatively, if all of the intermediate results are required (or, simply, to
-        avoid using an alternating buffer), an explicit value for ``save`` ( an integer)
-        must be provided.
-    time_dim : Dimension, optional
-        TimeDimension to be used in the TimeFunction. Defaults to ``grid.time_dim``.
-    staggered : Dimension or tuple of Dimension or Stagger, optional
+        Dimensions associated with the object. Only necessary if `grid` isn't
+        given.
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
+    save : int or Buffer, optional, default=None
+        By default, `save=None`, which indicates the use of alternating
+        buffers. This enables cyclic writes to the TimeFunction. For example,
+        if the TimeFunction `u(t, x)` has shape (3, 100), then, in an Operator,
+        `t` will assume the values `1, 2, 0, 1, 2, 0, 1, ...` (note that the
+        very first value depends on the stencil equation in which `u` is
+        written.). The default size of the time buffer when `save=None` is
+        `time_order + 1`.  To specify a different size for the time buffer, one
+        should use the syntax `save=Buffer(mysize)`.  Alternatively, if all of
+        the intermediate results are required (or, simply, to avoid using an
+        alternating buffer), an explicit value for `save` ( an integer) must be
+        provided.
+    time_dim : Dimension, optional, default=grid.time_dim
+        TimeDimension to be used in the TimeFunction.
+    staggered : Dimension or tuple of Dimension or Stagger, optional, default=None
         Define how the Function is staggered.
-    initializer : callable or any object exposing the buffer interface, optional
+    initializer : callable or any object exposing the buffer interface, default=None
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
     padding : int or tuple of ints, optional
-        .. deprecated:: shouldn't be used; padding is now automatically inserted.
-
         Allocate extra grid points to maximize data access alignment. When a tuple
         of ints, one int per Dimension should be provided.
 
     Examples
     --------
 
     Creation
@@ -1280,51 +1295,51 @@
     Derivative(f(t, x, y), x)
     >>> f.dt
     Derivative(f(t, x, y), t)
     >>> g.dt
     Derivative(g(t, x, y), t)
 
     When using the alternating buffer protocol, the size of the time dimension
-    is given by ``time_order + 1``
+    is given by `time_order + 1`
 
     >>> f.shape
     (2, 4, 4)
     >>> g.shape
     (3, 4, 4)
 
-    One can drop the alternating buffer protocol specifying a value for ``save``
+    One can drop the alternating buffer protocol specifying a value for `save`
 
     >>> h = TimeFunction(name='h', grid=grid, save=20)
     >>> h
     h(time, x, y)
     >>> h.shape
     (20, 4, 4)
 
     Notes
     -----
     The parameters must always be given as keyword arguments, since SymPy uses
-    ``*args`` to (re-)create the dimension arguments of the symbolic object.
-    If the parameter ``grid`` is provided, the values for ``shape``,
-    ``dimensions`` and ``dtype`` will be derived from it. When present, the
-    parameter ``shape`` should only define the spatial shape of the grid. The
+    `*args` to (re-)create the dimension arguments of the symbolic object.
+    If the parameter `grid` is provided, the values for `shape`,
+    `dimensions` and `dtype` will be derived from it. When present, the
+    parameter `shape` should only define the spatial shape of the grid. The
     temporal dimension will be inserted automatically as the leading dimension.
     """
 
     is_TimeFunction = True
     is_TimeDependent = True
 
     _time_position = 0
     """Position of time index among the function indices."""
 
     __rkwargs__ = Function.__rkwargs__ + ('time_order', 'save', 'time_dim')
 
     def __init_finalize__(self, *args, **kwargs):
         self.time_dim = kwargs.get('time_dim', self.dimensions[self._time_position])
         self._time_order = kwargs.get('time_order', 1)
-        super(TimeFunction, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         # Check we won't allocate too much memory for the system
         available_mem = virtual_memory().available
         if np.dtype(self.dtype).itemsize * self.size > available_mem:
             warning("Trying to allocate more memory for symbol %s " % self.name +
                     "than available on physical device, this will start swapping")
         if not isinstance(self.time_order, int):
@@ -1384,15 +1399,15 @@
                 shape.insert(cls._time_position, save)
             else:
                 raise TypeError("`save` can be None, int or Buffer, not %s" % type(save))
         elif dimensions is None:
             raise TypeError("`dimensions` required if both `grid` and "
                             "`shape` are provided")
         else:
-            shape = super(TimeFunction, cls).__shape_setup__(
+            shape = super().__shape_setup__(
                 grid=grid, shape=shape, dimensions=dimensions
             )
 
         return tuple(shape)
 
     @cached_property
     def _fd_priority(self):
@@ -1450,33 +1465,50 @@
     """
     A Function bound to a "parent" DiscreteFunction.
 
     A SubFunction hands control of argument binding and halo exchange to the
     DiscreteFunction it's bound to.
     """
 
+    __rkwargs__ = DiscreteFunction.__rkwargs__ + ('dimensions', 'shape')
+
+    def __init_finalize__(self, *args, **kwargs):
+        self._parent = kwargs.pop('parent', None)
+        super().__init_finalize__(*args, **kwargs)
+
     def __padding_setup__(self, **kwargs):
         # SubFunctions aren't expected to be used in time-consuming loops
         return tuple((0, 0) for i in range(self.ndim))
 
     def _halo_exchange(self):
         return
 
     def _arg_values(self, **kwargs):
-        if self.name in kwargs:
+        if self._parent is not None and self.parent.name not in kwargs:
+            return self._parent._arg_defaults(alias=self._parent).reduce_all()
+        elif self.name in kwargs:
             raise RuntimeError("`%s` is a SubFunction, so it can't be assigned "
                                "a value dynamically" % self.name)
+        else:
+            return self._arg_defaults(alias=self)
 
-        return self._arg_defaults(alias=self)
+    def _arg_apply(self, *args, **kwargs):
+        if self._parent is not None:
+            return self._parent._arg_apply(*args, **kwargs)
+        return super()._arg_apply(*args, **kwargs)
 
     @property
     def origin(self):
         # SubFunction have zero origin
         return DimensionTuple(*(0 for _ in range(self.ndim)), getters=self.dimensions)
 
+    @property
+    def parent(self):
+        return self._parent
+
 
 class TempFunction(DiscreteFunction):
 
     """
     Tensor symbol used to store an intermediate sub-expression extracted from
     one or more symbolic equations.
```

### Comparing `devito-4.8.3/devito/types/dimension.py` & `devito-4.8.4/devito/types/dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from collections import namedtuple
+import math
 
 import sympy
 from sympy.core.decorators import call_highest_priority
 import numpy as np
 from cached_property import cached_property
 
 from devito.data import LEFT, RIGHT
 from devito.exceptions import InvalidArgument
 from devito.logger import debug
 from devito.tools import Pickable, is_integer
 from devito.types.args import ArgProvider
 from devito.types.basic import Symbol, DataSymbol, Scalar
+from devito.types.constant import Constant
 
 __all__ = ['Dimension', 'SpaceDimension', 'TimeDimension', 'DefaultDimension',
            'CustomDimension', 'SteppingDimension', 'SubDimension', 'ConditionalDimension',
            'ModuloDimension', 'IncrDimension', 'BlockDimension', 'StencilDimension',
            'Spacing', 'dimensions']
 
 
@@ -44,15 +46,15 @@
                    |                   |
               SubDimension   ConditionalDimension
 
     Parameters
     ----------
     name : str
         Name of the dimension.
-    spacing : symbol, optional
+    spacing : symbol, optional, default=h_name
         A symbol to represent the physical spacing along this Dimension.
 
     Examples
     --------
     Dimensions are automatically created when a Grid is instantiated.
 
     >>> from devito import Grid
@@ -140,14 +142,17 @@
     def __dtype_setup__(cls, **kwargs):
         # Unlike other Symbols, Dimensions can only be integers
         return np.int32
 
     def __str__(self):
         return self.name
 
+    def _hashable_content(self):
+        return tuple(getattr(self, i) for i in self.__rargs__ + self.__rkwargs__)
+
     @property
     def spacing(self):
         """Symbol representing the physical spacing along the Dimension."""
         return self._spacing
 
     @cached_property
     def symbolic_size(self):
@@ -366,14 +371,28 @@
 
     def __new__(cls, *args, **kwargs):
         return Symbol.__new__(cls, *args, **kwargs)
 
     def __init_finalize__(self, name, spacing=None, **kwargs):
         self._spacing = spacing or Spacing(name='h_%s' % name, is_const=True)
 
+    def __eq__(self, other):
+        # Being of type Cached, Dimensions are by construction unique. But unlike
+        # Symbols, equality is much stricter -- we consider any two Dimensions
+        # equal iff they are the very same object. This has several advantages.
+        # First of all, it makes it much more difficult to trick the compiler
+        # to generate buggy code (e.g., using two different "x" Dimensions that
+        # actually represent the same iteration space). Secondly, comparison
+        # is much cheaper, since we avoid having to go through all of the
+        # __rargs__/__rkwargs__, and there can be quite a few depending on the
+        # specific Dimension type
+        return self is other
+
+    __hash__ = Symbol.__hash__
+
 
 class DefaultDimension(Dimension, DataSymbol):
 
     """
     Symbol defining an iteration space with statically-known size.
 
     Parameters
@@ -751,27 +770,27 @@
     Dimension, implemented by the compiler generating conditional "if-then" code
     within the parent Dimension's iteration space.
 
     Parameters
     ----------
     name : str
         Name of the dimension.
-    parent : Dimension, optional
+    parent : Dimension
         The parent Dimension.
-    factor : int, optional
+    factor : int, optional, default=None
         The number of iterations between two executions of the if-branch. If None
         (default), ``condition`` must be provided.
-    condition : expr-like, optional
+    condition : expr-like, optional, default=None
         An arbitrary SymPy expression, typically involving the ``parent``
         Dimension. When it evaluates to True, the if-branch is executed. If None
         (default), ``factor`` must be provided.
-    indirect : bool, optional
+    indirect : bool, optional, default=False
         If True, use `self`, rather than the parent Dimension, to
         index into arrays. A typical use case is when arrays are accessed
-        indirectly via the ``condition`` expression. Defaults to False.
+        indirectly via the ``condition`` expression.
 
     Examples
     --------
     Among the other things, ConditionalDimensions are indicated to implement
     Function subsampling. In the following example, an Operator evaluates the
     Function ``g`` and saves its content into ``f`` every ``factor=4`` iterations.
 
@@ -827,21 +846,30 @@
         # `parent=None` degenerates to a ConditionalDimension outside of
         # any iteration space
         if parent is None:
             parent = BOTTOM
 
         super().__init_finalize__(name, parent)
 
-        self._factor = factor
+        # Always make the factor symbolic to allow overrides with different factor.
+        if factor is None:
+            self._factor = None
+        elif is_integer(factor):
+            self._factor = Constant(name="%sf" % name, value=factor, dtype=np.int32)
+        elif factor.is_Constant and is_integer(factor.data):
+            self._factor = factor
+        else:
+            raise ValueError("factor must be an integer or integer Constant")
         self._condition = condition
         self._indirect = indirect
 
     @property
     def spacing(self):
-        return self.factor * self.parent.spacing
+        s = self._factor.data if self._factor is not None else 1
+        return s * self.parent.spacing
 
     @property
     def factor(self):
         return self._factor if self._factor is not None else 1
 
     @property
     def condition(self):
@@ -858,30 +886,47 @@
             retval |= self.condition.free_symbols
         try:
             retval |= self.factor.free_symbols
         except AttributeError:
             pass
         return retval
 
+    def _arg_values(self, interval, grid=None, **kwargs):
+        # Parent dimension define the interval
+        fact = self._factor.data if self._factor is not None else 1
+        toint = lambda x: math.ceil(x / fact)
+        vals = {}
+        try:
+            vals[self.min_name] = toint(kwargs.get(self.parent.min_name))
+        except (KeyError, TypeError):
+            pass
+
+        try:
+            vals[self.max_name] = toint(kwargs.get(self.parent.max_name))
+        except (KeyError, TypeError):
+            pass
+
+        return vals
+
     def _arg_defaults(self, _min=None, size=None, alias=None):
         defaults = super()._arg_defaults(_min=_min, size=size, alias=alias)
 
         # We can also add the parent's default endpoint. Note that exactly
         # `factor` endpoints are legal, so we return them all. It's then
         # up to the caller to decide which one to pick upon reduction
         dim = alias or self
         if dim._factor is None or size is None:
             return defaults
         try:
             # Is it a symbolic factor?
-            factor = defaults[dim._factor.name] = dim._factor.data
+            factor = defaults[dim._factor.name] = self._factor.data
         except AttributeError:
             factor = dim._factor
 
-        defaults[dim.parent.max_name] = range(1, factor*size - 1)
+        defaults[dim.parent.max_name] = range(0, factor*size - 1)
 
         return defaults
 
 
 # ***
 # The Dimensions below are for internal use only. They are created by the compiler
 # during the construction of an Operator
@@ -1382,34 +1427,45 @@
     spacing : expr-like, optional
         The space between two stencil points.
     """
 
     is_Stencil = True
 
     __rargs__ = BasicDimension.__rargs__ + ('_min', '_max')
+    __rkwargs__ = BasicDimension.__rkwargs__ + ('step',)
 
-    def __init_finalize__(self, name, _min, _max, spacing=None, **kwargs):
+    def __init_finalize__(self, name, _min, _max, spacing=None, step=1,
+                          **kwargs):
         self._spacing = sympy.sympify(spacing) or sympy.S.One
 
         if not is_integer(_min):
             raise ValueError("Expected integer `min` (got %s)" % _min)
         if not is_integer(_max):
             raise ValueError("Expected integer `max` (got %s)" % _max)
         if not is_integer(self._spacing):
             raise ValueError("Expected integer `spacing` (got %s)" % self._spacing)
+        if not is_integer(step):
+            raise ValueError("Expected integer `step` (got %s)" % step)
 
         self._min = _min
         self._max = _max
+        self._step = step
+
         self._size = _max - _min + 1
 
         if self._size < 1:
             raise ValueError("Expected size greater than 0 (got %s)" % self._size)
 
-    def _hashable_content(self):
-        return super()._hashable_content() + (self._min, self._max, self._spacing)
+    @property
+    def step(self):
+        return self._step
+
+    @property
+    def backward(self):
+        return self.step < 0
 
     @cached_property
     def symbolic_size(self):
         return sympy.Number(self._size)
 
     @cached_property
     def symbolic_min(self):
@@ -1419,14 +1475,17 @@
     def symbolic_max(self):
         return sympy.Number(self._max)
 
     @property
     def range(self):
         return range(self._min, self._max + 1)
 
+    def transpose(self):
+        return StencilDimension(self.name, -self._max, -self._min, step=-1)
+
     @property
     def _arg_names(self):
         return ()
 
     def _arg_defaults(self, **kwargs):
         return {}
 
@@ -1548,66 +1607,74 @@
 
 class AffineIndexAccessFunction(IndexAccessFunction):
     """
     An AffineIndexAccessFunction is the sum of three operands:
 
         * the "main" Dimension (in practice a SpaceDimension or a TimeDimension);
         * an offset (number or symbolic expression, of dtype integer).
-        * a StencilDimension;
+        * one or more StencilDimensions;
 
     Examples
     --------
     The AffineIndexAccessFunction `x + sd + 3`, with `sd in [-2, 2]`, represents
     the index access functions `[x + 1, x + 2, x + 3, x + 4, x + 5]`
     """
 
     def __new__(cls, *args, **kwargs):
+        # `args` may contain arbitrarily complicated expressions, so first of all
+        # we let SymPy simplify it, then we process the args and see if the
+        # resulting expression is indeed an AffineIndexAccessFunction
+        add = sympy.Add(*args, **kwargs)
+        if not isinstance(add, sympy.Add):
+            # E.g., reduced to a Symbol
+            return add
+
         d = 0
-        sd = 0
+        sds = []
         ofs_items = []
-        for a in args:
+        for a in add.args:
             if isinstance(a, StencilDimension):
-                if sd != 0:
-                    return sympy.Add(*args, **kwargs)
-                sd = a
+                sds.append(a)
             elif isinstance(a, Dimension):
                 d = cls._separate_dims(d, a, ofs_items)
                 if d is None:
-                    return sympy.Add(*args, **kwargs)
+                    return add
             elif isinstance(a, AffineIndexAccessFunction):
-                if sd != 0 and a.sd != 0:
-                    return sympy.Add(*args, **kwargs)
+                if sds and a.sds:
+                    return add
                 d = cls._separate_dims(d, a.d, ofs_items)
                 if d is None:
-                    return sympy.Add(*args, **kwargs)
-                sd = a.sd
+                    return add
+                sds = list(a.sds or sds)
                 ofs_items.append(a.ofs)
             else:
                 ofs_items.append(a)
 
         ofs = sympy.Add(*[i for i in ofs_items if i is not None])
         if not all(is_integer(i) or i.is_Symbol for i in ofs.free_symbols):
-            return sympy.Add(*args, **kwargs)
+            return add
+
+        sds = tuple(sds)
 
-        obj = IndexAccessFunction.__new__(cls, d, ofs, sd)
+        obj = IndexAccessFunction.__new__(cls, d, ofs, *sds)
 
         if isinstance(obj, AffineIndexAccessFunction):
             obj.d = d
             obj.ofs = ofs
-            obj.sd = sd
+            obj.sds = sds
         else:
             # E.g., SymPy simplified it to Zero or something else
             pass
 
         return obj
 
     @classmethod
     def _separate_dims(cls, d0, d1, ofs_items):
         if d0 == 0 and d1 == 0:
-            return None
+            return 0
         elif d0 == 0 and isinstance(d1, Dimension):
             return d1
         elif d1 == 0 and isinstance(d0, Dimension):
             return d0
         elif isinstance(d0, Dimension) and isinstance(d1, AbstractIncrDimension):
             # E.g., `time + x0_blk0` after skewing
             ofs_items.append(d1)
```

### Comparing `devito-4.8.3/devito/types/equation.py` & `devito-4.8.4/devito/types/equation.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     side may be any arbitrary expressions with numbers, Dimensions, Constants,
     Functions and SparseFunctions as operands.
 
     Parameters
     ----------
     lhs : Function or SparseFunction
         The left-hand side.
-    rhs : expr-like, optional
-        The right-hand side. Defaults to 0.
-    subdomain : SubDomain, optional
+    rhs : expr-like, optional, default=0
+        The right-hand side.
+    subdomain : SubDomain, optional, default=None
         To restrict the computation of the Eq to a particular sub-region in the
         computational domain.
-    coefficients : Substitutions, optional
+    coefficients : Substitutions, optional, default=None
         Can be used to replace symbolic finite difference weights with user
         defined weights.
-    implicit_dims : Dimension or list of Dimension, optional
+    implicit_dims : Dimension or list of Dimension, optional, default=None
         An ordered list of Dimensions that do not explicitly appear in either the
         left-hand side or in the right-hand side, but that should be honored when
         constructing an Operator.
 
     Examples
     --------
     >>> from devito import Grid, Function, Eq
@@ -102,15 +102,20 @@
     @property
     def _flatten(self):
         """
         Flatten vectorial/tensorial Equation into list of scalar Equations.
         """
         if self.lhs.is_Matrix:
             # Maps the Equations to retrieve the rhs from relevant lhs
-            eqs = dict(zip(as_tuple(self.lhs), as_tuple(self.rhs)))
+            try:
+                eqs = dict(zip(self.lhs, self.rhs))
+            except TypeError:
+                # Same rhs for all lhs
+                assert not self.rhs.is_Matrix
+                eqs = {i: self.rhs for i in self.lhs}
             # Get the relevant equations from the lhs structure. .values removes
             # the symmetric duplicates and off-diagonal zeros.
             lhss = self.lhs.values()
             return [self.func(l, eqs[l], subdomain=self.subdomain,
                               coefficients=self.substitutions,
                               implicit_dims=self._implicit_dims)
                     for l in lhss]
```

### Comparing `devito-4.8.3/devito/types/grid.py` & `devito-4.8.4/devito/types/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from devito.data import LEFT, RIGHT
 from devito.logger import warning
 from devito.mpi import Distributor, MPI
 from devito.tools import ReducerMap, as_tuple
 from devito.types.args import ArgProvider
 from devito.types.basic import Scalar
 from devito.types.dense import Function
+from devito.types.utils import DimensionTuple
 from devito.types.dimension import (Dimension, SpaceDimension, TimeDimension,
                                     Spacing, SteppingDimension, SubDimension)
 
 __all__ = ['Grid', 'SubDomain', 'SubDomainSet']
 
 
 GlobalLocal = namedtuple('GlobalLocal', 'glb loc')
@@ -33,15 +34,15 @@
         self._shape = as_tuple(shape)
         self._dimensions = as_tuple(dimensions)
         self._dtype = dtype
 
     @property
     def shape(self):
         """Shape of the physical domain."""
-        return self._shape
+        return DimensionTuple(*self._shape, getters=self.dimensions)
 
     @property
     def dimensions(self):
         """Spatial dimensions of the computational domain."""
         return self._dimensions
 
     @property
@@ -63,29 +64,26 @@
     A cartesian grid that encapsulates a computational domain over which
     to discretize a Function.
 
     Parameters
     ----------
     shape : tuple of ints
         Shape of the computational domain in grid points.
-    extent : tuple of floats, optional
-        Physical extent of the domain in m; defaults to a unit box of extent 1m
-        in all dimensions.
-    origin : tuple of floats, optional
-        Physical coordinate of the origin of the domain; defaults to 0.0 in all
-        dimensions.
+    extent : tuple of floats, default=unit box of extent 1m in all dimensions
+        Physical extent of the domain in m.
+    origin : tuple of floats, default=0.0 in all dimensions
+        Physical coordinate of the origin of the domain.
     dimensions : tuple of SpaceDimension, optional
         The dimensions of the computational domain encapsulated by this Grid.
     time_dimension : TimeDimension, optional
         The dimension used to define time in a `TimeFunction` created from
         this Grid.
-    dtype : data-type, optional
+    dtype : data-type, default=np.float32
         Any object that can be interpreted as a numpy data type, used as default
         data type to be inherited by all Functions created from this Grid.
-        Defaults to ``np.float32``.
     subdomains : tuple of SubDomain, optional
         If no subdomains are specified, the Grid only defines the two default
         subdomains ``interior`` and ``domain``.
     comm : MPI communicator, optional
         The set of processes over which the grid is distributed. Only relevant in
         case of MPI execution.
 
@@ -222,20 +220,21 @@
         return dict(zip(self.origin_symbols, self.origin))
 
     @property
     def origin_ioffset(self):
         """Offset index of the local (per-process) origin from the domain origin."""
         grid_origin = [min(i) for i in self.distributor.glb_numb]
         assert len(grid_origin) == len(self.spacing)
-        return tuple(grid_origin)
+        return DimensionTuple(*grid_origin, getters=self.dimensions)
 
     @property
     def origin_offset(self):
         """Physical offset of the local (per-process) origin from the domain origin."""
-        return tuple(i*h for i, h in zip(self.origin_ioffset, self.spacing))
+        return DimensionTuple(*[i*h for i, h in zip(self.origin_ioffset, self.spacing)],
+                              getters=self.dimensions)
 
     @property
     def time_dim(self):
         """Time dimension associated with this Grid."""
         return self._time_dim
 
     @property
@@ -274,15 +273,15 @@
         """Map between spacing symbols and their values for each SpaceDimension."""
         mapper = {}
         for d, s in zip(self.dimensions, self.spacing):
             if d.is_Conditional:
                 # Special case subsampling: `Grid.dimensions` -> (xb, yb, zb)`
                 # where `xb, yb, zb` are ConditionalDimensions whose parents
                 # are SpaceDimensions
-                mapper[d.root.spacing] = s/self.dtype(d.factor)
+                mapper[d.root.spacing] = s/self.dtype(d.factor.data)
             elif d.is_Space:
                 # Typical case: `Grid.dimensions` -> (x, y, z)` where `x, y, z` are
                 # the SpaceDimensions
                 mapper[d.spacing] = s
             else:
                 assert False
 
@@ -543,24 +542,35 @@
 
 class MultiSubDimension(SubDimension):
 
     """
     A special SubDimension for graceful lowering of MultiSubDomains.
     """
 
-    def __init_finalize__(self, name, parent, msd):
+    __rargs__ = ('name', 'parent', 'msd')
+    __rkwargs__ = ('thickness',)
+
+    def __init_finalize__(self, name, parent, msd, thickness=None):
         # NOTE: a MultiSubDimension stashes a reference to the originating MultiSubDomain.
         # This creates a circular pattern as the `msd` itself carries references to
         # its MultiSubDimensions. This is currently necessary because during compilation
         # we drop the MultiSubDomain early, but when the MultiSubDimensions are processed
         # we still need it to create the implicit equations. Untangling this is
         # definitely possible, but not straightforward
         self.msd = msd
 
-        lst, rst = self._symbolic_thickness(name)
+        if not thickness:
+            lst, rst = self._symbolic_thickness(name)
+        else:  # Used for rebuilding. Reuse thickness symbols rather than making new ones
+            try:
+                ((lst, _), (rst, _)) = thickness
+            except ValueError:
+                raise ValueError("Invalid thickness specification: %s does not match"
+                                 "expected format ((left_symbol, left_thickness),"
+                                 " (right_symbol, right_thickness))" % thickness)
         left = parent.symbolic_min + lst
         right = parent.symbolic_max - rst
 
         super().__init_finalize__(name, parent, left, right, ((lst, 0), (rst, 0)), False)
 
     def __hash__(self):
         # There is no possibility for two MultiSubDimensions to ever hash the same, since
```

### Comparing `devito-4.8.3/devito/types/lazy.py` & `devito-4.8.4/devito/types/lazy.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/object.py` & `devito-4.8.4/devito/types/object.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         return self.name
 
     __str__ = __repr__
 
     def _sympystr(self, printer):
         return str(self)
 
+    _ccode = _sympystr
+
     def _hashable_content(self):
         return (self.name, self.dtype)
 
     @property
     def dtype(self):
         return self._dtype
 
@@ -69,18 +71,14 @@
         return self.name
 
     @property
     def _C_ctype(self):
         return self.dtype
 
     @property
-    def base(self):
-        return self
-
-    @property
     def function(self):
         return self
 
     # Pickling support
     __reduce_ex__ = Pickable.__reduce_ex__
 
 
@@ -89,15 +87,15 @@
     """
     Object with derived type defined in Python.
     """
 
     is_Object = True
 
     def __init__(self, name, dtype, value=None):
-        super(Object, self).__init__(name, dtype)
+        super().__init__(name, dtype)
         self.value = value
 
     __hash__ = Uncached.__hash__
 
     @property
     def _mem_external(self):
         return True
@@ -135,15 +133,15 @@
     """
 
     __rargs__ = ('name', 'pname', 'pfields')
 
     def __init__(self, name, pname, pfields, value=None):
         dtype = CtypesFactory.generate(pname, pfields)
         value = self.__value_setup__(dtype, value)
-        super(CompositeObject, self).__init__(name, dtype, value)
+        super().__init__(name, dtype, value)
 
     def __value_setup__(self, dtype, value):
         return value or byref(dtype._type_())
 
     @property
     def pfields(self):
         return tuple(self.dtype._type_._fields_)
@@ -166,34 +164,58 @@
     is_LocalObject = True
 
     dtype = None
     """
     LocalObjects encode their dtype as a class attribute.
     """
 
+    default_initvalue = None
+    """
+    The initial value may or may not be a class-level attribute. In the latter
+    case, it is passed to the constructor.
+    """
+
     __rargs__ = ('name',)
-    __rkwargs__ = ('cargs', 'liveness')
+    __rkwargs__ = ('cargs', 'initvalue', 'liveness', 'is_global')
 
-    def __init__(self, name, cargs=None, **kwargs):
+    def __init__(self, name, cargs=None, initvalue=None, liveness='lazy',
+                 is_global=False, **kwargs):
         self.name = name
         self.cargs = as_tuple(cargs)
+        self.initvalue = initvalue or self.default_initvalue
+
+        assert liveness in ['eager', 'lazy']
+        self._liveness = liveness
 
-        self._liveness = kwargs.get('liveness', 'lazy')
-        assert self._liveness in ['eager', 'lazy']
+        self._is_global = is_global
 
     def _hashable_content(self):
-        return super()._hashable_content() + self.cargs + (self.liveness,)
+        return (super()._hashable_content() +
+                self.cargs +
+                (self.initvalue, self.liveness, self.is_global))
 
     @property
     def liveness(self):
         return self._liveness
 
     @property
+    def is_global(self):
+        return self._is_global
+
+    @property
     def free_symbols(self):
-        return super().free_symbols | set(self.cargs)
+        ret = set()
+        ret.update(super().free_symbols)
+        for i in self.cargs:
+            try:
+                ret.update(i.free_symbols)
+            except AttributeError:
+                # E.g., pure integers
+                pass
+        return ret
 
     @property
     def _C_init(self):
         """
         A symbolic initializer for the LocalObject, injected in the generated code.
 
         Notes
@@ -209,14 +231,25 @@
 
         Notes
         -----
         To be overridden by subclasses, ignored otherwise.
         """
         return None
 
+    _C_modifier = None
+    """
+    A modifier added to the LocalObject's C declaration when the object appears
+    in a function signature. For example, a subclass might define `_C_modifier = '&'`
+    to impose pass-by-reference semantics.
+    """
+
     @property
     def _mem_internal_eager(self):
         return self._liveness == 'eager'
 
     @property
     def _mem_internal_lazy(self):
         return self._liveness == 'lazy'
+
+    @property
+    def _mem_global(self):
+        return self._is_global
```

### Comparing `devito-4.8.3/devito/types/parallel.py` & `devito-4.8.4/devito/types/parallel.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 for the generation of threaded code (e.g., special symbols representing
 the number of threads in a parallel region, objects such as locks to
 implement thread synchronization, etc) and device code (e.g., a special symbol
 identifying a device attached to a node).
 """
 
 import os
-from ctypes import c_void_p
+from ctypes import POINTER, c_void_p
 
 from cached_property import cached_property
 import numpy as np
 
 from devito.exceptions import InvalidArgument
 from devito.parameters import configuration
 from devito.tools import as_list, as_tuple, is_integer
 from devito.types.array import Array, ArrayObject
 from devito.types.basic import Scalar, Symbol
 from devito.types.dimension import CustomDimension
-from devito.types.misc import VolatileInt
+from devito.types.misc import Fence, VolatileInt
 
 __all__ = ['NThreads', 'NThreadsNested', 'NThreadsNonaffine', 'NThreadsBase',
-           'DeviceID', 'ThreadID', 'Lock', 'PThreadArray', 'SharedData',
-           'NPThreads', 'DeviceRM', 'QueueID', 'Barrier']
+           'DeviceID', 'ThreadID', 'Lock', 'ThreadArray', 'PThreadArray',
+           'SharedData', 'NPThreads', 'DeviceRM', 'QueueID', 'Barrier', 'TBArray']
 
 
 class NThreadsBase(Scalar):
 
     is_Input = True
     is_PerfKnob = True
 
@@ -107,14 +107,17 @@
     @property
     def nthreads(self):
         return self.symbolic_size
 
 
 class ThreadArray(ArrayObject):
 
+    # Not a performance-sensitive object
+    _data_alignment = False
+
     @classmethod
     def __indices_setup__(cls, **kwargs):
         try:
             return as_tuple(kwargs['dimensions']), as_tuple(kwargs['dimensions'])
         except KeyError:
             nthreads = kwargs['npthreads']
             dim = CustomDimension(name='wi', symbolic_size=nthreads)
@@ -122,28 +125,28 @@
 
     @property
     def dim(self):
         assert len(self.dimensions) == 1
         return self.dimensions[0]
 
     @property
+    def npthreads(self):
+        return self.dim.symbolic_size
+
+    @property
     def index(self):
         if self.size == 1:
             return 0
         else:
             return self.dim
 
-    @cached_property
-    def symbolic_base(self):
-        return Symbol(name=self.name, dtype=None)
-
 
 class PThreadArray(ThreadArray):
 
-    dtype = type('pthread_t', (c_void_p,), {})
+    dtype = POINTER(type('pthread_t', (c_void_p,), {}))
 
     @classmethod
     def __dtype_setup__(cls, **kwargs):
         return cls.dtype
 
 
 class SharedData(ThreadArray):
@@ -200,14 +203,17 @@
     Note that this is generalisable to K values rather than just four -- should
     one need to define critical sections with multiple privilege values -- but
     we don't need it here.
     """
 
     is_volatile = True
 
+    # Not a performance-sensitive object
+    _data_alignment = False
+
     def __init_finalize__(self, *args, **kwargs):
         kwargs.setdefault('scope', 'stack')
 
         dimensions = as_tuple(kwargs.get('dimensions'))
         if len(dimensions) != 1:
             raise ValueError("Expected exactly one Dimension, got `%d`" % len(dimensions))
         d, = dimensions
@@ -283,14 +289,26 @@
 
     def __new__(cls, *args, **kwargs):
         kwargs['name'] = 'qid'
         kwargs.setdefault('is_const', True)
         return super().__new__(cls, *args, **kwargs)
 
 
-class Barrier(object):
+class Barrier(Fence):
 
     """
-    Mixin class for symbolic objects representing synchronization barriers.
+    A generic synchronization barrier for threads or processes.
     """
 
     pass
+
+
+class TBArray(Array):
+
+    """
+    An Array used for performance optimization within a thread block.
+    """
+
+    def __init_finalize__(self, *args, **kwargs):
+        kwargs['liveness'] = 'eager'
+
+        super().__init_finalize__(*args, **kwargs)
```

### Comparing `devito-4.8.3/devito/types/relational.py` & `devito-4.8.4/devito/types/relational.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/devito/types/sparse.py` & `devito-4.8.4/devito/types/sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import sympy
 import numpy as np
 from cached_property import cached_property
 
 from devito.finite_differences import generate_fd_shortcuts
 from devito.mpi import MPI, SparseDistributor
-from devito.operations import LinearInterpolator, PrecomputedInterpolator
+from devito.operations import (LinearInterpolator, PrecomputedInterpolator,
+                               SincInterpolator)
 from devito.symbolics import indexify, retrieve_function_carriers
 from devito.tools import (ReducerMap, as_tuple, flatten, prod, filter_ordered,
                           is_integer, dtype_to_mpidtype)
 from devito.types.dense import DiscreteFunction, SubFunction
 from devito.types.dimension import (Dimension, ConditionalDimension, DefaultDimension,
                                     DynamicDimension)
 from devito.types.dimension import dimensions as mkdims
@@ -25,14 +26,18 @@
 from devito.types.utils import IgnoreDimSort
 
 
 __all__ = ['SparseFunction', 'SparseTimeFunction', 'PrecomputedSparseFunction',
            'PrecomputedSparseTimeFunction', 'MatrixSparseTimeFunction']
 
 
+_interpolators = {'linear': LinearInterpolator, 'sinc': SincInterpolator}
+_default_radius = {'linear': 1, 'sinc': 4}
+
+
 class AbstractSparseFunction(DiscreteFunction):
 
     """
     An abstract class to define behaviours common to all sparse functions.
     """
 
     _sparse_position = -1
@@ -43,15 +48,15 @@
 
     _sub_functions = ()
     """SubFunctions encapsulated within this AbstractSparseFunction."""
 
     __rkwargs__ = DiscreteFunction.__rkwargs__ + ('npoint_global', 'space_order')
 
     def __init_finalize__(self, *args, **kwargs):
-        super(AbstractSparseFunction, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
         self._npoint = kwargs.get('npoint', kwargs.get('npoint_global'))
         self._space_order = kwargs.get('space_order', 0)
 
         # Dynamically add derivative short-cuts
         self._fd = self.__fd_setup__()
 
     @classmethod
@@ -68,36 +73,49 @@
     @classmethod
     def __shape_setup__(cls, **kwargs):
         grid = kwargs.get('grid')
         # A Grid must have been provided
         if grid is None:
             raise TypeError('Need `grid` argument')
         shape = kwargs.get('shape')
+        dimensions = kwargs.get('dimensions')
         npoint = kwargs.get('npoint', kwargs.get('npoint_global'))
+        glb_npoint = SparseDistributor.decompose(npoint, grid.distributor)
         if shape is None:
-            glb_npoint = SparseDistributor.decompose(npoint, grid.distributor)
-            shape = (glb_npoint[grid.distributor.myrank],)
-        return shape
+            loc_shape = (glb_npoint[grid.distributor.myrank],)
+        else:
+            loc_shape = []
+            assert len(dimensions) == len(shape)
+            for i, (d, s) in enumerate(zip(dimensions, shape)):
+                if i == cls._sparse_position:
+                    loc_shape.append(glb_npoint[grid.distributor.myrank])
+                elif d in grid.dimensions:
+                    loc_shape.append(grid.dimension_map[d].loc)
+                else:
+                    loc_shape.append(s)
+        return tuple(loc_shape)
 
     def __fd_setup__(self):
         """
         Dynamically add derivative short-cuts.
         """
         return generate_fd_shortcuts(self.dimensions, self.space_order)
 
     def __distributor_setup__(self, **kwargs):
         """
         A `SparseDistributor` handles the SparseFunction decomposition based on
         physical ownership, and allows to convert between global and local indices.
         """
-        return SparseDistributor(
-            kwargs.get('npoint', kwargs.get('npoint_global')),
-            self._sparse_dim,
-            kwargs['grid'].distributor
-        )
+        distributor = kwargs.get('distributor')
+        if distributor is None:
+            distributor = SparseDistributor(
+                kwargs.get('npoint', kwargs.get('npoint_global')),
+                self._sparse_dim, kwargs['grid'].distributor)
+
+        return distributor
 
     def __subfunc_setup__(self, key, suffix, dtype=None):
         # Shape and dimensions from args
         name = '%s_%s' % (self.name, suffix)
 
         if key is not None and not isinstance(key, SubFunction):
             key = np.array(key)
@@ -138,29 +156,33 @@
                 dtype = dtype or np.int32
             else:
                 dtype = dtype or self.dtype
 
         sf = SubFunction(
             name=name, dtype=dtype, dimensions=dimensions,
             shape=shape, space_order=0, initializer=key, alias=self.alias,
-            distributor=self._distributor
+            distributor=self._distributor, parent=self
         )
 
         if self.npoint == 0:
             # This is a corner case -- we might get here, for example, when
             # running with MPI and some processes get 0-size arrays after
             # domain decomposition. We "touch" the data anyway to avoid the
             # case ``self._data is None``
             sf.data
 
         return sf
 
     @property
+    def sparse_position(self):
+        return self._sparse_position
+
+    @property
     def _sparse_dim(self):
-        return self.dimensions[self._sparse_position]
+        return self.dimensions[self.sparse_position]
 
     @property
     def _mpitype(self):
         return dtype_to_mpidtype(self.dtype)
 
     @property
     def _smpitype(self):
@@ -713,30 +735,34 @@
         Name of the symbol.
     npoint : int
         Number of sparse points.
     grid : Grid
         The computational domain from which the sparse points are sampled.
     coordinates : np.ndarray, optional
         The coordinates of each sparse point.
-    space_order : int, optional
-        Discretisation order for space derivatives. Defaults to 0.
-    shape : tuple of ints, optional
-        Shape of the object. Defaults to ``(npoint,)``.
+    space_order : int, optional, default=0
+        Discretisation order for space derivatives.
+    shape : tuple of ints, optional, default=(npoint,)
+        Shape of the object.
     dimensions : tuple of Dimension, optional
         Dimensions associated with the object. Only necessary if the SparseFunction
         defines a multi-dimensional tensor.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to ``np.float32``.
-    initializer : callable or any object exposing the buffer interface, optional
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
+    initializer : callable or any object exposing the buffer interface, default=None
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
+    interpolation: String, optional, default='linear'
+        The interpolation type to be used by the SparseFunction. Supported types
+        are 'linear' and 'sinc'.
+    r: int, optional, default=1 for 'linear', 4 for 'sinc'
+        The radius of the interpolation operators provided by the SparseFunction.
 
     Examples
     --------
 
     Creation
 
     >>> from devito import Grid, SparseFunction
@@ -779,42 +805,65 @@
     A "gather" operation, executed before returning control to user-land,
     updates the physically owned sparse points in ``self.data`` by collecting
     the values computed during ``op.apply`` from different MPI ranks.
     """
 
     is_SparseFunction = True
 
-    _radius = 1
     """The radius of the stencil operators provided by the SparseFunction."""
 
     _sub_functions = ('coordinates',)
 
-    __rkwargs__ = AbstractSparseFunction.__rkwargs__ + ('coordinates',)
+    __rkwargs__ = AbstractSparseFunction.__rkwargs__ + ('coordinates', 'interpolation')
 
     def __init_finalize__(self, *args, **kwargs):
+        # Interpolation method
+        self.__interp_setup__(**kwargs)
+
+        # Initialization
         super().__init_finalize__(*args, **kwargs)
-        self.interpolator = LinearInterpolator(self)
 
         # Set up sparse point coordinates
         coordinates = kwargs.get('coordinates', kwargs.get('coordinates_data'))
         self._coordinates = self.__subfunc_setup__(coordinates, 'coords')
         self._dist_origin = {self._coordinates: self.grid.origin_offset}
 
+    def __interp_setup__(self, interpolation='linear', r=None, **kwargs):
+        self.interpolation = interpolation
+        self.interpolator = _interpolators[interpolation](self)
+        self._radius = r or _default_radius[interpolation]
+        if interpolation == 'sinc':
+            if self._radius < 2:
+                raise ValueError("'sinc' interpolator requires a radius of at least 2")
+            elif self._radius > 10:
+                raise ValueError("'sinc' interpolator requires a radius of at most 10")
+        elif interpolation == 'linear' and self._radius != 1:
+            self._radius = 1
+
     @cached_property
     def _coordinate_symbols(self):
         """Symbol representing the coordinate values in each Dimension."""
         d_dim = self.coordinates.dimensions[1]
         return tuple([self.coordinates._subs(d_dim, i)
                       for i in range(self.grid.dim)])
 
     @cached_property
     def _decomposition(self):
         mapper = {self._sparse_dim: self._distributor.decomposition[self._sparse_dim]}
         return tuple(mapper.get(d) for d in self.dimensions)
 
+    def _arg_defaults(self, alias=None):
+        defaults = super()._arg_defaults(alias=alias)
+
+        key = alias or self
+        coords = defaults.get(key.coordinates.name, key.coordinates.data)
+        defaults.update(key.interpolator._arg_defaults(coords=coords,
+                                                       sfunc=key))
+        return defaults
+
 
 class SparseTimeFunction(AbstractSparseTimeFunction, SparseFunction):
     """
     Tensor symbol representing a space- and time-varying sparse array in symbolic
     equations.
 
     Like SparseFunction, SparseTimeFunction carries multi-dimensional data that
@@ -832,27 +881,26 @@
         Number of sparse points.
     nt : int
         Number of timesteps along the time Dimension.
     grid : Grid
         The computational domain from which the sparse points are sampled.
     coordinates : np.ndarray, optional
         The coordinates of each sparse point.
-    space_order : int, optional
-        Discretisation order for space derivatives. Defaults to 0.
-    time_order : int, optional
-        Discretisation order for time derivatives. Defaults to 1.
-    shape : tuple of ints, optional
-        Shape of the object. Defaults to ``(nt, npoint)``.
+    space_order : int, optional, default=0
+        Discretisation order for space derivatives.
+    time_order : int, optional, default=1
+        Discretisation order for time derivatives.
+    shape : tuple of ints, optional, default=(nt, npoint)
+        Shape of the object.
     dimensions : tuple of Dimension, optional
         Dimensions associated with the object. Only necessary if the SparseFunction
         defines a multi-dimensional tensor.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to ``np.float32``.
-    initializer : callable or any object exposing the buffer interface, optional
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
+    initializer : callable or any object exposing the buffer interface, default=None
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
 
     Examples
@@ -892,15 +940,15 @@
     """
 
     is_SparseTimeFunction = True
 
     __rkwargs__ = tuple(filter_ordered(AbstractSparseTimeFunction.__rkwargs__ +
                                        SparseFunction.__rkwargs__))
 
-    def interpolate(self, expr, u_t=None, p_t=None, increment=False):
+    def interpolate(self, expr, u_t=None, p_t=None, increment=False, implicit_dims=None):
         """
         Generate equations interpolating an arbitrary expression into ``self``.
 
         Parameters
         ----------
         expr : expr-like
             Input expression to interpolate.
@@ -917,15 +965,16 @@
             time = self.grid.time_dim
             t = self.grid.stepping_dim
             expr = expr.subs({time: u_t, t: u_t})
 
         if p_t is not None:
             subs = {self.time_dim: p_t}
 
-        return super().interpolate(expr, increment=increment, self_subs=subs)
+        return super().interpolate(expr, increment=increment, self_subs=subs,
+                                   implicit_dims=implicit_dims)
 
     def inject(self, field, expr, u_t=None, p_t=None, implicit_dims=None):
         """
         Generate equations injecting an arbitrary expression into a field.
 
         Parameters
         ----------
@@ -981,24 +1030,23 @@
         (3D) gridpoints that each sparse point will be interpolated to. The
         coefficient is split across the n Dimensions such that the contribution
         of the point (i, j, k) will be multiplied by
         `interp_coeffs[..., i]*interp_coeffs[...,j]*interp_coeffs[...,k]`.
         So for `r=6`, we will store 18 coefficients per sparse point (instead of
         potentially 216).  Must be a three-dimensional array of shape
         `(npoint, grid.ndim, r)`.
-    space_order : int, optional
-        Discretisation order for space derivatives. Defaults to 0.
-    shape : tuple of ints, optional
-        Shape of the object. Defaults to `(npoint,)`.
+    space_order : int, optional, default=0
+        Discretisation order for space derivatives.
+    shape : tuple of ints, optional, default=(npoint,)
+        Shape of the object.
     dimensions : tuple of Dimension, optional
         Dimensions associated with the object. Only necessary if the SparseFunction
         defines a multi-dimensional tensor.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to `np.float32`.
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
     initializer : callable or any object exposing the buffer interface, optional
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
 
@@ -1102,15 +1150,15 @@
         mathematically equivalent expanded form `coord/spacing -
         origin/spacing`. This particular form is problematic when a sparse
         point is in close proximity of the grid origin, since due to a larger
         machine precision error it may cause a +-1 error in the computation of
         the position. We mitigate this problem by computing the positions
         individually (hence the need for a position map).
         """
-        if self.gridpoints is not None:
+        if self.gridpoints_data is not None:
             ddim = self.gridpoints.dimensions[-1]
             return OrderedDict((self.gridpoints._subs(ddim, di), p)
                                for (di, p) in zip(range(self.grid.dim),
                                                   self._pos_symbols))
         else:
             return super()._position_map
 
@@ -1146,27 +1194,26 @@
         (3D) gridpoints that each sparse point will be interpolated to. The
         coefficient is split across the n Dimensions such that the contribution
         of the point (i, j, k) will be multiplied by
         `interp_coeffs[..., i]*interp_coeffs[...,j]*interp_coeffs[...,k]`.
         So for `r=6`, we will store 18 coefficients per sparse point (instead of
         potentially 216).  Must be a three-dimensional array of shape
         `(npoint, grid.ndim, r)`.
-    space_order : int, optional
-        Discretisation order for space derivatives. Defaults to 0.
-    time_order : int, optional
-        Discretisation order for time derivatives. Default to 1.
-    shape : tuple of ints, optional
-        Shape of the object. Defaults to `(npoint,)`.
+    space_order : int, optional, default=0
+        Discretisation order for space derivatives.
+    time_order : int, optional, default=1
+        Discretisation order for time derivatives.
+    shape : tuple of ints, optional, default=(npoint,)
+        Shape of the object.
     dimensions : tuple of Dimension, optional
         Dimensions associated with the object. Only necessary if the SparseFunction
         defines a multi-dimensional tensor.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to `np.float32`.
-    initializer : callable or any object exposing the buffer interface, optional
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
+    initializer : callable or any object exposing the buffer interface, default=None
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
 
     Notes
```

### Comparing `devito-4.8.3/devito/types/tensor.py` & `devito-4.8.4/devito/types/tensor.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,49 +25,45 @@
     ----------
     name : str
         Name of the symbol.
     grid : Grid, optional
         Carries shape, dimensions, and dtype of the TensorFunction. When grid is not
         provided, shape and dimensions must be given. For MPI execution, a
         Grid is compulsory.
-    space_order : int or 3-tuple of ints, optional
-        Discretisation order for space derivatives. Defaults to 1. ``space_order`` also
+    space_order : int or 3-tuple of ints, optional, default=1
+        Discretisation order for space derivatives. ``space_order`` also
         impacts the number of points available around a generic point of interest.  By
         default, ``space_order`` points are available on both sides of a generic point of
         interest, including those nearby the grid boundary. Sometimes, fewer points
         suffice; in other scenarios, more points are necessary. In such cases, instead of
         an integer, one can pass a 3-tuple ``(o, lp, rp)`` indicating the discretization
         order (``o``) as well as the number of points on the left (``lp``) and right
         (``rp``) sides of a generic point of interest.
     shape : tuple of ints, optional
         Shape of the domain region in grid points. Only necessary if ``grid`` isn't given.
     dimensions : tuple of Dimension, optional
         Dimensions associated with the object. Only necessary if ``grid`` isn't given.
-    dtype : data-type, optional
-        Any object that can be interpreted as a numpy data type. Defaults
-        to ``np.float32``.
+    dtype : data-type, optional, default=np.float32
+        Any object that can be interpreted as a numpy data type.
     staggered : Dimension or tuple of Dimension or Stagger, optional
-        Define how the TensorFunction is staggered.
+        Staggering of each component, needs to have the size of the tensor. Defaults
+        to the Dimensions.
     initializer : callable or any object exposing the buffer interface, optional
         Data initializer. If a callable is provided, data is allocated lazily.
     allocator : MemoryAllocator, optional
         Controller for memory allocation. To be used, for example, when one wants
         to take advantage of the memory hierarchy in a NUMA architecture. Refer to
         `default_allocator.__doc__` for more information.
     padding : int or tuple of ints, optional
-        .. deprecated:: shouldn't be used; padding is now automatically inserted.
         Allocate extra grid points to maximize data access alignment. When a tuple
         of ints, one int per Dimension should be provided.
-    symmetric : bool, optional
-        Whether the tensor is symmetric or not. Defaults to True.
-    diagonal : Bool, optional
-        Whether the tensor is diagonal or not. Defaults to False.
-    staggered: tuple of Dimension, optional
-        Staggering of each component, needs to have the size of the tensor. Defaults
-        to the Dimensions.
+    symmetric : bool, optional, default=True
+        Whether the tensor is symmetric or not.
+    diagonal : Bool, optional, default=False
+        Whether the tensor is diagonal or not.
     """
 
     _is_TimeDependent = False
 
     _sub_type = Function
 
     _class_priority = 10
@@ -125,14 +121,16 @@
         """
         Try calling a dynamically created FD shortcut.
 
         Notes
         -----
         This method acts as a fallback for __getattribute__
         """
+        if name in ['_sympystr', '_pretty', '_latex']:
+            return super().__getattr__(self, name)
         try:
             return self.applyfunc(lambda x: x if x == 0 else getattr(x, name))
         except:
             raise AttributeError("%r object has no attribute %r" % (self.__class__, name))
 
     def _eval_at(self, func):
         """
@@ -169,52 +167,94 @@
     @property
     def is_diagonal(self):
         """Whether the tensor is diagonal."""
         return np.all([self[i, j] == 0 for j in range(self.cols)
                        for i in range(self.rows) if i != j])
 
     def _evaluate(self, **kwargs):
-        return self.applyfunc(lambda x: getattr(x, 'evaluate', x))
+        def _do_evaluate(x):
+            try:
+                expand = kwargs.get('expand', True)
+                return x._evaluate(expand=expand)
+            except AttributeError:
+                return x
+        return self.applyfunc(_do_evaluate)
 
     def values(self):
         if self.is_diagonal:
             return [self[i, i] for i in range(self.shape[0])]
         elif self.is_symmetric:
-            val = super(TensorFunction, self).values()
+            val = super().values()
             return list(OrderedDict.fromkeys(val))
         else:
-            return super(TensorFunction, self).values()
+            return super().values()
 
-    def div(self, shift=None):
+    def div(self, shift=None, order=None, method='FD'):
         """
         Divergence of the TensorFunction (is a VectorFunction).
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
         """
         comps = []
         func = vec_func(self)
         ndim = len(self.space_dimensions)
         shift_x0 = make_shift_x0(shift, (ndim, ndim))
+        order = order or self.space_order
         for i in range(len(self.space_dimensions)):
             comps.append(sum([getattr(self[j, i], 'd%s' % d.name)
-                              (x0=shift_x0(shift, d, i, j))
+                              (x0=shift_x0(shift, d, i, j), fd_order=order,
+                               method=method)
                               for j, d in enumerate(self.space_dimensions)]))
         return func._new(comps)
 
     @property
     def laplace(self):
         """
         Laplacian of the TensorFunction.
         """
+        return self.laplacian()
+
+    def laplacian(self, shift=None, order=None):
+        """
+        Laplacian of the TensorFunction with shifted derivatives and custom
+        FD order.
+
+        Each second derivative is left-right (i.e D^T D with D the first derivative ):
+        `(self.dx(x0=dim+shift*dim.spacing,
+                  fd_order=order)).dx(x0=dim-shift*dim.spacing, fd_order=order)`
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        """
         comps = []
         func = vec_func(self)
-        for j, d in enumerate(self.space_dimensions):
+        order = order or self.space_order
+        ndim = len(self.space_dimensions)
+        shift_x0 = make_shift_x0(shift, (ndim, ndim))
+        for j in range(ndim):
             comps.append(sum([getattr(self[j, i], 'd%s2' % d.name)
+                              (x0=shift_x0(shift, d, j, i), fd_order=order)
                               for i, d in enumerate(self.space_dimensions)]))
         return func._new(comps)
 
-    def grad(self, shift=None):
+    def grad(self, shift=None, order=None):
         raise AttributeError("Gradient of a second order tensor not supported")
 
     def new_from_mat(self, mat):
         func = tens_func(self)
         return func._new(self.rows, self.cols, mat)
 
     def classof_prod(self, other, mat):
@@ -272,57 +312,121 @@
     # Custom repr and str
     def __str__(self):
         st = ''.join([' %-2s,' % c for c in self])[1:-1]
         return "Vector(%s)" % st
 
     __repr__ = __str__
 
-    def div(self, shift=None):
+    def div(self, shift=None, order=None, method='FD'):
         """
         Divergence of the VectorFunction, creates the divergence Function.
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
         """
         shift_x0 = make_shift_x0(shift, (len(self.space_dimensions),))
-        return sum([getattr(self[i], 'd%s' % d.name)(x0=shift_x0(shift, d, None, i))
+        order = order or self.space_order
+        return sum([getattr(self[i], 'd%s' % d.name)(x0=shift_x0(shift, d, None, i),
+                                                     fd_order=order, method=method)
                     for i, d in enumerate(self.space_dimensions)])
 
     @property
     def laplace(self):
         """
         Laplacian of the VectorFunction, creates the Laplacian VectorFunction.
         """
+        return self.laplacian()
+
+    def laplacian(self, shift=None, order=None):
+        """
+        Laplacian of the VectorFunction, creates the Laplacian VectorFunction.
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        """
         func = vec_func(self)
-        comps = [sum([getattr(s, 'd%s2' % d.name) for d in self.space_dimensions])
+        shift_x0 = make_shift_x0(shift, (len(self.space_dimensions),))
+        order = order or self.space_order
+        comps = [sum([getattr(s, 'd%s2' % d.name)(x0=shift_x0(shift, d, None, i),
+                                                  fd_order=order)
+                      for i, d in enumerate(self.space_dimensions)])
                  for s in self]
         return func._new(comps)
 
-    @property
-    def curl(self):
+    def curl(self, shift=None, order=None, method='FD'):
         """
         Gradient of the (3D) VectorFunction, creates the curl VectorFunction.
-        """
 
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
+        """
         if len(self.space_dimensions) != 3:
             raise AttributeError("Curl only supported for 3D VectorFunction")
         # The curl of a VectorFunction is a VectorFunction
-        derivs = ['d%s' % d.name for d in self.space_dimensions]
-        comp1 = getattr(self[2], derivs[1]) - getattr(self[1], derivs[2])
-        comp2 = getattr(self[0], derivs[2]) - getattr(self[2], derivs[0])
-        comp3 = getattr(self[1], derivs[0]) - getattr(self[0], derivs[1])
-
+        dims = self.space_dimensions
+        derivs = ['d%s' % d.name for d in dims]
+        shift_x0 = make_shift_x0(shift, (len(dims), len(dims)))
+        order = order or self.space_order
+        comp1 = (getattr(self[2], derivs[1])(x0=shift_x0(shift, dims[1], 2, 1),
+                                             fd_order=order, method=method) -
+                 getattr(self[1], derivs[2])(x0=shift_x0(shift, dims[2], 1, 2),
+                                             fd_order=order, method=method))
+        comp2 = (getattr(self[0], derivs[2])(x0=shift_x0(shift, dims[2], 0, 2),
+                                             fd_order=order, method=method) -
+                 getattr(self[2], derivs[0])(x0=shift_x0(shift, dims[0], 2, 0),
+                                             fd_order=order, method=method))
+        comp3 = (getattr(self[1], derivs[0])(x0=shift_x0(shift, dims[0], 1, 0),
+                                             fd_order=order, method=method) -
+                 getattr(self[0], derivs[1])(x0=shift_x0(shift, dims[1], 0, 1),
+                                             fd_order=order, method=method))
         func = vec_func(self)
         return func._new(3, 1, [comp1, comp2, comp3])
 
-    def grad(self, shift=None):
+    def grad(self, shift=None, order=None, method='FD'):
         """
         Gradient of the VectorFunction, creates the gradient TensorFunction.
+
+        Parameters
+        ----------
+        shift: Number, optional, default=None
+            Shift for the center point of the derivative in number of gridpoints
+        order: int, optional, default=None
+            Discretization order for the finite differences.
+            Uses `func.space_order` when not specified
+        method: str, optional, default='FD'
+            Discretization method. Options are 'FD' (default) and
+            'RSFD' (rotated staggered grid finite-difference).
         """
         func = tens_func(self)
         ndim = len(self.space_dimensions)
         shift_x0 = make_shift_x0(shift, (ndim, ndim))
-        comps = [[getattr(f, 'd%s' % d.name)(x0=shift_x0(shift, d, i, j))
+        order = order or self.space_order
+        comps = [[getattr(f, 'd%s' % d.name)(x0=shift_x0(shift, d, i, j),
+                                             fd_order=order, method=method)
                   for j, d in enumerate(self.space_dimensions)]
                  for i, f in enumerate(self)]
         return func._new(comps)
 
     def outer(self, other):
         comps = [[self[i] * other[j] for i in range(self.cols)] for j in range(self.cols)]
         func = tens_func(self, other)
```

### Comparing `devito-4.8.3/devito/types/utils.py` & `devito-4.8.4/devito/types/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __all__ = ['Buffer', 'DimensionTuple', 'NODE', 'CELL', 'IgnoreDimSort',
            'HierarchyLayer', 'HostLayer']
 
 
 class Buffer(Tag):
 
     def __init__(self, value):
-        super(Buffer, self).__init__('Buffer', value)
+        super().__init__('Buffer', value)
 
 
 class Stagger(Tag):
     """Stagger region."""
     pass
 
 NODE = Stagger('node')  # noqa
```

### Comparing `devito-4.8.3/devito.egg-info/SOURCES.txt` & `devito-4.8.4/devito.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 devito/finite_differences/__init__.py
 devito/finite_differences/coefficients.py
 devito/finite_differences/derivative.py
 devito/finite_differences/differentiable.py
 devito/finite_differences/elementary.py
 devito/finite_differences/finite_difference.py
 devito/finite_differences/operators.py
+devito/finite_differences/rsfd.py
 devito/finite_differences/tools.py
 devito/ir/__init__.py
 devito/ir/clusters/__init__.py
 devito/ir/clusters/algorithms.py
 devito/ir/clusters/analysis.py
 devito/ir/clusters/cluster.py
 devito/ir/clusters/visitors.py
@@ -110,14 +111,15 @@
 devito/passes/clusters/utils.py
 devito/passes/equations/__init__.py
 devito/passes/equations/linearity.py
 devito/passes/iet/__init__.py
 devito/passes/iet/asynchrony.py
 devito/passes/iet/definitions.py
 devito/passes/iet/engine.py
+devito/passes/iet/errors.py
 devito/passes/iet/instrument.py
 devito/passes/iet/langbase.py
 devito/passes/iet/linearization.py
 devito/passes/iet/misc.py
 devito/passes/iet/mpi.py
 devito/passes/iet/orchestration.py
 devito/passes/iet/parpragma.py
@@ -202,8 +204,56 @@
 examples/seismic/viscoacoustic/operators.py
 examples/seismic/viscoacoustic/viscoacoustic_example.py
 examples/seismic/viscoacoustic/wavesolver.py
 examples/seismic/viscoelastic/__init__.py
 examples/seismic/viscoelastic/operators.py
 examples/seismic/viscoelastic/viscoelastic_example.py
 examples/seismic/viscoelastic/wavesolver.py
-examples/userapi/__init__.py
+examples/userapi/__init__.py
+tests/test_adjoint.py
+tests/test_autotuner.py
+tests/test_benchmark.py
+tests/test_buffering.py
+tests/test_builtins.py
+tests/test_caching.py
+tests/test_checkpointing.py
+tests/test_cinterface.py
+tests/test_constant.py
+tests/test_data.py
+tests/test_derivatives.py
+tests/test_differentiable.py
+tests/test_dimension.py
+tests/test_dle.py
+tests/test_docstrings.py
+tests/test_dse.py
+tests/test_environment.py
+tests/test_error_checking.py
+tests/test_fission.py
+tests/test_gpu_common.py
+tests/test_gpu_openacc.py
+tests/test_gpu_openmp.py
+tests/test_gradient.py
+tests/test_iet.py
+tests/test_interpolation.py
+tests/test_ir.py
+tests/test_linearize.py
+tests/test_lower_clusters.py
+tests/test_lower_exprs.py
+tests/test_mpi.py
+tests/test_operator.py
+tests/test_pickle.py
+tests/test_resample.py
+tests/test_roundoff.py
+tests/test_save.py
+tests/test_skewing.py
+tests/test_sparse.py
+tests/test_staggered_utils.py
+tests/test_subdomains.py
+tests/test_symbolic_coefficients.py
+tests/test_symbolics.py
+tests/test_tensors.py
+tests/test_threading.py
+tests/test_timestepping.py
+tests/test_tools.py
+tests/test_tti.py
+tests/test_unexpansion.py
+tests/test_visitors.py
```

### Comparing `devito-4.8.3/devito.egg-info/requires.txt` & `devito-4.8.4/devito.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 cached-property
 psutil<6.0,>=5.1.0
 py-cpuinfo<10
 cgen>=2020.1
 codepy>=2019.1
 click<9.0
 multidict
-anytree<=2.10.0,>=2.4.3
+anytree<=2.12.1,>=2.4.3
 cloudpickle
 
 [ python_version >= "3.8"]
 pooch
 
 [extras]
 matplotlib
 pandas
-pyrevolve==2.2.3
+pyrevolve==2.2.4
 scipy
 distributed
 
 [mpi]
 mpi4py<3.1.6
-ipyparallel<8.7
+ipyparallel<8.9
 
 [nvidia]
 cupy-cuda12x
 dask-cuda
 jupyterlab>=3
 jupyterlab-nvdashboard
 dask_labextension
 fsspec
 
 [tests]
-pytest<8.0,>=7.2
+pytest<9.0,>=7.2
 pytest-runner
 pytest-cov
 codecov
 flake8>=2.1.0
 nbval
 scipy
```

### Comparing `devito-4.8.3/examples/cfd/example_diffusion.py` & `devito-4.8.4/examples/cfd/example_diffusion.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/cfd/tools.py` & `devito-4.8.4/examples/cfd/tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/misc/linalg.py` & `devito-4.8.4/examples/misc/linalg.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/performance/utils.py` & `devito-4.8.4/examples/performance/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/acoustic/acoustic_example.py` & `devito-4.8.4/examples/seismic/acoustic/acoustic_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                    tn=500., kernel='OT2', space_order=4, nbl=10,
                    preset='layers-isotropic', fs=False, **kwargs):
     model = demo_model(preset, space_order=space_order, shape=shape, nbl=nbl,
                        dtype=kwargs.pop('dtype', np.float32), spacing=spacing,
                        fs=fs, **kwargs)
 
     # Source and receiver geometries
-    geometry = setup_geometry(model, tn)
+    geometry = setup_geometry(model, tn, **kwargs)
 
     # Create solver object to provide relevant operators
     solver = AcousticWaveSolver(model, geometry, kernel=kernel,
                                 space_order=space_order, **kwargs)
     return solver
 
 
@@ -56,29 +56,34 @@
 
     info("Applying Adjoint")
     solver.adjoint(rec, autotune=autotune)
     info("Applying Born")
     solver.jacobian(dm, autotune=autotune)
     info("Applying Gradient")
     solver.jacobian_adjoint(rec, u, autotune=autotune, checkpointing=checkpointing)
-    return summary.gflopss, summary.oi, summary.timings, [rec, u.data]
+    return summary.gflopss, summary.oi, summary.timings, [rec, u.data._local]
 
 
 @pytest.mark.parametrize('shape', [(101,), (51, 51), (16, 16, 16)])
 @pytest.mark.parametrize('k', ['OT2', 'OT4'])
-def test_isoacoustic_stability(shape, k):
+@pytest.mark.parametrize('interp', ['linear', 'sinc'])
+def test_isoacoustic_stability(shape, k, interp):
     spacing = tuple([20]*len(shape))
-    _, _, _, [rec, _] = run(shape=shape, spacing=spacing, tn=20000.0, nbl=0, kernel=k)
+    _, _, _, [rec, _] = run(shape=shape, spacing=spacing, tn=20000.0, nbl=0, kernel=k,
+                            interpolation=interp)
     assert np.isfinite(norm(rec))
 
 
-@pytest.mark.parametrize('fs, normrec, dtype', [(True, 369.955, np.float32),
-                                                (False, 459.1678, np.float64)])
-def test_isoacoustic(fs, normrec, dtype):
-    _, _, _, [rec, _] = run(fs=fs, dtype=dtype)
+@pytest.mark.parametrize('fs, normrec, dtype, interp', [
+    (True, 369.955, np.float32, 'linear'),
+    (False, 459.1678, np.float64, 'linear'),
+    (True, 402.216, np.float32, 'sinc'),
+    (False, 509.0681, np.float64, 'sinc')])
+def test_isoacoustic(fs, normrec, dtype, interp):
+    _, _, _, [rec, _] = run(fs=fs, dtype=dtype, interpolation=interp)
     assert np.isclose(norm(rec), normrec, rtol=1e-3, atol=0)
 
 
 if __name__ == "__main__":
     description = ("Example script for a set of acoustic operators.")
     parser = seismic_args(description)
     parser.add_argument('--fs', dest='fs', default=False, action='store_true',
@@ -94,8 +99,8 @@
     spacing = tuple(ndim * [15.0])
     tn = args.tn if args.tn > 0 else (750. if ndim < 3 else 1250.)
 
     preset = 'constant-isotropic' if args.constant else 'layers-isotropic'
     run(shape=shape, spacing=spacing, nbl=args.nbl, tn=tn, fs=args.fs,
         space_order=args.space_order, preset=preset, kernel=args.kernel,
         autotune=args.autotune, opt=args.opt, full_run=args.full,
-        checkpointing=args.checkpointing, dtype=args.dtype)
+        checkpointing=args.checkpointing, dtype=args.dtype, interpolation=args.interp)
```

### Comparing `devito-4.8.3/examples/seismic/acoustic/operators.py` & `devito-4.8.4/examples/seismic/acoustic/operators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 from devito import Eq, Operator, Function, TimeFunction, Inc, solve, sign
-from devito.symbolics import retrieve_functions, INT
-from examples.seismic import PointSource, Receiver
+from devito.symbolics import retrieve_functions, INT, retrieve_derivatives
 
 
 def freesurface(model, eq):
     """
     Generate the stencil that mirrors the field as a free surface modeling for
     the acoustic wave equation.
 
     Parameters
     ----------
     model : Model
         Physical model.
     eq : Eq
         Time-stepping stencil (time update) to mirror at the freesurface.
     """
-    lhs, rhs = eq.evaluate.args
+    lhs, rhs = eq.args
     # Get vertical dimension and corresponding subdimension
-    zfs = model.grid.subdomains['fsdomain'].dimensions[-1]
+    fsdomain = model.grid.subdomains['fsdomain']
+    zfs = fsdomain.dimensions[-1]
     z = zfs.parent
 
-    # Functions present in the stencil
-    funcs = retrieve_functions(rhs)
+    # Retrieve vertical derivatives
+    dzs = {d for d in retrieve_derivatives(rhs) if z in d.dims}
+    # Remove inner duplicate
+    dzs = dzs - {d for D in dzs for d in retrieve_derivatives(D.expr) if z in d.dims}
+    dzs = {d: d._eval_at(lhs).evaluate for d in dzs}
+
+    # Finally get functions for evaluated derivatives
+    funcs = {f for f in retrieve_functions(dzs.values())}
+
     mapper = {}
     # Antisymmetric mirror at negative indices
     # TODO: Make a proper "mirror_indices" tool function
     for f in funcs:
         zind = f.indices[-1]
         if (zind - z).as_coeff_Mul()[0] < 0:
             s = sign(zind.subs({z: zfs, z.spacing: 1}))
             mapper.update({f: s * f.subs({zind: INT(abs(zind))})})
-    return Eq(lhs, rhs.subs(mapper), subdomain=model.grid.subdomains['fsdomain'])
+
+    # Mapper for vertical derivatives
+    dzmapper = {d: v.subs(mapper) for d, v in dzs.items()}
+
+    fs_eq = [eq.func(lhs, rhs.subs(dzmapper), subdomain=fsdomain)]
+    fs_eq.append(eq.func(lhs._subs(z, 0), 0, subdomain=fsdomain))
+
+    return fs_eq
 
 
 def laplacian(field, model, kernel):
     """
     Spatial discretization for the isotropic acoustic wave equation. For a 4th
     order in time formulation, the 4th order time derivative is replaced by a
     double laplacian:
@@ -115,19 +129,16 @@
     """
     m = model.m
 
     # Create symbols for forward wavefield, source and receivers
     u = TimeFunction(name='u', grid=model.grid,
                      save=geometry.nt if save else None,
                      time_order=2, space_order=space_order)
-    src = PointSource(name='src', grid=geometry.grid, time_range=geometry.time_axis,
-                      npoint=geometry.nsrc)
-
-    rec = Receiver(name='rec', grid=geometry.grid, time_range=geometry.time_axis,
-                   npoint=geometry.nrec)
+    src = geometry.src
+    rec = geometry.rec
 
     s = model.grid.stepping_dim.spacing
     eqn = iso_stencil(u, model, kernel)
 
     # Construct expression to inject source values
     src_term = src.inject(field=u.forward, expr=src * s**2 / m)
 
@@ -156,18 +167,16 @@
     kernel : str, optional
         Type of discretization, 'OT2' or 'OT4'.
     """
     m = model.m
 
     v = TimeFunction(name='v', grid=model.grid, save=None,
                      time_order=2, space_order=space_order)
-    srca = PointSource(name='srca', grid=model.grid, time_range=geometry.time_axis,
-                       npoint=geometry.nsrc)
-    rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
-                   npoint=geometry.nrec)
+    srca = geometry.new_src(name='srca', src_type=None)
+    rec = geometry.rec
 
     s = model.grid.stepping_dim.spacing
     eqn = iso_stencil(v, model, kernel, forward=False)
 
     # Construct expression to inject receiver values
     receivers = rec.inject(field=v.backward, expr=rec * s**2 / m)
 
@@ -202,16 +211,15 @@
 
     # Gradient symbol and wavefield symbols
     grad = Function(name='grad', grid=model.grid)
     u = TimeFunction(name='u', grid=model.grid, save=geometry.nt if save
                      else None, time_order=2, space_order=space_order)
     v = TimeFunction(name='v', grid=model.grid, save=None,
                      time_order=2, space_order=space_order)
-    rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
-                   npoint=geometry.nrec)
+    rec = geometry.rec
 
     s = model.grid.stepping_dim.spacing
     eqn = iso_stencil(v, model, kernel, forward=False)
 
     if kernel == 'OT2':
         gradient_update = Inc(grad, - u * v.dt2)
     elif kernel == 'OT4':
@@ -240,19 +248,16 @@
         Space discretization order.
     kernel : str, optional
         Type of discretization, centered or shifted.
     """
     m = model.m
 
     # Create source and receiver symbols
-    src = Receiver(name='src', grid=model.grid, time_range=geometry.time_axis,
-                   npoint=geometry.nsrc)
-
-    rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
-                   npoint=geometry.nrec)
+    src = geometry.src
+    rec = geometry.rec
 
     # Create wavefields and a dm field
     u = TimeFunction(name="u", grid=model.grid, save=None,
                      time_order=2, space_order=space_order)
     U = TimeFunction(name="U", grid=model.grid, save=None,
                      time_order=2, space_order=space_order)
     dm = Function(name="dm", grid=model.grid, space_order=0)
```

### Comparing `devito-4.8.3/examples/seismic/acoustic/wavesolver.py` & `devito-4.8.4/examples/seismic/acoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/elastic/elastic_example.py` & `devito-4.8.4/examples/seismic/elastic/elastic_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             [rec1, rec2, v, tau])
 
 
 @pytest.mark.parametrize("dtype", [np.float32, np.float64])
 def test_elastic(dtype):
     _, _, _, [rec1, rec2, v, tau] = run(dtype=dtype)
     assert np.isclose(norm(rec1), 19.25636, atol=1e-3, rtol=0)
-    assert np.isclose(norm(rec2), 0.627606, atol=1e-3, rtol=0)
+    assert np.isclose(norm(rec2), 0.6276, atol=1e-3, rtol=0)
 
 
 @pytest.mark.parametrize('shape', [(51, 51), (16, 16, 16)])
 def test_elastic_stability(shape):
     spacing = tuple([20]*len(shape))
     _, _, _, [rec1, rec2, v, tau] = run(shape=shape, spacing=spacing, tn=20000.0, nbl=0)
     assert np.isfinite(norm(rec1))
```

### Comparing `devito-4.8.3/examples/seismic/elastic/operators.py` & `devito-4.8.4/examples/seismic/elastic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/elastic/wavesolver.py` & `devito-4.8.4/examples/seismic/elastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/model.py` & `devito-4.8.4/examples/seismic/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 class PhysicalDomain(SubDomain):
 
     name = 'physdomain'
 
     def __init__(self, so, fs=False):
-        super(PhysicalDomain, self).__init__()
+        super().__init__()
         self.so = so
         self.fs = fs
 
     def define(self, dimensions):
         map_d = {d: d for d in dimensions}
         if self.fs:
             map_d[dimensions[-1]] = ('middle', self.so, 0)
@@ -69,15 +69,15 @@
 
 
 class FSDomain(SubDomain):
 
     name = 'fsdomain'
 
     def __init__(self, so):
-        super(FSDomain, self).__init__()
+        super().__init__()
         self.size = so
 
     def define(self, dimensions):
         """
         Definition of the upper section of the domain for wrapped indices FS.
         """
 
@@ -163,15 +163,15 @@
         """
         Return all set physical parameters and update to input values if provided
         """
         known = [getattr(self, i) for i in self.physical_parameters]
         return {i.name: kwargs.get(i.name, i) or i for i in known}
 
     def _gen_phys_param(self, field, name, space_order, is_param=True,
-                        default_value=0):
+                        default_value=0, **kwargs):
         if field is None:
             return default_value
         if isinstance(field, np.ndarray):
             function = Function(name=name, grid=self.grid, space_order=space_order,
                                 parameter=is_param)
             initialize_function(function, field, self.padsizes)
         else:
@@ -266,16 +266,16 @@
         S-wave attenuation.
     """
     _known_parameters = ['vp', 'damp', 'vs', 'b', 'epsilon', 'delta',
                          'theta', 'phi', 'qp', 'qs', 'lam', 'mu']
 
     def __init__(self, origin, spacing, shape, space_order, vp, nbl=20, fs=False,
                  dtype=np.float32, subdomains=(), bcs="mask", grid=None, **kwargs):
-        super(SeismicModel, self).__init__(origin, spacing, shape, space_order, nbl,
-                                           dtype, subdomains, grid=grid, bcs=bcs, fs=fs)
+        super().__init__(origin, spacing, shape, space_order, nbl,
+                         dtype, subdomains, grid=grid, bcs=bcs, fs=fs)
 
         # Initialize physics
         self._initialize_physics(vp, space_order, **kwargs)
 
         # User provided dt
         self._dt = kwargs.get('dt')
         # Some wave equation need a rescaled dt that can't be infered from the model
```

### Comparing `devito-4.8.3/examples/seismic/plotting.py` & `devito-4.8.4/examples/seismic/plotting.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/preset_models.py` & `devito-4.8.4/examples/seismic/preset_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 import numpy as np
 
 from examples.seismic.model import SeismicModel
 
 __all__ = ['demo_model']
 
 
+def Gardners(vp, normalize=True):
+    """
+    Gardner's relation for vp in km/s
+    """
+    b = 1 / (0.31 * (1e3*vp)**0.25)
+    if normalize:
+        b[vp < 1.51] = 1.0
+    return b
+
+
 def demo_model(preset, **kwargs):
     """
     Utility function to create preset `Model` objects for
     demonstration and testing purposes. The particular presets are ::
 
     * `constant-isotropic` : Constant velocity (1.5 km/sec) isotropic model
     * `constant-tti` : Constant anisotropic model. Velocity is 1.5 km/sec and
@@ -45,14 +55,15 @@
     spacing = kwargs.pop('spacing', tuple([10. for _ in shape]))
     origin = kwargs.pop('origin', tuple([0. for _ in shape]))
     nbl = kwargs.pop('nbl', 10)
     dtype = kwargs.pop('dtype', np.float32)
     vp = kwargs.pop('vp', 1.5)
     nlayers = kwargs.pop('nlayers', 3)
     fs = kwargs.pop('fs', False)
+    density = kwargs.pop('density', False)
 
     if preset.lower() in ['constant-elastic']:
         # A constant single-layer model in a 2D or 3D domain
         # with velocity 1.5 km/s.
         vs = 0.5 * vp
         b = 1.0
 
@@ -72,15 +83,16 @@
                             qs=qs, b=b, origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl,
                             **kwargs)
 
     if preset.lower() in ['constant-isotropic']:
         # A constant single-layer model in a 2D or 3D domain
         # with velocity 1.5 km/s.
-
+        if density:
+            kwargs['b'] = 1
         return SeismicModel(space_order=space_order, vp=vp, origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl, fs=fs, **kwargs)
 
     if preset.lower() in ['constant-viscoacoustic']:
         # A constant single-layer model in a 2D or 3D domain
         # with velocity 1.5 km/s.
         qp = kwargs.pop('qp', 100.)
@@ -95,15 +107,16 @@
         # with velocity 1.5 km/s.
         epsilon = .3
         delta = .2
         theta = .7
         phi = None
         if len(shape) > 2 and preset.lower() not in ['constant-tti-noazimuth']:
             phi = .35
-
+        if density:
+            kwargs['b'] = 1
         return SeismicModel(space_order=space_order, vp=vp, origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl, epsilon=epsilon,
                             delta=delta, theta=theta, phi=phi, bcs="damp", **kwargs)
 
     elif preset.lower() in ['layers-isotropic']:
         # A n-layers model in a 2D or 3D domain with two different
         # velocities split across the height dimension:
@@ -115,14 +128,17 @@
         # Define a velocity profile in km/s
         v = np.empty(shape, dtype=dtype)
         v[:] = vp_top  # Top velocity (background)
         vp_i = np.linspace(vp_top, vp_bottom, nlayers)
         for i in range(1, nlayers):
             v[..., i*int(shape[-1] / nlayers):] = vp_i[i]  # Bottom velocity
 
+        if density:
+            kwargs['b'] = Gardners(v)
+
         return SeismicModel(space_order=space_order, vp=v, origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl, bcs="damp",
                             fs=fs, **kwargs)
 
     elif preset.lower() in ['layers-elastic']:
         # A n-layers model in a 2D or 3D domain with two different
         # velocities split across the height dimension:
@@ -135,16 +151,15 @@
         v = np.empty(shape, dtype=dtype)
         v[:] = vp_top  # Top velocity (background)
         vp_i = np.linspace(vp_top, vp_bottom, nlayers)
         for i in range(1, nlayers):
             v[..., i*int(shape[-1] / nlayers):] = vp_i[i]  # Bottom velocity
 
         vs = 0.5 * v[:]
-        b = 1 / (0.31 * (1e3*v)**0.25)
-        b[v < 1.51] = 1.0
+        b = Gardners(v)
         vs[v < 1.51] = 0.0
 
         return SeismicModel(space_order=space_order, vp=v, vs=vs, b=b,
                             origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl, **kwargs)
 
     elif preset.lower() in ['layers-viscoelastic', 'twolayer-viscoelastic',
@@ -203,20 +218,23 @@
         # Define a velocity profile in km/s
         v = np.empty(shape, dtype=dtype)
         v[:] = vp_top  # Top velocity (background)
         vp_i = np.linspace(vp_top, vp_bottom, nlayers)
         for i in range(1, nlayers):
             v[..., i*int(shape[-1] / nlayers):] = vp_i[i]  # Bottom velocity
 
-        epsilon = .3*(v - 1.5)
-        delta = .2*(v - 1.5)
-        theta = .5*(v - 1.5)
+        epsilon = .1*(v - vp_top)
+        delta = .05*(v - vp_top)
+        theta = .5*(v - vp_top)
         phi = None
         if len(shape) > 2 and preset.lower() not in ['layers-tti-noazimuth']:
-            phi = .25*(v - 1.5)
+            phi = .25*(v - vp_top)
+
+        if density:
+            kwargs['b'] = Gardners(v)
 
         model = SeismicModel(space_order=space_order, vp=v, origin=origin, shape=shape,
                              dtype=dtype, spacing=spacing, nbl=nbl, epsilon=epsilon,
                              delta=delta, theta=theta, phi=phi, bcs="damp",
                              fs=fs, **kwargs)
 
         if kwargs.get('smooth', False):
@@ -241,14 +259,17 @@
         v = np.empty(shape, dtype=dtype)
         v[:] = vp_background
 
         a, b = shape[0] / 2, shape[1] / 2
         y, x = np.ogrid[-a:shape[0]-a, -b:shape[1]-b]
         v[x*x + y*y <= r*r] = vp
 
+        if density:
+            kwargs['b'] = Gardners(v)
+
         return SeismicModel(space_order=space_order, vp=v, origin=origin, shape=shape,
                             dtype=dtype, spacing=spacing, nbl=nbl, bcs="damp",
                             fs=fs, **kwargs)
 
     elif preset.lower() in ['marmousi-isotropic', 'marmousi2d-isotropic']:
         shape = (1601, 401)
         spacing = (7.5, 7.5)
@@ -343,15 +364,15 @@
         vp[:] = vp_top  # Top velocity (background)
         vp_i = np.linspace(vp_top, vp_bottom, nlayers)
         for i in range(1, nlayers):
             vp[..., i*int(shape[-1] / nlayers):] = vp_i[i]  # Bottom velocity
 
         qp[:] = 3.516*((vp[:]*1000.)**2.2)*10**(-6)  # Li's empirical formula
 
-        b = 1 / (0.31*(vp[:]*1000.)**0.25)  # Gardner's relation
+        b = Gardners(vp, normalize=False)
 
         return SeismicModel(space_order=space_order, vp=vp, qp=qp, b=b, nbl=nbl,
                             dtype=dtype, origin=origin, shape=shape,
                             spacing=spacing, **kwargs)
 
     else:
         raise ValueError("Unknown model preset name")
```

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/example_iso.py` & `devito-4.8.4/examples/seismic/self_adjoint/example_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/operators.py` & `devito-4.8.4/examples/seismic/self_adjoint/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/test_utils.py` & `devito-4.8.4/examples/seismic/self_adjoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/test_wavesolver_iso.py` & `devito-4.8.4/examples/seismic/self_adjoint/test_wavesolver_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/utils.py` & `devito-4.8.4/examples/seismic/self_adjoint/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/self_adjoint/wavesolver.py` & `devito-4.8.4/examples/seismic/self_adjoint/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/source.py` & `devito-4.8.4/examples/seismic/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         return args, kwargs
 
     def __init_finalize__(self, *args, **kwargs):
         time_range = kwargs.pop('time_range')
         data = kwargs.pop('data', None)
 
         kwargs.setdefault('time_order', 2)
-        super(PointSource, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         self._time_range = time_range._rebuild()
 
         # If provided, copy initial data into the allocated buffer
         if data is not None:
             self.data[:] = data
 
@@ -201,18 +201,18 @@
 
     __rkwargs__ = PointSource.__rkwargs__ + ['f0', 'a', 't0']
 
     @classmethod
     def __args_setup__(cls, *args, **kwargs):
         kwargs.setdefault('npoint', 1)
 
-        return super(WaveletSource, cls).__args_setup__(*args, **kwargs)
+        return super().__args_setup__(*args, **kwargs)
 
     def __init_finalize__(self, *args, **kwargs):
-        super(WaveletSource, self).__init_finalize__(*args, **kwargs)
+        super().__init_finalize__(*args, **kwargs)
 
         self.f0 = kwargs.get('f0')
         self.a = kwargs.get('a')
         self.t0 = kwargs.get('t0')
 
         if not self.alias:
             for p in range(kwargs['npoint']):
```

### Comparing `devito-4.8.3/examples/seismic/test_seismic_utils.py` & `devito-4.8.4/examples/seismic/test_seismic_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/tti/operators.py` & `devito-4.8.4/examples/seismic/tti/operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from devito import (Eq, Operator, Function, TimeFunction, NODE, Inc, solve,
-                    cos, sin, sqrt)
+                    cos, sin, sqrt, div, grad)
 from examples.seismic import PointSource, Receiver
 from examples.seismic.acoustic.operators import freesurface
 
 
 def second_order_stencil(model, u, v, H0, Hz, qu, qv, forward=True):
     """
     Creates the stencil corresponding to the second order TTI wave equation
@@ -53,145 +53,109 @@
 
         cosphi = cos(phi)
         sinphi = sin(phi)
         return costheta, sintheta, cosphi, sinphi
     return costheta, sintheta
 
 
-def Gzz_centered(model, field, costheta, sintheta, cosphi, sinphi, space_order):
+def Gzz_centered(model, field):
     """
     3D rotated second order derivative in the direction z.
 
     Parameters
     ----------
+    model : Model
+        Physical parameters model structure.
     field : Function
         Input for which the derivative is computed.
-    costheta : Function or float
-        Cosine of the tilt angle.
-    sintheta : Function or float
-        Sine of the tilt angle.
-    cosphi : Function or float
-        Cosine of the azymuth angle.
-    sinphi : Function or float
-        Sine of the azymuth angle.
-    space_order : int
-        Space discretization order.
 
     Returns
     -------
     Rotated second order derivative w.r.t. z.
     """
-    order1 = space_order // 2
+    b = getattr(model, 'b', 1)
+    costheta, sintheta, cosphi, sinphi = trig_func(model)
+    order1 = field.space_order // 2
     Gz = -(sintheta * cosphi * field.dx(fd_order=order1) +
            sintheta * sinphi * field.dy(fd_order=order1) +
            costheta * field.dz(fd_order=order1))
 
-    Gzz = (Gz * costheta).dz(fd_order=order1).T
+    Gzz = (b * Gz * costheta).dz(fd_order=order1).T
     # Add rotated derivative if angles are not zero. If angles are
     # zeros then `0*Gz = 0` and doesn't have any `.dy` ....
     if sintheta != 0:
-        Gzz += (Gz * sintheta * cosphi).dx(fd_order=order1).T
+        Gzz += (b * Gz * sintheta * cosphi).dx(fd_order=order1).T
     if sinphi != 0:
-        Gzz += (Gz * sintheta * sinphi).dy(fd_order=order1).T
+        Gzz += (b * Gz * sintheta * sinphi).dy(fd_order=order1).T
 
     return Gzz
 
 
-def Gzz_centered_2d(model, field, costheta, sintheta, space_order):
+def Gzz_centered_2d(model, field):
     """
     2D rotated second order derivative in the direction z.
 
     Parameters
     ----------
+    model : Model
+        Physical parameters model structure.
     field : Function
         Input for which the derivative is computed.
-    costheta : Function or float
-        Cosine of the tilt angle.
-    sintheta : Function or float
-        Sine of the tilt angle.
-    space_order : int
-        Space discretization order.
 
     Returns
     -------
     Rotated second order derivative w.r.t. z.
     """
-    order1 = space_order // 2
+    costheta, sintheta = trig_func(model)
+    order1 = field.space_order // 2
+    b = getattr(model, 'b', 1)
     Gz = -(sintheta * field.dx(fd_order=order1) +
            costheta * field.dy(fd_order=order1))
-    Gzz = (Gz * costheta).dy(fd_order=order1).T
+    Gzz = (b * Gz * costheta).dy(fd_order=order1).T
 
     # Add rotated derivative if angles are not zero. If angles are
     # zeros then `0*Gz = 0` and doesn't have any `.dy` ....
     if sintheta != 0:
-        Gzz += (Gz * sintheta).dx(fd_order=order1).T
+        Gzz += (b * Gz * sintheta).dx(fd_order=order1).T
     return Gzz
 
 
 # Centered case produces directly Gxx + Gyy
-def Gxxyy_centered(model, field, costheta, sintheta, cosphi, sinphi, space_order):
+def Gh_centered(model, field):
     """
     Sum of the 3D rotated second order derivative in the direction x and y.
     As the Laplacian is rotation invariant, it is computed as the conventional
     Laplacian minus the second order rotated second order derivative in the direction z
     Gxx + Gyy = field.laplace - Gzz
 
     Parameters
     ----------
+    model : Model
+        Physical parameters model structure.
     field : Function
         Input field.
-    costheta : Function or float
-        Cosine of the tilt angle.
-    sintheta : Function or float
-        Sine of the tilt angle.
-    cosphi : Function or float
-        Cosine of the azymuth angle.
-    sinphi : Function or float
-        Sine of the azymuth angle.
-    space_order : int
-        Space discretization order.
 
     Returns
     -------
     Sum of the 3D rotated second order derivative in the direction x and y.
     """
-    Gzz = Gzz_centered(model, field, costheta, sintheta, cosphi, sinphi, space_order)
-    return field.laplace - Gzz
-
-
-def Gxx_centered_2d(model, field, costheta, sintheta, space_order):
-    """
-    2D rotated second order derivative in the direction x.
-    As the Laplacian is rotation invariant, it is computed as the conventional
-    Laplacian minus the second order rotated second order derivative in the direction z
-    Gxx = field.laplace - Gzz
-
-    Parameters
-    ----------
-    field : TimeFunction
-        Input field.
-    costheta : Function or float
-        Cosine of the tilt angle.
-    sintheta : Function or float
-        Sine of the tilt angle.
-    cosphi : Function or float
-        Cosine of the azymuth angle.
-    sinphi : Function or float
-        Sine of the azymuth angle.
-    space_order : int
-        Space discretization order.
-
-    Returns
-    -------
-    Sum of the 3D rotated second order derivative in the direction x.
-    """
-    return field.laplace - Gzz_centered_2d(model, field, costheta, sintheta, space_order)
+    if model.dim == 3:
+        Gzz = Gzz_centered(model, field)
+    else:
+        Gzz = Gzz_centered_2d(model, field)
+    b = getattr(model, 'b', None)
+    if b is not None:
+        so = field.space_order // 2
+        lap = div(b * grad(field, shift=.5, order=so), shift=-.5, order=so)
+    else:
+        lap = field.laplace
+    return lap - Gzz
 
 
-def kernel_centered_2d(model, u, v, space_order, **kwargs):
+def kernel_centered(model, u, v, **kwargs):
     """
     TTI finite difference kernel. The equation solved is:
 
     u.dt2 = H0
     v.dt2 = Hz
 
     where H0 and Hz are defined as:
@@ -225,145 +189,76 @@
     Returns
     -------
     u and v component of the rotated Laplacian in 2D.
     """
     # Forward or backward
     forward = kwargs.get('forward', True)
 
-    # Tilt and azymuth setup
-    costheta, sintheta = trig_func(model)
-
     delta, epsilon = model.delta, model.epsilon
     epsilon = 1 + 2*epsilon
     delta = sqrt(1 + 2*delta)
 
     # Get source
     qu = kwargs.get('qu', 0)
     qv = kwargs.get('qv', 0)
 
-    if forward:
-        Gxx = Gxx_centered_2d(model, u, costheta, sintheta, space_order)
-        Gzz = Gzz_centered_2d(model, v, costheta, sintheta, space_order)
-        H0 = epsilon*Gxx + delta*Gzz
-        Hz = delta*Gxx + Gzz
-        return second_order_stencil(model, u, v, H0, Hz, qu, qv)
-    else:
-        H0 = Gxx_centered_2d(model, (epsilon*u + delta*v), costheta,
-                             sintheta, space_order)
-        Hz = Gzz_centered_2d(model, (delta*u + v), costheta, sintheta, space_order)
-        return second_order_stencil(model, u, v, H0, Hz, qu, qv, forward=forward)
-
-
-def kernel_centered_3d(model, u, v, space_order, **kwargs):
-    """
-    TTI finite difference kernel. The equation solved is:
-
-    u.dt2 = H0
-    v.dt2 = Hz
-
-    where H0 and Hz are defined as:
-    H0 = (1+2 *epsilon) (Gxx(u)+Gyy(u)) + sqrt(1+ 2*delta) Gzz(v)
-    Hz = sqrt(1+ 2*delta) (Gxx(u)+Gyy(u)) +  Gzz(v)
-
-    and
-
-    H0 = (Gxx+Gyy)((1+2 *epsilon)*u + sqrt(1+ 2*delta)*v)
-    Hz = Gzz(sqrt(1+ 2*delta)*u + v)
-
-    for the forward and adjoint cases, respectively. Epsilon and delta are the Thomsen
-    parameters. This function computes H0 and Hz.
-
-    References:
-        * Zhang, Yu, Houzhu Zhang, and Guanquan Zhang. "A stable TTI reverse
-          time migration and its implementation." Geophysics 76.3 (2011): WA3-WA11.
-        * Louboutin, Mathias, Philipp Witte, and Felix J. Herrmann. "Effects of
-          wrong adjoints for RTM in TTI media." SEG Technical Program Expanded
-          Abstracts 2018. Society of Exploration Geophysicists, 2018. 331-335.
-
-    Parameters
-    ----------
-    u : TimeFunction
-        First TTI field.
-    v : TimeFunction
-        Second TTI field.
-    space_order : int
-        Space discretization order.
-
-    Returns
-    -------
-    u and v component of the rotated Laplacian in 3D.
-    """
-    # Forward or backward
-    forward = kwargs.get('forward', True)
-
-    costheta, sintheta, cosphi, sinphi = trig_func(model)
-
-    delta, epsilon = model.delta, model.epsilon
-    epsilon = 1 + 2*epsilon
-    delta = sqrt(1 + 2*delta)
-
-    # Get source
-    qu = kwargs.get('qu', 0)
-    qv = kwargs.get('qv', 0)
+    Gzz = Gzz_centered_2d if model.dim == 2 else Gzz_centered
 
     if forward:
-        Gxx = Gxxyy_centered(model, u, costheta, sintheta, cosphi, sinphi, space_order)
-        Gzz = Gzz_centered(model, v, costheta, sintheta, cosphi, sinphi, space_order)
+        Gxx = Gh_centered(model, u)
+        Gzz = Gzz(model, v)
         H0 = epsilon*Gxx + delta*Gzz
         Hz = delta*Gxx + Gzz
         return second_order_stencil(model, u, v, H0, Hz, qu, qv)
     else:
-        H0 = Gxxyy_centered(model, (epsilon*u + delta*v), costheta, sintheta,
-                            cosphi, sinphi, space_order)
-        Hz = Gzz_centered(model, (delta*u + v), costheta, sintheta, cosphi,
-                          sinphi, space_order)
+        H0 = Gh_centered(model, (epsilon*u + delta*v))
+        Hz = Gzz(model, (delta*u + v))
         return second_order_stencil(model, u, v, H0, Hz, qu, qv, forward=forward)
 
 
 def particle_velocity_fields(model, space_order):
     """
     Initialize particle velocity fields for staggered TTI.
     """
     if model.grid.dim == 2:
         x, z = model.space_dimensions
         stagg_x = x
         stagg_z = z
-        x, z = model.grid.dimensions
         # Create symbols for forward wavefield, source and receivers
         vx = TimeFunction(name='vx', grid=model.grid, staggered=stagg_x,
                           time_order=1, space_order=space_order)
         vz = TimeFunction(name='vz', grid=model.grid, staggered=stagg_z,
                           time_order=1, space_order=space_order)
         vy = None
     elif model.grid.dim == 3:
         x, y, z = model.space_dimensions
         stagg_x = x
         stagg_y = y
         stagg_z = z
-        x, y, z = model.grid.dimensions
         # Create symbols for forward wavefield, source and receivers
         vx = TimeFunction(name='vx', grid=model.grid, staggered=stagg_x,
                           time_order=1, space_order=space_order)
         vy = TimeFunction(name='vy', grid=model.grid, staggered=stagg_y,
                           time_order=1, space_order=space_order)
         vz = TimeFunction(name='vz', grid=model.grid, staggered=stagg_z,
                           time_order=1, space_order=space_order)
 
     return vx, vz, vy
 
 
-def kernel_staggered_2d(model, u, v, space_order, **kwargs):
+def kernel_staggered_2d(model, u, v, **kwargs):
     """
     TTI finite difference. The equation solved is:
 
     vx.dt = - u.dx
     vz.dt = - v.dx
     m * v.dt = - sqrt(1 + 2 delta) vx.dx - vz.dz + Fh
     m * u.dt = - (1 + 2 epsilon) vx.dx - sqrt(1 + 2 delta) vz.dz + Fv
     """
+    space_order = u.space_order
     # Forward or backward
     forward = kwargs.get('forward', True)
 
     dampl = 1 - model.damp
     m, epsilon, delta = model.m, model.epsilon, model.delta
     costheta, sintheta = trig_func(model)
     epsilon = 1 + 2 * epsilon
@@ -376,57 +271,58 @@
     qv = kwargs.get('qv', 0)
 
     # Staggered setup
     vx, vz, _ = particle_velocity_fields(model, space_order)
 
     if forward:
         # Stencils
-        phdx = costheta * u.dx - sintheta * u.dy
+        phdx = costheta * u.dx - sintheta * u.dyc
         u_vx = Eq(vx.forward, dampl * vx - dampl * s * phdx)
 
-        pvdz = sintheta * v.dx + costheta * v.dy
+        pvdz = sintheta * v.dxc + costheta * v.dy
         u_vz = Eq(vz.forward, dampl * vz - dampl * s * pvdz)
 
-        dvx = costheta * vx.forward.dx - sintheta * vx.forward.dy
-        dvz = sintheta * vz.forward.dx + costheta * vz.forward.dy
+        dvx = costheta * vx.forward.dx - sintheta * vx.forward.dyc
+        dvz = sintheta * vz.forward.dxc + costheta * vz.forward.dy
 
         # u and v equations
         pv_eq = Eq(v.forward, dampl * (v - s / m * (delta * dvx + dvz)) + s / m * qv)
         ph_eq = Eq(u.forward, dampl * (u - s / m * (epsilon * dvx + delta * dvz)) +
                    s / m * qu)
     else:
         # Stencils
-        phdx = ((costheta*epsilon*u).dx - (sintheta*epsilon*u).dy +
-                (costheta*delta*v).dx - (sintheta*delta*v).dy)
+        phdx = ((costheta*epsilon*u).dx - (sintheta*epsilon*u).dyc +
+                (costheta*delta*v).dxc - (sintheta*delta*v).dy)
         u_vx = Eq(vx.backward, dampl * vx + dampl * s * phdx)
 
-        pvdz = ((sintheta*delta*u).dx + (costheta*delta*u).dy +
-                (sintheta*v).dx + (costheta*v).dy)
+        pvdz = ((sintheta*delta*u).dx + (costheta*delta*u).dyc +
+                (sintheta*v).dxc + (costheta*v).dy)
         u_vz = Eq(vz.backward, dampl * vz + dampl * s * pvdz)
 
-        dvx = (costheta * vx.backward).dx - (sintheta * vx.backward).dy
-        dvz = (sintheta * vz.backward).dx + (costheta * vz.backward).dy
+        dvx = (costheta * vx.backward).dx - (sintheta * vx.backward).dyc
+        dvz = (sintheta * vz.backward).dxc + (costheta * vz.backward).dy
 
         # u and v equations
         pv_eq = Eq(v.backward, dampl * (v + s / m * dvz))
         ph_eq = Eq(u.backward, dampl * (u + s / m * dvx))
 
     return [u_vx, u_vz] + [pv_eq, ph_eq]
 
 
-def kernel_staggered_3d(model, u, v, space_order, **kwargs):
+def kernel_staggered_3d(model, u, v, **kwargs):
     """
     TTI finite difference. The equation solved is:
 
     vx.dt = - u.dx
     vy.dt = - u.dx
     vz.dt = - v.dx
     m * v.dt = - sqrt(1 + 2 delta) (vx.dx + vy.dy) - vz.dz + Fh
     m * u.dt = - (1 + 2 epsilon) (vx.dx + vy.dy) - sqrt(1 + 2 delta) vz.dz + Fv
     """
+    space_order = u.space_order
     # Forward or backward
     forward = kwargs.get('forward', True)
 
     dampl = 1 - model.damp
     m, epsilon, delta = model.m, model.epsilon, model.delta
     costheta, sintheta, cosphi, sinphi = trig_func(model)
     epsilon = 1 + 2 * epsilon
@@ -543,20 +439,19 @@
     src = PointSource(name='src', grid=model.grid, time_range=geometry.time_axis,
                       npoint=geometry.nsrc)
     rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
                    npoint=geometry.nrec)
 
     # FD kernels of the PDE
     FD_kernel = kernels[(kernel, len(model.shape))]
-    stencils = FD_kernel(model, u, v, space_order)
+    stencils = FD_kernel(model, u, v)
 
     # Source and receivers
     expr = src * dt / m if kernel == 'staggered' else src * dt**2 / m
-    stencils += src.inject(field=u.forward, expr=expr)
-    stencils += src.inject(field=v.forward, expr=expr)
+    stencils += src.inject(field=(u.forward, v.forward), expr=expr)
     stencils += rec.interpolate(expr=u + v)
 
     # Substitute spacing terms to reduce flops
     return Operator(stencils, subs=model.spacing_map, name='ForwardTTI', **kwargs)
 
 
 def AdjointOperator(model, geometry, space_order=4,
@@ -593,20 +488,19 @@
     srca = PointSource(name='srca', grid=model.grid, time_range=geometry.time_axis,
                        npoint=geometry.nsrc)
     rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
                    npoint=geometry.nrec)
 
     # FD kernels of the PDE
     FD_kernel = kernels[(kernel, len(model.shape))]
-    stencils = FD_kernel(model, p, r, space_order, forward=False)
+    stencils = FD_kernel(model, p, r, forward=False)
 
     # Construct expression to inject receiver values
     expr = rec * dt / m if kernel == 'staggered' else rec * dt**2 / m
-    stencils += rec.inject(field=p.backward, expr=expr)
-    stencils += rec.inject(field=r.backward, expr=expr)
+    stencils += rec.inject(field=(p.backward, r.backward), expr=expr)
 
     # Create interpolation expression for the adjoint-source
     stencils += srca.interpolate(expr=p + r)
 
     # Substitute spacing terms to reduce flops
     return Operator(stencils, subs=model.spacing_map, name='AdjointTTI', **kwargs)
 
@@ -648,25 +542,24 @@
                       time_order=2, space_order=space_order)
     dv = TimeFunction(name="dv", grid=model.grid, save=None,
                       time_order=2, space_order=space_order)
     dm = Function(name="dm", grid=model.grid, space_order=0)
 
     # FD kernels of the PDE
     FD_kernel = kernels[('centered', len(model.shape))]
-    eqn1 = FD_kernel(model, u0, v0, space_order)
+    eqn1 = FD_kernel(model, u0, v0)
 
     # Linearized source and stencil
     lin_usrc = -dm * u0.dt2
     lin_vsrc = -dm * v0.dt2
 
-    eqn2 = FD_kernel(model, du, dv, space_order, qu=lin_usrc, qv=lin_vsrc)
+    eqn2 = FD_kernel(model, du, dv, qu=lin_usrc, qv=lin_vsrc)
 
     # Construct expression to inject source values, injecting at u0(t+dt)/v0(t+dt)
-    src_term = src.inject(field=u0.forward, expr=src * dt**2 / m)
-    src_term += src.inject(field=v0.forward, expr=src * dt**2 / m)
+    src_term = src.inject(field=(u0.forward, v0.forward), expr=src * dt**2 / m)
 
     # Create interpolation expression for receivers, extracting at du(t)+dv(t)
     rec_term = rec.interpolate(expr=du + dv)
 
     # Substitute spacing terms to reduce flops
     return Operator(eqn1 + src_term + eqn2 + rec_term, subs=model.spacing_map,
                     name='BornTTI', **kwargs)
@@ -707,22 +600,21 @@
     dm = Function(name="dm", grid=model.grid)
 
     rec = Receiver(name='rec', grid=model.grid, time_range=geometry.time_axis,
                    npoint=geometry.nrec)
 
     # FD kernels of the PDE
     FD_kernel = kernels[('centered', len(model.shape))]
-    eqn = FD_kernel(model, du, dv, space_order, forward=False)
+    eqn = FD_kernel(model, du, dv, forward=False)
 
     dm_update = Inc(dm, - (u0 * du.dt2 + v0 * dv.dt2))
 
     # Add expression for receiver injection
-    rec_term = rec.inject(field=du.backward, expr=rec * dt**2 / m)
-    rec_term += rec.inject(field=dv.backward, expr=rec * dt**2 / m)
+    rec_term = rec.inject(field=(du.backward, dv.backward), expr=rec * dt**2 / m)
 
     # Substitute spacing terms to reduce flops
     return Operator(eqn + rec_term + [dm_update], subs=model.spacing_map,
                     name='GradientTTI', **kwargs)
 
 
-kernels = {('centered', 3): kernel_centered_3d, ('centered', 2): kernel_centered_2d,
+kernels = {('centered', 3): kernel_centered, ('centered', 2): kernel_centered,
            ('staggered', 3): kernel_staggered_3d, ('staggered', 2): kernel_staggered_2d}
```

### Comparing `devito-4.8.3/examples/seismic/tti/tti_example.py` & `devito-4.8.4/examples/seismic/tti/tti_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/tti/wavesolver.py` & `devito-4.8.4/examples/seismic/tti/wavesolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-from devito import (Function, TimeFunction, warning,
+from devito import (Function, TimeFunction, warning, NODE,
                     DevitoCheckpoint, CheckpointOperator, Revolver)
 from devito.tools import memoized_meth
 from examples.seismic.tti.operators import ForwardOperator, AdjointOperator
 from examples.seismic.tti.operators import JacobianOperator, JacobianAdjOperator
 from examples.seismic.tti.operators import particle_velocity_fields
 
 
@@ -114,17 +114,15 @@
 
         Returns
         -------
         Receiver, wavefield and performance summary.
         """
         if self.kernel == 'staggered':
             time_order = 1
-            dims = self.model.space_dimensions
-            stagg_u = (-dims[-1])
-            stagg_v = (-dims[0], -dims[1]) if self.model.grid.dim == 3 else (-dims[0])
+            stagg_u = stagg_v = NODE
         else:
             time_order = 2
             stagg_u = stagg_v = None
         # Source term is read-only, so re-use the default
         src = src or self.geometry.src
         # Create a new receiver object to store the result
         rec = rec or self.geometry.rec
@@ -189,17 +187,15 @@
 
         Returns
         -------
         Adjoint source, wavefield and performance summary.
         """
         if self.kernel == 'staggered':
             time_order = 1
-            dims = self.model.space_dimensions
-            stagg_p = (-dims[-1])
-            stagg_r = (-dims[0], -dims[1]) if self.model.grid.dim == 3 else (-dims[0])
+            stagg_p = stagg_r = NODE
         else:
             time_order = 2
             stagg_p = stagg_r = None
 
         # Source term is read-only, so re-use the default
         srca = srca or self.geometry.new_src(name='srca', src_type=None)
```

### Comparing `devito-4.8.3/examples/seismic/utils.py` & `devito-4.8.4/examples/seismic/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import numpy as np
 from argparse import Action, ArgumentError, ArgumentParser
 
 from devito import error, configuration, warning
 from devito.tools import Pickable
+from devito.types.sparse import _default_radius
 
 from .source import *
 
 __all__ = ['AcquisitionGeometry', 'setup_geometry', 'seismic_args']
 
 
-def setup_geometry(model, tn, f0=0.010):
+def setup_geometry(model, tn, f0=0.010, interpolation='linear', **kwargs):
     # Source and receiver geometries
     src_coordinates = np.empty((1, model.dim))
-    src_coordinates[0, :] = np.array(model.domain_size) * .5
     if model.dim > 1:
+        src_coordinates[0, :] = np.array(model.domain_size) * .5
         src_coordinates[0, -1] = model.origin[-1] + model.spacing[-1]
+    else:
+        src_coordinates[0, 0] = 2 * model.spacing[0]
 
     rec_coordinates = setup_rec_coords(model)
 
+    r = kwargs.get('r', _default_radius[interpolation])
     geometry = AcquisitionGeometry(model, rec_coordinates, src_coordinates,
-                                   t0=0.0, tn=tn, src_type='Ricker', f0=f0)
+                                   t0=0.0, tn=tn, src_type='Ricker', f0=f0,
+                                   interpolation=interpolation, r=r)
 
     return geometry
 
 
 def setup_rec_coords(model):
     nrecx = model.shape[0]
     recx = np.linspace(model.origin[0], model.domain_size[0], nrecx)
@@ -54,15 +59,15 @@
     - receiver positions and number
 
     In practice this would only point to a segy file with the
     necessary information
     """
 
     __rargs__ = ('grid', 'rec_positions', 'src_positions', 't0', 'tn')
-    __rkwargs__ = ('f0', 'src_type')
+    __rkwargs__ = ('f0', 'src_type', 'interpolation', 'r')
 
     def __init__(self, model, rec_positions, src_positions, t0, tn, **kwargs):
         """
         In practice would be __init__(segyfile) and all below parameters
         would come from a segy_read (at property call rather than at init)
         """
         src_positions = np.reshape(src_positions, (-1, model.dim))
@@ -81,14 +86,16 @@
                   " for source of type %s" % self._src_type)
 
         self._grid = model.grid
         self._model = model
         self._dt = model.critical_dt
         self._t0 = t0
         self._tn = tn
+        self._interpolation = kwargs.get('interpolation', 'linear')
+        self._r = kwargs.get('r', _default_radius[self.interpolation])
 
     def resample(self, dt):
         self._dt = dt
         return self
 
     @property
     def time_axis(self):
@@ -137,51 +144,63 @@
         return self._nsrc
 
     @property
     def dtype(self):
         return self.grid.dtype
 
     @property
+    def r(self):
+        return self._r
+
+    @property
+    def interpolation(self):
+        return self._interpolation
+
+    @property
     def rec(self):
         return self.new_rec()
 
     def new_rec(self, name='rec'):
         return Receiver(name=name, grid=self.grid,
                         time_range=self.time_axis, npoint=self.nrec,
-                        coordinates=self.rec_positions)
+                        coordinates=self.rec_positions,
+                        interpolation=self.interpolation, r=self._r)
 
     @property
     def adj_src(self):
         if self.src_type is None:
             warning("No source type defined, returning uninitiallized (zero) shot record")
             return self.new_rec()
         adj_src = sources[self.src_type](name='rec', grid=self.grid, f0=self.f0,
                                          time_range=self.time_axis, npoint=self.nrec,
                                          coordinates=self.rec_positions,
-                                         t0=self._t0w, a=self._a)
+                                         t0=self._t0w, a=self._a,
+                                         interpolation=self.interpolation, r=self._r)
         # Revert time axis to have a proper shot record and not compute on zeros
         for i in range(self.nrec):
             adj_src.data[:, i] = adj_src.wavelet[::-1]
         return adj_src
 
     @property
     def src(self):
         return self.new_src()
 
     def new_src(self, name='src', src_type='self'):
         if self.src_type is None or src_type is None:
             warning("No source type defined, returning uninitiallized (zero) source")
             return PointSource(name=name, grid=self.grid,
                                time_range=self.time_axis, npoint=self.nsrc,
-                               coordinates=self.src_positions)
+                               coordinates=self.src_positions,
+                               interpolation=self.interpolation, r=self._r)
         else:
             return sources[self.src_type](name=name, grid=self.grid, f0=self.f0,
                                           time_range=self.time_axis, npoint=self.nsrc,
                                           coordinates=self.src_positions,
-                                          t0=self._t0w, a=self._a)
+                                          t0=self._t0w, a=self._a,
+                                          interpolation=self.interpolation, r=self._r)
 
 
 sources = {'Wavelet': WaveletSource, 'Ricker': RickerSource, 'Gabor': GaborSource}
 
 
 def seismic_args(description):
     """
@@ -230,8 +249,10 @@
     parser.add_argument('-a', '--autotune', default='off',
                         choices=(configuration._accepted['autotuning']),
                         help="Operator auto-tuning mode")
     parser.add_argument("-tn", "--tn", default=0,
                         type=float, help="Simulation time in millisecond")
     parser.add_argument("-dtype", action=_dtype_store, dest="dtype", default=np.float32,
                         choices=['float32', 'float64'])
+    parser.add_argument("-interp", dest="interp", default="linear",
+                        choices=['linear', 'sinc'])
     return parser
```

### Comparing `devito-4.8.3/examples/seismic/viscoacoustic/operators.py` & `devito-4.8.4/examples/seismic/viscoacoustic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/viscoacoustic/viscoacoustic_example.py` & `devito-4.8.4/examples/seismic/viscoacoustic/viscoacoustic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/viscoacoustic/wavesolver.py` & `devito-4.8.4/examples/seismic/viscoacoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/viscoelastic/operators.py` & `devito-4.8.4/examples/seismic/viscoelastic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/examples/seismic/viscoelastic/viscoelastic_example.py` & `devito-4.8.4/examples/seismic/viscoelastic/viscoelastic_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             [rec1, rec2, v, tau])
 
 
 @pytest.mark.parametrize("dtype", [np.float32, np.float64])
 def test_viscoelastic(dtype):
     _, _, _, [rec1, rec2, v, tau] = run(dtype=dtype)
     assert np.isclose(norm(rec1), 12.28040, atol=1e-3, rtol=0)
-    assert np.isclose(norm(rec2), 0.312461, atol=1e-3, rtol=0)
+    assert np.isclose(norm(rec2), 0.312462, atol=1e-3, rtol=0)
 
 
 @pytest.mark.parametrize('shape', [(51, 51), (16, 16, 16)])
 def test_viscoelastic_stability(shape):
     spacing = tuple([20]*len(shape))
     _, _, _, [rec1, rec2, v, tau] = run(shape=shape, spacing=spacing, tn=20000.0, nbl=0)
     assert np.isfinite(norm(rec1))
```

### Comparing `devito-4.8.3/examples/seismic/viscoelastic/wavesolver.py` & `devito-4.8.4/examples/seismic/viscoelastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.3/versioneer.py` & `devito-4.8.4/versioneer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 
-# Version: 0.22
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain (CC0-1.0)
+* License: Public Domain (Unlicense)
 * Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils/setuptools-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -227,17 +255,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -259,188 +288,250 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
 
-def get_root():
+
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -448,16 +539,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -467,161 +565,187 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -629,52 +753,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -683,15 +852,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -708,34 +877,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -752,31 +922,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -795,20 +1013,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -817,15 +1064,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -837,15 +1084,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -857,47 +1104,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -910,15 +1161,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -937,83 +1188,95 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1021,52 +1284,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1075,15 +1383,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1100,91 +1408,95 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1193,50 +1505,49 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1253,31 +1564,79 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1296,20 +1655,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1318,15 +1706,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1338,15 +1726,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1358,32 +1746,36 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1394,30 +1786,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1470,109 +1862,152 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools subclasses used by Versioneer."""
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py: Any = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext: Any = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self) -> None:
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1588,20 +2023,20 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1614,30 +2049,67 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info: Any = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist: Any = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1682,29 +2154,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
 
-def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+
+def do_setup() -> int:
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1716,70 +2193,45 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1808,14 +2260,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

