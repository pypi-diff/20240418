# Comparing `tmp/gwsumm-2.2.4.tar.gz` & `tmp/gwsumm-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsumm-2.2.4.tar", last modified: Fri Apr  5 20:17:34 2024, max compression
+gzip compressed data, was "gwsumm-2.2.5.tar", last modified: Thu Apr 18 16:16:55 2024, max compression
```

## Comparing `gwsumm-2.2.4.tar` & `gwsumm-2.2.5.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.258291 gwsumm-2.2.4/
--rw-r--r--   0 egoetz     (501) staff       (20)      319 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.codeclimate.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2020-04-07 19:56:04.000000 gwsumm-2.2.4/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      126 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       32 2020-04-07 19:56:04.000000 gwsumm-2.2.4/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.137534 gwsumm-2.2.4/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.151520 gwsumm-2.2.4/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     3579 2024-03-26 21:53:27.000000 gwsumm-2.2.4/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      765 2024-03-26 21:53:27.000000 gwsumm-2.2.4/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      259 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      645 2024-03-25 16:15:43.000000 gwsumm-2.2.4/.readthedocs.yaml
--rw-r--r--   0 egoetz     (501) staff       (20)     2667 2021-03-09 19:10:52.000000 gwsumm-2.2.4/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.2.4/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       94 2023-11-01 22:18:02.000000 gwsumm-2.2.4/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-05 20:17:34.257513 gwsumm-2.2.4/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.2.4/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.161056 gwsumm-2.2.4/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6810 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.137925 gwsumm-2.2.4/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.161552 gwsumm-2.2.4/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.162195 gwsumm-2.2.4/docs/_templates/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.162833 gwsumm-2.2.4/docs/_templates/autoclass/
--rw-r--r--   0 egoetz     (501) staff       (20)      928 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.164817 gwsumm-2.2.4/docs/_templates/autosummary/
--rw-r--r--   0 egoetz     (501) staff       (20)      170 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1167 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      703 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/module.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      303 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/layout.html
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.165422 gwsumm-2.2.4/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       64 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      537 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/automation.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1427 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/cli.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10467 2023-11-01 22:18:02.000000 gwsumm-2.2.4/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.168513 gwsumm-2.2.4/docs/configuration/
--rw-r--r--   0 egoetz     (501) staff       (20)    12488 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/data.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1887 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/format.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      908 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     3433 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/tabs.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      555 2024-03-25 16:02:23.000000 gwsumm-2.2.4/docs/environment.yml
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.170520 gwsumm-2.2.4/docs/examples/
--rw-r--r--   0 egoetz     (501) staff       (20)    22257 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/examples/first.png
--rw-r--r--   0 egoetz     (501) staff       (20)    95352 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/examples/imc.png
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.172240 gwsumm-2.2.4/docs/images/
--rw-r--r--   0 egoetz     (501) staff       (20)   710629 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/images/screenshot.png
--rw-r--r--   0 egoetz     (501) staff       (20)     2948 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     6701 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/make.bat
--rw-r--r--   0 egoetz     (501) staff       (20)       28 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/modes.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2864 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/overview.rst
--rw-r--r--   0 egoetz     (501) staff       (20)       79 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/plots.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      100 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/states.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.179014 gwsumm-2.2.4/docs/tabs/
--rw-r--r--   0 egoetz     (501) staff       (20)       53 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/tabs/api.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1458 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2368 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/modes.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2202 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/websites.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.190977 gwsumm-2.2.4/gwsumm/
--rw-r--r--   0 egoetz     (501) staff       (20)     1326 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    28701 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-05 20:17:33.000000 gwsumm-2.2.4/gwsumm/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14914 2024-04-04 19:05:23.000000 gwsumm-2.2.4/gwsumm/archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10806 2024-04-05 20:16:21.000000 gwsumm-2.2.4/gwsumm/channels.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.196508 gwsumm-2.2.4/gwsumm/config/
--rw-r--r--   0 egoetz     (501) staff       (20)    14290 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/defaults.ini
--rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/matplotlib.ini
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.202891 gwsumm-2.2.4/gwsumm/data/
--rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    18673 2022-09-15 15:47:20.000000 gwsumm-2.2.4/gwsumm/data/coherence.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/mathutils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7193 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/data/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16530 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/data/spectral.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32307 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/data/timeseries.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/globalv.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.206335 gwsumm-2.2.4/gwsumm/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/html/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6404 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/html/html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2591 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/static.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.209925 gwsumm-2.2.4/gwsumm/html/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/html/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4297 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/tests/test_bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/html/tests/test_html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1940 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/html/tests/test_static.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/io.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/mode.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.219878 gwsumm-2.2.4/gwsumm/plot/
--rw-r--r--   0 egoetz     (501) staff       (20)     2834 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    37328 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/plot/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    27119 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.222062 gwsumm-2.2.4/gwsumm/plot/guardian/
--rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.223306 gwsumm-2.2.4/gwsumm/plot/guardian/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/plot/mixins.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8000 2023-11-02 17:15:14.000000 gwsumm-2.2.4/gwsumm/plot/noisebudget.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14079 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/plot/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    58958 2024-03-19 23:14:10.000000 gwsumm-2.2.4/gwsumm/plot/segments.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/plot/sei.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.226093 gwsumm-2.2.4/gwsumm/plot/triggers/
--rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.2.4/gwsumm/plot/triggers/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    21921 2023-11-02 17:15:14.000000 gwsumm-2.2.4/gwsumm/plot/triggers/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.227912 gwsumm-2.2.4/gwsumm/plot/triggers/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4987 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/plot/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12722 2024-01-25 21:39:34.000000 gwsumm-2.2.4/gwsumm/segments.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.231658 gwsumm-2.2.4/gwsumm/state/
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.2.4/gwsumm/state/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/state/all.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/state/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/state/registry.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.244791 gwsumm-2.2.4/gwsumm/tabs/
--rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    36826 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/tabs/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    39853 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/tabs/data.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15759 2024-01-31 17:20:38.000000 gwsumm-2.2.4/gwsumm/tabs/etg.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.2.4/gwsumm/tabs/fscan.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tabs/gracedb.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14124 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/tabs/guardian.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/management.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tabs/misc.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/sei.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.2.4/gwsumm/tabs/stamp.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.253845 gwsumm-2.2.4/gwsumm/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/common.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_channels.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_data.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_mode.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10913 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_tabs.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16412 2024-03-19 23:14:10.000000 gwsumm-2.2.4/gwsumm/triggers.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/units.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.254606 gwsumm-2.2.4/gwsumm.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2986 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      204 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      410 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        7 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     2891 2024-04-04 18:06:28.000000 gwsumm-2.2.4/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-05 20:17:34.258451 gwsumm-2.2.4/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.799503 gwsumm-2.2.5/
+-rw-r--r--   0 egoetz     (501) staff       (20)      319 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.codeclimate.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2020-04-07 19:56:04.000000 gwsumm-2.2.5/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      126 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       32 2020-04-07 19:56:04.000000 gwsumm-2.2.5/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.699010 gwsumm-2.2.5/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.711514 gwsumm-2.2.5/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3579 2024-03-26 21:53:27.000000 gwsumm-2.2.5/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      765 2024-03-26 21:53:27.000000 gwsumm-2.2.5/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      259 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      645 2024-03-25 16:15:43.000000 gwsumm-2.2.5/.readthedocs.yaml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2667 2021-03-09 19:10:52.000000 gwsumm-2.2.5/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.2.5/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       94 2023-11-01 22:18:02.000000 gwsumm-2.2.5/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-18 16:16:55.798589 gwsumm-2.2.5/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.2.5/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.720148 gwsumm-2.2.5/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6810 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.699534 gwsumm-2.2.5/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.720975 gwsumm-2.2.5/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.721783 gwsumm-2.2.5/docs/_templates/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.722880 gwsumm-2.2.5/docs/_templates/autoclass/
+-rw-r--r--   0 egoetz     (501) staff       (20)      928 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.725624 gwsumm-2.2.5/docs/_templates/autosummary/
+-rw-r--r--   0 egoetz     (501) staff       (20)      170 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1167 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      703 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      303 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/layout.html
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.726865 gwsumm-2.2.5/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       64 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      537 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/automation.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1427 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/cli.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10467 2023-11-01 22:18:02.000000 gwsumm-2.2.5/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.729685 gwsumm-2.2.5/docs/configuration/
+-rw-r--r--   0 egoetz     (501) staff       (20)    12488 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/data.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1887 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/format.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      908 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     3433 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/tabs.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      555 2024-03-25 16:02:23.000000 gwsumm-2.2.5/docs/environment.yml
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.731211 gwsumm-2.2.5/docs/examples/
+-rw-r--r--   0 egoetz     (501) staff       (20)    22257 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/examples/first.png
+-rw-r--r--   0 egoetz     (501) staff       (20)    95352 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/examples/imc.png
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.732590 gwsumm-2.2.5/docs/images/
+-rw-r--r--   0 egoetz     (501) staff       (20)   710629 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/images/screenshot.png
+-rw-r--r--   0 egoetz     (501) staff       (20)     2948 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     6701 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/make.bat
+-rw-r--r--   0 egoetz     (501) staff       (20)       28 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2864 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/overview.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)       79 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/plots.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      100 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/states.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.738832 gwsumm-2.2.5/docs/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)       53 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/tabs/api.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1458 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2368 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2202 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/websites.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.747158 gwsumm-2.2.5/gwsumm/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1326 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    28701 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16826 2024-04-17 23:14:02.000000 gwsumm-2.2.5/gwsumm/archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12777 2024-04-17 23:14:02.000000 gwsumm-2.2.5/gwsumm/channels.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.750606 gwsumm-2.2.5/gwsumm/config/
+-rw-r--r--   0 egoetz     (501) staff       (20)    14290 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/defaults.ini
+-rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/matplotlib.ini
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.756105 gwsumm-2.2.5/gwsumm/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20054 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/data/coherence.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/mathutils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7322 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/data/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16530 2024-04-05 20:16:32.000000 gwsumm-2.2.5/gwsumm/data/spectral.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32307 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/data/timeseries.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/globalv.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.758475 gwsumm-2.2.5/gwsumm/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/html/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6402 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/html/bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/html/html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2591 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/html/static.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.760724 gwsumm-2.2.5/gwsumm/html/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/html/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4297 2024-04-04 18:06:28.000000 gwsumm-2.2.5/gwsumm/html/tests/test_bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/html/tests/test_html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1940 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/html/tests/test_static.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/io.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/mode.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.768868 gwsumm-2.2.5/gwsumm/plot/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2834 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    37328 2024-04-05 20:16:32.000000 gwsumm-2.2.5/gwsumm/plot/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    27119 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.770800 gwsumm-2.2.5/gwsumm/plot/guardian/
+-rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.772053 gwsumm-2.2.5/gwsumm/plot/guardian/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/plot/mixins.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8000 2023-11-02 17:15:14.000000 gwsumm-2.2.5/gwsumm/plot/noisebudget.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14079 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/plot/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    58958 2024-03-19 23:14:10.000000 gwsumm-2.2.5/gwsumm/plot/segments.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/plot/sei.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.774206 gwsumm-2.2.5/gwsumm/plot/triggers/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.2.5/gwsumm/plot/triggers/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    21921 2023-11-02 17:15:14.000000 gwsumm-2.2.5/gwsumm/plot/triggers/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.775874 gwsumm-2.2.5/gwsumm/plot/triggers/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4987 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/plot/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12722 2024-01-25 21:39:34.000000 gwsumm-2.2.5/gwsumm/segments.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.778413 gwsumm-2.2.5/gwsumm/state/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.2.5/gwsumm/state/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/state/all.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/state/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/state/registry.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.788515 gwsumm-2.2.5/gwsumm/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    36826 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/tabs/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    39853 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/tabs/data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15759 2024-01-31 17:20:38.000000 gwsumm-2.2.5/gwsumm/tabs/etg.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.2.5/gwsumm/tabs/fscan.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tabs/gracedb.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14124 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/tabs/guardian.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/management.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tabs/misc.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/sei.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.2.5/gwsumm/tabs/stamp.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.795407 gwsumm-2.2.5/gwsumm/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/common.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_channels.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_mode.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10913 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_tabs.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16412 2024-03-19 23:14:10.000000 gwsumm-2.2.5/gwsumm/triggers.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/units.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.796074 gwsumm-2.2.5/gwsumm.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2986 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      204 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      410 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        7 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     2891 2024-04-18 16:13:50.000000 gwsumm-2.2.5/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-18 16:16:55.799671 gwsumm-2.2.5/setup.cfg
```

### Comparing `gwsumm-2.2.4/.github/workflows/build.yml` & `gwsumm-2.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/.github/workflows/lint.yml` & `gwsumm-2.2.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/.readthedocs.yaml` & `gwsumm-2.2.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/CONTRIBUTING.md` & `gwsumm-2.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/LICENSE` & `gwsumm-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/PKG-INFO` & `gwsumm-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.2.4
+Requires-Dist: gwdetchar>=2.2.5
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.4/README.rst` & `gwsumm-2.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/Makefile` & `gwsumm-2.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/_static/css/custom.css` & `gwsumm-2.2.5/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/_templates/autoclass/class.rst` & `gwsumm-2.2.5/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/_templates/autosummary/class.rst` & `gwsumm-2.2.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/_templates/autosummary/module.rst` & `gwsumm-2.2.5/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/automation.rst` & `gwsumm-2.2.5/docs/automation.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/cli.rst` & `gwsumm-2.2.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/conf.py` & `gwsumm-2.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/configuration/data.rst` & `gwsumm-2.2.5/docs/configuration/data.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/configuration/format.rst` & `gwsumm-2.2.5/docs/configuration/format.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/configuration/index.rst` & `gwsumm-2.2.5/docs/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/configuration/tabs.rst` & `gwsumm-2.2.5/docs/configuration/tabs.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/environment.yml` & `gwsumm-2.2.5/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/examples/first.png` & `gwsumm-2.2.5/docs/examples/first.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/examples/imc.png` & `gwsumm-2.2.5/docs/examples/imc.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/images/screenshot.png` & `gwsumm-2.2.5/docs/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/index.rst` & `gwsumm-2.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/make.bat` & `gwsumm-2.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/overview.rst` & `gwsumm-2.2.5/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/tabs/index.rst` & `gwsumm-2.2.5/docs/tabs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/tabs/modes.rst` & `gwsumm-2.2.5/docs/tabs/modes.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/docs/tabs/websites.rst` & `gwsumm-2.2.5/docs/tabs/websites.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/__init__.py` & `gwsumm-2.2.5/gwsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/__main__.py` & `gwsumm-2.2.5/gwsumm/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/archive.py` & `gwsumm-2.2.5/gwsumm/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -298,58 +298,129 @@
 
         for dataset in h5file.get('triggers', {}).values():
             load_table(dataset)
 
 
 def find_daily_archives(start, end, ifo, tag, basedir=os.curdir):
     """Find the daily archives spanning the given GPS [start, end) interval
+
+    Parameters
+    ----------
+    start : `float`, `~datetime.datetime`, `~astropy.time.Time`, `str`
+        start time of the archive file to find, any object that can be
+        converted into a `LIGOTimeGPS`, `~astropy.time.Time`, or
+        `~datetime.datetime` is acceptable
+    end : `float`, `~datetime.datetime`, `~astropy.time.Time`, `str`
+        end time of the archive file to find, any object that can be
+        converted into a `LIGOTimeGPS`, `~astropy.time.Time`, or
+        `~datetime.datetime` is acceptable
+    ifo : `str`
+        interferometer string, ex. 'H1'
+    tag : `str`
+        tag string for the archive file
+    basedir : `path-like`, optional
+        base path to archive files, default: '.'
+
+    Returns
+    -------
+    archives : `list`
+        list of matching archive files
+
+    Notes
+    -----
+    This will only search the day directories with the format `YYYYMMDD`
     """
     archives = []
+
+    # Convert start and end to properly formatted datetime objects
     s = from_gps(to_gps(start))
     e = from_gps(to_gps(end))
+
+    # append to the archives list as long as the iterating start time is
+    # earlier than the end time
     while s < e:
         daybase = mode.get_base(s, mode=mode.Mode.day)
         ds = to_gps(s)
         s += datetime.timedelta(days=1)
         de = to_gps(s)
         archivedir = os.path.join(basedir, daybase, 'archive')
-        arch = os.path.join(archivedir, '%s-%s-%d-%d.h5'
-                            % (ifo, tag, ds, de-ds))
+        arch = os.path.join(archivedir, f'{ifo}-{tag}-{ds}-{de-ds}.h5')
         if os.path.isfile(arch):
             archives.append(arch)
     return archives
 
 
 # -- utility methods --------------------------------------------------------
 
 def _write_object(data, *args, **kwargs):
     """Internal method to write something to HDF5 with error handling
+
+    Parameters
+    ----------
+    data : gwpy object
+        TimeSeries or FrequencySeries
+    args :
+        passed to underlying write method
+    kwargs :
+        passed to underlying write method
+
+    Warns
+    -----
+    TypeError
+    ValueError
+    RuntimeError
+        If the name already exists in the HDF5 file
+
+    Raises
+    ------
+    RuntimeError
+        Any error other than the object name already exists in the HDF5 file
     """
     try:
         return data.write(*args, **kwargs)
     except (TypeError, ValueError) as e:
         warnings.warn(str(e))
     except RuntimeError as e:
         if 'name already exists' in str(e).lower():
             warnings.warn(str(e))
         else:
             raise
 
 
 def segments_to_array(segmentlist):
     """Convert a `SegmentList` to a 2-dimensional `numpy.ndarray`
+
+    Parameters
+    ----------
+    segmentlist : `~gwpy.segments.SegmentList`
+        input segment list to convert
+
+    Returns
+    -------
+    out : `float` `numpy.ndarray`
+        output segment list as a numpy array
     """
     out = ndarray((len(segmentlist), 2), dtype=float)
     for i, seg in enumerate(segmentlist):
         out[i] = seg
     return out
 
 
 def segments_from_array(array):
     """Convert a 2-dimensional `numpy.ndarray` to a `SegmentList`
+
+    Parameters
+    ----------
+    array : `float` `numpy.ndarray`
+        input numpy array to convert into a segment list
+
+    Returns
+    -------
+    out : `~gwpy.segments.SegmentList`
+        output segment list
     """
     out = SegmentList()
     for row in array:
         out.append(Segment(*row))
     return out
```

### Comparing `gwsumm-2.2.4/gwsumm/batch.py` & `gwsumm-2.2.5/gwsumm/batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/channels.py` & `gwsumm-2.2.5/gwsumm/channels.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,26 @@
                         r'(?:\.[a-z]+)?'  # trend type
                         r'(?:,[a-z-]+)?')  # NDS channel type
 
 
 # -- channel creation ---------------------------------------------------------
 
 def _match(channel):
+    """Find a matching channel in global memory variable
+
+    Parameters
+    ----------
+    channel : `str`, `~gwpy.detector.Channel`
+        name of a channel
+
+    Returns
+    -------
+    found : `Channel`
+        matching channel from global memory or an empty list
+    """
     channel = Channel(channel)
     name = str(channel)
     type_ = channel.type
     found = globalv.CHANNELS.sieve(
         name=name, type=type_, exact_match=True)
 
     # if match, return now
@@ -65,30 +77,53 @@
 
 def _find_parent(channel):
     """Find the parent for a given channel
 
     This is either the raw channel from which a trend was generated, or the
     real channel for a mathematically-manipulated channel.
 
+    Parameters
+    ----------
+    channel : `~gwpy.detector.Channel`
+        trend channel or mathematically-manipulated channel
+
+    Returns
+    -------
+    parent_channel : `~gwpy.detector.Channel`
+        the raw channel from the trend or real channel from manipulated channel
+
     Raises
     ------
     ValueError
         if the parent cannot be parsed
     """
+    # If the channel is a trend, then get the part of the name before the dot
     if channel.trend:
         parent = str(channel).rsplit('.')[0]
     else:
         parent, = re_channel.findall(str(channel))
+    # If the parent and input channel are the same, then no parent is found
     if parent == str(channel):
-        raise ValueError("Cannot find parent for '{0!s}'".format(channel))
-    return get_channel(parent)
+        raise ValueError(f"Cannot find parent for '{str(channel)}'")
+    parent_channel = get_channel(parent)
+    return parent_channel
 
 
 def _update_dependent(channel):
     """Update a trend channel from its parent
+
+    TODO: what does this mean?
+
+    Parameters
+    ----------
+    channel : `~gwpy.detector.Channel`
+
+    Returns
+    -------
+    channel : `~gwpy.detector.Channel`
     """
     try:
         source = _find_parent(channel)
     except (ValueError, IndexError):
         return channel
     if source is channel:
         return channel
@@ -122,14 +157,30 @@
             out = _update_dependent(out)
         return out
     return wrapped_func
 
 
 def _new(channel, find_parent=True):
     """Create a new `~gwpy.detector.Channel` in the globalv cache.
+
+    Parameters
+    ----------
+    channel : `str`, `~gwpy.detector.Channel`
+        channel string or object to create in the global memory
+    find_parent : `bool`, optional, default: `True`
+        query for raw version of trend channel (trends not in CIS)
+
+    Returns
+    -------
+    Channel : `~gwpy.detector.Channel`
+        newly created channel
+
+    Raises
+    ------
+    RuntimeError
     """
     # convert to Channel
     if isinstance(channel, Channel):
         new = channel
     else:
         new = Channel(channel)
     name = str(channel)
@@ -225,15 +276,27 @@
                          % (str(channel), '\n    '.join(cstrings)))
 
     # otherwise there were no matches, so we create a new channel
     return _new(channel, find_parent=find_parent)
 
 
 def get_channels(channels, **kwargs):
-    """Find (or create) multiple channels.
+    """Find (or create) multiple channels calling get_channel()
+
+    Parameters
+    ----------
+    channels : `list`
+        list of channels as `str` or `~gwpy.detector.Channel` objects
+    **kwargs
+        keyword arguments applied to each channel in the list
+
+    Returns
+    -------
+    ChannelList : `~gwpy.detector.ChannelList`
+        a list of channels
 
     See Also
     --------
     get_channel
     """
     return ChannelList(get_channel(c, **kwargs) for c in channels)
 
@@ -248,14 +311,19 @@
 
     Parameters
     ----------
     channel : `~gwpy.detector.Channel`
         channel to update
     **kwargs
         `(key, value)` pairs to set
+
+    Returns
+    -------
+    target : `~gwpy.detector.Channel`
+        the channel after updating parameters
     """
     target = get_channel(str(channel))
     if isinstance(channel, Channel):
         for param in ['unit', 'sample_rate', 'frametype']:
             if getattr(target, param) is None or (
                     param == 'unit' and
                     getattr(target, param) is Unit('undef')):
@@ -288,14 +356,24 @@
 
 
 # -- string parsing -----------------------------------------------------------
 
 def split(channelstring):
     """Split a comma-separated list of channels that may, or may not
     contain NDS2 channel types as well
+
+    Parameters
+    ----------
+    channelstring : `str`
+        comma-separated string of channels
+
+    Returns
+    -------
+    out : `list`
+        list of strings for each channel
     """
     out = []
     channelstring = re_quote.sub('', channelstring)
     while True:
         channelstring = channelstring.strip('\' \n')
         if ',' not in channelstring:
             break
@@ -327,13 +405,17 @@
         out.append(channelstring)
     return out
 
 
 def split_combination(channelstring):
     """Split a math-combination of channels
 
+    Parameters
+    ----------
+    channelstring : `str`
+
     Returns
     -------
-    channels : `~gwpy.detector.ChannelList`
+    ChannelList : `~gwpy.detector.ChannelList`
     """
     return get_channels(re_channel.findall(str(channelstring)),
                         find_parent=False)
```

### Comparing `gwsumm-2.2.4/gwsumm/config/__init__.py` & `gwsumm-2.2.5/gwsumm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/config/defaults.ini` & `gwsumm-2.2.5/gwsumm/config/defaults.ini`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/data/__init__.py` & `gwsumm-2.2.5/gwsumm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/data/coherence.py` & `gwsumm-2.2.5/gwsumm/data/coherence.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 from itertools import zip_longest
 from collections import OrderedDict
 
 import numpy
 
 from astropy import units
 
-from gwpy.segments import (DataQualityFlag, SegmentList, Segment)
+from gwpy.segments import (DataQualityFlag, SegmentList,
+                           Segment, SegmentListDict)
 from gwpy.frequencyseries import FrequencySeries
 from gwpy.spectrogram import SpectrogramList
 
 from .. import globalv
 from ..utils import (vprint, safe_eval)
 from ..channels import get_channel
 from .utils import (use_segmentlist, get_fftparams, make_globalv_key)
@@ -127,16 +128,49 @@
                            dts2[0].sample_rate.value)
         except IndexError:
             sampling = None
     else:
         sampling = None
 
     # initialize component lists if they don't exist yet
+    # store compnents in a backup variable
+    coherence_bkp = {}
     for ck in ckeys:
         globalv.COHERENCE_COMPONENTS.setdefault(ck, SpectrogramList())
+        coherence_bkp[ck] = globalv.COHERENCE_COMPONENTS.get(
+            ck, SpectrogramList())
+
+    # When coherence components contain different segments,
+    # computing coherence for new segments can result in a
+    # ValueError traceback due to incompatible shapes.
+    # To prevent this issue, we collect segments from all components,
+    # clear them from the global variable, and then restore from the
+    # coherence_bkp only the data that the segments available in
+    # coherence all components.
+
+    # get the segment spans from all components
+    spans = SegmentListDict()
+    for ck in ckeys:
+        spans[ck] = SegmentList(
+            [spec.span for spec in globalv.COHERENCE_COMPONENTS[ck]])
+    # keep only the intersection of the segments
+    spans = spans.intersection(list(ckeys))
+
+    # clean the components in the global variable
+    globalv.COHERENCE_COMPONENTS.update(
+        {ck: SpectrogramList() for ck in ckeys})
+
+    # restore the data for segments available in all components
+    for seg in spans:
+        for ck in ckeys:
+            spec = _get_from_list(coherence_bkp[ck], seg)
+            add_coherence_component_spectrogram(spec, key=ck)
+
+    # explicitly delete the backup variable to decrease RAM consuption
+    del coherence_bkp
 
     # get data if query=True or if there are new segments
     query &= abs(new) != 0
 
     if query:
 
         # the intersecting segments will be calculated when needed
```

### Comparing `gwsumm-2.2.4/gwsumm/data/mathutils.py` & `gwsumm-2.2.5/gwsumm/data/mathutils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/data/range.py` & `gwsumm-2.2.5/gwsumm/data/range.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,24 +118,28 @@
                             outspec**(1/2.), key=key)
 
     if not return_:
         return
 
     # return correct data, according to state segment
     out = SpectrogramList()
-    for specgram in globalv.SPECTROGRAMS[key]:
-        for seg in segments:
-            if abs(seg) < specgram.dt.value:
-                continue
-            if specgram.span.intersects(seg):
-                common = specgram.span & type(seg)(seg[0],
-                                                   seg[1] + specgram.dt.value)
-                s = specgram.crop(*common)
-                if s.shape[0]:
-                    out.append(s)
+    try:
+        for specgram in globalv.SPECTROGRAMS[key]:
+            for seg in segments:
+                if abs(seg) < specgram.dt.value:
+                    continue
+                if specgram.span.intersects(seg):
+                    common = specgram.span & type(seg)(
+                        seg[0], seg[1] + specgram.dt.value)
+                    s = specgram.crop(*common)
+                    if s.shape[0]:
+                        out.append(s)
+    except KeyError:
+        # in case the key does not exist return empty SpectrogramList
+        return out
     return out.coalesce()
 
 
 @use_segmentlist
 def get_range_spectrum(channel, segments, config=None, cache=None, query=True,
                        nds=None, return_=True, nproc=1, datafind_error='raise',
                        frametype=None, stride=60, fftlength=None, overlap=None,
```

### Comparing `gwsumm-2.2.4/gwsumm/data/spectral.py` & `gwsumm-2.2.5/gwsumm/data/spectral.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/data/timeseries.py` & `gwsumm-2.2.5/gwsumm/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/data/utils.py` & `gwsumm-2.2.5/gwsumm/data/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/globalv.py` & `gwsumm-2.2.5/gwsumm/globalv.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/__init__.py` & `gwsumm-2.2.5/gwsumm/html/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/bootstrap.py` & `gwsumm-2.2.5/gwsumm/html/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     page.h6('Select below to view this page in another state (different '
             'time segments).', class_='dropdown-header')
     page.div('', class_='dropdown-divider')
     for i, (state, href) in enumerate(states):
         page.a(str(state), class_='dropdown-item state', title=str(state),
                id_='state_%s' % re_cchar.sub('_', str(state)).lower(),
                onclick='jQuery(this).load_state(\'%s\');' % href)
-    page.div.close()  # dropdown-menu dropdown-menu-right
+    page.div.close()  # dropdown-menu dropdown-menu-end
     page.li.close()  # nav-item dropdown state-switch
     page.ul.close()  # nav navbar-nav
     return page
 
 
 def base_map_dropdown(this, id_=None, bases=dict()):
     """Construct a dropdown menu that links to a version of the current
```

### Comparing `gwsumm-2.2.4/gwsumm/html/html5.py` & `gwsumm-2.2.5/gwsumm/html/html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/static.py` & `gwsumm-2.2.5/gwsumm/html/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 # build collection of CSS resources
 CSS = OrderedDict((
     ('font-awesome', 'https://cdnjs.cloudflare.com/ajax/libs/'
                      'font-awesome/6.5.1/css/fontawesome.min.css'),
     ('font-awesome-solid', 'https://cdnjs.cloudflare.com/ajax/libs/'
                            'font-awesome/6.5.1/css/solid.min.css'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.4/'
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
                     'lib/gwbootstrap.min.css'),
 ))
 
 # build collection of javascript resources
 JS = OrderedDict((
     ('jquery', 'https://code.jquery.com/jquery-3.7.1.min.js'),
     ('jquery-ui', 'https://code.jquery.com/ui/1.13.2/jquery-ui.min.js'),
@@ -47,15 +47,15 @@
     ('bootstrap', 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/'
                   'dist/js/bootstrap.bundle.min.js'),
     ('fancybox', 'https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/'
                  'dist/fancybox/fancybox.umd.js'),
     ('datepicker', 'https://cdnjs.cloudflare.com/ajax/libs/'
                    'bootstrap-datepicker/1.9.0/js/'
                    'bootstrap-datepicker.min.js'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.4/'
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
                     'lib/gwbootstrap-extra.min.js'),
 ))
 
 
 # -- utilities ----------------------------------------------------------------
 
 def get_css():
```

### Comparing `gwsumm-2.2.4/gwsumm/html/tests/__init__.py` & `gwsumm-2.2.5/gwsumm/html/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/tests/test_bootstrap.py` & `gwsumm-2.2.5/gwsumm/html/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/tests/test_html5.py` & `gwsumm-2.2.5/gwsumm/html/tests/test_html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/html/tests/test_static.py` & `gwsumm-2.2.5/gwsumm/html/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/io.py` & `gwsumm-2.2.5/gwsumm/io.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/mode.py` & `gwsumm-2.2.5/gwsumm/mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/__init__.py` & `gwsumm-2.2.5/gwsumm/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/builtin.py` & `gwsumm-2.2.5/gwsumm/plot/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/core.py` & `gwsumm-2.2.5/gwsumm/plot/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/guardian/__init__.py` & `gwsumm-2.2.5/gwsumm/plot/guardian/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/guardian/__main__.py` & `gwsumm-2.2.5/gwsumm/plot/guardian/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/guardian/core.py` & `gwsumm-2.2.5/gwsumm/plot/guardian/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/guardian/tests/__init__.py` & `gwsumm-2.2.5/gwsumm/plot/guardian/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/guardian/tests/test_main.py` & `gwsumm-2.2.5/gwsumm/plot/guardian/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/mixins.py` & `gwsumm-2.2.5/gwsumm/plot/mixins.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/noisebudget.py` & `gwsumm-2.2.5/gwsumm/plot/noisebudget.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/range.py` & `gwsumm-2.2.5/gwsumm/plot/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/registry.py` & `gwsumm-2.2.5/gwsumm/plot/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/segments.py` & `gwsumm-2.2.5/gwsumm/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/sei.py` & `gwsumm-2.2.5/gwsumm/plot/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/triggers/__init__.py` & `gwsumm-2.2.5/gwsumm/plot/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/triggers/__main__.py` & `gwsumm-2.2.5/gwsumm/plot/triggers/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/triggers/core.py` & `gwsumm-2.2.5/gwsumm/plot/triggers/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/triggers/tests/__init__.py` & `gwsumm-2.2.5/gwsumm/plot/triggers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/triggers/tests/test_main.py` & `gwsumm-2.2.5/gwsumm/plot/triggers/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/plot/utils.py` & `gwsumm-2.2.5/gwsumm/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/segments.py` & `gwsumm-2.2.5/gwsumm/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/state/__init__.py` & `gwsumm-2.2.5/gwsumm/state/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/state/all.py` & `gwsumm-2.2.5/gwsumm/state/all.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/state/core.py` & `gwsumm-2.2.5/gwsumm/state/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/state/registry.py` & `gwsumm-2.2.5/gwsumm/state/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/__init__.py` & `gwsumm-2.2.5/gwsumm/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/builtin.py` & `gwsumm-2.2.5/gwsumm/tabs/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/core.py` & `gwsumm-2.2.5/gwsumm/tabs/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/data.py` & `gwsumm-2.2.5/gwsumm/tabs/data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/etg.py` & `gwsumm-2.2.5/gwsumm/tabs/etg.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/fscan.py` & `gwsumm-2.2.5/gwsumm/tabs/fscan.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/gracedb.py` & `gwsumm-2.2.5/gwsumm/tabs/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/guardian.py` & `gwsumm-2.2.5/gwsumm/tabs/guardian.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/management.py` & `gwsumm-2.2.5/gwsumm/tabs/management.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/misc.py` & `gwsumm-2.2.5/gwsumm/tabs/misc.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/registry.py` & `gwsumm-2.2.5/gwsumm/tabs/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/sei.py` & `gwsumm-2.2.5/gwsumm/tabs/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tabs/stamp.py` & `gwsumm-2.2.5/gwsumm/tabs/stamp.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/__init__.py` & `gwsumm-2.2.5/gwsumm/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/common.py` & `gwsumm-2.2.5/gwsumm/tests/common.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_archive.py` & `gwsumm-2.2.5/gwsumm/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_batch.py` & `gwsumm-2.2.5/gwsumm/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_channels.py` & `gwsumm-2.2.5/gwsumm/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_config.py` & `gwsumm-2.2.5/gwsumm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_data.py` & `gwsumm-2.2.5/gwsumm/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_mode.py` & `gwsumm-2.2.5/gwsumm/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_plot.py` & `gwsumm-2.2.5/gwsumm/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_tabs.py` & `gwsumm-2.2.5/gwsumm/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/tests/test_utils.py` & `gwsumm-2.2.5/gwsumm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/triggers.py` & `gwsumm-2.2.5/gwsumm/triggers.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/units.py` & `gwsumm-2.2.5/gwsumm/units.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm/utils.py` & `gwsumm-2.2.5/gwsumm/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/gwsumm.egg-info/PKG-INFO` & `gwsumm-2.2.5/gwsumm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.2.4
+Requires-Dist: gwdetchar>=2.2.5
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.4/gwsumm.egg-info/SOURCES.txt` & `gwsumm-2.2.5/gwsumm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.4/pyproject.toml` & `gwsumm-2.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   "Topic :: Scientific/Engineering :: Astronomy",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 dependencies = [
   "astropy >=3.0.0",
   "gwdatafind >=1.1.1",
-  "gwdetchar >=2.2.4",
+  "gwdetchar >=2.2.5",
   "gwpy >=2.0.0",
   "gwtrigfind",
   "lalsuite",
   "ligo-segments",
   "lscsoft-glue >=1.60.0",
   "lxml",
   "markdown",
```

