# Comparing `tmp/asreview-makita-0.8.0.tar.gz` & `tmp/asreview_makita-0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-makita-0.8.0.tar", last modified: Wed Jan 10 13:50:10 2024, max compression
+gzip compressed data, was "asreview_makita-0.9rc1.tar", last modified: Thu Apr 18 13:14:58 2024, max compression
```

## Comparing `asreview-makita-0.8.0.tar` & `asreview_makita-0.9rc1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.270572 asreview-makita-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.218572 asreview-makita-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.222571 asreview-makita-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.github/workflows/ci-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.github/workflows/pythonpackage.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.222571 asreview-makita-0.8.0/.github/workflows/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.github/workflows/test_data/labels.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-01-10 13:50:10.270572 asreview-makita-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.270572 asreview-makita-0.8.0/asreview_makita.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-10 13:50:10.000000 asreview-makita-0.8.0/asreview_makita.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.218572 asreview-makita-0.8.0/asreviewcontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.226572 asreview-makita-0.8.0/asreviewcontrib/makita/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/template_arfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/template_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/template_multimodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.226572 asreview-makita-0.8.0/asreviewcontrib/makita/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/doc_README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_get_plot.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_metrics.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_tds.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_arfi.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_basic.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_multimodel.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/asreviewcontrib/makita/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.226572 asreview-makita-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.226572 asreview-makita-0.8.0/examples/arfi_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.230572 asreview-makita-0.8.0/examples/arfi_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.242572 asreview-makita-0.8.0/examples/arfi_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/arfi_example/scripts/merge_tds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.242572 asreview-makita-0.8.0/examples/basic_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.246572 asreview-makita-0.8.0/examples/basic_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.254572 asreview-makita-0.8.0/examples/basic_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/basic_example/scripts/merge_tds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.254572 asreview-makita-0.8.0/examples/multimodel_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.258572 asreview-makita-0.8.0/examples/multimodel_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13063 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:50:10.270572 asreview-makita-0.8.0/examples/multimodel_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_tds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-10 13:49:57.000000 asreview-makita-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 13:50:10.270572 asreview-makita-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.290781 asreview_makita-0.9rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.294781 asreview_makita-0.9rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/ci-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/pythonpackage.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.294781 asreview_makita-0.9rc1/.github/workflows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/test_data/labels.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/asreview_makita.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.290781 asreview_makita-0.9rc1/asreviewcontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/asreviewcontrib/makita/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_arfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_multimodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/doc_README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_plot.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_metrics.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_tds.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_arfi.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_basic.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_multimodel.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/examples/arfi_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/examples/arfi_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.302781 asreview_makita-0.9rc1/examples/arfi_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.310781 asreview_makita-0.9rc1/examples/arfi_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_tds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.310781 asreview_makita-0.9rc1/examples/basic_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.314781 asreview_makita-0.9rc1/examples/basic_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.326781 asreview_makita-0.9rc1/examples/basic_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_tds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.326781 asreview_makita-0.9rc1/examples/multimodel_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.330782 asreview_makita-0.9rc1/examples/multimodel_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13063 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/examples/multimodel_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_tds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/setup.cfg
```

### Comparing `asreview-makita-0.8.0/.github/workflows/pythonpackage.yml` & `asreview_makita-0.9rc1/.github/workflows/pythonpackage.yml`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
```

### Comparing `asreview-makita-0.8.0/.github/workflows/test_data/labels.csv` & `asreview_makita-0.9rc1/.github/workflows/test_data/labels.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/.gitignore` & `asreview_makita-0.9rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/CITATION.cff` & `asreview_makita-0.9rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/LICENSE` & `asreview_makita-0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/PKG-INFO` & `asreview_makita-0.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: asreview-makita
-Version: 0.8.0
+Version: 0.9rc1
 Summary: Makita workflow tool for the ASReview project
 Author-email: ASReview LAB developers <asreview@uu.nl>
 License: MIT
 Project-URL: homepage, https://asreview.ai
 Project-URL: repository, https://github.com/asreview/asreview-makita
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asreview
+Requires-Dist: asreview<2,>=1
 Requires-Dist: jinja2
 Requires-Dist: cfgtemplater
 Provides-Extra: lint
 Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
@@ -143,14 +144,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -170,14 +172,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -197,31 +200,32 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
-  --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
-  --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
+  --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
+  --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
-`--feature_extractors`, and `--impossible_models` option. For instance, if you
+`--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
 `tfidf`, use the following command:
 
 ```console
-asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --impossible_models nb,doc2vec logistic,tfidf
+asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --query_strategies max max_random max_uncertainty cluster --impossible_models nb,doc2vec logistic,tfidf
 ```
 
 ## Advanced usage
 
 ### Create and use custom templates
 
 It is possible to overwrite the internal templates. This can be useful for simulation studies with different needs.
```

### Comparing `asreview-makita-0.8.0/README.md` & `asreview_makita-0.9rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -144,14 +145,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -171,31 +173,32 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
-  --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
-  --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
+  --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
+  --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
-`--feature_extractors`, and `--impossible_models` option. For instance, if you
+`--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
 `tfidf`, use the following command:
 
 ```console
-asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --impossible_models nb,doc2vec logistic,tfidf
+asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --query_strategies max max_random max_uncertainty cluster --impossible_models nb,doc2vec logistic,tfidf
 ```
 
 ## Advanced usage
 
 ### Create and use custom templates
 
 It is possible to overwrite the internal templates. This can be useful for simulation studies with different needs.
```

### Comparing `asreview-makita-0.8.0/asreview_makita.egg-info/PKG-INFO` & `asreview_makita-0.9rc1/asreview_makita.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: asreview-makita
-Version: 0.8.0
+Version: 0.9rc1
 Summary: Makita workflow tool for the ASReview project
 Author-email: ASReview LAB developers <asreview@uu.nl>
 License: MIT
 Project-URL: homepage, https://asreview.ai
 Project-URL: repository, https://github.com/asreview/asreview-makita
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asreview
+Requires-Dist: asreview<2,>=1
 Requires-Dist: jinja2
 Requires-Dist: cfgtemplater
 Provides-Extra: lint
 Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
@@ -143,14 +144,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -170,14 +172,15 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
   --no_wordclouds                           Disables the generation of wordclouds.
+  --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
 ```
@@ -197,31 +200,32 @@
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
   --no_wordclouds                           Disables the generation of wordclouds.
-  --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
-  --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
+  --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
+  --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
-`--feature_extractors`, and `--impossible_models` option. For instance, if you
+`--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
 `tfidf`, use the following command:
 
 ```console
-asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --impossible_models nb,doc2vec logistic,tfidf
+asreview makita template multimodel --classifiers logistic nb --feature_extractors tfidf doc2vec --query_strategies max max_random max_uncertainty cluster --impossible_models nb,doc2vec logistic,tfidf
 ```
 
 ## Advanced usage
 
 ### Create and use custom templates
 
 It is possible to overwrite the internal templates. This can be useful for simulation studies with different needs.
```

### Comparing `asreview-makita-0.8.0/asreview_makita.egg-info/SOURCES.txt` & `asreview_makita-0.9rc1/asreview_makita.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 asreview_makita.egg-info/entry_points.txt
 asreview_makita.egg-info/requires.txt
 asreview_makita.egg-info/top_level.txt
 asreviewcontrib/makita/__init__.py
 asreviewcontrib/makita/config.py
 asreviewcontrib/makita/entrypoint.py
 asreviewcontrib/makita/template_arfi.py
+asreviewcontrib/makita/template_base.py
 asreviewcontrib/makita/template_basic.py
 asreviewcontrib/makita/template_multimodel.py
 asreviewcontrib/makita/utils.py
 asreviewcontrib/makita/templates/doc_README.md.template
 asreviewcontrib/makita/templates/script_get_plot.py.template
 asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
 asreviewcontrib/makita/templates/script_merge_descriptives.py.template
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/doc_README.md.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/doc_README.md.template`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 ## Installation
 
 This project depends on Python 3.7 or later (python.org/download), and [ASReview](https://asreview.nl/download/). Install the following dependencies to run the simulation and analysis in this project.
 
 ```sh
 pip install asreview>=1.0 asreview-insights>=1.1.2 asreview-datatools
 ```
-
-If wordcloud images are required, install the following dependencies.
+{% if not skip_wordclouds %}
+For generating wordclouds, install the following dependencies.
 
 ```sh
 pip install asreview-wordcloud
 ```
-
+{% endif %}
 ## Data
 
 The performance on the following datasets is evaluated:
 
 {% for dataset in datasets %}- {{ dataset }}
 {% endfor %}
 ## Run simulation
@@ -66,11 +66,10 @@
         |   ├── 📜tds_summary.xlsx{% for dataset in datasets %}
         |   ├── 📜metrics_sim_{{ dataset.stem }}_metrics.csv
         |   ├── 📜metrics_sim_{{ dataset.stem }}_metrics.xlsx{% endfor %}
         |   ├── 📜metrics_summary.csv
         |   └── 📜metrics_summary.xlsx
         └── 📂figures{% for dataset in datasets %}
             ├── 📈plot_recall_{{ dataset.stem }}.png{% endfor %}{% for dataset in datasets %}
-            ├── 📈wordcloud_{{ dataset.stem }}.png
+{% if not skip_wordclouds %}            ├── 📈wordcloud_{{ dataset.stem }}.png
             ├── 📈wordcloud_relevant_{{ dataset.stem }}.png
-            └── 📈wordcloud_irrelevant_{{ dataset.stem }}.png{% endfor %}
-{%endif %}
+            └── 📈wordcloud_irrelevant_{{ dataset.stem }}.png{%endif %}{% endfor %}{%endif %}
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_get_plot.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_plot.py.template`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,21 @@
     metadata = state.settings_metadata
     label = None
 
     if legend_option == "filename":
         label = state_file.stem
     elif legend_option == "model":
         label = " - ".join(
-            [metadata["settings"]["model"],
-             metadata["settings"]["feature_extraction"],
-             metadata["settings"]["balance_strategy"],
-             metadata["settings"]["query_strategy"]])
+            [
+                metadata["settings"]["model"],
+                metadata["settings"]["feature_extraction"],
+                metadata["settings"]["balance_strategy"],
+                metadata["settings"]["query_strategy"],
+            ]
+        )
     elif legend_option == "classifier":
         label = metadata["settings"]["model"]
     else:
         try:
             label = metadata["settings"][legend_option]
         except KeyError as err:
             raise ValueError(f"Invalid legend setting: '{legend_option}'") from err  # noqa: E501
@@ -78,35 +81,30 @@
     for state_file in states:
         with open_state(state_file) as state:
             plot_recall(ax, state)
             if legend:
                 _set_legend(ax, state, legend, label_to_line, state_file)
 
     if legend:
-        ax.legend(loc=4, prop={'size': 8})
+        ax.legend(loc=4, prop={"size": 8})
     fig.savefig(str(filename))
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         description="Generate an ASReview plot from the found state files."
     )
+    parser.add_argument("-s", type=str, help="States location")
+    parser.add_argument("-o", type=str, help="Output location")
     parser.add_argument(
-        "-s",
-        type=str,
-        help="States location")
-    parser.add_argument(
-        "-o",
+        "--show_legend",
+        "-l",
         type=str,
-        help="Output location")
-    parser.add_argument(
-        "--show_legend", "-l",
-        type=str,
-        help="Add a legend to the plot, based on the given parameter.")
+        help="Add a legend to the plot, based on the given parameter.",
+    )
     args = parser.parse_args()
 
     # load states
     states = list(Path(args.s).glob("*.asreview"))
 
     # check if states are found
     if len(states) == 0:
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template`

 * *Files 16% similar despite different names*

```diff
@@ -32,32 +32,21 @@
         Dict with model settings.
 
     """
 
     return state.settings.to_dict()
 
 
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser(
-        description='Convert ASReview state file to CSV'
-    )
-    parser.add_argument(
-        's',
-        type=str,
-        help='State file location')
-    parser.add_argument(
-        'o',
-        type=str,
-        help='Export file location (json)')
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="Convert ASReview state file to CSV")
+    parser.add_argument("s", type=str, help="State file location")
+    parser.add_argument("o", type=str, help="Export file location (json)")
     args = parser.parse_args()
 
     with open_state(args.s) as state:
-
         result = get_settings_from_state(state)
 
     # store result in output folder
     Path(args.o).parent.mkdir(parents=True, exist_ok=True)
 
     with open(Path(args.o), "w") as f:
         json.dump(result, f)
-
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_descriptives.py.template` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_descriptives.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 > python scripts/merge_descriptives.py -o my_table.json
 
 Authors
 -------
 - De Bruin, Jonathan
 """
 
-# version {{ version }}
+# version 0.0.0
 
 import argparse
 import glob
 import json
 from pathlib import Path
 
 import pandas as pd
@@ -31,39 +31,40 @@
 def create_table_descriptives(datasets):
     """Merge dataset descriptives."""
 
     stats = []
 
     for ds in datasets:
         with open(ds) as f:
-            data = json.load(f)['data']['items']
+            data = json.load(f)["data"]["items"]
             values = {}
             for item in data:
-                values[item['id']] = item['value']
+                values[item["id"]] = item["value"]
             stats.append(values)
 
     df = pd.DataFrame(stats, index=[Path(ds).name for ds in datasets])
     return df
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         description="Merge descriptives of multiple files into single table."
     )
     parser.add_argument(
         "-s",
         type=str,
-        default="{{ output_folder }}/simulation/*/descriptives/",
-        help="Datasets location")
+        default="output/simulation/*/descriptives/",
+        help="Datasets location",
+    )
     parser.add_argument(
         "-o",
         type=str,
-        default="{{ output_folder }}/tables/data_descriptives_all.csv",
-        help="Output table location")
+        default="output/tables/data_descriptives_all.csv",
+        help="Output table location",
+    )
     args = parser.parse_args()
 
     # load datasets
     datasets = glob.glob(args.s + "data_stats_*.json")
 
     # check if states are found
     if len(datasets) == 0:
@@ -71,9 +72,8 @@
 
     # merge results
     result = create_table_descriptives(datasets)
 
     # store result in output folder
     Path(args.o).parent.mkdir(parents=True, exist_ok=True)
     result.to_csv(Path(args.o))
-    result.to_excel(Path(args.o).with_suffix('.xlsx'))
-
+    result.to_excel(Path(args.o).with_suffix(".xlsx"))
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_metrics.py.template` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,61 +14,59 @@
 > python scripts/merge_metrics.py -o my_table.json
 
 Authors
 -------
 - De Bruin, Jonathan
 """
 
-# version {{ version }}
+# version 0.0.0
 
 import argparse
 import glob
 import json
 from pathlib import Path
 
 import pandas as pd
 
 
 def create_table_state_metrics(metric_files):
     metrics = []
 
     for metric in metric_files:
         with open(metric) as f:
-            data = json.load(f)['data']['items']
+            data = json.load(f)["data"]["items"]
             values = {}
-            values['file_name'] = Path(metric).name
+            values["file_name"] = Path(metric).name
             for item in data:
-                if item['id'] == 'td':
+                if item["id"] == "td":
                     continue
                 # check if value is a list
-                if item['value'] is not None and isinstance(item['value'], list):
-                    for value in item['value']:
-                        values[item['id'] + "_" + str(value[0])] = value[1]
+                if item["value"] is not None and isinstance(item["value"], list):
+                    for value in item["value"]:
+                        values[item["id"] + "_" + str(value[0])] = value[1]
                 else:
-                    values[item['id']] = item['value']
+                    values[item["id"]] = item["value"]
             metrics.append(values)
 
     return pd.DataFrame(metrics)
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         description="Merge metrics of multiple states into single table."
     )
     parser.add_argument(
-        "-s",
-        type=str,
-        default="{{ output_folder }}/simulation/*/metrics/",
-        help="states location")
+        "-s", type=str, default="output/simulation/*/metrics/", help="states location"
+    )
     parser.add_argument(
         "-o",
         type=str,
-        default="{{ output_folder }}/tables/metrics_sim_all.csv",
-        help="Output table location")
+        default="output/tables/metrics_sim_all.csv",
+        help="Output table location",
+    )
     args = parser.parse_args()
 
     # load metric files
     metric_files = glob.glob(args.s + "metrics_sim_*.json")
 
     # check if states are found
     if len(metric_files) == 0:
@@ -76,9 +74,8 @@
 
     # merge results
     result = create_table_state_metrics(metric_files)
 
     # store result in output folder
     Path(args.o).parent.mkdir(parents=True, exist_ok=True)
     result.to_csv(Path(args.o))
-    result.to_excel(Path(args.o).with_suffix('.xlsx'))
-
+    result.to_excel(Path(args.o).with_suffix(".xlsx"))
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_merge_tds.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_tds.py.template`

 * *Files 12% similar despite different names*

```diff
@@ -32,65 +32,59 @@
 
 def create_table_state_tds(metrics):
     values = []
     file_counter = 0
 
     for metric in metrics:
         with open(metric) as f:
-            i = next(filter(lambda x: x['id'] == 'td', json.load(f)['data']['items']))['value']  # noqa
+            i = next(filter(lambda x: x["id"] == "td", json.load(f)["data"]["items"]))[
+                "value"
+            ]
             values.extend((item[0], item[1], file_counter) for item in i)
             file_counter += 1
 
-    df = pd.DataFrame(values, columns=['record_id', 'td', 'metric_file'])
-    pivoted = df.pivot_table(index='record_id',
-                             columns='metric_file',
-                             values='td',
-                             aggfunc='first',
-                             fill_value=nan)
-    pivoted.columns = [f'td_sim_{col}' for col in pivoted.columns]
+    df = pd.DataFrame(values, columns=["record_id", "td", "metric_file"])
+    pivoted = df.pivot_table(
+        index="record_id",
+        columns="metric_file",
+        values="td",
+        aggfunc="first",
+        fill_value=nan,
+    )
+    pivoted.columns = [f"td_sim_{col}" for col in pivoted.columns]
     return pivoted
 
 
 def get_atd_values(df):
+    df["record_atd"] = df.mean(axis=1)
 
-    df['record_atd'] = df.mean(axis=1)
-
-    df.loc['average_simulation_TD'] = df.iloc[:, :-1].mean(axis=0)
+    df.loc["average_simulation_TD"] = df.iloc[:, :-1].mean(axis=0)
 
     return df
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Merge tds of multiple metrics into single table."
     )
-    parser.add_argument(
-        "-s",
-        type=str,
-        required=True,
-        help="metrics location")
-    parser.add_argument(
-        "-o",
-        type=str,
-        required=True,
-        help="Output table location")
+    parser.add_argument("-s", type=str, required=True, help="metrics location")
+    parser.add_argument("-o", type=str, required=True, help="Output table location")
     args = parser.parse_args()
 
     # load metric files
     metric_files = glob.glob(args.s + "metrics_sim_*.json")
 
     # check if states are found
     if len(metric_files) == 0:
         raise FileNotFoundError("No metrics found in " + args.s)
 
     # check if output file has .csv extension
-    if Path(args.o).suffix != '.csv':
+    if Path(args.o).suffix != ".csv":
         raise ValueError("Output file should have .csv extension")
 
     td_table = create_table_state_tds(metric_files)
     atd_table = get_atd_values(td_table)
 
     # store table
     Path(args.o).parent.mkdir(parents=True, exist_ok=True)
     atd_table.to_csv(Path(args.o))
-    atd_table.to_excel(Path(args.o).with_suffix('.xlsx'))
-
+    atd_table.to_excel(Path(args.o).with_suffix(".xlsx"))
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,7 @@
         nargs="*",
         default=None,
         type=str,
         help='Suffix for the new datasets.')
     args = parser.parse_args()
 
     etl(args.s, args.o, split=args.split, suffix=args.suffix)
-
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_arfi.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_arfi.txt.template`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # Create output folder
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics
 
 # Collect descriptives about the dataset
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives
 python -m asreview data describe {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/data_stats_{{ dataset.input_file_stem }}.json
-{% if create_wordclouds %}
+{% if not skip_wordclouds %}
 
 # Generate wordcloud visualizations of all datasets
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_{{ dataset.input_file_stem }}.png --width 800 --height 500
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_relevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --relevant
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_irrelevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --irrelevant
 {% endif %}
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_basic.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_basic.txt.template`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 # Create output folder
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics
 
 # Collect descriptives about the dataset {{ dataset.input_file_stem }}
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives
 python -m asreview data describe {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/data_stats_{{ dataset.input_file_stem }}.json
-{% if create_wordclouds %}
+{% if not skip_wordclouds %}
 
 # Generate wordcloud visualizations of all datasets
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_{{ dataset.input_file_stem }}.png --width 800 --height 500
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_relevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --relevant
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_irrelevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --irrelevant
 {% endif %}
 
 # Simulate runs
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files
-{% for run in range(dataset.n_runs) %}
-python -m asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ run }}.asreview --init_seed {{ dataset.init_seed + run }} --seed {{ dataset.model_seed + run }} -m {{ classifier }} -e {{ feature_extractor }} -q {{ query_strategy }} -b {{ balance_strategy }} --n_instances {{ instances_per_query }} --stop_if {{ stop_if }}
-python -m asreview metrics {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ run }}.asreview -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/metrics_sim_{{ dataset.input_file_stem }}_{{ run }}.json
+{% for run in range(n_runs) %}
+python -m asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}{{ "_{}".format(run) if n_runs > 1 else "" }}.asreview --init_seed {{ dataset.init_seed + run }} --seed {{ dataset.model_seed + run }} -m {{ classifier }} -e {{ feature_extractor }} -q {{ query_strategy }} -b {{ balance_strategy }} --n_instances {{ instances_per_query }} --stop_if {{ stop_if }}
+python -m asreview metrics {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}{{ "_{}".format(run) if n_runs > 1 else "" }}.asreview -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/metrics_sim_{{ dataset.input_file_stem }}{{ "_{}".format(run) if n_runs > 1 else "" }}.json
 {% endfor %}
 
 # Generate plot and tables for dataset
 python {{ scripts_folder }}/get_plot.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/ -o {{ output_folder }}/figures/plot_recall_sim_{{ dataset.input_file_stem }}.png
 python {{ scripts_folder }}/merge_metrics.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/ -o {{ output_folder }}/tables/metrics/metrics_sim_{{ dataset.input_file_stem }}.csv
 python {{ scripts_folder }}/merge_tds.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/ -o {{ output_folder }}/tables/time_to_discovery/tds_sim_{{ dataset.input_file_stem }}.csv
 {% endfor %}
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/templates/template_multimodel.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_multimodel.txt.template`

 * *Files 12% similar despite different names*

```diff
@@ -31,37 +31,41 @@
 # Create output folder
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics
 
 # Collect descriptives about the dataset {{ dataset.input_file_stem }}
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives
 python -m asreview data describe {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/data_stats_{{ dataset.input_file_stem }}.json
-{% if create_wordclouds %}
+{% if not skip_wordclouds %}
 
 # Generate wordcloud visualizations of all datasets
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_{{ dataset.input_file_stem }}.png --width 800 --height 500
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_relevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --relevant
 python -m asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/figures/wordcloud_irrelevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --irrelevant
 {% endif %}
 
 # Simulate runs
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files
 {% for classifier in all_classifiers %}
 {% for feature_extraction in all_feature_extractors %}
+{% for query_strategy in all_query_strategies %}
+{% for balance_strategy in all_balance_strategies %}
 {% set temp = [] %}{{ temp.append(classifier)|default("", True) }}{{ temp.append(feature_extraction)|default("", True) }}
 {% if temp in impossible_models %}
 
-# Skipped {{ classifier }} + {{ feature_extraction }} model
-{% else %}# Classifier = {{ classifier }}, Feature extractor = {{ feature_extraction }} , Query strategy = max
+# Skipped {{ classifier }} + {{ feature_extraction }} + {{ query_strategy}} model
+{% else %}# Classifier = {{ classifier }}, Feature extractor = {{ feature_extraction }}, Query strategy = {{ query_strategy }}, Balance strategy = {{balance_strategy}}
 {% for run in range(n_runs) %}
-python -m asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ run }}.asreview --model {{ classifier }} --query_strategy max --feature_extraction {{ feature_extraction }} --init_seed {{ dataset.init_seed + run }} --seed {{ dataset.model_seed }} -q {{ query_strategy }} -b {{ balance_strategy }} --n_instances {{ instances_per_query }} --stop_if {{ stop_if }}
-python -m asreview metrics {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ run }}.asreview -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/metrics_sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ run }}.json
+python -m asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ query_strategy }}_{{ balance_strategy }}{{ "_{}".format(run) if n_runs > 1 else "" }}.asreview --model {{ classifier }} --query_strategy {{query_strategy}} --feature_extraction {{ feature_extraction }} --init_seed {{ dataset.init_seed + run }} --seed {{ dataset.model_seed }} -q {{ query_strategy }} -b {{ balance_strategy }} --n_instances {{ instances_per_query }} --stop_if {{ stop_if }}
+python -m asreview metrics {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ query_strategy }}_{{ balance_strategy }}{{ "_{}".format(run) if n_runs > 1 else "" }}.asreview -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/metrics_sim_{{ dataset.input_file_stem }}_{{ classifier }}_{{ feature_extraction }}_{{ query_strategy }}_{{ balance_strategy }}{{ "_{}".format(run) if n_runs > 1 else "" }}.json
 {% endfor %}{% endif %}
 {% endfor %}
 {% endfor %}
+{% endfor %}
+{% endfor %}
 
 # Generate plot and tables for dataset
 python {{ scripts_folder }}/get_plot.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/ -o {{ output_folder }}/figures/plot_recall_sim_{{ dataset.input_file_stem }}.png --show_legend model
 python {{ scripts_folder }}/merge_metrics.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/ -o {{ output_folder }}/tables/metrics/metrics_sim_{{ dataset.input_file_stem }}.csv
 python {{ scripts_folder }}/merge_tds.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/ -o {{ output_folder }}/tables/time_to_discovery/tds_sim_{{ dataset.input_file_stem }}.csv
 {% endfor %}
```

### Comparing `asreview-makita-0.8.0/asreviewcontrib/makita/utils.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 class FileHandler:
     """
     The FileHandler class handles file operations such as adding files and rendering
     scripts.
     """
 
-    def __init__(self):
-        self.overwrite_all = False
-        self.total_files = 0
+    def __init__(self, allow_overwrite=False):
+        self.overwrite_all = allow_overwrite
+        self._total_files = 0
 
     def add_file(self, content, export_fp):
         """
         Add a file to the specified directory.
 
         Args:
         content (str): The content to be written into the file.
@@ -46,24 +46,26 @@
         # If the file does not exist, or overwrite all is True, or the user allows it:
         if not Path(export_fp).exists() or self.overwrite_all or allow_overwrite():
             # store result in output folder
             Path(export_fp).parent.mkdir(parents=True, exist_ok=True)
 
             with open(export_fp, "w") as f:
                 f.write(content)
+                f.write("\n")
 
-            print(f"Added {export_fp}")
-            self.total_files += 1
+            print(f"Created {export_fp}")
+
+            self._total_files += 1
 
     def print_summary(self):
         """
         Print the total number of files created by the FileHandler object.
         """
 
-        print(f"{self.total_files} file(s) created.")
+        print(f"\n{self._total_files} file(s) created.")
 
     def render_file_from_template(self, name, file_type, **kwargs):
         """
         Render a file from a template.
 
         Args:
         name (str): The name of the file to be rendered.
@@ -74,29 +76,12 @@
         str: The content of the file rendered from the template.
         """
 
         params = {
             "version": __version__,
         }
 
-        print(f"Loading {file_type} {name}")
-
         # open template
         with open(Path(TEMPLATES_FP, f"{file_type}_{name}.template")) as f:
             template = Template(f.read())
 
         return template.render({**params, **kwargs})
-
-
-def check_filename_dataset(fp):
-    """
-    Check if the filename of the dataset contains any whitespace.
-
-    Args:
-    fp (str): The file path of the dataset.
-
-    Raises:
-    ValueError: If the filename of the dataset contains whitespace.
-    """
-
-    if " " in Path(fp).stem:
-        raise ValueError(f"Dataset filename '{fp}' cannot contain whitespace.")
```

### Comparing `asreview-makita-0.8.0/examples/README.md` & `asreview_makita-0.9rc1/examples/README.md`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/README.md` & `asreview_makita-0.9rc1/examples/arfi_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/arfi_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/arfi_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/jobs.sh` & `asreview_makita-0.9rc1/examples/arfi_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_descriptives.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_metrics.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/arfi_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/README.md` & `asreview_makita-0.9rc1/examples/basic_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/basic_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/basic_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/jobs.sh` & `asreview_makita-0.9rc1/examples/basic_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_descriptives.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_metrics.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/basic_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/README.md` & `asreview_makita-0.9rc1/examples/multimodel_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/multimodel_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/multimodel_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/jobs.sh` & `asreview_makita-0.9rc1/examples/multimodel_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_descriptives.py.template`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 > python scripts/merge_descriptives.py -o my_table.json
 
 Authors
 -------
 - De Bruin, Jonathan
 """
 
-# version 0.0.0
+# version {{ version }}
 
 import argparse
 import glob
 import json
 from pathlib import Path
 
 import pandas as pd
@@ -48,21 +48,21 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Merge descriptives of multiple files into single table."
     )
     parser.add_argument(
         "-s",
         type=str,
-        default="output/simulation/*/descriptives/",
+        default="{{ output_folder }}/simulation/*/descriptives/",
         help="Datasets location",
     )
     parser.add_argument(
         "-o",
         type=str,
-        default="output/tables/data_descriptives_all.csv",
+        default="{{ output_folder }}/tables/data_descriptives_all.csv",
         help="Output table location",
     )
     args = parser.parse_args()
 
     # load datasets
     datasets = glob.glob(args.s + "data_stats_*.json")
```

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_metrics.py.template`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 > python scripts/merge_metrics.py -o my_table.json
 
 Authors
 -------
 - De Bruin, Jonathan
 """
 
-# version 0.0.0
+# version {{ version }}
 
 import argparse
 import glob
 import json
 from pathlib import Path
 
 import pandas as pd
@@ -51,20 +51,23 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Merge metrics of multiple states into single table."
     )
     parser.add_argument(
-        "-s", type=str, default="output/simulation/*/metrics/", help="states location"
+        "-s",
+        type=str,
+        default="{{ output_folder }}/simulation/*/metrics/",
+        help="states location",
     )
     parser.add_argument(
         "-o",
         type=str,
-        default="output/tables/metrics_sim_all.csv",
+        default="{{ output_folder }}/tables/metrics_sim_all.csv",
         help="Output table location",
     )
     args = parser.parse_args()
 
     # load metric files
     metric_files = glob.glob(args.s + "metrics_sim_*.json")
```

### Comparing `asreview-makita-0.8.0/examples/multimodel_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.8.0/pyproject.toml` & `asreview_makita-0.9rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,35 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 license = {text = "MIT"}
-dependencies = ["asreview", "jinja2", "cfgtemplater"]
+dependencies = ["asreview>=1,<2", "jinja2", "cfgtemplater"]
 dynamic = ["version"]
 requires-python = ">=3.7"
 
 [project.urls]
 homepage = "https://asreview.ai"
 repository = "https://github.com/asreview/asreview-makita"
 
 [project.entry-points."asreview.entry_points"]
 makita = "asreviewcontrib.makita.entrypoint:MakitaEntryPoint"
 
+[project.entry-points."asreview.makita.templates"]
+basic = "asreviewcontrib.makita.template_basic:TemplateBasic"
+arfi = "asreviewcontrib.makita.template_arfi:TemplateARFI"
+multimodel = "asreviewcontrib.makita.template_multimodel:TemplateMultiModel"
+multiple_models = "asreviewcontrib.makita.template_multimodel:TemplateMultiModel"
+
 [project.optional-dependencies]
 lint = ["ruff"]
 test = ["pytest"]
 
 [build-system]
 build-backend = 'setuptools.build_meta'
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
@@ -37,11 +44,12 @@
 [tool.setuptools]
 packages = ["asreviewcontrib"]
 
 [tool.setuptools_scm]
 write_to = "asreviewcontrib/makita/_version.py"
 
 [tool.ruff]
-select = ["E", "F", "UP", "I", "B"]
+lint.select = ["E", "F", "UP", "I", "B"]
+include = ["**/*.py", "**/*.py.template"]
 
-[tool.ruff.isort]
-force-single-line = true
+[tool.ruff.lint.isort]
+force-single-line = true
```

