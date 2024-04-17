# Comparing `tmp/multiview_stitcher-0.1.5.tar.gz` & `tmp/multiview_stitcher-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiview_stitcher-0.1.5.tar", last modified: Mon Apr 15 14:12:59 2024, max compression
+gzip compressed data, was "multiview_stitcher-0.1.6.tar", last modified: Wed Apr 17 21:31:27 2024, max compression
```

## Comparing `multiview_stitcher-0.1.5.tar` & `multiview_stitcher-0.1.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.698665 multiview_stitcher-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.702665 multiview_stitcher-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/documentation_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/documentation_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/fusion.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/registration.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/transformation.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/data_formats.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/docs_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/features.md
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)  1615078 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/images/20230929_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/napari_stitcher.md
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/objects.md
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/related_projects.md
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   114440 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_multi_view.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_multipos_2D_czi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.702665 multiview_stitcher-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.710665 multiview_stitcher-0.1.5/src/multiview_stitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.714665 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_mv_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_spatial_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_vis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    29677 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/msi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/mv_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/ngff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59895 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/spatial_image_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.714665 multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/
--rw-r--r--   0 runner    (1001) docker     (127)  2791008 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/mosaic_test.czi
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/vis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.718665 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.183449 multiview_stitcher-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.159449 multiview_stitcher-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.163449 multiview_stitcher-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/.github/workflows/documentation_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/.github/workflows/documentation_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-17 21:31:27.183449 multiview_stitcher-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.167449 multiview_stitcher-0.1.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.167449 multiview_stitcher-0.1.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/api/fusion.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/api/registration.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/api/transformation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/data_formats.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/docs_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/features.md
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.167449 multiview_stitcher-0.1.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  1615078 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/images/20230929_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/napari_stitcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/objects.md
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/docs/related_projects.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.171449 multiview_stitcher-0.1.6/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/notebooks/stitching_bigstitcher_grid_2d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   114440 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/notebooks/stitching_multi_view.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/notebooks/stitching_multipos_2D_czi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-17 21:31:27.183449 multiview_stitcher-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.163449 multiview_stitcher-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.171449 multiview_stitcher-0.1.6/src/multiview_stitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.175449 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_mv_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_spatial_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_vis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29677 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/msi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/mv_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/ngff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59189 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/spatial_image_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.175449 multiview_stitcher-0.1.6/src/multiview_stitcher/test-datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)  2791008 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/test-datasets/mosaic_test.czi
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/vis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/src/multiview_stitcher/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:31:27.179449 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 21:31:27.000000 multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-17 21:31:17.000000 multiview_stitcher-0.1.6/tox.ini
```

### Comparing `multiview_stitcher-0.1.5/.github/workflows/documentation_main.yml` & `multiview_stitcher-0.1.6/.github/workflows/documentation_main.yml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/.github/workflows/documentation_release.yml` & `multiview_stitcher-0.1.6/.github/workflows/documentation_release.yml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/.github/workflows/test_and_deploy.yml` & `multiview_stitcher-0.1.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/.gitignore` & `multiview_stitcher-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/.pre-commit-config.yaml` & `multiview_stitcher-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/LICENSE` & `multiview_stitcher-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/PKG-INFO` & `multiview_stitcher-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiview-stitcher
-Version: 0.1.5
+Version: 0.1.6
 Summary: Registration and fusion of large imaging datasets in 2D and 3D.
 Home-page: https://github.com/multiview-stitcher/multiview-stitcher
 Author: Marvin Albert
 Author-email: marvin.albert@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/multiview-stitcher/multiview-stitcher/issues
 Project-URL: Documentation, https://github.com/multiview-stitcher/multiview-stitcher#README.md
```

### Comparing `multiview_stitcher-0.1.5/README.md` & `multiview_stitcher-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/data_formats.md` & `multiview_stitcher-0.1.6/docs/data_formats.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/docs_requirements.txt` & `multiview_stitcher-0.1.6/docs/docs_requirements.txt`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/features.md` & `multiview_stitcher-0.1.6/docs/features.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/images/20230929_screenshot.png` & `multiview_stitcher-0.1.6/docs/images/20230929_screenshot.png`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/implementation_details.md` & `multiview_stitcher-0.1.6/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/index.md` & `multiview_stitcher-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/docs/objects.md` & `multiview_stitcher-0.1.6/docs/objects.md`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/mkdocs.yml` & `multiview_stitcher-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_2d.ipynb` & `multiview_stitcher-0.1.6/notebooks/stitching_bigstitcher_grid_2d.ipynb`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb` & `multiview_stitcher-0.1.6/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/notebooks/stitching_multi_view.ipynb` & `multiview_stitcher-0.1.6/notebooks/stitching_multi_view.ipynb`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/notebooks/stitching_multipos_2D_czi.ipynb` & `multiview_stitcher-0.1.6/notebooks/stitching_multipos_2D_czi.ipynb`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/pyproject.toml` & `multiview_stitcher-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/setup.cfg` & `multiview_stitcher-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_fusion.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_integration.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_io.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_io.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_mv_graph.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_mv_graph.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_registration.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,22 +248,25 @@
 
     assert len(params) == 2 ** (ndim - 1)
 
 
 @pytest.mark.parametrize(
     """
     groupwise_resolution_method,
+    type_of_residual,
     """,
     [
-        "shortest_paths",
-        "global_optimization",
+        ("shortest_paths", None),
+        ("global_optimization", "edge"),
+        ("global_optimization", "node"),
     ],
 )
 def test_cc_registration(
     groupwise_resolution_method,
+    type_of_residual,
 ):
     # Generate a cc
     sims = sample_data.generate_tiled_dataset(
         ndim=2,
         N_t=2,
         N_c=2,
         tile_size=15,
@@ -286,10 +289,15 @@
     params = registration.register(
         msims,
         reg_channel_index=0,
         transform_key=METADATA_TRANSFORM_KEY,
         pairwise_reg_func=registration.phase_correlation_registration,
         new_transform_key="affine_registered",
         groupwise_resolution_method=groupwise_resolution_method,
+        groupwise_resolution_kwargs={
+            "type_of_residual": type_of_residual,
+        }
+        if type_of_residual is not None
+        else {},
     )
 
     assert len(params) == 3
```

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_sample_data.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_sample_data.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_spatial_image_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_spatial_image_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_vis_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/_tests/test_vis_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/fusion.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/fusion.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/io.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/io.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/msi_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/msi_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/mv_graph.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/mv_graph.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/ngff_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/ngff_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/param_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/param_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/registration.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1287,15 +1287,14 @@
                             ]
                         )
                         for ie, e in enumerate(node_edges)
                     ]
                 )
 
                 for ie, e in enumerate(node_edges):
-                    # edge_residuals[e] = curr_edge_residuals[ie]
                     edge_residuals[tuple(sorted(e))].append(
                         curr_edge_residuals[ie]
                     )
 
                 iter_residuals.append(np.mean(curr_residuals))
 
                 if curr_node != ref_node:
@@ -1306,32 +1305,18 @@
                             ),
                             g_beads_subgraph.nodes[curr_node]["affine"],
                         )
                     )
                 else:
                     new_affines.append(param_utils.identity_transform(ndim))
 
-                # node_iter_info = {
-                #     "transform": g_beads_subgraph.nodes[curr_node]["affine"].data,
-                #     "node_pts": node_pts.flatten(),
-                #     "adjecent_pts": adjecent_pts.flatten(),
-                #     "residuals": curr_residuals,
-                # }
-
                 total_iterations += 1
 
                 df_iter_node = pd.concat(
                     [
-                        # xr.DataArray(
-                        #     g_beads_subgraph.nodes[curr_node]["affine"],
-                        #     name=str(curr_node),
-                        # )
-                        # .to_dataframe()
-                        # .reset_index()
-                        # .pivot_table(str(curr_node), [], ["x_in", "x_out"]),
                         pd.DataFrame(
                             {
                                 "residual": np.mean(curr_residuals),
                                 "iteration": iteration,
                                 "total_iteration": total_iterations,
                             },
                             index=[str(curr_node)],
@@ -1358,41 +1343,43 @@
                     / mean_residuals[-1]
                 )
                 if rel_change < rel_tol:
                     break
 
             # print(iteration, mean_residuals[-1], iter_residuals)
 
-        if not len(list(g_beads_subgraph.edges)):
+        # keep parameters after one iteration if there are
+        # less than two edges
+        if len(list(g_beads_subgraph.edges)) < 2:
             break
 
         if type_of_residual == "edge":
             edge_residuals = {k: np.mean(v) for k, v in edge_residuals.items()}
 
             edges, edge_residual_values = zip(*edge_residuals.items())
 
-            residual_max_mean_ratio = np.max(edge_residual_values) / np.mean(
-                edge_residual_values
-            )
-            # print("edge_residuals_max_mean_ratio", residual_max_mean_ratio)
-            logger.debug(
-                "edge_residuals_max_mean_ratio %s", residual_max_mean_ratio
-            )
+            mean_edge_residual_value = np.mean(edge_residual_values)
 
-            if residual_max_mean_ratio < max_residual_max_mean_ratio:
+            if (
+                mean_edge_residual_value < abs_tol
+                or np.max(edge_residual_values) / mean_edge_residual_value
+                < max_residual_max_mean_ratio
+            ):
                 edge_to_remove = None
             else:
                 edge_to_remove = edges[np.argmax(edge_residual_values)]
 
         elif type_of_residual == "node":
-            residual_max_mean_ratio = np.max(iter_residuals) / np.mean(
-                iter_residuals
-            )
+            mean_iter_residual = np.mean(iter_residuals)
 
-            if residual_max_mean_ratio > max_residual_max_mean_ratio:
+            if (
+                mean_iter_residual > abs_tol
+                and np.max(iter_residuals) / mean_iter_residual
+                > max_residual_max_mean_ratio
+            ):
                 # determine which edge to remove (formula from bigstitcher)
                 # c_value = (1-qij)**2 * sqrt(dijk) * log10(max(degi, degj))
                 c_value_dict = {
                     e: (1 / float(g_beads_subgraph.edges[e]["overlap"])) ** 2
                     * (1 - float(g_beads_subgraph.edges[e]["quality"])) ** 2
                     * np.sqrt(np.max(edge_residuals[e]))
                     * np.log10(
```

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/sample_data.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/sample_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
         x = ndimage.affine_transform(
             im_gt,
             matrix=np.eye(x.ndim) / zoom,
             offset=offset,
             output_shape=output_shape,
             mode="reflect",
+            order=1,
         )[None]
 
         return x
 
     # build the array
     tiles = da.empty(
         (N_t,)
```

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/spatial_image_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/spatial_image_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/mosaic_test.czi` & `multiview_stitcher-0.1.6/src/multiview_stitcher/test-datasets/mosaic_test.czi`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/transformation.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/transformation.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/vis_utils.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/vis_utils.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher/weights.py` & `multiview_stitcher-0.1.6/src/multiview_stitcher/weights.py`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/PKG-INFO` & `multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiview-stitcher
-Version: 0.1.5
+Version: 0.1.6
 Summary: Registration and fusion of large imaging datasets in 2D and 3D.
 Home-page: https://github.com/multiview-stitcher/multiview-stitcher
 Author: Marvin Albert
 Author-email: marvin.albert@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/multiview-stitcher/multiview-stitcher/issues
 Project-URL: Documentation, https://github.com/multiview-stitcher/multiview-stitcher#README.md
```

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/SOURCES.txt` & `multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/requires.txt` & `multiview_stitcher-0.1.6/src/multiview_stitcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `multiview_stitcher-0.1.5/tox.ini` & `multiview_stitcher-0.1.6/tox.ini`

 * *Files identical despite different names*

