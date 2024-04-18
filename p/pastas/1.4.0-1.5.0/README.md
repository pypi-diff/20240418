# Comparing `tmp/pastas-1.4.0.tar.gz` & `tmp/pastas-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastas-1.4.0.tar", last modified: Tue Feb 20 10:32:16 2024, max compression
+gzip compressed data, was "pastas-1.5.0.tar", last modified: Thu Apr 18 09:05:38 2024, max compression
```

## Comparing `pastas-1.4.0.tar` & `pastas-1.5.0.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.556303 pastas-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-20 10:32:02.000000 pastas-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-02-20 10:32:16.556303 pastas-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-02-20 10:32:02.000000 pastas-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.544303 pastas-1.4.0/pastas/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.548303 pastas-1.4.0/pastas/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/extensions/accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.548303 pastas-1.4.0/pastas/io/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/io/pas.py
--rw-r--r--   0 runner    (1001) docker     (127)    75693 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/modelstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/noisemodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/objective_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.548303 pastas-1.4.0/pastas/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36288 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/modelcompare.py
--rw-r--r--   0 runner    (1001) docker     (127)    37831 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/modelplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    22781 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)    33543 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/plotting/plotutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/rcparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    28339 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/recharge.py
--rw-r--r--   0 runner    (1001) docker     (127)    58592 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/rfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    35560 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.548303 pastas-1.4.0/pastas/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20815 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/dutch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20145 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/sgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    54277 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    18326 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stats/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    68738 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/stressmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29722 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/timeseries_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.548303 pastas-1.4.0/pastas/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/typing/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-20 10:32:02.000000 pastas-1.4.0/pastas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.552303 pastas-1.4.0/pastas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-02-20 10:32:16.000000 pastas-1.4.0/pastas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-20 10:32:16.000000 pastas-1.4.0/pastas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:32:16.000000 pastas-1.4.0/pastas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-20 10:32:16.000000 pastas-1.4.0/pastas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 10:32:16.000000 pastas-1.4.0/pastas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-02-20 10:32:02.000000 pastas-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:32:16.556303 pastas-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:32:16.552303 pastas-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_001.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_gxg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_notebooks_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_qgxg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_recharge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_rfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-20 10:32:02.000000 pastas-1.4.0/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.057287 pastas-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 09:05:24.000000 pastas-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-18 09:05:38.057287 pastas-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-18 09:05:24.000000 pastas-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.045286 pastas-1.5.0/pastas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.049286 pastas-1.5.0/pastas/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/extensions/accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.049286 pastas-1.5.0/pastas/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/io/pas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81291 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/modelstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/noisemodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/objective_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.049286 pastas-1.5.0/pastas/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36700 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/modelcompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39187 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/modelplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23306 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33536 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/plotting/plotutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/rcparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28339 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58346 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/rfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.049286 pastas-1.5.0/pastas/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20815 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/dutch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/sgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54378 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stats/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70469 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/stressmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29906 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/timeseries_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.053286 pastas-1.5.0/pastas/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/typing/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-18 09:05:25.000000 pastas-1.5.0/pastas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.053286 pastas-1.5.0/pastas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-18 09:05:38.000000 pastas-1.5.0/pastas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-18 09:05:38.000000 pastas-1.5.0/pastas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:05:38.000000 pastas-1.5.0/pastas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 09:05:38.000000 pastas-1.5.0/pastas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 09:05:38.000000 pastas-1.5.0/pastas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-18 09:05:25.000000 pastas-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:05:38.057287 pastas-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:38.053286 pastas-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_gxg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_notebooks_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_qgxg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_recharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_rfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-18 09:05:25.000000 pastas-1.5.0/tests/test_timeseries_utils.py
```

### Comparing `pastas-1.4.0/LICENSE` & `pastas-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/PKG-INFO` & `pastas-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastas
-Version: 1.4.0
+Version: 1.5.0
 Summary: Pastas is an open-source Python framework for the analysis of groundwater time series.
 Author: Collenteur et al. 2019
 Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <vonk.mart@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2021 R.A. Collenteur, M. Bakker, R. Calje, F. Schaars
         
@@ -31,22 +31,21 @@
 Project-URL: documentation, https://pastas.readthedocs.io/en/latest/
 Keywords: hydrology,groundwater,timeseries,analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: matplotlib>=3.1
 Requires-Dist: pandas>=1.1
 Requires-Dist: scipy>=1.8
 Requires-Dist: numba>=0.51
 Provides-Extra: solvers
@@ -69,14 +68,15 @@
 Requires-Dist: pastas[pytesting,solvers]; extra == "ci"
 Requires-Dist: jupyter; extra == "ci"
 Requires-Dist: coverage; extra == "ci"
 Requires-Dist: corner; extra == "ci"
 Requires-Dist: emcee; extra == "ci"
 Requires-Dist: tqdm; extra == "ci"
 Requires-Dist: plotly; extra == "ci"
+Requires-Dist: bokeh>=3.0; extra == "ci"
 Provides-Extra: rtd
 Requires-Dist: pastas[solvers]; extra == "rtd"
 Requires-Dist: Ipython; extra == "rtd"
 Requires-Dist: ipykernel; extra == "rtd"
 Requires-Dist: pydata-sphinx-theme; extra == "rtd"
 Requires-Dist: sphinx<6.0,>=3.1; extra == "rtd"
 Requires-Dist: sphinxcontrib-bibtex; extra == "rtd"
@@ -86,123 +86,136 @@
 Requires-Dist: myst_nb; extra == "rtd"
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pastas[ci,formatting,linting,rtd]; extra == "dev"
 Provides-Extra: numbascipy
 Requires-Dist: numba-scipy>=0.3.1; extra == "numbascipy"
 
-Pastas: Analysis of Groundwater Time Series
-===========================================
+# Pastas: Analysis of Groundwater Time Series
 
-.. image:: /doc/_static/logo_small.png
-   :width: 200px
-   :align: left
-
-.. image:: https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master
-   :target: https://github.com/pastas/pastas/actions/workflows/ci.yml
-.. image:: https://img.shields.io/pypi/v/pastas.svg
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/l/pastas.svg
-   :target: https://mit-license.org/
-.. image:: https://img.shields.io/pypi/pyversions/pastas
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/dm/pastas
-   :target: https://pypi.org/project/pastas/
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg
-   :target: https://doi.org/10.5281/zenodo.1465866
-.. image:: https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
-.. image:: https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9
-.. image:: https://readthedocs.org/projects/pastas/badge/?version=latest
-   :target: https://pastas.readthedocs.io/en/latest/?badge=latest
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb
-
-Pastas: what is it?
-~~~~~~~~~~~~~~~~~~~
-Pastas is an open source python package for processing, simulating and analyzing
-groundwater time series. The object oriented structure allows for the quick
-implementation of new model components. Time series models can be created,
-calibrated, and analysed with just a few lines of python code with the
-built-in optimization, visualisation, and statistical analysis tools.
-
-Documentation & Examples
-~~~~~~~~~~~~~~~~~~~~~~~~
-- Documentation is provided on the dedicated website `pastas.dev <http://www.pastas.dev/>`_
-- Examples can be found on the `examples directory on the documentation website <https://pastas.readthedocs.io/en/dev/examples/index.html>`_
-- View and edit a working example notebook of a Pastas model in `MyBinder <https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb>`_
-- A list of publications that use Pastas is available in a `dedicated Zotero group <https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list>`_
-
-Get in Touch
-~~~~~~~~~~~~
-- Questions on Pastas can be asked and answered on `Github Discussions <https://github.com/pastas/pastas/discussions>`_.
-- Bugs, feature requests and other improvements can be posted as `Github Issues <https://github.com/pastas/pastas/issues>`_.
-- Pull requests will only be accepted on the development branch (dev) of
-  this repository. Please take a look at the `developers section
-  <http://pastas.readthedocs.io/>`_ on the documentation website for more
-  information on how to contribute to Pastas.
-
-Quick installation guide
-~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
-installed on your computer. We recommend using the `Anaconda Distribution
-<https://www.continuum.io/downloads>`_ as it includes most of the python
-package dependencies and the Jupyter Notebook software to run the notebooks.
-However, you are free to install any Python distribution you want.
-
-Stable version
---------------
-To get the latest stable version, use::
-
-  pip install pastas
-
-Update
-------
-To update pastas, use::
-
-  pip install pastas --upgrade
-
-Developers
-----------
-To get the latest development version, use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
-
-Related packages
-~~~~~~~~~~~~~~~~
-- `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
-- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
-- `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
-- `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
-
-Dependencies
-~~~~~~~~~~~~
-Pastas depends on a number of Python packages, of which all of the necessary
-are automatically installed when using the pip install manager. To
-summarize, the dependencies necessary for a minimal function installation of
-Pastas
-
-- numpy>=1.7
-- matplotlib>=3.1
-- pandas>=1.1
-- scipy>=1.8
-- numba>=0.51
-
-To install the most important optional dependencies (solver LmFit and function visualisation Latexify) at the same time with Pastas use::
-
-   pip install pastas[full]
-
-or for the development version use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
-
-How to Cite Pastas?
-~~~~~~~~~~~~~~~~~~~
-If you use Pastas in one of your studies, please cite the Pastas article in Groundwater:
+> [!IMPORTANT]
+> As of Pastas 1.5, noisemodels are not added to the Pastas models by default anymore. [Read more about this change here](https://github.com/pastas/pastas/issues/735).
 
-- Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F. (2019) `Pastas: open source software for the analysis of groundwater time series <https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925>`_. Groundwater. doi: 10.1111/gwat.12925.
+![image](/doc/_static/logo_small.png)
+[![image](https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/pastas/pastas/actions/workflows/ci.yml)
+[![image](https://img.shields.io/pypi/v/pastas.svg)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/l/pastas.svg)](https://mit-license.org/)
+[![image](https://img.shields.io/pypi/pyversions/pastas)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/dm/pastas)](https://pypi.org/project/pastas/)
+[![image](https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg)](https://doi.org/10.5281/zenodo.1465866)
+[![image](https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![image](https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9)
+[![image](https://readthedocs.org/projects/pastas/badge/?version=latest)](https://pastas.readthedocs.io/en/latest/?badge=latest)
+[![image](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
 
-To cite a specific version of Python, you can use the DOI provided for each official release (>0.9.7) through Zenodo. Click on the link to get a specific version and DOI, depending on the Pastas version.
+## Pastas: what is it?
 
-- Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas: open-source software for time series analysis in hydrology (Version X.X.X). Zenodo. http://doi.org/10.5281/zenodo.1465866
+Pastas is an open source python package for processing, simulating and
+analyzing groundwater time series. The object oriented structure allows
+for the quick implementation of new model components. Time series models
+can be created, calibrated, and analysed with just a few lines of python
+code with the built-in optimization, visualisation, and statistical
+analysis tools.
 
+## Documentation & Examples
+
+-   Documentation is provided on the dedicated website
+    [pastas.dev](http://www.pastas.dev/)
+-   Examples can be found on the [examples directory on the
+    documentation
+    website](https://pastas.readthedocs.io/en/dev/examples/index.html)
+-   View and edit a working example notebook of a Pastas model in
+    [MyBinder](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
+-   A list of publications that use Pastas is available in a [dedicated
+    Zotero
+    group](https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list)
+
+## Get in Touch
+
+-   Questions on Pastas can be asked and answered on [Github
+    Discussions](https://github.com/pastas/pastas/discussions).
+-   Bugs, feature requests and other improvements can be posted as
+    [Github Issues](https://github.com/pastas/pastas/issues).
+-   Pull requests will only be accepted on the development branch (dev)
+    of this repository. Please take a look at the [developers
+    section](http://pastas.readthedocs.io/) on the documentation website
+    for more information on how to contribute to Pastas.
+
+## Quick installation guide
+
+To install Pastas, a working version of Python 3.9, 3.10, 3.11, or 3.12
+has to be installed on your computer. We recommend using the [Anaconda
+Distribution](https://www.continuum.io/downloads) as it includes most of
+the python package dependencies and the Jupyter Notebook software to run
+the notebooks. However, you are free to install any Python distribution
+you want.
+
+### Stable version
+
+To get the latest stable version, use:
+
+    pip install pastas
+
+### Update
+
+To update pastas, use:
+
+    pip install pastas --upgrade
+
+### Developers
+
+To get the latest development version, use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
+
+## Related packages
+
+-   [Pastastore](https://github.com/pastas/pastastore) is a Python
+    package for managing multiple timeseries and pastas models
+-   [Metran](https://github.com/pastas/metran) is a Python package to
+    perform multivariate timeseries analysis using a technique called
+    dynamic factor modelling.
+-   [Hydropandas](https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb)
+    can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
+-   [PyEt](https://github.com/phydrus/pyet) can be used to compute
+    potential evaporation from meteorological variables.
+
+## Dependencies
+
+Pastas depends on a number of Python packages, of which all of the
+necessary are automatically installed when using the pip install
+manager. To summarize, the dependencies necessary for a minimal function
+installation of Pastas
+
+-   numpy\>=1.7
+-   matplotlib\>=3.1
+-   pandas\>=1.1
+-   scipy\>=1.8
+-   numba\>=0.51
+
+To install the most important optional dependencies (solver LmFit and
+function visualisation Latexify) at the same time with Pastas use:
+
+    pip install pastas[full]
+
+or for the development version use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
+
+## How to Cite Pastas?
+
+If you use Pastas in one of your studies, please cite the Pastas article
+in Groundwater:
+
+-   Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F.
+    (2019) [Pastas: open source software for the analysis of groundwater
+    time
+    series](https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925).
+    Groundwater. doi: 10.1111/gwat.12925.
+
+To cite a specific version of Pastas, you can use the DOI provided for
+each official release (\>0.9.7) through Zenodo. Click on the link to get
+a specific version and DOI, depending on the Pastas version.
+
+-   Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas:
+    open-source software for time series analysis in hydrology (Version
+    X.X.X). Zenodo. <http://doi.org/10.5281/zenodo.1465866>
```

### Comparing `pastas-1.4.0/README.rst` & `pastas-1.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,129 @@
-Pastas: Analysis of Groundwater Time Series
-===========================================
+# Pastas: Analysis of Groundwater Time Series
 
-.. image:: /doc/_static/logo_small.png
-   :width: 200px
-   :align: left
-
-.. image:: https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master
-   :target: https://github.com/pastas/pastas/actions/workflows/ci.yml
-.. image:: https://img.shields.io/pypi/v/pastas.svg
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/l/pastas.svg
-   :target: https://mit-license.org/
-.. image:: https://img.shields.io/pypi/pyversions/pastas
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/dm/pastas
-   :target: https://pypi.org/project/pastas/
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg
-   :target: https://doi.org/10.5281/zenodo.1465866
-.. image:: https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
-.. image:: https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9
-.. image:: https://readthedocs.org/projects/pastas/badge/?version=latest
-   :target: https://pastas.readthedocs.io/en/latest/?badge=latest
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb
-
-Pastas: what is it?
-~~~~~~~~~~~~~~~~~~~
-Pastas is an open source python package for processing, simulating and analyzing
-groundwater time series. The object oriented structure allows for the quick
-implementation of new model components. Time series models can be created,
-calibrated, and analysed with just a few lines of python code with the
-built-in optimization, visualisation, and statistical analysis tools.
-
-Documentation & Examples
-~~~~~~~~~~~~~~~~~~~~~~~~
-- Documentation is provided on the dedicated website `pastas.dev <http://www.pastas.dev/>`_
-- Examples can be found on the `examples directory on the documentation website <https://pastas.readthedocs.io/en/dev/examples/index.html>`_
-- View and edit a working example notebook of a Pastas model in `MyBinder <https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb>`_
-- A list of publications that use Pastas is available in a `dedicated Zotero group <https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list>`_
-
-Get in Touch
-~~~~~~~~~~~~
-- Questions on Pastas can be asked and answered on `Github Discussions <https://github.com/pastas/pastas/discussions>`_.
-- Bugs, feature requests and other improvements can be posted as `Github Issues <https://github.com/pastas/pastas/issues>`_.
-- Pull requests will only be accepted on the development branch (dev) of
-  this repository. Please take a look at the `developers section
-  <http://pastas.readthedocs.io/>`_ on the documentation website for more
-  information on how to contribute to Pastas.
-
-Quick installation guide
-~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
-installed on your computer. We recommend using the `Anaconda Distribution
-<https://www.continuum.io/downloads>`_ as it includes most of the python
-package dependencies and the Jupyter Notebook software to run the notebooks.
-However, you are free to install any Python distribution you want.
-
-Stable version
---------------
-To get the latest stable version, use::
-
-  pip install pastas
-
-Update
-------
-To update pastas, use::
-
-  pip install pastas --upgrade
-
-Developers
-----------
-To get the latest development version, use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
-
-Related packages
-~~~~~~~~~~~~~~~~
-- `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
-- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
-- `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
-- `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
-
-Dependencies
-~~~~~~~~~~~~
-Pastas depends on a number of Python packages, of which all of the necessary
-are automatically installed when using the pip install manager. To
-summarize, the dependencies necessary for a minimal function installation of
-Pastas
-
-- numpy>=1.7
-- matplotlib>=3.1
-- pandas>=1.1
-- scipy>=1.8
-- numba>=0.51
-
-To install the most important optional dependencies (solver LmFit and function visualisation Latexify) at the same time with Pastas use::
-
-   pip install pastas[full]
-
-or for the development version use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
-
-How to Cite Pastas?
-~~~~~~~~~~~~~~~~~~~
-If you use Pastas in one of your studies, please cite the Pastas article in Groundwater:
+> [!IMPORTANT]
+> As of Pastas 1.5, noisemodels are not added to the Pastas models by default anymore. [Read more about this change here](https://github.com/pastas/pastas/issues/735).
 
-- Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F. (2019) `Pastas: open source software for the analysis of groundwater time series <https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925>`_. Groundwater. doi: 10.1111/gwat.12925.
+![image](/doc/_static/logo_small.png)
+[![image](https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/pastas/pastas/actions/workflows/ci.yml)
+[![image](https://img.shields.io/pypi/v/pastas.svg)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/l/pastas.svg)](https://mit-license.org/)
+[![image](https://img.shields.io/pypi/pyversions/pastas)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/dm/pastas)](https://pypi.org/project/pastas/)
+[![image](https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg)](https://doi.org/10.5281/zenodo.1465866)
+[![image](https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![image](https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9)
+[![image](https://readthedocs.org/projects/pastas/badge/?version=latest)](https://pastas.readthedocs.io/en/latest/?badge=latest)
+[![image](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
 
-To cite a specific version of Python, you can use the DOI provided for each official release (>0.9.7) through Zenodo. Click on the link to get a specific version and DOI, depending on the Pastas version.
+## Pastas: what is it?
 
-- Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas: open-source software for time series analysis in hydrology (Version X.X.X). Zenodo. http://doi.org/10.5281/zenodo.1465866
+Pastas is an open source python package for processing, simulating and
+analyzing groundwater time series. The object oriented structure allows
+for the quick implementation of new model components. Time series models
+can be created, calibrated, and analysed with just a few lines of python
+code with the built-in optimization, visualisation, and statistical
+analysis tools.
 
+## Documentation & Examples
+
+-   Documentation is provided on the dedicated website
+    [pastas.dev](http://www.pastas.dev/)
+-   Examples can be found on the [examples directory on the
+    documentation
+    website](https://pastas.readthedocs.io/en/dev/examples/index.html)
+-   View and edit a working example notebook of a Pastas model in
+    [MyBinder](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
+-   A list of publications that use Pastas is available in a [dedicated
+    Zotero
+    group](https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list)
+
+## Get in Touch
+
+-   Questions on Pastas can be asked and answered on [Github
+    Discussions](https://github.com/pastas/pastas/discussions).
+-   Bugs, feature requests and other improvements can be posted as
+    [Github Issues](https://github.com/pastas/pastas/issues).
+-   Pull requests will only be accepted on the development branch (dev)
+    of this repository. Please take a look at the [developers
+    section](http://pastas.readthedocs.io/) on the documentation website
+    for more information on how to contribute to Pastas.
+
+## Quick installation guide
+
+To install Pastas, a working version of Python 3.9, 3.10, 3.11, or 3.12
+has to be installed on your computer. We recommend using the [Anaconda
+Distribution](https://www.continuum.io/downloads) as it includes most of
+the python package dependencies and the Jupyter Notebook software to run
+the notebooks. However, you are free to install any Python distribution
+you want.
+
+### Stable version
+
+To get the latest stable version, use:
+
+    pip install pastas
+
+### Update
+
+To update pastas, use:
+
+    pip install pastas --upgrade
+
+### Developers
+
+To get the latest development version, use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
+
+## Related packages
+
+-   [Pastastore](https://github.com/pastas/pastastore) is a Python
+    package for managing multiple timeseries and pastas models
+-   [Metran](https://github.com/pastas/metran) is a Python package to
+    perform multivariate timeseries analysis using a technique called
+    dynamic factor modelling.
+-   [Hydropandas](https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb)
+    can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
+-   [PyEt](https://github.com/phydrus/pyet) can be used to compute
+    potential evaporation from meteorological variables.
+
+## Dependencies
+
+Pastas depends on a number of Python packages, of which all of the
+necessary are automatically installed when using the pip install
+manager. To summarize, the dependencies necessary for a minimal function
+installation of Pastas
+
+-   numpy\>=1.7
+-   matplotlib\>=3.1
+-   pandas\>=1.1
+-   scipy\>=1.8
+-   numba\>=0.51
+
+To install the most important optional dependencies (solver LmFit and
+function visualisation Latexify) at the same time with Pastas use:
+
+    pip install pastas[full]
+
+or for the development version use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
+
+## How to Cite Pastas?
+
+If you use Pastas in one of your studies, please cite the Pastas article
+in Groundwater:
+
+-   Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F.
+    (2019) [Pastas: open source software for the analysis of groundwater
+    time
+    series](https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925).
+    Groundwater. doi: 10.1111/gwat.12925.
+
+To cite a specific version of Pastas, you can use the DOI provided for
+each official release (\>0.9.7) through Zenodo. Click on the link to get
+a specific version and DOI, depending on the Pastas version.
+
+-   Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas:
+    open-source software for time series analysis in hydrology (Version
+    X.X.X). Zenodo. <http://doi.org/10.5281/zenodo.1465866>
```

### Comparing `pastas-1.4.0/pastas/decorators.py` & `pastas-1.5.0/pastas/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,34 +14,33 @@
     USE_NUMBA = b
 
 
 def set_parameter(function: Function) -> Function:
     @wraps(function)
     def _set_parameter(self, name: str, value: float, **kwargs):
         if name not in self.parameters.index:
-            logger.error(
-                "Parameter name %s does not exist, please choose from %s",
-                name,
-                self.parameters.index,
-            )
+            msg = "Parameter name %s does not exist, please choose from %s"
+            logger.error(msg, name, self.parameters.index)
+            raise KeyError(msg % (name, self.parameters.index))
         else:
             return function(self, name, value, **kwargs)
 
     return _set_parameter
 
 
 def get_stressmodel(function: Function) -> Function:
     @wraps(function)
     def _get_stressmodel(self, name: str, **kwargs):
         if name not in self.stressmodels.keys():
-            logger.error(
+            msg = (
                 "The stressmodel name you provided is not in the stressmodels dict. "
-                "Please select from the following list: %s",
-                self.stressmodels.keys(),
+                "Please select from the following list: %s"
             )
+            logger.error(msg, self.stressmodels.keys())
+            raise KeyError(msg % self.stressmodels.keys())
         else:
             return function(self, name, **kwargs)
 
     return _get_stressmodel
 
 
 def model_tmin_tmax(function: Function) -> Function:
@@ -63,15 +62,15 @@
     return _model_tmin_tmax
 
 
 def PastasDeprecationWarning(function: Function) -> Function:
     @wraps(function)
     def _function(*args, **kwargs):
         logger.warning(
-            "Method is deprecated and will be removed in Pastas version 1.2."
+            "Method is deprecated since 1.5 and will be removed in Pastas version 1.6"
         )
         return function(*args, **kwargs)
 
     return _function
 
 
 def njit(function: Optional[Function] = None, parallel: bool = False) -> Function:
```

### Comparing `pastas-1.4.0/pastas/extensions/accessor.py` & `pastas-1.5.0/pastas/extensions/accessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # copied and adapted from pandas/core/accessor.py
-import warnings
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class CachedAccessor:
     """
     Custom property-like object.
 
     A descriptor for caching accessors.
@@ -80,20 +82,19 @@
             In [1]: from pastas.plotting.plotly import Plotly
             In [2]: ml = ps.Model(oseries)
             In [3]: ml.plotly.plot()  # plots interactive figure
     """
 
     def decorator(accessor):
         if hasattr(cls, name):
-            warnings.warn(
-                f"registration of accessor {repr(accessor)} under name "
-                f"{repr(name)} for type {repr(cls)} is overriding a preexisting "
-                "attribute with the same name.",
-                UserWarning,
+            msg = (
+                "registration of accessor %s under name %s for type %s is overriding"
+                " a preexisting attribute with the same name."
             )
+            logger.warning(msg, repr(accessor), repr(name), repr(cls))
         setattr(cls, name, CachedAccessor(name, accessor))
         cls._accessors.add(name)
         return accessor
 
     return decorator
```

### Comparing `pastas-1.4.0/pastas/io/base.py` & `pastas-1.5.0/pastas/io/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,32 +33,36 @@
     Examples
     --------
     >>> import pastas as ps
     >>> ml = ps.io.load("model.pas")
 
     """
     if not path.exists(fname):
-        logger.error("File not found: %s", fname)
+        msg = "File not found: %s"
+        logger.error(msg, fname)
+        raise FileNotFoundError(msg % fname)
 
     # Dynamic import of the export module
     load_mod = import_module(f"pastas.io{path.splitext(fname)[1]}")
 
     # Get dicts for all data sources
     data = load_mod.load(fname, **kwargs)
 
     file_version = data["file_info"]["pastas_version"]
 
     # A single catch for old pas-files, no longer supported
     if version.parse(file_version) < version.parse("0.23.0"):
-        raise UserWarning(
+        msg = (
             "This file was created with a Pastas version prior to 0.23 "
             "and cannot be loaded with Pastas >= 1.0. Please load and "
             "save the file with Pastas 0.23 first to update the file "
             "format."
         )
+        logger.error(msg)
+        raise ValueError(msg)
 
     ml = _load_model(data)
 
     logger.info(
         "Pastas Model from file %s successfully loaded. This file was created with "
         "Pastas %s. Your current version of Pastas is: %s",
         fname,
@@ -80,28 +84,27 @@
         constant = False
 
     if "name" in data.keys():
         name = data["name"]
     else:
         name = None
 
-    if "noisemodel" in data.keys():
-        noise = True
-    else:
-        noise = False
-
     ml = ps.Model(
         oseries=oseries,
         constant=constant,
-        noisemodel=noise,
         name=name,
         metadata=metadata,
     )
 
     if "settings" in data.keys():
+        if "noise" in data["settings"]:
+            if not data["settings"]["noise"] and "noisemodel" in data:
+                # file is saved before pastas 1.5, and solved with ml.solve(noise=False)
+                # remove noisemodel from data
+                data.pop("noisemodel")
         ml.settings.update(data["settings"])
     if "file_info" in data.keys():
         ml.file_info.update(data["file_info"])
 
     # Add stressmodels
     for name, smdata in data["stressmodels"].items():
         sm = _load_stressmodel(smdata, data)
@@ -111,14 +114,20 @@
     if "transform" in data.keys():
         transform = getattr(ps.transform, data["transform"].pop("class"))
         transform = transform(**data["transform"])
         ml.add_transform(transform)
 
     # Add noisemodel if present
     if "noisemodel" in data.keys():
+        # fixes to read pas-files from before pastas version 1.5
+        # TODO: uncomment in pastas 2.0.0
+        # if data["noisemodel"]["class"] == "NoiseModel":
+        #     data["noisemodel"]["class"] = "ArNoiseModel"
+        # if data["noisemodel"]["class"] == "ArmaModel":
+        #     data["noisemodel"]["class"] = "ArmaNoiseModel"
         n = getattr(ps.noisemodels, data["noisemodel"].pop("class"))()
         ml.add_noisemodel(n)
 
     # Add solver object to the model from pas-files < 1.3.0  TODO Deprecate
     if "fit" in data.keys():
         logger.warning(
             "The solver object is stored in the model.solver attribute since Pastas "
```

### Comparing `pastas-1.4.0/pastas/io/pas.py` & `pastas-1.5.0/pastas/io/pas.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 
 import datetime
 import json
 from collections import OrderedDict
 from io import StringIO as stringIO
 from logging import getLogger
 
+try:
+    from shapely.geometry.base import BaseGeometry
+
+    SHAPELY = True
+except ModuleNotFoundError:
+    SHAPELY = False
+    BaseGeometry = None
+
 from pandas import (
     DataFrame,
     Series,
     Timedelta,
     Timestamp,
     isna,
     read_json,
-    to_numeric,
     to_timedelta,
 )
 
 logger = getLogger(__name__)
 
 
 def load(fname: str) -> dict:
@@ -74,23 +81,25 @@
     -----
     Currently supported formats are: DataFrame, Series, Timedelta, Timestamps.
 
     see: https://docs.python.org/3/library/json.html
     """
 
     def default(self, o):
-        if isinstance(o, (Timestamp, datetime.datetime)):
+        if isinstance(o, (Timestamp, datetime.datetime, datetime.date)):
             return o.isoformat()
         elif isinstance(o, Series):
             return o.to_json(date_format="iso", orient="split")
         elif isinstance(o, DataFrame):
             # Necessary to maintain order when using the JSON format!
             # Do not use o.to_json() because of float precision
             return json.dumps(o.to_dict(orient="index"), indent=0)
         elif isinstance(o, (Timedelta, datetime.timedelta)):
             if isinstance(o, datetime.timedelta):
                 o = to_timedelta(o)
             return o.to_timedelta64().__str__()
+        elif SHAPELY and isinstance(o, BaseGeometry):
+            return o.wkt
         elif isna(o):
             return None
         else:
             return super(PastasEncoder, self).default(o)
```

### Comparing `pastas-1.4.0/pastas/model.py` & `pastas-1.5.0/pastas/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     date_range,
 )
 
 # Internal Pastas
 from pastas.decorators import get_stressmodel
 from pastas.io.base import _load_model, dump
 from pastas.modelstats import Statistics
-from pastas.noisemodels import NoiseModel
+from pastas.noisemodels import ArNoiseModel
 from pastas.plotting.modelplots import Plotting, _table_formatter_stderr
 from pastas.rfunc import HantushWellModel
 from pastas.solver import LeastSquares
 from pastas.stressmodels import Constant
 from pastas.timeseries import TimeSeries
 from pastas.timeseries_utils import (
     _frequency_is_supported,
@@ -55,16 +55,18 @@
     ----------
     oseries: pandas.Series
         pandas.Series object containing the dependent time series. The observation
         can be non-equidistant.
     constant: bool, optional
         Add a constant to the model (Default=True).
     noisemodel: bool, optional
-        Add the default noisemodel to the model. A custom noisemodel can be added
-        later in the modelling process as well.
+        The noisemodel argument is deprecated and will be removed in Pastas version
+        2.0.0. To add a noisemodel, use ml.add_noisemodel(n), where is an instance
+        of a noisemodel (e.g., n = ps.ArNoiseModel()). The use of the noisemodel
+        argument will raise a ValueError.
     name: str, optional
         String with the name of the model, used in plotting and saving.
     metadata: dict, optional
         Dictionary containing metadata of the oseries, passed on to the oseries when
         creating a pastas TimeSeries object. hence, ml.oseries.metadata will give you
         the metadata.
     freq: str, optional
@@ -87,15 +89,15 @@
 
     _accessors = set()
 
     def __init__(
         self,
         oseries: Series,
         constant: bool = True,
-        noisemodel: bool = True,
+        noisemodel=None,  # will be removed in version 2.0.0
         name: Optional[str] = None,
         metadata: Optional[dict] = None,
         freq: str = "D",
     ) -> None:
         # Construct the different model components
         self.oseries = TimeSeries(oseries, settings="oseries", metadata=metadata)
 
@@ -127,25 +129,44 @@
         # Default solve/simulation settings
         self.settings = {
             "tmin": None,
             "tmax": None,
             "freq": freq,
             "warmup": Timedelta(3650, "D"),
             "time_offset": Timedelta(0),
-            "noise": noisemodel,
+            "noise": False,
             "solver": None,
             "fit_constant": True,
             "freq_obs": None,
         }
 
         if constant:
             constant = Constant(initial=self.oseries.series.mean(), name="constant")
             self.add_constant(constant)
-        if noisemodel:
-            self.add_noisemodel(NoiseModel())
+
+        if noisemodel is not None:
+            if noisemodel is True:
+                msg = (
+                    "The noisemodel argument is deprecated and will be removed in Pastas "
+                    "version 2.0.0. The new default is that no noisemodel is added "
+                    "anymore and a noisemodel has to be added explicitly to a Pastas "
+                    "model by the user. To fix this error, do not pass a "
+                    "noisemodel keyword to Model and use `ml.add_noisemodel`, if a "
+                    "noisemodel is desired. See this issue on GitHub for more "
+                    "information: https://github.com/pastas/pastas/issues/735"
+                )
+            elif noisemodel is False:
+                msg = (
+                    "The noisemodel argument is deprecated and will be removed in Pastas "
+                    "version 2.0.0. The new default is that no noisemodel is added "
+                    "anymore, so passing noisemodel=False is not needed anymore. To "
+                    "fix this error, do not pass noisemodel=False to Model."
+                )
+            logger.error(msg)
+            raise ValueError(msg)
 
         # File Information
         self.file_info = self._get_file_info()
 
         # initialize some attributes for solving and simulation
         self.sim_index = None
         self.oseries_calib = None
@@ -208,18 +229,21 @@
         pastas.stressmodels
         """
         # Method can take multiple stressmodels at once through args
         if isinstance(stressmodel, list):
             for sm in stressmodel:
                 self.add_stressmodel(sm)
         elif (stressmodel.name in self.stressmodels.keys()) and not replace:
-            logger.error(
+            msg = (
                 "The name for the stressmodel you are trying to add already exists "
                 "for this model. Select another name."
             )
+            logger.error(msg)
+            raise ValueError(msg)
+
         else:
             if stressmodel.name in self.stressmodels.keys():
                 logger.warning(
                     "The name for the stressmodel you are trying to add already "
                     "exists for this model. The stressmodel is replaced."
                 )
             self.stressmodels[stressmodel.name] = stressmodel
@@ -280,26 +304,34 @@
         Parameters
         ----------
         noisemodel: pastas.noisemodels.NoiseModelBase
             Instance of NoiseModelBase.
 
         Examples
         --------
-        >>> n = ps.NoiseModel()
+        >>> n = ps.ArNoiseModel()
         >>> ml.add_noisemodel(n)
+
+        Notes
+        -----
+        As of Pastas version 1.5.0, a noisemodel should be added to the model using this
+        method, and is not added by default anymore when constructing as Pastas Model.
+        If a noisemodel is present, it will always be used during optimization.
+
         """
         self.noisemodel = noisemodel
         self.noisemodel.set_init_parameters(oseries=self.oseries.series)
 
         # check whether noise_alpha is not smaller than ml.settings["freq"]
         freq_in_days = _get_dt(self.settings["freq"])
         noise_alpha = self.noisemodel.parameters.initial.iloc[0]
         if freq_in_days > noise_alpha:
             self.noisemodel._set_initial("noise_alpha", freq_in_days)
 
+        self.settings["noise"] = True
         self.parameters = self.get_init_parameters(initial=False)
 
     @get_stressmodel
     def del_stressmodel(self, name: str):
         """Method to safely delete a stress model from the Model.
 
         Parameters
@@ -335,14 +367,15 @@
     def del_noisemodel(self) -> None:
         """Method to safely delete the noise model from the Model."""
         if self.noisemodel is None:
             logger.warning("No noisemodel is present in this model.")
         else:
             self.noisemodel = None
             self.parameters = self.get_init_parameters(initial=False)
+            self.settings["noise"] = False
 
     def simulate(
         self,
         p: Optional[ArrayLike] = None,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         freq: Optional[str] = None,
@@ -425,15 +458,14 @@
 
         # Respect provided tmin/tmax at this point, since warmup matters for
         # simulation but should not be returned, unless return_warmup=True.
         if not return_warmup:
             sim = sim.loc[tmin:tmax]
 
         if sim.hasnans:
-            sim = sim.dropna()
             msg = (
                 "Simulation contains NaN-values. Check if time series settings "
                 "are provided for each stress model "
                 "(e.g. `ps.StressModel(stress, settings='prec')`!"
             )
             logger.error(msg)
             raise ValueError(msg)
@@ -476,20 +508,24 @@
         # Default options when tmin, tmax, freq and warmup are not provided.
         if tmin is None:
             tmin = self.settings["tmin"]
         if tmax is None:
             tmax = self.settings["tmax"]
         if freq is None:
             freq = self.settings["freq"]
+        if self.settings["freq_obs"] is None:
+            freq_obs = freq
+        else:
+            freq_obs = self.settings["freq_obs"]
 
         # simulate model
         sim = self.simulate(p, tmin, tmax, freq, warmup, return_warmup=False)
 
         # Get the oseries calibration series
-        oseries_calib = self.observations(tmin, tmax, freq)
+        oseries_calib = self.observations(tmin, tmax, freq_obs)
 
         # Get simulation at the correct indices
         if self.interpolate_simulation is None:
             if oseries_calib.index.difference(sim.index).size != 0:
                 self.interpolate_simulation = True
                 logger.info(
                     "There are observations between the simulation time steps. Linear "
@@ -558,15 +594,15 @@
             literature.
 
         Warnings
         --------
         This method returns None if no noise model is present in the model.
         """
         if self.noisemodel is None or self.settings["noise"] is False:
-            logger.error(
+            logger.warning(
                 "Noise cannot be calculated if there is no noisemodel present or is "
                 "not used during parameter estimation."
             )
             return None
 
         # Get parameters if none are provided
         if p is None:
@@ -680,24 +716,29 @@
         freq_obs: Optional[str] = None,
     ) -> None:
         """Method to initialize the model.
 
         This method is called by the solve-method, but can also be triggered
         manually. See the solve-method for a description of the arguments.
         """
-        if noise is None and self.noisemodel:
-            noise = True
-        elif noise is True and self.noisemodel is None:
-            logger.warning(
-                "Warning, solving with noise=True while no noisemodel is present. "
-                "noise set to False."
+
+        if noise is not None:
+            msg = (
+                "The noise argument is deprecated and will be removed in Pastas "
+                "version 2.0.0. The new behavior is that a noise model will always be "
+                "used if it is present. To add a noisemodel to a model called ml, "
+                "use the ml.add_noisemodel method. To solve without a noisemodel, "
+                "make sure sure no noisemodel is added or remove a noisemodel with "
+                "ml.del_noisemodel() before solving. See this issue on GitHub for "
+                "more information: https://github.com/pastas/pastas/issues/735"
             )
-            noise = False
+            logger.error(msg)
+            raise ValueError(msg)
 
-        self.settings["noise"] = noise
+        # Set the settings
         self.settings["weights"] = weights
         self.settings["fit_constant"] = fit_constant
         self.settings["freq_obs"] = freq_obs
 
         # Set the frequency & warmup
         if freq:
             self.settings["freq"] = _frequency_is_supported(freq)
@@ -728,26 +769,27 @@
         # Initialize parameters
         self.parameters = self.get_init_parameters(noise, initial)
 
         # Prepare model if not fitting the constant as a parameter
         if self.settings["fit_constant"] is False:
             if self.transform is not None:
                 msg = "fit_constant needs to be True (for now) when a transform is used"
+                logger.error(msg)
                 raise Exception(msg)
             self.parameters.loc["constant_d", "vary"] = False
             self.parameters.loc["constant_d", "initial"] = 0.0
             self.normalize_residuals = True
 
     def solve(
         self,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         freq: Optional[str] = None,
         warmup: Optional[float] = None,
-        noise: bool = True,
+        noise=None,  # will be removed in version 2.0.0
         solver: Optional[Solver] = None,
         report: bool = True,
         initial: bool = True,
         weights: Optional[Series] = None,
         fit_constant: bool = True,
         freq_obs: Optional[str] = None,
         **kwargs,
@@ -765,16 +807,19 @@
         freq: str, optional
             String with the frequency the stressmodels are simulated. Must be one of
             the following (D, h, m, s, ms, us, ns) or a multiple of that e.g. "7D".
         warmup: float, optional
             Warmup period (in Days) for which the simulation is calculated, but not
             used for the calibration period.
         noise: bool, optional
-            Argument that determines if a noisemodel is used (only if present). The
-            default is noise=True.
+            This argument is deprecated and will be removed in Pastas version 2.0.0.
+            To solve using a noisemodel (i.e. noise=True), add a noisemodel to the
+            model using ml.add_noisemodel(n), where n is an instance of a noisemodel
+            (e.g., n = ps.ArNoiseModel()). To solve without a noisemodel (noise=False),
+            remove the noisemodel first (if present) using ml.del_noisemodel().
         solver: Class pastas.solver.Solver, optional
             Instance of a pastas Solver class used to solve the model. Options are:
             ps.LeastSquares() (default) or ps.LmfitSolve(). An instance is needed as
             of Pastas 0.23, not a class!
         report: bool, optional
             Print a report to the screen after optimization finished. This can also
             be manually triggered after optimization by calling print(ml.fit_report(
@@ -807,24 +852,51 @@
           specific results are stored in ml.solver.result and can be accessed from there.
 
         See Also
         --------
         pastas.solver
             Different solver objects are available to estimate parameters.
         """
+        if noise is not None:
+            if noise is True:
+                msg = (
+                    "The noise argument is deprecated and will be removed in Pastas "
+                    "version 2.0.0. To solve using a noisemodel, add a noisemodel to a "
+                    "model called ml using ml.add_noisemodel(n), where n is an instance "
+                    "of a noisemodel (e.g., n = ps.ArNoiseModel()). See this issue on "
+                    "GitHub for more information: "
+                    "https://github.com/pastas/pastas/issues/735"
+                )
+            elif noise is False:
+                msg = (
+                    "The noise argument is deprecated and will be removed in Pastas "
+                    "version 2.0.0. To solve without a noisemodel, remove the noisemodel "
+                    "(if present) from a model called ml using ml.del_noisemodel() before "
+                    "solving. See this issue on GitHub for more information: "
+                    "https://github.com/pastas/pastas/issues/735"
+                )
+            logger.error(msg)
+            raise ValueError(msg)
 
         # Initialize the model
         self.initialize(
-            tmin, tmax, freq, warmup, noise, weights, initial, fit_constant, freq_obs
+            tmin=tmin,
+            tmax=tmax,
+            freq=freq,
+            warmup=warmup,
+            weights=weights,
+            initial=initial,
+            fit_constant=fit_constant,
+            freq_obs=freq_obs,
         )
 
         if self.oseries_calib.empty:
-            raise ValueError(
-                "Calibration series 'oseries_calib' is empty! Check 'tmin' or 'tmax'."
-            )
+            msg = "Calibration series 'oseries_calib' is empty! Check 'tmin' or 'tmax'."
+            logger.error(msg)
+            raise ValueError(msg)
 
         # If a solver is provided, use that one
         if solver is not None:
             self.solver = solver
             self.solver.set_model(self)
         # Create the default solver if None is provided or already present
         elif self.solver is None:
@@ -847,19 +919,18 @@
             optimal[self.parameters.name == self.constant.name] = res
 
         self.parameters.optimal = optimal
         self.parameters.stderr = stderr
         self._solve_success = success  # store for fit_report
 
         if report:
-            if isinstance(report, str):
-                output = report
+            if isinstance(report, str) and report == "full":
+                print(self.fit_report(corr=True, stderr=True))
             else:
-                output = None
-            print(self.fit_report(output=output))
+                print(self.fit_report())
 
     @property
     def fit(self):
         """Deprecated attribute, use ml.solver instead."""
         msg = (
             "Attribute 'fit' is deprecated and will be removed in a future version. "
             "Use 'solver' instead."
@@ -911,15 +982,15 @@
         It is highly recommended to use this method to set parameter properties.
         Changing the parameter properties directly in the parameter `DataFrame` may
         not work as expected.
         """
         if name not in self.parameters.index:
             msg = "parameter %s is not present in the model"
             logger.error(msg, name)
-            raise KeyError(msg, name)
+            raise KeyError(msg % name)
 
         # Because either of the following is not necessarily present
         noisemodel = self.noisemodel.name if self.noisemodel else "NotPresent"
         constant = self.constant.name if self.constant else "NotPresent"
         transform = self.transform.name if self.transform else "NotPresent"
 
         # Get the model component for the parameter
@@ -933,17 +1004,18 @@
             obj = self.constant
         elif cat == transform:
             obj = self.transform
 
         # Move pmin and pmax based on the initial
         if move_bounds and initial:
             if pmin or pmax:
-                raise KeyError(
-                    "Either pmin/pmax or move_bounds must be provided, but not both."
-                )
+                msg = "Either pmin/pmax or move_bounds must be provided, but not both."
+                logger.error(msg)
+                raise KeyError(msg)
+
             factor = initial / self.parameters.loc[name, "initial"]
             pmin = self.parameters.loc[name, "pmin"] * factor
             pmax = self.parameters.loc[name, "pmax"] * factor
 
         # Set the parameter properties
         if initial is not None:
             obj._set_initial(name, initial)
@@ -985,15 +1057,15 @@
                     base = t.min().ceil(freq)
                     mask = t >= base
                     if np.any(mask):
                         time_offsets.add(_get_time_offset(t[mask][0], freq))
         if len(time_offsets) > 1:
             msg = "The time-offset with the frequency is not the same for all stresses."
             logger.error(msg)
-            raise (Exception(msg))
+            raise Exception(msg)
         if len(time_offsets) == 1:
             return next(iter(time_offsets))
         else:
             return Timedelta(0)
 
     def _get_sim_index(
         self,
@@ -1457,24 +1529,25 @@
         df = [obs, sim, res, noise]
 
         if add_contributions:
             contribs = self.get_contributions(tmin=tmin, tmax=tmax, split=split)
             for contrib in contribs:
                 df.append(contrib)
 
-        df = concat(df, axis=1)
+        df = concat(df, axis=1, sort=True)
         return df
 
     def _get_response(
         self,
         block_or_step: str,
         name: str,
         p: Optional[ArrayLike] = None,
         dt: Optional[float] = None,
         add_0: bool = False,
+        istress: Optional[int] = None,
         **kwargs,
     ) -> Union[Series, None]:
         """Internal method to compute the block and step response.
 
         Parameters
         ----------
         block_or_step: str
@@ -1484,14 +1557,17 @@
         p : array_like, optional
             array_like object with the values as floats representing the model
             parameters. See Model.get_parameters() for more info if parameters is None.
         dt: float, optional
             timestep for the response function.
         add_0: bool, optional
             Add a zero at t=0.
+        istress: int, optional
+            When multiple stresses are present in a stressmodel, this keyword can be
+            used to obtain the respone to an individual stress.
         kwargs: dict: passed to rfunc.step() or rfunc.block()
 
         Returns
         -------
         response: pandas.Series or None
             Pandas.Series with the response, None if not present.
         """
@@ -1502,14 +1578,17 @@
             block_or_step = getattr(self.stressmodels[name].rfunc, block_or_step)
 
         if p is None:
             p = self.get_parameters(name)
 
         if dt is None:
             dt = _get_dt(self.settings["freq"])
+        if istress is not None and self.stressmodels[name].get_nsplit() > 1:
+            p = self.stressmodels[name].get_parameters(model=self, istress=istress)
+
         response = block_or_step(p, dt, **kwargs)
 
         if add_0:
             if isinstance(dt, np.ndarray):
                 t = dt
             else:
                 t = np.linspace(0, response.size * dt, response.size + 1)
@@ -1545,15 +1624,16 @@
         p: array_like, optional
             array_like object with the values as floats representing the model
             parameters. See Model.get_parameters() for more info if parameters is None.
         add_0: bool, optional
             Adds 0 at t=0 at the start of the response, defaults to False.
         dt: float, optional
             timestep for the response function.
-        kwargs: dict
+        kwargs: dict, optional
+            Kwargs are passed onto _get_response()
 
         Returns
         -------
         b: pandas.Series or None
             Pandas.Series with the block response. The index is based on the
             frequency that is present in the model.settings.
         """
@@ -1581,14 +1661,16 @@
         p: array_like, optional
             array_like object with the values as floats representing the model
             parameters. See Model.get_parameters() for more info if parameters is None.
         add_0: bool, optional
             Adds 0 at t=0 at the start of the response, defaults to False.
         dt: float, optional
             timestep for the response function.
+        kwargs: dict, optional
+            Kwargs are passed onto _get_response()
 
         Returns
         -------
         s: pandas.Series or None
             Pandas.Series with the step response. The index is based on the frequency
             that is present in the model.settings.
         """
@@ -1741,27 +1823,36 @@
         except:
             file_info["owner"] = "Unknown"
 
         return file_info
 
     def fit_report(
         self,
-        output: str = "basic",
+        corr: bool = False,
+        stderr: bool = False,
         warnings: bool = True,
+        output: str = None,
     ) -> str:
         """Method that reports on the fit after a model is optimized.
 
         Parameters
         ----------
-        output: str, optional
-            If any other value than "full" is provided, the parameter correlations
-            will be removed from the output.
+        corr : bool, optional
+            If True the parameter correlations are shown.
+        stderr : bool, optional
+            If True the standard error of the parameter values are shown. Please be
+            aware of the conditions for reliable uncertainty estimates, more information
+            here:
+            https://pastas.readthedocs.io/en/master/examples/diagnostic_checking.html
         warnings : bool, optional
             print warnings in case of optimization failure, parameters hitting
             bounds, or length of responses exceeding calibration period.
+        output : str, optional (deprecated)
+            deprecated argument, use corr and stderr arguments
+            instead.
 
         Returns
         -------
         report: str
             String with the report.
 
         Examples
@@ -1788,29 +1879,50 @@
             "solver": self.settings["solver"],
         }
 
         fit = {
             "EVP": f"{self.stats.evp():.2f}",
             "R2": f"{self.stats.rsq():.2f}",
             "RMSE": f"{self.stats.rmse():.2f}",
-            "AIC": f"{self.stats.aic():.2f}",
+            "AICc": f"{self.stats.aicc():.2f}",
             "BIC": f"{self.stats.bic():.2f}",
             "Obj": f"{self.solver.obj_func:.2f}",
             "___": "",
             "Interp.": "Yes" if self.interpolate_simulation else "No",
         }
 
+        if output is not None:
+            msg = (
+                "argument 'output' of the 'fit_report method' is deprecated and will"
+                "be removed in a future version. Use 'corr=True' instead."
+            )
+            logger.warning(msg)
+            if isinstance(output, str) and output == "full":
+                corr = True
+
         parameters = self.parameters.loc[:, ["optimal", "initial", "vary"]].copy()
-        stderr = self.parameters.loc[:, "stderr"] / self.parameters.loc[:, "optimal"]
-        parameters.loc[:, "stderr"] = stderr.abs().apply(
-            _table_formatter_stderr, na_rep="nan"
-        )
 
-        # Determine the width of the fit_report based on the parameters
-        width = len(parameters.to_string().split("\n")[1])
+        if stderr:
+            stderr = (
+                self.parameters.loc[:, "stderr"] / self.parameters.loc[:, "optimal"]
+            )
+            parameters.loc[:, "stderr"] = stderr.abs().apply(
+                _table_formatter_stderr, na_rep="nan"
+            )
+
+        # determine width of the fit_report
+        len_fit = max([len(v) for v in fit.values()]) + max(
+            [len(v) for v in fit.keys()]
+        )
+        len_model = max([len(v) for v in model.values() if isinstance(v, str)]) + max(
+            [len(v) for v in model.keys()]
+        )
+        len_param = len(parameters.to_string().split("\n")[1])
+        width = max((len_fit + len_model + 8), len_param)
+        string = "{:{fill}{align}{width}}"
         string = "{:{fill}{align}{width}}"
 
         # Create the first header with model information and stats
         wspace = max(width - (11 + 14 + len(self.name)), 1)
         mspace = width - wspace - (11 + 14)
         header = (
             f"Fit report {self.name:<{mspace}.{mspace}}"
@@ -1828,15 +1940,15 @@
         # Create the parameters block
         params = (
             f"\nParameters ({parameters.vary.sum()} optimized)\n"
             f"{string.format('', fill='=', align='>', width=width)}\n"
             f"{parameters.to_string()}"
         )
 
-        if output == "full":
+        if corr:
             cor = DataFrame(columns=["value"])
             for idx, col in combinations(self.solver.pcor, 2):
                 if np.abs(self.solver.pcor.loc[idx, col]) > 0.5:
                     cor.loc[f"{idx} {col}"] = self.solver.pcor.loc[idx, col]
 
             corr = (
                 f"\n\nParameter correlations |rho| > 0.5\n"
```

### Comparing `pastas-1.4.0/pastas/modelstats.py` & `pastas-1.5.0/pastas/modelstats.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,16 +40,18 @@
         "rmse",
         "rmsn",
         "sse",
         "mae",
         "nse",
         "evp",
         "rsq",
+        "kge",
         "bic",
         "aic",
+        "aicc",
     ]
 
     def __init__(self, ml: Model):
         """This class provides statistics to pastas Model class.
 
         Parameters
         ----------
@@ -63,15 +65,15 @@
         >>> print(ml.stats.ops)
         """
         # Save a reference to the model.
         self.ml = ml
 
     def __repr__(self):
         msg = """This module contains all the statistical functions included in Pastas.
-        
+
         To obtain a list of all statistics that are included type:
 
     >>> print(ml.stats.ops)"""
         return msg
 
     @model_tmin_tmax
     def rmse(
@@ -275,14 +277,45 @@
         pastas.stats.rsq
         """
         obs = self.ml.observations(tmin=tmin, tmax=tmax)
         res = self.ml.residuals(tmin=tmin, tmax=tmax)
         return metrics.rsq(obs=obs, res=res, weighted=weighted, **kwargs)
 
     @model_tmin_tmax
+    def kge(
+        self,
+        tmin: Optional[TimestampType] = None,
+        tmax: Optional[TimestampType] = None,
+        weighted: bool = False,
+        modified: bool = False,
+        **kwargs,
+    ) -> float:
+        """Kling-Gupta Efficiency.
+
+        Parameters
+        ----------
+        tmin: str or pandas.Timestamp, optional
+        tmax: str or pandas.Timestamp, optional
+        weighted: bool, optional
+            If weighted is True, the variances are computed using the time step
+            between observations as weights. Default is False.
+        modified: bool, optional
+            Use the modified KGE as proposed by :cite:t:`kling_runoff_2012`.
+
+        See Also
+        --------
+        pastas.stats.kge
+        """
+        sim = self.ml.simulate(tmin=tmin, tmax=tmax)
+        obs = self.ml.observations(tmin=tmin, tmax=tmax)
+        return metrics.kge(
+            obs=obs, sim=sim, weighted=weighted, modified=modified, **kwargs
+        )
+
+    @model_tmin_tmax
     def kge_2012(
         self,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         weighted: bool = False,
         **kwargs,
     ) -> float:
@@ -338,26 +371,50 @@
         Parameters
         ----------
         tmin: str or pandas.Timestamp, optional
         tmax: str or pandas.Timestamp, optional
 
         See Also
         --------
-        pastas.stats.bic
+        pastas.stats.aic
         """
         nparam = self.ml.parameters["vary"].sum()
         if self.ml.settings["noise"]:
             res = self.ml.noise(tmin=tmin, tmax=tmax) * self.ml.noise_weights(
                 tmin=tmin, tmax=tmax
             )
         else:
             res = self.ml.residuals(tmin=tmin, tmax=tmax)
         return metrics.aic(res=res, nparam=nparam)
 
     @model_tmin_tmax
+    def aicc(
+        self, tmin: Optional[TimestampType] = None, tmax: Optional[TimestampType] = None
+    ) -> float:
+        """Akaike Information Criterium with second order bias correction (AICc).
+
+        Parameters
+        ----------
+        tmin: str or pandas.Timestamp, optional
+        tmax: str or pandas.Timestamp, optional
+
+        See Also
+        --------
+        pastas.stats.aicc
+        """
+        nparam = self.ml.parameters["vary"].sum()
+        if self.ml.settings["noise"]:
+            res = self.ml.noise(tmin=tmin, tmax=tmax) * self.ml.noise_weights(
+                tmin=tmin, tmax=tmax
+            )
+        else:
+            res = self.ml.residuals(tmin=tmin, tmax=tmax)
+        return metrics.aicc(res=res, nparam=nparam)
+
+    @model_tmin_tmax
     def summary(
         self,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         stats: Optional[List[str]] = None,
     ) -> DataFrame:
         """Returns a Pandas DataFrame with goodness-of-fit metrics.
```

### Comparing `pastas-1.4.0/pastas/noisemodels.py` & `pastas-1.5.0/pastas/noisemodels.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 better represents white noise.
 
 Examples
 --------
 By default, a noise model is added to a Pastas model. It is possible to replace the
 default model with different models as follows:
 
->>> n = ps.ArmaModel()
+>>> n = ps.ArmaNoiseModel()
 >>> ml.add_noisemodel(n)
 
 or, to delete the noise model from the model:
 
 >>> ml.del_noisemodel()
 
 See Also
 --------
 pastas.model.Model.add_noisemodel
 """
 
-# Type Hinting
+from logging import getLogger
 from typing import Optional
 
 import numpy as np
-from pandas import DataFrame, Series, Timedelta
+from pandas import DataFrame, DatetimeIndex, Series, Timedelta
 
 from pastas.typing import ArrayLike
 
 from .decorators import njit, set_parameter
 
-__all__ = ["NoiseModel", "ArmaModel"]
+logger = getLogger(__name__)
+
+__all__ = ["ArNoiseModel", "ArmaNoiseModel"]
 
 
 class NoiseModelBase:
     _name = "NoiseModelBase"
 
     def __init__(self) -> None:
         self.nparam = 1
@@ -115,15 +117,15 @@
         return data
 
     @staticmethod
     def weights(res, p) -> int:
         return 1
 
 
-class NoiseModel(NoiseModelBase):
+class ArNoiseModel(NoiseModelBase):
     """Noise model with exponential decay of the residuals and weighting.
 
     Parameters
     ----------
     norm: boolean, optional
         Boolean to indicate whether weights are normalized according to the Von
         Asmuth and Bierkens (2005) paper. Default is True.
@@ -139,20 +141,20 @@
     Calculates the weights as
 
     .. math::
 
         w = 1 / \\sqrt{(1 - \\exp(-2 \\Delta t / \\alpha))}
 
     The units of the alpha parameter is always in days. The first value of the noise
-    is the residual ($v(t=0=r(t=0)$). First weight is 1 / sig_residuals (i.e.,
+    is the residual (:math:`v(t=0=r(t=0)`). First weight is 1 / sig_residuals (i.e.,
     delt = infty). Normalization of weights as in :cite:t:`von_asmuth_modeling_2005`,
     optional.
     """
 
-    _name = "NoiseModel"
+    _name = "ArNoiseModel"
 
     def __init__(self, norm: bool = True) -> None:
         NoiseModelBase.__init__(self)
         self.norm = norm
         self.nparam = 1
         self.set_init_parameters()
 
@@ -209,41 +211,94 @@
         odelt = np.append(1e12, np.diff(res.index.to_numpy()) / Timedelta("1D"))
         exp = np.exp(-2.0 / alpha * odelt)  # Twice as fast as 2*odelt/alpha
         w = 1 / np.sqrt(1.0 - exp)  # weights of noise, not noise^2
         if self.norm:
             w *= np.exp(1.0 / (2.0 * odelt.size) * np.sum(np.log(1.0 - exp)))
         return Series(data=w, index=res.index, name="noise_weights")
 
+    def get_correction(
+        self, res: Series, p: ArrayLike, tindex: DatetimeIndex
+    ) -> Series:
+        """Get the correction for a forecast using the noise model.
+
+        Parameters
+        ----------
+        res : Series
+            The residual series.
+        p : ArrayLike
+            The parameters of the noise model.
+        tindex : DatetimeIndex
+            The index of the forecast.
+
+        Returns
+        -------
+        Series
+            The correction to the forecast.
+
+        Notes
+        -----
+        The correction is calculated as:
+
+        .. math::
+
+                correction = \\exp(-\\Delta t / \\alpha) * last_residual
+
+        where :math:`\\Delta t` is the time difference between the last observation
+        and the forecast, and :math:`\\alpha` is the noise parameter.
+
+        """
+        alpha = p[0]
+        last_residual = res.iloc[-1]
+        last_date = res.index[-1]
+        dt = (tindex - last_date).days
+        correction = Series(
+            index=tindex,
+            name="correction",
+            dtype=float,
+            data=np.exp(-dt / alpha) * last_residual,
+        )
+        return correction
+
     def to_dict(self) -> dict:
         """Method to return a dict to store the noise model"""
         data = {"class": self._name, "norm": self.norm}
         return data
 
 
-class ArmaModel(NoiseModelBase):
+def NoiseModel(*args, **kwargs) -> ArNoiseModel:
+    logger.warning(
+        "NoiseModel has been renamed to ArNoiseModel and will be deprecated in Pastas "
+        "version 2.0. Please use ArNoiseModel."
+    )
+    n = ArNoiseModel(*args, **kwargs)
+    n._name = "NoiseModel"
+    return n
+
+
+class ArmaNoiseModel(NoiseModelBase):
     """ARMA(1,1) Noise model to simulate the noise as defined in
-        :cite:t:`collenteur_estimation_2021`.
+    :cite:t:`collenteur_estimation_2021`.
 
-        Notes
-        -----
-        Calculates the noise according to:
-    F
-        .. math::
-            \\upsilon_t = r_t - r_{t-1} e^{-\\Delta t/\\alpha} - \\upsilon_{t-1}
-            e^{-\\Delta t/\\beta}
+    Notes
+    -----
+    Calculates the noise according to:
 
-        The units of the alpha and beta parameters are always in days.
+    .. math::
+        \\upsilon_t = r_t - r_{t-1} e^{-\\Delta t/\\alpha} - \\upsilon_{t-1}
+        e^{-\\Delta t/\\beta}
 
-        Warnings
-        --------
-        This model has only been tested on regular time steps and should not be used for
-        irregular time steps yet.
+    The units of the alpha and beta parameters are always in days.
+
+    Warnings
+    --------
+    This model has only been tested on regular time steps and should not be used for
+    irregular time steps yet.
     """
 
-    _name = "ArmaModel"
+    _name = "ArmaNoiseModel"
 
     def __init__(self) -> None:
         NoiseModelBase.__init__(self)
         self.nparam = 2
         self.set_init_parameters()
 
     def set_init_parameters(self, oseries: Series = None) -> None:
@@ -296,7 +351,17 @@
         for i in range(1, res.size):
             a[i] = (
                 res[i]
                 - res[i - 1] * np.exp(-odelt[i - 1] / alpha)
                 - a[i - 1] * pm * np.exp(-odelt[i - 1] / np.abs(beta))
             )
         return a
+
+
+def ArmaModel(*args, **kwargs) -> ArmaNoiseModel:
+    logger.warning(
+        "ArmaModel has been renamed to ArmaNoiseModel and will be deprecated in Pastas "
+        "version 2.0. Please use ArmaNoiseModel."
+    )
+    n = ArmaNoiseModel(*args, **kwargs)
+    n._name = "ArmaModel"
+    return n
```

### Comparing `pastas-1.4.0/pastas/objective_functions.py` & `pastas-1.5.0/pastas/objective_functions.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/plotting/modelcompare.py` & `pastas-1.5.0/pastas/plotting/modelcompare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains tools for visually comparing multiple models.
 """
 
 from itertools import combinations
 from logging import getLogger
-from typing import List, Optional, Tuple
+from typing import List, Optional
 from warnings import warn
 
 import matplotlib.pyplot as plt
 import numpy as np
 from pandas import DataFrame, concat
 
 from pastas.plotting.plotutil import _table_formatter_params, share_xaxes, share_yaxes
@@ -88,17 +88,17 @@
         self.cmap = None
         self.adjust_height = False
         self.smdict = None
 
     def initialize_figure(
         self,
         mosaic: Optional[List[List[str]]] = None,
-        figsize: Tuple[int, int] = (10, 8),
         cmap: str = "tab10",
         return_ax: bool = False,
+        **fig_kwargs,
     ) -> None:
         """initialize a custom figure based on a mosaic.
 
         Parameters
         ----------
         mosaic : list, optional
             subplot mosaic, by default None which uses the default mosaic.
@@ -108,28 +108,28 @@
             colormap, by default "tab10".
         """
         if mosaic is None:
             mosaic = self.get_default_mosaic()
 
         self.cmap = plt.get_cmap(cmap)
 
-        figure, axes = plt.subplot_mosaic(mosaic, figsize=figsize)
+        figure, axes = plt.subplot_mosaic(mosaic, **fig_kwargs)
         if return_ax:
             return axes
 
         self.figure = figure
         self.axes = axes
         self.mosaic = mosaic
 
     def initialize_adjust_height_figure(
         self,
         mosaic: Optional[List[List[str]]] = None,
-        figsize: Tuple[int] = (10, 8),
         cmap: str = "tab10",
         smdict: Optional[dict] = None,
+        **fig_kwargs,
     ) -> None:
         """initialize subplots based on a mosaic with equal vertical scales.
 
         The height of each subplot is calculated based on the y-data limits in each
         subplot. This is calculation is performed on the first column of axes in the
         mosaic.
 
@@ -222,16 +222,16 @@
                 heights_list += [heights[ky] / hsum * hratio / nrows] * nrows
             else:  # use the ratio of mosaic
                 heights_list += [mosfrac[ky]]
 
         self.mosaic = mosaic
         fig, axes = plt.subplot_mosaic(
             self.mosaic,
-            figsize=figsize,
             gridspec_kw=dict(height_ratios=heights_list),
+            **fig_kwargs,
         )
 
         self.figure = fig
         self.axes = axes
         self.cmap = plt.get_cmap(cmap)
 
         # set ylimits to data limits for scaling properly
@@ -573,18 +573,22 @@
             for j, namlist in self.smdict.items():
                 for smn in namlist:
                     # skip if contribution not in model
                     if smn not in ml.stressmodels:
                         continue
                     if response == "step":
                         kwargs = {}
+                        p = None
                         if ml.stressmodels[smn].rfunc is not None:
                             if isinstance(ml.stressmodels[smn].rfunc, HantushWellModel):
                                 kwargs = {"warn": False}
-                        step = ml.get_step_response(smn, add_0=True, **kwargs)
+                                p = ml.stressmodels[smn].get_parameters(
+                                    model=ml, istress=0
+                                )
+                        step = ml.get_step_response(smn, p=p, add_0=True, **kwargs)
                         if step is None:
                             continue
                         if self.axes is None:
                             axs[axn.format(i=0)].plot(
                                 step.index,
                                 step.values,
                                 label=f"{smn}",
@@ -594,18 +598,22 @@
                                 step.index,
                                 step.values,
                                 label=f"{smn}",
                                 color=self.cmap(i),
                             )
                     elif response == "block":
                         kwargs = {}
+                        p = None
                         if ml.stressmodels[smn].rfunc is not None:
                             if isinstance(ml.stressmodels[smn].rfunc, HantushWellModel):
                                 kwargs = {"warn": False}
-                        block = ml.get_block_response(smn, **kwargs)
+                                p = ml.stressmodels[smn].get_parameters(
+                                    model=ml, istress=0
+                                )
+                        block = ml.get_block_response(smn, p=p, add_0=True, **kwargs)
                         if block is None:
                             continue
                         if self.axes is None:
                             axs[axn.format(i=0)].semilogx(
                                 block.index,
                                 block.values,
                                 label=f"{smn}",
@@ -830,25 +838,26 @@
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot table on, by default "met"
         metric_selection : list, optional
             list of str describing which metrics to include, by default None which
-            uses ["rsq", "aic"].
+            uses ["rsq", "aicc"].
         """
         if metric_selection is None:
-            metric_selection = ["rsq", "aic"]
+            metric_selection = ["rsq", "aicc"]
 
         metrics = self.get_metrics(self.models, metric_selection=metric_selection)
-        for met in ["aic", "bic"]:
+        for met in ["aic", "aicc", "bic"]:
             if met in metrics.index:
                 metrics.loc[met] -= metrics.loc[met].min()
+                metname = "AICc" if met == "aicc" else met.upper()
                 metrics = metrics.rename(
-                    index={met: f"\N{GREEK CAPITAL LETTER DELTA}{met.upper()}"}
+                    index={met: f"\N{GREEK CAPITAL LETTER DELTA}{metname}"}
                 )
         if "rsq" in metrics.index:
             metrics = metrics.rename(index={"rsq": "R\N{SUPERSCRIPT TWO}"})
 
         # add seperate column with parameter names
         metrics.loc[:, "Metrics"] = metrics.index
         cols = metrics.columns.to_list()[-1:] + metrics.columns.to_list()[:-1]
@@ -893,19 +902,19 @@
         share_yaxes(axes)
 
     def plot(
         self,
         smdict: Optional[dict] = None,
         normalized: bool = False,
         param_selection: Optional[list] = None,
-        figsize: Optional[tuple] = (10, 8),
         grid: bool = True,
         legend: bool = True,
         adjust_height: bool = False,
         legend_kwargs: Optional[dict] = None,
+        **fig_kwargs,
     ) -> None:
         """plot the models in a comparison plot.
 
         The resulting plot is similar to `ml.plots.results()`.
 
         Parameters
         ----------
@@ -917,32 +926,32 @@
             second. By default, None, which creates a separate subplot for each
             stressmodel.
         normalized : bool, optional
             normalize contributions such that minimum or maximum value is equal to
             zero, by default False.
         param_selection : list, optional
             list of (sub)strings of which parameters to show in table, by default None.
-        figsize : tuple, optional
-            figure size, by default (10, 8).
         grid : bool, optional
             grid in each subplot, by default True.
         legend : bool, optional
             add legend in each subplot, by default True.
         adjust_height : bool, optional
             adjust the height of the graphs, so that the vertical scale of all the
             subplots on the left is equal. Default is False. When combining stress
             contributions in one subplot, please also provide smdict for best results.
         legend_kwargs : dict, optional
             pass legend keyword arguments to plots.
         """
         self.adjust_height = adjust_height
+        if "figsize" not in fig_kwargs:
+            fig_kwargs["figsize"] = (10, 8)
         if self.axes is None and not self.adjust_height:
-            self.initialize_figure(figsize=figsize)
+            self.initialize_figure(**fig_kwargs)
         if self.axes is None and self.adjust_height:
-            self.initialize_adjust_height_figure(smdict=smdict, figsize=figsize)
+            self.initialize_adjust_height_figure(smdict=smdict, **fig_kwargs)
 
         # sim
         _ = self.plot_oseries()
         _ = self.plot_simulation()
 
         # res
         _ = self.plot_residuals()
```

### Comparing `pastas-1.4.0/pastas/plotting/modelplots.py` & `pastas-1.5.0/pastas/plotting/modelplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""This module contains all the plotting methods for Pastas Models."""
+"""This module contains plotting methods for Pastas Models."""
 
 import logging
 
 # Type Hinting
 from typing import Dict, List, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.ticker import LogFormatter, MultipleLocator
 from pandas import Series, Timestamp, concat
 
-from pastas.decorators import model_tmin_tmax
+from pastas.decorators import PastasDeprecationWarning, model_tmin_tmax
 from pastas.plotting.plots import cum_frequency, diagnostics, pairplot, series
 from pastas.plotting.plotutil import (
     _get_height_ratios,
     _get_stress_series,
     _table_formatter_params,
     _table_formatter_stderr,
 )
@@ -94,27 +94,26 @@
             if not o_nu.empty:
                 # plot parts of the oseries that are not used in grey
                 o_nu.plot(linestyle="", marker=".", color="0.5", label="", ax=ax)
             o.plot(linestyle="", marker=".", color="k", ax=ax)
 
         if simulation:
             sim = self.ml.simulate(tmin=tmin, tmax=tmax)
-            r2 = round(self.ml.stats.rsq(tmin=tmin, tmax=tmax) * 100, 1)
-            sim.plot(ax=ax, label=f"{sim.name} ($R^2$ = {r2}%)")
+            r2 = self.ml.stats.rsq(tmin=tmin, tmax=tmax)
+            sim.plot(ax=ax, label=f"{sim.name} ($R^2$={r2:.2%})")
 
         # Dress up the plot
         # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
         if tmin is not None:
             tmin = Timestamp(tmin)
         if tmax is not None:
             tmax = Timestamp(tmax)
 
         ax.set_xlim(tmin, tmax)
-        ax.set_ylabel("Groundwater levels [meter]")
-        ax.set_title("Results of {}".format(self.ml.name))
+        ax.set_ylabel("Head")
 
         if legend:
             ax.legend(ncol=2, numpoints=3)
         plt.tight_layout()
         return ax
 
     @model_tmin_tmax
@@ -123,14 +122,15 @@
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         figsize: tuple = (10, 8),
         split: bool = False,
         adjust_height: bool = True,
         return_warmup: bool = False,
         block_or_step: str = "step",
+        stderr: bool = False,
         fig: Optional[Figure] = None,
         **kwargs,
     ) -> Axes:
         """Plot different results in one window to get a quick overview.
 
         Parameters
         ----------
@@ -143,14 +143,19 @@
         adjust_height: bool, optional
             Adjust the height of the graphs, so that the vertical scale of all the
             subplots on the left is equal. Default is True.
         return_warmup: bool, optional
             Show the warmup-period. Default is false.
         block_or_step: str, optional
             Plot the block- or step-response on the right. Default is 'step'.
+        stderr : bool, optional
+            If True the standard error of the parameter values are shown. Please be
+            aware of the conditions for reliable uncertainty estimates, more
+            information here:
+            https://pastas.readthedocs.io/en/master/examples/diagnostic_checking.html
         fig: matplotib.Figure instance, optional
             Optionally provide a matplotib.Figure instance to plot onto.
         **kwargs: dict, optional
             Optional arguments, passed on to the matplotlib.pyplot.figure method.
 
         Returns
         -------
@@ -219,14 +224,15 @@
             )
 
         # add rsq to simulation
         r2 = self.ml.stats.rsq(tmin=tmin, tmax=tmax)
         sim.plot(ax=ax1, x_compat=True, label=f"{sim.name} ($R^2$={r2:.2%})")
         ax1.legend(loc=(0, 1), ncol=3, frameon=False, numpoints=3)
         ax1.set_ylim(ylims[0])
+        ax1.set_ylabel("Head")
 
         # Residuals and noise
         ax2 = fig.add_subplot(gs[1, 0], sharex=ax1)
         res.plot(ax=ax2, color="k", x_compat=True)
         if self.ml.settings["noise"] and self.ml.noisemodel:
             noise = self.ml.noise(tmin=tmin, tmax=tmax)
             noise.plot(ax=ax2, x_compat=True)
@@ -238,58 +244,50 @@
         rmax = 0  # tmax of the response
         axb = None
         i = 0
         for sm_name, sm in self.ml.stressmodels.items():
             # plot the contribution
             nsplit = sm.get_nsplit()
             if split and nsplit > 1:
-                for _ in range(nsplit):
+                for istress in range(nsplit):
                     ax = fig.add_subplot(gs[i + 2, 0], sharex=ax1)
                     contribs[i].plot(ax=ax, x_compat=True)
                     ax.legend(loc=(0, 1), ncol=3, frameon=False)
+                    ax.set_ylabel("Rise")
                     if adjust_height:
                         ax.set_ylim(ylims[i + 2])
+
                     i = i + 1
+
+                    # plot the response
+                    axb, rmin, rmax = self._plot_response_in_results(
+                        sm_name, block_or_step, rmin, rmax, axb, gs, i, istress=istress
+                    )
+
             else:
                 ax = fig.add_subplot(gs[i + 2, 0], sharex=ax1)
                 contribs[i].plot(ax=ax, x_compat=True)
                 title = [stress.name for stress in sm.stress]
                 if len(title) > 3:
                     title = title[:3] + ["..."]
                 ax.set_title(
                     f"Stresses: {title}",
                     loc="right",
                     fontsize=plt.rcParams["legend.fontsize"],
                 )
                 ax.legend(loc=(0, 1), ncol=3, frameon=False)
+                ax.set_ylabel("Rise")
                 if adjust_height:
                     ax.set_ylim(ylims[i + 2])
                 i = i + 1
 
-            # plot the step response
-            rkwargs = {}
-            if self.ml.stressmodels[sm_name].rfunc is not None:
-                if isinstance(self.ml.stressmodels[sm_name].rfunc, HantushWellModel):
-                    rkwargs = {"warn": False}
-            response = self.ml._get_response(
-                block_or_step=block_or_step, name=sm_name, add_0=True, **rkwargs
-            )
-
-            if response is not None:
-                rmax = max(rmax, response.index.max())
-                axb = fig.add_subplot(gs[i + 1, 1], sharex=axb)
-                response.plot(ax=axb)
-                if block_or_step == "block":
-                    title = "Block response"
-                    rmin = response.index[1]
-                    axb.set_xscale("log")
-                    axb.xaxis.set_major_formatter(LogFormatter())
-                else:
-                    title = "Step response"
-                axb.set_title(title, fontsize=plt.rcParams["legend.fontsize"])
+                # plot the response
+                axb, rmin, rmax = self._plot_response_in_results(
+                    sm_name, block_or_step, rmin, rmax, axb, gs, i
+                )
 
         if axb is not None:
             axb.set_xlim(rmin, rmax)
 
         # xlim sets minorticks back after plots:
         ax1.minorticks_off()
 
@@ -319,32 +317,67 @@
         ax3.set_title(
             f"Model Parameters ($n_c$={n_free})",
             loc="left",
             fontsize=plt.rcParams["legend.fontsize"],
         )
         p = self.ml.parameters.loc[:, ["name"]].copy()
         p.loc[:, "name"] = p.index
-        stderr = (
-            self.ml.parameters.loc[:, "stderr"] / self.ml.parameters.loc[:, "optimal"]
-        )
         p.loc[:, "optimal"] = self.ml.parameters.loc[:, "optimal"].apply(
             _table_formatter_params
         )
-        p.loc[:, "stderr"] = stderr.abs().apply(_table_formatter_stderr)
+        if stderr:
+            stderr = (
+                self.ml.parameters.loc[:, "stderr"]
+                / self.ml.parameters.loc[:, "optimal"]
+            )
+            p.loc[:, "stderr"] = stderr.abs().apply(_table_formatter_stderr)
 
         ax3.axis("off")
         ax3.table(
             bbox=(0.0, 0.0, 1.0, 1.0),
             cellText=p.values,
             colWidths=[0.5, 0.25, 0.25],
             colLabels=p.columns,
         )
 
         return fig.axes
 
+    def _plot_response_in_results(
+        self, sm_name, block_or_step, rmin, rmax, axb, gs, i, istress=None
+    ):
+        """Internal method to plot the response of a Stressmodel in the results-plot"""
+        rkwargs = {}
+        if self.ml.stressmodels[sm_name].rfunc is not None:
+            if isinstance(self.ml.stressmodels[sm_name].rfunc, HantushWellModel):
+                rkwargs = {"warn": False}
+                if istress is None:
+                    # show the response of the first well, which gives more information than istress = None
+                    istress = 0
+        response = self.ml._get_response(
+            block_or_step=block_or_step,
+            name=sm_name,
+            add_0=True,
+            istress=istress,
+            **rkwargs,
+        )
+
+        if response is not None:
+            rmax = max(rmax, response.index.max())
+            axb = gs.figure.add_subplot(gs[i + 1, 1], sharex=axb)
+            response.plot(ax=axb)
+            if block_or_step == "block":
+                title = "Block response"
+                rmin = response.index[1]
+                axb.set_xscale("log")
+                axb.xaxis.set_major_formatter(LogFormatter())
+            else:
+                title = "Step response"
+            axb.set_title(title, fontsize=plt.rcParams["legend.fontsize"])
+        return axb, rmin, rmax
+
     @model_tmin_tmax
     def decomposition(
         self,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         ytick_base: bool = True,
         split: bool = True,
@@ -459,20 +492,22 @@
             marker=".",
             color="k",
             label=o_label,
             markersize=3,
             ax=axes[0],
             x_compat=True,
         )
-        sim.plot(ax=axes[0], x_compat=True)
+
+        r2 = self.ml.stats.rsq(tmin=tmin, tmax=tmax)
+        sim.plot(ax=axes[0], x_compat=True, label=f"{sim.name} ($R^2$={r2:.2%})")
         if set_axes_properties:
-            axes[0].set_title("observations vs. simulation")
             axes[0].set_ylim(ylims[0])
         axes[0].grid(True)
         axes[0].legend(ncol=3, frameon=False, numpoints=3)
+        axes[0].set_ylabel("Head")
 
         if ytick_base and set_axes_properties:
             if isinstance(ytick_base, bool):
                 # determine the ytick-spacing of the top graph
                 yticks = axes[0].yaxis.get_ticklocs()
                 if len(yticks) > 1:
                     ytick_base = yticks[1] - yticks[0]
@@ -489,14 +524,15 @@
                     # set the ytick-spacing equal to the top graph
                     locator = MultipleLocator(base=ytick_base)
                     ax.yaxis.set_major_locator(locator)
                 ax.set_title(names[i])
                 ax.set_ylim(ylims[i + 1])
             ax.grid(True)
             ax.minorticks_off()
+            ax.set_ylabel("Rise")
         if set_axes_properties:
             # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
             if tmin is not None:
                 tmin = Timestamp(tmin)
             if tmax is not None:
                 tmax = Timestamp(tmax)
             axes[0].set_xlim(tmin, tmax)
@@ -744,14 +780,15 @@
             ax.legend([stress.name], loc=2)
 
         plt.xlim(tmin, tmax)
         fig.tight_layout(pad=0.0)
 
         return axes
 
+    @PastasDeprecationWarning
     @model_tmin_tmax
     def contributions_pie(
         self,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
         ax: Optional[Axes] = None,
         figsize: Optional[Figure] = None,
@@ -903,15 +940,15 @@
                         )
                         name = sml.stress[istress].name
                         if name is None:
                             name = sm
                         contributions.append((name, h))
 
                         # plot step responses for each well, scaled with distance
-                        p = sml.get_parameters(istress=istress)
+                        p = sml.get_parameters(model=self.ml, istress=istress)
                         step = self.ml.get_step_response(sm, p=p)
                         ax_step.plot(step.index, step, c=stackcolors[name], label=name)
                         # recalculate y-limits step response axes
                         ax_step.relim()
                 else:
                     h = self.ml.get_contribution(sm, tmin=tmin, tmax=tmax)
                     name = sm
```

### Comparing `pastas-1.4.0/pastas/plotting/plotly.py` & `pastas-1.5.0/pastas/plotting/plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+"""This module contains interactive plots for Pastas models.
+"""
+
 import numpy as np
 import pandas as pd
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 from scipy.stats import norm, probplot
 
 from pastas.extensions import register_model_accessor
 from pastas.plotting.plotutil import (
     _get_height_ratios,
     _table_formatter_params,
     _table_formatter_stderr,
 )
+from pastas.rfunc import HantushWellModel
 from pastas.stats import acf
 
 
 @register_model_accessor("plotly")
 class Plotly:
     """Extension class for interactive plotly figures for pastas Models.
 
     Usage
     -----
-    >>> ps.utils.register_plotly_extension()
+    >>> ps.extensions.register_plotly_extension()
     INFO: Registered plotly plotting methods in Model class, e.g. `ml.plotly.plot()`.
     >>> fig = ml.plotly.results()
     >>> fig.write_html("results_figure.html")
 
     Methods
     -------
     plot
@@ -242,16 +246,24 @@
                 xaxis="x",
                 yaxis=f"y{iax_contrib}",
                 showlegend=False,
             )
             traces.append(trace_c)
 
             # response
+            rkwargs = {}
+            p = None
+            if self._model.stressmodels[c.name].rfunc is not None:
+                if isinstance(self._model.stressmodels[c.name].rfunc, HantushWellModel):
+                    rkwargs = {"warn": False}
+                    p = self._model.stressmodels[c.name].get_parameters(
+                        model=self._model, istress=0
+                    )
             response = self._model._get_response(
-                block_or_step="step", name=c.name, add_0=True
+                block_or_step="step", name=c.name, p=p, add_0=True, **rkwargs
             )
             trace_r = go.Scatter(
                 x=response.index,
                 y=response.values,
                 mode="lines",
                 marker_color="#1F77B4",
                 name=f"{c.name}",
```

### Comparing `pastas-1.4.0/pastas/plotting/plots.py` & `pastas-1.5.0/pastas/plotting/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module contains all the plotting methods in Pastas."""
+"""This module contains plotting methods for Pastas."""
 
 import logging
 from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `pastas-1.4.0/pastas/plotting/plotutil.py` & `pastas-1.5.0/pastas/plotting/plotutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""This module contains utility functions for plotting.
+"""
+
 from typing import List, Union
 
 import numpy as np
 from pandas import Series
 
 from pastas.typing import Axes
```

### Comparing `pastas-1.4.0/pastas/rcparams.py` & `pastas-1.5.0/pastas/rcparams.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/recharge.py` & `pastas-1.5.0/pastas/recharge.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/rfunc.py` & `pastas-1.5.0/pastas/rfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,41 +166,33 @@
         Returns
         -------
         s: array_like
             Array with the step response.
         """
         return
 
-    def block(
-        self,
-        p: ArrayLike,
-        dt: float = 1.0,
-        cutoff: Optional[float] = None,
-        maxtmax: Optional[int] = None,
-    ) -> ArrayLike:
+    def block(self, p: ArrayLike, dt: float = 1.0, **kwargs) -> ArrayLike:
         """Method to return the block function.
 
         Parameters
         ----------
         p: array_like
             array_like object with the values as floats representing the model
             parameters.
         dt: float
             timestep as a multiple of one day.
-        cutoff: float, optional
-            proportion after which the step function is cut off.
-        maxtmax: int, optional
-            Maximum timestep to compute the block response for.
+        kwargs: dict
+            kwargs are passed onto self.step()
 
         Returns
         -------
         s: array_like
             Array with the block response.
         """
-        s = self.step(p=p, dt=dt, cutoff=cutoff, maxtmax=maxtmax)
+        s = self.step(p=p, dt=dt, **kwargs)
         return np.append(s[0], np.subtract(s[1:], s[:-1]))
 
     @staticmethod
     def impulse(t: ArrayLike, p: ArrayLike) -> ArrayLike:
         """Method to return the impulse response function.
 
         Parameters
```

### Comparing `pastas-1.4.0/pastas/solver.py` & `pastas-1.5.0/pastas/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,16 +347,17 @@
             if it > max_iter:
                 break
             else:
                 it += 1
 
         if samples.shape[0] < n:
             logger.warning(
-                "Parameter sample size is smaller than n: "
-                f"{samples.shape[0]}/{n}. Increase 'max_iter'."
+                "Parameter sample size is smaller than n: %s/%s Increase 'max_iter'.",
+                samples.shape[0],
+                n,
             )
         return samples[:n, :]
 
     def _get_realizations(
         self,
         func: Function,
         n: Optional[int] = None,
@@ -1012,15 +1013,15 @@
         # Return the distribution
         if dist == "uniform":
             loc = pmin
             scale = pmax - pmin
 
         if np.isnan(loc) or np.isnan(scale):
             msg = "Location and/or scale parameter is NaN."
-            logger.error(msg=msg)
+            logger.error(msg)
             raise ValueError(msg)
 
         return getattr(mod, dist)(loc=loc, scale=scale)
 
     def set_parameter(
         self,
         name: str,
@@ -1062,15 +1063,15 @@
         not work as expected.
 
         """
         # Check if the parameter is present in the solver
         if name not in self.parameters.index:
             msg = "parameter %s is not present in the solver."
             self.logger.error(msg, name)
-            raise KeyError(msg, name)
+            raise KeyError(msg % name)
 
         # Set the initial value
         if initial is not None:
             self.parameters.loc[name, "initial"] = float(initial)
 
         # Set the vary property
         if vary is not None:
```

### Comparing `pastas-1.4.0/pastas/stats/__init__.py` & `pastas-1.5.0/pastas/stats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 # flake8: noqa
 
 import pastas.stats.metrics as metrics
 import pastas.stats.signatures as signatures
 
 from .core import acf, ccf, mean, std, var
 from .dutch import ghg, glg, gvg, q_ghg, q_glg, q_gvg
-from .metrics import aic, bic, evp, kge_2012, mae, nse, pearsonr, rmse, rsq, sse
+from .metrics import aic, bic, evp, kge, kge_2012, mae, nse, pearsonr, rmse, rsq, sse
 from .sgi import sgi
 from .tests import diagnostics, durbin_watson, ljung_box, runs_test, stoffer_toloi
```

### Comparing `pastas-1.4.0/pastas/stats/core.py` & `pastas-1.5.0/pastas/stats/core.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/stats/dutch.py` & `pastas-1.5.0/pastas/stats/dutch.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/stats/metrics.py` & `pastas-1.5.0/pastas/stats/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 >>> ps.stats.rmse(sim, obs)
 
 or directly from a Pastas model:
 
 >>> ml.stats.rmse()
 """
 
-from logging import getLogger
-
-# Type Hinting
+from logging import captureWarnings, getLogger
 from typing import Optional
+from warnings import warn
 
 from numpy import abs as npabs
 from numpy import average, log, nan, sqrt
 from pandas import Series
 
 from pastas.stats.core import _get_weights, mean, std, var
 
@@ -28,18 +27,23 @@
     "sse",
     "mae",
     "nse",
     "evp",
     "rsq",
     "bic",
     "aic",
+    "aicc",
     "pearsonr",
-    "kge_2012",
+    "kge",
 ]
+
+captureWarnings(True)
 logger = getLogger(__name__)
+warnings_logger = getLogger("py.warnings")
+logger.addHandler(warnings_logger)
 
 
 # Absolute Error Metrics
 
 
 def mae(
     obs: Optional[Series] = None,
@@ -476,51 +480,111 @@
     Parameters
     ----------
     obs: pandas.Series, optional
         Series with the observed values.
     sim: pandas.Series, optional
         The Series with the simulated values.
     res: pandas.Series, optional
-        The Series with the residual values. If time series for the residuals are
-        provided, the sim and obs arguments are ignored. Note that the residuals
-        must be computed as `obs - sim` here.
+        The Series with the residual values. If time series for the residuals
+        are provided, the sim and obs arguments are ignored. Note that the
+        residuals must be computed as `obs - sim` here.
     nparam: int, optional
         number of calibrated parameters.
     missing: str, optional
-        string with the rule to deal with missing values. Only "drop" is supported now.
+        string with the rule to deal with missing values. Only "drop" is
+        supported now.
 
     Notes
     -----
     The Akaike Information Criterium (AIC) :cite:p:`akaike_new_1974` is computed as
     follows:
 
     .. math:: \\text{AIC} = -2 log(L) + 2 nparam
 
-    where :math:`n_{param}` is the number of calibration parameters and L is the
-    likelihood function for the model.
+    where :math:`n_{param}` is the number of calibration parameters and L is
+    the likelihood function for the model. In the case of ordinary least
+    squares:
+
+    .. math:: log(L) = - (nobs / 2) * log(RSS / -nobs)
+
+    where RSS denotes the residual sum of squares and nobs the number of
+    observations.
     """
     err = _compute_err(obs=obs, sim=sim, res=res, missing=missing)
 
     # Return nan if the time indices of the sim and obs don't match
     if err.index.size == 0:
         logger.warning("Time indices of the sim and obs don't match.")
         return nan
 
     n = err.index.size
 
     return n * log((err.to_numpy() ** 2.0).sum() / n) + 2.0 * nparam
 
 
+def aicc(
+    obs: Optional[Series] = None,
+    sim: Optional[Series] = None,
+    res: Optional[Series] = None,
+    missing: str = "drop",
+    nparam: int = 1,
+) -> float:
+    """Compute the Akaike Information Criterium with second order
+    bias correction for the number of observations (AICc)
+
+    Parameters
+    ----------
+    obs: pandas.Series, optional
+        Series with the observed values.
+    sim: pandas.Series, optional
+        The Series with the simulated values.
+    res: pandas.Series, optional
+        The Series with the residual values. If time series for the residuals
+        are provided, the sim and obs arguments are ignored. Note that the
+        residuals must be computed as `obs - sim` here.
+    nparam: int, optional
+        number of calibrated parameters.
+    missing: str, optional
+        string with the rule to deal with missing values. Only "drop" is
+        supported now.
+
+    Notes
+    -----
+
+    The corrected Akaike Information Criterium (AICc)
+    :cite:p:`suguria_aicc_1978` is computed as follows:
+
+    .. math:: \\text{AIC} = -2 log(L) + 2 nparam - (2 nparam (nparam + 1) / (nobs - nparam - 1))
+
+    where :math:`n_{param}` is the number of calibration parameters, nobs is
+    the number of observations and L is the likelihood function for the model.
+    In the case of ordinary least squares:
+
+    .. math:: log(L) = - (nobs / 2) * log(RSS / -nobs)
+
+    where RSS denotes the residual sum of squares.
+    """
+    err = _compute_err(obs=obs, sim=sim, res=res, missing=missing)
+
+    n = err.index.size
+
+    c_term = (2 * nparam * (nparam + 1)) / (n - nparam - 1)
+    return aic(res=-err, nparam=nparam) + c_term
+
+
 # Forecast Error Metrics
-def kge_2012(
+
+
+def kge(
     obs: Series,
     sim: Series,
     missing: str = "drop",
     weighted: bool = False,
     max_gap: int = 30,
+    modified: bool = False,
 ) -> float:
     """Compute the (weighted) Kling-Gupta Efficiency (KGE).
 
     Parameters
     ----------
     sim: pandas.Series
         Series with the simulated values.
@@ -532,26 +596,32 @@
     weighted: bool, optional
         Weight the values by the normalized time step to account for
         irregular time series. Default is False.
     max_gap: int, optional
         maximum allowed gap period in days to use for the computation of the
         weights. All time steps larger than max_gap are replace with the
         max_gap value. Default value is 30 days.
+    modified: bool, optional
+        Use the modified KGE as proposed by :cite:t:`kling_runoff_2012`.
+        According to the article this ensures that the bias and variability
+        ratios are not cross-correlated, which otherwise may occur when inputs
+        are biased.
 
     Notes
     -----
     The (weighted) Kling-Gupta Efficiency :cite:t:`kling_runoff_2012` is
     computed as follows:
 
     .. math:: \\text{KGE} = 1 - \\sqrt{(r-1)^2 + (\\beta-1)^2 - (\\gamma-1)^2}
 
     where :math:`\\beta = \\bar{x} / \\bar{y}` and :math:`\\gamma =
-    \\frac{\\bar{\\sigma}_x / \\bar{x}}{\\bar{\\sigma}_y / \\bar{y}}`. If
-    weighted equals True, the weighted mean, variance and pearson
-    correlation are used.
+    \\frac{\\bar{\\sigma}_x}{\\bar{\\sigma}_y}`. If modified equals True,
+    :math:`\\gamma = \\frac{\\bar{\\sigma}_x / \\bar{x}}{\\bar{\\sigma}_y /
+    \\bar{y}}`. If weighted equals True, the weighted mean, variance and
+    pearson correlation are used.
     """
     if missing == "drop":
         obs = obs.dropna()
 
     sim = sim.reindex(obs.index).dropna()
 
     # Return nan if the time indices of the sim and obs don't match
@@ -561,22 +631,81 @@
 
     r = pearsonr(obs=obs, sim=sim, weighted=weighted, max_gap=max_gap)
 
     mu_sim = mean(sim, weighted=weighted, max_gap=max_gap)
     mu_obs = mean(obs, weighted=weighted, max_gap=max_gap)
 
     beta = mu_sim / mu_obs
-    gamma = (std(sim, weighted=weighted, max_gap=max_gap) / mu_sim) / (
-        std(obs, weighted=weighted, max_gap=max_gap) / mu_obs
-    )
+    if modified:
+        gamma = (std(sim, weighted=weighted, max_gap=max_gap) / mu_sim) / (
+            std(obs, weighted=weighted, max_gap=max_gap) / mu_obs
+        )
+    else:
+        gamma = std(sim, weighted=weighted, max_gap=max_gap) / std(
+            obs, weighted=weighted, max_gap=max_gap
+        )
 
     kge = 1 - sqrt((r - 1) ** 2 + (beta - 1) ** 2 + (gamma - 1) ** 2)
     return kge
 
 
+def kge_2012(
+    obs: Series,
+    sim: Series,
+    missing: str = "drop",
+    weighted: bool = False,
+    max_gap: int = 30,
+) -> float:
+    """Compute the (weighted) Kling-Gupta Efficiency (KGE).
+
+    Parameters
+    ----------
+    sim: pandas.Series
+        Series with the simulated values.
+    obs: pandas.Series
+        The Series with the observed values.
+    missing: str, optional
+        string with the rule to deal with missing values. Only "drop" is
+        supported now.
+    weighted: bool, optional
+        Weight the values by the normalized time step to account for
+        irregular time series. Default is False.
+    max_gap: int, optional
+        maximum allowed gap period in days to use for the computation of the
+        weights. All time steps larger than max_gap are replace with the
+        max_gap value. Default value is 30 days.
+
+    Notes
+    -----
+    The (weighted) Kling-Gupta Efficiency :cite:t:`kling_runoff_2012` is
+    computed as follows:
+
+    .. math:: \\text{KGE} = 1 - \\sqrt{(r-1)^2 + (\\beta-1)^2 - (\\gamma-1)^2}
+
+    where :math:`\\beta = \\bar{x} / \\bar{y}` and :math:`\\gamma =
+    \\frac{\\bar{\\sigma}_x / \\bar{x}}{\\bar{\\sigma}_y / \\bar{y}}`. If
+    weighted equals True, the weighted mean, variance and pearson
+    correlation are used.
+    """
+
+    warn(
+        "This function `kge_2012` will be deprecated in Pastas version 2.0. Please use"
+        "`pastas.stats.kge(modified=True)` to get the same outcome.",
+        category=FutureWarning,
+    )
+    return kge(
+        obs=obs,
+        sim=sim,
+        missing=missing,
+        weighted=weighted,
+        max_gap=max_gap,
+        modified=True,
+    )
+
+
 def _compute_err(
     obs: Optional[Series] = None,
     sim: Optional[Series] = None,
     res: Optional[Series] = None,
     missing: str = "drop",
 ):
     """
```

### Comparing `pastas-1.4.0/pastas/stats/sgi.py` & `pastas-1.5.0/pastas/stats/sgi.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/stats/signatures.py` & `pastas-1.5.0/pastas/stats/signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""This module contains methods to compute the groundwater signatures."""
+"""This module contains methods to compute the groundwater signatures. Part of the
+signatures selection is based on the work of :cite:t:`heudorfer_index-based_2019`."""
 
 # Type Hinting
 from logging import getLogger
 from typing import Optional, Tuple, Union
 
 from numpy import (
     arctan,
@@ -478,15 +479,15 @@
     elif freq == "W":
         df["time"] = df.index.isocalendar().week
     elif freq == "D":
         df["time"] = df.index.isocalendar().day
     else:
         msg = "freq %s is not a supported option."
         logger.error(msg, freq)
-        raise ValueError(msg)
+        raise ValueError(msg % freq)
 
     df["values"] = 1.0
     df = df.pivot_table(columns="head", index="time", aggfunc="sum", values="values")
 
     # Count of rows and column items
     x = df.sum(axis=1)  # Time
     y = df.sum(axis=0)  # Head
@@ -988,15 +989,15 @@
     """
     # Get the time step in days
     dt = diff(series.index.to_numpy()) / Timedelta("1D")
 
     # Check if the time step is approximately daily
     if not (dt > 0.9).all() & (dt < 1.1).all():
         msg = (
-            "The time step is not approximately daily (>10% of time steps are"
+            "The time step is not approximately daily (>10%% of time steps are"
             "non-daily). This may lead to incorrect results."
         )
         logger.warning(msg)
         return nan
     else:
         series_diff = series.diff()
         reversals = (
@@ -1271,18 +1272,18 @@
     popt, _ = curve_fit(
         f, binned.index, binned.values, p0=[1, 100], bounds=(0, [100, 1e3])
     )
 
     # Return nan and raise warning if the decay constant is close to the boundary
     if isclose(popt[1], 0.0) or isclose(popt[1], 1e3):
         msg = (
-            "The estimated recession constant ({:.2f}) is close to the boundary. "
-            "This may lead to incorrect results.".format(popt[1])
+            "The estimated recession constant (%s) is close to the boundary. "
+            "This may lead to incorrect results."
         )
-        logger.warning(msg)
+        logger.warning(msg, round(popt[1], 2))
         return nan
     else:
         return popt[1]
 
 
 def recovery_constant(
     series: Series,
@@ -1342,18 +1343,18 @@
     popt, _ = curve_fit(
         f, binned.index, binned.values, p0=[1, 100], bounds=(0, [100, 1e3])
     )
 
     # Return nan and raise warning if the recovery constant is close to the boundary
     if isclose(popt[1], 0.0) or isclose(popt[1], 1e3):
         msg = (
-            "The estimated recovery constant ({:.2f}) is close to the boundary. "
-            "This may lead to incorrect results.".format(popt[1])
+            "The estimated recovery constant (%s) is close to the boundary. "
+            "This may lead to incorrect results."
         )
-        logger.warning(msg)
+        logger.warning(msg, round(popt[1], 2))
         return nan
     else:
         return popt[1]
 
 
 def duration_curve_slope(
     series: Series, l: float = 0.1, u: float = 0.9, normalize: bool = False
```

### Comparing `pastas-1.4.0/pastas/stats/tests.py` & `pastas-1.5.0/pastas/stats/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,18 @@
     if cutoff == "mean":
         cutoff = r.mean()
     elif cutoff == "median":
         cutoff = median(r)
     elif isinstance(cutoff, float):
         pass
     else:
-        raise NotImplementedError(f"Cutoff criterion {cutoff} is not " f"implemented.")
+        msg = """Cutoff criterion %s is not implemented. Cutoff should be 'mean',
+                 'median', or a float value."""
+        logger.error(msg, cutoff)
+        raise NotImplementedError(msg % cutoff)
 
     r[r > cutoff] = 1
     r[r < cutoff] = 0
 
     # Calculate number of positive and negative noise
     n_pos = r.sum()
     n_neg = r.size - n_pos
```

### Comparing `pastas-1.4.0/pastas/stressmodels.py` & `pastas-1.5.0/pastas/stressmodels.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,36 @@
         """
         if len(self.stress) == 0:
             settings = None
         else:
             settings = {stress.name: stress.settings for stress in self.stress}
         return settings
 
+    def get_parameters(self, model=None) -> ArrayLike:
+        """Get parameters and return as array.
+
+        Parameters
+        ----------
+        model : pastas.Model, optional
+            If provided, and the model is solved, return optimal model parameter-values.
+            Otherwise, return initial parameter-values.
+        istress : int, optional
+            if provided, return specific parameter set, else return all parameters.
+
+        Returns
+        -------
+        p : array_like
+            An array of the parameters of the stressmodel.
+        """
+        if model is None:
+            p = self.parameters.initial.values
+        else:
+            p = model.get_parameters(self.name)
+        return p
+
 
 class StressModel(StressModelBase):
     """Stress model convoluting a stress with a response function.
 
     Parameters
     ----------
     stress: pandas.Series
@@ -974,16 +996,16 @@
     def get_parameters(self, model=None, istress: Optional[int] = None) -> ArrayLike:
         """Get parameters including distance to observation point and return as array
         (dimensions = (nstresses, 4)).
 
         Parameters
         ----------
         model : pastas.Model, optional
-            if provided, return optimal model parameters, else return initial
-            parameters.
+            If provided, and the model is solved, return optimal model parameter-values.
+            Otherwise, return initial parameter-values.
         istress : int, optional
             if provided, return specific parameter set, else return all parameters.
 
         Returns
         -------
         p : array_like
             parameters for each stress as row of array, if istress is used returns
@@ -1516,14 +1538,43 @@
             temp = None
         df = self.recharge.get_water_balance(
             prec=prec, evap=evap, temp=temp, p=p[-self.recharge.nparam :]
         )
         df.index = self.prec.series.index
         return df
 
+    def get_parameters(self, model=None, istress: Optional[int] = None) -> ArrayLike:
+        """Get parameters and return as array.
+
+        Parameters
+        ----------
+        model : pastas.Model, optional
+            If provided, and the model is solved, return optimal model parameter-values.
+            Otherwise, return initial parameter-values.
+        istress : int, optional
+            if provided, return specific parameter set, else return all parameters.
+
+        Returns
+        -------
+        p : array_like
+            An array of the parameters of the stressmodel.
+        """
+        if model is None:
+            p = self.parameters.initial.values
+        else:
+            p = model.get_parameters(self.name)
+
+        if istress is not None and isinstance(self.recharge, Linear):
+            if istress == 0:
+                p = p[:-1]
+            elif istress == 1:
+                p[0] *= p[-1]
+                p = p[:-1]
+        return p
+
     def to_dict(self, series: bool = True) -> dict:
         """Method to export the RechargeModel object.
 
         Returns
         -------
         data: dict
             dictionary with all necessary information to reconstruct the object.
```

### Comparing `pastas-1.4.0/pastas/timer.py` & `pastas-1.5.0/pastas/timer.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/timeseries.py` & `pastas-1.5.0/pastas/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,20 @@
 
         # Update the settings with user-provided values, if any.
         if settings:
             if isinstance(settings, str):
                 if settings in self._predefined_settings.keys():
                     settings = self._predefined_settings[settings]
                 else:
-                    error = (
-                        f"Settings shortcut code '{settings}' is not in the "
-                        f"predefined settings options. Please choose from"
-                        f" {self._predefined_settings.keys()}"
+                    msg = (
+                        "Settings shortcut code '%s' is not in the predefined "
+                        "settings options. Please choose from %s.",
                     )
-                    raise KeyError(error)
+
+                    raise KeyError(msg, settings, self._predefined_settings.keys())
             self._update_settings(**settings)
 
         self.update_series(force_update=True, **self.settings)
 
     def __repr__(self) -> str:
         """Prints a simple string representation of the time series."""
         return (
@@ -443,18 +443,20 @@
         freq = self.settings["freq"]
         method = self.settings["fill_before"]
         tmin = self.settings["tmin"]
 
         if tmin is None:
             pass
         elif pd.Timestamp(tmin) > series.index.max():
-            logger.error(
+            msg = (
                 "The tmin is later than the last value of the time series. Pastas "
                 "does not support this. Please extend time series manually."
             )
+            logger.error(msg)
+            raise ValueError(msg)
         elif pd.Timestamp(tmin) >= series.index.min():
             series = series.loc[pd.Timestamp(tmin) :]
         else:
             index_extend = pd.date_range(
                 start=pd.Timestamp(tmin), end=series.index.min(), freq=freq
             )
             series = series.reindex(series.index.union(index_extend[:-1]))
@@ -486,21 +488,20 @@
                     "values.",
                     self.name,
                     series.index.min(),
                     method,
                 )
             elif method is None:
                 msg = (
-                    f"Time Series '{self.name}': cannot be extended into past to"
-                    f" {series.index.min()} as 'fill_before' method is 'None'. "
-                    "Provide settings to stress model, e.g. "
-                    "`ps.StressModel(stress, settings='prec')`."
+                    "Time Series '%s': cannot be extended into past to %s as "
+                    "'fill_before' method is 'None'. Provide settings to stress model,"
+                    "e.g. `ps.StressModel(stress, settings='prec')`."
                 )
-                logger.error(msg)
-                raise ValueError(msg)
+                logger.error(msg, self.name, series.index.min())
+                raise ValueError(msg % (self.name, series.index.min()))
             else:
                 logger.info(
                     "Time Series '%s': User-defined option for fill_before '%s' is not "
                     "supported.",
                     self.name,
                     method,
                 )
@@ -512,18 +513,20 @@
         freq = self.settings["freq"]
         method = self.settings["fill_after"]
         tmax = self.settings["tmax"]
 
         if tmax is None:
             pass
         elif pd.Timestamp(tmax) <= series.index.min():
-            logger.error(
+            msg = (
                 "The tmax is before the first value of the time series. Pastas does "
                 "not support this. Please extend time series manually."
             )
+            logger.error(msg)
+            raise ValueError(msg)
         elif pd.Timestamp(tmax) <= series.index.max():
             series = series.loc[: pd.Timestamp(tmax)]
         else:
             index_extend = pd.date_range(
                 start=series.index.max(), end=pd.Timestamp(tmax), freq=freq
             )
             series = series.reindex(series.index.union(index_extend))
@@ -555,21 +558,20 @@
                     "values.",
                     self.name,
                     series.index.max(),
                     method,
                 )
             elif method is None:
                 msg = (
-                    f"Time Series '{self.name}': cannot be extended into future to"
-                    f" {series.index.max()} as 'fill_after' method is 'None'. "
-                    "Provide settings to stress model, e.g. "
-                    "`ps.StressModel(stress, settings='prec')`."
+                    "Time Series '%s': cannot be extended into future to %s as "
+                    "'fill_after' method is 'None'. Provide settings to stress model, "
+                    "e.g. `ps.StressModel(stress, settings='prec')`."
                 )
-                logger.error(msg)
-                raise ValueError(msg)
+                logger.error(msg, self.name, series.index.max())
+                raise ValueError(msg % (self.name, series.index.max()))
             else:
                 logger.warning(
                     "Time Series '%s': User-defined option for fill_after '%s' is not "
                     "supported",
                     self.name,
                     method,
                 )
@@ -707,80 +709,80 @@
             # helpful specific message for multi-column DataFrames
             msg = "DataFrame with multiple columns. Please select one."
             logger.error(msg)
             raise ValueError(msg)
 
     # 0. Make sure it is a Series and not something else (e.g., DataFrame)
     if not isinstance(series, pd.Series):
-        msg = f"Expected a Pandas Series, got {type(series)}"
-        logger.error(msg)
-        raise ValueError(msg)
+        msg = "Expected a Pandas Series, got %s"
+        logger.error(msg, type(series))
+        raise ValueError(msg % type(series))
 
     name = series.name  # Only Series have a name, DateFrame do not
 
     # 1. Make sure the values are floats
     if not pd.api.types.is_float_dtype(series):
-        msg = f"Values of time series {name} are not dtype=float."
-        logger.error(msg)
-        raise ValueError(msg)
+        msg = "Values of time series %s are not dtype=float."
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 2. Make sure the index is a DatetimeIndex
     if not isinstance(series.index, pd.DatetimeIndex):
-        msg = f"Index of series {name} is not a pandas.DatetimeIndex."
-        logger.error(msg)
-        raise ValueError(msg)
+        msg = "Index of series %s is not a pandas.DatetimeIndex."
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 3. Make sure the indices are datetime64
     if not pd.api.types.is_datetime64_dtype(series.index):
-        msg = f"Indices os series {name} are not datetime64."
-        logger.error(msg)
-        raise ValueError(msg)
+        msg = "Indices os series %s are not datetime64."
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 4. Make sure there are no NaT in index
     if series.index.hasnans:
         msg = (
-            f"The index of series {name} contains NaNs. "
+            "The index of series %s contains NaNs. "
             "Try to remove these with `series.loc[series.index.dropna()]`."
         )
-        logger.error(msg)
-        raise ValueError(msg)
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 5. Make sure the index is monotonically increasing
     if not series.index.is_monotonic_increasing:
         msg = (
-            f"The time-indices of series {name} are not monotonically increasing. Try "
-            f"to use `series.sort_index()` to fix it."
+            "The time-indices of series %s are not monotonically increasing. Try "
+            "to use `series.sort_index()` to fix it."
         )
-        logger.error(msg)
-        raise ValueError(msg)
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 6. Make sure there are no duplicate indices
     if not series.index.is_unique:
         msg = (
-            f"duplicate time-indexes were found in the time series {name}. Make sure "
+            "duplicate time-indexes were found in the time series %s. Make sure "
             "there are no duplicate indices. For example by "
             "`grouped = series.groupby(level=0); series = grouped.mean()`"
             "or `series = series.loc[~series.index.duplicated(keep='first/last')]`"
         )
-        logger.error(msg)
-        raise ValueError(msg)
+        logger.error(msg, name)
+        raise ValueError(msg % name)
 
     # 7. Make sure the time series has no nan-values
     if series.hasnans:
         msg = (
             "The Time Series '%s' has nan-values. Pastas will use the fill_nan "
             "settings to fill up the nan-values."
         )
         logger.warning(msg, name)
 
     # 8. Make sure the time series has equidistant time steps
     if equidistant:
         if not pd.infer_freq(series.index):
             msg = (
-                f"The frequency of the index of time series {name} could not be "
-                f"inferred. Please provide a time series with a regular time step."
+                "The frequency of the index of time series %s could not be "
+                "inferred. Please provide a time series with a regular time step."
             )
-            logger.error(msg)
-            raise ValueError(msg)
+            logger.error(msg, name)
+            raise ValueError(msg % name)
 
     # If all checks are passed, return True
     return True
```

### Comparing `pastas-1.4.0/pastas/timeseries_utils.py` & `pastas-1.5.0/pastas/timeseries_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,24 @@
     S   secondly frequency
     L, ms       milliseconds
     U, us       microseconds
     N   nanoseconds
 
     """
     offset = to_offset(freq)
-    if not hasattr(offset, "delta"):
-        msg = "Frequency {} not supported.".format(freq)
-        logger.error(msg)
-        raise ValueError(msg)
+    try:
+        Timedelta(offset)
+    except:
+        msg = "Frequency %s not supported."
+        logger.error(msg, freq)
+        raise ValueError(msg % freq)
+    if offset.n == 1:
+        freq = offset.name
     else:
-        if offset.n == 1:
-            freq = offset.name
-        else:
-            freq = str(offset.n) + offset.name
+        freq = str(offset.n) + offset.name
     return freq
 
 
 def _get_stress_dt(freq: str) -> float:
     """Internal method to obtain a timestep in days from a frequency string.
 
     Parameters
@@ -83,17 +84,17 @@
     See http://pandas.pydata.org/pandas-docs/stable/timeseries.html#offset-aliases
     for the offset_aliases supported by Pandas.
     """
     if freq is None:
         return None
     # Get the frequency string and multiplier
     offset = to_offset(freq)
-    if hasattr(offset, "delta"):
+    try:
         dt = Timedelta(offset) / Timedelta(1, "D")
-    else:
+    except:
         num = offset.n
         freq = offset._prefix
         if freq in ["A", "Y", "AS", "YS", "BA", "BY", "BAS", "BYS"]:
             # year
             dt = num * 365
         elif freq in ["BQ", "BQS", "Q", "QS"]:
             # quarter
@@ -262,24 +263,24 @@
 
         # first mutiply by the timestep
         s_new = s * dt
 
         # calculate the cumulative sum
         s_new = s_new.cumsum()
 
-        # add NaNs at none-existing values in series at index
+        # add NaNs at non-existing values in series at index
         s_new = s_new.combine_first(Series(np.NaN, index))
 
         # interpolate these NaN's, only keep values at index
         s_new = s_new.interpolate("time")[index]
 
         # calculate the diff again (inverse of cumsum)
         s_new = s_new.diff()
 
-        # devide by the timestep again
+        # divide by the timestep again
         s_new = s_new / _get_dt_array(s_new.index)
 
         # set values after the end of the original series to NaN
         s_new[s_new.index > s.index[-1]] = np.NaN
     else:
         t_e = s.index.asi8
         t_s = t_e - dt
@@ -352,15 +353,22 @@
     sampling (meaning observations can be shifted in time), with additional filling
     logic that ensures each original measurement is only included once in the new
     time series. Values are filled as close as possible to their original timestamp
     in the new equidistant time series.
     """
 
     # build new equidistant index
-    idx = date_range(series.index[0], series.index[-1], freq=freq)
+    t_offset = _get_time_offset(series.index, freq).value_counts().idxmax()
+    # use t_offset to pick time that will keep the most data without shifting in time
+    # from the original series.
+    idx = date_range(
+        series.index[0].floor(freq) + t_offset,
+        series.index[-1].ceil(freq) + t_offset,
+        freq=freq,
+    )
 
     # get linear interpolated index from original series
     fl = interpolate.interp1d(
         series.index.asi8,
         np.arange(0, series.index.size),
         kind="linear",
         bounds_error=False,
```

### Comparing `pastas-1.4.0/pastas/transform.py` & `pastas-1.5.0/pastas/transform.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/typing/types.py` & `pastas-1.5.0/pastas/typing/types.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/pastas/utils.py` & `pastas-1.5.0/pastas/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,16 +194,17 @@
             "+",
         ]
 
     name = str(name)
     for char in ilchar:
         if char in name:
             msg = (
-                f"User-provided name '{name}' contains illegal character. Please "
-                f"remove '{char}' from name."
+                "User-provided name '%s' contains illegal character. Please "
+                "remove '%s' from name."
             )
             if raise_error:
-                raise Exception(msg)
+                logger.error(msg, name, char)
+                raise Exception(msg % (name, char))
             else:
-                logger.warning(msg)
+                logger.warning(msg, name, char)
 
     return name
```

### Comparing `pastas-1.4.0/pastas/version.py` & `pastas-1.5.0/pastas/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from importlib import import_module, metadata
 from platform import python_version
 
 logger = logging.getLogger(__name__)
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 
 def check_numba_scipy() -> bool:
     try:
         import_module("numba_scipy")
     except ImportError:
         logger.warning(
@@ -17,15 +17,15 @@
         return False
 
     scipy_version = metadata.version("scipy")
     scipy_version_nsc = [x for x in metadata.requires("numba-scipy") if "scipy" in x]
     scipy_version_nsc = scipy_version_nsc[0].split(",")[0].split("=")[-1]
     if scipy_version > scipy_version_nsc:
         logger.warning(
-            f"numba_scipy supports SciPy<={scipy_version_nsc}, found {scipy_version}"
+            "numba_scipy supports SciPy<=%s, found %s", scipy_version_nsc, scipy_version
         )
         return False
     return True
 
 
 def show_versions(lmfit: bool = True, latexify: bool = True) -> None:
     """Method to print the version of dependencies.
```

### Comparing `pastas-1.4.0/pastas.egg-info/PKG-INFO` & `pastas-1.5.0/pastas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastas
-Version: 1.4.0
+Version: 1.5.0
 Summary: Pastas is an open-source Python framework for the analysis of groundwater time series.
 Author: Collenteur et al. 2019
 Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <vonk.mart@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2021 R.A. Collenteur, M. Bakker, R. Calje, F. Schaars
         
@@ -31,22 +31,21 @@
 Project-URL: documentation, https://pastas.readthedocs.io/en/latest/
 Keywords: hydrology,groundwater,timeseries,analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: matplotlib>=3.1
 Requires-Dist: pandas>=1.1
 Requires-Dist: scipy>=1.8
 Requires-Dist: numba>=0.51
 Provides-Extra: solvers
@@ -69,14 +68,15 @@
 Requires-Dist: pastas[pytesting,solvers]; extra == "ci"
 Requires-Dist: jupyter; extra == "ci"
 Requires-Dist: coverage; extra == "ci"
 Requires-Dist: corner; extra == "ci"
 Requires-Dist: emcee; extra == "ci"
 Requires-Dist: tqdm; extra == "ci"
 Requires-Dist: plotly; extra == "ci"
+Requires-Dist: bokeh>=3.0; extra == "ci"
 Provides-Extra: rtd
 Requires-Dist: pastas[solvers]; extra == "rtd"
 Requires-Dist: Ipython; extra == "rtd"
 Requires-Dist: ipykernel; extra == "rtd"
 Requires-Dist: pydata-sphinx-theme; extra == "rtd"
 Requires-Dist: sphinx<6.0,>=3.1; extra == "rtd"
 Requires-Dist: sphinxcontrib-bibtex; extra == "rtd"
@@ -86,123 +86,136 @@
 Requires-Dist: myst_nb; extra == "rtd"
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pastas[ci,formatting,linting,rtd]; extra == "dev"
 Provides-Extra: numbascipy
 Requires-Dist: numba-scipy>=0.3.1; extra == "numbascipy"
 
-Pastas: Analysis of Groundwater Time Series
-===========================================
+# Pastas: Analysis of Groundwater Time Series
 
-.. image:: /doc/_static/logo_small.png
-   :width: 200px
-   :align: left
-
-.. image:: https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master
-   :target: https://github.com/pastas/pastas/actions/workflows/ci.yml
-.. image:: https://img.shields.io/pypi/v/pastas.svg
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/l/pastas.svg
-   :target: https://mit-license.org/
-.. image:: https://img.shields.io/pypi/pyversions/pastas
-   :target: https://pypi.python.org/pypi/pastas
-.. image:: https://img.shields.io/pypi/dm/pastas
-   :target: https://pypi.org/project/pastas/
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg
-   :target: https://doi.org/10.5281/zenodo.1465866
-.. image:: https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
-.. image:: https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434
-   :target: https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9
-.. image:: https://readthedocs.org/projects/pastas/badge/?version=latest
-   :target: https://pastas.readthedocs.io/en/latest/?badge=latest
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb
-
-Pastas: what is it?
-~~~~~~~~~~~~~~~~~~~
-Pastas is an open source python package for processing, simulating and analyzing
-groundwater time series. The object oriented structure allows for the quick
-implementation of new model components. Time series models can be created,
-calibrated, and analysed with just a few lines of python code with the
-built-in optimization, visualisation, and statistical analysis tools.
-
-Documentation & Examples
-~~~~~~~~~~~~~~~~~~~~~~~~
-- Documentation is provided on the dedicated website `pastas.dev <http://www.pastas.dev/>`_
-- Examples can be found on the `examples directory on the documentation website <https://pastas.readthedocs.io/en/dev/examples/index.html>`_
-- View and edit a working example notebook of a Pastas model in `MyBinder <https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb>`_
-- A list of publications that use Pastas is available in a `dedicated Zotero group <https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list>`_
-
-Get in Touch
-~~~~~~~~~~~~
-- Questions on Pastas can be asked and answered on `Github Discussions <https://github.com/pastas/pastas/discussions>`_.
-- Bugs, feature requests and other improvements can be posted as `Github Issues <https://github.com/pastas/pastas/issues>`_.
-- Pull requests will only be accepted on the development branch (dev) of
-  this repository. Please take a look at the `developers section
-  <http://pastas.readthedocs.io/>`_ on the documentation website for more
-  information on how to contribute to Pastas.
-
-Quick installation guide
-~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
-installed on your computer. We recommend using the `Anaconda Distribution
-<https://www.continuum.io/downloads>`_ as it includes most of the python
-package dependencies and the Jupyter Notebook software to run the notebooks.
-However, you are free to install any Python distribution you want.
-
-Stable version
---------------
-To get the latest stable version, use::
-
-  pip install pastas
-
-Update
-------
-To update pastas, use::
-
-  pip install pastas --upgrade
-
-Developers
-----------
-To get the latest development version, use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
-
-Related packages
-~~~~~~~~~~~~~~~~
-- `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
-- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
-- `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
-- `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
-
-Dependencies
-~~~~~~~~~~~~
-Pastas depends on a number of Python packages, of which all of the necessary
-are automatically installed when using the pip install manager. To
-summarize, the dependencies necessary for a minimal function installation of
-Pastas
-
-- numpy>=1.7
-- matplotlib>=3.1
-- pandas>=1.1
-- scipy>=1.8
-- numba>=0.51
-
-To install the most important optional dependencies (solver LmFit and function visualisation Latexify) at the same time with Pastas use::
-
-   pip install pastas[full]
-
-or for the development version use::
-
-   pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
-
-How to Cite Pastas?
-~~~~~~~~~~~~~~~~~~~
-If you use Pastas in one of your studies, please cite the Pastas article in Groundwater:
+> [!IMPORTANT]
+> As of Pastas 1.5, noisemodels are not added to the Pastas models by default anymore. [Read more about this change here](https://github.com/pastas/pastas/issues/735).
 
-- Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F. (2019) `Pastas: open source software for the analysis of groundwater time series <https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925>`_. Groundwater. doi: 10.1111/gwat.12925.
+![image](/doc/_static/logo_small.png)
+[![image](https://github.com/pastas/pastas/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/pastas/pastas/actions/workflows/ci.yml)
+[![image](https://img.shields.io/pypi/v/pastas.svg)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/l/pastas.svg)](https://mit-license.org/)
+[![image](https://img.shields.io/pypi/pyversions/pastas)](https://pypi.python.org/pypi/pastas)
+[![image](https://img.shields.io/pypi/dm/pastas)](https://pypi.org/project/pastas/)
+[![image](https://zenodo.org/badge/DOI/10.5281/zenodo.1465866.svg)](https://doi.org/10.5281/zenodo.1465866)
+[![image](https://app.codacy.com/project/badge/Grade/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![image](https://api.codacy.com/project/badge/Coverage/952f41c453854064ba0ee1fa0a0b4434)](https://app.codacy.com/gh/pastas/pastas/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage9)
+[![image](https://readthedocs.org/projects/pastas/badge/?version=latest)](https://pastas.readthedocs.io/en/latest/?badge=latest)
+[![image](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
 
-To cite a specific version of Python, you can use the DOI provided for each official release (>0.9.7) through Zenodo. Click on the link to get a specific version and DOI, depending on the Pastas version.
+## Pastas: what is it?
 
-- Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas: open-source software for time series analysis in hydrology (Version X.X.X). Zenodo. http://doi.org/10.5281/zenodo.1465866
+Pastas is an open source python package for processing, simulating and
+analyzing groundwater time series. The object oriented structure allows
+for the quick implementation of new model components. Time series models
+can be created, calibrated, and analysed with just a few lines of python
+code with the built-in optimization, visualisation, and statistical
+analysis tools.
 
+## Documentation & Examples
+
+-   Documentation is provided on the dedicated website
+    [pastas.dev](http://www.pastas.dev/)
+-   Examples can be found on the [examples directory on the
+    documentation
+    website](https://pastas.readthedocs.io/en/dev/examples/index.html)
+-   View and edit a working example notebook of a Pastas model in
+    [MyBinder](https://mybinder.org/v2/gh/pastas/pastas/master?filepath=examples%2Fnotebooks%2F1_basic_model.ipynb)
+-   A list of publications that use Pastas is available in a [dedicated
+    Zotero
+    group](https://www.zotero.org/groups/4846685/pastas/items/32FS5PTW/item-list)
+
+## Get in Touch
+
+-   Questions on Pastas can be asked and answered on [Github
+    Discussions](https://github.com/pastas/pastas/discussions).
+-   Bugs, feature requests and other improvements can be posted as
+    [Github Issues](https://github.com/pastas/pastas/issues).
+-   Pull requests will only be accepted on the development branch (dev)
+    of this repository. Please take a look at the [developers
+    section](http://pastas.readthedocs.io/) on the documentation website
+    for more information on how to contribute to Pastas.
+
+## Quick installation guide
+
+To install Pastas, a working version of Python 3.9, 3.10, 3.11, or 3.12
+has to be installed on your computer. We recommend using the [Anaconda
+Distribution](https://www.continuum.io/downloads) as it includes most of
+the python package dependencies and the Jupyter Notebook software to run
+the notebooks. However, you are free to install any Python distribution
+you want.
+
+### Stable version
+
+To get the latest stable version, use:
+
+    pip install pastas
+
+### Update
+
+To update pastas, use:
+
+    pip install pastas --upgrade
+
+### Developers
+
+To get the latest development version, use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
+
+## Related packages
+
+-   [Pastastore](https://github.com/pastas/pastastore) is a Python
+    package for managing multiple timeseries and pastas models
+-   [Metran](https://github.com/pastas/metran) is a Python package to
+    perform multivariate timeseries analysis using a technique called
+    dynamic factor modelling.
+-   [Hydropandas](https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb)
+    can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
+-   [PyEt](https://github.com/phydrus/pyet) can be used to compute
+    potential evaporation from meteorological variables.
+
+## Dependencies
+
+Pastas depends on a number of Python packages, of which all of the
+necessary are automatically installed when using the pip install
+manager. To summarize, the dependencies necessary for a minimal function
+installation of Pastas
+
+-   numpy\>=1.7
+-   matplotlib\>=3.1
+-   pandas\>=1.1
+-   scipy\>=1.8
+-   numba\>=0.51
+
+To install the most important optional dependencies (solver LmFit and
+function visualisation Latexify) at the same time with Pastas use:
+
+    pip install pastas[full]
+
+or for the development version use:
+
+    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas[full]
+
+## How to Cite Pastas?
+
+If you use Pastas in one of your studies, please cite the Pastas article
+in Groundwater:
+
+-   Collenteur, R.A., Bakker, M., Caljé, R., Klop, S.A., Schaars, F.
+    (2019) [Pastas: open source software for the analysis of groundwater
+    time
+    series](https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12925).
+    Groundwater. doi: 10.1111/gwat.12925.
+
+To cite a specific version of Pastas, you can use the DOI provided for
+each official release (\>0.9.7) through Zenodo. Click on the link to get
+a specific version and DOI, depending on the Pastas version.
+
+-   Collenteur, R., Bakker, M., Caljé, R. & Schaars, F. (XXXX). Pastas:
+    open-source software for time series analysis in hydrology (Version
+    X.X.X). Zenodo. <http://doi.org/10.5281/zenodo.1465866>
```

### Comparing `pastas-1.4.0/pastas.egg-info/SOURCES.txt` & `pastas-1.5.0/pastas.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
-README.rst
+README.md
 pyproject.toml
 pastas/__init__.py
+pastas/dataset.py
 pastas/decorators.py
 pastas/model.py
 pastas/modelstats.py
 pastas/noisemodels.py
 pastas/objective_functions.py
 pastas/rcparams.py
 pastas/recharge.py
@@ -25,14 +26,15 @@
 pastas.egg-info/top_level.txt
 pastas/extensions/__init__.py
 pastas/extensions/accessor.py
 pastas/io/__init__.py
 pastas/io/base.py
 pastas/io/pas.py
 pastas/plotting/__init__.py
+pastas/plotting/bokeh.py
 pastas/plotting/modelcompare.py
 pastas/plotting/modelplots.py
 pastas/plotting/plotly.py
 pastas/plotting/plots.py
 pastas/plotting/plotutil.py
 pastas/stats/__init__.py
 pastas/stats/core.py
@@ -41,20 +43,23 @@
 pastas/stats/sgi.py
 pastas/stats/signatures.py
 pastas/stats/tests.py
 pastas/typing/__init__.py
 pastas/typing/types.py
 tests/test_001.py
 tests/test_comparison.py
+tests/test_dataset.py
 tests/test_examples.py
 tests/test_extension.py
 tests/test_gxg.py
+tests/test_metrics.py
 tests/test_model.py
 tests/test_notebooks.py
 tests/test_notebooks_bench.py
 tests/test_plots.py
 tests/test_qgxg.py
 tests/test_recharge.py
 tests/test_rfuncs.py
 tests/test_signatures.py
 tests/test_solvers.py
-tests/test_stats.py
+tests/test_stats.py
+tests/test_timeseries_utils.py
```

### Comparing `pastas-1.4.0/pastas.egg-info/requires.txt` & `pastas-1.5.0/pastas.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pastas[pytesting,solvers]
 jupyter
 coverage
 corner
 emcee
 tqdm
 plotly
+bokeh>=3.0
 
 [dev]
 tox
 pastas[ci,formatting,linting,rtd]
 
 [formatting]
 isort
```

### Comparing `pastas-1.4.0/pyproject.toml` & `pastas-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pastas"
 dynamic = ["version"]
 description = "Pastas is an open-source Python framework for the analysis of groundwater time series."
 license = { file = "LICENSE" }
-readme = "README.rst"
+readme = "README.md"
 authors = [{ name = "Collenteur et al. 2019" }]
 maintainers = [
     { name = "R.A. Collenteur", email = "raoulcollenteur@gmail.com" },
     { name = "M. Bakker", email = "markbak@gmail.com" },
     { name = "R. Calje", email = "r.calje@artesia-water.nl" },
     { name = "F. Schaars", email = "f.schaars@artesia-water.nl" },
     { name = "D.A. Brakenhoff", email = "d.brakenhoff@artesia-water.nl" },
     { name = "O.N. Ebbens", email = "o.ebbens@artesia-water.nl" },
     { name = "M.A. Vonk", email = "vonk.mart@gmail.com" },
 ]
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 dependencies = [
     "numpy >= 1.17",
     "matplotlib >= 3.1",
     "pandas >= 1.1",
     "scipy >= 1.8",
     "numba >= 0.51",
 ]
 keywords = ["hydrology", "groundwater", "timeseries", "analysis"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Science/Research',
     'Intended Audience :: Other Audience',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Topic :: Scientific/Engineering :: Hydrology',
 ]
 
@@ -57,14 +56,15 @@
     "pastas[pytesting,solvers]",
     "jupyter",
     "coverage",
     "corner",
     "emcee",
     "tqdm",
     "plotly",
+    "bokeh >= 3.0",
 ]
 rtd = [
     "pastas[solvers]",
     "Ipython",
     "ipykernel",
     "pydata-sphinx-theme",
     "sphinx>=3.1, <6.0",
@@ -90,15 +90,15 @@
 addopts = "--strict-markers --durations=0"
 markers = ["notebooks: run notebooks", "bnotebooks: run benchmark notebooks"]
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     requires = tox>=4
-    env_list = format, lint, notebooks, py{38,39,310,311,312}
+    env_list = format, lint, notebooks, py{39,310,311,312}
 
     [testenv]
     description = run unit tests
     extras = ci
     commands =
             pytest tests -m "not notebooks and not bnotebooks"
```

### Comparing `pastas-1.4.0/tests/test_comparison.py` & `pastas-1.5.0/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_examples.py` & `pastas-1.5.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_gxg.py` & `pastas-1.5.0/tests/test_gxg.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_model.py` & `pastas-1.5.0/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         data=h[: len(input)],
     )
     return head
 
 
 def test_create_model() -> None:
     ml = ps.Model(obs, name="Test_Model")
+    ml.add_noisemodel(ps.ArNoiseModel())
 
 
 def test_add_stressmodel(ml_empty: ps.Model, sm_prec) -> None:
     ml_empty.add_stressmodel(sm_prec)
 
 
 def test_add_stressmodels(
@@ -52,40 +53,36 @@
 
 
 def test_del_constant(ml_empty: ps.Model) -> None:
     ml_empty.del_constant()
 
 
 def test_add_noisemodel(ml_empty: ps.Model) -> None:
-    ml_empty.add_noisemodel(ps.NoiseModel())
+    ml_empty.add_noisemodel(ps.ArNoiseModel())
 
 
 def test_armamodel() -> None:
-    ml = ps.Model(obs, name="Test_Model", noisemodel=False)
-    ml.add_noisemodel(ps.ArmaModel())
+    ml = ps.Model(obs, name="Test_Model")
+    ml.add_noisemodel(ps.ArmaNoiseModel())
     ml.solve()
     ml.to_file("test.pas")
 
 
 def test_del_noisemodel(ml_empty: ps.Model) -> None:
     ml_empty.del_noisemodel()
 
 
 def test_solve_model(ml: ps.Model) -> None:
     ml.solve()
 
 
 def test_solve_empty_model(ml: ps.Model) -> None:
-    try:
+    with pytest.raises(ValueError) as excinfo:
         ml.solve(tmin="2016")
-    except ValueError as e:
-        if e.args[0].startswith("Calibration series"):
-            return None
-        else:
-            raise e
+    assert excinfo.value.args[0].startswith("Calibration series")
 
 
 def test_save_model(ml: ps.Model) -> None:
     ml.to_file("test.pas")
 
 
 def test_load_model(ml: ps.Model) -> None:
@@ -157,31 +154,36 @@
 
 
 def test_modelstats(ml: ps.Model) -> None:
     ml.solve()
     ml.stats.summary()
 
 
+def test_fit_report(ml: ps.Model) -> None:
+    ml.solve(report=False)
+    ml.fit_report(corr=True, stderr=True)
+
+
 def test_model_freq_geq_daily() -> None:
     rf_rch = ps.Exponential()
     A_rch = 800
     a_rch = 50
     f_rch = -1.3
     constant = 20
 
     stress = prec + f_rch * evap
     head = generate_synthetic_heads(stress, rf_rch, (A_rch, a_rch), const=constant)
 
     models = []
     freqs = ["1D", "7D", "14D", "28D"]
     for freq in freqs:
-        iml = ps.Model(head, name=freq, noisemodel=False)
+        iml = ps.Model(head, name=freq)
         rm = ps.RechargeModel(prec, evap, rfunc=rf_rch, name="recharge")
         iml.add_stressmodel(rm)
-        iml.solve(freq=freq, noise=False, report=False)
+        iml.solve(freq=freq, report=False)
         models.append(iml)
 
     comparison = ps.CompareModels(models)
     assert (comparison.get_metrics(metric_selection=["rsq"]).squeeze() > 0.99).all()
 
 
 def test_model_freq_h():
@@ -203,11 +205,11 @@
     sm = ps.StressModel(
         tides,
         rfunc=ps.Exponential(),
         name="tide",
         settings="waterlevel",
     )
     ml_h.add_stressmodel(sm)
-    ml_h.solve(noise=False, report=False)
+    ml_h.solve(report=False)
 
     assert ml_h.simulate().index.freq == "h"
     assert ml_h.stats.rsq() > 0.99999
```

### Comparing `pastas-1.4.0/tests/test_notebooks.py` & `pastas-1.5.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_notebooks_bench.py` & `pastas-1.5.0/tests/test_notebooks_bench.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_plots.py` & `pastas-1.5.0/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_qgxg.py` & `pastas-1.5.0/tests/test_qgxg.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_recharge.py` & `pastas-1.5.0/tests/test_recharge.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_rfuncs.py` & `pastas-1.5.0/tests/test_rfuncs.py`

 * *Files identical despite different names*

### Comparing `pastas-1.4.0/tests/test_signatures.py` & `pastas-1.5.0/tests/test_signatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 def test_summary():
     """Test all signatures for minimal functioning."""
     idx = date_range("2000", "2010")
     head = Series(index=idx, data=np.random.rand(len(idx)), dtype=float)
     ps.stats.signatures.summary(head)
 
+
 def test_date_min():
-    """Test the date_min signature to have a mean of 1 if the head is at a minimum at 
+    """Test the date_min signature to have a mean of 1 if the head is at a minimum at
     the first of january of every year in a time series.
     """
     idx = date_range("2000", "2010")
     head = Series(index=idx, data=np.random.rand(len(idx)), dtype=float)
     head[head.index.dayofyear == 1] = head.min()
     assert round(ps.stats.signatures.date_min(head)) == 1
 
+
 def test_date_max():
-    """Test the date_max signature to have a mean of 1 if the head is at a maximum at 
+    """Test the date_max signature to have a mean of 1 if the head is at a maximum at
     the first of january of every year in a time series.
     """
     idx = date_range("2000", "2010")
     head = Series(index=idx, data=np.random.rand(len(idx)), dtype=float)
     head[head.index.dayofyear == 1] = head.max()
     assert round(ps.stats.signatures.date_max(head)) == 1
```

### Comparing `pastas-1.4.0/tests/test_solvers.py` & `pastas-1.5.0/tests/test_solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 
 def test_fit_constant(ml: ps.Model):
     ml.solve(fit_constant=False)
 
 
 def test_no_noise(ml: ps.Model):
-    ml.solve(noise=False)
+    ml.del_noisemodel()
+    ml.solve()
 
 
 # test the uncertainty method here
 def test_pred_interval(ml: ps.Model):
     ml.solve(solver=ps.LeastSquares())
     ml.solver.prediction_interval(n=10)
 
@@ -40,14 +41,14 @@
 
 
 # Test the EmceeSolver
 
 
 def test_emcee(ml: ps.Model):
     ml.solve(solver=ps.LeastSquares())
+    ml.del_noisemodel()
     ml.solve(
         solver=ps.EmceeSolve(nwalkers=20),
         initial=False,
         fit_constant=False,
-        noise=False,
         steps=10,
     )
```

### Comparing `pastas-1.4.0/tests/test_stats.py` & `pastas-1.5.0/tests/test_stats.py`

 * *Files identical despite different names*

