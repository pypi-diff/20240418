# Comparing `tmp/timeseriesflattener-2.1.0.tar.gz` & `tmp/timeseriesflattener-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.1.0.tar", last modified: Tue Feb 27 11:56:18 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.1.1.tar", last modified: Thu Apr 18 09:45:26 2024, max compression
```

## Comparing `timeseriesflattener-2.1.0.tar` & `timeseriesflattener-2.1.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.755848 timeseriesflattener-2.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.691848 timeseriesflattener-2.1.0/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.691848 timeseriesflattener-2.1.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.683848 timeseriesflattener-2.1.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.691848 timeseriesflattener-2.1.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.695848 timeseriesflattener-2.1.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.695848 timeseriesflattener-2.1.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2764 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.695848 timeseriesflattener-2.1.0/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    72853 2024-02-27 11:56:10.000000 timeseriesflattener-2.1.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11561 2024-02-27 11:56:18.755848 timeseriesflattener-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7629 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.699848 timeseriesflattener-2.1.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.699848 timeseriesflattener-2.1.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.699848 timeseriesflattener-2.1.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    40071 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    24394 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.703848 timeseriesflattener-2.1.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.703848 timeseriesflattener-2.1.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4699 2024-02-27 11:56:10.000000 timeseriesflattener-2.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     4879 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     3885 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 11:56:18.755848 timeseriesflattener-2.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.703848 timeseriesflattener-2.1.0/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.703848 timeseriesflattener-2.1.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      721 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3852 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.707848 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      215 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/default_column_names.py
--rw-r--r--   0 root         (0) root         (0)     3491 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2825 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     5993 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.707848 timeseriesflattener-2.1.0/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.711848 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)     6591 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)     8576 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)     9793 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.711848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.711848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.687848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.683848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.711848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.727848 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-02-27 11:56:08.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6112 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5535 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7823 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35049 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.687848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.687848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.731848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.735848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5446 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3232 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.751848 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:56:18.755848 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11561 2024-02-27 11:56:18.000000 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8537 2024-02-27 11:56:18.000000 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 11:56:18.000000 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      675 2024-02-27 11:56:18.000000 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-27 11:56:18.000000 timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-02-27 11:56:09.000000 timeseriesflattener-2.1.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.270775 timeseriesflattener-2.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.206774 timeseriesflattener-2.1.1/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.206774 timeseriesflattener-2.1.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.198774 timeseriesflattener-2.1.1/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.206774 timeseriesflattener-2.1.1/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.206774 timeseriesflattener-2.1.1/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.210774 timeseriesflattener-2.1.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)      869 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.210774 timeseriesflattener-2.1.1/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    73292 2024-04-18 09:45:20.000000 timeseriesflattener-2.1.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11505 2024-04-18 09:45:26.270775 timeseriesflattener-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7629 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.214774 timeseriesflattener-2.1.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.214774 timeseriesflattener-2.1.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.214774 timeseriesflattener-2.1.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    40071 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    24394 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5314 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.214774 timeseriesflattener-2.1.1/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.218774 timeseriesflattener-2.1.1/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-04-18 09:45:20.000000 timeseriesflattener-2.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 09:45:26.270775 timeseriesflattener-2.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.218774 timeseriesflattener-2.1.1/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.218774 timeseriesflattener-2.1.1/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      721 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.222774 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/default_column_names.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.222774 timeseriesflattener-2.1.1/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      644 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.226774 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)     6595 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)     8576 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.226774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.226774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.198774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.198774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.226774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.242774 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7823 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35049 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.202774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.202774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.246774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.250774 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.262775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5446 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3232 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:45:26.266775 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11505 2024-04-18 09:45:26.000000 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-04-18 09:45:26.000000 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 09:45:26.000000 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-04-18 09:45:26.000000 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-18 09:45:26.000000 timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-04-18 09:45:19.000000 timeseriesflattener-2.1.1/tasks.py
```

### Comparing `timeseriesflattener-2.1.0/.devcontainer/devcontainer.json` & `timeseriesflattener-2.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/actions/test/action.yml` & `timeseriesflattener-2.1.1/.github/actions/test/action.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     description: "Which Python version to run on"
     required: true
 
 runs:
   using: "composite"
   steps:
     - name: Checkout (GitHub)
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Replace python version in Dockerfile
       shell: bash
       run: |
         sed -i '/python:.*/c\FROM python:${{ inputs.python-version }}' Dockerfile
 
     - name: Create github hosts file
```

### Comparing `timeseriesflattener-2.1.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.1.1/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/dependabot.yml` & `timeseriesflattener-2.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/recommended_repo_setup.md` & `timeseriesflattener-2.1.1/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/workflows/benchmark.yml` & `timeseriesflattener-2.1.1/.github/workflows/benchmark.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   # performance analysis in order to generate initial data.
   workflow_dispatch:
 
 jobs:
   benchmarks:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: actions/setup-python@v3
         with:
           python-version: "3.9"
 
       - name: Install dependencies
         run: pip install .[test]
```

### Comparing `timeseriesflattener-2.1.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.1.1/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.1.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.1.1/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.1.1/.github/workflows/main_test_and_release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     env:
       python-version: ${{ matrix.python-version }}
 
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Run tests
         uses: ./.github/actions/test
         with:
           python-version: ${{ env.python-version }}
 
   jupyter-tutorials:
@@ -41,15 +41,15 @@
 
     strategy:
       matrix:
         os: [ubuntu-latest]
 
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Run tests
         uses: ./.github/actions/test_tutorials
         with:
           python-version: ${{ env.python-version }}
 
   release:
```

### Comparing `timeseriesflattener-2.1.0/.github/workflows/stalebot.yml` & `timeseriesflattener-2.1.1/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.1.1/.github/workflows/static_type_checks.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   static_type_checks:
     runs-on: ubuntu-latest
     permissions:
       pull-requests: write
     steps:
       - name: Checkout (GitHub)
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Create github hosts file
         run: | # If this file is not created, the dev container fails because of non-existent mount
           mkdir -p ~/.config/gh
           touch ~/.config/gh/hosts.yml
 
       - name: Pre-build dev container image
```

### Comparing `timeseriesflattener-2.1.0/.gitignore` & `timeseriesflattener-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.pre-commit-config.yaml` & `timeseriesflattener-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.vscode/tasks.json` & `timeseriesflattener-2.1.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/.zenodo.json` & `timeseriesflattener-2.1.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/CHANGELOG.md` & `timeseriesflattener-2.1.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.1 (2024-04-18)
+
+### Fix
+
+* Add option to set entity_id_col_name_out in legacy predictor group spec ([`4094dc1`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/4094dc103fb7b2ed18143c8104504f897e8f37fa))
+
+### Documentation
+
+* Update pre-commit.yml highlight legacy spec change ([`fcff53e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/fcff53efe2417ee65c7f97452bcd201f1f0d0dc0))
+
 ## v2.1.0 (2024-02-27)
 
 ### Feature
 
 * **#515:** Make the output col name of BooleanOutcomeSpec user-definable ([#522](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/issues/522)) ([`2082d01`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/2082d010c21d7dd0567b4aa29f615476e979c4e4))
 
 ### Fix
```

### Comparing `timeseriesflattener-2.1.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/CONTRIBUTING.md` & `timeseriesflattener-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/Dockerfile` & `timeseriesflattener-2.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/LICENSE` & `timeseriesflattener-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/PKG-INFO` & `timeseriesflattener-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.1.0
+Version: 2.1.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -46,28 +46,27 @@
 Requires-Dist: numpy>=1.23.3
 Requires-Dist: pyarrow>=8.0.0
 Requires-Dist: protobuf<=4.24.4
 Requires-Dist: frozendict>=2.3.4
 Requires-Dist: coloredlogs>14.0.0
 Requires-Dist: tqdm>4.1.0
 Requires-Dist: polars>0.19.0
-Requires-Dist: iterpy>=1.6.0
+Requires-Dist: iterpy==1.6.0
 Requires-Dist: rich>=13.0.0
 Provides-Extra: dev
 Requires-Dist: pyright==1.1.330.post0; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev"
 Requires-Dist: ruff==0.2.1; extra == "dev"
-Requires-Dist: pandas-stubs; extra == "dev"
+Requires-Dist: pandas-stubs==2.2.0.240218; extra == "dev"
 Requires-Dist: invoke==2.1.1; extra == "dev"
-Requires-Dist: lumberman; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest<7.3.0,>=7.1.3; extra == "test"
-Requires-Dist: pytest-cov<3.1.0,>=3.0.0; extra == "test"
-Requires-Dist: pytest-xdist<3.2.0,>=3.0.0; extra == "test"
-Requires-Dist: pytest-sugar<0.10.0,>=0.9.4; extra == "test"
+Requires-Dist: pytest==7.2.2; extra == "test"
+Requires-Dist: pytest-cov==3.0.0; extra == "test"
+Requires-Dist: pytest-xdist==3.1.0; extra == "test"
+Requires-Dist: pytest-sugar==0.9.7; extra == "test"
 Requires-Dist: pytest-testmon==2.1.0; extra == "test"
 Requires-Dist: pytest-benchmark==4.0.0; extra == "test"
 Requires-Dist: pytest-codspeed==2.2.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: furo==2023.3.27; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -28,23 +28,22 @@
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: <3.13.0,>=3.8.0 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: scipy>=1.8.0 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: pydantic>=2.0.0 Requires-Dist: pandas<=2.1.3,>=1.4.0 Requires-
 Dist: catalogue>=2.0.0 Requires-Dist: numpy>=1.23.3 Requires-Dist:
 pyarrow>=8.0.0 Requires-Dist: protobuf<=4.24.4 Requires-Dist: frozendict>=2.3.4
 Requires-Dist: coloredlogs>14.0.0 Requires-Dist: tqdm>4.1.0 Requires-Dist:
-polars>0.19.0 Requires-Dist: iterpy>=1.6.0 Requires-Dist: rich>=13.0.0
+polars>0.19.0 Requires-Dist: iterpy==1.6.0 Requires-Dist: rich>=13.0.0
 Provides-Extra: dev Requires-Dist: pyright==1.1.330.post0; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev" Requires-Dist: ruff==0.2.1;
-extra == "dev" Requires-Dist: pandas-stubs; extra == "dev" Requires-Dist:
-invoke==2.1.1; extra == "dev" Requires-Dist: lumberman; extra == "dev"
-Provides-Extra: test Requires-Dist: pytest<7.3.0,>=7.1.3; extra == "test"
-Requires-Dist: pytest-cov<3.1.0,>=3.0.0; extra == "test" Requires-Dist: pytest-
-xdist<3.2.0,>=3.0.0; extra == "test" Requires-Dist: pytest-
-sugar<0.10.0,>=0.9.4; extra == "test" Requires-Dist: pytest-testmon==2.1.0;
+extra == "dev" Requires-Dist: pandas-stubs==2.2.0.240218; extra == "dev"
+Requires-Dist: invoke==2.1.1; extra == "dev" Provides-Extra: test Requires-
+Dist: pytest==7.2.2; extra == "test" Requires-Dist: pytest-cov==3.0.0; extra ==
+"test" Requires-Dist: pytest-xdist==3.1.0; extra == "test" Requires-Dist:
+pytest-sugar==0.9.7; extra == "test" Requires-Dist: pytest-testmon==2.1.0;
 extra == "test" Requires-Dist: pytest-benchmark==4.0.0; extra == "test"
 Requires-Dist: pytest-codspeed==2.2.0; extra == "test" Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs" Requires-Dist: furo==2023.3.27;
 extra == "docs" Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "docs" Requires-Dist: myst-
 nb==0.17.2; extra == "docs" Requires-Dist: sphinx_design==0.3.0; extra ==
 "docs" Provides-Extra: tutorials Requires-Dist: jupyter<1.1.0,>=1.0.0; extra ==
```

### Comparing `timeseriesflattener-2.1.0/README.md` & `timeseriesflattener-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/citation.cff` & `timeseriesflattener-2.1.1/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/Makefile` & `timeseriesflattener-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/_static/favicon.ico` & `timeseriesflattener-2.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/_static/icon.png` & `timeseriesflattener-2.1.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/_static/icon_dark.png` & `timeseriesflattener-2.1.1/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/_static/terminology_figure.png` & `timeseriesflattener-2.1.1/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/conf.py` & `timeseriesflattener-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/faq.rst` & `timeseriesflattener-2.1.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/feature_specifications.rst` & `timeseriesflattener-2.1.1/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/index.rst` & `timeseriesflattener-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.1.1/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.1.1/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.1.1/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.1.1/docs/tutorials/04_from_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.1.1/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.1.1/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.1.1/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.1.1/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/example.py` & `timeseriesflattener-2.1.1/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/icon.png` & `timeseriesflattener-2.1.1/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/paper/paper.bib` & `timeseriesflattener-2.1.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/paper/paper.md` & `timeseriesflattener-2.1.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/pyproject.toml` & `timeseriesflattener-2.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
@@ -19,48 +19,47 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8.0,<3.13.0"
 dependencies = [
-    "scipy>=1.8.0",
-    "scikit-learn>=1.1.2",
-    "pydantic>=2.0.0",
-    "pandas>=1.4.0,<=2.1.3",
-    "catalogue>=2.0.0",
-    "numpy>=1.23.3",
-    "pyarrow>=8.0.0",
-    "protobuf<=4.24.4",
-    # Other versions give errors with pytest, super weird!
-    "frozendict>=2.3.4",
-    "coloredlogs>14.0.0",
-    "tqdm>4.1.0",
-    "polars>0.19.0",
-    "iterpy>=1.6.0",
-    "rich>=13.0.0",
+  "scipy>=1.8.0",
+  "scikit-learn>=1.1.2",
+  "pydantic>=2.0.0",
+  "pandas>=1.4.0,<=2.1.3",
+  "catalogue>=2.0.0",
+  "numpy>=1.23.3",
+  "pyarrow>=8.0.0",
+  "protobuf<=4.24.4",
+  # Other versions give errors with pytest, super weird!
+  "frozendict>=2.3.4",
+  "coloredlogs>14.0.0",
+  "tqdm>4.1.0",
+  "polars>0.19.0",
+  "iterpy==1.6.0",
+  "rich>=13.0.0",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
   "pyright==1.1.330.post0",
   "pre-commit==3.4.0",
-  "ruff==0.2.1",            # important that these match the pre-commit hooks
-  "pandas-stubs",           # type stubs for pandas
+  "ruff==0.2.1",                # important that these match the pre-commit hooks
+  "pandas-stubs==2.2.0.240218", # type stubs for pandas
   "invoke==2.1.1",
-  "lumberman",
 ]
 test = [
-  "pytest>=7.1.3,<7.3.0",
-  "pytest-cov>=3.0.0,<3.1.0",
-  "pytest-xdist>=3.0.0,<3.2.0",
-  "pytest-sugar>=0.9.4,<0.10.0",
+  "pytest==7.2.2",
+  "pytest-cov==3.0.0",
+  "pytest-xdist==3.1.0",
+  "pytest-sugar==0.9.7",
   "pytest-testmon==2.1.0",
   "pytest-benchmark==4.0.0",
   "pytest-codspeed==2.2.0",
 ]
 docs = [
   "sphinx==5.3.0",
   "furo==2023.3.27",
```

### Comparing `timeseriesflattener-2.1.0/src/conftest.py` & `timeseriesflattener-2.1.1/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/test_benchmark.py` & `timeseriesflattener-2.1.1/src/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/_intermediary_frames.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 @dataclass
 class PredictorGroupSpec(V1PGSProtocol):
     lookbehind_days: Sequence[float | tuple[float, float]]
     named_dataframes: Sequence[NamedDataframe]
     aggregation_fns: Sequence[AggregationFunType]
     fallback: Sequence[int | float | str]
     prefix: str = "pred"
+    entity_id_col_name_out: str = "entity_id"
 
     def _infer_entity_id_col_name(self, df: pd.DataFrame) -> str:
         return next(c for c in df.columns if "entity" in c.lower() or "borger" in c.lower())
 
     def create_combinations(self) -> Sequence[v2_specs.PredictorSpec]:
         if isinstance(self.lookbehind_days[0], tuple):
             lookbehind_days = [
@@ -85,15 +86,17 @@
                 Iter(self.named_dataframes)
                 .map(
                     lambda ndf: v2_specs.PredictorSpec(
                         value_frame=ValueFrame(
                             init_df=ndf.df.rename(
                                 {
                                     "value": ndf.name,
-                                    self._infer_entity_id_col_name(ndf.df): "entity_id",
+                                    self._infer_entity_id_col_name(
+                                        ndf.df
+                                    ): self.entity_id_col_name_out,
                                 },
                                 axis=1,
                             )
                         ),
                         lookbehind_distances=lookbehind_days,
                         fallback=fallback,  # noqa: B023
                         aggregators=aggregators.to_list(),
```

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/meta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/static.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/process_spec.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/temporal.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,12 +170,12 @@
             )
         )
         .flatten()
     )
 
     return ProcessedFrame(
         df=horizontally_concatenate_dfs(
-            aggregated_value_frames.to_list(),
+            dfs=aggregated_value_frames.to_list(),
             pred_time_uuid_col_name=predictiontime_frame.pred_time_uuid_col_name,
         ),
         pred_time_uuid_col_name=predictiontime_frame.pred_time_uuid_col_name,
     )
```

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/test_flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.1.1/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.1.0
+Version: 2.1.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -46,28 +46,27 @@
 Requires-Dist: numpy>=1.23.3
 Requires-Dist: pyarrow>=8.0.0
 Requires-Dist: protobuf<=4.24.4
 Requires-Dist: frozendict>=2.3.4
 Requires-Dist: coloredlogs>14.0.0
 Requires-Dist: tqdm>4.1.0
 Requires-Dist: polars>0.19.0
-Requires-Dist: iterpy>=1.6.0
+Requires-Dist: iterpy==1.6.0
 Requires-Dist: rich>=13.0.0
 Provides-Extra: dev
 Requires-Dist: pyright==1.1.330.post0; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev"
 Requires-Dist: ruff==0.2.1; extra == "dev"
-Requires-Dist: pandas-stubs; extra == "dev"
+Requires-Dist: pandas-stubs==2.2.0.240218; extra == "dev"
 Requires-Dist: invoke==2.1.1; extra == "dev"
-Requires-Dist: lumberman; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest<7.3.0,>=7.1.3; extra == "test"
-Requires-Dist: pytest-cov<3.1.0,>=3.0.0; extra == "test"
-Requires-Dist: pytest-xdist<3.2.0,>=3.0.0; extra == "test"
-Requires-Dist: pytest-sugar<0.10.0,>=0.9.4; extra == "test"
+Requires-Dist: pytest==7.2.2; extra == "test"
+Requires-Dist: pytest-cov==3.0.0; extra == "test"
+Requires-Dist: pytest-xdist==3.1.0; extra == "test"
+Requires-Dist: pytest-sugar==0.9.7; extra == "test"
 Requires-Dist: pytest-testmon==2.1.0; extra == "test"
 Requires-Dist: pytest-benchmark==4.0.0; extra == "test"
 Requires-Dist: pytest-codspeed==2.2.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: furo==2023.3.27; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -28,23 +28,22 @@
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: <3.13.0,>=3.8.0 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: scipy>=1.8.0 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: pydantic>=2.0.0 Requires-Dist: pandas<=2.1.3,>=1.4.0 Requires-
 Dist: catalogue>=2.0.0 Requires-Dist: numpy>=1.23.3 Requires-Dist:
 pyarrow>=8.0.0 Requires-Dist: protobuf<=4.24.4 Requires-Dist: frozendict>=2.3.4
 Requires-Dist: coloredlogs>14.0.0 Requires-Dist: tqdm>4.1.0 Requires-Dist:
-polars>0.19.0 Requires-Dist: iterpy>=1.6.0 Requires-Dist: rich>=13.0.0
+polars>0.19.0 Requires-Dist: iterpy==1.6.0 Requires-Dist: rich>=13.0.0
 Provides-Extra: dev Requires-Dist: pyright==1.1.330.post0; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev" Requires-Dist: ruff==0.2.1;
-extra == "dev" Requires-Dist: pandas-stubs; extra == "dev" Requires-Dist:
-invoke==2.1.1; extra == "dev" Requires-Dist: lumberman; extra == "dev"
-Provides-Extra: test Requires-Dist: pytest<7.3.0,>=7.1.3; extra == "test"
-Requires-Dist: pytest-cov<3.1.0,>=3.0.0; extra == "test" Requires-Dist: pytest-
-xdist<3.2.0,>=3.0.0; extra == "test" Requires-Dist: pytest-
-sugar<0.10.0,>=0.9.4; extra == "test" Requires-Dist: pytest-testmon==2.1.0;
+extra == "dev" Requires-Dist: pandas-stubs==2.2.0.240218; extra == "dev"
+Requires-Dist: invoke==2.1.1; extra == "dev" Provides-Extra: test Requires-
+Dist: pytest==7.2.2; extra == "test" Requires-Dist: pytest-cov==3.0.0; extra ==
+"test" Requires-Dist: pytest-xdist==3.1.0; extra == "test" Requires-Dist:
+pytest-sugar==0.9.7; extra == "test" Requires-Dist: pytest-testmon==2.1.0;
 extra == "test" Requires-Dist: pytest-benchmark==4.0.0; extra == "test"
 Requires-Dist: pytest-codspeed==2.2.0; extra == "test" Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs" Requires-Dist: furo==2023.3.27;
 extra == "docs" Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "docs" Requires-Dist: myst-
 nb==0.17.2; extra == "docs" Requires-Dist: sphinx_design==0.3.0; extra ==
 "docs" Provides-Extra: tutorials Requires-Dist: jupyter<1.1.0,>=1.0.0; extra ==
```

### Comparing `timeseriesflattener-2.1.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.1.1/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.0/tasks.py` & `timeseriesflattener-2.1.1/tasks.py`

 * *Files identical despite different names*

