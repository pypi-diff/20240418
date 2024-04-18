# Comparing `tmp/generic_exporters-0.0.5.tar.gz` & `tmp/generic_exporters-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_exporters-0.0.5.tar", last modified: Fri Mar 29 07:20:53 2024, max compression
+gzip compressed data, was "generic_exporters-0.0.6.tar", last modified: Thu Apr 18 01:39:15 2024, max compression
```

## Comparing `generic_exporters-0.0.5.tar` & `generic_exporters-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.521983 generic_exporters-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.521983 generic_exporters-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.525983 generic_exporters-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.521983 generic_exporters-0.0.5/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.521983 generic_exporters-0.0.5/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.525983 generic_exporters-0.0.5/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.525983 generic_exporters-0.0.5/generic_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/_awaitable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.529983 generic_exporters-0.0.5/generic_exporters/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.529983 generic_exporters-0.0.5/generic_exporters/processors/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.529983 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.529983 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/exporters/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/framer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/processors/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/generic_exporters/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/generic_exporters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-29 07:20:53.000000 generic_exporters-0.0.5/generic_exporters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-29 07:20:53.000000 generic_exporters-0.0.5/generic_exporters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 07:20:53.000000 generic_exporters-0.0.5/generic_exporters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 07:20:53.000000 generic_exporters-0.0.5/generic_exporters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-29 07:20:53.000000 generic_exporters-0.0.5/generic_exporters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/tests/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/tests/processors/exporters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/tests/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/datastores/test_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:53.533983 generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/test_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/test_victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/exporters/test_exporter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/processors/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-29 07:20:43.000000 generic_exporters-0.0.5/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.coverage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.001582 generic_exporters-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.001582 generic_exporters-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.005582 generic_exporters-0.0.6/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.005582 generic_exporters-0.0.6/generic_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_awaitable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/framer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/generic_exporters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/exporters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/test_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/test_exporter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_timeseries.py
```

### Comparing `generic_exporters-0.0.5/.coverage` & `generic_exporters-0.0.6/.coverage`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/.github/workflows/deploy-docs.yaml` & `generic_exporters-0.0.6/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/.github/workflows/pages.yml` & `generic_exporters-0.0.6/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/.github/workflows/pytest.yaml` & `generic_exporters-0.0.6/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/.github/workflows/release.yaml` & `generic_exporters-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/Makefile` & `generic_exporters-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/alabaster.css` & `generic_exporters-0.0.6/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/basic.css` & `generic_exporters-0.0.6/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/doctools.js` & `generic_exporters-0.0.6/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/language_data.js` & `generic_exporters-0.0.6/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/pygments.css` & `generic_exporters-0.0.6/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/searchtools.js` & `generic_exporters-0.0.6/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/_build/html/_static/sphinx_highlight.js` & `generic_exporters-0.0.6/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/docs/conf.py` & `generic_exporters-0.0.6/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,20 +17,30 @@
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
+    'sphinx.ext.intersphinx',
+    'a_sync.sphinx.ext',
 ]
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
-
+intersphinx_mapping = {
+    'a_sync': ('https://bobthebuidler.github.io/ez-a-sync', None),
+    'aiohttp': ('https://docs.aiohttp.org/', None),
+    'bqplot': ('https://bqplot.github.io/bqplot/', None),
+    'msgspec': ('https://jcristharif.com/msgspec/', None),
+    'pandas': ('https://pandas.pydata.org/pandas-docs/', None),
+    'pony': ('https://docs.ponyorm.org/', None),
+    'python': ('https://docs.python.org/3', None),
+}
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'alabaster'
 html_static_path = ['_static']
```

### Comparing `generic_exporters-0.0.5/docs/make.bat` & `generic_exporters-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/_awaitable.py` & `generic_exporters-0.0.6/generic_exporters/_awaitable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/_constant.py` & `generic_exporters-0.0.6/generic_exporters/_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/_mathable.py` & `generic_exporters-0.0.6/generic_exporters/_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/_time.py` & `generic_exporters-0.0.6/generic_exporters/_time.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/dataset.py` & `generic_exporters-0.0.6/generic_exporters/dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/metric.py` & `generic_exporters-0.0.6/generic_exporters/metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/plan.py` & `generic_exporters-0.0.6/generic_exporters/plan.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/_base.py` & `generic_exporters-0.0.6/generic_exporters/processors/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from abc import abstractmethod
 from datetime import datetime
 from decimal import Decimal
-from typing import TYPE_CHECKING, Dict, TypeVar
+from typing import TYPE_CHECKING, Dict, Optional, TypeVar
 
 import a_sync
 
 from generic_exporters._awaitable import _AwaitableMixin
 from generic_exporters.plan import QueryPlan
 
 if TYPE_CHECKING:
@@ -28,19 +28,23 @@
 
 
 class _TimeSeriesProcessorBase(_ProcessorBase[_T]):
     def __init__(
         self, 
         query: QueryPlan, 
         *,
+        concurrency: Optional[int] = None,
         sync: bool = True,
     ) -> None:
         super().__init__(sync=sync)
         if not isinstance(query, QueryPlan):
             raise TypeError(f'`query` must be `QueryPlan`. You passed {query}')
         self.query = query
+        if concurrency is not None and not isinstance(concurrency, int):
+            raise TypeError(f'`concurrency` must be int. You passed {concurrency}')
+        self.concurrency = concurrency
 
 
 class _GatheringTimeSeriesProcessorBase(_TimeSeriesProcessorBase[_T]):
     """Inherit from this class when you need to collect all the data before processing"""
     async def _gather(self) -> Dict[datetime, Dict["Metric", Decimal]]:
         return await a_sync.gather({ts: self.query[ts] async for ts in self.query._aiter_timestamps()})
```

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/_base.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 class _TimeSeriesExporterBase(_TimeSeriesProcessorBase, _ExporterBase):
     """I dont remember why I made this base class. Maybe I will"""
     def __init__(
         self, 
         query_plan: "QueryPlan", 
         datastore: Optional[TimeSeriesDataStoreBase], 
         *, 
+        concurrency: Optional[int] = None,
         sync: bool = True,
     ) -> None:
-        super().__init__(query_plan, sync=sync)
+        super().__init__(query_plan, concurrency=concurrency, sync=sync)
         if isinstance(datastore, TimeSeriesDataStoreBase):
             self.datastore = datastore
         elif datastore is None:
             self.datastore = SQLTimeSeriesKeyValueStore()
         else:
             raise TypeError(datastore)
         self.datastore = datastore
```

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/default.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/default.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/multi.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/sql.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/sql.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/datastores/timeseries/victoria.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/exporters/exporter.py` & `generic_exporters-0.0.6/generic_exporters/processors/exporters/exporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
-import asyncio
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from typing import Literal, NoReturn, Optional, Union, overload
 
 import a_sync
-from a_sync.utils.iterators import exhaust_iterator
 from generic_exporters.plan import QueryPlan
 from generic_exporters.processors.exporters._base import _TimeSeriesExporterBase
 from generic_exporters.processors.exporters.datastores.timeseries._base import TimeSeriesDataStoreBase
 
 
 class TimeSeriesExporter(_TimeSeriesExporterBase):
     """
@@ -22,28 +20,34 @@
         query: QueryPlan, 
         datastore: TimeSeriesDataStoreBase, 
         *, 
         buffer: timedelta = timedelta(minutes=5), 
         concurrency: Optional[int] = None, 
         sync: bool = True,
     ) -> None:
-        super().__init__(query, datastore, sync=sync)
+        super().__init__(query, datastore, concurrency=concurrency, sync=sync)
         self.buffer = buffer
-        self.concurrency = concurrency
-    
-    @abstractmethod
-    async def data_exists(self, timestamp: datetime) -> bool:
-        """Returns True if data exists at `timestamp`, False if it does not and must be exported."""
+        self.ensure_data = a_sync.ProcessingQueue(self._ensure_data, concurrency, return_data=False)
+        self._push = a_sync.ProcessingQueue(self.datastore.push, concurrency*10, return_data=False)
 
     @overload
     async def run(self, run_forever: Literal[True]) -> NoReturn:...
     @overload
     async def run(self, run_forever: Literal[False]) -> None:...
     async def run(self, run_forever: bool = False) -> Union[None, NoReturn]:
         """Exports the full history for this exporter's `Metric` to the datastore"""
-        export_fn = lambda ts: self.ensure_data(ts, sync=False)
-        await exhaust_iterator(a_sync.TaskMapping(export_fn, concurrency=self.concurrency).map(self.query._aiter_timestamps(run_forever)))
+        async for ts in self.query._aiter_timestamps(run_forever):
+            self.ensure_data(ts)
+        # wait for all rpc activity to complete
+        await self.ensure_data.join()
+        # wait for all data to be pushed to datastore
+        await self._push.join()
+    
+    @abstractmethod
+    async def data_exists(self, timestamp: datetime) -> bool:
+        """Returns True if data exists at `timestamp`, False if it does not and must be exported."""
 
-    async def ensure_data(self, ts: datetime) -> None:
+    async def _ensure_data(self, ts: datetime) -> None:
         if not await self.data_exists(ts, sync=False):
             data = await self.query[ts]
-            await asyncio.gather(*[self.datastore.push(key, ts, value) for key, value in data.items()])
+            for key, value in data.items():
+                self._push(key, ts, value)
```

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/framer.py` & `generic_exporters-0.0.6/generic_exporters/processors/framer.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/processors/plotter.py` & `generic_exporters-0.0.6/generic_exporters/processors/plotter.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters/timeseries.py` & `generic_exporters-0.0.6/generic_exporters/timeseries.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/generic_exporters.egg-info/SOURCES.txt` & `generic_exporters-0.0.6/generic_exporters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/setup.py` & `generic_exporters-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/fixtures.py` & `generic_exporters-0.0.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/processors/exporters/datastores/test_multi.py` & `generic_exporters-0.0.6/tests/processors/exporters/datastores/test_multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/test_sql.py` & `generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_sql.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/processors/exporters/datastores/timeseries/test_victoria.py` & `generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/processors/test_base.py` & `generic_exporters-0.0.6/tests/processors/test_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_constant.py` & `generic_exporters-0.0.6/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_dataset.py` & `generic_exporters-0.0.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_mathable.py` & `generic_exporters-0.0.6/tests/test_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_metric.py` & `generic_exporters-0.0.6/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_plan.py` & `generic_exporters-0.0.6/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.5/tests/test_timeseries.py` & `generic_exporters-0.0.6/tests/test_timeseries.py`

 * *Files identical despite different names*

