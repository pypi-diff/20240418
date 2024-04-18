# Comparing `tmp/neura_library-0.0.2.tar.gz` & `tmp/neura_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neura_library-0.0.2.tar", last modified: Mon Apr 15 15:44:41 2024, max compression
+gzip compressed data, was "neura_library-0.0.3.tar", last modified: Thu Apr 18 14:32:00 2024, max compression
```

## Comparing `neura_library-0.0.2.tar` & `neura_library-0.0.3.tar`

### file list

```diff
@@ -1,173 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.738708 neura_library-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-15 15:44:35.000000 neura_library-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-15 15:44:41.738708 neura_library-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-15 15:44:35.000000 neura_library-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-15 15:44:35.000000 neura_library-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 15:44:35.000000 neura_library-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:44:41.738708 neura_library-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.710707 neura_library-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.738708 neura_library-0.0.2/src/neura_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 15:44:41.000000 neura_library-0.0.2/src/neura_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.718707 neura_library-0.0.2/src/neuralib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.718707 neura_library-0.0.2/src/neuralib/argp/
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/argp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/argp/_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/argp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/argp/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.718707 neura_library-0.0.2/src/neuralib/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/allen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.718707 neura_library-0.0.2/src/neuralib/atlas/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/probe_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/roi_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/brainrender/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.718707 neura_library-0.0.2/src/neuralib/atlas/ccf/
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ccf/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ccf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ccf/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ccf/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/atlas/cellatlas/
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/cellatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/cellatlas/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/atlas/ibl/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ibl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/ibl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/atlas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/bokeh_model/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/example_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/bokeh_model/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_animal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/bokeh_model/view_brain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/calimg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/calimg/scan_image/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/scan_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/scan_image/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/calimg/scanbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/scanbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/scanbox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/scanbox/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.722707 neura_library-0.0.2/src/neuralib/calimg/suite2p/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/suite2p/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/calimg/suite2p/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/imglib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/imglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/imglib/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/imglib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/persistence/cli_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/persistence/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/plot/venn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/scanner/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/scanner/czi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/scanner/lsm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.726707 neura_library-0.0.2/src/neuralib/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/segmentation/cellpose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/cellpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/cellpose/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/cellpose/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/cellpose/run_subproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/segmentation/stardist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/segmentation/stardist/run_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/stimpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/baselog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/baseprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/camlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/event.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/stimpy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/stimpy_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/stimpy_pyv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/stimulus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/stimpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/tools/pkl_parq_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/tools/pkl_parq_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/tools/pkl_parq_view/main_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.730708 neura_library-0.0.2/src/neuralib/tools/slack_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/tools/slack_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/tools/slack_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.734707 neura_library-0.0.2/src/neuralib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/color_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/segement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/util_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/util_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.734707 neura_library-0.0.2/src/neuralib/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.734707 neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.734707 neura_library-0.0.2/src/neuralib/wrapper/facemap/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/facemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/facemap/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/facemap/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.734707 neura_library-0.0.2/src/neuralib/wrapper/rastermap/
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-15 15:44:35.000000 neura_library-0.0.2/src/neuralib/wrapper/rastermap/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:41.738708 neura_library-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_argp.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_argp_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_csv_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_persistence_autoinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_pyvstim_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    62247 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_stimpy_bitbucket_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-04-15 15:44:35.000000 neura_library-0.0.2/test/test_stimpy_github_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.270921 neura_library-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-18 14:31:53.000000 neura_library-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-18 14:32:00.270921 neura_library-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-18 14:31:53.000000 neura_library-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 14:31:53.000000 neura_library-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 14:31:53.000000 neura_library-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:32:00.270921 neura_library-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.238921 neura_library-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.270921 neura_library-0.0.3/src/neura_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 14:32:00.000000 neura_library-0.0.3/src/neura_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.246921 neura_library-0.0.3/src/neuralib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.246921 neura_library-0.0.3/src/neuralib/argp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/argp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/argp/_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/argp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/argp/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.246921 neura_library-0.0.3/src/neuralib/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/allen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.250921 neura_library-0.0.3/src/neuralib/atlas/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/probe_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/roi_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/brainrender/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.250921 neura_library-0.0.3/src/neuralib/atlas/ccf/
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ccf/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ccf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ccf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ccf/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.250921 neura_library-0.0.3/src/neuralib/atlas/cellatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/cellatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/cellatlas/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.250921 neura_library-0.0.3/src/neuralib/atlas/ibl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ibl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/ibl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/atlas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/bokeh_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/example_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/bokeh_model/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_animal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/bokeh_model/view_brain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/calimg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/calimg/scan_image/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/scan_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/scan_image/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/calimg/scanbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/scanbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/scanbox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/scanbox/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.254921 neura_library-0.0.3/src/neuralib/calimg/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/suite2p/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/calimg/suite2p/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/imglib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/imglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/imglib/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/imglib/labeller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/imglib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/model/bayes_decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/model/bayes_decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/model/bayes_decoding/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/persistence/cli_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/persistence/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/plot/venn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.258921 neura_library-0.0.3/src/neuralib/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/scanner/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/scanner/czi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/scanner/lsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/segmentation/cellpose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/cellpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/cellpose/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/cellpose/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/cellpose/run_subproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/segmentation/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/segmentation/stardist/run_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/stimpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/baselog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/baseprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/camlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/stimpy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/stimpy_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/stimpy_pyv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/stimulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/stimpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.262921 neura_library-0.0.3/src/neuralib/tools/pkl_parq_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/tools/pkl_parq_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/tools/pkl_parq_view/main_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.266921 neura_library-0.0.3/src/neuralib/tools/slack_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/tools/slack_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/tools/slack_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.266921 neura_library-0.0.3/src/neuralib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/color_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/segement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/util_cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/util_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.266921 neura_library-0.0.3/src/neuralib/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.266921 neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.270921 neura_library-0.0.3/src/neuralib/wrapper/facemap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/facemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/facemap/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/facemap/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.270921 neura_library-0.0.3/src/neuralib/wrapper/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-18 14:31:53.000000 neura_library-0.0.3/src/neuralib/wrapper/rastermap/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:00.270921 neura_library-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_argp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_argp_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_csv_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_persistence_autoinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_pyvstim_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62247 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_stimpy_bitbucket_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-04-18 14:31:53.000000 neura_library-0.0.3/test/test_stimpy_github_parser.py
```

### Comparing `neura_library-0.0.2/LICENSE` & `neura_library-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/PKG-INFO` & `neura_library-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
@@ -46,39 +46,37 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0
 Requires-Dist: colorama
 Requires-Dist: matplotlib
 Requires-Dist: seaborn~=0.12.1
-Requires-Dist: memory_profiler
-Requires-Dist: numpy
-Requires-Dist: numba
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.12
+Requires-Dist: scikit-image
 Requires-Dist: pandas~=1.5.0
-Requires-Dist: pyarrow
-Requires-Dist: psutil
 Requires-Dist: polars>=0.20.9
-Requires-Dist: sbxreader
-Requires-Dist: scikit-image
-Requires-Dist: scipy>=1.12
+Requires-Dist: pyarrow
 Requires-Dist: tifffile==2023.4.12
+Requires-Dist: opencv-python~=4.8.0.76
 Requires-Dist: tqdm~=4.62.3
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: typing_extensions
-Requires-Dist: gspread~=5.7.2
-Requires-Dist: opencv-python~=4.8.0.76
 
 
 # neuralib
 
 [![Document Status](https://readthedocs.org/projects/neuralib/badge/?version=latest)](https://neuralib.readthedocs.io/en/latest/index.html)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neura-library)
+[![PyPI version](https://badge.fury.io/py/neura-library.svg)](https://badge.fury.io/py/neura-library)
+[![Downloads](https://static.pepy.tech/badge/neura-library)](https://pepy.tech/project/neura-library)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ytsimon2004/neuralib)
 
-- Utility tools for system neuroscience research, including Open Source Wrapper or Parser
+- Utility tools for rodent system neuroscience research, including Open Source Wrapper or Parser
 
 ## Installation
 
 - `pip install neura-library` in your conda env with Python >= 3.9
 - According to purpose, install the optional package [requirements-optional.txt](requirements-optional.txt)
 
 ## Usage
@@ -165,14 +163,8 @@
 
 ## project.scripts using cli
 
 ### `brender`
 
 - see examples in [api](https://neuralib.readthedocs.io/en/latest/api/neuralib.atlas.brainrender.html)
 
-### `ppv`
 
-- python pickle/parquet file viewer
-  ~~~
-  ppv <FILE>
-  ~~~
-- see `-h` for detail
```

### Comparing `neura_library-0.0.2/README.md` & `neura_library-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 # neuralib
 
 [![Document Status](https://readthedocs.org/projects/neuralib/badge/?version=latest)](https://neuralib.readthedocs.io/en/latest/index.html)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neura-library)
+[![PyPI version](https://badge.fury.io/py/neura-library.svg)](https://badge.fury.io/py/neura-library)
+[![Downloads](https://static.pepy.tech/badge/neura-library)](https://pepy.tech/project/neura-library)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ytsimon2004/neuralib)
 
-- Utility tools for system neuroscience research, including Open Source Wrapper or Parser
+- Utility tools for rodent system neuroscience research, including Open Source Wrapper or Parser
 
 ## Installation
 
 - `pip install neura-library` in your conda env with Python >= 3.9
 - According to purpose, install the optional package [requirements-optional.txt](requirements-optional.txt)
 
 ## Usage
@@ -95,14 +98,8 @@
 
 ## project.scripts using cli
 
 ### `brender`
 
 - see examples in [api](https://neuralib.readthedocs.io/en/latest/api/neuralib.atlas.brainrender.html)
 
-### `ppv`
 
-- python pickle/parquet file viewer
-  ~~~
-  ppv <FILE>
-  ~~~
-- see `-h` for detail
```

### Comparing `neura_library-0.0.2/pyproject.toml` & `neura_library-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neura-library"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.9"
 description = "Utility tools for system neuroscience research, including Open Source Wrapper or Parser"
 authors = [
     { name = "Yu-Ting Wei", email = "ytsimon2004@gmail.com" },
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `neura_library-0.0.2/src/neura_library.egg-info/PKG-INFO` & `neura_library-0.0.3/src/neura_library.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
@@ -46,39 +46,37 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0
 Requires-Dist: colorama
 Requires-Dist: matplotlib
 Requires-Dist: seaborn~=0.12.1
-Requires-Dist: memory_profiler
-Requires-Dist: numpy
-Requires-Dist: numba
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.12
+Requires-Dist: scikit-image
 Requires-Dist: pandas~=1.5.0
-Requires-Dist: pyarrow
-Requires-Dist: psutil
 Requires-Dist: polars>=0.20.9
-Requires-Dist: sbxreader
-Requires-Dist: scikit-image
-Requires-Dist: scipy>=1.12
+Requires-Dist: pyarrow
 Requires-Dist: tifffile==2023.4.12
+Requires-Dist: opencv-python~=4.8.0.76
 Requires-Dist: tqdm~=4.62.3
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: typing_extensions
-Requires-Dist: gspread~=5.7.2
-Requires-Dist: opencv-python~=4.8.0.76
 
 
 # neuralib
 
 [![Document Status](https://readthedocs.org/projects/neuralib/badge/?version=latest)](https://neuralib.readthedocs.io/en/latest/index.html)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neura-library)
+[![PyPI version](https://badge.fury.io/py/neura-library.svg)](https://badge.fury.io/py/neura-library)
+[![Downloads](https://static.pepy.tech/badge/neura-library)](https://pepy.tech/project/neura-library)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ytsimon2004/neuralib)
 
-- Utility tools for system neuroscience research, including Open Source Wrapper or Parser
+- Utility tools for rodent system neuroscience research, including Open Source Wrapper or Parser
 
 ## Installation
 
 - `pip install neura-library` in your conda env with Python >= 3.9
 - According to purpose, install the optional package [requirements-optional.txt](requirements-optional.txt)
 
 ## Usage
@@ -165,14 +163,8 @@
 
 ## project.scripts using cli
 
 ### `brender`
 
 - see examples in [api](https://neuralib.readthedocs.io/en/latest/api/neuralib.atlas.brainrender.html)
 
-### `ppv`
 
-- python pickle/parquet file viewer
-  ~~~
-  ppv <FILE>
-  ~~~
-- see `-h` for detail
```

### Comparing `neura_library-0.0.2/src/neura_library.egg-info/SOURCES.txt` & `neura_library-0.0.3/src/neura_library.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,19 @@
 src/neuralib/calimg/scanbox/core.py
 src/neuralib/calimg/scanbox/viewer.py
 src/neuralib/calimg/suite2p/__init__.py
 src/neuralib/calimg/suite2p/core.py
 src/neuralib/calimg/suite2p/signals.py
 src/neuralib/imglib/__init__.py
 src/neuralib/imglib/factory.py
+src/neuralib/imglib/labeller.py
 src/neuralib/imglib/util.py
 src/neuralib/model/__init__.py
+src/neuralib/model/bayes_decoding/__init__.py
+src/neuralib/model/bayes_decoding/position.py
 src/neuralib/persistence/__init__.py
 src/neuralib/persistence/cli_persistence.py
 src/neuralib/persistence/persistence.py
 src/neuralib/plot/__init__.py
 src/neuralib/plot/animation.py
 src/neuralib/plot/colormap.py
 src/neuralib/plot/figure.py
@@ -111,14 +114,15 @@
 src/neuralib/util/gpu.py
 src/neuralib/util/io.py
 src/neuralib/util/json.py
 src/neuralib/util/profile_test.py
 src/neuralib/util/segement.py
 src/neuralib/util/table.py
 src/neuralib/util/tqdm.py
+src/neuralib/util/util_cv2.py
 src/neuralib/util/util_type.py
 src/neuralib/util/util_verbose.py
 src/neuralib/util/utils.py
 src/neuralib/util/version.py
 src/neuralib/wrapper/__init__.py
 src/neuralib/wrapper/deeplabcut/__init__.py
 src/neuralib/wrapper/deeplabcut/core.py
```

### Comparing `neura_library-0.0.2/src/neuralib/argp/__init__.py` & `neura_library-0.0.3/src/neuralib/argp/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/argp/_type.py` & `neura_library-0.0.3/src/neuralib/argp/_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/argp/core.py` & `neura_library-0.0.3/src/neuralib/argp/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/argp/dispatch.py` & `neura_library-0.0.3/src/neuralib/argp/dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/allen.py` & `neura_library-0.0.3/src/neuralib/atlas/allen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import io
 from io import BytesIO
 from pathlib import Path
+from pprint import pprint
 from typing import ClassVar, TypedDict, Literal
 
 import allensdk.core.structure_tree
 import numpy as np
 import pandas as pd
 import polars as pl
 from allensdk.core.reference_space_cache import ReferenceSpaceCache
@@ -15,15 +16,16 @@
 from neuralib.atlas.view import AbstractSliceView
 from neuralib.util.io import CCF_CACHE_DIRECTORY
 from neuralib.util.tqdm import download_with_tqdm
 from neuralib.util.util_type import PathLike, DataFrame
 from neuralib.util.util_verbose import fprint
 from neuralib.util.utils import uglob
 
-__all__ = ['AllenReferenceWrapper']
+__all__ = ['AllenReferenceWrapper',
+           'create_allen_structure_dict']
 
 
 class StructureTreeDict(TypedDict):
     """allen structure tree dict"""
     acronym: str
     graph_id: int
     graph_order: int
@@ -246,7 +248,28 @@
             .sort('total_voxel_count', descending=True)
         )
 
         if to_pandas:
             df = df.to_pandas()
 
         return df
+
+
+# ==================== #
+
+def create_allen_structure_dict(verbose=False) -> dict[str, str]:
+    """
+    Get the acronym/name pairing from structure_tree.csv
+
+    :return: key: acronym; value: full name
+    """
+    tree = AllenReferenceWrapper.load_structure_tree()
+    tree = tree.select('name', 'acronym').sort('name')
+
+    ret = {
+        acry: name
+        for name, acry in tree.iter_rows()
+    }
+    if verbose:
+        pprint(ret)
+
+    return ret
```

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/__init__.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/core.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/main_app.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/probe_rst.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/probe_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/roi_rst.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/roi_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/brainrender/util.py` & `neura_library-0.0.3/src/neuralib/atlas/brainrender/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ccf/__init__.py` & `neura_library-0.0.3/src/neuralib/atlas/ccf/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ccf/classifier.py` & `neura_library-0.0.3/src/neuralib/atlas/ccf/classifier.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ccf/core.py` & `neura_library-0.0.3/src/neuralib/atlas/ccf/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ccf/norm.py` & `neura_library-0.0.3/src/neuralib/atlas/ccf/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ccf/query.py` & `neura_library-0.0.3/src/neuralib/atlas/ccf/query.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/cellatlas/__init__.py` & `neura_library-0.0.3/src/neuralib/atlas/cellatlas/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/cellatlas/core.py` & `neura_library-0.0.3/src/neuralib/atlas/cellatlas/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ibl/__init__.py` & `neura_library-0.0.3/src/neuralib/atlas/ibl/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/ibl/plot.py` & `neura_library-0.0.3/src/neuralib/atlas/ibl/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/map.py` & `neura_library-0.0.3/src/neuralib/atlas/map.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/plot.py` & `neura_library-0.0.3/src/neuralib/atlas/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/util.py` & `neura_library-0.0.3/src/neuralib/atlas/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/atlas/view.py` & `neura_library-0.0.3/src/neuralib/atlas/view.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/base.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/example.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/example.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/example_multi.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/example_multi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_all.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_all.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_animal.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_animal.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/examples/view_figure.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/examples/view_figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/tool.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/tool.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/util.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/bokeh_model/view_brain.py` & `neura_library-0.0.3/src/neuralib/bokeh_model/view_brain.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/calimg/scan_image/wrapper.py` & `neura_library-0.0.3/src/neuralib/calimg/scan_image/wrapper.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/calimg/scanbox/core.py` & `neura_library-0.0.3/src/neuralib/calimg/scanbox/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,17 @@
 from neuralib.util.json import JsonEncodeHandler
 from neuralib.util.util_type import PathLike
 
 __all__ = [
     'SBXInfo',
     'sbx_to_json',
     #
-    'SBXScreenShot'
+    'screenshot_to_tiff'
 ]
 
-from neuralib.util.util_verbose import fprint
-
-# TODO ALSO CHECK the `res/rig/sbx/rig1/scanbox_config.m`
-
 T = TypeVar('T')  # matstruct
 A = TypeVar('A')  # sbx attr
 
 
 @dataclass(frozen=True)
 class SBXInfo(Generic[T, A]):
     """for each recording session, `exp.mat` from scanbox"""
@@ -59,15 +55,15 @@
     nchan: int | None
 
     @property
     def magidx(self) -> int:
         """info.config.magnification, used for `CalibrationInfo` idx"""
         return self.config.magnification - 1
 
-    def print_as_dict(self):
+    def print_asdict(self) -> None:
         from dataclasses import asdict
         pprint(asdict(self))
 
     @staticmethod
     def _try_find_attr(obj: T, attr: str) -> A | list:
         try:
             ret: A = getattr(obj, attr)
@@ -77,15 +73,15 @@
             return ret
 
     # =============================== #
     # attributes from SBX .mat output #
     # =============================== #
 
     @classmethod
-    def load(cls, root: Path | str) -> SBXInfo:
+    def load(cls, root: PathLike) -> SBXInfo:
         info = loadmat(root, squeeze_me=True, struct_as_record=False)['info']
 
         try:
             nchan = info.chan.nchan  # version >= 3
         except AttributeError:
             nchan = None
 
@@ -241,61 +237,92 @@
 
     # =============================== #
     # attributes from SBX .mat output #
     # =============================== #
 
     @property
     def fov_distance(self) -> tuple[float, float]:
-        """(X, Y) in um"""
-        if not self._validate_fov_distance():
-            fprint('check the runconfig for ScanBox during recording', vtype='error')
+        """(X, Y) in um.
+
+        Note this value might be hardware dependent. value return is internal usage for the lab
+        """
+        lines = self.get_config_info(self.config).lines
+
+        if self.objective == 'Nikon 16x/0.8w/WD3.0':
+            obj = 16
+        else:
+            raise NotImplementedError('')
+
+        zoom = float(self.get_config_info(self.config).magnification_list[self.magidx])
 
-        return 892, 667
+        return _get_default_scanbox_fov_dimension(lines, obj, zoom)
 
     def _validate_fov_distance(self) -> bool:
         """due to this is the info only seen in GUI"""
         obj_type = self.objective == 'Nikon 16x/0.8w/WD3.0'
         n_line = self.get_config_info(self.config).lines == 528
         mag = self.get_config_info(self.config).magnification_list[self.magidx] == '1.7'
         return all([obj_type, n_line, mag])
 
 
-def load_scanbox_config(root: Path) -> dict:
-    """load for Rig-specific default setting config of the scanbox `scanbox_config.m`
-    Note that the actual value could be changed via scanbox GUI"""
-    ret = {}
-    with root.open() as f:
-        for line in f:
-            line = line.strip().replace(' ', '')
-            if line.startswith('sbconfig'):
-                kidx = line.find('.')
-                vidx = line.find('=')
-
-                try:
-                    eidx = line.index(';')
-                    ret[line[kidx + 1:vidx]] = line[vidx + 1:eidx]
-                except ValueError:
-                    ret[line[kidx + 1:vidx]] = 'NOT IMPLEMENT'  # TODO matlab line change and `switch/case`
-                    pass
+def _get_default_scanbox_fov_dimension(lines: int,
+                                       obj_type: int,
+                                       zoom: float) -> tuple[float, float]:
+    """
+    Hardware/settings dependent fov size according to recording configuration
+
+    :param lines: number of lines for the scanning fov
+    :param obj_type: objective magnification. i.e., 16X
+    :param zoom: zoom setting during acquisition
+    :return: (X, Y) in um
+    """
+    # ~ 30hz
+    if lines == 528 and obj_type == 16:
+        if zoom == 1:
+            return 1396, 1056
+        elif zoom == 1.2:
+            return 1284, 978
+        elif zoom == 1.4:
+            return 1023, 765
+        elif zoom == 1.7:
+            return 892, 667
+        elif zoom == 2.0:
+            return 716, 531
+        elif zoom == 2.4:
+            return 632, 463
+        else:
+            raise NotImplementedError('check scanbox GUI directly')
 
-    return ret
+    else:
+        raise NotImplementedError('check scanbox GUI directly')
 
 
 def sbx_to_json(matfile: Path | str,
-                output: Path | None = None):
-    """save .mat file to json"""
+                output: Path | None = None,
+                verbose: bool = True) -> None:
+    """
+    save .mat scanbox output file as json file
+
+    :param matfile: .mat filepath
+    :param output: output filepath, if None, create a json file in the same directory
+    :param verbose: pprint as dict
+    :return:
+    """
     if isinstance(matfile, str):
         matfile = Path(matfile)
 
     mat = SBXInfo.load(matfile)
     if output is None:
         output = matfile.with_name('sbx').with_suffix('.json')
 
     dy = dataclasses.asdict(mat)
-    pprint(dy)
+
+    if verbose:
+        pprint(dy)
+
     with open(output, "w") as outfile:
         json.dump(dy, outfile, sort_keys=True, indent=4, cls=JsonEncodeHandler)
 
 
 # ========== #
 # ScreenShot #
 # ========== #
```

### Comparing `neura_library-0.0.2/src/neuralib/calimg/scanbox/viewer.py` & `neura_library-0.0.3/src/neuralib/calimg/scanbox/viewer.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,32 +4,57 @@
 from typing import Any
 
 import numpy as np
 import sbxreader
 
 from neuralib.argp import int_tuple_type
 from neuralib.calimg.scanbox.core import SBXInfo
+from neuralib.imglib.labeller import SequenceLabeller
 from neuralib.util.util_type import PathLike
+from neuralib.util.utils import uglob
+
+__all__ = ['SBXViewer']
 
 
 class SBXViewer:
+    """wrapper for sbxreader
+
+    `Dimension parameters`:
+
+        F = number of frames
+
+        P = number of optical planes
+
+        C = number of PMT channels
+
+        W = FOV width
+
+        H = FOV height
+
     """
-    wrapper for sbxreader.
-    note to check meta & sbxinfo consistency
-    """
+
     info: SBXInfo
+    """:class:`~neuralib.calimg.scanbox.core.SBXInfo`"""
+
     sbx_map: sbxreader.sbx_memmap
     """(F, P, C, W, H)"""
 
-    def __init__(self, file: PathLike):
-        if Path(file).suffix != '.sbx':
-            raise ValueError('')
+    def __init__(self, directory: PathLike):
+        """
+        :param directory: scanbox file (.sbx). In the same directory should contain the corresponding .mat file
+        """
+
+        if not Path(directory).is_dir():
+            raise NotADirectoryError(f'{directory}')
 
-        self.info = SBXInfo.load(file.with_suffix('.mat'))
-        self.sbx_map = sbxreader.sbx_memmap(file)
+        sbx = uglob(directory, '*.sbx')
+        self.sbx_map = sbxreader.sbx_memmap(sbx)
+
+        info = uglob(directory, '*.mat')
+        self.info = SBXInfo.load(info)
 
     @property
     def meta(self) -> dict[str, Any]:
         return self.sbx_map.metadata
 
     @property
     def version(self) -> int:
@@ -62,58 +87,82 @@
             else:
                 raise RuntimeError('')
         else:
             return self.info.nchan
 
     @property
     def n_frames(self) -> int:
+        """number of frames/images"""
         return int(self.info.config.frames / self.n_planes)
 
-    def display(self, frames: slice | np.ndarray | None,
-                plane: int,
-                channel: int):
-        # from rscvp.util.imglib.viewer import ImageSequencesViewer # TODO fix
+    def play(self,
+             frames: slice | np.ndarray | None,
+             plane: int,
+             channel: int):
+        """
+        Play the selected frames using customized CV2 player.
+
+        See :class:`~neuralib.imglib.labeller.SequenceLabeller`
+
+        :param frames: selected frames. If None, play all sequences
+        :param plane: number of optical planes
+        :param channel: number of PMT channel
+        :return:
+        """
 
         if frames is None:
             frames = np.arange(0, self.n_frames)
 
         data = self.sbx_map[frames, plane, channel, :, :]
         data = np.asarray(data)
-        ImageSequencesViewer.load(data).main()
 
-    def to_tiff(self, frames: slice | np.ndarray | None,
+        SequenceLabeller.load_sequences(data).main()
+
+    def to_tiff(self,
+                frames: slice | np.ndarray | None,
                 plane: int,
                 channel: int,
                 output: PathLike):
+        """
+        Convert the selected frames to tiff file
+
+        :param frames: selected frames. If None, convert all sequences
+        :param plane: number of optical planes
+        :param channel: number of PMT channel
+        :param output: output filename
+        :return:
+        """
         import tifffile
 
         if frames is None:
             frames = np.arange(0, self.n_frames)
         data = self.sbx_map[frames, plane, channel, :, :]
         tifffile.imwrite(output, data)
 
 
 def main():
     import argparse
-    ap = argparse.ArgumentParser()
+    ap = argparse.ArgumentParser(description='view or save the sbx file, If specify the output using -O, save as tiff'
+                                             'otherwise, play.')
 
     ap.add_argument('-D', '--dir', type=Path, required=True, help='directory containing .sbx/.mat scanbox output',
                     dest='directory')
     ap.add_argument('-F', '--frames', metavar='SLICE', type=int_tuple_type, default=None,
                     help='image sequences slice type', dest='frames')
     ap.add_argument('-P', '--plane', type=int, required=True, help='which optic plane', dest='plane')
     ap.add_argument('-C', '--channel', type=int, required=True, help='which pmt channel', dest='channel')
     ap.add_argument('-O', '--output', default=None, help='tiff output, if None, display the sequence', dest='output')
 
     opt = ap.parse_args()
 
-    sbx = SBXViewer(opt.directory)
+    viewer = SBXViewer(opt.directory)
     frames = np.arange(*opt.frames).astype(int) if opt.frames is not None else None
 
-    if opt.output is not None:
-        sbx.to_tiff(frames, opt.plane, opt.channel, opt.output)
+    #
+    if opt.output is None:
+        viewer.play(frames, opt.plane, opt.channel)
     else:
-        sbx.display(frames, opt.plane, opt.channel)
+        viewer.to_tiff(frames, opt.plane, opt.channel, opt.output)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `neura_library-0.0.2/src/neuralib/calimg/suite2p/__init__.py` & `neura_library-0.0.3/src/neuralib/calimg/suite2p/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/calimg/suite2p/core.py` & `neura_library-0.0.3/src/neuralib/calimg/suite2p/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/calimg/suite2p/signals.py` & `neura_library-0.0.3/src/neuralib/calimg/suite2p/signals.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/imglib/factory.py` & `neura_library-0.0.3/src/neuralib/imglib/factory.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/imglib/util.py` & `neura_library-0.0.3/src/neuralib/imglib/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 import numpy as np
 
 from neuralib.util.util_type import PathLike
 
 __all__ = [
     #
     'read_avi',
-    'pdf_as_image',
+    'read_pdf',
     #
     'tif_to_gif',
     'normalize_sequences',
     'handle_invalid_value'
 ]
 
 
 def read_avi(avi_file: PathLike,
              grey_scale: bool = True) -> np.ndarray:
-    """simple read for avi file, and collect as image array (F, W, H, *3). *optional"""
+    """simple read for avi file, and collect as image array
+
+    :param avi_file: avi filepath
+    :param grey_scale: convert to grayscale
+    :return: (F, W, H, <3>) sequences array
+    """
     cap = cv2.VideoCapture(str(avi_file))
     if not cap.isOpened():
         raise RuntimeError(f'error opening avi: {avi_file}')
 
     ret = []
     while cap.isOpened():
         flag, frame = cap.read()
@@ -33,33 +38,47 @@
         if grey_scale:
             frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
         ret.append(frame)
 
     return np.array(ret)
 
 
-def pdf_as_image(file: PathLike,
-                 single_image: bool = True,
-                 poppler_path: str | None = None,
-                 **kwargs) -> np.ndarray:
+def read_pdf(file: PathLike,
+             single_image: bool = True,
+             poppler_path: str | None = None,
+             **kwargs) -> np.ndarray:
+    """
+    Read pdf as an image array
+
+    :param file:
+    :param single_image:
+    :param poppler_path: if poppler not installed in a system level. Specify the path.
+        for example: ``Release-23.08.0-0\poppler-23.08.0\Library\bin``
+
+        .. seealso::
+
+            `<https://stackoverflow.com/questions/53481088/poppler-in-path-for-pdf2image>`_
+    :param kwargs: pass through `convert_from_path`
+    :return: image array
+    """
     from pdf2image import convert_from_path
     from pdf2image.exceptions import PDFInfoNotInstalledError
 
     if single_image:
         try:
             conv = convert_from_path(file, **kwargs)[0]
         except PDFInfoNotInstalledError:
             if poppler_path is None:
-                # https://stackoverflow.com/questions/53481088/poppler-in-path-for-pdf2image
-                poppler_path = r'C:\Users\yu-ting\Downloads\Release-23.08.0-0\poppler-23.08.0\Library\bin'
+                raise RuntimeError('download poppler first. or using apt-get / brew depending on OS')
+
             conv = convert_from_path(file, poppler_path=poppler_path, **kwargs)[0]
     else:
-        raise NotImplementedError('')
+        raise NotImplementedError('multi-pages pdf not currently support')
 
-    return np.array(conv)
+    return cv2.cvtColor(np.array(conv), cv2.COLOR_BGR2RGB)
 
 
 def tif_to_gif(image_file: PathLike,
                output_path: PathLike,
                fps: int = 30,
                **kwargs) -> None:
     """convert tif sequences to GIF"""
@@ -74,18 +93,18 @@
                         gamma_value: float = 0.5,
                         to_8bit: bool = False) -> list[np.ndarray]:
     """
     Do the normalization for the image sequences
 
     :param frames: list of image array
     :param handle_invalid: handle Nan and negative value
-    :param gamma_correction:
-    :param gamma_value
-    :param to_8bit
-    :return:
+    :param gamma_correction: to the gamma correction
+    :param gamma_value: gamma correction value
+    :param to_8bit: to 8bit images
+    :return: list of normalized image array
     """
     if handle_invalid:
         frames = handle_invalid_value(frames)
 
     if gamma_correction:
         frames = [np.power(f, gamma_value) for f in frames]
```

### Comparing `neura_library-0.0.2/src/neuralib/persistence/cli_persistence.py` & `neura_library-0.0.3/src/neuralib/persistence/cli_persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/persistence/persistence.py` & `neura_library-0.0.3/src/neuralib/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/animation.py` & `neura_library-0.0.3/src/neuralib/plot/animation.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/colormap.py` & `neura_library-0.0.3/src/neuralib/plot/colormap.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/figure.py` & `neura_library-0.0.3/src/neuralib/plot/figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                         plt.tight_layout()
                 except:
                     pass
 
                 try:
                     plt.savefig(output, dpi=dpi if dpi is not None else None)
                     break
-                except OSError as e:  # fucking bkrunch annoying
+                except OSError as e:
                     print(e)
                     input('press to continue')
 
     finally:
         plt.clf()
         plt.close('all')
```

### Comparing `neura_library-0.0.2/src/neuralib/plot/misc.py` & `neura_library-0.0.3/src/neuralib/plot/misc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/plot.py` & `neura_library-0.0.3/src/neuralib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/setting.py` & `neura_library-0.0.3/src/neuralib/plot/setting.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/tools.py` & `neura_library-0.0.3/src/neuralib/plot/tools.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/plot/venn.py` & `neura_library-0.0.3/src/neuralib/plot/venn.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/scanner/__init__.py` & `neura_library-0.0.3/src/neuralib/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/scanner/core.py` & `neura_library-0.0.3/src/neuralib/scanner/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/scanner/czi.py` & `neura_library-0.0.3/src/neuralib/scanner/czi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/scanner/lsm.py` & `neura_library-0.0.3/src/neuralib/scanner/lsm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/segmentation/base.py` & `neura_library-0.0.3/src/neuralib/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/segmentation/cellpose/core.py` & `neura_library-0.0.3/src/neuralib/segmentation/cellpose/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/segmentation/cellpose/run_api.py` & `neura_library-0.0.3/src/neuralib/segmentation/cellpose/run_api.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/segmentation/cellpose/run_subproc.py` & `neura_library-0.0.3/src/neuralib/segmentation/cellpose/run_subproc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/segmentation/stardist/run_2d.py` & `neura_library-0.0.3/src/neuralib/segmentation/stardist/run_2d.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/__init__.py` & `neura_library-0.0.3/src/neuralib/stimpy/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/baselog.py` & `neura_library-0.0.3/src/neuralib/stimpy/baselog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/baseprot.py` & `neura_library-0.0.3/src/neuralib/stimpy/baseprot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/camlog.py` & `neura_library-0.0.3/src/neuralib/stimpy/camlog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/event.py` & `neura_library-0.0.3/src/neuralib/stimpy/event.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/session.py` & `neura_library-0.0.3/src/neuralib/stimpy/session.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/stimpy_core.py` & `neura_library-0.0.3/src/neuralib/stimpy/stimpy_core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/stimpy_git.py` & `neura_library-0.0.3/src/neuralib/stimpy/stimpy_git.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/stimpy_pyv.py` & `neura_library-0.0.3/src/neuralib/stimpy/stimpy_pyv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/stimulus.py` & `neura_library-0.0.3/src/neuralib/stimpy/stimulus.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/stimpy/util.py` & `neura_library-0.0.3/src/neuralib/stimpy/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/tools/pkl_parq_view/main_app.py` & `neura_library-0.0.3/src/neuralib/tools/pkl_parq_view/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/tools/slack_bot/bot.py` & `neura_library-0.0.3/src/neuralib/tools/slack_bot/bot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/cli_args.py` & `neura_library-0.0.3/src/neuralib/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/color_logging.py` & `neura_library-0.0.3/src/neuralib/util/color_logging.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/csv.py` & `neura_library-0.0.3/src/neuralib/util/csv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/func.py` & `neura_library-0.0.3/src/neuralib/util/func.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/gpu.py` & `neura_library-0.0.3/src/neuralib/util/gpu.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/io.py` & `neura_library-0.0.3/src/neuralib/util/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/json.py` & `neura_library-0.0.3/src/neuralib/util/json.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/profile_test.py` & `neura_library-0.0.3/src/neuralib/util/profile_test.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/segement.py` & `neura_library-0.0.3/src/neuralib/util/segement.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/table.py` & `neura_library-0.0.3/src/neuralib/util/table.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/util_type.py` & `neura_library-0.0.3/src/neuralib/util/util_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/util_verbose.py` & `neura_library-0.0.3/src/neuralib/util/util_verbose.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/util/utils.py` & `neura_library-0.0.3/src/neuralib/util/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,23 @@
            'key_from_value']
 
 
 def uglob(d: PathLike,
           pattern: str,
           sort: bool = True,
           is_dir: bool = False) -> Path:
-    """Unique glob"""
+    """
+    Unique glob
+
+    :param d: directory
+    :param pattern: pattern string
+    :param sort: if sort
+    :param is_dir: only return if is a directory
+    :return: unique path
+    """
     if not isinstance(d, Path):
         d = Path(d)
 
     if not d.is_dir():
         raise ValueError(f'{d} is not a directory')
 
     f = list(d.glob(pattern))
```

### Comparing `neura_library-0.0.2/src/neuralib/util/version.py` & `neura_library-0.0.3/src/neuralib/util/version.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/core.py` & `neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/deeplabcut/util.py` & `neura_library-0.0.3/src/neuralib/wrapper/deeplabcut/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/facemap/__init__.py` & `neura_library-0.0.3/src/neuralib/wrapper/facemap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/facemap/core.py` & `neura_library-0.0.3/src/neuralib/wrapper/facemap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/facemap/util.py` & `neura_library-0.0.3/src/neuralib/wrapper/facemap/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/rastermap/__init__.py` & `neura_library-0.0.3/src/neuralib/wrapper/rastermap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/src/neuralib/wrapper/rastermap/core.py` & `neura_library-0.0.3/src/neuralib/wrapper/rastermap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_argp.py` & `neura_library-0.0.3/test/test_argp.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_argp_dispatch.py` & `neura_library-0.0.3/test/test_argp_dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_csv_context_manager.py` & `neura_library-0.0.3/test/test_csv_context_manager.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_persistence_autoinc.py` & `neura_library-0.0.3/test/test_persistence_autoinc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_pyvstim_parser.py` & `neura_library-0.0.3/test/test_pyvstim_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_stimpy_bitbucket_parser.py` & `neura_library-0.0.3/test/test_stimpy_bitbucket_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.2/test/test_stimpy_github_parser.py` & `neura_library-0.0.3/test/test_stimpy_github_parser.py`

 * *Files identical despite different names*

