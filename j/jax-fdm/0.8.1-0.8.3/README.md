# Comparing `tmp/jax_fdm-0.8.1.tar.gz` & `tmp/jax_fdm-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_fdm-0.8.1.tar", last modified: Tue Dec  5 14:46:31 2023, max compression
+gzip compressed data, was "jax_fdm-0.8.3.tar", last modified: Thu Apr 18 20:12:40 2024, max compression
```

## Comparing `jax_fdm-0.8.1.tar` & `jax_fdm-0.8.3.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-05 14:46:31.242041 jax_fdm-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.218042 jax_fdm-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.222041 jax_fdm-0.8.1/src/jax_fdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.222041 jax_fdm-0.8.1/src/jax_fdm/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.222041 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/edge/length.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.226041 jax_fdm-0.8.1/src/jax_fdm/constraints/network/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/network/force.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/network/length.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.226041 jax_fdm-0.8.1/src/jax_fdm/constraints/node/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/constraints/node/tangent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.226041 jax_fdm-0.8.1/src/jax_fdm/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/datastructures/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/datastructures/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/datastructures/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.226041 jax_fdm-0.8.1/src/jax_fdm/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/fdm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/loads.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.226041 jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.230041 jax_fdm-0.8.1/src/jax_fdm/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14171 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.230041 jax_fdm-0.8.1/src/jax_fdm/goals/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/abstract_goal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.230041 jax_fdm-0.8.1/src/jax_fdm/goals/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/edge/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/goal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.230041 jax_fdm-0.8.1/src/jax_fdm/goals/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/mesh/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/mesh/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.230041 jax_fdm-0.8.1/src/jax_fdm/goals/network/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/network/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/network/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.234042 jax_fdm-0.8.1/src/jax_fdm/goals/node/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/goals/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.234042 jax_fdm-0.8.1/src/jax_fdm/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/losses/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/losses/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.234042 jax_fdm-0.8.1/src/jax_fdm/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.234042 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/constrained.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/second_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/optimization/recorders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.234042 jax_fdm-0.8.1/src/jax_fdm/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/parameters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/parameters/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm/visualization/artists/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/artists/network_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/loss_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/vector_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-12-05 14:46:19.000000 jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:46:31.238041 jax_fdm-0.8.1/src/jax_fdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-05 14:46:31.000000 jax_fdm-0.8.1/src/jax_fdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19537 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.788622 jax_fdm-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.792622 jax_fdm-0.8.3/src/jax_fdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/length.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/tangent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/fdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/goals/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/abstract_goal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/goals/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/goal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/recorders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/network_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/loss_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/vector_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/top_level.txt
```

### Comparing `jax_fdm-0.8.1/CHANGELOG.md` & `jax_fdm-0.8.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,47 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## Unreleased
+
+### Added
+
+### Changed
+
+### Removed
+
+
+## [0.8.3] 2024-04-18
+
+### Added
+
+#### Goals
+- Implemented `EdgeLoadPathGoal`.
+
+### Changed
+
+#### Floating-point arithmetic
+- Updated how to enable double floating precision (`float64`) to comply with changes of `jax.config` in `jax==0.4.25`.
+
+#### Equilibrium
+- Fixed duplicated fixed point iteration in `EquilibriumModel.equilibrium_iterative`. This led to unnecessarily long runtimes. This change also fixes the "mysterious" bug that made `jaxopt` implicit differentiation incompatible with sparse matrices. 
+
+#### Visualization
+- `LossPlotter` exposes `plot_legend` to choose whether or not to show legend with curve labels.
+- `FDNetworkArtist` takes absolute force density values to calculate viz colors in `"fd"` mode.
+- Fixed bug in `FDNetworkViewerArtist` that threw error when inputing a custom list of edges to display. The problem was that the artist could not find the width of all the edges connected to a node because `edge_width` is only computed for the custom list of edges. The artist was expecting a dictionary with _all_ the edge widths.
+- Package `compas-notebook` became an optional dependency because it does not support `compas<2.0` anymore.
+
+### Removed
+
+
 ## [0.8.1] 2023-12-05
 
 ### Added
 
 #### Losses
 - Implemented `LogMaxError`. The goal of this error function is to work as a barrier soft constraint for target maximum values. One good use example would be to restrict the height of a shell to a maximum height.
```

### Comparing `jax_fdm-0.8.1/LICENSE` & `jax_fdm-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/PKG-INFO` & `jax_fdm-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.8.1
+Version: 0.8.3
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -22,17 +22,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: jax[cpu]
-Requires-Dist: compas
+Requires-Dist: compas<2.0
 Requires-Dist: compas_singular
-Requires-Dist: compas-notebook
 Requires-Dist: scipy
 Requires-Dist: equinox
 Requires-Dist: jaxopt
 
 <h1 align='center'>JAX FDM</h1>
 
 <!-- Badges -->
```

### Comparing `jax_fdm-0.8.1/README.md` & `jax_fdm-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/setup.cfg` & `jax_fdm-0.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/setup.py` & `jax_fdm-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="jax_fdm",
-    version="0.8.1",
+    version="0.8.3",
     description="Auto-differentiable and hardware-accelerated force density method",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arpastrana/jax_fdm",
     author="Rafael Pastrana",
     author_email="arpastrana@princeton.edu",
     license="MIT license",
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/__init__.py` & `jax_fdm-0.8.3/src/jax_fdm/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 
 
 __author__ = ["Rafael Pastrana"]
 __copyright__ = "Rafael Pastrana"
 __license__ = "MIT License"
 __email__ = "arpastrana@princeton.edu"
-__version__ = "0.8.1"
+__version__ = "0.8.3"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
@@ -42,9 +42,9 @@
 DTYPE_JAX = jnp.float64
 
 DTYPE_INT_NP = jnp.int32
 DTYPE_INT_JAX = jnp.int32
 
 # this only works on startup!
 if DTYPE_JAX == jnp.float64 or DTYPE_NP == np.float64:
-    from jax.config import config
-    config.update("jax_enable_x64", True)
+    import jax
+    jax.config.update("jax_enable_x64", True)
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/constraint.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/edge/angle.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/node/coordinates.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/node/curvature.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/node/curvature.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/node/normal.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/constraints/node/tangent.py` & `jax_fdm-0.8.3/src/jax_fdm/constraints/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/datastructures/datastructure.py` & `jax_fdm-0.8.3/src/jax_fdm/datastructures/datastructure.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/datastructures/mesh.py` & `jax_fdm-0.8.3/src/jax_fdm/datastructures/mesh.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/datastructures/network.py` & `jax_fdm-0.8.3/src/jax_fdm/datastructures/network.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/fdm.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/fdm.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/loads.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/loads.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/models.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,28 +237,31 @@
         A = self.stiffness_matrix(q, structure)
         f_fixed = self.force_fixed_matrix(q, xyz_fixed, structure)
 
         solver = solver or self.itersolve_fn
         solver_config = {"tmax": tmax,
                          "eta": eta,
                          "verbose": verbose,
-                         # For jaxopt compatibility (as it does not support sparse matrices yet)
-                         "implicit": False if self.linearsolve_fn is spsolve else True}
+                         "implicit": True}
+        # For jaxopt compatibility (as it does not support sparse matrices yet)
+        #  "implicit": False if self.linearsolve_fn is spsolve else True}
 
         solver_kwargs = {"solver_config": solver_config,
                          "f": equilibrium_iterative_fn,
                          "a": (A, f_fixed, xyz_fixed, load_state),
                          "x_init": xyz_init}
 
         if implicit_diff:
-            xyz_new = fixed_point(solver, **solver_kwargs)
+            # xyz_new = fixed_point(solver, **solver_kwargs)
+            return fixed_point(solver, **solver_kwargs)
 
-        xyz_new = solver(**solver_kwargs)
+        # xyz_new = solver(**solver_kwargs)
+        return solver(**solver_kwargs)
 
-        return xyz_new
+        # return xyz_new
 
     # ----------------------------------------------------------------------
     # Equilibrium state
     # ----------------------------------------------------------------------
 
     def equilibrium_state(self, q, xyz, loads_nodes, structure):
         """
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/solvers.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/solvers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/sparse.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/sparse.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/states.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/states.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/mixins.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/mixins.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/structures.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/structures.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/equilibrium/structures/topology.py` & `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/topology.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/geometry/geometry.py` & `jax_fdm-0.8.3/src/jax_fdm/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/abstract_goal.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/abstract_goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/edge/angle.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/edge/direction.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/edge/direction.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/edge/edge.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/edge/edge.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/edge/force.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/edge/force.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/edge/length.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/edge/length.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/goal.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/helpers.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/mesh/area.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/mesh/area.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/mesh/laplacian.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/mesh/laplacian.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/network/laplacian.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/network/laplacian.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/network/loadpath.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/network/loadpath.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/coordinates.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/line.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/line.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/node.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/node.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/normal.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/plane.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/plane.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/residual.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/residual.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/goals/node/tangent.py` & `jax_fdm-0.8.3/src/jax_fdm/goals/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/losses/errors.py` & `jax_fdm-0.8.3/src/jax_fdm/losses/errors.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/losses/loss.py` & `jax_fdm-0.8.3/src/jax_fdm/losses/loss.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/collections.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/collections.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/constrained.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/constrained.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/ipopt.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/ipopt.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/optimizer.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/scipy.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/optimizers/second_order.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/second_order.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/optimization/recorders.py` & `jax_fdm-0.8.3/src/jax_fdm/optimization/recorders.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/parameters/helpers.py` & `jax_fdm-0.8.3/src/jax_fdm/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/parameters/manager.py` & `jax_fdm-0.8.3/src/jax_fdm/parameters/manager.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/parameters/parameters.py` & `jax_fdm-0.8.3/src/jax_fdm/parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/artists/network_artist.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/artists/network_artist.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             self._edge_color = {edge: color for edge in self.edges}
 
         elif isinstance(color, str):
             network = self.network
 
             if color == "fd":
                 cmap = self.default_fdcolormap
-                values = [network.edge_forcedensity(edge) for edge in self.edges]
+                values = [fabs(network.edge_forcedensity(edge)) for edge in self.edges]
                 try:
                     ratios = remap_values(values)
                 except ZeroDivisionError:
                     ratios = [0.0] * len(self.edges)
 
                 self._edge_color = {edge: cmap(ratio) for edge, ratio in zip(self.edges, ratios)}
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/network_artist.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/shapes.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/shapes.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/notebooks/viewer.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from math import radians
 
 from compas.artists import Artist
 
-from compas_notebook.app import App as NotebookApp
+try:
+    from compas_notebook.app import App as NotebookApp
+except ImportError:
+    class NotebookApp:
+        pass
 
 from jax_fdm.datastructures import FDNetwork
 
 
 __all__ = ["NotebookViewer"]
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/loss_plotter.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/loss_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Plot a loss function.
     """
     def __init__(self, loss, datastructure, *args, **kwargs):
         self.loss = loss
         self.structure = structure_from_datastructure(datastructure, sparse=False)
         self.fig = plt.figure(**kwargs)
 
-    def plot(self, history, print_breakdown=True):
+    def plot(self, history, print_breakdown=True, plot_legend=True):
         """
         Plot the loss function and its error components on a list of fdm parameter states.
         """
         print("\nPlotting loss function...")
         start_time = time()
 
         # Create batched parameter state
@@ -68,18 +68,22 @@
 
         plt.plot(losses, label=self.loss.name)
 
         plt.xlabel("Optimization iterations")
         plt.ylabel("Loss")
         plt.yscale("log")
         plt.grid()
-        plt.legend()
+
+        if plot_legend:
+            plt.legend()
 
         print(f"Plotting time: {(time() - start_time):.4} seconds")
 
+        return losses
+
     def show(self):
         """
         Display the plot.
         """
         plt.show()
 
     @staticmethod
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/network_artist.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/register.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/register.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/plotters/vector_artist.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/vector_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/network_artist.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/network_artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,21 @@
 
         xyz = self.network.node_coordinates(node)
 
         # shift start to make arrow head touch the node the load is applied to
         start = add_vectors(xyz, scale_vector(vector, -scale))
 
         # shift start to account for half size of edge thickness
-        widths = [self.edge_width[edge] for edge in self.network.connected_edges(node)]
+        widths = []
+        for edge in self.network.connected_edges(node):
+            width = self.edge_width.get(edge)
+            if not width:
+                width = 0.0
+            widths.append(width)
+
         start = add_vectors(start, scale_vector(normalize_vector(vector), -max(widths)))
 
         return self.draw_vector(vector, start, scale)
 
     def add_load(self, load, color):
         """
         Add one load to the viewer.
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm/visualization/viewers/viewer.py` & `jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.1/src/jax_fdm.egg-info/PKG-INFO` & `jax_fdm-0.8.3/src/jax_fdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jax-fdm
-Version: 0.8.1
+Name: jax_fdm
+Version: 0.8.3
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -22,17 +22,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: jax[cpu]
-Requires-Dist: compas
+Requires-Dist: compas<2.0
 Requires-Dist: compas_singular
-Requires-Dist: compas-notebook
 Requires-Dist: scipy
 Requires-Dist: equinox
 Requires-Dist: jaxopt
 
 <h1 align='center'>JAX FDM</h1>
 
 <!-- Badges -->
```

### Comparing `jax_fdm-0.8.1/src/jax_fdm.egg-info/SOURCES.txt` & `jax_fdm-0.8.3/src/jax_fdm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 src/jax_fdm/goals/state.py
 src/jax_fdm/goals/edge/__init__.py
 src/jax_fdm/goals/edge/angle.py
 src/jax_fdm/goals/edge/direction.py
 src/jax_fdm/goals/edge/edge.py
 src/jax_fdm/goals/edge/force.py
 src/jax_fdm/goals/edge/length.py
+src/jax_fdm/goals/edge/loadpath.py
 src/jax_fdm/goals/mesh/__init__.py
 src/jax_fdm/goals/mesh/area.py
 src/jax_fdm/goals/mesh/laplacian.py
 src/jax_fdm/goals/mesh/mesh.py
 src/jax_fdm/goals/network/__init__.py
 src/jax_fdm/goals/network/laplacian.py
 src/jax_fdm/goals/network/loadpath.py
```

