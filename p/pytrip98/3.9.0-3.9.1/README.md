# Comparing `tmp/pytrip98-3.9.0.tar.gz` & `tmp/pytrip98-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrip98-3.9.0.tar", last modified: Sat Sep 23 19:43:30 2023, max compression
+gzip compressed data, was "pytrip98-3.9.1.tar", last modified: Thu Apr 18 12:13:55 2024, max compression
```

## Comparing `pytrip98-3.9.0.tar` & `pytrip98-3.9.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.828268 pytrip98-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-23 19:43:22.000000 pytrip98-3.9.0/GPL_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-09-23 19:43:22.000000 pytrip98-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-09-23 19:43:22.000000 pytrip98-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-09-23 19:43:30.828268 pytrip98-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-23 19:43:22.000000 pytrip98-3.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.820268 pytrip98-3.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.820268 pytrip98-3.9.0/docs/apidoc/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/apidoc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/apidoc/pytrip.rst
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/technical.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-09-23 19:43:22.000000 pytrip98-3.9.0/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.820268 pytrip98-3.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-09-23 19:43:22.000000 pytrip98-3.9.0/examples/example00_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-09-23 19:43:22.000000 pytrip98-3.9.0/examples/example01_vdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2023-09-23 19:43:22.000000 pytrip98-3.9.0/examples/example02_trip98.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.824268 pytrip98-3.9.0/pytrip/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-09-23 19:43:28.000000 pytrip98-3.9.0/pytrip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    43981 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/cube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.824268 pytrip98-3.9.0/pytrip/data/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/data/OER_barendsen.dat
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/data/OER_furusawa_HSG_C12.dat
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/data/OER_furusawa_V79_C12.dat
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/data/hlut_den.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/ddd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/dicomhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/let.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.824268 pytrip98-3.9.0/pytrip/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    65865 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/lib/cntr.c
--rw-r--r--   0 runner    (1001) docker     (127)    38277 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/lib/core.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.824268 pytrip98-3.9.0/pytrip/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/models/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/models/proton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/models/rcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/models/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    12804 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.824268 pytrip98-3.9.0/pytrip/res/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/res/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/res/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/res/point.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/res/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26613 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/spc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.828268 pytrip98-3.9.0/pytrip/tripexecuter/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/execparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    28227 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/executor_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    27196 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/tripexecuter/projectile.py
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.828268 pytrip98-3.9.0/pytrip/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3922 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/bevlet2oer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14404 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/cubeslice.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/dicom2trip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4174 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/dvhplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/gd2agr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11138 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/gd2dat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2143 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/rst2sobp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2843 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/rst_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/spc2pdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2681 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/utils/trip2dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)    80619 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/vdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-09-23 19:43:22.000000 pytrip98-3.9.0/pytrip/volhist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 19:43:30.828268 pytrip98-3.9.0/pytrip98.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-23 19:43:30.000000 pytrip98-3.9.0/pytrip98.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-09-23 19:43:22.000000 pytrip98-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-09-23 19:43:30.828268 pytrip98-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2023-09-23 19:43:22.000000 pytrip98-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.512236 pytrip98-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 12:13:48.000000 pytrip98-3.9.1/GPL_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-18 12:13:48.000000 pytrip98-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 12:13:48.000000 pytrip98-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-18 12:13:55.512236 pytrip98-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-18 12:13:48.000000 pytrip98-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.500236 pytrip98-3.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.500236 pytrip98-3.9.1/docs/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/apidoc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/apidoc/pytrip.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/technical.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-18 12:13:48.000000 pytrip98-3.9.1/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.500236 pytrip98-3.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-18 12:13:48.000000 pytrip98-3.9.1/examples/example00_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-18 12:13:48.000000 pytrip98-3.9.1/examples/example01_vdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-18 12:13:48.000000 pytrip98-3.9.1/examples/example02_trip98.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.504236 pytrip98-3.9.1/pytrip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-18 12:13:53.000000 pytrip98-3.9.1/pytrip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43984 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.504236 pytrip98-3.9.1/pytrip/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/data/OER_barendsen.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/data/OER_furusawa_HSG_C12.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/data/OER_furusawa_V79_C12.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/data/hlut_den.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/ddd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/dicomhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/let.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.504236 pytrip98-3.9.1/pytrip/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    65865 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/lib/cntr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/lib/core.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.504236 pytrip98-3.9.1/pytrip/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/models/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/models/proton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/models/rcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/models/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.508237 pytrip98-3.9.1/pytrip/res/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/res/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/res/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/res/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/res/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/spc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.508237 pytrip98-3.9.1/pytrip/tripexecuter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/execparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28227 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/executor_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/tripexecuter/projectile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.508237 pytrip98-3.9.1/pytrip/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4250 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/bevlet2oer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14404 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/cubeslice.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/dicom2trip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4174 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/dvhplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/gd2agr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11138 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/gd2dat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2143 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/rst2sobp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2843 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/rst_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/spc2pdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2681 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/utils/trip2dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80619 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/vdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-18 12:13:48.000000 pytrip98-3.9.1/pytrip/volhist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:13:55.512236 pytrip98-3.9.1/pytrip98.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 12:13:55.000000 pytrip98-3.9.1/pytrip98.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 12:13:48.000000 pytrip98-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 12:13:55.512236 pytrip98-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-18 12:13:48.000000 pytrip98-3.9.1/setup.py
```

### Comparing `pytrip98-3.9.0/GPL_LICENSE` & `pytrip98-3.9.1/GPL_LICENSE`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/LICENSE` & `pytrip98-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/PKG-INFO` & `pytrip98-3.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrip98
-Version: 3.9.0
+Version: 3.9.1
 Summary: PyTRiP
 Home-page: https://github.com/pytrip/pytrip
 Author: Jakob Toftegaard, Niels Bassler, Leszek Grzanka
 Author-email: leszek.grzanka@ifj.edu.pl
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,23 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: matplotlib
-Requires-Dist: pydicom>=2.3.1; python_version == "3.11"
-Requires-Dist: pydicom; python_version < "3.11"
+Requires-Dist: pydicom
 Requires-Dist: scipy
+Requires-Dist: packaging
+Requires-Dist: numpy>=1.26.0; python_version == "3.12"
 Requires-Dist: numpy>=1.23.3; python_version == "3.11"
 Requires-Dist: numpy>=1.21.4; python_version == "3.10"
 Requires-Dist: numpy>=1.20; python_version == "3.9"
 Requires-Dist: numpy>=1.18; python_version == "3.8"
 Requires-Dist: numpy>=1.15; python_version == "3.7"
 Requires-Dist: numpy<1.20,>=1.12; python_version == "3.6"
 Provides-Extra: remote
```

### Comparing `pytrip98-3.9.0/README.rst` & `pytrip98-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/authors.rst` & `pytrip98-3.9.1/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/conf.py` & `pytrip98-3.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/contributing.rst` & `pytrip98-3.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/examples.rst` & `pytrip98-3.9.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/getting_started.rst` & `pytrip98-3.9.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/install.rst` & `pytrip98-3.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/technical.rst` & `pytrip98-3.9.1/docs/technical.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/docs/user_guide.rst` & `pytrip98-3.9.1/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/examples/example00_basic.py` & `pytrip98-3.9.1/examples/example00_basic.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/examples/example01_vdx.py` & `pytrip98-3.9.1/examples/example01_vdx.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/examples/example02_trip98.py` & `pytrip98-3.9.1/examples/example02_trip98.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/__init__.py` & `pytrip98-3.9.1/pytrip/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,8 +38,8 @@
            'Rst']
 
 # if an application using pytrip doesn't configure any logging level, then an error will occur
 # to prevent it, we add null logging handler, as suggested by Python documentation:
 # as described here: https://docs.python.org/3/howto/logging.html#library-config
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
-__version__ = '3.9.0'
+__version__ = '3.9.1'
```

### Comparing `pytrip98-3.9.0/pytrip/ctx.py` & `pytrip98-3.9.1/pytrip/ctx.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/cube.py` & `pytrip98-3.9.1/pytrip/cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,19 +218,19 @@
 
         :params Cube a: the first cube to be compared with the second (b).
         :params Cube b: the second cube to be compared with the first (a).
 
         """
         eps = 1e-5
 
-        x_dim_compatible = (a.dimx == b.dimx)
-        y_dim_compatible = (a.dimy == b.dimy)
-        z_dim_compatible = (a.dimz == b.dimz)
-        pixel_size_compatible = (a.pixel_size - b.pixel_size <= eps)
-        slice_distance_compatible = (a.slice_distance == b.slice_distance)
+        x_dim_compatible = a.dimx == b.dimx
+        y_dim_compatible = a.dimy == b.dimy
+        z_dim_compatible = a.dimz == b.dimz
+        pixel_size_compatible = a.pixel_size - b.pixel_size <= eps
+        slice_distance_compatible = a.slice_distance == b.slice_distance
         return x_dim_compatible and y_dim_compatible and z_dim_compatible and pixel_size_compatible and \
             slice_distance_compatible
 
     def indices_to_pos(self, indices):
         """ Translate index number of a voxel to real position in [mm], including any offsets.
 
         The z position is always following the slice positions.
@@ -715,19 +715,20 @@
         return header_path, datafile_path
 
     def _write_trip_header(self, path):
         """ Write a TRiP98 formatted header file, based on the available meta data.
 
         :param path: fully qualified path, including file extension (.hed)
         """
-        from distutils.version import LooseVersion  # skipcq: PYL-W0402
+        from packaging.version import parse as parse_version  # skipcq: PYL-W0402
+
         output_str = "version " + self.version + "\n"
         output_str += "modality " + self.modality + "\n"
         # include created_by and creation_info only for files newer than 1.4
-        if LooseVersion(self.version) >= LooseVersion("1.4"):
+        if parse_version(self.version) >= parse_version("1.4"):
             output_str += f"created_by {self.created_by}\n"
             output_str += f"creation_info {self.creation_info}\n"
         output_str += "primary_view " + self.primary_view + "\n"
         output_str += "data_type " + self.data_type + "\n"
         output_str += "num_bytes " + str(self.num_bytes) + "\n"
         output_str += "byte_order " + self.byte_order + "\n"
         if self.patient_name == "":
```

### Comparing `pytrip98-3.9.0/pytrip/data/OER_barendsen.dat` & `pytrip98-3.9.1/pytrip/data/OER_barendsen.dat`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/data/OER_furusawa_HSG_C12.dat` & `pytrip98-3.9.1/pytrip/data/OER_furusawa_HSG_C12.dat`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/data/OER_furusawa_V79_C12.dat` & `pytrip98-3.9.1/pytrip/data/OER_furusawa_V79_C12.dat`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/ddd.py` & `pytrip98-3.9.1/pytrip/ddd.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/dicomhelper.py` & `pytrip98-3.9.1/pytrip/dicomhelper.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/dos.py` & `pytrip98-3.9.1/pytrip/dos.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/error.py` & `pytrip98-3.9.1/pytrip/error.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/field.py` & `pytrip98-3.9.1/pytrip/field.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/file_parser.py` & `pytrip98-3.9.1/pytrip/file_parser.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/let.py` & `pytrip98-3.9.1/pytrip/let.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/lib/cntr.c` & `pytrip98-3.9.1/pytrip/lib/cntr.c`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/lib/core.c` & `pytrip98-3.9.1/pytrip/lib/core.c`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/models/__init__.py` & `pytrip98-3.9.1/pytrip/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/models/extra.py` & `pytrip98-3.9.1/pytrip/models/extra.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/models/proton.py` & `pytrip98-3.9.1/pytrip/models/proton.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/models/rcr.py` & `pytrip98-3.9.1/pytrip/models/rcr.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/models/tcp.py` & `pytrip98-3.9.1/pytrip/models/tcp.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/paths.py` & `pytrip98-3.9.1/pytrip/paths.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/raster.py` & `pytrip98-3.9.1/pytrip/raster.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/res/__init__.py` & `pytrip98-3.9.1/pytrip/res/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/res/contour.py` & `pytrip98-3.9.1/pytrip/res/contour.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/res/interpolate.py` & `pytrip98-3.9.1/pytrip/res/interpolate.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/res/point.py` & `pytrip98-3.9.1/pytrip/res/point.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/res/utils.py` & `pytrip98-3.9.1/pytrip/res/utils.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/spc.py` & `pytrip98-3.9.1/pytrip/spc.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/__init__.py` & `pytrip98-3.9.1/pytrip/tripexecuter/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/execparser.py` & `pytrip98-3.9.1/pytrip/tripexecuter/execparser.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/execute.py` & `pytrip98-3.9.1/pytrip/tripexecuter/execute.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/executor_logger.py` & `pytrip98-3.9.1/pytrip/tripexecuter/executor_logger.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/field.py` & `pytrip98-3.9.1/pytrip/tripexecuter/field.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/kernel.py` & `pytrip98-3.9.1/pytrip/tripexecuter/kernel.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/plan.py` & `pytrip98-3.9.1/pytrip/tripexecuter/plan.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/tripexecuter/projectile.py` & `pytrip98-3.9.1/pytrip/tripexecuter/projectile.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/util.py` & `pytrip98-3.9.1/pytrip/util.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/__init__.py` & `pytrip98-3.9.1/pytrip/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/bevlet2oer.py` & `pytrip98-3.9.1/pytrip/utils/bevlet2oer.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,20 +43,26 @@
         """
 
         if not os.path.isfile(gd_filename):
             raise IOError("Could not find file " + gd_filename)
 
         if _dataset > 2:
             print("DOS: Error- only 0,1,2 OER set available. Got:", _dataset)
-        from pkg_resources import resource_string
-
         model_files = ('OER_furusawa_V79_C12.dat', 'OER_furusawa_HSG_C12.dat', 'OER_barendsen.dat')
-        model_data = resource_string('pytrip', os.path.join('data', model_files[_dataset]))
 
-        lines = model_data.decode('ascii').split('\n')
+        try:
+            from importlib import resources
+            with resources.files('pytrip.data').joinpath(model_files[_dataset]).open('r') as file:
+                model_data = file.read()
+            lines = model_data.split('\n')
+        except (FileNotFoundError, AttributeError, TypeError, ImportError):
+            from pkg_resources import resource_string
+            model_data = resource_string('pytrip', os.path.join('data', model_files[_dataset]))
+            lines = model_data.decode('ascii').split('\n')
+
         x = np.asarray([float(line.split()[0]) for line in lines if line])
         y = np.asarray([float(line.split()[1]) for line in lines if line])
         us = RegularInterpolator(x, y, kind='linear')
 
         with open(gd_filename, 'r') as gd_file:
             gd_lines = gd_file.readlines()
```

### Comparing `pytrip98-3.9.0/pytrip/utils/cubeslice.py` & `pytrip98-3.9.1/pytrip/utils/cubeslice.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/dicom2trip.py` & `pytrip98-3.9.1/pytrip/utils/dicom2trip.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/dvhplot.py` & `pytrip98-3.9.1/pytrip/utils/dvhplot.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/gd2agr.py` & `pytrip98-3.9.1/pytrip/utils/gd2agr.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/gd2dat.py` & `pytrip98-3.9.1/pytrip/utils/gd2dat.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/rst2sobp.py` & `pytrip98-3.9.1/pytrip/utils/rst2sobp.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/rst_plot.py` & `pytrip98-3.9.1/pytrip/utils/rst_plot.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/spc2pdf.py` & `pytrip98-3.9.1/pytrip/utils/spc2pdf.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/utils/trip2dicom.py` & `pytrip98-3.9.1/pytrip/utils/trip2dicom.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/vdx.py` & `pytrip98-3.9.1/pytrip/vdx.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip/volhist.py` & `pytrip98-3.9.1/pytrip/volhist.py`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/pytrip98.egg-info/PKG-INFO` & `pytrip98-3.9.1/pytrip98.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrip98
-Version: 3.9.0
+Version: 3.9.1
 Summary: PyTRiP
 Home-page: https://github.com/pytrip/pytrip
 Author: Jakob Toftegaard, Niels Bassler, Leszek Grzanka
 Author-email: leszek.grzanka@ifj.edu.pl
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,23 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: matplotlib
-Requires-Dist: pydicom>=2.3.1; python_version == "3.11"
-Requires-Dist: pydicom; python_version < "3.11"
+Requires-Dist: pydicom
 Requires-Dist: scipy
+Requires-Dist: packaging
+Requires-Dist: numpy>=1.26.0; python_version == "3.12"
 Requires-Dist: numpy>=1.23.3; python_version == "3.11"
 Requires-Dist: numpy>=1.21.4; python_version == "3.10"
 Requires-Dist: numpy>=1.20; python_version == "3.9"
 Requires-Dist: numpy>=1.18; python_version == "3.8"
 Requires-Dist: numpy>=1.15; python_version == "3.7"
 Requires-Dist: numpy<1.20,>=1.12; python_version == "3.6"
 Provides-Extra: remote
```

### Comparing `pytrip98-3.9.0/pytrip98.egg-info/SOURCES.txt` & `pytrip98-3.9.1/pytrip98.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrip98-3.9.0/setup.py` & `pytrip98-3.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,30 @@
 
 class build_ext(_build_ext):
     """
     From https://stackoverflow.com/questions/19919905/how-to-bootstrap-numpy-installation-in-setup-py/21621689#21621689
     """
     def finalize_options(self):
         _build_ext.finalize_options(self)
-        # Prevent numpy from thinking it is still in its setup process:
-        __builtins__.__NUMPY_SETUP__ = False
+
         import numpy
+
+        # Prevent numpy from thinking it is still in its setup process
+        # http://stackoverflow.com/questions/19919905/how-to-bootstrap-numpy-installation-in-setup-py
+        #
+        # Newer numpy versions don't support this hack, nor do they need it.
+        # https://github.com/pyvista/pyacvd/pull/23#issue-1298467701
+        #
+        # inspired by https://github.com/piskvorky/gensim/commit/2fd3e89ca42a7812a71c608572aba2e858377c8c
+        import builtins
+        try:
+            builtins.__NUMPY_SETUP__ = False
+        except Exception as ex:
+            print(f'could not use __NUMPY_SETUP__ hack (numpy version: {numpy.__version__}): {ex}')
+
         print("Building package with numpy version {}".format(numpy.__version__))  # skipcq: PYL-C0209
         self.include_dirs.append(numpy.get_include())
 
 
 def git_version():
     """
     Inspired by https://github.com/numpy/numpy/blob/master/setup.py
@@ -63,17 +76,17 @@
         GIT_REVISION = out.strip().decode('ascii')
         if GIT_REVISION:
             no_of_commits_since_last_tag = int(GIT_REVISION.split('-')[1])
             tag_name = GIT_REVISION.split('-')[0][1:]
             if no_of_commits_since_last_tag == 0:
                 return tag_name
             return '{}+rev{}'.format(tag_name, no_of_commits_since_last_tag)  # skipcq: PYL-C0209
-        return "Unknown"
+        return "0.0.0"
     except OSError:
-        return "Unknown"
+        return "0.0.0"
 
 
 def pytrip_init_version():
     """
     read pytrip/__init__.py file and get __version__ variable
     we don't import it, because that module may require packages that are not available yet
     :return: version from pytrip
@@ -82,20 +95,20 @@
         lines = f.readlines()
     for line in reversed(lines):
         if line.startswith("__version__"):
             line = line.split('#')[0]  # remove comment
             delim = '"' if '"' in line else "'"  # check if string is in " or '
             version = line.split(delim)[1]
             return version
-    return "Unknown"
+    return "0.0.0"
 
 
 def get_version():
     version = git_version()
-    if version != "Unknown":
+    if version != "0.0.0":
         return version
     return pytrip_init_version()
 
 
 def write_version_py(version, filename='pytrip/__init__.py'):
     if not filename.endswith('.py'):
         print("Wrong filename")
@@ -116,20 +129,21 @@
 
 
 # packages specified in setup_requires are needed only when running setup.py, in our case it is only numpy
 # which needs to provide header files (via numpy.get_include()) required to build C extension
 # numpy is also added install_requires which is list of dependencies needed by pip when running `pip install`
 #
 # from time to time numpy is introducing new binary API
-# detailed list of API versions: https://github.com/numpy/numpy/blob/main/numpy/core/code_generators/cversions.txt
+# detailed list of API versions: https://github.com/numpy/numpy/blob/main/numpy/_core/code_generators/cversions.txt
 # we are taking the approach to build pytrip wheel package with oldest available API version for given python version
 # here is table with corresponding numpy versions, numpy API version and supported python versions
 # ----------------------------------------------------------------|
 # | numpy version | numpy API | python versions |    OS support   |
 # ----------------------------------------------------------------|
+# |    1.25.0-    | 17 (0x11) |   3.11 - 3.12   | linux, mac, win |
 # |    1.23.3-    | 16 (0x10) |    3.8 - 3.11   | linux, mac, win |
 # | 1.23.0-1.23.2 | 16 (0x10) |    3.8 - 3.10   | linux, mac, win |
 # |      1.22     | 15 (0xf)  |    3.8 - 3.10   | linux, mac, win |
 # |   1.21.4-     | 14 (0xe)  |    3.7 - 3.10   | linux, mac, win |
 # | 1.21.0-1.21.3 | 14 (0xe)  |    3.7 - 3.9    | linux, mac, win |
 # |      1.20     | 14 (0xe)  |    3.7 - 3.9    | linux, mac, win |
 # |      1.19     | 13 (0xd)  |    3.6 - 3.8    | linux, mac, win |
@@ -139,31 +153,32 @@
 # |      1.15     | 12 (0xc)  | 2.7,  3.4 - 3.7 | linux, mac, win |
 # |      1.14     | 12 (0xc)  | 2.7,  3.4 - 3.6 | linux, mac, win |
 # |      1.13     | 11 (0xb)  | 2.7,  3.4 - 3.6 | linux, mac, win |
 # |      1.12     | 10 (0xa)  | 2.7,  3.4 - 3.6 | linux, mac, win |
 # ----------------------------------------------------------------|
 
 
-# as for now pydicom is broken under python 3.11, once this is fixed we need to replace it with normal version
 install_requires = [
     "matplotlib",
-    "pydicom>=2.3.1 ; python_version == '3.11'",
-    "pydicom ; python_version < '3.11'",
+    "pydicom",
     "scipy",
+    "packaging",
     # full range of NumPy version with support for given python version
+    "numpy>=1.26.0 ; python_version == '3.12'",
     "numpy>=1.23.3 ; python_version == '3.11'",
     "numpy>=1.21.4 ; python_version == '3.10'",
     "numpy>=1.20 ; python_version == '3.9'",
     "numpy>=1.18 ; python_version == '3.8'",
     "numpy>=1.15 ; python_version == '3.7'",
     "numpy>=1.12,<1.20 ; python_version == '3.6'"
 ]
 
 # oldest NumPy version with support for given python version
 setup_requires = [
+    "numpy==1.26.0 ; python_version == '3.12'",
     "numpy==1.23.3 ; python_version == '3.11'",
     "numpy==1.21.4 ; python_version == '3.10'",
     "numpy==1.20.0 ; python_version == '3.9'",
     "numpy==1.18.0 ; python_version == '3.8'",
     "numpy==1.15.0 ; python_version == '3.7'",
     "numpy==1.12.0 ; python_version == '3.6'"
 ]
@@ -212,14 +227,15 @@
         'Programming Language :: C',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython'
     ],
     package_data={'pytrip': ['data/*.dat', 'pytriplib.*', 'cntr.*']},
     setup_requires=setup_requires,
     install_requires=install_requires,
     extras_require=extras_require,
     ext_package='pytrip',
```

