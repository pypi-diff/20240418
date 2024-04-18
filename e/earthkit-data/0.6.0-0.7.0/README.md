# Comparing `tmp/earthkit-data-0.6.0.tar.gz` & `tmp/earthkit_data-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-data-0.6.0.tar", last modified: Wed Mar 27 15:33:37 2024, max compression
+gzip compressed data, was "earthkit_data-0.7.0.tar", last modified: Thu Apr 18 11:33:33 2024, max compression
```

## Comparing `earthkit-data-0.6.0.tar` & `earthkit_data-0.7.0.tar`

### file list

```diff
@@ -1,463 +1,494 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.255408 earthkit-data-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.191407 earthkit-data-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/ci-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/ci-hpc-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.191407 earthkit-data-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/workflows/ci_other.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/workflows/label-public-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-27 15:33:37.255408 earthkit-data-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.195407 earthkit-data-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.195407 earthkit-data-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    65385 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/_static/earthkit-data.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.195407 earthkit-data-0.6.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/development.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.203407 earthkit-data-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/ads.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/bufr_synop.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    80838 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/bufr_temp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/cds.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/default_fdb_schema
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/demo_sources_plugin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/ecmwf_open_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    57129 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/fdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    27906 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/from_object.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_fdb_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_file_pattern.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    51752 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_from_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_indexing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_lat_lon_value.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    88654 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_missing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_multi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_nearest_gridpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   105069 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    47387 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_tar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_time_series.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_to_netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28758 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_url.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/grib_url_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    34283 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/list_of_dict.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/mars.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    49512 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/missing.grib
--rw-r--r--   0 runner    (1001) docker     (127)    39146 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    65465 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/netcdf_fieldlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    34708 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/numpy_fieldlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/odb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36797 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/pandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/polytope.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   442939 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/projection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/settings.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/synop_10.bufr
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/temp_10.bufr
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/test.grib
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/test.nc
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/test.odb
--rw-r--r--   0 runner    (1001) docker     (127)   521712 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/test4.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/test6.grib
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/time_series.grib
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/tuv_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/tuv_pl.nc
--rw-r--r--   0 runner    (1001) docker     (127)    35809 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples/wekeo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.203407 earthkit-data-0.6.0/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/caching.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/docs/guide/data_format/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/bufr.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/data_format/odb.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/docs/guide/include/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/include/settings-get.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/include/settings-reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/include/settings-set.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/include/settings-temporary.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29025 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/sources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/guide/split_on.rst
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/howtos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/plugins/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/plugins/sources_plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/docs/release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/version_0.2_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/version_0.3_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/version_0.4_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/version_0.5_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/release_notes/version_0.6_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/docs/skip_api_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.183407 earthkit-data-0.6.0/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/earthkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.207407 earthkit-data-0.6.0/earthkit/data/arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/args_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/earthkit_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/input_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/arguments/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.211408 earthkit-data-0.6.0/earthkit/data/conf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.211408 earthkit-data-0.6.0/earthkit/data/conf/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/css/tab.css
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/css/table.css
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/css/tree.css
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/global_grids.json
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/gridspec.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/conf/gridspec_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.211408 earthkit-data-0.6.0/earthkit/data/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    40827 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/fieldlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/geography.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    20927 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/select.py
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/temporary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/core/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.211408 earthkit-data-0.6.0/earthkit/data/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/geo/distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.211408 earthkit-data-0.6.0/earthkit/data/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/indexing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.215407 earthkit-data-0.6.0/earthkit/data/indexing/database/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/indexing/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/indexing/database/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    19393 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/indexing/database/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/indexing/database/stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.215407 earthkit-data-0.6.0/earthkit/data/mergers/
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/mergers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/mergers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/mergers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.215407 earthkit-data-0.6.0/earthkit/data/mirrors/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/mirrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/mirrors/directory_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.215407 earthkit-data-0.6.0/earthkit/data/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.215407 earthkit-data-0.6.0/earthkit/data/readers/bufr/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/bufr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/bufr/bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/bufr/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/covjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/geojson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.219408 earthkit-data-0.6.0/earthkit/data/readers/grib/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/gridspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.219408 earthkit-data-0.6.0/earthkit/data/readers/grib/index/
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/index/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/index/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/index/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/index/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/grib/xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/odb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/readers/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.223408 earthkit-data-0.6.0/earthkit/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/dummy.grib
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/dummy_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/ecmwf_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/ecmwf_open_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/fdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/file_indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/file_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/numpy_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/polytope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/virtual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/virtual_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/wekeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sources/wekeocds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.223408 earthkit-data-0.6.0/earthkit/data/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sphinxext/generate_settings_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sphinxext/module_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/sphinxext/xref.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.223408 earthkit-data-0.6.0/earthkit/data/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/translators/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/translators/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/translators/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/translators/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.227408 earthkit-data-0.6.0/earthkit/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    19711 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/factorise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/module_inputs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/parts.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.227408 earthkit-data-0.6.0/earthkit/data/utils/projections/
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/projections/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/projections/proj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.227408 earthkit-data-0.6.0/earthkit/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/vocabularies/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/vocabularies/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/vocabularies/grib-paramid.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/vocabularies/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.227408 earthkit-data-0.6.0/earthkit/data/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/wrappers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.227408 earthkit-data-0.6.0/earthkit/data/writers/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/earthkit/data/writers/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.255408 earthkit-data-0.6.0/earthkit_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 15:33:37.000000 earthkit-data-0.6.0/earthkit_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-27 15:33:37.255408 earthkit-data-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.231408 earthkit-data-0.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.231408 earthkit-data-0.6.0/tests/bufr/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/bufr/test_bufr_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.231408 earthkit-data-0.6.0/tests/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/constants_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_constants_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_constants_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_constants_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_constants_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_constants_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/constants/test_contants_proc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.231408 earthkit-data-0.6.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/core/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/core/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/core/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.239408 earthkit-data-0.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2542596 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/NUTS_RG_20M_2021_3035.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   640295 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.239408 earthkit-data-0.6.0/tests/data/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/constants/proc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/era5_2t_1.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/era5_2t_2.nc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.239408 earthkit-data-0.6.0/tests/data/gridspec/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/healpix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/reduced_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/reduced_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/reduced_rotated_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/regular_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/regular_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/rotated_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/rotated_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/sh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1
--rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/mercator.grib
--rw-r--r--   0 runner    (1001) docker     (127)    47520 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/ml_data.grib
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/rgg_small_subarea_cellarea_ref.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/t_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/t_time_series.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/test_icon.grib
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/test_single.grib
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/test_single.nc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/test_single_with_missing.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/time_series.covjson
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/u_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/data/v_pl.grib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.239408 earthkit-data-0.6.0/tests/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/documentation/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/documentation/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/downstream-ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/environment-unit-tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.239408 earthkit-data-0.6.0/tests/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/geo/geo_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/geo/test_geo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.243408 earthkit-data-0.6.0/tests/grib/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/grib_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_inidces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_url.py
--rw-r--r--   0 runner    (1001) docker     (127)    14376 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_url_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/grib/test_grib_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.243408 earthkit-data-0.6.0/tests/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/indexing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_indexing_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_indexing_isel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_indexing_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_indexing_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_order_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/indexing/test_selection_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.247408 earthkit-data-0.6.0/tests/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_fieldlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/netcdf/test_netcdf_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.247408 earthkit-data-0.6.0/tests/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/aliases.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/availability.json
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_aliases_grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_normalize_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/normalize/test_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.247408 earthkit-data-0.6.0/tests/numpy_fs/
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/numpy_fs_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.247408 earthkit-data-0.6.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/plugins/test_sources_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.251408 earthkit-data-0.6.0/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_covjson_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_geojson_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_grib_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_netcdf_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_odb_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_reader_padding_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_tar_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_unknown_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/test_zip_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/unknown_file.unknown_ext
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/readers/unknown_text_file.unknown_ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.251408 earthkit-data-0.6.0/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_ecmwf_open_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_fdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_polytope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_wekeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/sources/test_wekeocds.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/test_00_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.251408 earthkit-data-0.6.0/tests/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/translators/test_translators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.251408 earthkit-data-0.6.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_download_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_module_inputs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/utils/test_projections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:33:37.255408 earthkit-data-0.6.0/tests/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/wrappers/test_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/wrappers/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/wrappers/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-27 15:33:22.000000 earthkit-data-0.6.0/tests/wrappers/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/ci-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/ci-hpc-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/ci_other.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    65385 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/earthkit-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/development.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/ads.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25628 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/bufr_synop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    80839 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/bufr_temp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/cds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    51752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/data_from_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/default_fdb_schema
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/demo_sources_plugin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/ecmwf_open_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    57129 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30675 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/file_parts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27906 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/from_object.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/geojson_geopandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25900 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_array_backends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_fdb_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23026 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_indexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_lat_lon_value.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    88655 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_missing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_nearest_gridpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   105060 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47388 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_time_series.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_to_netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34283 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/list_of_dict.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/mars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    49512 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/missing.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    16882 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/multi_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    39146 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    65479 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf_fieldlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35982 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf_opendap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/numpy_fieldlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/odb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/polytope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   442939 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/projection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/settings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/shapefile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/synop_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tar_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/temp_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.odb
+-rw-r--r--   0 runner    (1001) docker     (127)   521712 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test4.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test6.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tuv_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tuv_pl.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    28753 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url_parts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35809 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/wekeo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/data_format/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/bufr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/odb.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/parts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/split_on.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    36947 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/howtos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/sources_plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/docs/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.2_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.3_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.4_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.5_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.6_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.7_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/skip_api_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.296596 earthkit_data-0.7.0/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/earthkit_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/conf/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/tab.css
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/tree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/global_grids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/gridspec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/gridspec_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47136 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21054 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/indexing/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/stdout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/mergers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/mirrors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mirrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mirrors/directory_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/bufr/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/covjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/geojson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/gridspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/grib/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.332597 earthkit_data-0.7.0/earthkit/data/readers/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/array_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ecmwf_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/fdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/numpy_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/virtual_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/wekeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/wekeocds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/generate_settings_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/module_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/xref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/module_inputs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/projections/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/proj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/grib-paramid.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/writers/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/earthkit_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 11:33:33.372597 earthkit_data-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/array_fieldlist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/array_fl_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fl_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/bufr/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_file_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/constants_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_contants_proc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.348597 earthkit_data-0.7.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.352597 earthkit_data-0.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2542596 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   640295 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.352597 earthkit_data-0.7.0/tests/data/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/constants/proc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/empty_file.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/era5_2t_1.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/era5_2t_2.nc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/data/gridspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/healpix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_rotated_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/regular_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/regular_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/rotated_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/rotated_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1308 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/hovexp_vert_area.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/mercator.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    47520 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/ml_data.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/rgg_small_subarea_cellarea_ref.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/t_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/t_time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_icon.grib
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single.nc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single_with_missing.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/time_series.covjson
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/u_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/v_pl.grib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/documentation/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/documentation/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/downstream-ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/environment-unit-tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/grib_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_file_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_inidces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_url_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/indexing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_isel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_order_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_selection_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/availability.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_aliases_grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/plugins/test_sources_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_covjson_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_geojson_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_grib_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_netcdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_odb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_reader_padding_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_shapefile_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_tar_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_unknown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_zip_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/unknown_file.unknown_ext
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/unknown_text_file.unknown_ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_fdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_polytope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_wekeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_wekeocds.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/translators/test_translators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_download_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_module_inputs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_projections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/tests/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_xarray.py
```

### Comparing `earthkit-data-0.6.0/.github/ci-hpc-config.yml` & `earthkit_data-0.7.0/.github/ci-hpc-config.yml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/.github/workflows/ci.yml` & `earthkit_data-0.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/.github/workflows/ci_other.yml` & `earthkit_data-0.7.0/.github/workflows/ci_other.yml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/.gitignore` & `earthkit_data-0.7.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
 docs/_build/
 docs/examples/*.tar
 docs/examples/*.zip
 docs/examples/_*
 docs/examples/earthkit_use_cases/*.grib
 docs/examples/_fdb
 docs/examples/*.db
+docs/examples/*.json
+docs/examples/*.geojson
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
```

### Comparing `earthkit-data-0.6.0/.pre-commit-config.yaml` & `earthkit_data-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/LICENSE` & `earthkit_data-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/Makefile` & `earthkit_data-0.7.0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 default: qa unit-tests type-check
 
 qa:
 	pre-commit run --all-files
 
 unit-tests:
-	python -m pytest -vv -m 'not notebook and not no_cache_init and not plugin' --cov=. --cov-report=$(COV_REPORT)
+	python -m pytest -vv -m 'not notebook and not no_cache_init' --cov=. --cov-report=$(COV_REPORT)
 	python -m pytest -v -m "notebook"
 	python -m pytest --forked -vv -m 'no_cache_init'
-	python -m pytest -v -m "plugin"
 
 # type-check:
 # 	python -m mypy .
 
 conda-env-update:
 	$(CONDA) env update $(CONDAFLAGS) -f environment.yml
```

### Comparing `earthkit-data-0.6.0/README.md` & `earthkit_data-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/Makefile` & `earthkit_data-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/_static/earthkit-data.png` & `earthkit_data-0.7.0/docs/_static/earthkit-data.png`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/_static/style.css` & `earthkit_data-0.7.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/api.rst` & `earthkit_data-0.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/conf.py` & `earthkit_data-0.7.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,19 @@
 html_static_path = ["_static"]
 html_css_files = ["style.css"]
 
 html_logo = "_static/earthkit-data.png"
 
 xref_links = {
     "cfgrib": ("cfgirb", "https://github.com/ecmwf/cfgrib"),
+    "earthkit": ("earthkit", "https://earthkit.readthedocs.io/en/latest/"),
+    "earthkit-geo": (
+        "earthkit-geo",
+        "https://earthkit-geo.readthedocs.io/en/latest/",
+    ),
     "earthkit-regrid": (
         "earthkit-regrid",
         "https://earthkit-regrid.readthedocs.io/en/latest/",
     ),
     "eccodes": (
         "ecCodes",
         "https://confluence.ecmwf.int/display/ECC/ecCodes+Home",
```

### Comparing `earthkit-data-0.6.0/docs/development.rst` & `earthkit_data-0.7.0/docs/development.rst`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,27 @@
 Run unit tests
 ---------------
 
 To run the test suite, you can use the following command:
 
 .. code-block:: shell
 
-    pytest
+    make unit-tests
+
+Please note this will not run any of the tests based on remote services e.g. :ref:`data-sources-mars`. These are disabled by default because they can take a very long time to complete or just hang. To enable all these tests you need to run:
+
+.. code-block:: shell
+
+    pytest -E long -v
+
+If just want to run e.g. the :ref:`data-sources-cds` tests you can use:
+
+.. code-block:: shell
+
+    pytest -E long -v -k cds
 
 
 Build documentation
 -------------------
 
 To build the documentation locally, please install the Python dependencies first:
```

### Comparing `earthkit-data-0.6.0/docs/examples/ads.ipynb` & `earthkit_data-0.7.0/docs/examples/ads.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'cells'": "{0: {'source': ['## Retrieving data from the ADS']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Retrieving CAMS data from the ADS"
+                "## Retrieving data from the ADS"
             ]
         },
         {
             "cell_type": "raw",
             "id": "fdb1ce5a-2f75-44e4-85fb-6bd47084cadd",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/bufr_synop.ipynb` & `earthkit_data-0.7.0/docs/examples/bufr_synop.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'cells'": "{0: {'source': ['## BUFR: using SYNOP data']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Using BUFR SYNOP data"
+                "## BUFR: using SYNOP data"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e11bb141-5f5d-42c2-9083-3cccbf9b7799",
             "metadata": {},
```

### Comparing `earthkit-data-0.6.0/docs/examples/bufr_temp.ipynb` & `earthkit_data-0.7.0/docs/examples/bufr_temp.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'cells'": "{0: {'source': ['## BUFR: using TEMP data']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Using BUFR TEMP data"
+                "## BUFR: using TEMP data"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e11bb141-5f5d-42c2-9083-3cccbf9b7799",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.6.0/docs/examples/cache.ipynb` & `earthkit_data-0.7.0/docs/examples/cache.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/cds.ipynb` & `earthkit_data-0.7.0/docs/examples/cds.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'cells'": "{0: {'source': ['## Retrieving data from the CDS']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Retrieving ERA5 data from the CDS"
+                "## Retrieving data from the CDS"
             ]
         },
         {
             "cell_type": "raw",
             "id": "589c568f-19c3-4a23-9e7a-37b0220bebfb",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/default_fdb_schema` & `earthkit_data-0.7.0/docs/examples/default_fdb_schema`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/demo_sources_plugin.ipynb` & `earthkit_data-0.7.0/docs/examples/demo_sources_plugin.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/ecmwf_open_data.ipynb` & `earthkit_data-0.7.0/docs/examples/ecmwf_open_data.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9869346013144842%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(3, '        step=[0, 24, 48]\\n'), (4, '       )')], "*

 * *            "delete: [3]}}, 4: {'outputs': {0: {'data': {'text/html': {insert: [(37, '      "*

 * *            "<td>20240306</td>\\n'), (38, '      <td>0</td>\\n'), (50, '      "*

 * *            "<td>20240306</td>\\n'), (51, '      <td>0</td>\\n'), (63, '      "*

 * *            "<td>20240306</td>\\n'), (64, '      <td>0</td>\\n'), (65, '      <td>24</td>\\n'), "*

 * *            "(76, '      <td>20240306</td>\\n'), (77, '      <td>0 […]*

```diff
@@ -51,15 +51,16 @@
             "id": "bcc2e1e1-a048-40c5-b830-b8aa601f97ac",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = earthkit.data.from_source(\"ecmwf-open-data\",  \n",
                 "        param=[\"t\", \"gh\"],\n",
                 "        levelist=\"500\",\n",
-                "        step=[0,6,12])"
+                "        step=[0, 24, 48]\n",
+                "       )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "e505cce0-917c-47bc-ae69-6a172382b069",
             "metadata": {},
@@ -100,98 +101,98 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>gh</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
-                            "      <td>6</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>24</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>gh</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
-                            "      <td>6</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>24</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
-                            "      <td>12</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>48</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>gh</td>\n",
                             "      <td>isobaricInhPa</td>\n",
                             "      <td>500</td>\n",
-                            "      <td>20230630</td>\n",
-                            "      <td>600</td>\n",
-                            "      <td>12</td>\n",
+                            "      <td>20240306</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>48</td>\n",
                             "      <td>fc</td>\n",
                             "      <td>None</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    500  20230630       600         0   \n",
-                            "1   ecmf        gh  isobaricInhPa    500  20230630       600         0   \n",
-                            "2   ecmf         t  isobaricInhPa    500  20230630       600         6   \n",
-                            "3   ecmf        gh  isobaricInhPa    500  20230630       600         6   \n",
-                            "4   ecmf         t  isobaricInhPa    500  20230630       600        12   \n",
-                            "5   ecmf        gh  isobaricInhPa    500  20230630       600        12   \n",
+                            "0   ecmf         t  isobaricInhPa    500  20240306         0         0   \n",
+                            "1   ecmf        gh  isobaricInhPa    500  20240306         0         0   \n",
+                            "2   ecmf         t  isobaricInhPa    500  20240306         0        24   \n",
+                            "3   ecmf        gh  isobaricInhPa    500  20240306         0        24   \n",
+                            "4   ecmf         t  isobaricInhPa    500  20240306         0        48   \n",
+                            "5   ecmf        gh  isobaricInhPa    500  20240306         0        48   \n",
                             "\n",
                             "  dataType number    gridType  \n",
                             "0       fc   None  regular_ll  \n",
                             "1       fc   None  regular_ll  \n",
                             "2       fc   None  regular_ll  \n",
                             "3       fc   None  regular_ll  \n",
                             "4       fc   None  regular_ll  \n",
@@ -206,25 +207,25 @@
             "source": [
                 "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1d489e50-8076-4fad-a090-0faffe64b7eb",
+            "id": "e59c45e5-fa81-42ee-9ec8-8d3908f5111e",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "dev_ecc",
             "language": "python",
-            "name": "dev"
+            "name": "dev_ecc"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `earthkit-data-0.6.0/docs/examples/fdb.ipynb` & `earthkit_data-0.7.0/docs/examples/fdb.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/from_object.ipynb` & `earthkit_data-0.7.0/docs/examples/from_object.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/grib_fdb_write.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_fdb_write.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988839285714286%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: writing data into FDB']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Writing GRIB data into FDB"
+                "## GRIB: writing data into FDB"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "behind-carry",
             "metadata": {
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_from_stream.ipynb` & `earthkit_data-0.7.0/docs/examples/data_from_stream.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995777027027026%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading data from a stream']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Reading GRIB from a stream"
+                "## Reading data from a stream"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "sticky-refrigerator",
             "metadata": {},
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_indexing.ipynb` & `earthkit_data-0.7.0/docs/examples/pandas.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888896372126437%*

 * *Differences: {"'cells'": "{0: {'source': ['## Using pandas data']}, 1: {'source': ['import pandas as pd\\n', "*

 * *            "'import geopandas as gpd\\n', 'import numpy as np\\n', '\\n', 'from earthkit.data "*

 * *            "import download_example_file, from_object, from_source']}, 2: {'source': ['Construct "*

 * *            "a sample pandas objects for demonstration']}, 3: {'execution_count': 2, 'outputs': "*

 * *            "[OrderedDict([('data', OrderedDict([('text/html', ['<div>\\n', '<style scoped>\\n', "*

 * *            "'    .d […]*

```diff
@@ -6,383 +6,40 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Using GRIB indexing "
+                "## Using pandas data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data"
+                "import pandas as pd\n",
+                "import geopandas as gpd\n",
+                "import numpy as np\n",
+                "\n",
+                "from earthkit.data import download_example_file, from_object, from_source"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First we prepare the data:"
+                "Construct a sample pandas objects for demonstration"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "earthkit.data.download_example_file([\"test.grib\", \"tuv_pl.grib\"])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "!test -d _grib_dir_with_sql || (mkdir -p _grib_dir_with_sql; cp -f test.grib tuv_pl.grib _grib_dir_with_sql/)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "### Indexing"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "We can perform indexing on the input GRIB data by using the **indexing** option in :ref:`from_source() <data-sources-file>`. The indexing is performed on first data access using the MARS ecCodes keys. The index-data is stored in a sqlite database, which is located in the earthkit-data cache. Subsequent loading of the same data is very fast because it will use the cached index-data."
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "Indexing only works when :ref:`caching <caching>` is enabled. We ensure a :ref:`user cache <user_cache_policy>` is used for this example and no settings are saved into the configuration file. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "from earthkit.data import settings\n",
-                "settings.auto_save_settings = False\n",
-                "settings.set(\"cache-policy\", \"user\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "fs = earthkit.data.from_source(\"file\", \"tuv_pl.grib\", indexing=True)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "18"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "len(fs)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Indexing works for a list of files or directories (here \"\\_grib_dir_with_sql\") is a directory:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "20"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "len(fs)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "### Methods using the SQL database"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "When calling :py:meth:`~data.readers.grib.index.GribFieldList.sel`, :py:meth:`~data.readers.grib.index.GribFieldList.isel` or :py:meth:`~data.readers.grib.index.GribFieldList.order_by` the metadata is directly read from the index database, so there is no need to load/open any of the GRIB messages."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "3"
-                        ]
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "a = fs.sel(level=500)\n",
-                "len(a)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 10,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "20"
-                        ]
-                    },
-                    "execution_count": 10,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "a = fs.order_by(\"param\")\n",
-                "len(a)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "3"
-                        ]
-                    },
-                    "execution_count": 11,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "a = fs.isel(level=2)\n",
-                "len(a)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "When keys not present in the index db are used the functions above do not work:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "try:\n",
-                "    a = fs.sel(gridType=\"regular_ll\")\n",
-                "except KeyError as e:\n",
-                "    print(f\"error: {e}\")   "
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "###\u00a0Methods not using the SQL database"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "Most of the other methods still need to load/open the GRIB messages to extract the required :py:meth:`~data.readers.grib.index.GribFieldList.metadata`. Ideally they should all use the index database. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 13,
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "GribField(u,1000,20180801,1200,0,0)\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print(fs[1])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['v', 't']"
-                        ]
-                    },
-                    "execution_count": 14,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "fs[2:4].metadata(\"param\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### from_source() arguments"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "source": [
-                "Selection and sorting arguments can be directly passed to :ref:`from_source() <data-sources-file>`:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 15,
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
@@ -404,98 +61,212 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>centre</th>\n",
-                            "      <th>shortName</th>\n",
-                            "      <th>typeOfLevel</th>\n",
-                            "      <th>level</th>\n",
-                            "      <th>dataDate</th>\n",
-                            "      <th>dataTime</th>\n",
-                            "      <th>stepRange</th>\n",
-                            "      <th>dataType</th>\n",
-                            "      <th>number</th>\n",
-                            "      <th>gridType</th>\n",
+                            "      <th>t2m</th>\n",
+                            "      <th>latitude</th>\n",
+                            "      <th>longitude</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>date</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>u</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>v</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <th>2022-01-01</th>\n",
+                            "      <td>273.150000</td>\n",
+                            "      <td>50.0</td>\n",
+                            "      <td>-1.000000e+00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-02</th>\n",
+                            "      <td>274.194737</td>\n",
+                            "      <td>50.1</td>\n",
+                            "      <td>-9.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-03</th>\n",
+                            "      <td>275.239474</td>\n",
+                            "      <td>50.2</td>\n",
+                            "      <td>-8.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-04</th>\n",
+                            "      <td>276.284211</td>\n",
+                            "      <td>50.3</td>\n",
+                            "      <td>-7.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-05</th>\n",
+                            "      <td>277.328947</td>\n",
+                            "      <td>50.4</td>\n",
+                            "      <td>-6.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-06</th>\n",
+                            "      <td>278.373684</td>\n",
+                            "      <td>50.5</td>\n",
+                            "      <td>-5.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-07</th>\n",
+                            "      <td>279.418421</td>\n",
+                            "      <td>50.6</td>\n",
+                            "      <td>-4.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-08</th>\n",
+                            "      <td>280.463158</td>\n",
+                            "      <td>50.7</td>\n",
+                            "      <td>-3.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-09</th>\n",
+                            "      <td>281.507895</td>\n",
+                            "      <td>50.8</td>\n",
+                            "      <td>-2.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-10</th>\n",
+                            "      <td>282.552632</td>\n",
+                            "      <td>50.9</td>\n",
+                            "      <td>-1.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-11</th>\n",
+                            "      <td>283.597368</td>\n",
+                            "      <td>51.0</td>\n",
+                            "      <td>-2.220446e-16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-12</th>\n",
+                            "      <td>284.642105</td>\n",
+                            "      <td>51.1</td>\n",
+                            "      <td>1.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-13</th>\n",
+                            "      <td>285.686842</td>\n",
+                            "      <td>51.2</td>\n",
+                            "      <td>2.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-14</th>\n",
+                            "      <td>286.731579</td>\n",
+                            "      <td>51.3</td>\n",
+                            "      <td>3.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-15</th>\n",
+                            "      <td>287.776316</td>\n",
+                            "      <td>51.4</td>\n",
+                            "      <td>4.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-16</th>\n",
+                            "      <td>288.821053</td>\n",
+                            "      <td>51.5</td>\n",
+                            "      <td>5.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-17</th>\n",
+                            "      <td>289.865789</td>\n",
+                            "      <td>51.6</td>\n",
+                            "      <td>6.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-18</th>\n",
+                            "      <td>290.910526</td>\n",
+                            "      <td>51.7</td>\n",
+                            "      <td>7.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-19</th>\n",
+                            "      <td>291.955263</td>\n",
+                            "      <td>51.8</td>\n",
+                            "      <td>8.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-20</th>\n",
+                            "      <td>293.000000</td>\n",
+                            "      <td>51.9</td>\n",
+                            "      <td>9.000000e-01</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "1   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
-                            "\n",
-                            "  dataType  number    gridType  \n",
-                            "0       an       0  regular_ll  \n",
-                            "1       an       0  regular_ll  \n",
-                            "2       an       0  regular_ll  "
+                            "                   t2m  latitude     longitude\n",
+                            "date                                          \n",
+                            "2022-01-01  273.150000      50.0 -1.000000e+00\n",
+                            "2022-01-02  274.194737      50.1 -9.000000e-01\n",
+                            "2022-01-03  275.239474      50.2 -8.000000e-01\n",
+                            "2022-01-04  276.284211      50.3 -7.000000e-01\n",
+                            "2022-01-05  277.328947      50.4 -6.000000e-01\n",
+                            "2022-01-06  278.373684      50.5 -5.000000e-01\n",
+                            "2022-01-07  279.418421      50.6 -4.000000e-01\n",
+                            "2022-01-08  280.463158      50.7 -3.000000e-01\n",
+                            "2022-01-09  281.507895      50.8 -2.000000e-01\n",
+                            "2022-01-10  282.552632      50.9 -1.000000e-01\n",
+                            "2022-01-11  283.597368      51.0 -2.220446e-16\n",
+                            "2022-01-12  284.642105      51.1  1.000000e-01\n",
+                            "2022-01-13  285.686842      51.2  2.000000e-01\n",
+                            "2022-01-14  286.731579      51.3  3.000000e-01\n",
+                            "2022-01-15  287.776316      51.4  4.000000e-01\n",
+                            "2022-01-16  288.821053      51.5  5.000000e-01\n",
+                            "2022-01-17  289.865789      51.6  6.000000e-01\n",
+                            "2022-01-18  290.910526      51.7  7.000000e-01\n",
+                            "2022-01-19  291.955263      51.8  8.000000e-01\n",
+                            "2022-01-20  293.000000      51.9  9.000000e-01"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True, level=500)\n",
-                "fs.ls()"
+                "t2m_series = pd.Series(np.linspace(273.15,293,20), name='t2m')\n",
+                "lat_series = pd.Series(np.arange(50,52,0.1), name='latitude')\n",
+                "lon_series = pd.Series(np.arange(-1,1,0.1), name='longitude')\n",
+                "date_series = pd.Series(pd.date_range('2022-01-01', '2022-01-20'), name='date')\n",
+                "\n",
+                "date_series\n",
+                "t2m_df = pd.concat([t2m_series, lat_series, lon_series], axis=1).set_index(date_series)\n",
+                "t2m_df"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Create an earthkit object from the pandas object, and use earthkit methods"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "t2m\n",
+                        "latitude\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -508,144 +279,203 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>centre</th>\n",
-                            "      <th>shortName</th>\n",
-                            "      <th>typeOfLevel</th>\n",
-                            "      <th>level</th>\n",
-                            "      <th>dataDate</th>\n",
-                            "      <th>dataTime</th>\n",
-                            "      <th>stepRange</th>\n",
-                            "      <th>dataType</th>\n",
-                            "      <th>number</th>\n",
-                            "      <th>gridType</th>\n",
+                            "      <th>t2m</th>\n",
+                            "      <th>latitude</th>\n",
+                            "      <th>longitude</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>date</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>u</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>u</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>v</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>v</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>an</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <th>2022-01-01</th>\n",
+                            "      <td>273.150000</td>\n",
+                            "      <td>50.0</td>\n",
+                            "      <td>-1.000000e+00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-02</th>\n",
+                            "      <td>274.194737</td>\n",
+                            "      <td>50.1</td>\n",
+                            "      <td>-9.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-03</th>\n",
+                            "      <td>275.239474</td>\n",
+                            "      <td>50.2</td>\n",
+                            "      <td>-8.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-04</th>\n",
+                            "      <td>276.284211</td>\n",
+                            "      <td>50.3</td>\n",
+                            "      <td>-7.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-05</th>\n",
+                            "      <td>277.328947</td>\n",
+                            "      <td>50.4</td>\n",
+                            "      <td>-6.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-06</th>\n",
+                            "      <td>278.373684</td>\n",
+                            "      <td>50.5</td>\n",
+                            "      <td>-5.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-07</th>\n",
+                            "      <td>279.418421</td>\n",
+                            "      <td>50.6</td>\n",
+                            "      <td>-4.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-08</th>\n",
+                            "      <td>280.463158</td>\n",
+                            "      <td>50.7</td>\n",
+                            "      <td>-3.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-09</th>\n",
+                            "      <td>281.507895</td>\n",
+                            "      <td>50.8</td>\n",
+                            "      <td>-2.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-10</th>\n",
+                            "      <td>282.552632</td>\n",
+                            "      <td>50.9</td>\n",
+                            "      <td>-1.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-11</th>\n",
+                            "      <td>283.597368</td>\n",
+                            "      <td>51.0</td>\n",
+                            "      <td>-2.220446e-16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-12</th>\n",
+                            "      <td>284.642105</td>\n",
+                            "      <td>51.1</td>\n",
+                            "      <td>1.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-13</th>\n",
+                            "      <td>285.686842</td>\n",
+                            "      <td>51.2</td>\n",
+                            "      <td>2.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-14</th>\n",
+                            "      <td>286.731579</td>\n",
+                            "      <td>51.3</td>\n",
+                            "      <td>3.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-15</th>\n",
+                            "      <td>287.776316</td>\n",
+                            "      <td>51.4</td>\n",
+                            "      <td>4.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-16</th>\n",
+                            "      <td>288.821053</td>\n",
+                            "      <td>51.5</td>\n",
+                            "      <td>5.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-17</th>\n",
+                            "      <td>289.865789</td>\n",
+                            "      <td>51.6</td>\n",
+                            "      <td>6.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-18</th>\n",
+                            "      <td>290.910526</td>\n",
+                            "      <td>51.7</td>\n",
+                            "      <td>7.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-19</th>\n",
+                            "      <td>291.955263</td>\n",
+                            "      <td>51.8</td>\n",
+                            "      <td>8.000000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-01-20</th>\n",
+                            "      <td>293.000000</td>\n",
+                            "      <td>51.9</td>\n",
+                            "      <td>9.000000e-01</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
-                            "3   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
-                            "4   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
-                            "5   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
-                            "\n",
-                            "  dataType  number    gridType  \n",
-                            "0       an       0  regular_ll  \n",
-                            "1       an       0  regular_ll  \n",
-                            "2       an       0  regular_ll  \n",
-                            "3       an       0  regular_ll  \n",
-                            "4       an       0  regular_ll  \n",
-                            "5       an       0  regular_ll  "
+                            "                   t2m  latitude     longitude\n",
+                            "date                                          \n",
+                            "2022-01-01  273.150000      50.0 -1.000000e+00\n",
+                            "2022-01-02  274.194737      50.1 -9.000000e-01\n",
+                            "2022-01-03  275.239474      50.2 -8.000000e-01\n",
+                            "2022-01-04  276.284211      50.3 -7.000000e-01\n",
+                            "2022-01-05  277.328947      50.4 -6.000000e-01\n",
+                            "2022-01-06  278.373684      50.5 -5.000000e-01\n",
+                            "2022-01-07  279.418421      50.6 -4.000000e-01\n",
+                            "2022-01-08  280.463158      50.7 -3.000000e-01\n",
+                            "2022-01-09  281.507895      50.8 -2.000000e-01\n",
+                            "2022-01-10  282.552632      50.9 -1.000000e-01\n",
+                            "2022-01-11  283.597368      51.0 -2.220446e-16\n",
+                            "2022-01-12  284.642105      51.1  1.000000e-01\n",
+                            "2022-01-13  285.686842      51.2  2.000000e-01\n",
+                            "2022-01-14  286.731579      51.3  3.000000e-01\n",
+                            "2022-01-15  287.776316      51.4  4.000000e-01\n",
+                            "2022-01-16  288.821053      51.5  5.000000e-01\n",
+                            "2022-01-17  289.865789      51.6  6.000000e-01\n",
+                            "2022-01-18  290.910526      51.7  7.000000e-01\n",
+                            "2022-01-19  291.955263      51.8  8.000000e-01\n",
+                            "2022-01-20  293.000000      51.9  9.000000e-01"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True, level=[500, 850], \n",
-                "                               order_by=\"variable\")\n",
-                "fs.ls()"
+                "ek_pandas = from_object(t2m_df)\n",
+                "# iterating behaves as a pandas DF\n",
+                "for thing in ek_pandas[:2]:\n",
+                "    print(thing)\n",
+                "\n",
+                "# Describe representation is a pandas dataframe\n",
+                "ek_pandas.describe()\n"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev_ecc",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "dev_ecc"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_lat_lon_value.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_lat_lon_value.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996603260869565%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: getting latitudes, longitudes and values']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Getting latitudes, longitudes and values from GRIB"
+                "## GRIB: getting latitudes, longitudes and values"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c74a86a6-79ae-44bc-a9c9-8cc8a3aaa484",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_metadata.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_metadata.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995471014492754%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: inspecting contents']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Inspecting GRIB contents"
+                "## GRIB: inspecting contents"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_missing.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_missing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: missing values']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## GRIB missing values"
+                "## GRIB: missing values"
             ]
         },
         {
             "attachments": {},
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_multi.ipynb` & `earthkit_data-0.7.0/docs/examples/multi_files.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990942028985508%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading multiple files']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Handling multiple GRIB files"
+                "## Reading multiple files"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "First we prepare the data."
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_nearest_gridpoint.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_nearest_gridpoint.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9885912698412698%*

 * *Differences: {"'cells'": "{0: {'source': ['### GRIB: nearest gridpoint']}, 2: {'source': {insert: [(1, 'from "*

 * *            "earthkit.geo import nearest_point_haversine, nearest_point_kdtree, GeoKDTree')], "*

 * *            "delete: [1]}}, 3: {'source': {insert: [(0, "*

 * *            '\'download_example_file("test.grib")\\n\')]}}}',*

 * * "'metadata'": "{'kernelspec': {'display_name': 'dev_ecc', 'name': 'dev_ecc'}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "### GRIB nearest gridpoint"
+                "### GRIB: nearest gridpoint"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ddb547b2-1d39-4c50-9777-19591bd0f6fa",
             "metadata": {},
             "source": [
@@ -26,24 +26,25 @@
             "cell_type": "code",
             "execution_count": 1,
             "id": "87e4f240-b145-4c4d-9906-38db9a7b3a99",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from earthkit.data import download_example_file, from_source\n",
-                "from earthkit.data.geo import nearest_point_haversine, nearest_point_kdtree, GeoKDTree"
+                "from earthkit.geo import nearest_point_haversine, nearest_point_kdtree, GeoKDTree"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "8ff42074-f9af-4f1b-a7c3-3d19ae54cf43",
             "metadata": {},
             "outputs": [],
             "source": [
+                "download_example_file(\"test.grib\")\n",
                 "ds = from_source(\"file\", \"test.grib\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c9a78d17-7f63-4944-ab3e-22349954e601",
             "metadata": {},
@@ -439,17 +440,17 @@
             "source": [
                 "### "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "dev_ecc",
             "language": "python",
-            "name": "dev"
+            "name": "dev_ecc"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_overview.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_overview.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995915032679739%*

 * *Differences: {"'cells'": "{0: {'source': ['## Using GRIB data']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Using GRIB data overview"
+                "## Using GRIB data"
             ]
         },
         {
             "attachments": {},
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_selection.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_selection.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995370370370371%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: selection using metadata']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## GRIB selection using metadata"
+                "## GRIB: selection using metadata"
             ]
         },
         {
             "attachments": {},
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_tar.ipynb` & `earthkit_data-0.7.0/docs/examples/tar_files.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976851851851851%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading tar or zip archive']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Reading GRIB in tar or zip archive"
+                "## Reading tar or zip archive"
             ]
         },
         {
             "attachments": {},
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_time_series.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_time_series.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9877314814814815%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: generating time series']}, 2: {'source': {insert: [(1, "*

 * *            "'from earthkit.geo import nearest_point_haversine')], delete: [1]}}, 3: {'source': "*

 * *            '{insert: [(0, \'download_example_file("time_series.grib")\\n\')]}}}',*

 * * "'metadata'": "{'kernelspec': {'display_name': 'dev_ecc', 'name': 'dev_ecc'}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "### Generating time series from GRIB"
+                "## GRIB: generating time series"
             ]
         },
         {
             "cell_type": "raw",
             "id": "5eb4fabf-b21e-4e10-b572-8095daaacd70",
             "metadata": {
                 "editable": true,
@@ -39,24 +39,25 @@
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from earthkit.data import download_example_file, from_source\n",
-                "from earthkit.data.geo import nearest_point_haversine"
+                "from earthkit.geo import nearest_point_haversine"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "8ff42074-f9af-4f1b-a7c3-3d19ae54cf43",
             "metadata": {},
             "outputs": [],
             "source": [
+                "download_example_file(\"time_series.grib\")\n",
                 "ds = from_source(\"file\", \"time_series.grib\").sel(param=\"t\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e35f59b4-586c-42b5-a24f-5a8c50db98aa",
             "metadata": {},
@@ -208,17 +209,17 @@
             "source": [
                 "### "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "dev_ecc",
             "language": "python",
-            "name": "dev"
+            "name": "dev_ecc"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_to_netcdf.ipynb` & `earthkit_data-0.7.0/docs/examples/grib_to_netcdf.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: converting to NetCDF']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Converting GRIB to NetCDF"
+                "## GRIB: converting to NetCDF"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "950b9aa8-6b76-47f8-b470-17476f99a733",
             "metadata": {},
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_url.ipynb` & `earthkit_data-0.7.0/docs/examples/url.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990808823529411%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading data from URLs']}}"}*

```diff
@@ -7,15 +7,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Getting GRIB data from URLs"
+                "## Reading data from URLs"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2c9d2ae0-aa05-4426-b8de-0d49495abee4",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.6.0/docs/examples/grib_url_stream.ipynb` & `earthkit_data-0.7.0/docs/examples/url_stream.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666667%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading data from URLs as a stream']}}"}*

```diff
@@ -8,15 +8,15 @@
                 "raw_mimetype": "",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## Reading GRIB from an URL as a stream"
+                "## Reading data from URLs as a stream"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "c23ffb07-747c-4535-b608-66b080d6d4e5",
             "metadata": {
```

### Comparing `earthkit-data-0.6.0/docs/examples/list_of_dict.ipynb` & `earthkit_data-0.7.0/docs/examples/list_of_dict.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/mars.ipynb` & `earthkit_data-0.7.0/docs/examples/mars.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/metadata.ipynb` & `earthkit_data-0.7.0/docs/examples/metadata.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/missing.grib` & `earthkit_data-0.7.0/docs/examples/missing.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/netcdf.ipynb` & `earthkit_data-0.7.0/docs/examples/netcdf.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/netcdf_fieldlist.ipynb` & `earthkit_data-0.7.0/docs/examples/netcdf_fieldlist.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995265151515151%*

 * *Differences: {"'cells'": "{0: {'source': ['## NetCDF: working with fieldlists']}}"}*

```diff
@@ -6,15 +6,15 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## NetCDF fieldlists"
+                "## NetCDF: working with fieldlists"
             ]
         },
         {
             "attachments": {},
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
```

### Comparing `earthkit-data-0.6.0/docs/examples/numpy_fieldlist.ipynb` & `earthkit_data-0.7.0/docs/examples/numpy_fieldlist.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969088753387534%*

 * *Differences: {"'cells'": "{0: {'source': ['## GRIB: create fieldlist from array and metadata']}, 1: {'source': "*

 * *            "{insert: [(0, 'In this notebook we will show how to do some computations with GRIB "*

 * *            'data and generate a :py:class:`~data.sources.numpy_list.ArrayFieldList` from the '*

 * *            "results.\\n')], delete: [0]}}, 13: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['<earthkit.data.readers.grib.metadata.GribMetadata at 0x1379bfe20>']}}}}, 16: "*

 * *            "{'source': ['A new Fi […]*

```diff
@@ -7,30 +7,30 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "## FieldList from numpy array and metadata"
+                "## GRIB: create fieldlist from array and metadata"
             ]
         },
         {
             "cell_type": "raw",
             "id": "a8eca176-b7fc-41d8-a1ac-e243c5f8070b",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "In this notebook we will show how to do some computations with GRIB data and generate a :py:class:`~data.sources.numpy_list.NumpyFieldList` from the results.\n",
+                "In this notebook we will show how to do some computations with GRIB data and generate a :py:class:`~data.sources.numpy_list.ArrayFieldList` from the results.\n",
                 "\n",
                 "First we :ref:`read <data-sources-file>` some GRIB data containing pressure level fields."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
@@ -224,15 +224,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<earthkit.data.readers.grib.metadata.GribMetadata at 0x10870bdf0>"
+                            "<earthkit.data.readers.grib.metadata.GribMetadata at 0x1379bfe20>"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -277,15 +277,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "A new FieldList (type of :py:class:`~data.sources.numpy_list.NumpyFieldList`) can be created from the resulting ndarray and the modified metadata. It behaves as if it were a :py:class:`~data.readers.grib.index.GribFieldList`."
+                "A new FieldList (type of :py:class:`~data.sources.numpy_list.ArrayFieldList`) can be created from the resulting ndarray and the modified metadata. It behaves as if it were a :py:class:`~data.readers.grib.index.GribFieldList`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "5a2557a6-091c-4345-a792-d3bfa7876c77",
             "metadata": {
@@ -357,28 +357,28 @@
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ds_new = FieldList.from_numpy(t_new, md_new)\n",
+                "ds_new = FieldList.from_array(t_new, md_new)\n",
                 "ds_new.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "2ccde1fc-f8c4-4d4d-abda-3ca3feebd02e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "NumpyField(pt,850,20180801,1200,0,0)"
+                            "ArrayField()"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -386,15 +386,21 @@
                 "ds_new[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "4113f204-dd96-422d-acb5-e2e0901cfb7a",
-            "metadata": {},
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([285.48786915, 285.48786915, 285.48786915, 285.48786915,\n",
                             "       285.48786915, 285.48786915, 285.48786915, 285.48786915,\n",
                             "       285.48786915, 285.48786915])"
@@ -438,15 +444,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We can save the :py:class:`~data.sources.numpy_list.NumpyFieldList` into a GRIB file:"
+                "We can save the :py:class:`~data.sources.numpy_list.ArrayFieldList` into a GRIB file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "c22a23fc-fccd-45ef-887e-95ab61b0dee1",
             "metadata": {
@@ -707,15 +713,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We create a :py:class:`~data.sources.numpy_list.NumpyFieldList` from the resulting ndarray and the modified metadata."
+                "We create a :py:class:`~data.sources.numpy_list.ArrayFieldList` from the resulting ndarray and the modified metadata."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "id": "ab0c805e-9e33-40f1-a816-501c2cff64a1",
             "metadata": {
@@ -818,15 +824,15 @@
                     "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "md_new = [f.metadata().override(shortName=\"pt\") for f in fs]\n",
-                "ds_new = FieldList.from_numpy(t_new, md_new)\n",
+                "ds_new = FieldList.from_array(t_new, md_new)\n",
                 "ds_new.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "id": "b0298472-345e-41f4-836e-a05b45509b2b",
@@ -878,15 +884,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We can save the :py:class:`~data.sources.numpy_list.NumpyFieldList` into a GRIB file:"
+                "We can save the :py:class:`~data.sources.numpy_list.ArrayFieldList` into a GRIB file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "id": "e8e1c8a2-87aa-4ec2-895e-8ea7bd83e101",
             "metadata": {
@@ -1041,15 +1047,15 @@
                 "\n",
                 "for f in fs:\n",
                 "    p = f.metadata(\"level\")*100. # hPa -> Pa\n",
                 "    t_new = potential_temperature(f.values, p)\n",
                 "    md_new = f.metadata().override(shortName=\"pt\")\n",
                 "    \n",
                 "    # create new numpy fieldlist with a single field\n",
-                "    ds_new = FieldList.from_numpy(t_new, md_new)\n",
+                "    ds_new = FieldList.from_array(t_new, md_new)\n",
                 "\n",
                 "    # add it to the resulting fieldlist\n",
                 "    ds_r += ds_new"
             ]
         },
         {
             "cell_type": "code",
@@ -1163,15 +1169,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We can save the :py:class:`~data.sources.numpy_list.NumpyFieldList` into a GRIB file:"
+                "We can save the :py:class:`~data.sources.numpy_list.ArrayFieldList` into a GRIB file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "id": "a149caa0-b1ba-4b8e-b2d0-6aad7ee224a6",
             "metadata": {},
```

### Comparing `earthkit-data-0.6.0/docs/examples/odb.ipynb` & `earthkit_data-0.7.0/docs/examples/odb.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/pandas.ipynb` & `earthkit_data-0.7.0/docs/examples/url_parts.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7874938133372911%*

 * *Differences: {"'cells'": "{0: {'source': ['## Reading data parts from URLs'], 'id': "*

 * *            "'7b42e29a-7d97-4b49-ab49-db2d73d79311'}, 1: {'execution_count': 1, 'metadata': "*

 * *            "{replace: OrderedDict([('editable', True), ('slideshow', OrderedDict([('slide_type', "*

 * *            "'')])), ('tags', [])])}, 'source': ['import earthkit.data'], 'id': "*

 * *            "'2beb1bac-4968-4f0a-aa1c-8fedbf234b0e'}, 5: {'source': ['### Single files'], 'id': "*

 * *            "'f348d7e7-d864-4e23-bb1b-adf6f1143c9c'}, 7: {'execut […]*

```diff
@@ -1,47 +1,73 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "7b42e29a-7d97-4b49-ab49-db2d73d79311",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "# Using pandas and geopandas data"
+                "## Reading data parts from URLs"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {},
+            "execution_count": 1,
+            "id": "2beb1bac-4968-4f0a-aa1c-8fedbf234b0e",
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "import pandas as pd\n",
-                "import geopandas as gpd\n",
-                "import numpy as np\n",
-                "\n",
-                "from earthkit.data import from_object, from_source\n",
-                "from earthkit.data.testing import earthkit_file"
+                "import earthkit.data"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
+            "cell_type": "raw",
+            "id": "a499dce2-5b62-4d7c-b994-ee2020c35468",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "source": [
-                "## Pandas\n",
-                "Construct a sample pandas objects for demonstration"
+                "This notebook demonstartes how to download only :ref:`parts <parts>` (byte ranges) from URLs."
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "id": "e9ccbcb7-a8d2-4e61-9055-1412cdc372ed",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
+            "source": [
+                "We download one of the files and inspect the contents with :py:meth:`~data.readers.grib.index.GribFieldList.ls`. By using the \"offset\" key we can get the byte positions where each message starts within the file. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 2,
+            "id": "27820099-8b9c-4c6c-9ee0-a72ef4224dac",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
@@ -63,209 +89,182 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>t2m</th>\n",
-                            "      <th>latitude</th>\n",
-                            "      <th>longitude</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>date</th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
+                            "      <th>offset</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-01</th>\n",
-                            "      <td>273.150000</td>\n",
-                            "      <td>50.0</td>\n",
-                            "      <td>-1.000000e+00</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-02</th>\n",
-                            "      <td>274.194737</td>\n",
-                            "      <td>50.1</td>\n",
-                            "      <td>-9.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-03</th>\n",
-                            "      <td>275.239474</td>\n",
-                            "      <td>50.2</td>\n",
-                            "      <td>-8.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-04</th>\n",
-                            "      <td>276.284211</td>\n",
-                            "      <td>50.3</td>\n",
-                            "      <td>-7.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-05</th>\n",
-                            "      <td>277.328947</td>\n",
-                            "      <td>50.4</td>\n",
-                            "      <td>-6.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-06</th>\n",
-                            "      <td>278.373684</td>\n",
-                            "      <td>50.5</td>\n",
-                            "      <td>-5.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-07</th>\n",
-                            "      <td>279.418421</td>\n",
-                            "      <td>50.6</td>\n",
-                            "      <td>-4.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-08</th>\n",
-                            "      <td>280.463158</td>\n",
-                            "      <td>50.7</td>\n",
-                            "      <td>-3.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-09</th>\n",
-                            "      <td>281.507895</td>\n",
-                            "      <td>50.8</td>\n",
-                            "      <td>-2.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-10</th>\n",
-                            "      <td>282.552632</td>\n",
-                            "      <td>50.9</td>\n",
-                            "      <td>-1.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-11</th>\n",
-                            "      <td>283.597368</td>\n",
-                            "      <td>51.0</td>\n",
-                            "      <td>-2.220446e-16</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-12</th>\n",
-                            "      <td>284.642105</td>\n",
-                            "      <td>51.1</td>\n",
-                            "      <td>1.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-13</th>\n",
-                            "      <td>285.686842</td>\n",
-                            "      <td>51.2</td>\n",
-                            "      <td>2.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-14</th>\n",
-                            "      <td>286.731579</td>\n",
-                            "      <td>51.3</td>\n",
-                            "      <td>3.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-15</th>\n",
-                            "      <td>287.776316</td>\n",
-                            "      <td>51.4</td>\n",
-                            "      <td>4.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-16</th>\n",
-                            "      <td>288.821053</td>\n",
-                            "      <td>51.5</td>\n",
-                            "      <td>5.000000e-01</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-17</th>\n",
-                            "      <td>289.865789</td>\n",
-                            "      <td>51.6</td>\n",
-                            "      <td>6.000000e-01</td>\n",
+                            "      <th>1</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>u</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>240.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-18</th>\n",
-                            "      <td>290.910526</td>\n",
-                            "      <td>51.7</td>\n",
-                            "      <td>7.000000e-01</td>\n",
+                            "      <th>2</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>480.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-19</th>\n",
-                            "      <td>291.955263</td>\n",
-                            "      <td>51.8</td>\n",
-                            "      <td>8.000000e-01</td>\n",
+                            "      <th>3</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>720.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-20</th>\n",
-                            "      <td>293.000000</td>\n",
-                            "      <td>51.9</td>\n",
-                            "      <td>9.000000e-01</td>\n",
+                            "      <th>4</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>u</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>960.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "      <td>1200.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                   t2m  latitude     longitude\n",
-                            "date                                          \n",
-                            "2022-01-01  273.150000      50.0 -1.000000e+00\n",
-                            "2022-01-02  274.194737      50.1 -9.000000e-01\n",
-                            "2022-01-03  275.239474      50.2 -8.000000e-01\n",
-                            "2022-01-04  276.284211      50.3 -7.000000e-01\n",
-                            "2022-01-05  277.328947      50.4 -6.000000e-01\n",
-                            "2022-01-06  278.373684      50.5 -5.000000e-01\n",
-                            "2022-01-07  279.418421      50.6 -4.000000e-01\n",
-                            "2022-01-08  280.463158      50.7 -3.000000e-01\n",
-                            "2022-01-09  281.507895      50.8 -2.000000e-01\n",
-                            "2022-01-10  282.552632      50.9 -1.000000e-01\n",
-                            "2022-01-11  283.597368      51.0 -2.220446e-16\n",
-                            "2022-01-12  284.642105      51.1  1.000000e-01\n",
-                            "2022-01-13  285.686842      51.2  2.000000e-01\n",
-                            "2022-01-14  286.731579      51.3  3.000000e-01\n",
-                            "2022-01-15  287.776316      51.4  4.000000e-01\n",
-                            "2022-01-16  288.821053      51.5  5.000000e-01\n",
-                            "2022-01-17  289.865789      51.6  6.000000e-01\n",
-                            "2022-01-18  290.910526      51.7  7.000000e-01\n",
-                            "2022-01-19  291.955263      51.8  8.000000e-01\n",
-                            "2022-01-20  293.000000      51.9  9.000000e-01"
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
+                            "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  offset  \n",
+                            "0       an       0  regular_ll     0.0  \n",
+                            "1       an       0  regular_ll   240.0  \n",
+                            "2       an       0  regular_ll   480.0  \n",
+                            "3       an       0  regular_ll   720.0  \n",
+                            "4       an       0  regular_ll   960.0  \n",
+                            "5       an       0  regular_ll  1200.0  "
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "t2m_series = pd.Series(np.linspace(273.15,293,20), name='t2m')\n",
-                "lat_series = pd.Series(np.arange(50,52,0.1), name='latitude')\n",
-                "lon_series = pd.Series(np.arange(-1,1,0.1), name='longitude')\n",
-                "date_series = pd.Series(pd.date_range('2022-01-01', '2022-01-20'), name='date')\n",
-                "\n",
-                "date_series\n",
-                "t2m_df = pd.concat([t2m_series, lat_series, lon_series], axis=1).set_index(date_series)\n",
-                "t2m_df"
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\")\n",
+                "ds.ls(extra_keys=\"offset\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f348d7e7-d864-4e23-bb1b-adf6f1143c9c",
             "metadata": {},
             "source": [
-                "Create an earthkit object from the pandas object, and use earthkit methods"
+                "### Single files"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "id": "e8346eb4-804f-4093-bda8-80acec9873ae",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
+            "source": [
+                "The **parts** option in :ref:`from_source() <data-sources-url>` specifies the **byte range(s)** we want to read from a remote file. A single :ref:`part <parts>` is a tuple or list in the following format: *(offset, length)*. \n",
+                "\n",
+                "Using the offsets from the example above we can specify the :ref:`part <parts>` for the fist message."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 3,
+            "id": "5a048a9f-7ea2-4613-997f-4d7464a7db98",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "t2m\n",
-                        "latitude\n"
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -281,233 +280,290 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>t2m</th>\n",
-                            "      <th>latitude</th>\n",
-                            "      <th>longitude</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>date</th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-01</th>\n",
-                            "      <td>273.150000</td>\n",
-                            "      <td>50.0</td>\n",
-                            "      <td>-1.000000e+00</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-02</th>\n",
-                            "      <td>274.194737</td>\n",
-                            "      <td>50.1</td>\n",
-                            "      <td>-9.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-03</th>\n",
-                            "      <td>275.239474</td>\n",
-                            "      <td>50.2</td>\n",
-                            "      <td>-8.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-04</th>\n",
-                            "      <td>276.284211</td>\n",
-                            "      <td>50.3</td>\n",
-                            "      <td>-7.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-05</th>\n",
-                            "      <td>277.328947</td>\n",
-                            "      <td>50.4</td>\n",
-                            "      <td>-6.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-06</th>\n",
-                            "      <td>278.373684</td>\n",
-                            "      <td>50.5</td>\n",
-                            "      <td>-5.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-07</th>\n",
-                            "      <td>279.418421</td>\n",
-                            "      <td>50.6</td>\n",
-                            "      <td>-4.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-08</th>\n",
-                            "      <td>280.463158</td>\n",
-                            "      <td>50.7</td>\n",
-                            "      <td>-3.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-09</th>\n",
-                            "      <td>281.507895</td>\n",
-                            "      <td>50.8</td>\n",
-                            "      <td>-2.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-10</th>\n",
-                            "      <td>282.552632</td>\n",
-                            "      <td>50.9</td>\n",
-                            "      <td>-1.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-11</th>\n",
-                            "      <td>283.597368</td>\n",
-                            "      <td>51.0</td>\n",
-                            "      <td>-2.220446e-16</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-12</th>\n",
-                            "      <td>284.642105</td>\n",
-                            "      <td>51.1</td>\n",
-                            "      <td>1.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-13</th>\n",
-                            "      <td>285.686842</td>\n",
-                            "      <td>51.2</td>\n",
-                            "      <td>2.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-14</th>\n",
-                            "      <td>286.731579</td>\n",
-                            "      <td>51.3</td>\n",
-                            "      <td>3.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-15</th>\n",
-                            "      <td>287.776316</td>\n",
-                            "      <td>51.4</td>\n",
-                            "      <td>4.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-16</th>\n",
-                            "      <td>288.821053</td>\n",
-                            "      <td>51.5</td>\n",
-                            "      <td>5.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-17</th>\n",
-                            "      <td>289.865789</td>\n",
-                            "      <td>51.6</td>\n",
-                            "      <td>6.000000e-01</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-18</th>\n",
-                            "      <td>290.910526</td>\n",
-                            "      <td>51.7</td>\n",
-                            "      <td>7.000000e-01</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-01-19</th>\n",
-                            "      <td>291.955263</td>\n",
-                            "      <td>51.8</td>\n",
-                            "      <td>8.000000e-01</td>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  "
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "        parts=(0, 240))\n",
+                "ds.ls()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b40e2a4d-d000-4a3f-b756-0c8780e6bf09",
+            "metadata": {},
+            "source": [
+                "The call above can also be written as:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "661e7ebb-13f7-4db6-8e87-ee59848c47b2",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
                             "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2022-01-20</th>\n",
-                            "      <td>293.000000</td>\n",
-                            "      <td>51.9</td>\n",
-                            "      <td>9.000000e-01</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                   t2m  latitude     longitude\n",
-                            "date                                          \n",
-                            "2022-01-01  273.150000      50.0 -1.000000e+00\n",
-                            "2022-01-02  274.194737      50.1 -9.000000e-01\n",
-                            "2022-01-03  275.239474      50.2 -8.000000e-01\n",
-                            "2022-01-04  276.284211      50.3 -7.000000e-01\n",
-                            "2022-01-05  277.328947      50.4 -6.000000e-01\n",
-                            "2022-01-06  278.373684      50.5 -5.000000e-01\n",
-                            "2022-01-07  279.418421      50.6 -4.000000e-01\n",
-                            "2022-01-08  280.463158      50.7 -3.000000e-01\n",
-                            "2022-01-09  281.507895      50.8 -2.000000e-01\n",
-                            "2022-01-10  282.552632      50.9 -1.000000e-01\n",
-                            "2022-01-11  283.597368      51.0 -2.220446e-16\n",
-                            "2022-01-12  284.642105      51.1  1.000000e-01\n",
-                            "2022-01-13  285.686842      51.2  2.000000e-01\n",
-                            "2022-01-14  286.731579      51.3  3.000000e-01\n",
-                            "2022-01-15  287.776316      51.4  4.000000e-01\n",
-                            "2022-01-16  288.821053      51.5  5.000000e-01\n",
-                            "2022-01-17  289.865789      51.6  6.000000e-01\n",
-                            "2022-01-18  290.910526      51.7  7.000000e-01\n",
-                            "2022-01-19  291.955263      51.8  8.000000e-01\n",
-                            "2022-01-20  293.000000      51.9  9.000000e-01"
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ek_pandas = from_object(t2m_df)\n",
-                "# iterating behaves as a pandas DF\n",
-                "for thing in ek_pandas[:2]:\n",
-                "    print(thing)\n",
-                "\n",
-                "# Describe representation is a pandas dataframe\n",
-                "ek_pandas.describe()\n"
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "        parts=[(0, 240)])\n",
+                "ds.ls()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
+            "id": "5c8001e3-5413-4c8f-ac4e-ff3a7d168a43",
+            "metadata": {},
+            "source": [
+                "A part can go over a message boundary. Here bytes 240-244 belong to the second message, which is not read because not all of its bytes are specified."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "cdbd5356-8696-4e73-9d1d-1996667f1792",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
+                    ]
                 },
-                "tags": []
-            },
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  "
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "## Geopandas"
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "        parts=[(0, 245)])\n",
+                "ds.ls()"
             ]
         },
         {
             "cell_type": "raw",
+            "id": "d2c2aa43-802c-4739-b7da-92c5fc22b7b2",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "Load a geojson object as a \"file\" source using :ref:`from_source() <data-sources-file>`. Default representation is a geopandas dataframe"
+                "Multiple :ref:`parts <parts>` can be used."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 6,
+            "id": "53c60306-ff16-40ce-9922-6552bab3244f",
             "metadata": {
                 "editable": true,
+                "scrolled": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
-                            "<h3>GeojsonReader(represented as a geopandas object):</h3><div>\n",
+                            "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
                             "\n",
                             "    .dataframe tbody tr th {\n",
                             "        vertical-align: top;\n",
@@ -517,264 +573,171 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>id</th>\n",
-                            "      <th>NUTS_ID</th>\n",
-                            "      <th>LEVL_CODE</th>\n",
-                            "      <th>CNTR_CODE</th>\n",
-                            "      <th>NAME_LATN</th>\n",
-                            "      <th>NUTS_NAME</th>\n",
-                            "      <th>MOUNT_TYPE</th>\n",
-                            "      <th>URBN_TYPE</th>\n",
-                            "      <th>COAST_TYPE</th>\n",
-                            "      <th>FID</th>\n",
-                            "      <th>geometry</th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>FR</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>France</td>\n",
-                            "      <td>France</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>MULTIPOLYGON (((9954236.116 -3059379.316, 9961...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>Hrvatska</td>\n",
-                            "      <td>Hrvatska</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>MULTIPOLYGON (((4827385.889 2618351.326, 48483...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>Magyarorsz\u00e1g</td>\n",
-                            "      <td>Magyarorsz\u00e1g</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>POLYGON ((5214660.069 2880853.832, 5216710.220...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>Shqip\u00ebria</td>\n",
-                            "      <td>Shqip\u00ebria</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>POLYGON ((5129579.170 2204098.752, 5148385.473...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>\u00d6sterreich</td>\n",
-                            "      <td>\u00d6sterreich</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>POLYGON ((4742889.368 2876362.725, 4783217.798...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2005</th>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TR</td>\n",
-                            "      <td>\u015eanl\u0131urfa</td>\n",
-                            "      <td>\u015eanl\u0131urfa</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>POLYGON ((6904684.585 2120354.802, 6938677.828...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2006</th>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TR</td>\n",
-                            "      <td>Diyarbak\u0131r</td>\n",
-                            "      <td>Diyarbak\u0131r</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>POLYGON ((6989716.599 2273670.524, 6982786.486...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2007</th>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Svalbard</td>\n",
-                            "      <td>Svalbard</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>MULTIPOLYGON (((4754167.335 6382461.409, 47465...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2008</th>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Jan Mayen and Svalbard</td>\n",
-                            "      <td>Jan Mayen and Svalbard</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>MULTIPOLYGON (((4754167.335 6382461.409, 47465...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2009</th>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Jan Mayen</td>\n",
-                            "      <td>Jan Mayen</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>POLYGON ((3642785.362 5404637.884, 3624291.510...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>2010 rows \u00d7 11 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "GeojsonReader(/Users/edwardcomyn-platt/Work/Git_Repositories/EARTHKIT/earthkit-data/tests/data/NUTS_RG_20M_2021_3035.geojson)"
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "1   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  \n",
+                            "2       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Test the geojson reader\n",
-                "geojson_source = from_source(\"file\", earthkit_file(\"tests/data/NUTS_RG_20M_2021_3035.geojson\"))\n",
-                "geojson_source"
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "        parts=[(0, 240), (480, 480)])\n",
+                "ds.ls()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a9b26883-6f17-4933-90ad-d2342ac1a26b",
             "metadata": {},
             "source": [
-                "Iterating over geojson/geopandas objects iterates over rows (feature) instead of the pandas default (columns).\n",
-                "This is more useful for geopandas."
+                "Parts cannot overlap."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "metadata": {},
+            "execution_count": 7,
+            "id": "01e41b9b-6900-4057-bbe8-958ba2b021bf",
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "id                                                           FR\n",
-                        "NUTS_ID                                                      FR\n",
-                        "LEVL_CODE                                                     0\n",
-                        "CNTR_CODE                                                    FR\n",
-                        "NAME_LATN                                                France\n",
-                        "NUTS_NAME                                                France\n",
-                        "MOUNT_TYPE                                                  0.0\n",
-                        "URBN_TYPE                                                     0\n",
-                        "COAST_TYPE                                                    0\n",
-                        "FID                                                          FR\n",
-                        "geometry      MULTIPOLYGON (((9954236.1162 -3059379.3164, 99...\n",
-                        "Name: 0, dtype: object\n",
-                        "id                                                           HR\n",
-                        "NUTS_ID                                                      HR\n",
-                        "LEVL_CODE                                                     0\n",
-                        "CNTR_CODE                                                    HR\n",
-                        "NAME_LATN                                              Hrvatska\n",
-                        "NUTS_NAME                                              Hrvatska\n",
-                        "MOUNT_TYPE                                                  0.0\n",
-                        "URBN_TYPE                                                     0\n",
-                        "COAST_TYPE                                                    0\n",
-                        "FID                                                          HR\n",
-                        "geometry      MULTIPOLYGON (((4827385.8894 2618351.326199999...\n",
-                        "Name: 1, dtype: object\n"
+                        "Offsets and lengths must be in order, and not overlapping: offset=220, end of previous part=240\n"
                     ]
                 }
             ],
             "source": [
-                "for thing in geojson_source[:2]:\n",
-                "    print(thing)"
+                "try:\n",
+                "    ds = earthkit.data.from_source(\n",
+                "            \"url\", \n",
+                "            \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "             parts=[(0, 240), (220, 240)])\n",
+                "except Exception as e:\n",
+                "    print(e)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f090b522-b8dc-4d54-8b49-3ea2a78ed16f",
             "metadata": {},
             "source": [
-                "It is also possible to create an earthkit-data object from an already instantiated geopandas dataframe"
+                "### Multiple files"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "id": "28957198-65d5-480d-809d-26a1aac27a30",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
+            "source": [
+                "When using multiple URLs we can specify the :ref:`part <parts>` for each file with the following syntax:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 8,
+            "id": "4b1a35fe-db43-4e33-b00e-f55c5c2332d1",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib does not support byte ranges, downloading whole file\n",
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -787,300 +750,364 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>id</th>\n",
-                            "      <th>NUTS_ID</th>\n",
-                            "      <th>LEVL_CODE</th>\n",
-                            "      <th>CNTR_CODE</th>\n",
-                            "      <th>NAME_LATN</th>\n",
-                            "      <th>NUTS_NAME</th>\n",
-                            "      <th>MOUNT_TYPE</th>\n",
-                            "      <th>URBN_TYPE</th>\n",
-                            "      <th>COAST_TYPE</th>\n",
-                            "      <th>FID</th>\n",
-                            "      <th>geometry</th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>FR</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>France</td>\n",
-                            "      <td>France</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>20200513</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>FR</td>\n",
-                            "      <td>MULTIPOLYGON (((9954236.116 -3059379.316, 9961...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>Hrvatska</td>\n",
-                            "      <td>Hrvatska</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>HR</td>\n",
-                            "      <td>MULTIPOLYGON (((4827385.889 2618351.326, 48483...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>Magyarorsz\u00e1g</td>\n",
-                            "      <td>Magyarorsz\u00e1g</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>HU</td>\n",
-                            "      <td>POLYGON ((5214660.069 2880853.832, 5216710.220...</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf        2t        surface      0  20200513      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  \n",
+                            "2       an       0  regular_ll  "
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "ds = earthkit.data.from_source(\"url\", [\n",
+                "                               [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\", (0,526)], \n",
+                "                               [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\", [(0, 240), (480, 240)]]\n",
+                "                              ])\n",
+                "ds.ls()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b77c770f-0f3c-48f4-afe4-bcac35d424a0",
+            "metadata": {},
+            "source": [
+                "When a part is None for a given file the whole file will be used."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "ba09e8ea-19c1-4763-b603-acedad380ed5",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
                             "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>AL</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>Shqip\u00ebria</td>\n",
-                            "      <td>Shqip\u00ebria</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>20200513</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>AL</td>\n",
-                            "      <td>POLYGON ((5129579.170 2204098.752, 5148385.473...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>AT</td>\n",
+                            "      <th>1</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>msl</td>\n",
+                            "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>\u00d6sterreich</td>\n",
-                            "      <td>\u00d6sterreich</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>20200513</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>AT</td>\n",
-                            "      <td>POLYGON ((4742889.368 2876362.725, 4783217.798...</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2005</th>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TR</td>\n",
-                            "      <td>\u015eanl\u0131urfa</td>\n",
-                            "      <td>\u015eanl\u0131urfa</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TRC21</td>\n",
-                            "      <td>POLYGON ((6904684.585 2120354.802, 6938677.828...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2006</th>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TR</td>\n",
-                            "      <td>Diyarbak\u0131r</td>\n",
-                            "      <td>Diyarbak\u0131r</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>TRC22</td>\n",
-                            "      <td>POLYGON ((6989716.599 2273670.524, 6982786.486...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2007</th>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Svalbard</td>\n",
-                            "      <td>Svalbard</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>NO0B2</td>\n",
-                            "      <td>MULTIPOLYGON (((4754167.335 6382461.409, 47465...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2008</th>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Jan Mayen and Svalbard</td>\n",
-                            "      <td>Jan Mayen and Svalbard</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>NO0B</td>\n",
-                            "      <td>MULTIPOLYGON (((4754167.335 6382461.409, 47465...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2009</th>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>NO</td>\n",
-                            "      <td>Jan Mayen</td>\n",
-                            "      <td>Jan Mayen</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>NO0B1</td>\n",
-                            "      <td>POLYGON ((3642785.362 5404637.884, 3624291.510...</td>\n",
+                            "      <th>3</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>2010 rows \u00d7 11 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "         id NUTS_ID  LEVL_CODE CNTR_CODE               NAME_LATN  \\\n",
-                            "0        FR      FR          0        FR                  France   \n",
-                            "1        HR      HR          0        HR                Hrvatska   \n",
-                            "2        HU      HU          0        HU            Magyarorsz\u00e1g   \n",
-                            "3        AL      AL          0        AL               Shqip\u00ebria   \n",
-                            "4        AT      AT          0        AT              \u00d6sterreich   \n",
-                            "...     ...     ...        ...       ...                     ...   \n",
-                            "2005  TRC21   TRC21          3        TR               \u015eanl\u0131urfa   \n",
-                            "2006  TRC22   TRC22          3        TR              Diyarbak\u0131r   \n",
-                            "2007  NO0B2   NO0B2          3        NO                Svalbard   \n",
-                            "2008   NO0B    NO0B          2        NO  Jan Mayen and Svalbard   \n",
-                            "2009  NO0B1   NO0B1          3        NO               Jan Mayen   \n",
-                            "\n",
-                            "                   NUTS_NAME  MOUNT_TYPE  URBN_TYPE  COAST_TYPE    FID  \\\n",
-                            "0                     France         0.0          0           0     FR   \n",
-                            "1                   Hrvatska         0.0          0           0     HR   \n",
-                            "2               Magyarorsz\u00e1g         0.0          0           0     HU   \n",
-                            "3                  Shqip\u00ebria         0.0          0           0     AL   \n",
-                            "4                 \u00d6sterreich         0.0          0           0     AT   \n",
-                            "...                      ...         ...        ...         ...    ...   \n",
-                            "2005               \u015eanl\u0131urfa         4.0          2           3  TRC21   \n",
-                            "2006              Diyarbak\u0131r         4.0          2           3  TRC22   \n",
-                            "2007                Svalbard         3.0          3           1  NO0B2   \n",
-                            "2008  Jan Mayen and Svalbard         NaN          0           0   NO0B   \n",
-                            "2009               Jan Mayen         3.0          3           1  NO0B1   \n",
-                            "\n",
-                            "                                               geometry  \n",
-                            "0     MULTIPOLYGON (((9954236.116 -3059379.316, 9961...  \n",
-                            "1     MULTIPOLYGON (((4827385.889 2618351.326, 48483...  \n",
-                            "2     POLYGON ((5214660.069 2880853.832, 5216710.220...  \n",
-                            "3     POLYGON ((5129579.170 2204098.752, 5148385.473...  \n",
-                            "4     POLYGON ((4742889.368 2876362.725, 4783217.798...  \n",
-                            "...                                                 ...  \n",
-                            "2005  POLYGON ((6904684.585 2120354.802, 6938677.828...  \n",
-                            "2006  POLYGON ((6989716.599 2273670.524, 6982786.486...  \n",
-                            "2007  MULTIPOLYGON (((4754167.335 6382461.409, 47465...  \n",
-                            "2008  MULTIPOLYGON (((4754167.335 6382461.409, 47465...  \n",
-                            "2009  POLYGON ((3642785.362 5404637.884, 3624291.510...  \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf        2t        surface      0  20200513      1200         0   \n",
+                            "1   ecmf       msl        surface      0  20200513      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "3   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
-                            "[2010 rows x 11 columns]"
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  \n",
+                            "2       an       0  regular_ll  \n",
+                            "3       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "gpd_df = gpd.read_file(geojson_source.path)\n",
-                "ek_gpd_df = from_object(gpd_df)\n",
-                "ek_gpd_df.describe()"
+                "ds = earthkit.data.from_source(\n",
+                "    \"url\", [\n",
+                "        [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\", None], \n",
+                "        [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\", [(0,240), (480, 240)]]\n",
+                "        ])\n",
+                "ds.ls()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "77361bdd-5294-4a0b-8b9e-0a283483ff80",
+            "metadata": {},
+            "source": [
+                "The **parts** kwarg can still be used for multiple files; in this case it will be applied to each of them one by one."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 10,
+            "id": "007d715f-291a-4f17-b252-7cf717ad7426",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Number of polygons in geopandas: 2010\n",
-                        "Iterate of polygons:\n",
-                        "id                                                           FR\n",
-                        "NUTS_ID                                                      FR\n",
-                        "LEVL_CODE                                                     0\n",
-                        "CNTR_CODE                                                    FR\n",
-                        "NAME_LATN                                                France\n",
-                        "NUTS_NAME                                                France\n",
-                        "MOUNT_TYPE                                                  0.0\n",
-                        "URBN_TYPE                                                     0\n",
-                        "COAST_TYPE                                                    0\n",
-                        "FID                                                          FR\n",
-                        "geometry      MULTIPOLYGON (((9954236.1162 -3059379.3164, 99...\n",
-                        "Name: 0, dtype: object\n",
-                        "id                                                           HR\n",
-                        "NUTS_ID                                                      HR\n",
-                        "LEVL_CODE                                                     0\n",
-                        "CNTR_CODE                                                    HR\n",
-                        "NAME_LATN                                              Hrvatska\n",
-                        "NUTS_NAME                                              Hrvatska\n",
-                        "MOUNT_TYPE                                                  0.0\n",
-                        "URBN_TYPE                                                     0\n",
-                        "COAST_TYPE                                                    0\n",
-                        "FID                                                          HR\n",
-                        "geometry      MULTIPOLYGON (((4827385.8894 2618351.326199999...\n",
-                        "Name: 1, dtype: object\n"
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib does not support byte ranges, downloading whole file\n",
+                        "Server for https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib does not support byte ranges, downloading whole file\n"
                     ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  "
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "print(f\"Number of polygons in geopandas: {len(ek_gpd_df)}\")\n",
-                "\n",
-                "print(\"Iterate of polygons:\")\n",
-                "for thing in ek_gpd_df[:2]:\n",
-                "    print(thing)"
+                "ds = earthkit.data.from_source(\n",
+                "        \"url\", \n",
+                "        [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib\",\n",
+                "         \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib\"], \n",
+                "        parts=(0,240))\n",
+                "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "id": "53be8b67-8260-456b-bc58-12aa4a3380d3",
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "dev_ecc",
             "language": "python",
-            "name": "python3"
+            "name": "dev_ecc"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
@@ -1088,9 +1115,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.13"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `earthkit-data-0.6.0/docs/examples/polytope.ipynb` & `earthkit_data-0.7.0/docs/examples/polytope.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/projection.ipynb` & `earthkit_data-0.7.0/docs/examples/projection.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/settings.ipynb` & `earthkit_data-0.7.0/docs/examples/settings.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/synop_10.bufr` & `earthkit_data-0.7.0/docs/examples/synop_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/temp_10.bufr` & `earthkit_data-0.7.0/docs/examples/temp_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/test.grib` & `earthkit_data-0.7.0/docs/examples/test.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/test.nc` & `earthkit_data-0.7.0/docs/examples/test.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/test.odb` & `earthkit_data-0.7.0/docs/examples/test.odb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/test4.grib` & `earthkit_data-0.7.0/docs/examples/test4.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/test6.grib` & `earthkit_data-0.7.0/docs/examples/test6.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/time_series.grib` & `earthkit_data-0.7.0/docs/examples/time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/tuv_pl.grib` & `earthkit_data-0.7.0/docs/examples/tuv_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/tuv_pl.nc` & `earthkit_data-0.7.0/docs/examples/tuv_pl.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/examples/wekeo.ipynb` & `earthkit_data-0.7.0/docs/examples/wekeo.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/caching.rst` & `earthkit_data-0.7.0/docs/guide/caching.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/data.rst` & `earthkit_data-0.7.0/docs/guide/data.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/data_format/bufr.rst` & `earthkit_data-0.7.0/docs/guide/data_format/bufr.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/data_format/grib.rst` & `earthkit_data-0.7.0/docs/guide/data_format/grib.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/include/settings-set.py` & `earthkit_data-0.7.0/docs/guide/include/settings-set.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/settings.rst` & `earthkit_data-0.7.0/docs/guide/settings.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/guide/sources.rst` & `earthkit_data-0.7.0/docs/guide/sources.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,53 +28,61 @@
       - read data from a file/files
     * - :ref:`data-sources-file-pattern`
       - read data from a list of files  created from a pattern
     * - :ref:`data-sources-url`
       - read data from a URL
     * - :ref:`data-sources-url-pattern`
       - read data from a list of URLs created from a pattern
+    * - :ref:`data-sources-sample`
+      - read example data
     * - :ref:`data-sources-stream`
       - read data from a stream
     * - :ref:`data-sources-memory`
       - read data from a memory buffer
+    * - :ref:`data-sources-multi`
+      - read data from multiple sources
     * - :ref:`data-sources-ads`
       - retrieve data from the `Copernicus Atmosphere Data Store <https://ads.atmosphere.copernicus.eu/>`_ (ADS)
     * - :ref:`data-sources-cds`
       - retrieve data from the `Copernicus Climate Data Store <https://cds.climate.copernicus.eu/>`_ (CDS)
     * - :ref:`data-sources-eod`
       - retrieve `ECMWF open data <https://www.ecmwf.int/en/forecasts/datasets/open-data>`_
     * - :ref:`data-sources-fdb`
       - retrieve data from the `Fields DataBase <https://fields-database.readthedocs.io/en/latest/>`_ (FDB)
     * - :ref:`data-sources-mars`
       - retrieve data from the ECMWF `MARS archive <https://confluence.ecmwf.int/display/UDOC/MARS+user+documentation>`_
+    * - :ref:`data-sources-opendap`
+      - retrieve NetCDF data from `OPEnDAP <https://en.wikipedia.org/wiki/OPeNDAP>`_ services
     * - :ref:`data-sources-polytope`
       - retrieve data from the `Polytope services <https://polytope-client.readthedocs.io/en/latest/>`_
     * - :ref:`data-sources-wekeo`
       - retrieve data from `WEkEO`_ using the WEkEO grammar
     * - :ref:`data-sources-wekeocds`
       - retrieve `CDS <https://cds.climate.copernicus.eu/>`_ data stored on `WEkEO`_ using the `cdsapi`_ grammar
 
 ----------------------------------
 
 .. _data-sources-file:
 
 file
 ----
 
-.. py:function:: from_source("file", path, expand_user=True, expand_vars=False, unix_glob=True, recursive_glob=True)
+.. py:function:: from_source("file", path, expand_user=True, expand_vars=False, unix_glob=True, recursive_glob=True, parts=None)
   :noindex:
 
-  The simplest source is ``file`` that can access a local file/list of files.
+  The simplest source is ``file``, which can access a local file/list of files.
 
-  :param path: input path(s)
-  :type path: str, list
+  :param path: input path(s). Each path can contain the :ref:`parts <parts>` defining the byte ranges to read.
+  :type path: str, list, tuple
   :param bool expand_user: replace the leading ~ or ~user in ``path`` by that user's home directory. See ``os.path.expanduser``
   :param bool expand_vars:  expand shell environment variables in ``path``. See ``os.path.expandpath``
   :param bool unix_glob: allow UNIX globbing in ``path``
   :param bool recursive_glob: allow recursive scanning of directories. Only used when ``uxix_glob`` is True
+  :param parts: the :ref:`parts <parts>` to read from the file(s) specified by ``path``. Cannot be used when ``path`` already defines the :ref:`parts <parts>`.
+  :type parts: pair, list or tuple of pairs, None
 
   *earthkit-data* will inspect the content of the files to check for any of the
   supported :ref:`data formats <data-format>`.
 
   When the input is an archive format such as ``.zip``, ``.tar``, ``.tar.gz``, etc,
   *earthkit-data* will attempt to open it and extract any usable files, which are then stored in the :ref:`cache <caching>`.
 
@@ -90,18 +98,43 @@
       # list of files can be specified
       ds = earthkit.data.from_source("file", ["path/to/f1.grib", "path/to/f2.grib"])
 
       # a path can be a directory, in this case it is recursively scanned for supported files
       ds = earthkit.data.from_source("file", "path/to/dir")
 
 
+  The following examples using parts:
+
+  .. code:: python
+
+      import earthkit.data
+
+      # reading only certain parts (byte ranges) from a single file
+      ds = earthkit.data.from_source("file", "my.grib", parts=[(0, 150), (400, 160)])
+
+      # reading only certain parts (byte ranges) from multiple files
+      ds = earthkit.data.from_source(
+          "file",
+          [
+              ("a.grib", (0, 150)),
+              ("b.grib", (240, 120)),
+              ("c.grib", None),
+              ("d.grib", [(240, 120), (720, 120)]),
+          ],
+      )
+
+
+
   Further examples:
 
+    - :ref:`/examples/files.ipynb`
+    - :ref:`/examples/multi_files.ipynb`
+    - :ref:`/examples/file_parts.ipynb`
+    - :ref:`/examples/tar_files.ipynb`
     - :ref:`/examples/grib_overview.ipynb`
-    - :ref:`/examples/grib_multi.ipynb`
     - :ref:`/examples/bufr_temp.ipynb`
     - :ref:`/examples/netcdf.ipynb`
     - :ref:`/examples/odb.ipynb`
 
 .. _data-sources-file-pattern:
 
 file-pattern
@@ -134,48 +167,71 @@
   The code above will read the following files::
 
     path/to/data-2020-05-02-12-t2.grib
     path/to/data-2020-05-02-12-msl.grib
     path/to/data-2020-05-02-18-t2.grib
     path/to/data-2020-05-02-18-msl.grib
 
+Further examples:
+
+    - :ref:`/examples/files.ipynb`
+
 
 .. _data-sources-url:
 
 url
 ---
 
-.. py:function:: from_source("url", url, unpack=True, stream=False, batch_size=1, group_by=None)
+.. py:function:: from_source("url", url, unpack=True, parts=None, stream=False, batch_size=1, group_by=None)
   :noindex:
 
   The ``url`` source will download the data from the address specified and store it in the :ref:`cache <caching>`. The supported data formats are the same as for the :ref:`file <data-sources-file>` data source above.
 
-  :param url: the URL to download
+  :param url: the URL(s) to download. Each URL can contain the :ref:`parts <parts>` defining the byte ranges to read.
   :type url: str
   :param bool unpack: for archive formats such as ``.zip``, ``.tar``, ``.tar.gz``, etc, *earthkit-data* will attempt to open it and extract any usable file. To keep the downloaded file as is use ``unpack=False``
+  :param parts: the :ref:`parts <parts>` to read from the resource(s) specified by ``url``. Cannot be used when ``url`` already defines the :ref:`parts <parts>`.
+  :type parts: pair, list or tuple of pairs, None
   :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. This option only works for GRIB data. No archive formats supported (``unpack`` is ignored). ``stream`` only works for ``http`` and ``https`` URLs.
   :param int batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. For details see :ref:`stream source <data-sources-stream>`.
   :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. For details see :ref:`stream source <data-sources-stream>`.
   :type group_by: str, list of str
   :param dict **kwargs: other keyword arguments specifying the request
 
   .. code-block:: python
 
       >>> import earthkit.data
       >>> ds = earthkit.data.from_source(
       ...     "url",
       ...     "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib",
       ... )
-      >>> len(ds)
-      4
+      >>> ds.ls()
+        centre shortName    typeOfLevel  level  dataDate  dataTime stepRange dataType  number    gridType
+      0   ecmf         t  isobaricInhPa    500  20070101      1200         0       an       0  regular_ll
+      1   ecmf         z  isobaricInhPa    500  20070101      1200         0       an       0  regular_ll
+      2   ecmf         t  isobaricInhPa    850  20070101      1200         0       an       0  regular_ll
+      3   ecmf         z  isobaricInhPa    850  20070101      1200         0       an       0  regular_ll
+
+  .. code-block:: python
+
+      >>> import earthkit.data
+      >>> ds = earthkit.data.from_source(
+      ...     "url",
+      ...     "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib",
+      ...     parts=[(0, 130428), (260856, 130428)],
+      ... )
+      >>> ds.ls()
+        centre shortName    typeOfLevel  level  dataDate  dataTime stepRange dataType  number    gridType
+      0   ecmf         t  isobaricInhPa    500  20070101      1200         0       an       0  regular_ll
+      1   ecmf         t  isobaricInhPa    850  20070101      1200         0       an       0  regular_ll
 
   Further examples:
 
-    - :ref:`/examples/grib_url.ipynb`
-    - :ref:`/examples/grib_url_stream.ipynb`
+    - :ref:`/examples/url.ipynb`
+    - :ref:`/examples/url_stream.ipynb`
 
 
 .. _data-sources-url-pattern:
 
 
 url-pattern
 -----------
@@ -211,14 +267,40 @@
     https://www.example.com/data-2-b-unique.csv
     https://www.example.com/data-3-b-unique.csv
 
   If the urls are pointing to archive format, the data will be unpacked by
   ``url-pattern`` according to the **unpack** argument, similarly to what
   the source ``url`` does (see above the :ref:`data-sources-url` source).
 
+
+
+.. _data-sources-sample:
+
+sample
+------
+
+.. py:function:: from_source("sample", name_or_path)
+  :noindex:
+
+  The ``sample`` source will download example data prepared for earthkit and store it in the :ref:`cache <caching>`. The supported data formats are the same as for the :ref:`file <data-sources-file>` data source above.
+
+  :param name_or_path: input file name(s) or relative path(s) to the root of the remote storage folder.
+  :type name_or_path: str, list, tuple
+
+  .. code-block:: python
+
+    >>> import earthkit.data
+    >>> ds = earthkit.data.from_source("sample", "storm_ophelia_wind_850.grib")
+    >>> ds.ls()
+      centre shortName    typeOfLevel  level  dataDate  dataTime stepRange dataType  number    gridType
+    0   ecmf         u  isobaricInhPa    850  20171016         0         0       an       0  regular_ll
+    1   ecmf         v  isobaricInhPa    850  20171016         0         0       an       0  regular_ll
+
+
+
 .. _data-sources-stream:
 
 stream
 --------------
 
 .. py:function:: from_source("stream", stream, batch_size=1, group_by=None)
   :noindex:
@@ -303,17 +385,17 @@
       >>> len(ds)
       4
 
       # now ds stores all the messages in memory
 
   See the following notebook examples for further details:
 
-    - :ref:`/examples/grib_from_stream.ipynb`
+    - :ref:`/examples/data_from_stream.ipynb`
     - :ref:`/examples/fdb.ipynb`
-    - :ref:`/examples/grib_url_stream.ipynb`
+    - :ref:`/examples/url_stream.ipynb`
 
 
 .. _data-sources-memory:
 
 memory
 --------------
 
@@ -334,14 +416,34 @@
       stream = io.BytesIO(buffer)
 
       ds = earthkit.data.from_source("stream", stream)
       for f in ds:
           print(f.metadata("param"))
 
 
+.. _data-sources-multi:
+
+multi
+--------------
+
+.. py:function:: from_source("multi", *sources, merger=None, **kwargs)
+  :noindex:
+
+  The ``multi`` source reads multiple sources.
+
+  :param tuple *sources: the sources
+  :param merger: if it is None an attempt is made to merge/concatenate the sources by their classes (using the nearest common class). Otherwise the sources are merged/concatenated using the merger in a lazy way. The merger can one of the following:
+
+    - class/object implementing  the :func:`to_xarray` or :func:`to_pandas` methods
+    - callable
+    - str, describing a call either to "concat" or "merge". E.g.: "concat(concat_dim=time)"
+    - tuple with 2 elements. The fist element is a str, either "concat" or "merge", and the second element is a dict with the keyword arguments for the call. E.g.: ("concat", {"concat_dim": "time"})
+  :param dict **kwargs: other keyword arguments
+
+
 
 .. _data-sources-ads:
 
 ads
 ---
 
 .. py:function:: from_source("ads", dataset, *args, **kwargs)
@@ -378,22 +480,27 @@
 
 
 .. _data-sources-cds:
 
 cds
 ---
 
-.. py:function:: from_source("cds", dataset, *args, **kwargs)
+.. py:function:: from_source("cds", dataset, *args, prompt=True, **kwargs)
   :noindex:
 
   The ``cds`` source accesses the `Copernicus Climate Data Store`_ (CDS), using the cdsapi_ package. In addition to data retrieval, the request has post-processing options such as ``grid`` and ``area`` for regridding and sub-area extraction respectively. It can
   also contain the earthkit-data specific :ref:`split_on <split_on>` parameter.
 
   :param str dataset: the name of the CDS dataset
   :param tuple *args: specify the request as dict. A sequence of dicts can be used to specify multiple requests.
+  :param bool prompt: when True it can offer a prompt to specify the credentials for cdsapi_ and write them into the default RC file ``~/.cdsapirc``. The prompt only appears when:
+
+    - no cdsapi_ RC file exists at the default location ``~/.cdsapirc``
+    - no cdsapi_ RC file exists at the location specified via the ``CDSAPI_RC`` environment variable
+    - no credentials specified via the ``CDSAPI_URL`` and ``CDSAPI_KEY`` environment variables
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves ERA5 reanalysis GRIB data for a subarea for 2 surface parameters. The request is specified using ``kwargs``:
 
   .. code-block:: python
 
       import earthkit.data
@@ -439,20 +546,22 @@
 
 
 .. _data-sources-eod:
 
 ecmwf-open-data
 -------------------
 
-.. py:function:: from_source("ecmwf-open-data", *args, **kwargs)
+.. py:function:: from_source("ecmwf-open-data", *args, source="ecmwf", model="ifs", **kwargs)
   :noindex:
 
   The ``ecmwf-open-data`` source provides access to the `ECMWF open data`_, which is a subset of ECMWF real-time forecast data made available to the public free of charge.  It uses the `ecmwf-opendata <https://github.com/ecmwf/ecmwf-opendata>`_ package.
 
   :param tuple *args: specify the request as a dict
+  :param str source: either the name of the server to contact or a fully qualified URL. Possible values are "ecmwf" to access ECMWF's servers, or "azure" to access data hosted on Microsoft's Azure. Default is "ecmwf".
+  :param str model: name of the model that produced the data. Use "ifs" for the physics-driven model and "aifs" for the data-driven model. Please note that "aifs" is currently experimental and only produces a small subset of fields. Default is "ifs".
   :param dict **kwargs: other keyword arguments specifying the request
 
   Details about the request format can be found `here <https://github.com/ecmwf/ecmwf-opendata>`__.
 
   The following example retrieves forecast for 2 surface parameters from the latest forecast:
 
   .. code-block:: python
@@ -559,26 +668,31 @@
 
 
 .. _data-sources-mars:
 
 mars
 --------------
 
-.. py:function:: from_source("mars", *args, **kwargs)
+.. py:function:: from_source("mars", *args, prompt=True, **kwargs)
   :noindex:
 
   The ``mars`` source will retrieve data from the ECMWF MARS (Meteorological Archival and Retrieval System) archive. In addition
   to data retrieval, the request specified as ``*args`` and/or ``**kwargs`` also has GRIB post-processing options such as ``grid`` and ``area`` for regridding and
   sub-area extraction, respectively.
 
   To figure out which data you need, or discover relevant data available in MARS, see the publicly accessible `MARS catalog`_ (or this `access restricted catalog <https://apps.ecmwf.int/mars-catalogue/>`_).
 
   The MARS access is direct when the MARS client is installed (as at ECMWF), otherwise it will use the `web API`_. In order to use the `web API`_ you will need to register and retrieve an access token. For a more extensive documentation about MARS, please refer to the `MARS user documentation`_.
 
   :param tuple *args: positional arguments specifying the request as a dict
+  :param bool prompt: when True it can offer a prompt to specify the credentials for `web API`_ and write them into the default RC file ``~/.ecmwfapirc``. The prompt only appears when:
+
+    - no `web API`_ RC file exists at the default location ``~/.ecmwfapirc``
+    - no `web API`_ RC file exists at the location specified via the ``ECMWF_API_RC_FILE`` environment variable
+    - no credentials specified via the ``ECMWF_API_URL`` and ``ECMWF_API_KEY``  environment variables
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves analysis GRIB data for a subarea for 2 surface parameters:
 
   .. code-block:: python
 
       import earthkit.data
@@ -597,31 +711,52 @@
   Data downloaded from MARS is stored in the :ref:`cache <caching>`.
 
   Further examples:
 
       - :ref:`/examples/mars.ipynb`
 
 
+.. _data-sources-opendap:
+
+opendap
+--------
+
+.. py:function:: from_source("opendap", url)
+  :noindex:
+
+  The ``opendap`` source accesses NetCDF data from `OPeNDAP <https://en.wikipedia.org/wiki/OPeNDAP>`_ services. OPenDAP is an acronym for "Open-source Project for a Network Data Access Protocol".
+
+  :param str url: the url of the remote NetCDF file
+
+  Examples:
+
+      - :ref:`/examples/netcdf_opendap.ipynb`
+
+
 .. _data-sources-polytope:
 
 polytope
 --------
 
-.. py:function:: from_source("polytope", collection, *args, stream=True,  batch_size=1, group_by=None, **kwargs)
+.. py:function:: from_source("polytope", collection, *args, address=None, user_email=None, user_key=None, stream=True, batch_size=1, group_by=None, **kwargs)
   :noindex:
 
   The ``polytope`` source accesses the `Polytope web services <https://polytope-client.readthedocs.io/en/latest/>`_ , using the polytope-client_ package.
 
   :param str collection: the name of the polytope collection
   :param tuple *args: specify the request as a dict
+  :param str address: specify the address of the polytope service
+  :param str user_email: specify the user email credential. Must be used together with ``user_key``. This is an alternative to using the ``POLYTOPE_USER_EMAIL`` environment variable. *Added in version 0.7.0*
+  :param str user_key: specify the user key credential. Must be used together with ``user_email``. This is an alternative to using the ``POLYTOPE_USER_KEY`` environment variable. *Added in version 0.7.0*
   :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. Stream-based access only works for :ref:`grib` and CoverageJson data.
   :param int batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the data is read straight to memory. For details see :ref:`stream source <data-sources-stream>`.
   :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. For details see :ref:`stream source <data-sources-stream>`.
   :type group_by: str, list of str
-  :param dict **kwargs: other keyword arguments specifying the request
+  :param dict **kwargs: other keyword arguments, these can include options passed to the polytope-client_
+
 
   The following example retrieves GRIB data from the "ecmwf-mars" polytope collection:
 
   .. code-block:: python
 
       import earthkit.data
 
@@ -653,21 +788,26 @@
 
 
 .. _data-sources-wekeo:
 
 wekeo
 -----
 
-.. py:function:: from_source("wekeo", dataset, *args, **kwargs)
+.. py:function:: from_source("wekeo", dataset, *args, prompt=True, **kwargs)
   :noindex:
 
   `WEkEO`_ is the Copernicus DIAS reference service for environmental data and virtual processing environments. The ``wekeo`` source provides access to `WEkEO`_ using the WEkEO grammar. The retrieval is based on the hda_ Python API.
 
   :param str dataset: the name of the WEkEO dataset
   :param tuple *args: specify the request as a dict
+  :param bool prompt: when True it can offer a prompt to specify the credentials for hda_ and write them into the default RC file ``~/.hdarc``. The prompt only appears when:
+
+    - no hda_ RC file exists at the default location ``~/.hdarc``
+    - no hda_ RC file exists at the location specified via the ``HDA_RC`` environment variable
+    - no credentials specified via the ``HDA_URL``, ``HDA_USER`` and ``HDA_PASSWORD`` environment variables
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves Normalized Difference Vegetation Index data derived from EO satellite imagery in NetCDF format:
 
   .. code-block:: python
 
       import earthkit.data
@@ -698,21 +838,26 @@
 
 
 .. _data-sources-wekeocds:
 
 wekeocds
 --------
 
-.. py:function:: from_source("wekeocds", dataset, *args, **kwargs)
+.. py:function:: from_source("wekeocds", dataset, *args, prompt=True, **kwargs)
   :noindex:
 
   `WEkEO`_ is the Copernicus DIAS reference service for environmental data and virtual processing environments. The ``wekeocds`` source provides access to `Copernicus Climate Data Store`_ (CDS) datasets served on `WEkEO`_ using the `cdsapi`_ grammar. The retrieval is based on the hda_ Python API.
 
   :param str dataset: the name of the WEkEO dataset
   :param tuple *args: specify the request as a dict
+  :param bool prompt: when True it can offer a prompt to specify the credentials for hda_ and write them into the default RC file ``~/.hdarc``. The prompt only appears when:
+
+    - no hda_ RC file exists at the default location ``~/.hdarc``
+    - no hda_ RC file exists at the location specified via the ``HDA_RC`` environment variable
+    - no credentials specified via the ``HDA_URL``, ``HDA_USER`` and ``HDA_PASSWORD`` environment variables
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves ERA5 surface data for multiple days in GRIB format:
 
   .. code-block:: python
 
       import earthkit.data
```

### Comparing `earthkit-data-0.6.0/docs/guide/split_on.rst` & `earthkit_data-0.7.0/docs/guide/misc/split_on.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/index.rst` & `earthkit_data-0.7.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ======================================================
 
 .. warning::
 
    This project is in the **BETA** stage of development. Please be aware that interfaces and functionality may change as the project develops. If this software is to be used in operational systems you are **strongly advised to use a released tag in your system configuration**, and you should be willing to accept incoming changes and bug fixes that require adaptations on your part. ECMWF **does use** this software in operations and abides by the same caveats.
 
 **earthkit-data** is a format-agnostic Python interface for geospatial data with a focus on meteorology and
-climate science.
+climate science. It is the data handling component of :xref:`earthkit`.
 
 **earthkit-data** makes it simple to read, inspect and slice data from a wide range of
 geospatial input types (:ref:`grib`, :ref:`netcdf` and more) and transform them into
 familiar scientific Python objects (including numpy arrays, pandas dataframes, xarray datasets).
 
 .. code-block:: python
 
@@ -23,17 +23,16 @@
 **earthkit-data** provides additional convenient methods for quickly inspecting certain
 features of your input data, such as data dimensionality, axes, coordinate
 reference systems and bounding boxes.
 
 .. toctree::
    :maxdepth: 1
    :caption: Examples
-   :titlesonly:
 
-   examples
+   examples/index
 
 .. toctree::
    :maxdepth: 1
    :caption: Documentation
 
    howtos
    guide/index
@@ -50,14 +49,20 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: Plugins
 
    plugins/index
 
+.. toctree::
+   :maxdepth: 1
+   :caption: Projects
+
+   earthkit <https://earthkit.readthedocs.io/en/latest>
+
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 
 .. * :ref:`modindex`
```

### Comparing `earthkit-data-0.6.0/docs/licence.rst` & `earthkit_data-0.7.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/make.bat` & `earthkit_data-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/plugins/index.rst` & `earthkit_data-0.7.0/docs/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/plugins/plugins.rst` & `earthkit_data-0.7.0/docs/plugins/plugins.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/plugins/sources_plugin.rst` & `earthkit_data-0.7.0/docs/plugins/sources_plugin.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/release_notes/version_0.2_updates.rst` & `earthkit_data-0.7.0/docs/release_notes/version_0.2_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/release_notes/version_0.3_updates.rst` & `earthkit_data-0.7.0/docs/release_notes/version_0.3_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/release_notes/version_0.4_updates.rst` & `earthkit_data-0.7.0/docs/release_notes/version_0.4_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/docs/release_notes/version_0.5_updates.rst` & `earthkit_data-0.7.0/docs/release_notes/version_0.5_updates.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 New features
 ++++++++++++++++
 
 - changed the default :ref:`cache policy <cache_policies>` to :ref:`off <off_cache_policy>`. See the :ref:`/examples/cache.ipynb` notebook example.
 - enabled the :ref:`off <off_cache_policy>` cache policy to access remote sources like :ref:`data-sources-mars`
 - allowed creating source :ref:`plugins <plugin-overview>`
-- enabled reading :ref:`data-sources-url` sources as streams. See the :ref:`/examples/grib_url_stream.ipynb` notebook example
+- enabled reading :ref:`data-sources-url` sources as streams. See the :ref:`/examples/url_stream.ipynb` notebook example
 - enabled reading :ref:`data-sources-polytope` sources as streams
 - added the :meth:`FieldList.to_fieldlist() <data.core.fieldlist.FieldList.to_fieldlist>` method to convert to a new :class:`FieldList` based on a given backend
 - added the :meth:`nearest_point_haversine` and :meth:`nearest_point_kdtree` methods to find the nearest point out of a set of locations. See the :ref:`/examples/grib_nearest_gridpoint.ipynb` and :ref:`/examples/grib_time_series.ipynb` notebook examples.
 - enabled using multiple keys and dictionaries in the :ref:`split_on <split_on>` request parameter for :ref:`data-sources-cds` retrievals
 - enabled using list of requests in :ref:`data-sources-cds` retrievals
 - added the experimental "constants" source type
 - ensured consistent usage of ``pandas_read_csv_kwargs`` for :ref:`data-sources-file` and :ref:`data-sources-cds` sources
```

### Comparing `earthkit-data-0.6.0/docs/skip_api_rules.py` & `earthkit_data-0.7.0/docs/skip_api_rules.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/__init__.py` & `earthkit_data-0.7.0/earthkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/__init__.py` & `earthkit_data-0.7.0/earthkit/data/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/args_kwargs.py` & `earthkit_data-0.7.0/earthkit/data/arguments/args_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/argument.py` & `earthkit_data-0.7.0/earthkit/data/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/earthkit_types.py` & `earthkit_data-0.7.0/earthkit/data/arguments/earthkit_types.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/input_manager.py` & `earthkit_data-0.7.0/earthkit/data/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/arguments/transformers.py` & `earthkit_data-0.7.0/earthkit/data/arguments/transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/conf/css/tab.css` & `earthkit_data-0.7.0/earthkit/data/conf/css/tab.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/conf/css/tree.css` & `earthkit_data-0.7.0/earthkit/data/conf/css/tree.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/conf/global_grids.json` & `earthkit_data-0.7.0/earthkit/data/conf/global_grids.json`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/conf/gridspec.yaml` & `earthkit_data-0.7.0/earthkit/data/conf/gridspec.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/conf/gridspec_schema.json` & `earthkit_data-0.7.0/earthkit/data/conf/gridspec_schema.json`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/__init__.py` & `earthkit_data-0.7.0/earthkit/data/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     def unique_values(self, *coords, remapping=None, progress_bar=True):
         """
         Given a list of metadata attributes, such as date, param, levels,
         returns the list of unique values for each attributes
         """
         from earthkit.data.core.order import build_remapping
-        from earthkit.data.utils import progress_bar
+        from earthkit.data.utils.progbar import progress_bar
 
         assert len(coords)
         assert all(isinstance(k, str) for k in coords), coords
 
         remapping = build_remapping(remapping)
         iterable = self
```

### Comparing `earthkit-data-0.6.0/earthkit/data/core/caching.py` & `earthkit_data-0.7.0/earthkit/data/core/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 import sqlite3
 import threading
 import time
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from random import randrange
 
-import pandas as pd
-from filelock import FileLock
-
 from earthkit.data.core.settings import SETTINGS
 from earthkit.data.core.temporary import temp_directory
 from earthkit.data.utils import humanize
 from earthkit.data.utils.html import css
 
 VERSION = 2
 CACHE_DB = f"cache-{VERSION}.db"
@@ -83,14 +80,16 @@
 
 
 def disk_usage(path):
     return DiskUsage(path)
 
 
 def default_serialiser(o):
+    import pandas as pd
+
     if isinstance(o, (datetime.date, datetime.datetime)):
         return o.isoformat()
     if isinstance(o, (pd.Timestamp)):
         return o.isoformat()
     if isinstance(o, (pd.DatetimeIndex)):
         return [_.isoformat() for _ in o]
     return json.JSONEncoder.default(o)
@@ -1032,19 +1031,22 @@
             if callable(force):
                 owner_data = record["owner_data"]
                 if owner_data is not None:
                     owner_data = json.loads(owner_data)
                 force = force(args, path, owner_data)
 
             if force:
+                LOG.debug(f"decache file by force: {path=}")
                 CACHE._decache_file(path)
+                record = CACHE._register_cache_file(path, owner, args)
 
         if not os.path.exists(path):
-            lock = path + ".lock"
+            from filelock import FileLock
 
+            lock = path + ".lock"
             with FileLock(lock):
                 if not os.path.exists(
                     path
                 ):  # Check again, another thread/process may have created the file
                     owner_data = create(path + ".tmp", args)
                     os.rename(path + ".tmp", path)
                     CACHE._update_entry(path, owner_data)
@@ -1067,14 +1069,16 @@
                 owner.lower(),
                 m.hexdigest(),
                 extension,
             ),
         )
 
         if not os.path.exists(path):
+            from filelock import FileLock
+
             lock = path + ".lock"
             with FileLock(lock):
                 if not os.path.exists(
                     path
                 ):  # Check again, another thread/process may have created the file
                     owner_data = create(path + ".tmp", args)
                     os.rename(path + ".tmp", path)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/core/fieldlist.py` & `earthkit_data-0.7.0/earthkit/data/core/fieldlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,50 +9,110 @@
 
 import math
 from abc import abstractmethod
 from collections import defaultdict
 
 from earthkit.data.core import Base
 from earthkit.data.core.index import Index
-from earthkit.data.decorators import cached_method
+from earthkit.data.decorators import cached_method, detect_out_filename
+from earthkit.data.utils.array import ensure_backend, numpy_backend
 from earthkit.data.utils.metadata import metadata_argument
 
 
 class Field(Base):
-    r"""Represents a Field."""
+    r"""Represent a Field."""
 
-    def __init__(self, metadata=None):
+    def __init__(
+        self,
+        array_backend,
+        metadata=None,
+        raw_values_backend=None,
+        raw_other_backend=None,
+    ):
         self.__metadata = metadata
+        self._array_backend = array_backend
+        self._raw_values_backend = ensure_backend(raw_values_backend)
+        self._raw_other_backend = ensure_backend(raw_other_backend)
+
+    @property
+    def array_backend(self):
+        r""":obj:`ArrayBackend`: Return the array backend of the field."""
+        return self._array_backend
+
+    @property
+    def raw_values_backend(self):
+        r""":obj:`ArrayBackend`: Return the array backend used by the low level API
+        to extract the field values.
+        """
+        return self._raw_values_backend
+
+    @property
+    def raw_other_backend(self):
+        r""":obj:`ArrayBackend`: Return the array backend used by the low level API
+        to extract non-field-related values, e.g. latitudes, longitudes.
+        """
+        return self._raw_other_backend
+
+    def _to_array(self, v, array_backend=None, source_backend=None):
+        r"""Convert an array into an ``array backend``.
+
+        Parameters
+        ----------
+        v: array-like
+            The values.
+        array_backend: :obj:`ArrayBackend`
+            The target array backend. When it is None ``self.array_backend`` will
+            be used.
+        source_backend: :obj:`ArrayBackend`
+            The array backend of ``v``. When None, it will be automatically detected.
+
+        Returns
+        -------
+        array-like
+            ``v`` converted onto the ``array_backend``.
+
+        """
+        if array_backend is None:
+            return self._array_backend.to_array(v, source_backend)
+        else:
+            array_backend = ensure_backend(array_backend)
+            return array_backend.to_array(v, source_backend)
 
     @abstractmethod
     def _values(self, dtype=None):
-        r"""Return the values stored in the field as an ndarray.
+        r"""Return the raw values extracted from the underlying storage format
+        of the field.
 
         Parameters
         ----------
-        dtype: str, numpy.dtype or None
+        dtype: str, array.dtype or None
             Typecode or data-type of the array. When it is :obj:`None` the default
             type used by the underlying data accessor is used. For GRIB it is
-            ``np.float64``.
+            ``float64``.
+
+        The original shape and array backend type of the raw values are kept.
 
         Returns
         -------
-        ndarray
-            Field values
+        array-like
+            Field values in the format specified by :attr:`raw_values_backend`.
 
         """
         self._not_implemented()
 
     @property
     def values(self):
-        r"""ndarray: Get the values stored in the field as a 1D ndarray."""
-        v = self._values()
+        r"""array-like: Get the values stored in the field as a 1D array. The array type
+        is defined by :attr:`array_backend`
+        """
+        v = self._to_array(self._values(), source_backend=self.raw_values_backend)
         if len(v.shape) != 1:
             n = math.prod(v.shape)
-            return v.reshape(n)
+            n = (n,)
+            return self._array_backend.array_ns.reshape(v, n)
         return v
 
     def _make_metadata(self):
         r"""Create a field metadata object."""
         self._not_implemented()
 
     @property
@@ -68,28 +128,58 @@
         Parameters
         ----------
         flatten: bool
             When it is True a flat ndarray is returned. Otherwise an ndarray with the field's
             :obj:`shape` is returned.
         dtype: str, numpy.dtype or None
             Typecode or data-type of the array. When it is :obj:`None` the default
-            type used by the underlying data accessor is used. For GRIB it is ``np.float64``.
+            type used by the underlying data accessor is used. For GRIB it is ``float64``.
 
         Returns
         -------
         ndarray
             Field values
 
         """
         v = self._values(dtype=dtype)
+        v = numpy_backend().to_array(v, self.raw_values_backend)
         shape = self._required_shape(flatten)
         if shape != v.shape:
             return v.reshape(shape)
         return v
 
+    def to_array(self, flatten=False, dtype=None, array_backend=None):
+        r"""Return the values stored in the field in the
+        format of :attr:`array_backend`.
+
+        Parameters
+        ----------
+        flatten: bool
+            When it is True a flat array is returned. Otherwise an array with the field's
+            :obj:`shape` is returned.
+        dtype: str, array.dtype or None
+            Typecode or data-type of the array. When it is :obj:`None` the default
+            type used by the underlying data accessor is used. For GRIB it is ``float64``.
+
+        Returns
+        -------
+        array-array
+            Field values in the format od :attr:`array_backend`.
+
+        """
+        v = self._to_array(
+            self._values(dtype=dtype),
+            array_backend=array_backend,
+            source_backend=self.raw_values_backend,
+        )
+        shape = self._required_shape(flatten)
+        if shape != v.shape:
+            return self._array_backend.array_ns.reshape(v, shape)
+        return v
+
     def _required_shape(self, flatten):
         return self.shape if not flatten else (math.prod(self.shape),)
 
     def _array_matches(self, array, flatten=False, dtype=None):
         shape = self._required_shape(flatten)
         return shape == array.shape and (dtype is None or dtype == array.dtype)
 
@@ -98,27 +188,28 @@
 
         Parameters
         ----------
         keys: :obj:`str`, :obj:`list` or :obj:`tuple`
             Specifies the type of data to be returned. Any combination of "lat", "lon" and "value"
             is allowed here.
         flatten: bool
-            When it is True a flat ndarray per key is returned. Otherwise an ndarray with the field's
+            When it is True a flat array per key is returned. Otherwise an array with the field's
             :obj:`shape` is returned for each key.
-        dtype: str, numpy.dtype or None
+        dtype: str, array.dtype or None
             Typecode or data-type of the arrays. When it is :obj:`None` the default
-            type used by the underlying data accessor is used. For GRIB it is ``np.float64``.
+            type used by the underlying data accessor is used. For GRIB it is ``float64``.
 
 
         Returns
         -------
-        ndarray
-            An ndarray containing one ndarray per key is returned
+        array-like
+            An multi-dimensional array containing one array per key is returned
             (following the order in ``keys``). When ``keys`` is a single value only the
-            ndarray belonging to the key is returned.
+            array belonging to the key is returned. The array format is specified by
+            :attr:`array_backend`.
 
 
         Examples
         --------
         - :ref:`/examples/grib_lat_lon_value.ipynb`
 
         >>> import earthkit.data
@@ -143,75 +234,80 @@
         to_latlon
         to_points
         to_numpy
         values
 
         """
         _keys = dict(
-            lat=self._metadata.geography.latitudes,
-            lon=self._metadata.geography.longitudes,
-            value=self._values,
+            lat=(self._metadata.geography.latitudes, self.raw_other_backend),
+            lon=(self._metadata.geography.longitudes, self.raw_other_backend),
+            value=(self._values, self.raw_values_backend),
         )
 
         if isinstance(keys, str):
             keys = [keys]
 
         for k in keys:
             if k not in _keys:
                 raise ValueError(f"data: invalid argument: {k}")
 
-        r = [_keys[k](dtype=dtype) for k in keys]
+        r = [
+            self._to_array(_keys[k][0](dtype=dtype), source_backend=_keys[k][1])
+            for k in keys
+        ]
         shape = self._required_shape(flatten)
         if shape != r[0].shape:
-            r = [x.reshape(shape) for x in r]
+            # r = [x.reshape(shape) for x in r]
+            r = [self._array_backend.array_ns.reshape(x, shape) for x in r]
 
         if len(r) == 1:
             return r[0]
         else:
-            import numpy as np
-
-            return np.array(r)
+            return self._array_backend.array_ns.stack(r)
 
     def to_points(self, flatten=False, dtype=None):
         r"""Return the geographical coordinates in the data's original
         Coordinate Reference System (CRS).
 
         Parameters
         ----------
         flatten: bool
-            When it is True 1D ndarrays are returned. Otherwise ndarrays with the field's
+            When it is True 1D arrays are returned. Otherwise arrays with the field's
             :obj:`shape` are returned.
-        dtype: str, numpy.dtype or None
+        dtype: str, array.dtype or None
             Typecode or data-type of the arrays. When it is :obj:`None` the default
             type used by the underlying data accessor is used. For GRIB it is
-            ``np.float64``.
+            ``float64``.
 
         Returns
         -------
         dict
-            Dictionary with items "x" and "y", containing the ndarrays of the x and
-            y coordinates, respectively.
+            Dictionary with items "x" and "y", containing the arrays of the x and
+            y coordinates, respectively. The array format is specified by
+            :attr:`array_backend`.
 
         Raises
         ------
         ValueError
             When the coordinates in the data's original CRS are not available.
 
         See Also
         --------
         to_latlon
 
         """
         x = self._metadata.geography.x(dtype=dtype)
         y = self._metadata.geography.y(dtype=dtype)
         if x is not None and y is not None:
+            x = self._to_array(x, source_backend=self.raw_other_backend)
+            y = self._to_array(y, source_backend=self.raw_other_backend)
             shape = self._required_shape(flatten)
             if shape != x.shape:
-                x = x.reshape(shape)
-                y = y.reshape(shape)
+                x = self._array_backend.array_ns.reshape(x, shape)
+                y = self._array_backend.array_ns.reshape(y, shape)
             return dict(x=x, y=y)
         elif self.projection().CARTOPY_CRS == "PlateCarree":
             lon, lat = self.data(("lon", "lat"), flatten=flatten, dtype=dtype)
             return dict(x=lon, y=lat)
         else:
             raise ValueError(
                 "to_points(): geographical coordinates in original CRS are not available"
@@ -219,26 +315,27 @@
 
     def to_latlon(self, flatten=False, dtype=None):
         r"""Return the latitudes/longitudes of all the gridpoints in the field.
 
         Parameters
         ----------
         flatten: bool
-            When it is True 1D ndarrays are returned. Otherwise ndarrays with the field's
+            When it is True 1D arrays are returned. Otherwise arrays with the field's
             :obj:`shape` are returned.
-        dtype: str, numpy.dtype or None
+        dtype: str, array.dtype or None
             Typecode or data-type of the arrays. When it is :obj:`None` the default
             type used by the underlying data accessor is used. For GRIB it is
-            ``np.float64``.
+            ``float64``.
 
         Returns
         -------
         dict
-            Dictionary with items "lat" and "lon", containing the ndarrays of the latitudes and
-            longitudes, respectively.
+            Dictionary with items "lat" and "lon", containing the arrays of the latitudes and
+            longitudes, respectively. The array format is specified by
+            :attr:`array_backend`.
 
         See Also
         --------
         to_points
 
         """
         lon, lat = self.data(("lon", "lat"), flatten=flatten, dtype=dtype)
@@ -531,26 +628,66 @@
         result = {}
         for name in names:
             result[name] = self._metadata.get(name, None)
         return result
 
 
 class FieldList(Index):
-    r"""Represents a list of :obj:`Field` \s."""
+    r"""Represent a list of :obj:`Field` \s.
+
+    Parameters
+    ----------
+    array_backend: str, :obj:`ArrayBackend`
+        The array backend. When it is None the array backend
+        defaults to "numpy".
+    """
 
     _md_indices = {}
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, array_backend=None, **kwargs):
+        self._array_backend = ensure_backend(array_backend)
+        super().__init__(**kwargs)
+
+    def _init_from_mask(self, index):
+        self._array_backend = index._index.array_backend
+
+    def _init_from_multi(self, index):
+        self._array_backend = index._indexes[0].array_backend
 
     @staticmethod
     def from_numpy(array, metadata):
-        from earthkit.data.sources.numpy_list import NumpyFieldList
+        from earthkit.data.sources.array_list import ArrayFieldList
+
+        return ArrayFieldList(array, metadata, array_backend=numpy_backend())
+
+    @staticmethod
+    def from_array(array, metadata):
+        r"""Create an :class:`ArrayFieldList`.
+
+        Parameters
+        ----------
+        array: array-like, list
+            The fields' values. When it is a list it must contain one array per field.
+            The array type must be supported by :class:`ArrayBackend`.
+        metadata: list
+            The fields' metadata. Must contain one :class:`Metadata` object per field.
+
+        In the generated :class:`ArrayFieldList`, each field is represented by an array
+        storing the field values and a :class:`MetaData` object holding
+        the field metadata. The shape and dtype of the array is controlled by the ``kwargs``.
+        Please note that generated :class:`ArrayFieldList` stores all the field values in
+        a single array.
+        """
+        from earthkit.data.sources.array_list import ArrayFieldList
+
+        return ArrayFieldList(array, metadata)
 
-        return NumpyFieldList(array, metadata)
+    @property
+    def array_backend(self):
+        return self._array_backend
 
     def ignore(self):
         # When the concrete type is Fieldlist we assume the object was
         # created with Fieldlist() i.e. it is empty. We ignore it from
         # all the merge operations.
         if type(self) is FieldList:
             return True
@@ -659,43 +796,67 @@
         if key in self.indices():
             return self.indices()[key]
 
         self._md_indices[key] = self._find_index_values(key)
         return self._md_indices[key]
 
     def to_numpy(self, **kwargs):
-        r"""Return the field values as an ndarray. It is formed as the array of the
+        r"""Return all the fields' values as an ndarray. It is formed as the array of the
         :obj:`data.core.fieldlist.Field.to_numpy` values per field.
 
         Parameters
         ----------
         **kwargs: dict, optional
             Keyword arguments passed to :obj:`data.core.fieldlist.Field.to_numpy`
 
         Returns
         -------
         ndarray
             Array containing the field values.
 
         See Also
         --------
+        to_array
         values
         """
         import numpy as np
 
         return np.array([f.to_numpy(**kwargs) for f in self])
 
+    def to_array(self, **kwargs):
+        r"""Return all the fields' values as an array. It is formed as the array of the
+        :obj:`data.core.fieldlist.Field.to_array` values per field.
+
+        Parameters
+        ----------
+        **kwargs: dict, optional
+            Keyword arguments passed to :obj:`data.core.fieldlist.Field.to_array`
+
+        Returns
+        -------
+        array-like
+            Array containing the field values. The array format is specified by
+            :attr:`array_backend`.
+
+        See Also
+        --------
+        values
+        to_numpy
+        """
+        x = [f.to_array(**kwargs) for f in self]
+        return self._array_backend.array_ns.stack(x)
+
     @property
     def values(self):
-        r"""ndarray: Get the field values as a 2D ndarray. It is formed as the array of
+        r"""array-likr: Get all the fields' values as a 2D array. It is formed as the array of
         :obj:`GribField.values <data.readers.grib.codes.GribField.values>` per field.
 
         See Also
         --------
-        to_numpy
+        to_array
 
 
         >>> import earthkit.data
         >>> ds = earthkit.data.from_source("file", "docs/examples/test.grib")
         >>> for f in ds:
         ...     print(f.values.shape)
         ...
@@ -704,40 +865,39 @@
         >>> v = ds.values
         >>> v.shape
         (2, 209)
         >>> v[0][:3]
         array([262.78027344, 267.44726562, 268.61230469])
 
         """
-        import numpy as np
-
-        return np.array([f.values for f in self])
+        x = [f.values for f in self]
+        return self._array_backend.array_ns.stack(x)
 
     def data(self, keys=("lat", "lon", "value"), flatten=False, dtype=None):
         r"""Return the values and/or the geographical coordinates.
 
         Only works when all the fields have the same grid geometry.
 
         Parameters
         ----------
         keys: :obj:`str`, :obj:`list` or :obj:`tuple`
             Specifies the type of data to be returned. Any combination of "lat", "lon" and "value"
             is allowed here.
         flatten: bool
             When it is True the "lat", "lon" arrays and the "value" arrays per field
             will all be flattened. Otherwise they will preserve the field's :obj:`shape`.
-        dtype: str, numpy.dtype or None
+        dtype: str, array.dtype or None
             Typecode or data-type of the arrays. When it is :obj:`None` the default
             type used by the underlying data accessor is used. For GRIB it is
-            ``np.float64``.
+            ``float64``.
 
         Returns
         -------
-        ndarray
-            The elements of the ndarray (in the order of the ``keys``) are as follows:
+        array-like
+            The elements of the array (in the order of the ``keys``) are as follows:
 
             * the latitudes array from the first field  when "lat" is in ``keys``
             * the longitudes array from the first field when "lon" is in ``keys``
             * a values array per field when "values" is in ``keys``
 
 
         Raises
@@ -774,38 +934,36 @@
         --------
         to_latlon
         to_points
         to_numpy
         values
 
         """
-        import numpy as np
-
         if self._is_shared_grid():
             if isinstance(keys, str):
                 keys = [keys]
 
             if "lat" in keys or "lon" in keys:
                 latlon = self[0].to_latlon(flatten=flatten, dtype=dtype)
 
             r = []
             for k in keys:
                 if k == "lat":
                     r.append(latlon["lat"])
                 elif k == "lon":
                     r.append(latlon["lon"])
                 elif k == "value":
-                    r.extend([f.to_numpy(flatten=flatten, dtype=dtype) for f in self])
+                    r.extend([f.to_array(flatten=flatten, dtype=dtype) for f in self])
                 else:
                     raise ValueError(f"data: invalid argument: {k}")
 
-            return np.array(r)
+            return self._array_backend.array_ns.stack(r)
 
         elif len(self) == 0:
-            return np.array([])
+            return self._array_backend.array_ns.stack([])
         else:
             raise ValueError("Fields do not have the same grid geometry")
 
     def metadata(self, *args, **kwargs):
         r"""Return the metadata values for each field.
 
         Parameters
@@ -1034,16 +1192,17 @@
         **kwargs: dict, optional
             Keyword arguments passed to
             :obj:`Field.to_points() <data.core.fieldlist.Field.to_points>`
 
         Returns
         -------
         dict
-            Dictionary with items "x" and "y", containing the ndarrays of the x and
-            y coordinates, respectively.
+            Dictionary with items "x" and "y", containing the arrays of the x and
+            y coordinates, respectively. The array format is specified by
+            :attr:`array_backend`.
 
         Raises
         ------
         ValueError
             When not all the fields have the same grid geometry.
         """
         if self._is_shared_grid():
@@ -1061,16 +1220,17 @@
         **kwargs: dict, optional
             Keyword arguments passed to
             :meth:`Field.to_latlon() <data.core.fieldlist.Field.to_latlon>`
 
         Returns
         -------
         dict
-            Dictionary with items "lat" and "lon", containing the ndarrays of the latitudes and
-            longitudes, respectively.
+            Dictionary with items "lat" and "lon", containing the arrays of the latitudes and
+            longitudes, respectively. The array format is specified by
+            :attr:`array_backend`.
 
         Raises
         ------
         ValueError
             When not all the fields have the same grid geometry
 
         Examples
@@ -1160,93 +1320,99 @@
             grid = self[0].metadata().geography._unique_grid_id()
             if grid is not None:
                 return all(
                     f.metadata().geography._unique_grid_id() == grid for f in self
                 )
         return False
 
+    @detect_out_filename
     def save(self, filename, append=False, **kwargs):
         r"""Write all the fields into a file.
 
         Parameters
         ----------
-        filename: str
-            The target file path.
-        append: bool
+        filename: str, optional
+            The target file path, if not defined attempts will be made to detect the filename
+        append: bool, optional
             When it is true append data to the target file. Otherwise
-            the target file be overwritten if already exists.
+            the target file be overwritten if already exists. Default is False
         **kwargs: dict, optional
             Other keyword arguments passed to :obj:`write`.
+
+        See Also
+        --------
+        :obj:`write`
+        :meth:`GribFieldList.save() <data.readers.grib.index.GribFieldList.save>`
+        :meth:`NumpyFieldList.save() <data.sources.numpy_list.NumpyFieldList.save>`
+
         """
         flag = "wb" if not append else "ab"
         with open(filename, flag) as f:
             self.write(f, **kwargs)
 
     def write(self, f, **kwargs):
         r"""Write all the fields to a file object.
 
         Parameters
         ----------
         f: file object
             The target file object.
         **kwargs: dict, optional
             Other keyword arguments passed to the underlying field implementation.
+
+        See Also
+        --------
+        read
+
         """
         for s in self:
             s.write(f, **kwargs)
 
-    def to_fieldlist(self, backend, **kwargs):
-        r"""Convert to a new :class:`FieldList` based on the ``backend``.
+    def to_fieldlist(self, array_backend=None, **kwargs):
+        r"""Convert to a new :class:`FieldList`.
 
         When the :class:`FieldList` is already in the required format no new
         :class:`FieldList` is created but the current one is returned.
 
         Parameters
         ----------
-        backend: str
-            Specifies the backend for the generated fieldlist. The supported values are as follows:
-
-            - "numpy": the generated fieldlist is a :class:`NumpyFieldList`, which represents
-              each field by an ndarray storing the field values and a :class:`MetaData` object holding
-              the field metadata. The shape and dtype of the ndarray is controlled by the ``kwargs``.
-              Please note that generated :class:`NumpyFieldList` stores all the field values in
-              a single ndarray.
+        array_backend: str, :obj:`ArrayBackend`
+            Specifies the array backend for the generated :class:`FieldList`. The array
+            type must be supported by :class:`ArrayBackend`.
 
         **kwargs: dict, optional
-            When ``backend`` is "numpy" ``kwargs`` are passed to :obj:`to_numpy` to
+            ``kwargs`` are passed to :obj:`to_array` to
             extract the field values the resulting object will store.
 
         Returns
         -------
         :class:`FieldList`
             - the current :class:`FieldList` if it is already in the required format
-            - :class:`NumpyFieldList` when ``backend`` is "numpy"
+            - a new :class:`ArrayFieldList` otherwise
 
         Examples
         --------
         The following example will convert a fieldlist read from a file into a
-        :class:`NumpyFieldList` storing single precision field values.
+        :class:`ArrayFieldList` storing single precision field values.
 
         >>> import numpy as np
         >>> import earthkit.data
         >>> ds = earthkit.data.from_source("file", "docs/examples/tuv_pl.grib")
         >>> ds.path
         'docs/examples/tuv_pl.grib'
-        >>> r = ds.to_fieldlist("numpy", dtype=np.float32)
+        >>> r = ds.to_fieldlist(array_backend="numpy", dtype=np.float32)
         >>> r
-        NumpyFieldList(fields=18)
+        ArrayFieldList(fields=18)
         >>> hasattr(r, "path")
         False
         >>> r.to_numpy().dtype
         dtype('float32')
 
         """
-        converter = fieldlist_converters.get(backend, None)
-        if converter is not None:
-            return getattr(self, converter)(**kwargs)
+        if array_backend is None:
+            array_backend = self._array_backend
+        array_backend = ensure_backend(array_backend)
+        return self._to_array_fieldlist(array_backend=array_backend, **kwargs)
 
-    def _to_numpy_fieldlist(self, **kwargs):
+    def _to_array_fieldlist(self, **kwargs):
         md = [f.metadata() for f in self]
-        return self.from_numpy(self.to_numpy(**kwargs), md)
-
-
-fieldlist_converters = {"numpy": "_to_numpy_fieldlist"}
+        return self.from_array(self.to_array(**kwargs), md)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/core/geography.py` & `earthkit_data-0.7.0/earthkit/data/core/geography.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/gridspec.py` & `earthkit_data-0.7.0/earthkit/data/core/gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/index.py` & `earthkit_data-0.7.0/earthkit/data/core/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 import functools
 import logging
 import math
 from abc import abstractmethod
 from collections import defaultdict
 
-import numpy as np
-
 import earthkit.data
 from earthkit.data.core.order import build_remapping, normalize_order_by
 from earthkit.data.core.select import normalize_selection, selection_from_index
 from earthkit.data.sources import Source
 
 LOG = logging.getLogger(__name__)
 
@@ -506,29 +504,37 @@
         indices = list(range(len(self)))
         indices = sorted(indices, key=functools.cmp_to_key(cmp))
         return self.new_mask_index(self, indices)
 
     def __getitem__(self, n):
         if isinstance(n, slice):
             return self.from_slice(n)
-        if isinstance(n, (tuple, list, np.ndarray)):
+        if isinstance(n, (tuple, list)):
             return self.from_multi(n)
         if isinstance(n, dict):
             return self.from_dict(n)
+        else:
+            import numpy as np
+
+            if isinstance(n, np.ndarray):
+                return self.from_multi(n)
+
         return self._getitem(n)
 
     def from_slice(self, s):
         indices = range(len(self))[s]
         return self.new_mask_index(self, indices)
 
     def from_mask(self, lst):
         indices = [i for i, x in enumerate(lst) if x]
         return self.new_mask_index(self, indices)
 
     def from_multi(self, a):
+        import numpy as np
+
         # will raise IndexError if an index is out of bounds
         n = len(self)
         indices = np.arange(0, n if n > 0 else 0)
         indices = indices[a].tolist()
         return self.new_mask_index(self, indices)
 
     def from_dict(self, dic):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/core/ipython.py` & `earthkit_data-0.7.0/earthkit/data/core/ipython.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/metadata.py` & `earthkit_data-0.7.0/earthkit/data/core/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,63 +29,120 @@
     DATA_FORMAT = None
     NAMESPACES = []
     LS_KEYS = []
     DESCRIBE_KEYS = []
     INDEX_KEYS = []
     CUSTOM_KEYS = [DATETIME, GRIDSPEC]
 
+    extra = None
+
     def __iter__(self):
         """Return an iterator over the metadata keys."""
         return iter(self.keys())
 
-    @abstractmethod
     def __len__(self):
         r"""Return the number of metadata entries."""
+        if not self.extra:
+            return self._len()
+        else:
+            extra = sum([1 for x in self.extra if not self._contains(x)])
+            return extra + self._len()
+
+    @abstractmethod
+    def _len(self):
+        r"""Return the number of metadata entries without the extra items."""
         pass
 
     def __getitem__(self, key):
         r"""Return the value for ``key``.
 
         Raises
         ------
         KeyError
             When ``key`` is not available.
         """
         return self.get(key, raise_on_missing=True)
 
-    @abstractmethod
     def __contains__(self, key):
         r"""Check if ``key`` is available.
 
         Returns
         -------
         bool
         """
-        pass
+        if not self.extra:
+            return self._contains(key)
+        else:
+            if key in self.extra:
+                return True
+            return self._contains(key)
 
     @abstractmethod
+    def _contains(self, key):
+        r"""Check if ``key`` is available in the non extra-keys.
+
+        Returns
+        -------
+        bool
+        """
+        pass
+
     def keys(self):
         r"""Return the metadata keys.
 
         Returns
         -------
         Iterable of str
 
         """
-        pass
+        if not self.extra:
+            return self._keys()
+        else:
+            extra = [x for x in self.extra if x not in self._keys()]
+            if len(extra) == 0:
+                return self._keys()
+            else:
+                r = list(self._keys()) + extra
+                return r
 
     @abstractmethod
+    def _keys(self):
+        r"""Return the metadata keys without the extra keys.
+
+        Returns
+        -------
+        Iterable of str
+
+        """
+        pass
+
     def items(self):
         r"""Return the metadata items.
 
         Returns
         -------
         Iterable of :obj:`(key,value)` pairs
 
         """
+        if not self.extra:
+            return self._items()
+        else:
+            r = dict(self._items())
+            r.update(self.extra)
+            return r.items()
+
+    @abstractmethod
+    def _items(self):
+        r"""Return the metadata items without the extra keys.
+
+        Returns
+        -------
+        Iterable of :obj:`(key,value)` pairs
+
+        """
         pass
 
     def get(self, key, default=None, *, astype=None, raise_on_missing=False):
         r"""Return the value for ``key``.
 
         Parameters
         ----------
@@ -111,27 +168,42 @@
         Raises
         ------
         KeyError
             If ``raise_on_missing`` is True and ``key`` is not found or it has
             a missing value.
 
         """
+        if self._is_extra_key(key):
+            return self._get_extra_key(key, default=default, astype=astype)
         if self._is_custom_key(key):
             return self._get_custom_key(
                 key, default=default, astype=astype, raise_on_missing=raise_on_missing
             )
         else:
             return self._get(
                 key, default=default, astype=astype, raise_on_missing=raise_on_missing
             )
 
     @abstractmethod
     def _get(self, key, astype=None, default=None, raise_on_missing=False):
         pass
 
+    def _is_extra_key(self, key):
+        return self.extra is not None and key in self.extra
+
+    def _get_extra_key(self, key, default=None, astype=None, **kwargs):
+        v = self.extra.get(key, default)
+
+        if astype is not None and v is not None:
+            try:
+                return astype(v)
+            except Exception:
+                return None
+        return v
+
     def _is_custom_key(self, key):
         return key in self.CUSTOM_KEYS and key not in self
 
     def _get_custom_key(self, key, default=None, raise_on_missing=True, **kwargs):
         if self._is_custom_key(key):
             try:
                 if key == DATETIME:
@@ -306,17 +378,23 @@
         d = dict(**self._d)
         d.update(*args, **kwargs)
         return RawMetadata(d)
 
     def __len__(self):
         return len(self._d)
 
+    def _len(self):
+        return self._len()
+
     def __contains__(self, key):
         return key in self._d
 
+    def _contains(self, key):
+        pass
+
     def _get(self, key, astype=None, default=None, raise_on_missing=False):
         if not raise_on_missing:
             v = self._d.get(key, default)
         else:
             v = self._d[key]
 
         if astype is not None:
@@ -325,17 +403,23 @@
             except Exception:
                 return None
         return v
 
     def keys(self):
         return self._d.keys()
 
+    def _keys(self):
+        pass
+
     def items(self):
         return self._d.items()
 
+    def _items(self):
+        pass
+
     def _base_datetime(self):
         return None
 
     def _valid_datetime(self):
         return None
 
     def as_namespace(self, namespace):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/core/order.py` & `earthkit_data-0.7.0/earthkit/data/core/order.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/plugins.py` & `earthkit_data-0.7.0/earthkit/data/core/plugins.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/select.py` & `earthkit_data-0.7.0/earthkit/data/core/select.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/settings.py` & `earthkit_data-0.7.0/earthkit/data/core/settings.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/statistics.py` & `earthkit_data-0.7.0/earthkit/data/core/statistics.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/temporary.py` & `earthkit_data-0.7.0/earthkit/data/core/temporary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/core/thread.py` & `earthkit_data-0.7.0/earthkit/data/core/thread.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/decorators.py` & `earthkit_data-0.7.0/earthkit/data/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 import functools
 import inspect
 import logging
 import os
 import re
 import threading
+import warnings
 
 from earthkit.data.utils import load_json_or_yaml
 from earthkit.data.utils.availability import Availability
 
 LOG = logging.getLogger(__name__)
 
 
@@ -31,14 +32,47 @@
                 m.append(q)
         p.update(kwargs)
         return func(*m, **p)
 
     return wrapped
 
 
+def detect_out_filename(func):
+    @functools.wraps(func)
+    def wrapped(self, *args, **kwargs):
+        # Detect filename:
+        if len(args) == 0:
+            for att in ["source_filename", "path"]:
+                if hasattr(self, att) and getattr(self, att) is not None:
+                    args = [os.path.basename(getattr(self, att))]
+                    break
+            else:
+                raise TypeError("Please provide an output filename")
+
+        # Ensure we do not overwrite file that is being read:
+        if (
+            args[0] is not None
+            and os.path.isfile(args[0])
+            and hasattr(self, "path")
+            and self.path is not None
+            and os.path.isfile(self.path)
+            and os.path.samefile(args[0], self.path)
+        ):
+            warnings.warn(
+                UserWarning(
+                    f"Earhtkit refusing to overwrite the file we are currently reading: {args[0]}"
+                )
+            )
+            return
+
+        return func(self, *args, **kwargs)
+
+    return wrapped
+
+
 LOCK = threading.RLock()
 
 
 def locked(func):
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         with LOCK:
```

### Comparing `earthkit-data-0.6.0/earthkit/data/indexing/__init__.py` & `earthkit_data-0.7.0/earthkit/data/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/indexing/database/__init__.py` & `earthkit_data-0.7.0/earthkit/data/indexing/database/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/indexing/database/json.py` & `earthkit_data-0.7.0/earthkit/data/indexing/database/json.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/indexing/database/sql.py` & `earthkit_data-0.7.0/earthkit/data/indexing/database/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from threading import local
 
 import numpy as np
 
 import earthkit.data
 from earthkit.data.core.order import build_remapping
 from earthkit.data.indexing.database.json import json_serialiser
-from earthkit.data.utils import tqdm
 from earthkit.data.utils.parts import Part
 
 from . import (
     FILEPARTS_KEY_NAMES,
     MORE_KEY_NAMES,
     MORE_KEY_NAMES_WITH_UNDERSCORE,
     STATISTICS_KEY_NAMES,
@@ -220,14 +219,15 @@
             self.path_table.insert(path, date)
 
         return count
 
     def build_sql_indexes(self):
         indexed_columns = [k for k, v in self.keys.items() if k.startswith("i_")]
         indexed_columns += ["path"]
+        from earthkit.data.utils.progbar import tqdm
 
         pbar = tqdm(indexed_columns, desc="Building indexes")
         for n in pbar:
             pbar.set_description(f"Building index for {n}")
             execute(
                 self.connection,
                 f"CREATE INDEX IF NOT EXISTS {n}_index ON {self.table_name} ({n});",
```

### Comparing `earthkit-data-0.6.0/earthkit/data/indexing/database/stdout.py` & `earthkit_data-0.7.0/earthkit/data/indexing/database/stdout.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/mergers/__init__.py` & `earthkit_data-0.7.0/earthkit/data/mergers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 
+from earthkit.data.readers import Reader
 from earthkit.data.sources.file import FileSource
 from earthkit.data.utils import string_to_args
 
 LOG = logging.getLogger(__name__)
 
-FORWARDS = ("to_xarray", "to_pandas", "to_tfdataset")
+FORWARDS = ("to_xarray", "to_pandas")
 
 
 def _nearest_common_class(objects):
     # mro() is "method resolution order"
     mros = [type(o).mro() for o in objects]
 
     first = mros[0]
@@ -54,18 +55,22 @@
 
         self.paths = None
         self.reader_class = None
         self.common = _nearest_common_class(sources)
         LOG.debug("nearest_common_class %s", self.common)
 
         if issubclass(self.common, FileSource):
+            # TODO: avoid calling _ methods
             readers = [s._reader for s in self.sources]
             self.reader_class = _nearest_common_class(readers)
             LOG.debug("nearest_common_class %s", self.reader_class)
             self.paths = [s.path for s in self.sources]
+        elif issubclass(self.common, Reader):
+            self.reader_class = self.common
+            self.paths = [s.path for s in self.sources]
 
     @property
     def paths_or_sources(self):
         if self.paths is not None:
             return self.paths
         return self.sources
 
@@ -77,24 +82,14 @@
         return merge(
             sources=self.sources,
             paths=self.paths,
             reader_class=self.reader_class,
             **kwargs,
         )
 
-    def to_tfdataset(self, **kwargs):
-        from .tfdataset import merge
-
-        return merge(
-            sources=self.sources,
-            paths=self.paths,
-            reader_class=self.reader_class,
-            **kwargs,
-        )
-
     def to_xarray(self, **kwargs):
         from .xarray import merge
 
         return merge(
             sources=self.sources,
             paths=self.paths,
             reader_class=self.reader_class,
@@ -109,29 +104,25 @@
 
     def to_xarray(self, *args, **kwargs):
         return self.obj.to_xarray(self.paths_or_sources, **kwargs)
 
     def to_pandas(self, *args, **kwargs):
         return self.obj.to_pandas(self.paths_or_sources, **kwargs)
 
-    def to_tfdataset(self, *args, **kwargs):
-        return self.obj.to_tfdataset(self.paths_or_sources, **kwargs)
-
 
 class CallableMerger(Merger):
     def __init__(self, func, sources, *args, **kwargs):
         super().__init__(sources)
         self.func = func
 
     def _call_func(self, *args, **kwargs):
         return self.func(self.paths_or_sources, **kwargs)
 
     to_xarray = _call_func
     to_pandas = _call_func
-    to_tfdataset = _call_func
 
 
 class XarrayGenericMerger(Merger):
     def __init__(self, sources, **options):
         super().__init__(sources)
         self.options = options
```

### Comparing `earthkit-data-0.6.0/earthkit/data/mergers/pandas.py` & `earthkit_data-0.7.0/earthkit/data/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/mergers/xarray.py` & `earthkit_data-0.7.0/earthkit/data/mergers/xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # since version 0.20, xarray checks the class and change os.PathLike to
 # strings. We don't want that, as we want to keep our objects
 class WrappedSource:
     def __init__(self, source):
         self.source = source
 
 
-class CMLEngine(BackendEntrypoint):
+class EKDEngine(BackendEntrypoint):
     @classmethod
     def open_dataset(cls, filename_or_obj, *args, **kwargs):
         assert isinstance(filename_or_obj, WrappedSource)
         return filename_or_obj.source.to_xarray()
 
 
 def infer_open_mfdataset_kwargs(
@@ -83,10 +83,10 @@
 
         LOG.debug(f"xr.open_mfdataset with options={options}")
         return xr.open_mfdataset(paths, **options)
 
     LOG.debug(f"xr.open_mfdataset with options= {options}")
     return xr.open_mfdataset(
         [WrappedSource(s) for s in sources],
-        engine=CMLEngine,
+        engine=EKDEngine,
         **options,
     )
```

### Comparing `earthkit-data-0.6.0/earthkit/data/mirrors/__init__.py` & `earthkit_data-0.7.0/earthkit/data/mirrors/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/mirrors/directory_mirror.py` & `earthkit_data-0.7.0/earthkit/data/mirrors/directory_mirror.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/__init__.py` & `earthkit_data-0.7.0/earthkit/data/readers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 import logging
 import os
 import weakref
 from importlib import import_module
 
 from earthkit.data.core import Base
 from earthkit.data.core.settings import SETTINGS
-from earthkit.data.decorators import locked
+from earthkit.data.decorators import detect_out_filename, locked
 
 LOG = logging.getLogger(__name__)
 
 
 class ReaderMeta(type(Base), type(os.PathLike)):
     pass
 
 
 class Reader(Base, os.PathLike, metaclass=ReaderMeta):
-    appendable = False  # Set to True if the data can be appened to and existing file
+    appendable = False  # Set to True if the data can be appended to and existing file
     binary = True
 
     def __init__(self, source, path):
         LOG.debug("Reader for %s is %s", path, self.__class__.__name__)
 
         self._source = weakref.ref(source)
         self.path = path
+        self.source_filename = self.source.source_filename
 
     @property
     def source(self):
         return self._source()
 
     @property
     def filter(self):
@@ -56,14 +57,15 @@
     def ignore(self):
         # Used by multi-source
         return False
 
     def cache_file(self, *args, **kwargs):
         return self.source.cache_file(*args, **kwargs)
 
+    @detect_out_filename
     def save(self, path, **kwargs):
         mode = "wb" if self.binary else "w"
         with open(path, mode) as f:
             self.write(f, **kwargs)
 
     def write(self, f, **kwargs):
         if not self.appendable:
@@ -79,14 +81,17 @@
     def __fspath__(self):
         return self.path
 
     def index_content(self):
         LOG.warning(f"index-content(): Ignoring {self.path}")
         return []
 
+    def ranges(self):
+        self.source._kw
+
 
 _READERS = {}
 
 
 # TODO: Add plugins
 @locked
 def _readers(method_name):
@@ -136,15 +141,15 @@
         "reader": UnknownReader,
         "stream_reader": UnknownStreamReader,
         "memory_reader": UnknownMemoryReader,
     }
     return unknowns[method_name](source, path_or_data, **kwargs)
 
 
-def reader(source, path, content_type=None):
+def reader(source, path, **kwargs):
     """Create the reader for a file/directory specified by path"""
     assert isinstance(path, str), source
 
     if hasattr(source, "reader"):
         reader = source.reader
         LOG.debug("Looking for a reader for %s (%s)", path, reader)
         if callable(reader):
@@ -160,39 +165,45 @@
 
     if os.path.isdir(path):
         from .directory import DirectoryReader
 
         return DirectoryReader(source, path).mutate()
     LOG.debug("Reader for %s", path)
 
+    if not os.path.exists(path):
+        raise FileExistsError(f"No such file exists: '{path}'")
+
+    if os.path.getsize(path) == 0:
+        raise Exception(f"File is empty: '{path}'")
+
     n_bytes = SETTINGS.get("reader-type-check-bytes")
     with open(path, "rb") as f:
         magic = f.read(n_bytes)
 
     LOG.debug("Looking for a reader for %s (%s)", path, magic)
 
     return _find_reader(
         "reader",
         source,
         path,
         magic=magic,
-        content_type=content_type,
+        **kwargs,
     )
 
 
-def memory_reader(source, buffer):
+def memory_reader(source, buffer, **kwargs):
     """Create a reader for data held in a memory buffer"""
     assert isinstance(buffer, (bytes, bytearray)), source
     n_bytes = SETTINGS.get("reader-type-check-bytes")
     magic = buffer[: min(n_bytes, len(buffer) - 1)]
 
-    return _find_reader("memory_reader", source, buffer, magic=magic)
+    return _find_reader("memory_reader", source, buffer, magic=magic, **kwargs)
 
 
-def stream_reader(source, stream, memory, content_type=None):
+def stream_reader(source, stream, memory, **kwargs):
     """Create a reader for a stream"""
     magic = None
     if hasattr(stream, "peek") and callable(stream.peek):
         try:
             n_bytes = SETTINGS.get("reader-type-check-bytes")
             magic = stream.peek(n_bytes)
             if len(magic) > n_bytes:
@@ -202,9 +213,9 @@
 
     return _find_reader(
         "stream_reader",
         source,
         stream,
         magic=magic,
         memory=memory,
-        content_type=content_type,
+        **kwargs,
     )
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/archive.py` & `earthkit_data-0.7.0/earthkit/data/readers/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 import os
 
-from earthkit.data.utils import tqdm
-
 from . import Reader
 from . import reader as find_reader
 
 LOG = logging.getLogger(__name__)
 
 
 class ArchiveReader(Reader):
@@ -56,14 +54,15 @@
 
     def expand(self, archive, members, **kwargs):
         def unpack(target, args):
             try:
                 os.mkdir(target)
             except FileExistsError:
                 pass
+            from earthkit.data.utils.progbar import tqdm
 
             for member in tqdm(iterable=members, total=len(members), leave=False):
                 if not self.check(member):
                     continue
                 archive.extract(member=member, path=target, **kwargs)
 
         try:
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/bufr/__init__.py` & `earthkit_data-0.7.0/earthkit/data/readers/bufr/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         if not deeper_check:
             return len(magic) >= 4 and magic[:4] == type_id
         else:
             return type_id in magic
     return False
 
 
-def reader(source, path, *, magic=None, deeper_check=False, **kwargs):
+def reader(source, path, *, magic=None, deeper_check=False, parts=None, **kwargs):
     if _match_magic(magic, deeper_check):
         from .bufr import BUFRReader
 
-        return BUFRReader(source, path)
+        return BUFRReader(source, path, parts=parts)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/bufr/bufr.py` & `earthkit_data-0.7.0/earthkit/data/readers/bufr/bufr.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,47 +41,46 @@
     "ident": "ident",
     "lat": "localLatitude",
     "lon": "localLongitude",
 }
 
 
 class BufrCodesMessagePositionIndex(CodesMessagePositionIndex):
+    MAGIC = b"BUFR"
+
     # This does not belong here, should be in the C library
-    def _get_message_positions(self, path):
-        fd = os.open(path, os.O_RDONLY)
-        try:
+    def _get_message_positions_part(self, fd, part):
+        assert part is not None
+        assert len(part) == 2
 
-            def get(count):
-                buf = os.read(fd, count)
-                assert len(buf) == count
-                return int.from_bytes(
-                    buf,
-                    byteorder="big",
-                    signed=False,
-                )
-
-            offset = 0
-            while True:
-                code = os.read(fd, 4)
-                if len(code) < 4:
-                    break
+        offset = part[0]
+        end_pos = part[0] + part[1] if part[1] > 0 else -1
+
+        if os.lseek(fd, offset, os.SEEK_SET) != offset:
+            return
+
+        while True:
+            code = os.read(fd, 4)
+            if len(code) < 4:
+                break
+
+            if code != self.MAGIC:
+                offset = os.lseek(fd, offset + 1, os.SEEK_SET)
+                continue
+
+            length = self._get_bytes(fd, 3)
+            edition = self._get_bytes(fd, 1)
+
+            if end_pos > 0 and offset + length > end_pos:
+                return
 
-                if code != b"BUFR":
-                    offset = os.lseek(fd, offset + 1, os.SEEK_SET)
-                    continue
-
-                length = get(3)
-                edition = get(1)
-
-                if edition in [3, 4]:
-                    yield offset, length
-                    offset = os.lseek(fd, offset + length, os.SEEK_SET)
+            if edition in [3, 4]:
+                yield offset, length
 
-        finally:
-            os.close(fd)
+            offset = os.lseek(fd, offset + length, os.SEEK_SET)
 
 
 class BUFRCodesHandle(CodesHandle):
     PRODUCT_ID = eccodes.CODES_PRODUCT_BUFR
 
     def __init__(self, handle, path, offset):
         super().__init__(handle, path, offset)
@@ -625,18 +624,14 @@
 
 class MultiBUFRList(BUFRList, MultiIndex):
     def __init__(self, *args, **kwargs):
         MultiIndex.__init__(self, *args, **kwargs)
 
 
 class BUFRInFiles(BUFRList):
-    # Remote BUFRLists (with urls) are also here,
-    # as the actual fieldlist is accessed on a file in cache.
-    # This class changes the interface (__getitem__ and __len__)
-    # into the interface (part and number_of_parts).
     def _getitem(self, n):
         if isinstance(n, int):
             part = self.part(n if n >= 0 else len(self) + n)
             return BUFRMessage(part.path, part.offset, part.length)
 
     def __len__(self):
         return self.number_of_parts()
@@ -647,39 +642,42 @@
 
     @abstractmethod
     def number_of_parts(self):
         self._not_implemented()
 
 
 class BUFRInOneFile(BUFRInFiles):
-    def __init__(self, path):
+    def __init__(self, path, parts=None):
         self.path = path
+        self._file_parts = parts
         self.__positions = None
 
     @property
     def _positions(self):
         if self.__positions is None:
-            self.__positions = BufrCodesMessagePositionIndex(self.path)
+            self.__positions = BufrCodesMessagePositionIndex(
+                self.path, parts=self._file_parts
+            )
         return self.__positions
 
     def part(self, n):
         return Part(self.path, self._positions.offsets[n], self._positions.lengths[n])
 
     def number_of_parts(self):
         return len(self._positions)
 
 
 class BUFRReader(BUFRInOneFile, Reader):
     """Represents a BUFR file"""
 
     appendable = True  # BUFR messages can be added to the same file
 
-    def __init__(self, source, path):
+    def __init__(self, source, path, parts=None):
         Reader.__init__(self, source, path)
-        BUFRInOneFile.__init__(self, path)
+        BUFRInOneFile.__init__(self, path, parts=parts)
 
     def __repr__(self):
         return "BUFRReader(%s)" % (self.path,)
 
     @classmethod
     def merge(cls, readers):
         assert all(isinstance(s, BUFRReader) for s in readers), readers
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/bufr/pandas.py` & `earthkit_data-0.7.0/earthkit/data/readers/bufr/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/covjson.py` & `earthkit_data-0.7.0/earthkit/data/readers/covjson.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 from earthkit.data.readers import Reader
 
 
 class XarrayMixIn:
     def to_xarray(self, **kwargs):
         try:
             from eccovjson.api import Eccovjson
-        except Exception:
-            raise ModuleNotFoundError(
-                "this feature requires 'eccovjson' to be installed!"
-            )
+        except ImportError:
+            raise ImportError("covjason handling requires 'eccovjson' to be installed")
 
         decoder = Eccovjson().decode(self._json())
         return decoder.to_xarray()
 
 
 class CovjsonReader(XarrayMixIn, Reader):
     def __init__(self, source, path):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/csv.py` & `earthkit_data-0.7.0/earthkit/data/readers/csv.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/directory.py` & `earthkit_data-0.7.0/earthkit/data/readers/directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,9 +87,9 @@
         shutil.copytree(self.path, path)
 
     def write(self, f, **kwargs):
         raise NotImplementedError()
 
 
 def reader(source, path, *, magic=None, deeper_check=False, **kwargs):
-    if magic is None or os.path.isdir(path):
+    if magic is None and os.path.isdir(path):
         return DirectoryReader(source, path)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/geojson.py` & `earthkit_data-0.7.0/earthkit/data/readers/geojson.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,15 +87,18 @@
         return self.to_pandas(**kwargs)
 
     def to_xarray(self, **kwargs):
         return self.to_pandas(**kwargs).to_xarray()
 
     @classmethod
     def to_pandas_from_multi_paths(cls, paths, **kwargs):
-        import geopandas as gpd
+        try:
+            import geopandas as gpd
+        except ImportError:
+            raise ImportError("Geojson handling requires 'geopandas' to be installed")
 
         geo_df = gpd.pd.concat([gpd.read_file(path, **kwargs) for path in paths])
 
         return geo_df.set_index(np.arange(len(geo_df)))
 
     def _to_geopandas_dataframe_wrapper(self, **kwargs):
         return GeoPandasDataFrameWrapper(self.to_pandas(**kwargs))
@@ -103,9 +106,9 @@
 
 def reader(source, path, *, magic=None, deeper_check=False, **kwargs):
     kind, compression = mimetypes.guess_type(path)
     ext = path.split(".")[-1]
 
     geojson_extensions = ["geojson"]
     geojson_mimetypes = ["application/geo+json"]
-    if magic is None or ext in geojson_extensions or kind in geojson_mimetypes:
+    if ext in geojson_extensions or kind in geojson_mimetypes:
         return GeojsonReader(source, path)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/__init__.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,38 +23,40 @@
 
 def _is_default(magic, content_type):
     return (magic is None or len(magic) == 0) and (
         content_type is None or len(content_type) == 0
     )
 
 
-def reader(source, path, *, magic=None, deeper_check=False, **kwargs):
+def reader(source, path, *, magic=None, deeper_check=False, parts=None, **kwargs):
     if _match_magic(magic, deeper_check):
         from .reader import GRIBReader
 
-        return GRIBReader(source, path)
+        return GRIBReader(source, path, parts=parts)
 
 
 def memory_reader(source, buffer, *, magic=None, deeper_check=False, **kwargs):
     if _match_magic(magic, deeper_check):
         from .memory import GribFieldListInMemory, GribMessageMemoryReader
 
-        return GribFieldListInMemory(source, GribMessageMemoryReader(buffer))
+        return GribFieldListInMemory(
+            source, GribMessageMemoryReader(buffer, **kwargs), **kwargs
+        )
 
 
 def stream_reader(
     source,
     stream,
     magic=None,
     *,
     deeper_check=False,
     content_type=None,
     memory=False,
-    **kwargs
+    **kwargs,
 ):
     if _is_default(magic, content_type) or _match_magic(magic, deeper_check):
         from .memory import GribFieldListInMemory, GribStreamReader
 
-        r = GribStreamReader(stream)
+        r = GribStreamReader(stream, **kwargs)
         if memory:
-            r = GribFieldListInMemory(source, r)
+            r = GribFieldListInMemory(source, r, **kwargs)
         return r
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/codes.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/codes.py`

 * *Files 15% similar despite different names*

```diff
@@ -80,72 +80,70 @@
 
 VALUE_ACCESSOR = GribCodesValueAccessor()
 LATITUDE_ACCESSOR = GribCodesLatitudeAccessor()
 LONGITUDE_ACCESSOR = GribCodesLongitudeAccessor()
 
 
 class GribCodesMessagePositionIndex(CodesMessagePositionIndex):
-    # This does not belong here, should be in the C library
-    def _get_message_positions(self, path):
-        fd = os.open(path, os.O_RDONLY)
-        try:
+    MAGIC = b"GRIB"
 
-            def get(count):
-                buf = os.read(fd, count)
-                assert len(buf) == count
-                return int.from_bytes(
-                    buf,
-                    byteorder="big",
-                    signed=False,
-                )
-
-            offset = 0
-            while True:
-                code = os.read(fd, 4)
-                if len(code) < 4:
-                    break
-
-                if code != b"GRIB":
-                    offset = os.lseek(fd, offset + 1, os.SEEK_SET)
-                    continue
-
-                length = get(3)
-                edition = get(1)
-
-                if edition == 1:
-                    if length & 0x800000:
-                        sec1len = get(3)
-                        os.lseek(fd, 4, os.SEEK_CUR)
-                        flags = get(1)
-                        os.lseek(fd, sec1len - 8, os.SEEK_CUR)
-
-                        if flags & (1 << 7):
-                            sec2len = get(3)
-                            os.lseek(fd, sec2len - 3, os.SEEK_CUR)
-
-                        if flags & (1 << 6):
-                            sec3len = get(3)
-                            os.lseek(fd, sec3len - 3, os.SEEK_CUR)
-
-                        sec4len = get(3)
-
-                        if sec4len < 120:
-                            length &= 0x7FFFFF
-                            length *= 120
-                            length -= sec4len
-                            length += 4
+    # This does not belong here, should be in the C library
+    def _get_message_positions_part(self, fd, part):
+        assert part is not None
+        assert len(part) == 2
+
+        offset = part[0]
+        end_pos = part[0] + part[1] if part[1] > 0 else -1
+
+        if os.lseek(fd, offset, os.SEEK_SET) != offset:
+            return
+
+        while True:
+            code = os.read(fd, 4)
+            if len(code) < 4:
+                break
+
+            if code != self.MAGIC:
+                offset = os.lseek(fd, offset + 1, os.SEEK_SET)
+                continue
+
+            length = self._get_bytes(fd, 3)
+            edition = self._get_bytes(fd, 1)
+
+            if edition == 1:
+                if length & 0x800000:
+                    sec1len = self._get_bytes(fd, 3)
+                    os.lseek(fd, 4, os.SEEK_CUR)
+                    flags = self._get_bytes(fd, 1)
+                    os.lseek(fd, sec1len - 8, os.SEEK_CUR)
+
+                    if flags & (1 << 7):
+                        sec2len = self._get_bytes(fd, 3)
+                        os.lseek(fd, sec2len - 3, os.SEEK_CUR)
+
+                    if flags & (1 << 6):
+                        sec3len = self._get_bytes(fd, 3)
+                        os.lseek(fd, sec3len - 3, os.SEEK_CUR)
+
+                    sec4len = self._get_bytes(fd, 3)
+
+                    if sec4len < 120:
+                        length &= 0x7FFFFF
+                        length *= 120
+                        length -= sec4len
+                        length += 4
 
-                if edition == 2:
-                    length = get(8)
+            if edition == 2:
+                length = self._get_bytes(fd, 8)
 
-                yield offset, length
-                offset = os.lseek(fd, offset + length, os.SEEK_SET)
+            if end_pos > 0 and offset + length > end_pos:
+                return
 
-        finally:
-            os.close(fd)
+            yield offset, length
+            offset = os.lseek(fd, offset + length, os.SEEK_SET)
 
 
 class GribCodesHandle(CodesHandle):
     PRODUCT_ID = eccodes.CODES_PRODUCT_GRIB
 
     # TODO: just a wrapper around the base class implementation to handle the
     # s,l,d qualifiers. Once these are implemented in the base class this method can
@@ -243,16 +241,16 @@
         Path to the GRIB file
     offset: number
         File offset of the message (in bytes)
     length: number
         Size of the message (in bytes)
     """
 
-    def __init__(self, path, offset, length):
-        super().__init__()
+    def __init__(self, path, offset, length, backend):
+        super().__init__(backend)
         self.path = path
         self._offset = offset
         self._length = length
         self._handle = None
 
     @property
     def handle(self):
@@ -289,24 +287,33 @@
     #     """Private, for testing only"""
     #     # paramId is renamed as param to get rid of the
     #     # additional '.128' (in earthkit/data/scripts/grib.py)
     #     if name == "param":
     #         name = "paramId"
     #     return self.handle.get(name)
 
-    def write(self, f):
+    def write(self, f, bits_per_value=None):
         r"""Writes the message to a file object.
 
         Parameters
         ----------
         f: file object
             The target file object.
+        bits_per_value: int or None
+            Set the ``bitsPerValue`` GRIB key in the generated GRIB message. When
+            None the ``bitsPerValue`` stored in the metadata will be used.
         """
+        if bits_per_value is not None:
+            handle = self.handle.clone()
+            handle.set_long("bitsPerValue", bits_per_value)
+        else:
+            handle = self.handle
+
         # assert isinstance(f, io.IOBase)
-        self.handle.write_to(f)
+        handle.write_to(f)
 
     def message(self):
         r"""Returns a buffer containing the encoded message.
 
         Returns
         -------
         bytes
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/gridspec.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/index/__init__.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/index/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 import logging
 import math
 import os
 from abc import abstractmethod
 
 from earthkit.data.core.fieldlist import FieldList
-from earthkit.data.core.index import Index, MaskIndex, MultiIndex
-from earthkit.data.decorators import alias_argument
+from earthkit.data.core.index import MaskIndex, MultiIndex
+from earthkit.data.decorators import alias_argument, detect_out_filename
 from earthkit.data.indexing.database import (
     FILEPARTS_KEY_NAMES,
     MORE_KEY_NAMES,
     MORE_KEY_NAMES_WITH_UNDERSCORE,
     STATISTICS_KEY_NAMES,
 )
 from earthkit.data.readers.grib.codes import GribField
 from earthkit.data.readers.grib.pandas import PandasMixIn
 from earthkit.data.readers.grib.xarray import XarrayMixIn
-from earthkit.data.utils import progress_bar
 from earthkit.data.utils.availability import Availability
+from earthkit.data.utils.progbar import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 
 class GribFieldList(PandasMixIn, XarrayMixIn, FieldList):
     r"""Represents a list of :obj:`GribField <data.readers.grib.codes.GribField>`\ s.
 
@@ -105,27 +105,36 @@
 
     def __init__(self, *args, **kwargs):
         if self.availability_path is not None and os.path.exists(
             self.availability_path
         ):
             self._availability = Availability(self.availability_path)
 
-        Index.__init__(self, *args, **kwargs)
+        # Index.__init__(self, *args, **kwargs)
+        FieldList.__init__(self, *args, **kwargs)
 
     @classmethod
-    def new_mask_index(self, *args, **kwargs):
+    def new_mask_index(cls, *args, **kwargs):
         return GribMaskFieldList(*args, **kwargs)
 
     @property
     def availability_path(self):
         return None
 
     @classmethod
     def merge(cls, sources):
-        assert all(isinstance(_, GribFieldList) for _ in sources)
+        if not all(isinstance(_, GribFieldList) for _ in sources):
+            raise ValueError(
+                "GribFieldList can only be merged to another GribFieldLists"
+            )
+        if not all(s.array_backend is s[0].array_backend for s in sources):
+            raise ValueError(
+                "Only fieldlists with the same array backend can be merged"
+            )
+
         return GribMultiFieldList(sources)
 
     def _custom_availability(self, ignore_keys=None, filter_keys=lambda k: True):
         def dicts():
             for i in progress_bar(
                 iterable=range(len(self)), desc="Building availability"
             ):
@@ -175,34 +184,59 @@
     @alias_argument("levtype", ["leveltype"])
     @alias_argument("param", ["variable", "parameter"])
     @alias_argument("number", ["realization", "realisation"])
     @alias_argument("class", "klass")
     def _normalize_kwargs_names(self, **kwargs):
         return kwargs
 
+    @detect_out_filename
+    def save(self, filename, append=False, bits_per_value=None):
+        r"""Write all the fields into a file.
+
+        Parameters
+        ----------
+        filename: str
+            The target file path.
+        append: bool
+            When it is true append data to the target file. Otherwise
+            the target file be overwritten if already exists.
+        bits_per_value: int or None
+            Set the ``bitsPerValue`` GRIB key for each message in the generated
+            output. When None the ``bitsPerValue`` stored in the message metadata
+            will be used.
+
+        See Also
+        --------
+        write
+
+        """
+        super().save(
+            filename,
+            append=append,
+            bits_per_value=bits_per_value,
+        )
+
 
 class GribMaskFieldList(GribFieldList, MaskIndex):
     def __init__(self, *args, **kwargs):
         MaskIndex.__init__(self, *args, **kwargs)
+        FieldList._init_from_mask(self, self)
 
 
 class GribMultiFieldList(GribFieldList, MultiIndex):
     def __init__(self, *args, **kwargs):
         MultiIndex.__init__(self, *args, **kwargs)
+        FieldList._init_from_multi(self, self)
 
 
 class GribFieldListInFiles(GribFieldList):
-    # Remote FieldLists (with urls) are also here,
-    # as the actual fieldlist is accessed on a file in cache.
-    # This class changes the interface (__getitem__ and __len__)
-    # into the interface (part and number_of_parts).
     def _getitem(self, n):
         if isinstance(n, int):
             part = self.part(n if n >= 0 else len(self) + n)
-            return GribField(part.path, part.offset, part.length)
+            return GribField(part.path, part.offset, part.length, self.array_backend)
 
     def __len__(self):
         return self.number_of_parts()
 
     @abstractmethod
     def part(self, n):
         self._not_implemented()
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/index/db.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/index/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 
 import json
 import logging
 import os
 from urllib.parse import urljoin
 
-from earthkit.data.core.caching import CACHE, cache_file
+from earthkit.data.core.caching import cache_file
 from earthkit.data.readers.grib.index import GribFieldListInFiles
-from earthkit.data.utils import progress_bar
+from earthkit.data.utils.progbar import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 
 class FieldListInFilesWithDBIndex(GribFieldListInFiles):
     def __init__(self, db, **kwargs):
         """Should not be instantiated directly.
@@ -51,17 +51,14 @@
         **kwargs,
     ):
         def load(target, *args):
             LOG.debug(f"Building db in {target}")
             db = cls.DBCLASS(target)
             db.load_iterator(iterator)
 
-        if not CACHE.policy.managed():
-            raise RuntimeError("Cannot perform grib indexing when caching is disabled")
-
         db_name = cache_file(
             "grib-index",
             load,
             cache_metadata,
             hash_extra=cls.DBCLASS.VERSION,
             extension=cls.DBCLASS.EXTENSION,
         )
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/index/file.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/index/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 class GribFieldListInOneFile(GribFieldListInFiles):
     VERSION = 1
 
     @property
     def availability_path(self):
         return os.path.join(self.path, ".availability.pickle")
 
-    def __init__(self, path, **kwargs):
+    def __init__(self, path, parts=None, **kwargs):
         assert isinstance(path, str), path
 
         self.path = path
+        self._file_parts = parts
         self.__positions = None
         super().__init__(**kwargs)
 
     @property
     def _positions(self):
         if self.__positions is None:
-            self.__positions = GribCodesMessagePositionIndex(self.path)
+            self.__positions = GribCodesMessagePositionIndex(
+                self.path, self._file_parts
+            )
         return self.__positions
 
     def part(self, n):
         return Part(self.path, self._positions.offsets[n], self._positions.lengths[n])
 
     def number_of_parts(self):
-        return len(self._positions.offsets)
+        return len(self._positions)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/index/json.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/index/json.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/index/sql.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/index/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/memory.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 import logging
 
 import eccodes
 
 from earthkit.data.readers import Reader
 from earthkit.data.readers.grib.codes import GribCodesHandle, GribField
 from earthkit.data.readers.grib.index import GribFieldList
+from earthkit.data.utils.array import ensure_backend
 
 LOG = logging.getLogger(__name__)
 
 
 class GribMemoryReader(Reader):
-    def __init__(self):
+    def __init__(self, array_backend=None):
         self._peeked = None
+        self._array_backend = ensure_backend(array_backend)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self._peeked is not None:
             msg = self._peeked
@@ -37,15 +39,17 @@
         raise StopIteration
 
     def _next_handle(self):
         raise NotImplementedError
 
     def _message_from_handle(self, handle):
         if handle is not None:
-            return GribFieldInMemory(GribCodesHandle(handle, None, None))
+            return GribFieldInMemory(
+                GribCodesHandle(handle, None, None), self._array_backend
+            )
 
     def peek(self):
         """Returns the next available message without consuming it"""
         if self._peeked is None:
             handle = self._next_handle()
             self._peeked = self._message_from_handle(handle)
         return self._peeked
@@ -83,28 +87,28 @@
             else:
                 raise StopIteration
 
         return GribFieldListInMemory.from_fields(fields)
 
 
 class GribFileMemoryReader(GribMemoryReader):
-    def __init__(self, path):
-        super().__init__()
+    def __init__(self, path, **kwargs):
+        super().__init__(**kwargs)
         self.fp = open(path, "rb")
 
     def __del__(self):
         self.fp.close()
 
     def _next_handle(self):
         return eccodes.codes_new_from_file(self.fp, eccodes.CODES_PRODUCT_GRIB)
 
 
 class GribMessageMemoryReader(GribMemoryReader):
-    def __init__(self, buf):
-        super().__init__()
+    def __init__(self, buf, **kwargs):
+        super().__init__(**kwargs)
         self.buf = buf
 
     def __del__(self):
         self.buf = None
 
     def _next_handle(self):
         if self.buf is None:
@@ -117,15 +121,15 @@
 class GribStreamReader(GribMemoryReader):
     """Wrapper around eccodes.Streamreader. The problem is that when iterating via
     the StreamReader it returns an eccodes.GRIBMessage that releases the handle when deleted.
     However, the handle has to be managed by earthkit-data so we access it directly
     using _next_handle
     """
 
-    def __init__(self, stream):
+    def __init__(self, stream, **kwargs):
         super().__init__()
         self._stream = stream
         self._reader = eccodes.StreamReader(stream)
 
     def __del__(self):
         self._stream.close()
 
@@ -138,16 +142,16 @@
     def mutate_source(self):
         return self
 
 
 class GribFieldInMemory(GribField):
     """Represents a GRIB message in memory"""
 
-    def __init__(self, handle):
-        super().__init__(None, None, None)
+    def __init__(self, handle, array_backend=None):
+        super().__init__(None, None, None, array_backend)
         self._handle = handle
 
     @GribField.handle.getter
     def handle(self):
         return self._handle
 
     @GribField.handle.getter
@@ -155,16 +159,18 @@
         return None
 
 
 class GribFieldListInMemory(GribFieldList, Reader):
     """Represent a GRIB field list in memory"""
 
     @staticmethod
-    def from_fields(fields):
-        fs = GribFieldListInMemory(None, None)
+    def from_fields(fields, array_backend=None):
+        if array_backend is None and len(fields) > 0:
+            array_backend = fields[0].array_backend
+        fs = GribFieldListInMemory(None, None, array_backend=array_backend)
         fs._fields = fields
         fs._loaded = True
         return fs
 
     def __init__(self, source, reader, *args, **kwargs):
         """
         The reader must support __next__.
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/metadata.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # nor does it submit to any jurisdiction.
 #
 
 import datetime
 
 from earthkit.data.core.geography import Geography
 from earthkit.data.core.metadata import Metadata
+from earthkit.data.decorators import cached_method
 from earthkit.data.indexing.database import GRIB_KEYS_NAMES
 from earthkit.data.readers.grib.gridspec import make_gridspec
 from earthkit.data.utils.bbox import BoundingBox
 from earthkit.data.utils.projections import Projection
 
 
 def missing_is_none(x):
@@ -203,43 +204,45 @@
         "vertical",
     ]
 
     DATA_FORMAT = "grib"
 
     __handle_type = None
 
-    def __init__(self, handle):
+    def __init__(self, handle, extra=None):
         if not isinstance(handle, self._handle_type()):
             raise TypeError(
                 f"GribMetadata: expected handle type {self._handle_type()}, got {type(handle)}"
             )
         self._handle = handle
         self._geo = None
+        if extra is not None:
+            self.extra = extra
 
     @staticmethod
     def _handle_type():
         """Return the expected handle type. Implemented like this
         to avoid cyclic import
         """
         if GribMetadata.__handle_type is None:
             from earthkit.data.readers.grib.codes import GribCodesHandle
 
             GribMetadata.__handle_type = GribCodesHandle
         return GribMetadata.__handle_type
 
-    def __len__(self):
-        return sum(map(lambda i: 1, self.keys()))
+    def _len(self):
+        return sum(map(lambda i: 1, self._keys()))
 
-    def __contains__(self, key):
+    def _contains(self, key):
         return self._handle.__contains__(key)
 
-    def keys(self):
+    def _keys(self):
         return self._handle.keys()
 
-    def items(self):
+    def _items(self):
         return self._handle.items()
 
     def _get(self, key, astype=None, default=None, raise_on_missing=False):
         def _key_name(key):
             if key == "param":
                 key = "shortName"
             elif key == "_param_id":
@@ -255,39 +258,46 @@
     def _is_custom_key(self, key):
         return key in self.CUSTOM_KEYS
 
     def override(self, *args, **kwargs):
         d = dict(*args, **kwargs)
 
         new_value_size = None
+        extra = None
         gridspec = d.pop("gridspec", None)
         if gridspec is not None:
             from earthkit.data.readers.grib.gridspec import GridSpecConverter
 
             edition = d.get("edition", self["edition"])
             md, new_value_size = GridSpecConverter.to_metadata(
                 gridspec, edition=edition
             )
             d.update(md)
 
-            # at the moment we cannot use headers_only clone when setting the
-            # geography
-            handle = self._handle.clone()
-        else:
-            handle = self._handle.clone(headers_only=True)
+        handle = self._handle.clone(headers_only=True)
+        # whether headers_only=True works depends on the eccCodes version and the
+        # message properties. We check it by comparing the message lengths.
+        shrunk = handle.get_long("totalLength") < self._handle.get_long("totalLength")
+
+        # some keys, needed later, are not copied into the clone when
+        # headers_only=True. We store them as extra keys.
+        if shrunk:
+            extra = {"bitsPerValue": self._handle.get("bitsPerValue", default=0)}
 
         handle.set_multiple(d)
 
+        # we need to set the values to the new size otherwise the clone generated
+        # with headers_only=True will be inconsistent
         if new_value_size is not None and new_value_size > 0:
             import numpy as np
 
             vals = np.zeros(new_value_size)
             handle.set_values(vals)
 
-        return GribMetadata(handle)
+        return GribMetadata(handle, extra=extra)
 
     def as_namespace(self, namespace=None):
         r"""Return all the keys/values from a namespace.
 
         Parameters
         ----------
         namespace: str, None
@@ -388,14 +398,17 @@
 
 
 # TODO: this is a temporary solution
 class RestrictedGribMetadata(GribMetadata):
     """Hide internal keys and namespaces in GRIB metadata"""
 
     EKD_NAMESPACE = "grib"
+
+    # ideally bitsPerValue should be here. However, it is treated as an
+    # extra key and cannot be an internal key.
     INTERNAL_KEYS = [
         "minimum",
         "maximum",
         "average",
         "standardDeviation",
         "skewness",
         "kurtosis",
@@ -406,69 +419,72 @@
         "skew",
         "kurt",
         "const",
         "isConstant",
         "numberOfMissing",
         "numberOfCodedValues",
         "bitmapPresent",
-        "bitsPerValue",
         "offsetValuesBy",
         "packingError",
         "referenceValue",
         "referenceValueError",
         "unpackedError",
         "values",
     ]
     INTERNAL_NAMESPACES = ["statistics"]
 
     def __init__(self, md):
-        super().__init__(md._handle)
+        super().__init__(md._handle, extra=md.extra)
 
-    def __len__(self):
+    @cached_method
+    def _len(self):
         if self.INTERNAL_KEYS:
-            return len(self.keys())
+            # NOTE: argumentless super cannot be used in list comprehension
+            m = super()._contains
+            surplus = [1 for x in self.INTERNAL_KEYS if not m(x)]
+            return super()._len() + len(surplus)
         else:
-            return super().__len__()
+            return super()._len()
 
     def _is_internal(self, key):
         ns, _, name = key.partition(".")
         if name == "":
             name = key
             ns = ""
 
         if ns == self.EKD_NAMESPACE:
             return False
         else:
             return name in self.INTERNAL_KEYS
 
-    def __contains__(self, key):
+    def _contains(self, key):
         if self.INTERNAL_KEYS:
-            return not self._is_internal(key) and super().__contains__(key)
+            return not self._is_internal(key) and super()._contains(key)
         else:
-            return super().__contains__(key)
+            return super()._contains(key)
 
-    def keys(self):
+    def _keys(self):
         if self.INTERNAL_KEYS:
             r = []
-            for k in super().keys():
+            for k in super()._keys():
                 if k not in self.INTERNAL_KEYS:
                     r.append(k)
             return r
         else:
-            return super().keys()
+            return super()._keys()
 
-    def items(self):
+    def _items(self):
         if self.INTERNAL_KEYS:
             r = {}
-            for k, v in super().items():
+            for k, v in super()._items():
                 if k not in self.INTERNAL_KEYS:
                     r[k] = v
             return r.items()
         else:
-            return super().items()
+            return super()._items()
 
     def get(self, key, default=None, *, astype=None, raise_on_missing=False):
         ns, _, name = key.partition(".")
         if name == "":
             name = key
             ns = ""
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/output.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 _ORDER = (
     "edition",
     "setLocalDefinition",
     "typeOfGeneratingProcess",
     "productDefinitionTemplateNumber",
 )
 
+NOT_IN_EDITION_1 = (
+    "productDefinitionTemplateNumber",
+    "typeOfGeneratingProcess",
+)
+
+
 ORDER = {}
 for i, k in enumerate(_ORDER):
     ORDER[k] = i
 
 
 def order(key):
     ORDER.setdefault(key, len(ORDER))
@@ -39,14 +45,15 @@
 
 class Combined:
     def __init__(self, handle, metadata):
         self.handle = handle
         self.metadata = metadata
 
     def __contains__(self, key):
+        # return key in self.metadata or key in self.handle
         raise NotImplementedError()
 
     def __getitem__(self, key):
         if key in self.metadata:
             return self.metadata[key]
         return self.handle.get(key, default=None)
 
@@ -91,51 +98,56 @@
         # Make a copy as we may modify it
         md = self._normalize_kwargs_names(**self.kwargs)
         md.update(self._normalize_kwargs_names(**metadata))
         md.update(self._normalize_kwargs_names(**kwargs))
 
         metadata = md
 
-        compulsory = ("date", ("param", "paramId", "shortName"))
+        compulsory = (("date", "referenceDate"), ("param", "paramId", "shortName"))
 
         if template is None:
             template = self.template
 
         if template is None:
             handle = self.handle_from_metadata(values, metadata, compulsory)
         else:
             handle = template.handle.clone()
 
         # print("->", metadata)
         self.update_metadata(handle, metadata, compulsory)
         # print("<-", metadata)
 
-        if check_nans:
+        if check_nans and values is not None:
             import numpy as np
 
             if np.isnan(values).any():
                 # missing_value = np.finfo(values.dtype).max
                 missing_value = 9999
                 values = np.nan_to_num(values, nan=missing_value)
                 metadata["missingValue"] = missing_value
                 metadata["bitmapPresent"] = 1
 
         metadata = {
             k: v for k, v in sorted(metadata.items(), key=lambda x: order(x[0]))
         }
 
+        if str(metadata.get("edition")) == "1":
+            for k in NOT_IN_EDITION_1:
+                metadata.pop(k, None)
+
         if "generatingProcessIdentifier" not in metadata:
             metadata["generatingProcessIdentifier"] = 255
 
         LOG.debug("GribOutput.metadata %s", metadata)
 
         for k, v in metadata.items():
             handle.set(k, v)
 
-        handle.set_values(values)
+        if values is not None:
+            handle.set_values(values)
 
         file, path = self.f(handle)
         handle.write(file)
 
         return handle, path
 
     def close(self):
@@ -148,15 +160,15 @@
     def __exit__(self, exc_type, exc_value, trace):
         self.close()
 
     def update_metadata(self, handle, metadata, compulsory):
         # TODO: revisit that logic
         combined = Combined(handle, metadata)
 
-        if "step" in metadata:
+        if "step" in metadata or "endStep" in metadata:
             if combined["type"] == "an":
                 metadata["type"] = "fc"
 
         if "time" in metadata:  # TODO, use a normalizer
             try:
                 time = int(metadata["time"])
                 if time < 100:
@@ -319,14 +331,15 @@
             213988: (200, False),
             348528: (256, False),
             542080: (320, False),
             843490: (400, False),
             1373624: (512, False),
             2140702: (640, False),
             5447118: (1024, False),
+            6599680: (1280, True),
             8505906: (1280, False),
             20696844: (2000, False),
         }
 
         n = len(values)
         if n not in GAUSSIAN:
             raise ValueError(f"Unsupported GAUSSIAN grid. Number of grid points {n:,}")
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/pandas.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/parsing.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/parsing.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/grib/xarray.py` & `earthkit_data-0.7.0/earthkit/data/readers/grib/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/numpy.py` & `earthkit_data-0.7.0/earthkit/data/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/odb.py` & `earthkit_data-0.7.0/earthkit/data/readers/odb.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 
 class ODBReader(Reader):
     def to_pandas(self, **kwargs):
         try:
             import codc as odc
         except Exception:
-            import pyodc as odc
-
+            try:
+                import pyodc as odc
+            except ImportError:
+                raise ImportError("ODC handling requires 'pyodc' to be installed")
             LOG.debug("Using pure Python odc decoder.")
 
         odc_read_odb_kwargs = kwargs.get("odc_read_odb_kwargs", {})
         return odc.read_odb(self.path, single=True, **odc_read_odb_kwargs)
 
 
 def _match_magic(magic, deeper_check):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/tar.py` & `earthkit_data-0.7.0/earthkit/data/readers/tar.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/text.py` & `earthkit_data-0.7.0/earthkit/data/readers/text.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/readers/zip.py` & `earthkit_data-0.7.0/earthkit/data/readers/zip.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/__init__.py` & `earthkit_data-0.7.0/earthkit/data/sources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     licence = "-"
     documentation = "-"
     citation = "-"
 
     _dataset = None
     _parent = None
 
+    source_filename = None
+
     def __init__(self, **kwargs):
         self._kwargs = kwargs
 
     def settings(self, name):
         return SETTINGS.get(name)
 
     def mutate(self):
@@ -113,23 +115,24 @@
         return entry.source
 
     def load_remote(self, name):
         return None
 
 
 class SourceMaker:
+    SOURCES = {}
+
     def __call__(self, name, *args, **kwargs):
         loader = SourceLoader()
 
-        klass = find_plugin(os.path.dirname(__file__), name, loader)
-
-        # if os.environ.get("FIEDLIST_TESTING_ENABLE_MOCKUP_SOURCE", False):
-        #     from earthkit.data.mockup import SourceMockup
-
-        #     klass = SourceMockup
+        if name in self.SOURCES:
+            klass = self.SOURCES[name]
+        else:
+            klass = find_plugin(os.path.dirname(__file__), name, loader)
+            self.SOURCES[name] = klass
 
         source = klass(*args, **kwargs)
 
         if getattr(source, "name", None) is None:
             source.name = name
 
         return source
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/ads.py` & `earthkit_data-0.7.0/earthkit/data/sources/ads.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import os
 
-import cdsapi
+try:
+    import cdsapi
+except ImportError:
+    raise ImportError("ADS access requires 'cdsapi' to be installed")
+
 import yaml
 
 from .cds import CdsRetriever
 from .prompt import APIKeyPrompt
 
 
 class ADSAPIKeyPrompt(APIKeyPrompt):
@@ -37,27 +40,21 @@
     ]
 
     rcfile = "~/.adsapirc"
 
     def save(self, input, file):
         yaml.dump(input, file, default_flow_style=False)
 
+    def load(self, file):
+        return yaml.safe_load(file.read())
+
 
 def client():
     prompt = ADSAPIKeyPrompt()
-    prompt.check()
-
-    path = os.path.expanduser(prompt.rcfile)
-
-    if not os.path.exists(path):
-        prompt.ask_user_and_save()
-
-    with open(path) as f:
-        rc = yaml.safe_load(f.read())
-
+    rc = prompt.check(load=True)
     return cdsapi.Client(**rc)
 
 
 EXTENSIONS = {
     "grib": ".grib",
     "netcdf": ".nc",
 }
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/cds.py` & `earthkit_data-0.7.0/earthkit/data/sources/cds.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
-import collections.abc
+
 import itertools
+import logging
 import sys
 from functools import cached_property
 
-import cdsapi
+try:
+    import cdsapi
+except ImportError:
+    raise ImportError("CDS access requires 'cdsapi' to be installed")
+
 import yaml
 
 from earthkit.data.core.thread import SoftThreadPool
 from earthkit.data.decorators import normalize
-from earthkit.data.utils import tqdm
+from earthkit.data.utils import ensure_iterable
+from earthkit.data.utils.progbar import tqdm
 
 from .file import FileSource
 from .prompt import APIKeyPrompt
 
 if sys.version_info >= (3, 12):
     from itertools import batched
 else:
@@ -30,18 +36,15 @@
         if n < 1:
             raise ValueError("n must be at least one")
         it = iter(iterable)
         while batch := tuple(itertools.islice(it, n)):
             yield batch
 
 
-def ensure_iterable(obj):
-    if isinstance(obj, str) or not isinstance(obj, collections.abc.Iterable):
-        return [obj]
-    return obj
+LOG = logging.getLogger(__name__)
 
 
 class CDSAPIKeyPrompt(APIKeyPrompt):
     register_or_sign_in_url = "https://cds.climate.copernicus.eu/"
     retrieve_api_key_url = "https://cds.climate.copernicus.eu/api-how-to"
 
     prompts = [
@@ -57,62 +60,71 @@
             title="API key",
             hidden=True,
             validate=r"\d+:[\-0-9a-f]+",
         ),
     ]
 
     rcfile = "~/.cdsapirc"
+    rcfile_env = "CDSAPI_RC"
+    config_env = ("CDSAPI_URL", "CDSAPI_KEY")
 
     def save(self, input, file):
         yaml.dump(input, file, default_flow_style=False)
 
+    def load(self, file):
+        return yaml.safe_load(file.read())
 
-def client():
-    prompt = CDSAPIKeyPrompt()
-    prompt.check()
 
-    try:
-        return cdsapi.Client()
-    except Exception as e:
-        if ".cdsapirc" in str(e):
-            prompt.ask_user_and_save()
+def client(use_prompt):
+    if use_prompt:
+        prompt = CDSAPIKeyPrompt()
+        prompt.check()
+
+        try:
             return cdsapi.Client()
+        except Exception as e:
+            if ".cdsapirc" in str(e) or not prompt.has_config_env():
+                LOG.warning(e)
+                LOG.exception(f"Could not load cds api client. {e}")
+                prompt.ask_user_and_save()
+                return cdsapi.Client()
 
-        raise
+            raise
+    else:
+        return cdsapi.Client()
 
 
 EXTENSIONS = {
     "grib": ".grib",
     "netcdf": ".nc",
 }
 
 
 class CdsRetriever(FileSource):
     sphinxdoc = """
     CdsRetriever
     """
 
-    def client(self):
-        return client()
-
-    def __init__(self, dataset, *args, **kwargs):
+    def __init__(self, dataset, *args, prompt=True, **kwargs):
         super().__init__()
 
+        self.prompt = prompt
+
         assert isinstance(dataset, str)
         if args and kwargs:
             raise TypeError(
                 "CdsRetriever: cannot specify request using both args and kwargs"
             )
 
         if not args:
             args = (kwargs,)
         assert all(isinstance(request, dict) for request in args)
         self._args = args
 
-        self.client()  # Trigger password prompt before thraeding
+        self.client()  # Trigger password prompt before threading
 
         nthreads = min(self.settings("number-of-download-threads"), len(self.requests))
 
         if nthreads < 2:
             self.path = [self._retrieve(dataset, r) for r in self.requests]
         else:
             with SoftThreadPool(nthreads=nthreads) as pool:
@@ -121,21 +133,24 @@
                 ]
 
                 iterator = (f.result() for f in futures)
                 self.path = list(tqdm(iterator, leave=True, total=len(self.requests)))
 
     def _retrieve(self, dataset, request):
         def retrieve(target, args):
-            self.client().retrieve(args[0], args[1], target)
+            cds_result = self.client().retrieve(args[0], args[1])
+            self.source_filename = cds_result.location.split("/")[-1]
+            cds_result.download(target=target)
 
-        return self.cache_file(
+        return_object = self.cache_file(
             retrieve,
             (dataset, request),
             extension=EXTENSIONS.get(request.get("format"), ".cache"),
         )
+        return return_object
 
     @staticmethod
     @normalize("date", "date-list(%Y-%m-%d)")
     @normalize("area", "bounding-box(list)")
     def _normalize_request(**kwargs):
         return kwargs
 
@@ -151,12 +166,15 @@
 
             if not isinstance(split_on, dict):
                 split_on = {k: 1 for k in ensure_iterable(split_on)}
             for values in itertools.product(
                 *[batched(ensure_iterable(request[k]), v) for k, v in split_on.items()]
             ):
                 subrequest = dict(zip(split_on, values))
-                requests.append(request | subrequest)
+                requests.append({**request, **subrequest})
         return requests
 
+    def client(self):
+        return client(self.prompt)
+
 
 source = CdsRetriever
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/constants.py` & `earthkit_data-0.7.0/earthkit/data/sources/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,28 +182,28 @@
             self.latitude_(),
             self.longitude_(),
         )
         return result.flatten()
 
 
 class ConstantField(Field):
-    def __init__(self, date, param, proc, shape, geometry):
+    def __init__(self, date, param, proc, shape, geometry, backend):
         self.date = date
         self.param = param
         self.proc = proc
         self._shape = shape
         self._geometry = geometry
         d = dict(
             valid_datetime=date if isinstance(date, str) else date.isoformat(),
             param=param,
             level=None,
             levelist=None,
             number=None,
         )
-        super().__init__(metadata=ConstantMetadata(d, geometry))
+        super().__init__(backend, metadata=ConstantMetadata(d, geometry))
 
     def _make_metadata(self):
         pass
 
     def _values(self, dtype=None):
         values = self.proc(self.date)
         if dtype is not None:
@@ -283,14 +283,16 @@
         if not isinstance(self.params, list):
             self.params = [self.params]
         self.repeat = repeat  # For ensembles
         self.maker = ConstantMaker(source_or_dataset)
         self.procs = {param: getattr(self.maker, param) for param in self.params}
         self._len = len(self.dates) * len(self.params) * self.repeat
 
+        super().__init__(**kwargs)
+
     @normalize("date", "date-list")
     @normalize("time", "int-list")
     @normalize("number", "int-list")
     def _request(self, **request):
         return request
 
     @classmethod
@@ -322,16 +324,18 @@
             param = self.params[param]
             return ConstantField(
                 date,
                 param,
                 self.procs[param],
                 self.maker.shape,
                 self.maker.field.metadata().geography,
+                self.array_backend,
             )
 
 
 class ConstantsMaskFieldList(ConstantsFieldListCore, MaskIndex):
     def __init__(self, *args, **kwargs):
         MaskIndex.__init__(self, *args, **kwargs)
+        FieldList._init_from_mask(self, self)
 
 
 source = ConstantsFieldList
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/dummy_source.py` & `earthkit_data-0.7.0/earthkit/data/sources/dummy_source.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/ecmwf_api.py` & `earthkit_data-0.7.0/earthkit/data/sources/ecmwf_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 
 from earthkit.data.core.thread import SoftThreadPool
 from earthkit.data.decorators import normalize
-from earthkit.data.utils import tqdm
 
 from .file import FileSource
 from .prompt import APIKeyPrompt
 
 LOG = logging.getLogger(__name__)
 
 
@@ -33,41 +32,44 @@
         dict(
             name="key",
             example="b295aad8af30332fad2fa8c963ab7900",
             title="API key",
             hidden=True,
             validate="[0-9a-z]{32}",
         ),
-        dict(
-            name="email",
-            title="Your email",
-        ),
+        dict(name="email", title="Your email", env="ECMWF_API_EMAIL"),
     ]
 
     rcfile = "~/.ecmwfapirc"
+    rcfile_env = "ECMWF_API_RC_FILE"
+    config_env = ("ECMWF_API_KEY", "ECMWF_API_URL")
 
 
 class ECMWFApi(FileSource):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, prompt=True, **kwargs):
         super().__init__()
 
+        self.prompt = prompt
+
         request = {}
         for a in args:
             request.update(a)
         request.update(kwargs)
 
         requests = self.requests(**request)
 
         self.service()  # Trigger password prompt before threading
 
         nthreads = min(self.settings("number-of-download-threads"), len(requests))
 
         if nthreads < 2:
             self.path = [self._retrieve(r) for r in requests]
         else:
+            from earthkit.data.utils.progbar import tqdm
+
             with SoftThreadPool(nthreads=nthreads) as pool:
                 futures = [pool.submit(self._retrieve, r) for r in requests]
 
                 iterator = (f.result() for f in futures)
                 self.path = list(tqdm(iterator, leave=True, total=len(requests)))
 
     def _retrieve(self, request):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/ecmwf_open_data.py` & `earthkit_data-0.7.0/earthkit/data/sources/ecmwf_open_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,35 +3,43 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import ecmwf.opendata
+
+try:
+    import ecmwf.opendata
+except ImportError:
+    raise ImportError(
+        "ECMWF Open Data access requires 'ecmwf-opendata' to be installed"
+    )
 
 from .file import FileSource
 
 
 class EODRetriever(FileSource):
     sphinxdoc = """
     EODRetriever
     """
 
-    def __init__(self, source="ecmwf", *args, **kwargs):
+    def __init__(self, *args, source="ecmwf", model="ifs", **kwargs):
         super().__init__()
         if len(args):
             assert len(args) == 1
             assert isinstance(args[0], dict)
             assert not kwargs
             kwargs = args[0]
 
         self.source_kwargs = self.request(**kwargs)
 
-        self.client = ecmwf.opendata.Client(source=source, preserve_request_order=True)
+        self.client = ecmwf.opendata.Client(
+            source=source, model=model, preserve_request_order=True
+        )
 
         self.path = self._retrieve(self.source_kwargs)
 
     def connect_to_mirror(self, mirror):
         return mirror.connection_for_eod(self)
 
     def _retrieve(self, request):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/empty.py` & `earthkit_data-0.7.0/earthkit/data/sources/empty.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/fdb.py` & `earthkit_data-0.7.0/earthkit/data/sources/fdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 import os
 import shutil
 
-import pyfdb
+try:
+    import pyfdb
+except ImportError:
+    raise ImportError("FDB access requires 'pyfdb' to be installed")
 
 from earthkit.data.sources.file import FileSource
 from earthkit.data.sources.stream import StreamSource
 
 from . import Source
 
 LOG = logging.getLogger(__name__)
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/file.py` & `earthkit_data-0.7.0/earthkit/data/sources/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,47 +10,60 @@
 
 import glob
 import logging
 import os
 
 from earthkit.data import from_source
 from earthkit.data.core.caching import CACHE
+from earthkit.data.decorators import detect_out_filename
 from earthkit.data.readers import reader
+from earthkit.data.utils.parts import PathAndParts
 
 from . import Source
 
 LOG = logging.getLogger(__name__)
 
 
+class FileSourcePathAndParts(PathAndParts):
+    compress = False
+
+
 class FileSourceMeta(type(Source), type(os.PathLike)):
     def patch(cls, obj, *args, **kwargs):
         if "reader" in kwargs:
             setattr(obj, "reader", kwargs.pop("reader"))
 
         return super().patch(obj, *args, **kwargs)
 
 
 class FileSource(Source, os.PathLike, metaclass=FileSourceMeta):
     _reader_ = None
     content_type = None
 
-    def __init__(self, path=None, filter=None, merger=None, **kwargs):
+    def __init__(self, path=None, filter=None, merger=None, parts=None, **kwargs):
         Source.__init__(self, **kwargs)
-        self.path = path
         self.filter = filter
         self.merger = merger
+        self._path_and_parts = FileSourcePathAndParts(path, parts)
+
+        if self._kwargs.get("indexing", False):
+            if not self._path_and_parts.is_empty():
+                raise ValueError("Cannot specify parts when indexing is enabled!")
 
     def mutate(self):
         if isinstance(self.path, (list, tuple)):
             if len(self.path) == 1:
                 self.path = self.path[0]
             else:
                 return from_source(
                     "multi",
-                    [from_source("file", p, **self._kwargs) for p in self.path],
+                    [
+                        from_source("file", p, parts=part, **self._kwargs)
+                        for p, part in zip(self.path, self.parts)
+                    ],
                     filter=self.filter,
                     merger=self.merger,
                 )
 
         # here we must have a file or a directory
         if self._kwargs.get("indexing", False):
             from earthkit.data.sources.file_indexed import FileIndexedSource
@@ -76,15 +89,17 @@
 
         assert all(isinstance(s, FileSource) for s in sources)
         return merge_by_class([s._reader for s in sources])
 
     @property
     def _reader(self):
         if self._reader_ is None:
-            self._reader_ = reader(self, self.path, content_type=self.content_type)
+            self._reader_ = reader(
+                self, self.path, content_type=self.content_type, parts=self.parts
+            )
         return self._reader_
 
     def __iter__(self):
         return iter(self._reader)
 
     def __len__(self):
         return len(self._reader)
@@ -111,14 +126,15 @@
     def to_numpy(self, **kwargs):
         return self._reader.to_numpy(**kwargs)
 
     @property
     def values(self):
         return self._reader.values
 
+    @detect_out_filename
     def save(self, path, **kwargs):
         return self._reader.save(path, **kwargs)
 
     def write(self, f, **kwargs):
         return self._reader.write(f, **kwargs)
 
     def scaled(self, *args, **kwargs):
@@ -173,14 +189,26 @@
 
     def bounding_box(self):
         return self._reader.bounding_box()
 
     def statistics(self, **kwargs):
         return self._reader.statistics(**kwargs)
 
+    @property
+    def path(self):
+        return self._path_and_parts.path
+
+    @path.setter
+    def path(self, v):
+        self._path_and_parts.update(v)
+
+    @property
+    def parts(self):
+        return self._path_and_parts.parts
+
 
 class IndexedFileSource(FileSource):
     def mutate(self):
         pass
 
 
 class File(FileSource):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/file_indexed.py` & `earthkit_data-0.7.0/earthkit/data/sources/file_indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/file_pattern.py` & `earthkit_data-0.7.0/earthkit/data/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/indexed.py` & `earthkit_data-0.7.0/earthkit/data/sources/indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/list_of_dicts.py` & `earthkit_data-0.7.0/earthkit/data/sources/list_of_dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,16 +167,16 @@
             east=self.get("longitudeOfLastGridPointInDegrees", None),
         )
 
     from earthkit.data.core.geography import Geography
 
 
 class VirtualGribField(Field):
-    def __init__(self, d):
-        super().__init__(metadata=VirtualGribMetadata(d))
+    def __init__(self, d, backend):
+        super().__init__(backend, metadata=VirtualGribMetadata(d))
 
     def _values(self, dtype=None):
         v = self._metadata["values"]
         if dtype is None:
             return v
         else:
             return v.astype(dtype)
@@ -187,14 +187,14 @@
 
 class GribFromDicts(GribFieldList):
     def __init__(self, list_of_dicts, *args, **kwargs):
         self.list_of_dicts = list_of_dicts
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, n):
-        return VirtualGribField(self.list_of_dicts[n])
+        return VirtualGribField(self.list_of_dicts[n], self.array_backend)
 
     def __len__(self):
         return len(self.list_of_dicts)
 
 
 source = GribFromDicts
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/mars.py` & `earthkit_data-0.7.0/earthkit/data/sources/mars.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 import os
 import subprocess
 
-import ecmwfapi
+try:
+    import ecmwfapi
+except ImportError:
+    raise ImportError("MARS access requires 'ecmwf-api-client' to be installed")
 
 from earthkit.data.core.settings import SETTINGS
 from earthkit.data.core.temporary import temp_file
 
 from .ecmwf_api import ECMWFApi, MARSAPIKeyPrompt
 
 LOG = logging.getLogger(__name__)
@@ -48,21 +51,26 @@
 
 class MarsRetriever(ECMWFApi):
     def service(self):
         if SETTINGS.get("use-standalone-mars-client-when-available"):
             if os.path.exists(StandaloneMarsClient.EXE):
                 return StandaloneMarsClient()
 
-        prompt = MARSAPIKeyPrompt()
-        prompt.check()
+        if self.prompt:
+            prompt = MARSAPIKeyPrompt()
+            prompt.check()
 
-        try:
-            return ecmwfapi.ECMWFService("mars")
-        except Exception as e:
-            if ".ecmwfapirc" in str(e):
-                prompt.ask_user_and_save()
+            try:
                 return ecmwfapi.ECMWFService("mars")
+            except Exception as e:
+                if ".ecmwfapirc" in str(e) or not prompt.env_configured():
+                    LOG.warning(e)
+                    LOG.exception(f"Could not load ecmwf api (mars) client. {e}")
+                    prompt.ask_user_and_save()
+                    return ecmwfapi.ECMWFService("mars")
 
-            raise
+                raise
+        else:
+            return ecmwfapi.ECMWFService("mars")
 
 
 source = MarsRetriever
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/memory.py` & `earthkit_data-0.7.0/earthkit/data/sources/memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/multi.py` & `earthkit_data-0.7.0/earthkit/data/sources/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import itertools
 import logging
 
 from earthkit.data.core.thread import SoftThreadPool
 from earthkit.data.mergers import make_merger, merge_by_class
 from earthkit.data.sources.empty import EmptySource
-from earthkit.data.utils import tqdm
 from earthkit.data.utils.bbox import BoundingBox
 
 from . import Source
 
 LOG = logging.getLogger(__name__)
 
 
@@ -119,14 +118,16 @@
         nthreads = min(self.settings("number-of-download-threads"), len(callables))
         if nthreads < 2:
             return [s() for s in sources]
 
         def _call(s, *args, **kwargs):
             return s(*args, **kwargs)
 
+        from earthkit.data.utils.progbar import tqdm
+
         with SoftThreadPool(nthreads=nthreads) as pool:
             futures = [pool.submit(_call, s, observer=pool) for s in sources]
 
             iterator = (f.result() for f in futures)
             sources = list(tqdm(iterator, leave=False, total=len(futures)))
 
         return sources
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/multi_url.py` & `earthkit_data-0.7.0/earthkit/data/sources/multi_url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/polytope.py` & `earthkit_data-0.7.0/earthkit/data/sources/polytope.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,40 +5,43 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 
+try:
+    import polytope
+except ImportError:
+    raise ImportError("Polytope access requires 'polytope-client' to be installed")
+
 from . import Source
 from .multi_url import MultiUrl
 from .prompt import APIKeyPrompt
 from .url import Url
 
 LOG = logging.getLogger(__name__)
 
 
 class PolytopeWebKeyPrompt(APIKeyPrompt):
     register_or_sign_in_url = ("",)
     retrieve_api_key_url = ("",)
     prompts = [
-        dict(
-            name="user_email",
-            title="Your email",
-        ),
+        dict(name="user_email", title="Your email"),
         dict(
             name="user_key",
             example="b295aad8af30332fad2fa8c963ab7900",
             title="API key",
             hidden=True,
             validate="[0-9a-z]{32}",
         ),
     ]
 
     rcfile = "~/.polytopeapirc"
+    config_env = ("POLYTOPE_USER_EMAIL", "POLYTOPE_USER_KEY")
 
 
 class Polytope(Source):
     """
     Retrieve data using the Polytope Web API.
     See polytope-client.readthedocs.io for more information.
 
@@ -52,40 +55,35 @@
     Examples
     --------
     >>> src = earthkit.data.from_source("polytope", "ecmwf-mars", request)
     >>> src.to_pandas()  # if tabular data
     >>> src.to_xarray()  # if datacube
     """
 
-    def __init__(self, dataset, request, address=None, stream=True, **kwargs) -> None:
-        try:
-            import polytope
-        except ImportError:
-            raise ImportError(
-                "Polytope Web Client must be installed with 'pip install polytope-client'"
-            )
-
+    def __init__(
+        self,
+        dataset,
+        request,
+        stream=True,
+        **kwargs,
+    ) -> None:
         super().__init__()
         assert isinstance(dataset, str)
 
         self._stream_kwargs = dict()
         for k in ["group_by", "batch_size"]:
             if k in kwargs:
                 self._stream_kwargs[k] = kwargs.pop(k)
 
         self.stream = stream
 
         self.request = dict(dataset=dataset, request=request)
 
-        credentials = PolytopeWebKeyPrompt().check(load=True)
-
-        client_kwargs = {}
-        if address is not None:
-            client_kwargs = {"address": address}
-        self.client = polytope.api.Client(**credentials, **client_kwargs)
+        # all the kwargs are passed to the client!
+        self.client = polytope.api.Client(**kwargs)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.request['dataset']}, {self.request['request']})"
 
     def mutate(self) -> Source:
         pointers = self.client.retrieve(
             self.request["dataset"],
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/prompt.py` & `earthkit_data-0.7.0/earthkit/data/sources/prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 import json
 import logging
 import os
 import re
 import stat
 from getpass import getpass
 
-import markdown
-
 from earthkit.data.core.ipython import HTML, display, ipython_active
+from earthkit.data.utils.humanize import list_to_human
 
 LOG = logging.getLogger(__name__)
 
 
 # See https://medium.com/analytics-vidhya/the-ultimate-markdown-guide-for-jupyter-notebook-d5e5abf728fd
 HTML_MESSAGE = """
 <div style='border: 1px solid orange; color: black;
@@ -40,28 +39,61 @@
 
 MESSAGE = """
 An API key is needed to access this dataset. Please visit
 {register_or_sign_in_url} to register or sign-in
 then visit {retrieve_api_key_url} to retrieve you API key.
 """
 
+RC_MESSAGE_BASE = """
+You can store the credentials in {rcfile}; if you follow the
+instructions below it will be automatically done for you.
+"""
+
+RC_MESSAGE_EXT = """
+You can store the credentials in {rcfile} or in the file
+pointed by the {rcfile_env} environment variable. If you follow
+the instructions below {rcfile} will be automatically created
+for you.
+"""
+
 
 class RegexValidate:
     def __init__(self, pattern):
         self.pattern = pattern
 
     def __call__(self, value):
         assert re.fullmatch(self.pattern, value), (self.pattern, value)
         return value
 
 
 class Prompt:
     def __init__(self, owner):
         self.owner = owner
 
+    def _rc_message(self):
+        if self.owner.rcfile:
+            if self.owner.rcfile_env:
+                return RC_MESSAGE_EXT.format(
+                    rcfile=self.owner.rcfile, rcfile_env=self.owner.rcfile_env
+                )
+            else:
+                return RC_MESSAGE_BASE.format(rcfile=self.owner.rcfile)
+
+        return ""
+
+    def _config_env_message(self):
+        ev = self.owner.config_env
+        if ev:
+            plural = "s" if len(ev) > 1 else ""
+            return (
+                f" Alternatively, you can use the {list_to_human(ev)}"
+                f" environment variable{plural} to specify the credentials."
+            )
+        return ""
+
     def ask_user(self):
         self.print_message()
 
         result = {}
 
         for p in self.owner.prompts:
             method = getpass if p.get("hidden", False) else input
@@ -83,60 +115,73 @@
 class Text(Prompt):
     def print_message(self):
         print(
             MESSAGE.format(
                 register_or_sign_in_url=self.owner.register_or_sign_in_url,
                 retrieve_api_key_url=self.owner.retrieve_api_key_url,
             )
+            + self._rc_message()
+            + self._config_env_message()
         )
 
     def ask(self, p, method):
         message = f"Please enter a value for '{p.get('title')}'"
         if "default" in p:
             message += f" or leave empty for the default value '{p.get('default')}'"
         message += ", then press <ENTER>"
         return method(p.get("title") + ": ").strip()
 
 
 class Markdown(Prompt):
     def print_message(self):
+        import markdown
+
         message = markdown.markdown(
             MESSAGE.format(
                 register_or_sign_in_url=f"<{self.owner.register_or_sign_in_url}>",
                 retrieve_api_key_url=f"<{self.owner.retrieve_api_key_url}>",
+                rcfile=f"{self.owner.rcfile}",
             )
+            + self._rc_message()
+            + self._config_env_message()
         )
         # We use Python's markdown instead of IPython's Markdown because
         # jupyter lab/colab/deepnotes all behave differently
         display(HTML(HTML_MESSAGE.format(message=message)))
 
     def ask(self, p, method):
+        import markdown
+
         message = f"Please enter a value for <span style='color: red;'>{p.get('title')}</span>"
         if "default" in p:
             message += (
-                " or leave empty for the default value ",
-                f"<span style='color: red;'>{p.get('default')}</span>",
+                " or leave empty for the default value "
+                f"<span style='color: red;'>{p.get('default')}</span>"
             )
         message += ", then press *ENTER*"
         if "example" in p:
             message += f" The value should look like  <span style='color: red;'>{p.get('example')}</span>"
         message = markdown.markdown(message)
         display(HTML(HTML_ASK.format(message=message)))
         return method(p.get("title") + ": ").strip()
 
 
 class APIKeyPrompt:
+    rcfile_env = None
+    config_env = []
+
     def check(self, load=False):
-        rcfile = os.path.expanduser(self.rcfile)
-        if not os.path.exists(rcfile):
+        if not self.has_api_config():
             self.ask_user_and_save()
 
         if load:
-            with open(rcfile) as f:
-                return self.load(f)
+            rcfile = self.existing_rcfile_path()
+            if rcfile is not None:
+                with open(rcfile) as f:
+                    return self.load(f)
 
     def ask_user(self):
         if ipython_active:
             prompt = Markdown(self)
         else:
             prompt = Text(self)
 
@@ -160,9 +205,29 @@
 
     def save(self, input, file):
         json.dump(input, file, indent=4)
 
     def load(self, file):
         return json.load(file)
 
+    def existing_rcfile_path(self):
+        rcfile = os.path.expanduser(self.rcfile)
+        if os.path.exists(rcfile):
+            return rcfile
+
+        if self.rcfile_env:
+            rcfile = os.path.expanduser(os.getenv(self.rcfile_env, ""))
+            if os.path.exists(rcfile):
+                return rcfile
+
+    def has_config_env(self):
+        for ev in self.config_env:
+            v = os.getenv(ev, "")
+            if v is None or v == "":
+                return False
+        return True if len(self.config_env) > 0 else False
+
+    def has_api_config(self):
+        return self.existing_rcfile_path() is not None or self.has_config_env()
+
     def validate(self, input):
         return input
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/stream.py` & `earthkit_data-0.7.0/earthkit/data/sources/stream.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,44 +55,45 @@
         super().__init__(**kwargs)
         self._stream = stream
         self._reader_ = None
 
     @property
     def _reader(self):
         if self._reader_ is None:
-            self._reader_ = stream_reader(self, self._stream, True)
+            self._reader_ = stream_reader(self, self._stream, True, **self._kwargs)
             if self._reader_ is None:
                 raise TypeError(f"could not create reader for stream={self._stream}")
         return self._reader_
 
     def mutate(self):
         source = self._reader.mutate_source()
         if source not in (None, self):
             source._parent = self
             return source
         return self
 
 
 class StreamSourceBase(Source):
-    def __init__(self, stream, *, batch_size=1, group_by=None):
+    def __init__(self, stream, *, batch_size=1, group_by=None, **kwargs):
         super().__init__()
         self._reader_ = None
         self._stream = stream
         self.batch_size, self.group_by = check_stream_kwargs(batch_size, group_by)
+        self._kwargs = kwargs
 
     def __iter__(self):
         return self
 
     def mutate(self):
         return self
 
     @property
     def _reader(self):
         if self._reader_ is None:
-            self._reader_ = stream_reader(self, self._stream, False)
+            self._reader_ = stream_reader(self, self._stream, False, **self._kwargs)
             if self._reader_ is None:
                 raise TypeError(f"could not create reader for stream={self._stream}")
         return self._reader_
 
 
 class StreamSingleSource(StreamSourceBase):
     def __init__(self, stream, **kwargs):
@@ -210,73 +211,70 @@
         return r
 
 
 class StreamSource(StreamSourceBase):
     def __init__(self, stream, **kwargs):
         super().__init__(stream, **kwargs)
 
-        # print(f"kwargs={kwargs} {id(kwargs)}")
-        # if kwargs:
-        #     raise TypeError(f"got invalid keyword argument(s): {list(kwargs.keys())}")
-
     def mutate(self):
         assert self._reader_ is None
 
         return _from_stream(
-            self._stream, batch_size=self.batch_size, group_by=self.group_by
+            self._stream,
+            batch_size=self.batch_size,
+            group_by=self.group_by,
+            **self._kwargs,
         )
 
 
 class StreamSourceMaker:
-    def __init__(self, source, stream_kwargs):
+    def __init__(self, source, stream_kwargs, **kwargs):
         self.in_source = source
+        self._kwargs = kwargs
         self.stream_kwargs = dict(stream_kwargs)
         self.source = None
 
     def __call__(self):
         if self.source is None:
             stream = self.in_source.to_stream()
-            self.source = _from_stream(stream, **self.stream_kwargs)
+            self.source = _from_stream(stream, **self.stream_kwargs, **self._kwargs)
 
             prev = None
             src = self.source
             while src is not prev:
                 prev = src
                 src = src.mutate()
             self.source = src
 
         return self.source
 
 
-def _from_stream(stream, group_by, batch_size):
+def _from_stream(stream, group_by, batch_size, **kwargs):
     _kwargs = dict(batch_size=batch_size, group_by=group_by)
 
     if group_by:
-        return StreamGroupSource(stream, **_kwargs)
+        return StreamGroupSource(stream, **_kwargs, **kwargs)
     elif batch_size == 0:
-        return StreamMemorySource(stream)
+        return StreamMemorySource(stream, **kwargs)
     elif batch_size > 1:
-        return StreamBatchSource(stream, **_kwargs)
+        return StreamBatchSource(stream, **_kwargs, **kwargs)
     elif batch_size == 1:
-        return StreamSingleSource(stream, **_kwargs)
+        return StreamSingleSource(stream, **_kwargs, **kwargs)
 
     raise ValueError(f"Unsupported stream parameters {batch_size=} {group_by=}")
 
 
 def _from_source(source, **kwargs):
     stream_kwargs, kwargs = parse_stream_kwargs(**kwargs)
 
-    if kwargs:
-        raise TypeError(f"got invalid keyword argument(s): {list(kwargs.keys())}")
-
     if not isinstance(source, (list, tuple)):
         source = [source]
 
     if len(source) == 1:
-        maker = StreamSourceMaker(source[0], stream_kwargs)
+        maker = StreamSourceMaker(source[0], stream_kwargs, **kwargs)
         return maker()
     else:
-        sources = [StreamSourceMaker(s, stream_kwargs) for s in source]
+        sources = [StreamSourceMaker(s, stream_kwargs, **kwargs) for s in source]
         return MultiStreamSource(sources, **stream_kwargs)
 
 
 source = StreamSource
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/url.py` & `earthkit_data-0.7.0/earthkit/data/sources/url.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import logging
 
 from multiurl import Downloader
 
 from earthkit.data.core.caching import cache_file
 from earthkit.data.core.settings import SETTINGS
 from earthkit.data.core.statistics import record_statistics
-from earthkit.data.utils import progress_bar
+from earthkit.data.utils.parts import PathAndParts
+from earthkit.data.utils.progbar import progress_bar
 
 from .file import FileSource
 
 LOG = logging.getLogger(__name__)
 
 
 def _ignore(*args, **kwargs):
@@ -103,14 +104,18 @@
         extension=extension,
         force=force,
     )
 
     return path
 
 
+class UrlSourcePathAndParts(PathAndParts):
+    compress = True
+
+
 class UrlBase(FileSource):
     def __init__(
         self,
         url,
         chunk_size=1024 * 1024,
         parts=None,
         filter=None,
@@ -121,49 +126,50 @@
         fake_headers=None,  # When HEAD is not allowed but you know the size
         stream=False,
         auth=None,
         **kwargs,
     ):
         super().__init__(filter=filter, merger=merger)
 
-        self.url = url
+        self._url_and_parts = UrlSourcePathAndParts(url, parts)
         self.chunk_size = chunk_size
-        self.parts = parts
         self.http_headers = http_headers
         self.auth = auth
         self.verify = verify
         self.range_method = range_method
         self.fake_headers = fake_headers
         self.stream = stream
         self._kwargs = kwargs
         LOG.debug(
-            f"url={self.url} parts={self.parts} auth={self.auth} _kwargs={self._kwargs}"
+            f"url={self.url} url_parts={self.url_parts} auth={self.auth} _kwargs={self._kwargs}"
         )
 
     def connect_to_mirror(self, mirror):
-        return mirror.connection_for_url(self, self.url, self.parts)
+        return mirror.connection_for_url(self, self.url, self.url_parts)
 
     def prepare_headers(self, url):
         headers = {}
         if self.http_headers is not None:
             headers = dict(self.http_headers)
 
         if self.auth is not None:
             headers.update(self.auth.auth_header(url))
 
         if not headers:
             headers = None
 
         return headers
 
-    def _get_parts(self, url):
-        if isinstance(self.parts, dict):
-            return self.parts.get(url, None)
-        else:
-            return self.parts
+    @property
+    def url(self):
+        return self._url_and_parts.path
+
+    @property
+    def url_parts(self):
+        return self._url_and_parts.parts
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.url})"
 
 
 class Url(UrlBase):
     """Represent a URL source.
@@ -192,41 +198,37 @@
         **kwargs,
     ):
         super().__init__(url, **kwargs)
 
         # TODO: re-enable this feature
         extension = None
 
-        self.prepare()
-
         if not self.stream:
             self.update_if_out_of_date = update_if_out_of_date
 
             LOG.debug(
                 (
-                    f"url={self.url} parts={self.parts} auth={self.auth}) "
-                    f"http_headers={self.http_headers} parts_kwargs={self.parts_kwargs}"
+                    f"url={self.url} url_parts={self.url_parts} auth={self.auth}) "
+                    f"http_headers={self.http_headers}"
                     f" _kwargs={self._kwargs}"
                 )
             )
-
             self.downloader = Downloader(
-                self.url,
+                self._url_and_parts.zipped(),
                 chunk_size=self.chunk_size,
                 timeout=SETTINGS.get("url-download-timeout"),
                 verify=self.verify,
                 range_method=self.range_method,
                 http_headers=self.prepare_headers(self.url),
                 fake_headers=self.fake_headers,
                 statistics_gatherer=record_statistics,
                 progress_bar=progress_bar,
                 resume_transfers=True,
                 override_target_file=False,
                 download_file_extension=".download",
-                **self.parts_kwargs,
             )
 
             if extension and extension[0] != ".":
                 extension = "." + extension
 
             if extension is None:
                 extension = self.downloader.extension()
@@ -240,36 +242,29 @@
 
             def download(target, _):
                 self.downloader.download(target)
                 return self.downloader.cache_data()
 
             self.path = self.cache_file(
                 download,
-                dict(url=self.url, parts=self.parts),
+                dict(url=self.url, parts=self.url_parts),
                 extension=extension,
                 force=force,
             )
 
             # cache data may contain the result of the http HEAD request
             h = self.downloader.cache_data()
             if isinstance(h, dict):
                 self.content_type = h.get("content-type")
 
     def mutate(self):
         if self.stream:
-            # create one stream source per url
-            from multiurl.downloader import _canonicalize
-
+            # # create one stream source per url
             s = []
-            _kwargs = dict(**self.parts_kwargs)
-            # if self.parts is not None:
-            #     _kwargs = {"parts": self.parts}
-            urls, _ = _canonicalize(self.url, **_kwargs)
-
-            for url, parts in urls:
+            for url, parts in self._url_and_parts:
                 s.append(
                     SingleUrlStream(
                         url,
                         parts=parts,
                         verify=True,
                         range_method="auto",
                         http_headers=self.prepare_headers(url),
@@ -280,40 +275,14 @@
 
             from .stream import _from_source
 
             return _from_source(s, **self._kwargs)
         else:
             return super().mutate()
 
-    def prepare(self):
-        # ensure no parts kwargs is used when the parts are defined together with the urls
-        self.parts_kwargs = {}
-        urls = self.url
-
-        if not isinstance(urls, (list, tuple)):
-            urls = [urls]
-
-        # a single url as [url, parts] is not allowed by multiurl
-        if (
-            len(urls) == 2
-            and isinstance(urls[0], str)
-            and (urls[1] is None or isinstance(urls[1], (list, tuple)))
-        ):
-            if self.parts is not None:
-                raise ValueError("Cannot specify parts both as arg and kwarg")
-            self.url, self.parts = urls
-            self.parts_kwargs = {"parts": self.parts}
-        # each url is a [url, parts]
-        elif isinstance(urls[0], (list, tuple)):
-            if self.parts is not None:
-                raise ValueError("Cannot specify parts both as arg and kwarg")
-        # each url is a str
-        else:
-            self.parts_kwargs = {"parts": self.parts}
-
     def out_of_date(self, url, path, cache_data):
         if SETTINGS.get("check-out-of-date-urls") is False:
             return False
 
         if self.downloader.out_of_date(path, cache_data):
             if SETTINGS.get("download-out-of-date-urls") or self.update_if_out_of_date:
                 LOG.warning(
@@ -470,15 +439,15 @@
 
         return _from_source(self, **self._kwargs)
 
     def to_stream(self):
         downloader = Downloader(
             self.url,
             chunk_size=self.chunk_size,
-            parts=self.parts,
+            parts=self.url_parts,
             timeout=SETTINGS.get("url-download-timeout"),
             verify=self.verify,
             range_method=self.range_method,
             http_headers=self.prepare_headers(self.url),
             fake_headers=self.fake_headers,
             statistics_gatherer=_ignore,
             progress_bar=progress_bar,
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/url_pattern.py` & `earthkit_data-0.7.0/earthkit/data/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/virtual.py` & `earthkit_data-0.7.0/earthkit/data/sources/virtual.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/virtual_directory.py` & `earthkit_data-0.7.0/earthkit/data/sources/virtual_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 import logging
 import warnings
 from collections import defaultdict
 
 from earthkit.data.readers.grib.index import FieldListInFilesWithSqlIndex
 from earthkit.data.sources.directory import DirectorySource
-from earthkit.data.utils import progress_bar
+from earthkit.data.utils.progbar import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 USE_REFERENCE = [
     "distinctLatitudes",
     "distinctLongitudes",
     "gridType",
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/wekeo.py` & `earthkit_data-0.7.0/earthkit/data/sources/wekeo.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
+import logging
 import os
 
-import hda
+try:
+    import hda
+except ImportError:
+    raise ImportError("WEkEO access requires 'hda' to be installed")
+
 import yaml
 from hda.api import DataOrderRequest
 
 from earthkit.data.core.thread import SoftThreadPool
-from earthkit.data.utils import tqdm
 
 from .file import FileSource
 from .prompt import APIKeyPrompt
 
+LOG = logging.getLogger(__name__)
+
 
 class HDAAPIKeyPrompt(APIKeyPrompt):
     register_or_sign_in_url = "https://www.wekeo.eu"
     retrieve_api_key_url = "https://www.wekeo.eu"
 
     prompts = [
         dict(
@@ -44,18 +50,23 @@
             title="Password",
             hidden=True,
             validate=r"[0-9A-z\!\@\#\$\%\&\*]{5,30}",
         ),
     ]
 
     rcfile = "~/.hdarc"
+    rcfile_env = "HDA_RC"
+    config_env = ("HDA_URL", "HDA_USER", "HDA_PASSWORD")
 
     def save(self, input, file):
         yaml.dump(input, file, default_flow_style=False)
 
+    def load(self, file):
+        return yaml.safe_load(file.read())
+
 
 class ApiClient(hda.Client):
     name = "wekeo"
 
     def __int__(self, *args, **kwargs):
         super().__init__(self, *args, **kwargs)
 
@@ -89,55 +100,66 @@
 
 
 class WekeoRetriever(FileSource):
     sphinxdoc = """
     WekeoRetriever
     """
 
-    @staticmethod
-    def client():
-        prompt = HDAAPIKeyPrompt()
-        prompt.check()
-
-        try:
-            return ApiClient()
-        except Exception as e:
-            if ".hdarc" in str(e):
-                prompt.ask_user_and_save()
-                return ApiClient()
-            raise
-
-    def __init__(self, dataset, *args, **kwargs):
+    def __init__(self, dataset, *args, prompt=True, **kwargs):
         super().__init__()
 
+        self.prompt = prompt
+
         assert isinstance(dataset, str)
         if len(args):
             assert len(args) == 1
             assert isinstance(args[0], dict)
             assert not kwargs
             kwargs = args[0]
 
         requests = self.requests(**kwargs)
 
-        self.client()  # Trigger password prompt before thraeding
+        self.client(self.prompt)  # Trigger password prompt before threading
 
         nthreads = min(self.settings("number-of-download-threads"), len(requests))
 
         if nthreads < 2:
             self.path = [self._retrieve(dataset, r) for r in requests]
         else:
+            from earthkit.data.utils.progbar import tqdm
+
             with SoftThreadPool(nthreads=nthreads) as pool:
                 futures = [pool.submit(self._retrieve, dataset, r) for r in requests]
 
                 iterator = (f.result() for f in futures)
                 self.path = list(tqdm(iterator, leave=True, total=len(requests)))
 
+    @staticmethod
+    def client(use_prompt):
+        if use_prompt:
+            prompt = HDAAPIKeyPrompt()
+            prompt.check()
+
+            try:
+                return ApiClient()
+            except Exception as e:
+                # if no rc file is available hda throws
+                # ConfigurationError: Missing or incomplete configuration
+                if ".hdarc" in str(e) or not prompt.has_config_env():
+                    LOG.warning(e)
+                    LOG.exception(f"Could not load hda client. {e}")
+                    prompt.ask_user_and_save()
+                    return ApiClient()
+                raise
+        else:
+            return ApiClient()
+
     def _retrieve(self, dataset, request):
         def retrieve(target, args):
-            self.client().retrieve(args[0], args[1], target)
+            self.client(self.prompt).retrieve(args[0], args[1], target)
 
         return self.cache_file(
             retrieve,
             (dataset, request),
             extension=EXTENSIONS.get(request.get("format"), ".cache"),
         )
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sources/wekeocds.py` & `earthkit_data-0.7.0/earthkit/data/sources/wekeocds.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
+import logging
 import os
 
-from hda.api import DataOrderRequest
+try:
+    from hda.api import DataOrderRequest
+except ImportError:
+    raise ImportError("WEkEO access requires 'hda' to be installed")
 
 from earthkit.data.core.thread import SoftThreadPool
 from earthkit.data.decorators import normalize
-from earthkit.data.utils import tqdm
 
 from .file import FileSource
 from .wekeo import EXTENSIONS
 from .wekeo import ApiClient as WekeoClient
 from .wekeo import HDAAPIKeyPrompt
 
+LOG = logging.getLogger(__name__)
+
 
 class ApiClient(WekeoClient):
     name = "wekeocds"
 
     def __int__(self, *args, **kwargs):
         super().__init__(self, *args, **kwargs)
 
@@ -53,55 +58,46 @@
 
 
 class WekeoCdsRetriever(FileSource):
     sphinxdoc = """
     WekeoCdsRetriever
     """
 
-    @staticmethod
-    def client():
-        prompt = HDAAPIKeyPrompt()
-        prompt.check()
-        try:
-            return ApiClient()
-        except Exception as e:
-            if ".hdarc" in str(e):
-                prompt.ask_user_and_save()
-                return ApiClient()
-
-            raise
-
-    def __init__(self, dataset, *args, **kwargs):
+    def __init__(self, dataset, *args, prompt=True, **kwargs):
         super().__init__()
 
+        self.prompt = prompt
+
         assert isinstance(dataset, str)
         if len(args):
             assert len(args) == 1
             assert isinstance(args[0], dict)
             assert not kwargs
             kwargs = args[0]
 
         requests = self.requests(**kwargs)
 
-        self.client()  # Trigger password prompt before thraeding
+        self.client(self.prompt)  # Trigger password prompt before threading
 
         nthreads = min(self.settings("number-of-download-threads"), len(requests))
 
         if nthreads < 2:
             self.path = [self._retrieve(dataset, r) for r in requests]
         else:
+            from earthkit.data.utils.progbar import tqdm
+
             with SoftThreadPool(nthreads=nthreads) as pool:
                 futures = [pool.submit(self._retrieve, dataset, r) for r in requests]
 
                 iterator = (f.result() for f in futures)
                 self.path = list(tqdm(iterator, leave=True, total=len(requests)))
 
     def _retrieve(self, dataset, request):
         def retrieve(target, args):
-            self.client().retrieve(args[0], args[1], target)
+            self.client(self.prompt).retrieve(args[0], args[1], target)
 
         return self.cache_file(
             retrieve,
             (dataset, request),
             extension=EXTENSIONS.get(request.get("format"), ".cache"),
         )
 
@@ -123,9 +119,29 @@
         for v in kwargs[split_on]:
             r = dict(**kwargs)
             r[split_on] = v
             result.append(r)
 
         return result
 
+    @staticmethod
+    def client(use_prompt):
+        if use_prompt:
+            prompt = HDAAPIKeyPrompt()
+            prompt.check()
+
+            try:
+                return ApiClient()
+            except Exception as e:
+                # if no rc file is available hda throws
+                # ConfigurationError: Missing or incomplete configuration
+                if ".hdarc" in str(e) or not prompt.has_config_env():
+                    LOG.warning(e)
+                    LOG.exception(f"Could not load hda client. {e}")
+                    prompt.ask_user_and_save()
+                    return ApiClient()
+                raise
+        else:
+            return ApiClient()
+
 
 source = WekeoCdsRetriever
```

### Comparing `earthkit-data-0.6.0/earthkit/data/sphinxext/generate_settings_rst.py` & `earthkit_data-0.7.0/earthkit/data/sphinxext/generate_settings_rst.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sphinxext/module_output.py` & `earthkit_data-0.7.0/earthkit/data/sphinxext/module_output.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/sphinxext/xref.py` & `earthkit_data-0.7.0/earthkit/data/sphinxext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/testing.py` & `earthkit_data-0.7.0/earthkit/data/testing.py`

 * *Files 23% similar despite different names*

```diff
@@ -97,14 +97,23 @@
     fdb_home = os.environ.get("FDB_HOME", None)
     NO_FDB = fdb_home is None
 except Exception:
     NO_FDB = True
 
 NO_POLYTOPE = not os.path.exists(os.path.expanduser("~/.polytopeapirc"))
 NO_ECCOVJSON = not modules_installed("eccovjson")
+NO_PYTORCH = not modules_installed("torch")
+NO_CUPY = not modules_installed("cupy")
+if not NO_CUPY:
+    try:
+        import cupy as cp
+
+        a = cp.ones(2)
+    except Exception:
+        NO_CUPY = True
 
 
 def MISSING(*modules):
     return not modules_installed(*modules)
 
 
 UNSAFE_SAMPLES_URL = "https://github.com/jwilk/traversal-archives/releases/download/0"
@@ -145,14 +154,42 @@
         return from_source("file", path)
     else:
         import xarray
 
         return from_object(xarray.open_dataset(path))
 
 
+def check_array_type(v, backend, **kwargs):
+    from earthkit.data.utils.array import ensure_backend
+
+    b = ensure_backend(backend)
+    assert b.is_native_array(v, **kwargs), f"{type(v)}, {backend=}, {kwargs=}"
+
+
+def get_array_namespace(backend):
+    from earthkit.data.utils.array import ensure_backend
+
+    return ensure_backend(backend).array_ns
+
+
+def get_array(v, backend, **kwargs):
+    from earthkit.data.utils.array import ensure_backend
+
+    b = ensure_backend(backend)
+    return b.from_other(v, **kwargs)
+
+
+ARRAY_BACKENDS = ["numpy"]
+if not NO_PYTORCH:
+    ARRAY_BACKENDS.append("pytorch")
+
+if not NO_CUPY:
+    ARRAY_BACKENDS.append("cupy")
+
+
 def main(path):
     import sys
 
     import pytest
 
     # Parallel does not work on darwin, gets RuntimeError: context has already been set
     # because pytest-parallel changes the context from `spawn` to `fork`
```

### Comparing `earthkit-data-0.6.0/earthkit/data/translators/__init__.py` & `earthkit_data-0.7.0/earthkit/data/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/translators/ndarray.py` & `earthkit_data-0.7.0/earthkit/data/translators/ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/translators/pandas.py` & `earthkit_data-0.7.0/earthkit/data/translators/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/translators/string.py` & `earthkit_data-0.7.0/earthkit/data/translators/string.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/translators/xarray.py` & `earthkit_data-0.7.0/earthkit/data/translators/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/__init__.py` & `earthkit_data-0.7.0/earthkit/data/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 import inspect
 import json
 import re
 
-import requests
 import yaml
 
-try:
-    # There is a bug in tqdm that expects ipywidgets
-    # to be installed if running in a notebook
-    import ipywidgets  # noqa F401
-    from tqdm.auto import tqdm  # noqa F401
-except ImportError:
-    from tqdm import tqdm  # noqa F401
-
 
 def download_and_cache(url, return_none_on_404=False, **kwargs):
+    import requests
+
     from earthkit.data.sources.url import download_and_cache
 
     try:
         return download_and_cache(url, **kwargs)
     except requests.HTTPError as e:
         if return_none_on_404:
             if e.response is not None and e.response.status_code == 404:
@@ -150,28 +143,13 @@
         if path.endswith(".yaml") or path.endswith(".yml"):
             return yaml.safe_load(f)
         raise ValueError(
             f"Cannot read file {path}. Need json or yaml with appropriate extension."
         )
 
 
-def progress_bar(*, total=None, iterable=None, initial=0, desc=None):
-    return tqdm(
-        iterable=iterable,
-        total=total,
-        initial=initial,
-        unit_scale=True,
-        unit_divisor=1024,
-        unit="B",
-        disable=False,
-        leave=False,
-        desc=desc,
-        # dynamic_ncols=True, # make this the default?
-    )
-
-
 def ensure_iterable(obj):
     import collections.abc
 
     if isinstance(obj, str) or not isinstance(obj, collections.abc.Iterable):
         return [obj]
     return obj
```

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/availability.py` & `earthkit_data-0.7.0/earthkit/data/utils/availability.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/bbox.py` & `earthkit_data-0.7.0/earthkit/data/utils/bbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,14 +73,20 @@
 
     def __eq__(self, other):
         if self.__class__ is not other.__class__:
             return False
 
         return self.as_tuple() == other.as_tuple()
 
+    @classmethod
+    def make_invalid(cls):
+        import numpy as np
+
+        return cls(north=np.nan, west=np.nan, south=np.nan, east=np.nan)
+
     @property
     def width(self):
         """number: Returns the East-West size (degrees)"""
         return self.east - self.west
 
     @property
     def height(self):
@@ -233,14 +239,22 @@
 
     def as_tuple(self):
         return (self.north, self.west, self.south, self.east)
 
     def as_dict(self):
         return dict(north=self.north, west=self.west, south=self.south, east=self.east)
 
+    @classmethod
+    def from_geopandas(cls, gdf):
+        try:
+            bb = gdf.crs.area_of_use.bounds
+            return BoundingBox(east=bb[0], south=bb[1], west=bb[2], north=bb[3])
+        except AttributeError:
+            return BoundingBox.make_invalid()
+
 
 def bounding_box(obj):
     if isinstance(obj, BoundingBox):
         return obj
 
     if isinstance(obj, (list, tuple)):
         return BoundingBox(north=obj[0], west=obj[1], south=obj[2], east=obj[3])
```

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/conventions.py` & `earthkit_data-0.7.0/earthkit/data/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/dates.py` & `earthkit_data-0.7.0/earthkit/data/utils/dates.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/examples.py` & `earthkit_data-0.7.0/earthkit/data/utils/examples.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/factorise.py` & `earthkit_data-0.7.0/earthkit/data/utils/factorise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/html.py` & `earthkit_data-0.7.0/earthkit/data/utils/html.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/humanize.py` & `earthkit_data-0.7.0/earthkit/data/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/interval.py` & `earthkit_data-0.7.0/earthkit/data/utils/interval.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/kwargs.py` & `earthkit_data-0.7.0/earthkit/data/utils/kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/lazy.py` & `earthkit_data-0.7.0/earthkit/data/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/message.py` & `earthkit_data-0.7.0/earthkit/data/utils/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             self._py_version = tuple([int(x) for x in v["bindings"].split(".")])
         except Exception:
             self._py_version = (0, 0, 0)
 
         LOG.debug(f"ecCodes versions: {self.versions}")
 
     def check_clone_kwargs(self, **kwargs):
-        if not (self._py_version >= (1, 7, 0) and self._version >= (2, 34, 0)):
+        if not (self._py_version >= (1, 7, 0) and self._version >= (2, 35, 0)):
             kwargs = dict(**kwargs)
             kwargs.pop("headers_only", None)
         return kwargs
 
     @property
     def versions(self):
         return f"ecCodes: {self._version} eccodes-python: {self._py_version}"
@@ -70,33 +70,63 @@
         return func(*args, **kwargs)
 
     return wrapped
 
 
 class CodesMessagePositionIndex:
     VERSION = 1
+    MAGIC = None
 
-    def __init__(self, path):
+    def __init__(self, path, parts=None):
         self.path = path
         self.offsets = None
         self.lengths = None
+        self.parts = parts
         self._cache_file = None
         self._load()
 
     def __len__(self):
         return len(self.offsets)
 
-    def _get_message_positions(self, path):
+    def _get_message_positions(self, path, parts):
+        fd = os.open(path, os.O_RDONLY)
+
+        try:
+            if parts is None:
+                yield from self._get_message_positions_part(fd, (0, -1))
+            else:
+                for part in parts:
+                    try:
+                        yield from self._get_message_positions_part(fd, part)
+                    except Exception:
+                        pass
+        except Exception:
+            pass
+        finally:
+            os.close(fd)
+
+    def _get_message_positions_part(self, path, part):
         raise NotImplementedError
 
+    @staticmethod
+    def _get_bytes(fd, count):
+        buf = os.read(fd, count)
+        if len(buf) != count:
+            raise Exception
+        return int.from_bytes(
+            buf,
+            byteorder="big",
+            signed=False,
+        )
+
     def _build(self):
         offsets = []
         lengths = []
 
-        for offset, length in self._get_message_positions(self.path):
+        for offset, length in self._get_message_positions(self.path, self.parts):
             offsets.append(offset)
             lengths.append(length)
 
         self.offsets = offsets
         self.lengths = lengths
 
     def _load(self):
```

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/metadata.py` & `earthkit_data-0.7.0/earthkit/data/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/module_inputs_wrapper.py` & `earthkit_data-0.7.0/earthkit/data/utils/module_inputs_wrapper.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/paths.py` & `earthkit_data-0.7.0/earthkit/data/utils/paths.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/patterns.py` & `earthkit_data-0.7.0/earthkit/data/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/projections/__init__.py` & `earthkit_data-0.7.0/earthkit/data/utils/projections/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
 try:
     import cartopy.crs as ccrs
 
     NO_CARTOPY = False
 except ImportError:
     NO_CARTOPY = True
-CARTOPY_WARNING = (
-    "no cartopy installation found; cartopy must be installed to use this feature"
-)
+
+CARTOPY_WARNING = "This feature requires 'cartopy' to be installed"
 
 
 DEFAULT_LATLON_PROJ_STRING = (
     "+proj=eqc +ellps=WGS84 +a=6378137.0 +lon_0=0.0 +to_meter=111319.4907932736 "
     "+no_defs +type=crs"
 )
 
@@ -111,14 +110,20 @@
 
 class LambertAzimuthalEqualArea(Projection):
     PROJ_NAME = "laea"
     CF_GRID_MAPPING_NAME = "lambert_azimuthal_equal_area"
     CARTOPY_CRS = "LambertAzimuthalEqualArea"
 
 
+class LambertConformal(Projection):
+    PROJ_NAME = "lcc"
+    CF_GRID_MAPPING_NAME = "lambert_conformal_conic"
+    CARTOPY_CRS = "LambertConformal"
+
+
 class AlbersEqualArea(Projection):
     PROJ_NAME = "aea"
     CF_GRID_MAPPING_NAME = "albers_conical_equal_area"
     CARTOPY_CRS = "AlbersEqualArea"
 
 
 class Mercator(Projection):
@@ -127,10 +132,11 @@
     CARTOPY_CRS = "Mercator"
 
 
 _PROJECTIONS = [
     EquidistantCylindrical,
     LongLat,
     LambertAzimuthalEqualArea,
+    LambertConformal,
     AlbersEqualArea,
     Mercator,
 ]
```

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/projections/cf.py` & `earthkit_data-0.7.0/earthkit/data/utils/projections/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/projections/proj.py` & `earthkit_data-0.7.0/earthkit/data/utils/projections/proj.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     "x_0": "false_easting",
     "y_0": "false_northing",
     "k": "scale_factor",
     "zone": "zone",
     "proj": "proj_name",
 }
 
+STANDARD_PARALLELS = ["lat_1", "lat_2"]
+
 PROJ_PARAMS_TO_GLOBE_KWARGS = {
     "a": "semimajor_axis",
     "b": "semiminor_axis",
     "datum": "datum",
     "ellps": "ellipse",
     "f": "flattening",
     "rf": "inverse_flattening",
@@ -59,8 +61,14 @@
     kwargs = {
         PROJ_PARAMS_TO_KWARGS[k]: v
         for k, v in proj_params.items()
         if k in PROJ_PARAMS_TO_KWARGS
     }
     kwargs["globe"] = globe_params
 
+    standard_parallels = tuple(
+        proj_params[param] for param in STANDARD_PARALLELS if param in proj_params
+    )
+    if standard_parallels:
+        kwargs["standard_parallels"] = standard_parallels
+
     return kwargs
```

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/serialise.py` & `earthkit_data-0.7.0/earthkit/data/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/summary.py` & `earthkit_data-0.7.0/earthkit/data/utils/summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/utils/url.py` & `earthkit_data-0.7.0/earthkit/data/utils/url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/vocabularies/__init__.py` & `earthkit_data-0.7.0/earthkit/data/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/vocabularies/aliases.py` & `earthkit_data-0.7.0/earthkit/data/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/vocabularies/cf.py` & `earthkit_data-0.7.0/earthkit/data/vocabularies/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/vocabularies/grib-paramid.csv` & `earthkit_data-0.7.0/earthkit/data/vocabularies/grib-paramid.csv`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/vocabularies/grib.py` & `earthkit_data-0.7.0/earthkit/data/vocabularies/grib.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/__init__.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/integer.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/integer.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/ndarray.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/pandas.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,19 +182,19 @@
 
 def wrapper(data, *args, **kwargs):
     import pandas as pd
 
     try:
         import geopandas as gpd
 
-        l_gpd = True
+        has_gpd = True
     except ImportError:
-        l_gpd = False
+        has_gpd = False
 
-    if l_gpd and isinstance(data, gpd.geodataframe.GeoDataFrame):
+    if has_gpd and isinstance(data, gpd.geodataframe.GeoDataFrame):
         return GeoPandasDataFrameWrapper(data, *args, **kwargs)
     if isinstance(data, pd.DataFrame):
         return PandasDataFrameWrapper(data, *args, **kwargs)
     if isinstance(data, pd.Series):
         return PandasSeriesWrapper(data, *args, **kwargs)
 
     return None
```

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/string.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/string.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/wrappers/xarray.py` & `earthkit_data-0.7.0/earthkit/data/wrappers/xarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 
 # from emohawk.metadata import AXES, COMPONENTS
 
-from earthkit.data.readers import netcdf
+# from earthkit.data.readers import netcdf
 from earthkit.data.wrappers import Wrapper
 
 
 class XArrayDataArrayWrapper(Wrapper):
     """Wrapper around an xarray `DataArray`, offering polymorphism and
     convenience methods.
     """
@@ -140,14 +140,16 @@
     elif isinstance(data, xr.DataArray):
         try:
             ds = data.to_dataset()
         except ValueError:
             return XArrayDataArrayWrapper(data, *args, **kwargs)
 
     if ds is not None:
-        fs = netcdf.XArrayFieldList(ds, **kwargs)
+        from earthkit.data.readers.netcdf.fieldlist import XArrayFieldList
+
+        fs = XArrayFieldList(ds, **kwargs)
         if fs.has_fields():
             return fs
         else:
             return XArrayDatasetWrapper(ds, *args, **kwargs)
 
     return None
```

### Comparing `earthkit-data-0.6.0/earthkit/data/writers/__init__.py` & `earthkit_data-0.7.0/earthkit/data/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/earthkit/data/writers/grib.py` & `earthkit_data-0.7.0/earthkit/data/writers/grib.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 
 from . import Writer
 
 
 class GribWriter(Writer):
     DATA_FORMAT = "grib"
 
-    def write(self, f, values, metadata, check_nans=True, bits_per_value=16):
+    def write(self, f, values, metadata, check_nans=True, bits_per_value=None):
         r"""Write a GRIB field to a file object.
 
         Parameters
         ----------
         f: file object
             The target file object.
         values: ndarray
             Values of the GRIB field.
         metadata: :class:`GribMetadata`
             Metadata of the GRIB field.
         check_nans: bool
-            Replace nans in ``values`` with GRIB missing values when writing to``f``.
-        bits_per_value: int
-            Set the ``bitsPerValue`` GRIB key in the generated GRIB message.
+            Replace nans in ``values`` with GRIB missing values when writing to ``f``.
+        bits_per_value: int or None
+            Set the ``bitsPerValue`` GRIB key in the generated GRIB message. When
+            None the ``bitsPerValue`` stored in the metadata will be used.
         """
         handle = metadata._handle.clone()
 
-        handle.set_long("bitsPerValue", bits_per_value)
+        if bits_per_value is None:
+            bits_per_value = metadata.get("bitsPerValue", 0)
+
+        if bits_per_value != 0:
+            handle.set_long("bitsPerValue", bits_per_value)
 
         if check_nans:
             import numpy as np
 
             if np.isnan(values).any():
                 missing_value = handle.MISSING_VALUE
                 values = np.nan_to_num(values, nan=missing_value)
```

### Comparing `earthkit-data-0.6.0/earthkit_data.egg-info/SOURCES.txt` & `earthkit_data-0.7.0/earthkit_data.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 .github/workflows/label-public-pr.yml
 .github/workflows/notify-new-issue.yml
 .github/workflows/notify-new-pr.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/development.rst
-docs/examples.rst
 docs/howtos.rst
 docs/index.rst
 docs/install.rst
 docs/licence.rst
 docs/make.bat
 docs/requirements.txt
 docs/skip_api_rules.py
@@ -33,83 +32,93 @@
 docs/_static/style.css
 docs/_templates/.gitkeep
 docs/examples/ads.ipynb
 docs/examples/bufr_synop.ipynb
 docs/examples/bufr_temp.ipynb
 docs/examples/cache.ipynb
 docs/examples/cds.ipynb
+docs/examples/data_from_stream.ipynb
 docs/examples/default_fdb_schema
 docs/examples/demo_sources_plugin.ipynb
 docs/examples/ecmwf_open_data.ipynb
 docs/examples/fdb.ipynb
+docs/examples/file_parts.ipynb
+docs/examples/files.ipynb
 docs/examples/from_object.ipynb
+docs/examples/geojson_geopandas.ipynb
+docs/examples/grib_array_backends.ipynb
 docs/examples/grib_fdb_write.ipynb
-docs/examples/grib_file_pattern.ipynb
-docs/examples/grib_from_stream.ipynb
 docs/examples/grib_indexing.ipynb
 docs/examples/grib_lat_lon_value.ipynb
 docs/examples/grib_metadata.ipynb
 docs/examples/grib_missing.ipynb
-docs/examples/grib_multi.ipynb
 docs/examples/grib_nearest_gridpoint.ipynb
 docs/examples/grib_overview.ipynb
 docs/examples/grib_selection.ipynb
-docs/examples/grib_tar.ipynb
 docs/examples/grib_time_series.ipynb
 docs/examples/grib_to_netcdf.ipynb
-docs/examples/grib_url.ipynb
-docs/examples/grib_url_stream.ipynb
+docs/examples/index.rst
 docs/examples/list_of_dict.ipynb
 docs/examples/mars.ipynb
 docs/examples/metadata.ipynb
 docs/examples/missing.grib
+docs/examples/multi_files.ipynb
 docs/examples/netcdf.ipynb
 docs/examples/netcdf_fieldlist.ipynb
+docs/examples/netcdf_opendap.ipynb
 docs/examples/numpy_fieldlist.ipynb
 docs/examples/odb.ipynb
 docs/examples/pandas.ipynb
 docs/examples/polytope.ipynb
 docs/examples/projection.ipynb
 docs/examples/settings.ipynb
+docs/examples/shapefile.ipynb
 docs/examples/synop_10.bufr
+docs/examples/tar_files.ipynb
 docs/examples/temp_10.bufr
 docs/examples/test.grib
 docs/examples/test.nc
 docs/examples/test.odb
 docs/examples/test4.grib
 docs/examples/test6.grib
 docs/examples/time_series.grib
 docs/examples/tuv_pl.grib
 docs/examples/tuv_pl.nc
+docs/examples/url.ipynb
+docs/examples/url_parts.ipynb
+docs/examples/url_stream.ipynb
 docs/examples/wekeo.ipynb
 docs/guide/caching.rst
 docs/guide/data.rst
 docs/guide/index.rst
 docs/guide/settings.rst
 docs/guide/sources.rst
-docs/guide/split_on.rst
 docs/guide/data_format/bufr.rst
 docs/guide/data_format/csv.rst
 docs/guide/data_format/grib.rst
 docs/guide/data_format/index.rst
 docs/guide/data_format/netcdf.rst
 docs/guide/data_format/odb.rst
 docs/guide/include/settings-get.py
 docs/guide/include/settings-reset.py
 docs/guide/include/settings-set.py
 docs/guide/include/settings-temporary.py
+docs/guide/misc/index.rst
+docs/guide/misc/parts.rst
+docs/guide/misc/split_on.rst
 docs/plugins/index.rst
 docs/plugins/plugins.rst
 docs/plugins/sources_plugin.rst
 docs/release_notes/index.rst
 docs/release_notes/version_0.2_updates.rst
 docs/release_notes/version_0.3_updates.rst
 docs/release_notes/version_0.4_updates.rst
 docs/release_notes/version_0.5_updates.rst
 docs/release_notes/version_0.6_updates.rst
+docs/release_notes/version_0.7_updates.rst
 earthkit/data/__init__.py
 earthkit/data/decorators.py
 earthkit/data/testing.py
 earthkit/data/version.py
 earthkit/data/arguments/__init__.py
 earthkit/data/arguments/args_kwargs.py
 earthkit/data/arguments/argument.py
@@ -134,16 +143,14 @@
 earthkit/data/core/order.py
 earthkit/data/core/plugins.py
 earthkit/data/core/select.py
 earthkit/data/core/settings.py
 earthkit/data/core/statistics.py
 earthkit/data/core/temporary.py
 earthkit/data/core/thread.py
-earthkit/data/geo/__init__.py
-earthkit/data/geo/distance.py
 earthkit/data/indexing/__init__.py
 earthkit/data/indexing/database/__init__.py
 earthkit/data/indexing/database/json.py
 earthkit/data/indexing/database/sql.py
 earthkit/data/indexing/database/stdout.py
 earthkit/data/mergers/__init__.py
 earthkit/data/mergers/pandas.py
@@ -152,17 +159,17 @@
 earthkit/data/mirrors/directory_mirror.py
 earthkit/data/readers/__init__.py
 earthkit/data/readers/archive.py
 earthkit/data/readers/covjson.py
 earthkit/data/readers/csv.py
 earthkit/data/readers/directory.py
 earthkit/data/readers/geojson.py
-earthkit/data/readers/netcdf.py
 earthkit/data/readers/numpy.py
 earthkit/data/readers/odb.py
+earthkit/data/readers/shapefile.py
 earthkit/data/readers/tar.py
 earthkit/data/readers/text.py
 earthkit/data/readers/unknown.py
 earthkit/data/readers/zip.py
 earthkit/data/readers/bufr/__init__.py
 earthkit/data/readers/bufr/bufr.py
 earthkit/data/readers/bufr/pandas.py
@@ -177,16 +184,22 @@
 earthkit/data/readers/grib/reader.py
 earthkit/data/readers/grib/xarray.py
 earthkit/data/readers/grib/index/__init__.py
 earthkit/data/readers/grib/index/db.py
 earthkit/data/readers/grib/index/file.py
 earthkit/data/readers/grib/index/json.py
 earthkit/data/readers/grib/index/sql.py
+earthkit/data/readers/netcdf/__init__.py
+earthkit/data/readers/netcdf/coords.py
+earthkit/data/readers/netcdf/dataset.py
+earthkit/data/readers/netcdf/field.py
+earthkit/data/readers/netcdf/fieldlist.py
 earthkit/data/sources/__init__.py
 earthkit/data/sources/ads.py
+earthkit/data/sources/array_list.py
 earthkit/data/sources/cds.py
 earthkit/data/sources/constants.py
 earthkit/data/sources/dummy.grib
 earthkit/data/sources/dummy_source.py
 earthkit/data/sources/ecmwf_api.py
 earthkit/data/sources/ecmwf_open_data.py
 earthkit/data/sources/empty.py
@@ -197,16 +210,18 @@
 earthkit/data/sources/indexed.py
 earthkit/data/sources/list_of_dicts.py
 earthkit/data/sources/mars.py
 earthkit/data/sources/memory.py
 earthkit/data/sources/multi.py
 earthkit/data/sources/multi_url.py
 earthkit/data/sources/numpy_list.py
+earthkit/data/sources/opendap.py
 earthkit/data/sources/polytope.py
 earthkit/data/sources/prompt.py
+earthkit/data/sources/sample.py
 earthkit/data/sources/stream.py
 earthkit/data/sources/url.py
 earthkit/data/sources/url_pattern.py
 earthkit/data/sources/virtual.py
 earthkit/data/sources/virtual_directory.py
 earthkit/data/sources/wekeo.py
 earthkit/data/sources/wekeocds.py
@@ -233,17 +248,22 @@
 earthkit/data/utils/lazy.py
 earthkit/data/utils/message.py
 earthkit/data/utils/metadata.py
 earthkit/data/utils/module_inputs_wrapper.py
 earthkit/data/utils/parts.py
 earthkit/data/utils/paths.py
 earthkit/data/utils/patterns.py
+earthkit/data/utils/progbar.py
 earthkit/data/utils/serialise.py
 earthkit/data/utils/summary.py
 earthkit/data/utils/url.py
+earthkit/data/utils/array/__init__.py
+earthkit/data/utils/array/cupy.py
+earthkit/data/utils/array/numpy.py
+earthkit/data/utils/array/pytorch.py
 earthkit/data/utils/projections/__init__.py
 earthkit/data/utils/projections/cf.py
 earthkit/data/utils/projections/proj.py
 earthkit/data/vocabularies/__init__.py
 earthkit/data/vocabularies/aliases.py
 earthkit/data/vocabularies/cf.py
 earthkit/data/vocabularies/grib-paramid.csv
@@ -261,17 +281,24 @@
 earthkit_data.egg-info/dependency_links.txt
 earthkit_data.egg-info/requires.txt
 earthkit_data.egg-info/top_level.txt
 tests/conftest.py
 tests/downstream-ci-requirements.txt
 tests/environment-unit-tests.yml
 tests/test_00_version.py
+tests/array_fieldlist/array_fl_fixtures.py
+tests/array_fieldlist/test_numpy_fl_write.py
+tests/array_fieldlist/test_numpy_fs.py
+tests/array_fieldlist/test_numpy_fs_concat.py
+tests/array_fieldlist/test_numpy_fs_metadata.py
+tests/array_fieldlist/test_numpy_fs_summary.py
 tests/bufr/test_bufr_concat.py
 tests/bufr/test_bufr_contents.py
 tests/bufr/test_bufr_convert.py
+tests/bufr/test_bufr_file_parts.py
 tests/bufr/test_bufr_order_by.py
 tests/bufr/test_bufr_sel.py
 tests/bufr/test_bufr_summary.py
 tests/constants/constants_fixtures.py
 tests/constants/test_constants_metadata.py
 tests/constants/test_constants_sel.py
 tests/constants/test_constants_slice.py
@@ -281,16 +308,18 @@
 tests/core/test_cache.py
 tests/core/test_gridspec.py
 tests/core/test_metadata.py
 tests/core/test_settings.py
 tests/core/test_version.py
 tests/data/NUTS_RG_20M_2021_3035.geojson
 tests/data/NUTS_RG_20M_2021_3035.shp.zip
+tests/data/empty_file.grib
 tests/data/era5_2t_1.nc
 tests/data/era5_2t_2.nc
+tests/data/hovexp_vert_area.nc
 tests/data/mercator.grib
 tests/data/ml_data.grib
 tests/data/rgg_small_subarea_cellarea_ref.grib
 tests/data/t_pl.grib
 tests/data/t_time_series.grib
 tests/data/test_icon.grib
 tests/data/test_single.grib
@@ -308,19 +337,19 @@
 tests/data/gridspec/regular_ll.yaml
 tests/data/gridspec/rotated_gg.yaml
 tests/data/gridspec/rotated_ll.yaml
 tests/data/gridspec/sh.yaml
 tests/data/gridspec/t_75_-60_10_40_5x5.grib1
 tests/documentation/test_examples.py
 tests/documentation/test_notebooks.py
-tests/geo/geo_fixtures.py
-tests/geo/test_geo.py
 tests/grib/grib_fixtures.py
+tests/grib/test_grib_backend.py
 tests/grib/test_grib_concat.py
 tests/grib/test_grib_convert.py
+tests/grib/test_grib_file_parts.py
 tests/grib/test_grib_geography.py
 tests/grib/test_grib_gridspec.py
 tests/grib/test_grib_inidces.py
 tests/grib/test_grib_memory.py
 tests/grib/test_grib_metadata.py
 tests/grib/test_grib_order_by.py
 tests/grib/test_grib_output.py
@@ -335,17 +364,19 @@
 tests/indexing/test_indexing_db.py
 tests/indexing/test_indexing_isel.py
 tests/indexing/test_indexing_order_by.py
 tests/indexing/test_indexing_serialisation.py
 tests/indexing/test_order_kwargs.py
 tests/indexing/test_selection_kwargs.py
 tests/netcdf/test_netcdf_concat.py
+tests/netcdf/test_netcdf_convert.py
 tests/netcdf/test_netcdf_fieldlist.py
 tests/netcdf/test_netcdf_geography.py
 tests/netcdf/test_netcdf_metadata.py
+tests/netcdf/test_netcdf_opendap.py
 tests/netcdf/test_netcdf_output.py
 tests/netcdf/test_netcdf_sel.py
 tests/netcdf/test_netcdf_slice.py
 tests/netcdf/test_netcdf_summary.py
 tests/netcdf/test_netcdf_values.py
 tests/normalize/aliases.json
 tests/normalize/availability.json
@@ -355,52 +386,51 @@
 tests/normalize/test_normalize_bbox.py
 tests/normalize/test_normalize_date.py
 tests/normalize/test_normalize_enum.py
 tests/normalize/test_normalize_errors.py
 tests/normalize/test_normalize_kwargs.py
 tests/normalize/test_normalize_parameter.py
 tests/normalize/test_transformers.py
-tests/numpy_fs/numpy_fs_fixtures.py
-tests/numpy_fs/test_numpy_fs.py
-tests/numpy_fs/test_numpy_fs_concat.py
-tests/numpy_fs/test_numpy_fs_metadata.py
-tests/numpy_fs/test_numpy_fs_summary.py
-tests/numpy_fs/test_numpy_fs_write.py
 tests/plugins/test_sources_plugin.py
 tests/readers/test_covjson_reader.py
 tests/readers/test_csv_reader.py
+tests/readers/test_empty_file.py
 tests/readers/test_geojson_reader.py
 tests/readers/test_grib_reader.py
 tests/readers/test_netcdf_reader.py
 tests/readers/test_odb_reader.py
 tests/readers/test_reader_padding_bytes.py
+tests/readers/test_shapefile_reader.py
 tests/readers/test_tar_reader.py
 tests/readers/test_unknown_reader.py
 tests/readers/test_zip_reader.py
 tests/readers/unknown_file.unknown_ext
 tests/readers/unknown_text_file.unknown_ext
 tests/sources/test_ads.py
 tests/sources/test_cds.py
 tests/sources/test_ecmwf_open_data.py
 tests/sources/test_fdb.py
 tests/sources/test_file.py
 tests/sources/test_list_of_dicts.py
 tests/sources/test_mars.py
 tests/sources/test_multi.py
 tests/sources/test_polytope.py
+tests/sources/test_samples.py
 tests/sources/test_url.py
 tests/sources/test_url_pattern.py
 tests/sources/test_wekeo.py
 tests/sources/test_wekeocds.py
 tests/translators/test_translators.py
 tests/utils/__init__.py
 tests/utils/dummy_module.py
+tests/utils/test_array.py
 tests/utils/test_bbox.py
 tests/utils/test_dates.py
 tests/utils/test_download_examples.py
 tests/utils/test_interval.py
 tests/utils/test_module_inputs_wrapper.py
+tests/utils/test_parts.py
 tests/utils/test_projections.py
 tests/wrappers/test_ndarray.py
 tests/wrappers/test_pandas.py
 tests/wrappers/test_string.py
 tests/wrappers/test_xarray.py
```

### Comparing `earthkit-data-0.6.0/environment.yml` & `earthkit_data-0.7.0/environment.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: earthkit-data
 channels:
 - conda-forge
 - nodefaults
 dependencies:
-- eccodes=>2.34.1
+- eccodes=>2.35.0
 - python-eccodes>=1.7.0
 - pip
 - numpy
 - pandas
 - xarray>=0.19.0
 - dask
 - netcdf4
@@ -17,23 +17,23 @@
 - filelock
 - pyyaml
 - entrypoints
 - jupyterlab
 - ecmwf-api-client>=1.6.1
 - cdsapi
 - hda
-- scipy
 - pip:
-  - git+https://github.com/ecmwf/multiurl
+  - multiurl
   - git+https://github.com/ecmwf/pyfdb
   - ecmwf-opendata>=0.1.2
-  - polytope-client>=0.7.2
+  - polytope-client>=0.7.4
   - earthkit-meteo>=0.0.1
   - eccovjson>=0.0.5
-- tqdm
+  - earthkit-geo
+- tqdm>=4.63.0
 - markdown
 - make
 - mypy
 - myst-parser
 - pre-commit
 - pydata-sphinx-theme
 - pytest
```

### Comparing `earthkit-data-0.6.0/pytest.ini` & `earthkit_data-0.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/setup.cfg` & `earthkit_data-0.7.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -17,46 +17,59 @@
 long_description_content_type = text/markdown
 long_description = file: README.md
 test_suite = tests
 
 [options]
 packages = find_namespace:
 install_requires = 
-	cdsapi
 	cfgrib>=0.9.10.1
 	eccodes>=1.7.0
-	ecmwf-api-client>=1.6.1
-	ecmwf-opendata>=0.1.2
-	polytope-client>=0.7.2
 	dask
 	entrypoints
 	filelock
-	hda
 	jinja2
+	jsonschema
 	markdown
 	multiurl
 	netcdf4
+	pandas
 	pdbufr>=0.11.0
-	pyfdb
-	pyodc
 	pyyaml
-	scipy
-	tqdm
+	tqdm>=4.63.0
 	xarray>=0.19.0
 	earthkit-meteo>=0.0.1
-	aws-requests-auth
-	eccovjson>=0.0.5
-	jsonschema
 include_package_data = True
 
 [options.packages.find]
 include = earthkit.*
 
 [options.extras_require]
+mars = ecmwf-api-client>=1.6.1
+cds = cdsapi
+fdb = pyfdb
+polytope = polytope-client>=0.7.4
+wekeo = hda
+ecmwf-opendata = ecmwf-opendata>=0.3.3
+odb = pyodc
+projection = cartopy
+geopandas = geopandas
+eccovjson = eccovjson>=0.0.5
+all = 
+	earthkit-data[mars]
+	earthkit-data[cds]
+	earthkit-data[ecmwf-opendata]
+	earthkit-data[fdb]
+	earthkit-data[polytope]
+	earthkit-data[wekeo]
+	earthkit-data[odb]
+	earthkit-data[projection]
+	earthkit-data[geopandas]
+	earthkit-data[eccovjson]
 test = 
+	earthkit-data[all]
 	pytest
 	pytest-cov
 	pytest-forked
 	pytest-timeout
 	nbformat
 	nbconvert
```

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_concat.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_contents.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_contents.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_convert.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_order_by.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_sel.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_sel.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/bufr/test_bufr_summary.py` & `earthkit_data-0.7.0/tests/bufr/test_bufr_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/conftest.py` & `earthkit_data-0.7.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     "short": ["download", "ftp", "long_test"],
     "long": ["ftp"],
     "release": [],
     "documentation": None,
 }
 
 
+def pytest_configure(config):
+    pytest.CDS_TIMEOUT = config.getoption("--cds-timeout")
+
+
 def pytest_addoption(parser):
     help_str = "NAME: short, long, release, documentation. Runs a subset of tests.\n"
     for k, v in SKIP.items():
         if v:
             help_str += f"'{k}': skip tests marked as {','.join(v)}.\n"
         else:
             help_str += f"'{k}': do not skip tests.\n"
@@ -20,14 +24,22 @@
         "-E",
         action="store",
         metavar="NAME",
         default="short",
         help=help_str,
     )
 
+    parser.addoption(
+        "--cds-timeout",
+        action="store",
+        metavar="TIMEOUT",
+        default=30,
+        help="Timeout in seconds for cds tests. 0 means no timeout. Default is 30.",
+    )
+
 
 def pytest_runtest_setup(item):
     # print(f"config {item.config.option}")
     flag = item.config.getoption("-E")
     marks_to_skip = SKIP[flag]
 
     marks_in_items = list([m.name for m in item.iter_markers()])
```

### Comparing `earthkit-data-0.6.0/tests/constants/constants_fixtures.py` & `earthkit_data-0.7.0/tests/constants/constants_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_constants_metadata.py` & `earthkit_data-0.7.0/tests/constants/test_constants_metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_constants_sel.py` & `earthkit_data-0.7.0/tests/constants/test_constants_sel.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_constants_slice.py` & `earthkit_data-0.7.0/tests/constants/test_constants_slice.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_constants_source.py` & `earthkit_data-0.7.0/tests/constants/test_constants_source.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_constants_values.py` & `earthkit_data-0.7.0/tests/constants/test_constants_values.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/constants/test_contants_proc.py` & `earthkit_data-0.7.0/tests/constants/test_contants_proc.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/core/test_cache.py` & `earthkit_data-0.7.0/tests/core/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -324,11 +324,54 @@
             cache.purge()
             num, size = cache.summary_dump_database()
             assert num == 0
             assert size == 0
             assert len(cache.entries()) == 0
 
 
+@pytest.mark.cache
+def test_cache_force():
+    import time
+
+    def _force_true(args, path, owner_data):
+        time.sleep(0.001)
+        return True
+
+    def _force_false(args, path, owner_data):
+        time.sleep(0.001)
+        return False
+
+    data_size = 10 * 1024
+    ds = from_source("dummy-source", "zeros", size=data_size, n=0)
+    st = os.stat(ds.path)
+    m_time_ref = st.st_mtime_ns
+
+    ds1 = from_source("dummy-source", "zeros", size=data_size, n=0)
+    assert ds1.path == ds.path
+    st = os.stat(ds1.path)
+    m_time = st.st_mtime_ns
+    assert m_time == m_time_ref
+
+    ds2 = from_source("dummy-source", "zeros", force=_force_false, size=data_size, n=0)
+    assert ds2.path == ds.path
+    st = os.stat(ds2.path)
+    m_time = st.st_mtime_ns
+    assert m_time == m_time_ref
+
+    ds3 = from_source("dummy-source", "zeros", force=_force_true, size=data_size, n=0)
+    assert ds3.path == ds.path
+    st = os.stat(ds3.path)
+    m_time = st.st_mtime_ns
+    assert m_time != m_time_ref
+    m_time_ref = m_time
+
+    ds4 = from_source("dummy-source", "zeros", size=data_size, n=0)
+    assert ds4.path == ds.path
+    st = os.stat(ds4.path)
+    m_time = st.st_mtime_ns
+    assert m_time == m_time_ref
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/core/test_gridspec.py` & `earthkit_data-0.7.0/tests/core/test_gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/core/test_metadata.py` & `earthkit_data-0.7.0/tests/core/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,11 +253,45 @@
 
     # invalid value
     with pytest.raises(Exception) as e:
         md.override({"level": -100})
     assert "EncodingError" in e.typename
 
 
+def test_grib_metadata_override_extra():
+    ds = from_source("file", earthkit_examples_file("test.grib"))
+    md = ds[0].metadata()
+    md_num = len(md)
+
+    assert md["perturbationNumber"] == 0
+    assert md["shortName"] == "2t"
+
+    extra = {"my_custom_key": "2", "shortName": "N", "perturbationNumber": 2}
+    md = GribMetadata(md._handle, extra=extra)
+
+    assert md["my_custom_key"] == "2"
+    assert md["perturbationNumber"] == 2
+    assert md["shortName"] == "N"
+    assert md["typeOfLevel"] == "surface"
+
+    keys = md.keys()
+    assert len(keys) == md_num + 1
+
+    for k in md.keys():
+        assert isinstance(k, str)
+        assert k != ""
+        break
+
+    items = md.items()
+    assert len(items) == md_num + 1
+
+    for k, v in md.items():
+        assert isinstance(k, str)
+        assert k != ""
+        assert v is not None
+        break
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/core/test_settings.py` & `earthkit_data-0.7.0/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/core/test_version.py` & `earthkit_data-0.7.0/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/NUTS_RG_20M_2021_3035.geojson` & `earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.geojson`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip` & `earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/constants/proc.yaml` & `earthkit_data-0.7.0/tests/data/constants/proc.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/era5_2t_1.nc` & `earthkit_data-0.7.0/tests/data/era5_2t_1.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/era5_2t_2.nc` & `earthkit_data-0.7.0/tests/data/era5_2t_2.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/healpix.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/healpix.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/reduced_gg.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/reduced_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/reduced_ll.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/reduced_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/reduced_rotated_gg.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/reduced_rotated_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/regular_gg.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/regular_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/regular_ll.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/regular_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/rotated_gg.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/rotated_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/rotated_ll.yaml` & `earthkit_data-0.7.0/tests/data/gridspec/rotated_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1` & `earthkit_data-0.7.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/mercator.grib` & `earthkit_data-0.7.0/tests/data/mercator.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/ml_data.grib` & `earthkit_data-0.7.0/tests/data/ml_data.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/rgg_small_subarea_cellarea_ref.grib` & `earthkit_data-0.7.0/tests/data/rgg_small_subarea_cellarea_ref.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/t_pl.grib` & `earthkit_data-0.7.0/tests/data/t_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/t_time_series.grib` & `earthkit_data-0.7.0/tests/data/t_time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/test_icon.grib` & `earthkit_data-0.7.0/tests/data/test_icon.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/test_single.nc` & `earthkit_data-0.7.0/tests/data/test_single.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/time_series.covjson` & `earthkit_data-0.7.0/tests/data/time_series.covjson`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/u_pl.grib` & `earthkit_data-0.7.0/tests/data/u_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/data/v_pl.grib` & `earthkit_data-0.7.0/tests/data/v_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/documentation/test_examples.py` & `earthkit_data-0.7.0/tests/documentation/test_examples.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/documentation/test_notebooks.py` & `earthkit_data-0.7.0/tests/documentation/test_notebooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import os
 import re
 import sys
 
 import pytest
 
-from earthkit.data.testing import MISSING, earthkit_file
+from earthkit.data.testing import MISSING, NO_PYTORCH, earthkit_file
 
 # See https://www.blog.pythonlibrary.org/2018/10/16/testing-jupyter-notebooks/
 
 
 EXAMPLES = earthkit_file("docs", "examples")
 
 SKIP = [
@@ -27,16 +27,21 @@
     "mars.ipynb",
     "cds.ipynb",
     "ads.ipynb",
     "wekeo.ipynb",
     "polytope.ipynb",
     "grib_fdb_write.ipynb",
     "demo_source_plugin.ipynb",
+    "ecmwf_open_data.ipynb",
+    "shapefile.ipynb",
 ]
 
+if NO_PYTORCH:
+    SKIP.append("grib_array_backends.ipynb")
+
 
 def notebooks_list():
     notebooks = []
     for path in os.listdir(EXAMPLES):
         if re.match(r".+\.ipynb$", path):
             # if re.match(r"^\d\d-.*\.ipynb$", path):
             if "Copy" not in path:
```

### Comparing `earthkit-data-0.6.0/tests/environment-unit-tests.yml` & `earthkit_data-0.7.0/tests/environment-unit-tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: earthkit-data
 channels:
 - conda-forge
 - nodefaults
 dependencies:
-- eccodes=>2.34.1
+- eccodes=>2.35.0
 - python-eccodes>=1.7.0
 - pip
 - numpy
 - pandas
 - xarray>=0.19.0
 - cartopy
 - dask
@@ -18,25 +18,25 @@
 - filelock
 - pyyaml
 - entrypoints
 - jupyterlab
 - ecmwf-api-client>=1.6.1
 - cdsapi
 - hda
-- scipy
 - jsonschema
 - pip:
-  - git+https://github.com/ecmwf/multiurl
+  - multiurl
   - git+https://github.com/ecmwf/pyfdb
-  - ecmwf-opendata>=0.1.2
-  - polytope-client>=0.7.2
+  - ecmwf-opendata>=0.3.3
+  - polytope-client>=0.7.4
   - earthkit-meteo>=0.0.1
   - git+https://github.com/ecmwf/earthkit-data-demo-source
   - eccovjson>=0.0.5
-- tqdm
+  - earthkit-geo
+- tqdm>=4.63.0
 - markdown
 - make
 - mypy
 - myst-parser
 - pre-commit
 - pydata-sphinx-theme
 - pytest
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_concat.py` & `earthkit_data-0.7.0/tests/grib/test_grib_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_convert.py` & `earthkit_data-0.7.0/tests/grib/test_grib_convert.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,50 +13,53 @@
 import sys
 
 import numpy as np
 import pytest
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
+from grib_fixtures import FL_TYPES, load_grib_data  # noqa: E402
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_icon_to_xarray(mode):
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
+def test_icon_to_xarray(fl_type, array_backend):
     # test the conversion to xarray for an icon (unstructured grid) grib file.
-    g = load_file_or_numpy_fs("test_icon.grib", mode, folder="data")
+    g = load_grib_data("test_icon.grib", fl_type, array_backend, folder="data")
 
     ds = g.to_xarray()
     assert len(ds.data_vars) == 1
     # Dataset contains 9 levels and 9 grid points per level
     ref_levs = g.metadata("level")
     assert ds["pres"].sizes["generalVerticalLayer"] == len(ref_levs)
     assert ds["pres"].sizes["values"] == 6
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_to_xarray_filter_by_keys(mode):
-    g = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
+def test_to_xarray_filter_by_keys(fl_type, array_backend):
+    g = load_grib_data("tuv_pl.grib", fl_type, array_backend)
     g = g.sel(param="t", level=500) + g.sel(param="u")
     assert len(g) > 1
 
     # see github #250
     r = g.to_xarray(
         xarray_open_dataset_kwargs={
             "backend_kwargs": {"filter_by_keys": {"shortName": "t"}}
         }
     )
 
     assert len(r.data_vars) == 1
     assert r["t"].sizes["isobaricInhPa"] == 1
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_pandas(mode):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
+def test_grib_to_pandas(fl_type, array_backend):
+    f = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
 
     # all points
     df = f.to_pandas()
     assert len(df) == 84
     cols = [
         "lat",
         "lon",
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_geography.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_geography.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,216 +5,242 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import os
-import sys
-
 import numpy as np
 import pytest
 
+from earthkit.data import from_source
+from earthkit.data.testing import (
+    earthkit_examples_file,
+    earthkit_remote_test_data_file,
+    earthkit_test_data_file,
+)
 from earthkit.data.utils import projections
 
-here = os.path.dirname(__file__)
-sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
-
 
 def check_array(v, shape=None, first=None, last=None, meanv=None, eps=1e-3):
     assert v.shape == shape
     assert np.isclose(v[0], first, eps)
     assert np.isclose(v[-1], last, eps)
     assert np.isclose(v.mean(), meanv, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("index", [0, None])
-def test_grib_to_latlon_single(mode, index):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+@pytest.mark.parametrize(
+    "dtype,expected_dtype",
+    [(None, np.float64), (np.float32, np.float32), (np.float64, np.float64)],
+)
+def test_netcdf_to_points_1(dtype, expected_dtype):
+    ds = from_source("file", earthkit_test_data_file("test_single.nc"))
 
     eps = 1e-5
-    g = f[index] if index is not None else f
-    v = g.to_latlon(flatten=True)
+
+    v = ds[0].to_points(flatten=True, dtype=dtype)
     assert isinstance(v, dict)
-    assert isinstance(v["lon"], np.ndarray)
-    assert isinstance(v["lat"], np.ndarray)
-    assert v["lon"].dtype == np.float64
-    assert v["lat"].dtype == np.float64
+    assert isinstance(v["x"], np.ndarray)
+    assert isinstance(v["y"], np.ndarray)
+    assert v["x"].dtype == expected_dtype
+    assert v["y"].dtype == expected_dtype
     check_array(
-        v["lon"],
+        v["x"],
         (84,),
         first=0.0,
         last=330.0,
         meanv=165.0,
         eps=eps,
     )
     check_array(
-        v["lat"],
+        v["y"],
         (84,),
         first=90,
         last=-90,
         meanv=0,
         eps=eps,
     )
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("index", [0, None])
-def test_grib_to_latlon_single_shape(mode, index):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+def test_netcdf_to_points_2():
+    ds = from_source("file", earthkit_examples_file("test.nc"))
 
-    g = f[index] if index is not None else f
-    v = g.to_latlon()
-    assert isinstance(v, dict)
-    assert isinstance(v["lon"], np.ndarray)
-    assert isinstance(v["lat"], np.ndarray)
+    assert len(ds) == 2
 
-    # x
-    assert v["lon"].shape == (7, 12)
-    assert v["lon"].dtype == np.float64
-    for x in v["lon"]:
-        assert np.allclose(x, np.linspace(0, 330, 12))
-
-    # y
-    assert v["lat"].shape == (7, 12)
-    assert v["lon"].dtype == np.float64
-    for i, y in enumerate(v["lat"]):
-        assert np.allclose(y, np.ones(12) * (90 - i * 30))
-
-
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("dtype", [np.float32, np.float64])
-def test_grib_to_latlon_multi(mode, dtype):
-    f = load_file_or_numpy_fs("test.grib", mode)
+    import xarray as xr
 
-    v_ref = f[0].to_latlon(flatten=True, dtype=dtype)
-    v = f.to_latlon(flatten=True, dtype=dtype)
-    assert isinstance(v, dict)
-    assert v.keys() == v_ref.keys()
+    xr_ds = xr.open_dataset(earthkit_examples_file("test.nc"))
 
-    assert isinstance(v, dict)
-    assert np.allclose(v["lat"], v_ref["lat"])
-    assert np.allclose(v["lon"], v_ref["lon"])
-    assert v["lat"].dtype == dtype
-    assert v["lon"].dtype == dtype
-
-
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_latlon_multi_non_shared_grid(mode):
-    f1 = load_file_or_numpy_fs("test.grib", mode)
-    f2 = load_file_or_numpy_fs("test4.grib", mode)
-    f = f1 + f2
-
-    with pytest.raises(ValueError):
-        f.to_latlon()
-
-
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("index", [0, None])
-def test_grib_to_points_single(mode, index):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+    for f in ds:
+        v = f.to_points()
+        assert isinstance(v, dict)
 
-    eps = 1e-5
-    g = f[index] if index is not None else f
-    v = g.to_points(flatten=True)
-    assert isinstance(v, dict)
-    assert isinstance(v["x"], np.ndarray)
-    assert isinstance(v["y"], np.ndarray)
-    assert v["x"].dtype == np.float64
-    assert v["y"].dtype == np.float64
-    check_array(
-        v["x"],
-        (84,),
-        first=0.0,
-        last=330.0,
-        meanv=165.0,
-        eps=eps,
-    )
-    check_array(
-        v["y"],
-        (84,),
-        first=90,
-        last=-90,
-        meanv=0,
-        eps=eps,
-    )
+        # x
+        assert isinstance(v["x"], np.ndarray)
+        assert v["x"].shape == (11, 19)
+        for x in v["x"]:
+            assert np.allclose(x, np.arange(-27, 45 + 4, 4))
 
+        # y
+        assert isinstance(v["y"], np.ndarray)
+        assert v["y"].shape == (11, 19)
+        for i, y in enumerate(v["y"]):
+            assert np.allclose(y, np.ones(19) * (73 - i * 4))
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_points_unsupported_grid(mode):
-    f = load_file_or_numpy_fs("mercator.grib", mode, folder="data")
-    with pytest.raises(ValueError):
-        f[0].to_points()
+        ref = xr_ds[f.name].sel(latitude=57, longitude=-7).values
 
+        x = 5
+        y = 4
+        assert np.isclose(f.to_numpy()[y, x], ref)
+        assert np.isclose(v["x"][y, x], -7)
+        assert np.isclose(v["y"][y, x], 57)
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("dtype", [np.float32, np.float64])
-def test_grib_to_points_multi(mode, dtype):
-    f = load_file_or_numpy_fs("test.grib", mode)
 
-    v_ref = f[0].to_points(flatten=True, dtype=dtype)
-    v = f.to_points(flatten=True, dtype=dtype)
-    assert isinstance(v, dict)
-    assert v.keys() == v_ref.keys()
+def test_netcdf_to_latlon():
+    ds = from_source("file", earthkit_examples_file("test.nc"))
 
-    assert isinstance(v, dict)
-    assert np.allclose(v["x"], v_ref["x"])
-    assert np.allclose(v["y"], v_ref["y"])
-    assert v["x"].dtype == dtype
-    assert v["y"].dtype == dtype
+    assert len(ds) == 2
+
+    import xarray as xr
+
+    xr_ds = xr.open_dataset(earthkit_examples_file("test.nc"))
+
+    for f in ds:
+        v = f.to_latlon()
+        assert isinstance(v, dict)
 
+        # lon
+        assert isinstance(v["lon"], np.ndarray)
+        assert v["lon"].shape == (11, 19)
+        for x in v["lon"]:
+            assert np.allclose(x, np.arange(-27, 45 + 4, 4))
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_points_multi_non_shared_grid(mode):
-    f1 = load_file_or_numpy_fs("test.grib", mode)
-    f2 = load_file_or_numpy_fs("test4.grib", mode)
-    f = f1 + f2
+        # lat
+        assert isinstance(v["lat"], np.ndarray)
+        assert v["lat"].shape == (11, 19)
+        for i, y in enumerate(v["lat"]):
+            assert np.allclose(y, np.ones(19) * (73 - i * 4))
 
-    with pytest.raises(ValueError):
-        f.to_points()
+        ref = xr_ds[f.name].sel(latitude=57, longitude=-7).values
 
+        x = 5
+        y = 4
+        assert np.isclose(f.to_numpy()[y, x], ref)
+        assert np.isclose(v["lon"][y, x], -7)
+        assert np.isclose(v["lat"][y, x], 57)
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_bbox(mode):
-    ds = load_file_or_numpy_fs("test.grib", mode)
+
+def test_bbox():
+    ds = from_source("file", earthkit_examples_file("test.nc"))
     bb = ds.bounding_box()
     assert len(bb) == 2
     for b in bb:
         assert b.as_tuple() == (73, -27, 33, 45)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-@pytest.mark.parametrize("index", [0, None])
-def test_grib_projection_ll(mode, index):
-    f = load_file_or_numpy_fs("test.grib", mode)
-
-    if index is not None:
-        g = f[index]
-    else:
-        g = f
-    assert isinstance(
-        g.projection(), (projections.EquidistantCylindrical, projections.LongLat)
-    )
+def test_netcdf_proj_string_non_cf():
+    f = from_source("file", earthkit_examples_file("test.nc"))
+    with pytest.raises(AttributeError):
+        f[0].projection()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_projection_mercator(mode):
-    f = load_file_or_numpy_fs("mercator.grib", mode, folder="data")
+def test_netcdf_projection_laea():
+    f = from_source("url", earthkit_remote_test_data_file("examples", "efas.nc"))
     projection = f[0].projection()
-    assert isinstance(projection, projections.Mercator)
+    assert isinstance(projection, projections.LambertAzimuthalEqualArea)
     assert projection.parameters == {
-        "true_scale_latitude": 20,
-        "central_latitude": 0,
-        "central_longitude": 0,
-        "false_easting": 0,
-        "false_northing": 0,
+        "central_latitude": 52.0,
+        "central_longitude": 10.0,
+        "false_northing": 3210000.0,
+        "false_easting": 4321000.0,
+    }
+    assert projection.globe == {
+        "ellipse": "GRS80",
     }
-    assert projection.globe == dict()
+
+
+def test_netcdf_proj_string_laea():
+    f = from_source("url", earthkit_remote_test_data_file("examples", "efas.nc"))
+    r = f[0].projection()
+    assert (
+        r.to_proj_string()
+        == "+proj=laea +lat_0=52 +lon_0=10 +x_0=4321000 +y_0=3210000 +ellps=GRS80 +units=m +no_defs"
+    )
+
+
+def test_netcdf_to_points_laea():
+    ds = from_source("url", earthkit_remote_test_data_file("examples", "efas.nc"))
+
+    assert len(ds) == 3
+
+    pos = [(0, 0), (0, -1), (-1, 0), (-1, -1)]
+
+    # we must check multiple fields
+    for idx in range(2):
+        v = ds[idx].to_points()
+        assert isinstance(v, dict)
+
+        # lon
+        assert isinstance(v["x"], np.ndarray)
+        assert v["x"].shape == (950, 1000)
+
+        ref = np.array([2502500.0, 7497500.0, 2502500.0, 7497500.0])
+        for i, x in enumerate(pos):
+            assert np.isclose(v["x"][x], ref[i]), f"{i=}, {x=}"
+
+        # lat
+        assert isinstance(v["y"], np.ndarray)
+        assert v["y"].shape == (950, 1000)
+
+        ref = np.array([5497500.0, 5497500.0, 752500.0, 752500.0])
+        for i, x in enumerate(pos):
+            assert np.isclose(v["y"][x], ref[i]), f"{i=}, {x=}"
+
+
+def test_netcdf_to_latlon_laea():
+    ds = from_source("url", earthkit_remote_test_data_file("examples", "efas.nc"))
+
+    assert len(ds) == 3
+
+    pos = [(0, 0), (0, -1), (-1, 0), (-1, -1)]
+
+    # we must check multiple fields
+    for idx in range(2):
+        v = ds[idx].to_latlon()
+        assert isinstance(v, dict)
+
+        # lon
+        assert isinstance(v["lon"], np.ndarray)
+        assert v["lon"].shape == (950, 1000)
+
+        ref = np.array(
+            [
+                -35.034023999999995,
+                73.93767587613708,
+                -8.229274420493763,
+                41.13970495087975,
+            ]
+        )
+        for i, x in enumerate(pos):
+            assert np.isclose(v["lon"][x], ref[i]), f"{i=}, {x=}"
+
+        # lat
+        assert isinstance(v["lat"], np.ndarray)
+        assert v["lat"].shape == (950, 1000)
+
+        ref = np.array(
+            [
+                66.9821429989222,
+                58.24673887576243,
+                27.802844211251625,
+                23.942342882929605,
+            ]
+        )
+        for i, x in enumerate(pos):
+            assert np.isclose(v["lat"][x], ref[i]), f"{i=}, {x=}"
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
-    main()
+    # test_datetime()
+    main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_gridspec.py` & `earthkit_data-0.7.0/tests/grib/test_grib_gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_memory.py` & `earthkit_data-0.7.0/tests/grib/test_grib_memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_order_by.py` & `earthkit_data-0.7.0/tests/grib/test_grib_order_by.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 import datetime
 import os
 import sys
 
 import pytest
 
 from earthkit.data import from_source
+from earthkit.data.testing import ARRAY_BACKENDS
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
+from grib_fixtures import FL_TYPES, load_grib_data  # noqa: E402
 
 
 # @pytest.mark.skipif(("GITHUB_WORKFLOW" in os.environ) or True, reason="Not yet ready")
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_order_by_single_message(mode):
-    s = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_order_by_single_message(fl_type, array_backend):
+    s = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
 
     r = s.order_by("shortName")
     assert len(r) == 1
     assert r[0].metadata("shortName") == "2t"
 
     r = s.order_by(["shortName"])
     assert len(r) == 1
@@ -49,15 +51,16 @@
             return 0
         if a > b:
             return 1
         if a < b:
             return -1
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "params,expected_meta",
     [
         ("shortName", dict(shortName=["t", "t", "u", "u", "v", "v"])),
         (["shortName"], dict(shortName=["t", "t", "u", "u", "v", "v"])),
         (
             ["shortName", "level"],
@@ -96,28 +99,30 @@
                 shortName=["u", "u", "v", "v", "t", "t"],
                 level=[1000, 850, 1000, 850, 1000, 850],
             ),
         ),
     ],
 )
 def test_grib_order_by_single_file_(
-    mode,
+    fl_type,
+    array_backend,
     params,
     expected_meta,
 ):
-    f = load_file_or_numpy_fs("test6.grib", mode)
+    f = load_grib_data("test6.grib", fl_type, array_backend)
 
     g = f.order_by(params)
     assert len(g) == len(f)
 
     for k, v in expected_meta.items():
         assert g.metadata(k) == v
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "params,expected_meta",
     [
         (
             "shortName",
             dict(shortName=["t", "t", "t", "t", "u", "u", "v", "v", "z", "z"]),
         ),
@@ -138,46 +143,48 @@
         ),
         (
             dict(shortName="descending"),
             dict(shortName=["z", "z", "v", "v", "u", "u", "t", "t", "t", "t"]),
         ),
     ],
 )
-def test_grib_order_by_multi_file(mode, params, expected_meta):
-    f1 = load_file_or_numpy_fs("test4.grib", mode)
-    f2 = load_file_or_numpy_fs("test6.grib", mode)
+def test_grib_order_by_multi_file(fl_type, array_backend, params, expected_meta):
+    f1 = load_grib_data("test4.grib", fl_type, array_backend)
+    f2 = load_grib_data("test6.grib", fl_type, array_backend)
     f = from_source("multi", [f1, f2])
 
     g = f.order_by(params)
     assert len(g) == len(f)
 
     for k, v in expected_meta.items():
         assert g.metadata(k) == v
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_order_by_with_sel(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_order_by_with_sel(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     g = f.sel(level=500)
     assert len(g) == 3
     r = g.order_by("shortName")
     assert len(r) == len(g)
     assert r.metadata("shortName") == ["t", "u", "v"]
 
     g = f.sel(level=500)
     assert len(g) == 3
     r = g.order_by({"shortName": "descending"})
     assert len(r) == len(g)
     assert r.metadata("shortName") == ["v", "u", "t"]
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_order_by_valid_datetime(mode):
-    f = load_file_or_numpy_fs("t_time_series.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_order_by_valid_datetime(fl_type, array_backend):
+    f = load_grib_data("t_time_series.grib", fl_type, array_backend, folder="data")
 
     g = f.order_by(valid_datetime="descending")
     assert len(g) == 10
 
     ref = [
         datetime.datetime(2020, 12, 23, 12, 0),
         datetime.datetime(2020, 12, 23, 12, 0),
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_output.py` & `earthkit_data-0.7.0/tests/grib/test_grib_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,28 +16,44 @@
 
 import numpy as np
 import pytest
 
 import earthkit.data
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
-from earthkit.data.testing import earthkit_examples_file
+from earthkit.data.testing import ARRAY_BACKENDS, earthkit_examples_file
 
 EPSILON = 1e-4
 
 
-def test_grib_save_when_loaded_from_file():
-    fs = from_source("file", earthkit_examples_file("test6.grib"))
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_save_when_loaded_from_file(array_backend):
+    fs = from_source(
+        "file", earthkit_examples_file("test6.grib"), array_backend=array_backend
+    )
     assert len(fs) == 6
     with temp_file() as tmp:
         fs.save(tmp)
         fs_saved = from_source("file", tmp)
         assert len(fs) == len(fs_saved)
 
 
+@pytest.mark.parametrize(
+    "_kwargs,expected_value",
+    [({}, 16), ({"bits_per_value": 12}, 12), ({"bits_per_value": None}, 16)],
+)
+def test_grib_save_bits_per_value(_kwargs, expected_value):
+    ds = from_source("file", earthkit_examples_file("test.grib"))
+
+    with temp_file() as tmp:
+        ds.save(tmp, **_kwargs)
+        ds1 = from_source("file", tmp)
+        assert ds1.metadata("bitsPerValue") == [expected_value] * len(ds)
+
+
 @pytest.mark.skipif(
     sys.version_info < (3, 10),
     reason="ignore_cleanup_errors requires Python 3.10 or later",
 )
 def test_grib_output_latlon():
     data = np.random.random((181, 360))
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_slice.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_slice.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,181 +5,177 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import os
-import sys
-
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
-from earthkit.data.testing import earthkit_examples_file
-
-here = os.path.dirname(__file__)
-sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
+from earthkit.data.testing import earthkit_examples_file, load_nc_or_xr_source
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize(
     "index,expected_meta",
     [
         (0, ["t", 1000]),
-        (2, ["v", 1000]),
+        (2, ["t", 700]),
         (17, ["v", 300]),
         (-1, ["v", 300]),
-        (-5, ["u", 400]),
+        (-5, ["v", 850]),
     ],
 )
-def test_grib_single_index(mode, index, expected_meta):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
-    # f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
+def test_netcdf_single_index(mode, index, expected_meta):
+    f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
 
     r = f[index]
-    assert r.metadata(["shortName", "level"]) == expected_meta
+    assert r.metadata(["variable", "level"]) == expected_meta
     v = r.values
     assert v.shape == (84,)
     # eps = 0.001
     # assert np.isclose(v[1088], 304.5642, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_single_index_bad(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_netcdf_single_index_bad():
+    f = from_source("file", earthkit_examples_file("tuv_pl.nc"))
     with pytest.raises(IndexError):
         f[27]
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize(
     "indexes,expected_meta",
     [
-        (slice(0, 4), [["t", 1000], ["u", 1000], ["v", 1000], ["t", 850]]),
-        (slice(None, 4), [["t", 1000], ["u", 1000], ["v", 1000], ["t", 850]]),
-        (slice(2, 9, 2), [["v", 1000], ["u", 850], ["t", 700], ["v", 700]]),
-        (slice(8, 1, -2), [["v", 700], ["t", 700], ["u", 850], ["v", 1000]]),
-        (slice(14, 18), [["v", 400], ["t", 300], ["u", 300], ["v", 300]]),
-        (slice(14, None), [["v", 400], ["t", 300], ["u", 300], ["v", 300]]),
+        (slice(0, 4), [["t", 1000], ["t", 850], ["t", 700], ["t", 500]]),
+        (slice(None, 4), [["t", 1000], ["t", 850], ["t", 700], ["t", 500]]),
+        (slice(2, 9, 2), [["t", 700], ["t", 400], ["u", 1000], ["u", 700]]),
+        (slice(8, 1, -2), [["u", 700], ["u", 1000], ["t", 400], ["t", 700]]),
+        (slice(14, 18), [["v", 700], ["v", 500], ["v", 400], ["v", 300]]),
+        (slice(14, None), [["v", 700], ["v", 500], ["v", 400], ["v", 300]]),
     ],
 )
-def test_grib_slice_single_file(mode, indexes, expected_meta):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_netcdf_slice_single_file(mode, indexes, expected_meta):
+    f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
     r = f[indexes]
     assert len(r) == 4
-    assert r.metadata(["shortName", "level"]) == expected_meta
+    assert r.metadata(["variable", "level"]) == expected_meta
     v = r.values
     assert v.shape == (4, 84)
     # check the original fieldlist
     assert len(f) == 18
-    assert f.metadata("shortName") == ["t", "u", "v"] * 6
+    assert f.metadata("variable") == ["t"] * 6 + ["u"] * 6 + ["v"] * 6
 
 
+@pytest.mark.xfail
 @pytest.mark.parametrize(
     "indexes,expected_meta",
     [
         (slice(1, 4), [["msl", 0], ["t", 500], ["z", 500]]),
         (slice(1, 6, 2), [["msl", 0], ["z", 500], ["z", 850]]),
         (slice(5, 0, -2), [["z", 850], ["z", 500], ["msl", 0]]),
         (slice(3, 6), [["z", 500], ["t", 850], ["z", 850]]),
     ],
 )
-def test_grib_slice_multi_file(indexes, expected_meta):
+def test_netcdf_slice_multi_file(indexes, expected_meta):
     f = from_source(
         "file",
-        [earthkit_examples_file("test.grib"), earthkit_examples_file("test4.grib")],
+        [earthkit_examples_file("test.nc"), earthkit_examples_file("tuv_pl.nc")],
     )
     r = f[indexes]
     assert len(r) == 3
-    assert r.metadata(["shortName", "level"]) == expected_meta
+    assert r.metadata(["variable", "level"]) == expected_meta
     # v = r.values
     # assert v.shape == (3, 84)
     # check the original fieldlist
-    assert len(f) == 6
+    assert len(f) == 2 + 18
     assert f.metadata("shortName") == ["2t", "msl", "t", "z", "t", "z"]
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize(
     "indexes1,indexes2",
     [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
 )
-def test_grib_array_indexing(mode, indexes1, indexes2):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_netcdf_array_indexing(mode, indexes1, indexes2):
+    f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
 
     r = f[indexes1]
     assert len(r) == 4
-    assert r.metadata("shortName") == ["u", "u", "v", "t"]
+    assert r.metadata("variable") == ["t", "v", "t", "u"]
 
     r1 = r[indexes2]
     assert len(r1) == 2
-    assert r1.metadata("shortName") == ["u", "t"]
+    assert r1.metadata("variable") == ["v", "u"]
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize("indexes", [(np.array([1, 19, 5, 9])), ([1, 19, 5, 9])])
-def test_grib_array_indexing_bad(mode, indexes):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_netcdf_array_indexing_bad(mode, indexes):
+    f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
     with pytest.raises(IndexError):
         f[indexes]
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_fieldlist_iterator(mode):
-    g = load_file_or_numpy_fs("tuv_pl.grib", mode)
-    sn = g.metadata("shortName")
+@pytest.mark.parametrize("mode", ["nc", "xr"])
+def test_netcdf_fieldlist_iterator(mode):
+    g = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
+    sn = g.metadata("variable")
     assert len(sn) == 18
-    iter_sn = [f.metadata("shortName") for f in g]
+    iter_sn = [f.metadata("variable") for f in g]
     assert iter_sn == sn
     # repeated iteration
-    iter_sn = [f.metadata("shortName") for f in g]
+    iter_sn = [f.metadata("variable") for f in g]
     assert iter_sn == sn
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_fieldlist_iterator_with_zip(mode):
-    # test something different to the iterator - does not try to
+def test_netcdf_fieldlist_iterator_with_zip():
+    # this tests something different with the iterator - this does not try to
     # 'go off the edge' of the fieldlist, because the length is determined by
     # the list of levels
-    g = load_file_or_numpy_fs("tuv_pl.grib", mode)
+    g = from_source("file", earthkit_examples_file("tuv_pl.nc"))
     ref_levs = g.metadata("level")
     assert len(ref_levs) == 18
     levs1 = []
     levs2 = []
     for k, f in zip(g.metadata("level"), g):
         levs1.append(k)
         levs2.append(f.metadata("level"))
     assert levs1 == ref_levs
     assert levs2 == ref_levs
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_fieldlist_iterator_with_zip_multiple(mode):
+def test_netcdf_fieldlist_iterator_with_zip_multiple():
     # same as test_fieldlist_iterator_with_zip() but multiple times
-    g = load_file_or_numpy_fs("tuv_pl.grib", mode)
+    g = from_source("file", earthkit_examples_file("tuv_pl.nc"))
     ref_levs = g.metadata("level")
     assert len(ref_levs) == 18
     for i in range(2):
         levs1 = []
         levs2 = []
         for k, f in zip(g.metadata("level"), g):
             levs1.append(k)
             levs2.append(f.metadata("level"))
         assert levs1 == ref_levs, i
         assert levs2 == ref_levs, i
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_fieldlist_reverse_iterator(mode):
-    g = load_file_or_numpy_fs("tuv_pl.grib", mode)
-    sn = g.metadata("shortName")
+@pytest.mark.parametrize("mode", ["nc", "xr"])
+def test_netcdf_fieldlist_reverse_iterator(mode):
+    g = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
+    sn = g.metadata("variable")
     sn_reversed = list(reversed(sn))
     assert sn_reversed[0] == "v"
     assert sn_reversed[17] == "t"
     gr = reversed(g)
-    iter_sn = [f.metadata("shortName") for f in gr]
+    iter_sn = [f.metadata("variable") for f in gr]
     assert len(iter_sn) == len(sn_reversed)
     assert iter_sn == sn_reversed
-    assert iter_sn == ["v", "u", "t"] * 6
+    assert iter_sn == ["v"] * 6 + ["u"] * 6 + ["t"] * 6
+
+
+if __name__ == "__main__":
+    from earthkit.data.testing import main
+
+    main()
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_stream.py` & `earthkit_data-0.7.0/tests/grib/test_grib_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,62 +10,65 @@
 #
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
-from earthkit.data.testing import earthkit_examples_file
+from earthkit.data.testing import ARRAY_BACKENDS, earthkit_examples_file
 
 
 def repeat_list_items(items, count):
     return sum([[x] * count for x in items], [])
 
 
 @pytest.mark.parametrize(
     "_kwargs,error",
     [
-        (dict(order_by="level"), TypeError),
+        # (dict(order_by="level"), TypeError),
         (dict(group_by=1), TypeError),
         (dict(group_by=["level", 1]), TypeError),
         # (dict(group_by="level", batch_size=1), TypeError),
         (dict(batch_size=-1), ValueError),
     ],
 )
 def test_grib_from_stream_invalid_args(_kwargs, error):
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         with pytest.raises(error):
             from_source("stream", stream, **_kwargs)
 
 
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "_kwargs",
     [
         {"group_by": "level"},
         {"group_by": "level", "batch_size": 0},
         {"group_by": "level", "batch_size": 1},
         {"group_by": ["level", "gridType"]},
     ],
 )
-def test_grib_from_stream_group_by(_kwargs):
+def test_grib_from_stream_group_by(array_backend, _kwargs):
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, **_kwargs)
+        fs = from_source("stream", stream, **_kwargs, array_backend=array_backend)
 
         # no methods are available
         with pytest.raises(TypeError):
             len(fs)
 
         ref = [
             [("t", 1000), ("u", 1000), ("v", 1000)],
             [("t", 850), ("u", 850), ("v", 850)],
         ]
         for i, f in enumerate(fs):
             assert len(f) == 3
             assert f.metadata(("param", "level")) == ref[i]
-            assert f.to_fieldlist("numpy") is not f
+            afl = f.to_fieldlist(array_backend=array_backend)
+            assert afl is not f
+            assert len(afl) == 3
 
         # stream consumed, no data is available
         assert sum([1 for _ in fs]) == 0
 
 
 @pytest.mark.parametrize(
     "convert_kwargs,expected_shape",
@@ -91,20 +94,20 @@
             [("t", 850), ("u", 850), ("v", 850)],
         ]
 
         if convert_kwargs is None:
             convert_kwargs = {}
 
         for i, f in enumerate(ds):
-            df = f.to_fieldlist("numpy", **convert_kwargs)
+            df = f.to_fieldlist(array_backend="numpy", **convert_kwargs)
             assert len(df) == 3
             assert df.metadata(("param", "level")) == ref[i]
             assert df._array.shape == expected_shape
             assert df.to_numpy(**convert_kwargs).shape == expected_shape
-            assert df.to_fieldlist("numpy", **convert_kwargs) is df
+            assert df.to_fieldlist(array_backend="numpy", **convert_kwargs) is df
 
         # stream consumed, no data is available
         assert sum([1 for _ in ds]) == 0
 
 
 @pytest.mark.parametrize(
     "_kwargs",
@@ -186,19 +189,19 @@
             [("u", 850), ("v", 850)],
         ]
 
         if convert_kwargs is None:
             convert_kwargs = {}
 
         for i, f in enumerate(ds):
-            df = f.to_fieldlist("numpy", **convert_kwargs)
+            df = f.to_fieldlist(array_backend="numpy", **convert_kwargs)
             assert df.metadata(("param", "level")) == ref[i], i
             assert df._array.shape == expected_shape, i
             assert df.to_numpy(**convert_kwargs).shape == expected_shape, i
-            assert df.to_fieldlist("numpy", **convert_kwargs) is df, i
+            assert df.to_fieldlist(array_backend="numpy", **convert_kwargs) is df, i
 
         # stream consumed, no data is available
         assert sum([1 for _ in ds]) == 0
 
 
 def test_grib_from_stream_in_memory():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
@@ -282,15 +285,15 @@
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         ds_s = from_source(
             "stream",
             stream,
             batch_size=0,
         )
 
-        ds = ds_s.to_fieldlist("numpy", **convert_kwargs)
+        ds = ds_s.to_fieldlist(array_backend="numpy", **convert_kwargs)
 
         assert len(ds) == 6
 
         ref = ["t", "u", "v", "t", "u", "v"]
         val = []
 
         # iteration
@@ -322,15 +325,15 @@
         if len(expected_shape) == 3:
             vals = ds.to_numpy(**convert_kwargs)[:, 0, 0]
         else:
             vals = ds.to_numpy(**convert_kwargs)[:, 0]
 
         assert np.allclose(vals, ref)
         assert ds._array.shape == expected_shape
-        assert ds.to_fieldlist("numpy", **convert_kwargs) is ds
+        assert ds.to_fieldlist(array_backend="numpy", **convert_kwargs) is ds
 
 
 def test_grib_save_when_loaded_from_stream():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         fs = from_source("stream", stream, batch_size=0)
         assert len(fs) == 6
         with temp_file() as tmp:
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_summary.py` & `earthkit_data-0.7.0/tests/grib/test_grib_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 # nor does it submit to any jurisdiction.
 
 import os
 import sys
 
 import pytest
 
+from earthkit.data.testing import ARRAY_BACKENDS
+
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
+from grib_fixtures import FL_TYPES, load_grib_data  # noqa: E402
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_describe(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_describe(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # full contents
     df = f.describe()
     df = df.data
 
     ref = {
         "level": {
@@ -139,17 +142,18 @@
     assert ref[0] == df[0].to_dict()
 
     df = f.describe(param=130)
     df = df.data
     assert ref[0] == df[0].to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # default keys
     f1 = f[0:4]
     df = f1.ls()
 
     ref = {
         "centre": {0: "ecmf", 1: "ecmf", 2: "ecmf", 3: "ecmf"},
@@ -193,17 +197,18 @@
         "gridType": {0: "regular_ll", 1: "regular_ll"},
         "paramId": {0: 130, 1: 131},
     }
 
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls_keys(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls_keys(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # default keys
     # positive num (=head)
     df = f.ls(n=2, keys=["shortName", "bottomLevel", "gridType"])
     ref = {
         "shortName": {0: "t", 1: "u"},
         "bottomLevel": {0: 1000, 1: 1000},
@@ -219,17 +224,18 @@
         "bottomLevel": {0: 300, 1: 300},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls_namespace(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls_namespace(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     df = f.ls(n=2, namespace="vertical")
     ref = {
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
     }
     assert ref == df.to_dict()
@@ -240,35 +246,38 @@
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
         "shortName": {0: "t", 1: "u"},
     }
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls_invalid_num(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls_invalid_num(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     with pytest.raises(ValueError):
         f.ls(n=0)
 
     with pytest.raises(ValueError):
         f.ls(0)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls_invalid_arg(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls_invalid_arg(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
     with pytest.raises(TypeError):
         f.ls(invalid=1)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_ls_num(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_ls_num(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # default keys
 
     # positive num (=head)
     df = f.ls(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
@@ -305,17 +314,18 @@
 
     assert ref == df.to_dict()
 
     df = f.ls(-2)
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_head_num(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_head_num(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # default keys
     df = f.head(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "t", 1: "u"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
@@ -330,17 +340,18 @@
 
     assert ref == df.to_dict()
 
     df = f.head(2)
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_tail_num(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_tail_num(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     # default keys
     df = f.tail(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "u", 1: "v"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
@@ -355,17 +366,18 @@
 
     assert ref == df.to_dict()
 
     df = f.tail(2)
     assert ref == df.to_dict()
 
 
-@pytest.mark.parametrize("mode", ["file"])
-def test_grib_dump(mode):
-    f = load_file_or_numpy_fs("test6.grib", mode)
+@pytest.mark.parametrize("fl_type", ["file"])
+@pytest.mark.parametrize("array_backend", [None])
+def test_grib_dump(fl_type, array_backend):
+    f = load_grib_data("test6.grib", fl_type, array_backend)
 
     namespaces = (
         "default",
         "geography",
         "ls",
         "mars",
         "parameter",
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_url.py` & `earthkit_data-0.7.0/tests/indexing/test_indexing_isel.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,87 +5,91 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
+import os
+import sys
+
 import pytest
 
 from earthkit.data import from_source
-from earthkit.data.testing import earthkit_remote_test_data_file
 
-
-@pytest.mark.parametrize(
-    "parts,expected_meta",
-    [
-        ([(0, 150)], [("t", 1000)]),
-        ([(240, 150)], [("u", 1000)]),
-        ([(240, 480)], [("u", 1000), ("v", 1000)]),
-    ],
-)
-def test_grib_single_url_parts(parts, expected_meta):
-    ds = from_source(
-        "url", earthkit_remote_test_data_file("examples/test6.grib"), parts=parts
-    )
-
-    assert len(ds) == len(expected_meta)
-
-    cnt = 0
-    for i, f in enumerate(ds):
-        assert f.metadata(("param", "level")) == expected_meta[i], i
-        cnt += 1
-
-    assert cnt == len(expected_meta)
+here = os.path.dirname(__file__)
+sys.path.insert(0, here)
+from indexing_fixtures import get_tmp_fixture  # noqa
 
 
+@pytest.mark.cache
+@pytest.mark.parametrize("mode", ["file", "multi", "directory"])
 @pytest.mark.parametrize(
-    "parts1,parts2,expected_meta",
+    "params,expected_meta,metadata_keys",
     [
+        (dict(param=1, level=2), [["u", 500]], ["shortName", "level:l"]),
+        (dict(param=1, level=2), [[131, 500]], ["paramId", "level:l"]),
         (
-            [(240, 150)],
-            None,
-            [("u", 1000), ("2t", 0), ("msl", 0)],
+            dict(param=[0, 1], level=[2, 3]),
+            [
+                ["t", 500],
+                ["t", 700],
+                ["u", 500],
+                ["u", 700],
+            ],
+            ["shortName", "level:l"],
         ),
         (
-            None,
-            [(0, 526)],
+            dict(param=[0], level=[3, 2], type=0),
             [
-                ("t", 1000),
-                ("u", 1000),
-                ("v", 1000),
-                ("t", 850),
-                ("u", 850),
-                ("v", 850),
-                ("2t", 0),
+                ["t", 500, "an"],
+                ["t", 700, "an"],
             ],
+            ["shortName", "level:l", "marsType"],
         ),
         (
-            [(240, 150)],
-            [(0, 526)],
-            [("u", 1000), ("2t", 0)],
+            dict(level=-1),
+            [
+                ["t", 1000],
+                ["u", 1000],
+                ["v", 1000],
+            ],
+            ["shortName", "level:l"],
         ),
     ],
 )
-def test_grib_multi_url_parts(parts1, parts2, expected_meta):
-    ds = from_source(
-        "url",
-        [
-            [earthkit_remote_test_data_file("examples/test6.grib"), parts1],
-            [earthkit_remote_test_data_file("examples/test.grib"), parts2],
-        ],
-    )
-
-    assert len(ds) == len(expected_meta)
-
-    cnt = 0
-    for i, f in enumerate(ds):
-        assert f.metadata(("param", "level")) == expected_meta[i], i
-        cnt += 1
+def test_indexing_isel_grib_file(mode, params, expected_meta, metadata_keys):
+    tmp, path = get_tmp_fixture(mode)
+    ds = from_source("file", path, indexing=True)
+    assert len(ds) == 18
+
+    g = ds.isel(**params)
+    assert len(g) == len(expected_meta)
+
+    # we sort the result to make the contents checking simpler
+    g = g.order_by(["param", "level"])
+
+    if len(expected_meta) > 0:
+        keys = list(params.keys())
+        if metadata_keys:
+            keys = metadata_keys
+
+        assert g.metadata(keys) == expected_meta
+
+
+@pytest.mark.cache
+def test_indexing_isel_grib_file_invalid_key():
+    tmp, path = get_tmp_fixture("file")
+    ds = from_source("file", path, indexing=True)
+    assert len(ds) == 18
+
+    r = ds.isel(INVALIDKEY=0)
+    assert len(r) == 0
 
-    assert cnt == len(expected_meta)
+    with pytest.raises(IndexError):
+        ds.isel(level=500)
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
-    main()
+    main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_url_stream.py` & `earthkit_data-0.7.0/tests/grib/test_grib_url_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def repeat_list_items(items, count):
     return sum([[x] * count for x in items], [])
 
 
 @pytest.mark.parametrize(
     "_kwargs,error",
     [
-        (dict(order_by="level"), TypeError),
+        # (dict(order_by="level"), TypeError),
         (dict(group_by=1), TypeError),
         (dict(group_by=["level", 1]), TypeError),
         # (dict(group_by="level", batch_size=1), TypeError),
         (dict(batch_size=-1), ValueError),
     ],
 )
 def test_grib_url_stream_invalid_args(_kwargs, error):
@@ -66,15 +66,15 @@
         [("t", 1000), ("u", 1000), ("v", 1000)],
         [("t", 850), ("u", 850), ("v", 850)],
     ]
     cnt = 0
     for i, f in enumerate(fs):
         assert len(f) == 3
         assert f.metadata(("param", "level")) == ref[i]
-        assert f.to_fieldlist("numpy") is not f
+        assert f.to_fieldlist(array_backend="numpy") is not f
         cnt += 1
 
     assert cnt == len(ref)
 
     # stream consumed, no data is available
     assert sum([1 for _ in fs]) == 0
 
@@ -405,15 +405,15 @@
         ([(0, 150)], [("t", 1000)]),
         (
             None,
             [("t", 1000), ("u", 1000), ("v", 1000), ("t", 850), ("u", 850), ("v", 850)],
         ),
     ],
 )
-def test_grib_single_url_stream_parts_as_arg(parts, expected_meta):
+def test_grib_single_url_stream_parts_as_arg_valid(parts, expected_meta):
     ds = from_source(
         "url",
         [earthkit_remote_test_data_file("examples/test6.grib"), parts],
         stream=True,
     )
 
     # no fieldlist methods are available
```

### Comparing `earthkit-data-0.6.0/tests/grib/test_grib_values.py` & `earthkit_data-0.7.0/tests/grib/test_grib_values.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,62 +11,72 @@
 
 import os
 import sys
 
 import numpy as np
 import pytest
 
+from earthkit.data.testing import (
+    ARRAY_BACKENDS,
+    check_array_type,
+    get_array,
+    get_array_namespace,
+)
+
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from grib_fixtures import load_file_or_numpy_fs  # noqa: E402
+from grib_fixtures import FL_TYPES, load_grib_data  # noqa: E402
 
 
 def check_array(v, shape=None, first=None, last=None, meanv=None, eps=1e-3):
     assert v.shape == shape
     assert np.isclose(v[0], first, eps)
     assert np.isclose(v[-1], last, eps)
     assert np.isclose(v.mean(), meanv, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_values_1(mode):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_values_1(fl_type, array_backend):
+    f = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
     eps = 1e-5
 
     # whole file
     v = f.values
-    assert isinstance(v, np.ndarray)
-    assert v.dtype == np.float64
+    check_array_type(v, array_backend, dtype="float64")
     assert v.shape == (1, 84)
     v = v[0].flatten()
     check_array(
         v,
         (84,),
         first=260.43560791015625,
         last=227.18560791015625,
         meanv=274.36566743396577,
         eps=eps,
     )
 
     # field
     v1 = f[0].values
-    assert isinstance(v1, np.ndarray)
+
+    check_array_type(v1, array_backend)
     assert v1.shape == (84,)
     assert np.allclose(v, v1, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_values_18(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+# @pytest.mark.parametrize("fl_type", FL_TYPES)
+# @pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+@pytest.mark.parametrize("fl_type", ["file"])
+@pytest.mark.parametrize("array_backend", ["numpy"])
+def test_grib_values_18(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
     eps = 1e-5
 
     # whole file
     v = f.values
-    assert isinstance(v, np.ndarray)
-    assert v.dtype == np.float64
+    check_array_type(v, array_backend, dtype="float64")
     assert v.shape == (18, 84)
     vf = v[0].flatten()
     check_array(
         vf,
         (84,),
         first=272.5642,
         last=240.56417846679688,
@@ -81,17 +91,18 @@
         first=226.6531524658203,
         last=206.6531524658203,
         meanv=227.84362865629652,
         eps=eps,
     )
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_numpy_1(mode):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_to_numpy_1(fl_type, array_backend):
+    f = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
 
     eps = 1e-5
     v = f.to_numpy()
     assert isinstance(v, np.ndarray)
     assert v.dtype == np.float64
     v = v[0].flatten()
     check_array(
@@ -100,44 +111,46 @@
         first=260.43560791015625,
         last=227.18560791015625,
         meanv=274.36566743396577,
         eps=eps,
     )
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "first,options, expected_shape",
     [
         (False, {}, (1, 7, 12)),
         (False, {"flatten": True}, (1, 84)),
         (False, {"flatten": False}, (1, 7, 12)),
         (True, {}, (7, 12)),
         (True, {"flatten": True}, (84,)),
         (True, {"flatten": False}, (7, 12)),
     ],
 )
-def test_grib_to_numpy_1_shape(mode, first, options, expected_shape):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+def test_grib_to_numpy_1_shape(fl_type, array_backend, first, options, expected_shape):
+    f = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
 
     v_ref = f[0].to_numpy().flatten()
     eps = 1e-5
 
     data = f[0] if first else f
     v1 = data.to_numpy(**options)
     assert isinstance(v1, np.ndarray)
     assert v1.dtype == np.float64
     assert v1.shape == expected_shape
     v1 = v1.flatten()
     assert np.allclose(v_ref, v1, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_to_numpy_18(mode):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_to_numpy_18(fl_type, array_backend):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     eps = 1e-5
 
     # whole file
     v = f.to_numpy(flatten=True)
     assert isinstance(v, np.ndarray)
     assert v.dtype == np.float64
@@ -159,15 +172,16 @@
         first=226.6531524658203,
         last=206.6531524658203,
         meanv=227.84362865629652,
         eps=eps,
     )
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "options, expected_shape",
     [
         (
             {},
             (
                 18,
@@ -181,16 +195,16 @@
                 18,
                 84,
             ),
         ),
         ({"flatten": False}, (18, 7, 12)),
     ],
 )
-def test_grib_to_numpy_18_shape(mode, options, expected_shape):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_grib_to_numpy_18_shape(fl_type, array_backend, options, expected_shape):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     eps = 1e-5
 
     # whole file
     v = f.to_numpy()
     assert isinstance(v, np.ndarray)
     assert v.dtype == np.float64
@@ -206,53 +220,56 @@
     assert v1.shape == expected_shape
     vr = v1[0].flatten()
     assert np.allclose(vf0, vr, eps)
     vr = v1[15].flatten()
     assert np.allclose(vf15, vr, eps)
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
 @pytest.mark.parametrize("dtype", [np.float32, np.float64])
-def test_grib_to_numpy_1_dtype(mode, dtype):
-    f = load_file_or_numpy_fs("test_single.grib", mode, folder="data")
+def test_grib_to_numpy_1_dtype(fl_type, array_backend, dtype):
+    f = load_grib_data("test_single.grib", fl_type, array_backend, folder="data")
 
     v = f[0].to_numpy(dtype=dtype)
     assert v.dtype == dtype
 
     v = f.to_numpy(dtype=dtype)
     assert v.dtype == dtype
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
 @pytest.mark.parametrize("dtype", [np.float32, np.float64])
-def test_grib_to_numpy_18_dtype(mode, dtype):
-    f = load_file_or_numpy_fs("tuv_pl.grib", mode)
+def test_grib_to_numpy_18_dtype(fl_type, array_backend, dtype):
+    f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     v = f[0].to_numpy(dtype=dtype)
     assert v.dtype == dtype
 
     v = f.to_numpy(dtype=dtype)
     assert v.dtype == dtype
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
 @pytest.mark.parametrize(
     "kwarg,expected_shape,expected_dtype",
     [
         ({}, (11, 19), np.float64),
         ({"flatten": True}, (209,), np.float64),
         ({"flatten": True, "dtype": np.float32}, (209,), np.float32),
         ({"flatten": True, "dtype": np.float64}, (209,), np.float64),
         ({"flatten": False}, (11, 19), np.float64),
         ({"flatten": False, "dtype": np.float32}, (11, 19), np.float32),
         ({"flatten": False, "dtype": np.float64}, (11, 19), np.float64),
     ],
 )
-def test_grib_field_data(mode, kwarg, expected_shape, expected_dtype):
-    ds = load_file_or_numpy_fs("test.grib", mode)
+def test_grib_field_data(fl_type, array_backend, kwarg, expected_shape, expected_dtype):
+    ds = load_grib_data("test.grib", fl_type, array_backend)
 
     latlon = ds[0].to_latlon(**kwarg)
     v = ds[0].to_numpy(**kwarg)
 
     d = ds[0].data(**kwarg)
     assert isinstance(d, np.ndarray)
     assert d.dtype == expected_dtype
@@ -281,29 +298,32 @@
     assert isinstance(d, np.ndarray)
     assert d.dtype == expected_dtype
     assert len(d) == 2
     assert np.allclose(d[0], v)
     assert np.allclose(d[1], latlon["lon"])
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ["numpy"])
 @pytest.mark.parametrize(
     "kwarg,expected_shape,expected_dtype",
     [
         ({}, (11, 19), np.float64),
         ({"flatten": True}, (209,), np.float64),
         ({"flatten": True, "dtype": np.float32}, (209,), np.float32),
         ({"flatten": True, "dtype": np.float64}, (209,), np.float64),
         ({"flatten": False}, (11, 19), np.float64),
         ({"flatten": False, "dtype": np.float32}, (11, 19), np.float32),
         ({"flatten": False, "dtype": np.float64}, (11, 19), np.float64),
     ],
 )
-def test_grib_fieldlist_data(mode, kwarg, expected_shape, expected_dtype):
-    ds = load_file_or_numpy_fs("test.grib", mode)
+def test_grib_fieldlist_data(
+    fl_type, array_backend, kwarg, expected_shape, expected_dtype
+):
+    ds = load_grib_data("test.grib", fl_type, array_backend)
 
     latlon = ds.to_latlon(**kwarg)
     v = ds.to_numpy(**kwarg)
 
     d = ds.data(**kwarg)
     assert isinstance(d, np.ndarray)
     assert d.shape == tuple([4, *expected_shape])
@@ -333,29 +353,35 @@
     assert d.shape == tuple([3, *expected_shape])
     assert d.dtype == expected_dtype
     assert np.allclose(d[0], v[0])
     assert np.allclose(d[1], v[1])
     assert np.allclose(d[2], latlon["lon"])
 
 
-@pytest.mark.parametrize("mode", ["file", "numpy_fs"])
-def test_grib_values_with_missing(mode):
-    f = load_file_or_numpy_fs("test_single_with_missing.grib", mode, folder="data")
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_values_with_missing(fl_type, array_backend):
+    f = load_grib_data(
+        "test_single_with_missing.grib", fl_type, array_backend, folder="data"
+    )
 
     v = f[0].values
-    assert isinstance(v, np.ndarray)
+    check_array_type(v, array_backend)
     assert v.shape == (84,)
     eps = 0.001
-    assert np.count_nonzero(np.isnan(v)) == 38
-    mask = np.array([12, 14, 15, 24, 25, 26] + list(range(28, 60)))
+
+    ns = get_array_namespace(array_backend)
+
+    assert ns.count_nonzero(ns.isnan(v)) == 38
+    mask = get_array([12, 14, 15, 24, 25, 26] + list(range(28, 60)), array_backend)
     assert np.isclose(v[0], 260.4356, eps)
     assert np.isclose(v[11], 260.4356, eps)
     assert np.isclose(v[-1], 227.1856, eps)
     m = v[mask]
     assert len(m) == 38
-    assert np.count_nonzero(np.isnan(m)) == 38
+    assert ns.count_nonzero(ns.isnan(m)) == 38
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit-data-0.6.0/tests/indexing/indexing_fixtures.py` & `earthkit_data-0.7.0/tests/indexing/indexing_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/indexing/test_indexing_db.py` & `earthkit_data-0.7.0/tests/indexing/test_indexing_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/indexing/test_indexing_order_by.py` & `earthkit_data-0.7.0/tests/indexing/test_indexing_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/indexing/test_indexing_serialisation.py` & `earthkit_data-0.7.0/tests/indexing/test_indexing_serialisation.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/indexing/test_order_kwargs.py` & `earthkit_data-0.7.0/tests/indexing/test_order_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/indexing/test_selection_kwargs.py` & `earthkit_data-0.7.0/tests/indexing/test_selection_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_fieldlist.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_fieldlist.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,22 +22,25 @@
             [[11, 12, 13], [21, 22, 23], [31, 32, 33]],
             [[14, 15, 16], [24, 25, 26], [34, 35, 36]],
         ],
         coords={"level": ["500", "700"], "x": [1, 2, 3], "y": [4, 5, 6]},
         name="dummyvar",
     )
 
+    # sanity check
+    assert np.allclose(a.sel(level="500", x=2).values, np.array([21, 22, 23]))
+
     ds = earthkit.data.from_object(a)
 
     assert ds
     assert len(ds) == 2
     assert ds.metadata("level") == ["500", "700"]
 
-    x_ref = np.array([[1, 2, 3], [1, 2, 3], [1, 2, 3]])
-    y_ref = np.array([[4, 4, 4], [5, 5, 5], [6, 6, 6]])
+    x_ref = np.array([[1, 1, 1], [2, 2, 2], [3, 3, 3]])
+    y_ref = np.array([[4, 5, 6], [4, 5, 6], [4, 5, 6]])
     assert np.allclose(ds[0].to_points()["x"], x_ref)
     assert np.allclose(ds[0].to_points()["y"], y_ref)
 
 
 def test_netcdf_fieldlist_bounds():
     """Check if having non string values in bounds does not cause a crash"""
     import xarray as xr
```

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_metadata.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,20 @@
 
 
 @pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize(
     "key,expected_value",
     [
         ("variable", "t"),
-        # ("variable:s", "t"),
-        # ("variable:str", "t"),
-        # ("centre", "ecmf"),
-        # ("centre:l", 98),
         ("level", 1000),
-        # ("level:l", 1000),
-        # ("level:int", 1000),
         (["variable"], ["t"]),
         (["variable", "level"], ["t", 1000]),
         (("variable"), "t"),
         (("variable", "level"), ("t", 1000)),
+        (("param", "levelist"), ("t", 1000)),
     ],
 )
 def test_netcdf_metadata_single_field(mode, key, expected_value):
     f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
 
     # sn = f.metadata(key)
     # assert sn == [expected_value]
```

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_output.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,33 +16,46 @@
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
 from earthkit.data.testing import earthkit_examples_file
 
 
 def test_netcdf_fieldlist_save():
     ds = from_source("file", earthkit_examples_file("test.nc"))
-    assert len(ds) == 2
 
-    tmp = temp_file()
-    ds.save(tmp.path)
-    assert os.path.exists(tmp.path)
-    r_tmp = from_source("file", tmp.path)
-    assert len(r_tmp) == 2
+    # the file must be saved without loading the fields
+    assert ds._reader._fields is None
+
+    with temp_file() as tmp:
+        ds.save(tmp)
+        assert ds._reader._fields is None
+        assert os.path.exists(tmp)
+        r_tmp = from_source("file", tmp)
+        assert len(r_tmp) == 2
 
 
-def test_netcdf_fieldlist_subset_save():
+def test_netcdf_fieldlist_subset_save_1():
     ds = from_source("file", earthkit_examples_file("test.nc"))
     assert len(ds) == 2
     r = ds[1]
 
     tmp = temp_file()
     with pytest.raises(NotImplementedError):
         r.save(tmp.path)
 
 
+def test_netcdf_fieldlist_subset_save_2():
+    ds = from_source("file", earthkit_examples_file("tuv_pl.nc"))
+    assert len(ds) == 18
+    r = ds[1:4]
+
+    tmp = temp_file()
+    with pytest.raises(NotImplementedError):
+        r.save(tmp.path)
+
+
 def test_netcdf_fieldlist_multi_subset_save():
     ds1 = from_source("file", earthkit_examples_file("test.nc"))
     ds2 = from_source("file", earthkit_examples_file("tuv_pl.nc"))
 
     ds = ds1 + ds2
     assert len(ds) == 20
```

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_sel.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_sel.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,21 +33,34 @@
         ),
         (dict(variable="w"), [], []),
         (dict(INVALIDKEY="w"), [], []),
         (
             dict(
                 variable=["t"],
                 level=[500, 700],
-                time=datetime.datetime(2018, 8, 1, 12, 0),
+                valid_datetime=datetime.datetime(2018, 8, 1, 12, 0),
             ),
             [
                 ["t", 700, datetime.datetime(2018, 8, 1, 12, 0)],
                 ["t", 500, datetime.datetime(2018, 8, 1, 12, 0)],
             ],
-            ["variable", "level", "time"],
+            ["variable", "level", "valid_datetime"],
+        ),
+        (
+            dict(
+                variable=["t"],
+                level=[500, 700],
+                date=20180801,
+                time=1200,
+            ),
+            [
+                ["t", 700, 20180801, 1200],
+                ["t", 500, 20180801, 1200],
+            ],
+            ["variable", "level", "date", "time"],
         ),
     ],
 )
 def test_netcdf_sel_single_file_1(mode, params, expected_meta, metadata_keys):
     f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
 
     g = f.sel(**params)
```

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_summary.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # default keys
     f1 = f[:4]
     df = f1.ls()
 
     ref = {
         "variable": {0: "t", 1: "t", 2: "t", 3: "t"},
         "level": {0: 1000, 1: 850, 2: 700, 3: 500},
-        "time": {
+        "valid_datetime": {
             0: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
             1: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
             2: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
             3: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
         },
         "units": {0: "K", 1: "K", 2: "K", 3: "K"},
     }
@@ -40,15 +40,15 @@
     # extra keys
     f1 = f[:2]
     df = f1.ls(extra_keys=["long_name"])
 
     ref = {
         "variable": {0: "t", 1: "t"},
         "level": {0: 1000, 1: 850},
-        "time": {
+        "valid_datetime": {
             0: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
             1: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
         },
         "units": {0: "K", 1: "K"},
         "long_name": {0: "Temperature", 1: "Temperature"},
     }
     assert ref == df.to_dict()
```

### Comparing `earthkit-data-0.6.0/tests/netcdf/test_netcdf_values.py` & `earthkit_data-0.7.0/tests/netcdf/test_netcdf_values.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_aliases.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_aliases_grib.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_aliases_grib.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_availability.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_availability.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_bbox.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_bbox.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_date.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_date.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_enum.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_enum.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_errors.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_errors.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_kwargs.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_normalize_parameter.py` & `earthkit_data-0.7.0/tests/normalize/test_normalize_parameter.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/normalize/test_transformers.py` & `earthkit_data-0.7.0/tests/normalize/test_transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs.py` & `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 from earthkit.data import from_source
 from earthkit.data.core.fieldlist import FieldList
 from earthkit.data.core.temporary import temp_file
 from earthkit.data.testing import earthkit_examples_file
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from numpy_fs_fixtures import (  # noqa: E402
-    check_numpy_fs,
-    check_numpy_fs_from_to_fieldlist,
+from array_fl_fixtures import (  # noqa: E402
+    check_array_fl,
+    check_array_fl_from_to_fieldlist,
 )
 
 
-def test_numpy_fs_grib_single_field():
+def test_array_fl_grib_single_field():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     assert ds[0].metadata("shortName") == "2t"
 
     lat, lon, v = ds[0].data(flatten=True)
     v1 = v + 1
 
@@ -56,15 +56,15 @@
     tmp = temp_file()
     r.save(tmp.path)
     assert os.path.exists(tmp.path)
     r_tmp = from_source("file", tmp.path)
     _check_field(r_tmp)
 
 
-def test_numpy_fs_grib_multi_field():
+def test_array_fl_grib_multi_field():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     assert ds[0].metadata("shortName") == "2t"
 
     v = ds.values
     v1 = v + 1
 
@@ -87,27 +87,27 @@
     assert np.allclose(v1, r_tmp.values)
     for i, f in enumerate(r_tmp):
         assert f.shape == ds[i].shape
         assert f.metadata("shortName") == "2d", f"shortName {i}"
         assert f.metadata("name") == "2 metre dewpoint temperature", f"name {i}"
 
 
-def test_numpy_fs_grib_from_list_of_arrays():
+def test_array_fl_grib_from_list_of_arrays():
     ds = from_source("file", earthkit_examples_file("test.grib"))
     md_full = ds.metadata("param")
     assert len(ds) == 2
 
     v = [ds[0].values, ds[1].values]
     md = [f.metadata().override(generatingProcessIdentifier=150) for f in ds]
     r = FieldList.from_numpy(v, md)
 
-    check_numpy_fs(r, [ds], md_full)
+    check_array_fl(r, [ds], md_full)
 
 
-def test_numpy_fs_grib_from_list_of_arrays_bad():
+def test_array_fl_grib_from_list_of_arrays_bad():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     v = ds[0].values
     md = [f.metadata().override(generatingProcessIdentifier=150) for f in ds]
 
     with pytest.raises(ValueError):
         _ = FieldList.from_numpy(v, md)
@@ -122,35 +122,35 @@
         {},
         {"dtype": np.float32},
         {"flatten": False},
         {"flatten": True},
         {"flatten": True, "dtype": np.float32},
     ],
 )
-def test_numpy_fs_grib_from_to_fieldlist(kwargs):
+def test_array_fl_grib_from_to_fieldlist(kwargs):
     ds = from_source("file", earthkit_examples_file("test.grib"))
     md_full = ds.metadata("param")
     assert len(ds) == 2
 
-    r = ds.to_fieldlist("numpy", **kwargs)
-    check_numpy_fs_from_to_fieldlist(r, [ds], md_full, **kwargs)
+    r = ds.to_fieldlist(array_backend="numpy", **kwargs)
+    check_array_fl_from_to_fieldlist(r, [ds], md_full, **kwargs)
 
 
-def test_numpy_fs_grib_from_to_fieldlist_repeat():
+def test_array_fl_grib_from_to_fieldlist_repeat():
     ds = from_source("file", earthkit_examples_file("test.grib"))
     md_full = ds.metadata("param")
     assert len(ds) == 2
 
     kwargs = {}
-    r = ds.to_fieldlist("numpy", **kwargs)
-    check_numpy_fs_from_to_fieldlist(r, [ds], md_full, **kwargs)
+    r = ds.to_fieldlist(array_backend="numpy", **kwargs)
+    check_array_fl_from_to_fieldlist(r, [ds], md_full, **kwargs)
 
     kwargs = {"flatten": True, "dtype": np.float32}
-    r1 = r.to_fieldlist("numpy", **kwargs)
+    r1 = r.to_fieldlist(array_backend="numpy", **kwargs)
     assert r1 is not r
-    check_numpy_fs_from_to_fieldlist(r1, [ds], md_full, **kwargs)
+    check_array_fl_from_to_fieldlist(r1, [ds], md_full, **kwargs)
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_concat.py` & `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_concat.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,116 +15,116 @@
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.fieldlist import FieldList
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from numpy_fs_fixtures import (  # noqa: E402
-    check_numpy_fs,
+from array_fl_fixtures import (  # noqa: E402
+    check_array_fl,
     check_save_to_disk,
-    load_numpy_fs,
+    load_array_fl,
 )
 
 
 @pytest.mark.parametrize("mode", ["oper", "multi"])
-def test_numpy_fs_grib_concat_2a(mode):
-    ds1, ds2, md = load_numpy_fs(2)
+def test_array_fl_grib_concat_2a(mode):
+    ds1, ds2, md = load_array_fl(2)
 
     if mode == "oper":
         ds = ds1 + ds2
     else:
         ds = from_source("multi", ds1, ds2)
 
-    check_numpy_fs(ds, [ds1, ds2], md)
+    check_array_fl(ds, [ds1, ds2], md)
     check_save_to_disk(ds, 8, md)
 
 
-def test_numpy_fs_grib_concat_2b():
-    ds1, ds2, md = load_numpy_fs(2)
+def test_array_fl_grib_concat_2b():
+    ds1, ds2, md = load_array_fl(2)
     ds1_ori = ds1
     ds1 += ds2
 
-    check_numpy_fs(ds1, [ds1_ori, ds2], md)
+    check_array_fl(ds1, [ds1_ori, ds2], md)
     check_save_to_disk(ds1, 8, md)
 
 
 @pytest.mark.parametrize("mode", ["oper", "multi"])
-def test_numpy_fs_grib_concat_3a(mode):
-    ds1, ds2, ds3, md = load_numpy_fs(3)
+def test_array_fl_grib_concat_3a(mode):
+    ds1, ds2, ds3, md = load_array_fl(3)
 
     if mode == "oper":
         ds = ds1 + ds2
         ds = ds + ds3
     else:
         ds = from_source("multi", ds1, ds2)
         ds = from_source("multi", ds, ds3)
 
-    check_numpy_fs(ds, [ds1, ds2, ds3], md)
+    check_array_fl(ds, [ds1, ds2, ds3], md)
     check_save_to_disk(ds, 26, md)
 
 
 @pytest.mark.parametrize("mode", ["oper", "multi"])
-def test_numpy_fs_grib_concat_3b(mode):
-    ds1, ds2, ds3, md = load_numpy_fs(3)
+def test_array_fl_grib_concat_3b(mode):
+    ds1, ds2, ds3, md = load_array_fl(3)
 
     if mode == "oper":
         ds = ds1 + ds2 + ds3
     else:
         ds = from_source("multi", ds1, ds2, ds3)
 
-    check_numpy_fs(ds, [ds1, ds2, ds3], md)
+    check_array_fl(ds, [ds1, ds2, ds3], md)
     check_save_to_disk(ds, 26, md)
 
 
-def test_numpy_fs_grib_from_empty_1():
+def test_array_fl_grib_from_empty_1():
     ds_e = FieldList()
-    ds, md = load_numpy_fs(1)
+    ds, md = load_array_fl(1)
     ds1 = ds_e + ds
     assert id(ds1) == id(ds)
     assert len(ds1) == 2
     assert ds1.metadata("param") == md
     check_save_to_disk(ds1, 2, md)
 
 
-def test_numpy_fs_grib_from_empty_2():
+def test_array_fl_grib_from_empty_2():
     ds_e = FieldList()
-    ds, md = load_numpy_fs(1)
+    ds, md = load_array_fl(1)
     ds1 = ds + ds_e
     assert id(ds1) == id(ds)
     assert len(ds1) == 2
     assert ds1.metadata("param") == md
     check_save_to_disk(ds1, 2, md)
 
 
-def test_numpy_fs_grib_from_empty_3():
+def test_array_fl_grib_from_empty_3():
     ds_e = FieldList()
-    ds1, ds2, md = load_numpy_fs(2)
+    ds1, ds2, md = load_array_fl(2)
     ds = ds_e + ds1 + ds2
 
-    check_numpy_fs(ds, [ds1, ds2], md)
+    check_array_fl(ds, [ds1, ds2], md)
     check_save_to_disk(ds, 8, md)
 
 
-def test_numpy_fs_grib_from_empty_4():
+def test_array_fl_grib_from_empty_4():
     ds = FieldList()
-    ds1, md = load_numpy_fs(1)
+    ds1, md = load_array_fl(1)
     ds += ds1
     assert id(ds) == id(ds1)
     assert len(ds) == 2
     assert ds.metadata("param") == md
     check_save_to_disk(ds, 2, md)
 
 
-def test_numpy_fs_grib_from_empty_5():
+def test_array_fl_grib_from_empty_5():
     ds = FieldList()
-    ds1, ds2, md = load_numpy_fs(2)
+    ds1, ds2, md = load_array_fl(2)
     ds += ds1 + ds2
 
-    check_numpy_fs(ds, [ds1, ds2], md)
+    check_array_fl(ds, [ds1, ds2], md)
     check_save_to_disk(ds, 8, md)
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_metadata.py` & `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 import os
 import sys
 
 import pytest
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from numpy_fs_fixtures import load_numpy_fs, load_numpy_fs_file  # noqa: E402
+from array_fl_fixtures import load_array_fl, load_array_fl_file  # noqa: E402
 
 # Note: Almost all grib metadata tests are also run for numpyfs.
 # See grib/test_grib_metadata.py
 
 
-def test_numpy_fs_values_metadata():
-    ds, _ = load_numpy_fs(1)
+def test_array_fl_values_metadata():
+    ds, _ = load_array_fl(1)
 
     # values metadata
     keys = [
         "min",
         "max",
         "avg",
         "ds",
@@ -40,29 +40,32 @@
         "values",
     ]
     for k in keys:
         assert ds[0].metadata(k, default=None) is None, k
         with pytest.raises(KeyError):
             ds[0].metadata(k)
 
+    # bits per value must be kept from the original GRIB data
+    assert ds[0].metadata("bitsPerValue") == 16
 
-def test_numpy_fs_values_metadata_internal():
-    ds, _ = load_numpy_fs(1)
+
+def test_array_fl_values_metadata_internal():
+    ds, _ = load_array_fl(1)
 
     keys = {
         "shortName": "2t",
         "grib.shortName": "2t",
     }
 
     for k, v in keys.items():
         assert ds[0].metadata(k) == v, k
 
 
-def test_numpy_fs_metadata_keys():
-    ds, _ = load_numpy_fs(1)
+def test_array_fl_metadata_keys():
+    ds, _ = load_array_fl(1)
 
     # The number/order of metadata keys can vary with the ecCodes version.
     # The same is true for the namespaces.
 
     md = ds[0].metadata()
     md_num = len(md)
     assert md_num > 100
@@ -86,16 +89,16 @@
 
     assert "max" not in md
     assert "maximum" not in md
     assert "statistics.max" not in md
     assert "validityDate" in md
 
 
-def test_numpy_fs_metadata_namespace():
-    f, _ = load_numpy_fs_file("tuv_pl.grib")
+def test_array_fl_metadata_namespace():
+    f, _ = load_array_fl_file("tuv_pl.grib")
 
     r = f[0].metadata(namespace="vertical")
     ref = {"level": 1000, "typeOfLevel": "isobaricInhPa"}
     assert r == ref
 
     r = f[0].metadata(namespace=["vertical", "time"])
     ref = {
```

### Comparing `earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_summary.py` & `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 #
 
 import os
 import sys
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from numpy_fs_fixtures import load_numpy_fs_file  # noqa: E402
+from array_fl_fixtures import load_array_fl_file  # noqa: E402
 
 # Note: Almost all grib metadata tests are also run for numpyfs.
 # See grib/test_grib_summary.py
 
 
-def test_numpy_fs_dump():
-    f, _ = load_numpy_fs_file("test6.grib")
+def test_array_fl_dump():
+    f, _ = load_array_fl_file("test6.grib")
 
     namespaces = (
         "default",
         "geography",
         "ls",
         "mars",
         "parameter",
```

### Comparing `earthkit-data-0.6.0/tests/numpy_fs/test_numpy_fs_write.py` & `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fl_write.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,54 +15,87 @@
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.fieldlist import FieldList
 from earthkit.data.core.temporary import temp_file
-from earthkit.data.testing import earthkit_examples_file
+from earthkit.data.testing import (
+    ARRAY_BACKENDS,
+    check_array_type,
+    earthkit_examples_file,
+    get_array_namespace,
+)
 
 here = os.path.dirname(__file__)
 sys.path.insert(0, here)
-from numpy_fs_fixtures import load_numpy_fs  # noqa: E402
+from array_fl_fixtures import load_array_fl  # noqa: E402
 
 LOG = logging.getLogger(__name__)
 
 
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_array_fl_grib_write(array_backend):
+    ds = from_source(
+        "file", earthkit_examples_file("test.grib"), array_backend=array_backend
+    )
+    ns = get_array_namespace(array_backend)
+
+    assert ds[0].metadata("shortName") == "2t"
+    assert len(ds) == 2
+    v1 = ds[0].values + 1
+    check_array_type(v1, array_backend)
+
+    md = ds[0].metadata()
+    md1 = md.override(shortName="msl")
+    r = FieldList.from_array(v1, md1)
+
+    with temp_file() as tmp:
+        r.save(tmp)
+        assert os.path.exists(tmp)
+        r_tmp = from_source("file", tmp, array_backend=array_backend)
+        v_tmp = r_tmp[0].values
+        assert ns.allclose(v1, v_tmp)
+
+
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize("_kwargs", [{}, {"check_nans": True}])
-def test_numpy_fs_grib_write_missing(_kwargs):
-    ds = from_source("file", earthkit_examples_file("test.grib"))
+def test_array_fl_grib_write_missing(array_backend, _kwargs):
+    ds = from_source(
+        "file", earthkit_examples_file("test.grib"), array_backend=array_backend
+    )
+    ns = get_array_namespace(array_backend)
 
     assert ds[0].metadata("shortName") == "2t"
 
     v = ds[0].values
     v1 = v + 1
-    assert not np.isnan(v1[0])
-    assert not np.isnan(v1[1])
-    v1[0] = np.nan
-    assert np.isnan(v1[0])
-    assert not np.isnan(v1[1])
+    assert not ns.isnan(v1[0])
+    assert not ns.isnan(v1[1])
+    v1[0] = ns.nan
+    assert ns.isnan(v1[0])
+    assert not ns.isnan(v1[1])
 
     md = ds[0].metadata()
     md1 = md.override(shortName="msl")
-    r = FieldList.from_numpy(v1, md1)
+    r = FieldList.from_array(v1, md1)
 
-    assert np.isnan(r[0].values[0])
-    assert not np.isnan(r[0].values[1])
+    assert ns.isnan(r[0].values[0])
+    assert not ns.isnan(r[0].values[1])
 
     with temp_file() as tmp:
         r.save(tmp, **_kwargs)
         assert os.path.exists(tmp)
-        r_tmp = from_source("file", tmp)
+        r_tmp = from_source("file", tmp, array_backend=array_backend)
         v_tmp = r_tmp[0].values
-        assert np.isnan(v_tmp[0])
-        assert not np.isnan(v_tmp[1])
+        assert ns.isnan(v_tmp[0])
+        assert not ns.isnan(v_tmp[1])
 
 
-def test_numpy_fs_grib_write_check_nans_bad():
+def test_array_fl_grib_write_check_nans_bad():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     assert ds[0].metadata("shortName") == "2t"
 
     v = ds[0].values
     v1 = v + 1
     assert not np.isnan(v1[0])
@@ -81,15 +114,15 @@
     with temp_file() as tmp:
         from eccodes import EncodingError
 
         with pytest.raises(EncodingError):
             r.save(tmp, check_nans=False)
 
 
-def test_numpy_fs_grib_write_append():
+def test_array_fl_grib_write_append():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     assert ds[0].metadata("shortName") == "2t"
 
     v = ds[0].values
     v1 = v + 1
     v2 = v + 2
@@ -114,15 +147,15 @@
     r2.save(tmp.path, append=True)
     assert os.path.exists(tmp.path)
     r_tmp = from_source("file", tmp.path)
     assert len(r_tmp) == 2
     assert r_tmp.metadata("shortName") == ["msl", "2d"]
 
 
-def test_numpy_fs_grib_write_generating_proc_id():
+def test_array_fl_grib_write_generating_proc_id():
     ds = from_source("file", earthkit_examples_file("test.grib"))
 
     assert ds[0].metadata("shortName") == "2t"
 
     v = ds[0].values
     v1 = v + 1
     v2 = v + 2
@@ -145,19 +178,24 @@
             150,
         ]
 
         assert np.allclose(r_tmp.values[0], v1)
         assert np.allclose(r_tmp.values[1], v2)
 
 
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
-    "_kwargs,expected_value", [({}, 16), ({"bits_per_value": 12}, 12)]
+    "_kwargs,expected_value",
+    [({}, None), ({"bits_per_value": 12}, 12), ({"bits_per_value": None}, None)],
 )
-def test_numpy_fs_grib_write_bits_per_value(_kwargs, expected_value):
-    ds, _ = load_numpy_fs(1)
+def test_array_fl_grib_write_bits_per_value(array_backend, _kwargs, expected_value):
+    ds, _ = load_array_fl(1, array_backend)
+
+    if expected_value is None:
+        expected_value = ds[0].metadata("bitsPerValue")
 
     with temp_file() as tmp:
         ds.save(tmp, **_kwargs)
         ds1 = from_source("file", tmp)
         assert ds1.metadata("bitsPerValue") == [expected_value] * len(ds)
```

### Comparing `earthkit-data-0.6.0/tests/plugins/test_sources_plugin.py` & `earthkit_data-0.7.0/tests/plugins/test_sources_plugin.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_covjson_reader.py` & `earthkit_data-0.7.0/tests/readers/test_covjson_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_csv_reader.py` & `earthkit_data-0.7.0/tests/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_geojson_reader.py` & `earthkit_data-0.7.0/tests/readers/test_geojson_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_grib_reader.py` & `earthkit_data-0.7.0/tests/readers/test_grib_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_netcdf_reader.py` & `earthkit_data-0.7.0/tests/readers/test_netcdf_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 import os
 import tempfile
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
-from earthkit.data.readers.netcdf import NetCDFField
+from earthkit.data.core.temporary import temp_file
+from earthkit.data.readers.netcdf.field import NetCDFField
 from earthkit.data.testing import (
     NO_CDS,
     earthkit_examples_file,
     earthkit_file,
-    earthkit_remote_test_data_file,
     earthkit_test_data_file,
 )
 
 
 def check_array(v, shape=None, first=None, last=None, meanv=None, eps=1e-3):
     assert v.shape == shape
     assert np.isclose(v[0], first, eps)
@@ -221,43 +221,63 @@
     with tempfile.TemporaryDirectory() as tmp_dir:
         fpath = os.path.join(tmp_dir, "tmp.nc")
         ds.to_netcdf(fpath)
         fs = from_source("file", earthkit_test_data_file(fpath))
         assert len(fs) == 2
 
 
+# @pytest.mark.no_eccodes
+# def test_netcdf_non_fieldlist_0():
+#     ek_ch4_l2 = from_source(
+#         "url",
+#         earthkit_remote_test_data_file(
+#             "test-data/20210101-C3S-L2_GHG-GHG_PRODUCTS-TANSO2-GOSAT2-SRFP-DAILY-v2.0.0.nc"
+#         ),
+#         # Data from this CDS request:
+#         # "cds",
+#         # "satellite-methane",
+#         # {
+#         #     "processing_level": "level_2",
+#         #     "sensor_and_algorithm": "tanso2_fts2_srfp",
+#         #     "year": "2021",
+#         #     "month": "01",
+#         #     "day": "01",
+#         #     "version": "2.0.0",
+#         # },
+#     )
+#     # TODO: add more conditions to this test when it is clear what methods it should have
+#     ek_ch4_l2.to_xarray()
+
+
 @pytest.mark.no_eccodes
 def test_netcdf_non_fieldlist():
-    ek_ch4_l2 = from_source(
-        "url",
-        earthkit_remote_test_data_file(
-            "test-data/20210101-C3S-L2_GHG-GHG_PRODUCTS-TANSO2-GOSAT2-SRFP-DAILY-v2.0.0.nc"
-        )
-        # Data from this CDS request:
-        # "cds",
-        # "satellite-methane",
-        # {
-        #     "processing_level": "level_2",
-        #     "sensor_and_algorithm": "tanso2_fts2_srfp",
-        #     "year": "2021",
-        #     "month": "01",
-        #     "day": "01",
-        #     "version": "2.0.0",
-        # },
-    )
-    # TODO: add more conditions to this test when it is clear what methods it should have
-    ek_ch4_l2.to_xarray()
+    ds = from_source("file", earthkit_test_data_file("hovexp_vert_area.nc"))
+    with pytest.raises(TypeError):
+        len(ds)
+
+    import xarray as xr
+
+    ref = xr.open_dataset(earthkit_test_data_file("hovexp_vert_area.nc"))
+    res = ds.to_xarray()
+
+    assert ref.identical(res)
+    assert ds.to_numpy().shape == (1, 6, 5)
+
+    with temp_file() as tmp:
+        ds.save(tmp)
+        assert os.path.exists(tmp)
+        ds_saved = from_source("file", tmp)
+        assert ds_saved.to_xarray().identical(res)
 
 
 @pytest.mark.no_eccodes
 def test_netcdf_lazy_fieldlist_scan():
     ds = from_source("file", earthkit_examples_file("test.nc"))
-    assert ds._fields is None
+    assert ds._reader._fields is None
     assert len(ds) == 2
-    assert len(ds._fields) == 2
+    assert len(ds._reader._fields) == 2
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
-    # test_datetime()
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/readers/test_odb_reader.py` & `earthkit_data-0.7.0/tests/readers/test_odb_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_reader_padding_bytes.py` & `earthkit_data-0.7.0/tests/readers/test_reader_padding_bytes.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_tar_reader.py` & `earthkit_data-0.7.0/tests/readers/test_tar_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_unknown_reader.py` & `earthkit_data-0.7.0/tests/readers/test_unknown_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/readers/test_zip_reader.py` & `earthkit_data-0.7.0/tests/readers/test_zip_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_ads.py` & `earthkit_data-0.7.0/tests/sources/test_ads.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 NO_ADS = not os.path.exists(os.path.expanduser("~/.adsapirc"))
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_ADS, reason="No access to ADS")
-def test_ads_grib_1():
+@pytest.mark.parametrize("prompt", [True, False])
+def test_ads_grib_1_prompt(prompt):
     s = from_source(
         "ads",
         "cams-global-reanalysis-eac4",
         variable=["particulate_matter_10um", "particulate_matter_1um"],
         area=[50, -50, 20, 50],
         date="2012-12-12",
+        prompt=prompt,
         time="12:00",
     )
     assert len(s) == 2
 
 
 @pytest.mark.long_test
 @pytest.mark.download
```

### Comparing `earthkit-data-0.6.0/tests/sources/test_cds.py` & `earthkit_data-0.7.0/tests/sources/test_cds.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,23 +5,49 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
+import os
+
 import pytest
 
 from earthkit.data import from_source
+from earthkit.data.core.temporary import temp_directory
 from earthkit.data.testing import NO_CDS
 
+CDS_TIMEOUT = pytest.CDS_TIMEOUT
+
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.parametrize("prompt", [True, False])
+@pytest.mark.timeout(CDS_TIMEOUT)
+def test_cds_grib_prompt(prompt):
+    s = from_source(
+        "cds",
+        "reanalysis-era5-single-levels",
+        variable=["2t", "msl"],
+        product_type="reanalysis",
+        area=[50, -50, 20, 50],
+        date="2012-12-12",
+        prompt=prompt,
+        time="12:00",
+    )
+    assert len(s) == 2
+    assert s.metadata("param") == ["2t", "msl"]
+
+
+@pytest.mark.long_test
+@pytest.mark.download
+@pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_kwargs():
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
         variable=["2t", "msl"],
         product_type="reanalysis",
         area=[50, -50, 20, 50],
@@ -31,14 +57,15 @@
     assert len(s) == 2
     assert s.metadata("param") == ["2t", "msl"]
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_dict():
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
         dict(
             variable=["2t", "msl"],
             product_type="reanalysis",
@@ -50,14 +77,15 @@
     assert len(s) == 2
     assert s.metadata("param") == ["2t", "msl"]
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_invalid_args_kwargs():
     with pytest.raises(TypeError):
         from_source(
             "cds",
             "reanalysis-era5-single-levels",
             dict(
                 variable=["2t", "msl"],
@@ -68,14 +96,15 @@
             time="12:00",
         )
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_split_on_var():
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
         variable=["2t", "msl"],
         product_type="reanalysis",
         area=[50, -50, 20, 50],
@@ -101,14 +130,15 @@
             [20140512, 20140512, 20140513, 20140513, 20140514, 20140514],
         ),
     ],
 )
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_multi_var_date(date, expected_date):
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
         variable=["2t", "msl"],
         product_type="reanalysis",
         area=[50, -50, 20, 50],
@@ -119,14 +149,52 @@
     assert s.metadata("param") == ["2t", "msl"] * 3
     assert s.metadata("date") == expected_date
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
+def test_cds_grib_save():
+    s = from_source(
+        "cds",
+        "reanalysis-era5-single-levels",
+        variable=["2t", "msl"],
+        product_type="reanalysis",
+        area=[50, -50, 20, 50],
+        date="2012-12-12",
+        time="12:00",
+    )
+    with temp_directory() as tmpdir:
+        # Check file save to assigned filename
+        s.save(os.path.join(tmpdir, "test.grib"))
+        assert os.path.isfile(os.path.join(tmpdir, "test.grib"))
+
+    s = from_source(
+        "cds",
+        "reanalysis-era5-single-levels",
+        variable=["2t", "msl"],
+        product_type="reanalysis",
+        area=[50, -50, 20, 50],
+        date="2012-12-12",
+        time="12:00",
+    )
+    with temp_directory() as tmpdir:
+        # Check file can be saved in current dir with detected filename:
+        here = os.curdir
+        os.chdir(tmpdir)
+        s.save()
+        assert os.path.isfile(os.path.basename(s.source_filename))
+        os.chdir(here)
+
+
+@pytest.mark.long_test
+@pytest.mark.download
+@pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 @pytest.mark.parametrize(
     "split_on,expected_file_num,expected_param,expected_time",
     (
         [None, 1, ["2t", "msl", "2t", "msl"], [0, 0, 1200, 1200]],
         [[], 1, ["2t", "msl", "2t", "msl"], [0, 0, 1200, 1200]],
         [{}, 1, ["2t", "msl", "2t", "msl"], [0, 0, 1200, 1200]],
         ["variable", 2, ["2t", "2t", "msl", "msl"], [0, 1200] * 2],
@@ -161,14 +229,15 @@
     assert s.metadata("param") == expected_param
     assert s.metadata("time") == expected_time
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 @pytest.mark.parametrize(
     "split_on1,split_on2,expected_file_num,expected_param,expected_time",
     (
         [None, None, 2, ["2t", "2t", "msl", "msl"], [0, 1200, 0, 1200]],
         [None, "time", 3, ["2t", "2t", "msl", "msl"], [0, 1200, 0, 1200]],
         ["time", "time", 4, ["2t", "2t", "msl", "msl"], [0, 1200, 0, 1200]],
     ),
@@ -181,26 +250,27 @@
         area=[50, -50, 20, 50],
         date="2012-12-12",
         time=["00:00", "12:00"],
     )
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
-        base_request | {"variable": "2t", "split_on": split_on1},
-        base_request | {"variable": "msl", "split_on": split_on2},
+        {**base_request, **{"variable": "2t", "split_on": split_on1}},
+        {**base_request, **{"variable": "msl", "split_on": split_on2}},
     )
     assert len(s._indexes) == expected_file_num
     assert len(s) == 4
     assert s.metadata("param") == expected_param
     assert s.metadata("time") == expected_time
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_netcdf():
     s = from_source(
         "cds",
         "reanalysis-era5-single-levels",
         variable=["2t", "msl"],
         product_type="reanalysis",
         area=[50, -50, 20, 50],
@@ -211,14 +281,40 @@
     assert len(s) == 2
     assert s.metadata("variable") == ["t2m", "msl"]
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
+def test_cds_netcdf_save():
+    s = from_source(
+        "cds",
+        "reanalysis-era5-single-levels",
+        variable=["2t", "msl"],
+        product_type="reanalysis",
+        area=[50, -50, 20, 50],
+        date="2012-12-12",
+        time="12:00",
+        format="netcdf",
+    )
+
+    with temp_directory() as tmpdir:
+        # Check file can be saved in current dir with detected filename:
+        here = os.curdir
+        os.chdir(tmpdir)
+        s.save()
+        assert os.path.isfile(os.path.basename(s.source_filename))
+        os.chdir(here)
+
+
+@pytest.mark.long_test
+@pytest.mark.download
+@pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(60)
 def test_cds_netcdf_selection_limited():
     s = from_source(
         "cds",
         "satellite-albedo",
         {
             "variable": "albb_bh",
             "satellite": "noaa_7",
@@ -243,14 +339,15 @@
         "QFLAG",
     ]
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_observation_csv_file_to_pandas_xarray():
     collection_id = "insitu-observations-gruan-reference-network"
     request = {
         "format": "csv-lev.zip",
         "year": "2006",
         "month": "05",
         "variable": ["air_temperature", "altitude"],
@@ -268,14 +365,15 @@
     assert len(df) == 11318
     assert list(df.columns)[:2] == ["station_name", "report_timestamp"]
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_non_observation_csv_file_to_pandas_xarray():
     collection_id = "sis-energy-derived-projections"
     request = {
         "format": "zip",
         "variable": "wind_power_generation_onshore",
         "spatial_aggregation": "country_level",
         "energy_product_type": "capacity_factor_ratio",
@@ -292,14 +390,15 @@
     assert data_cds.to_pandas().equals(data_file.to_pandas())
     assert data_cds.to_xarray().equals(data_file.to_xarray())
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_grib_to_pandas_xarray():
     collection_id = "reanalysis-era5-single-levels"
     request = dict(
         variable=["2t", "msl"],
         product_type="reanalysis",
         area=[50, -50, 20, 50],
         date="2012-12-12/to/2012-12-15",
@@ -320,14 +419,15 @@
     assert len(ds) == 2
     assert len(ds.data_vars) == 2
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
+@pytest.mark.timeout(CDS_TIMEOUT)
 def test_cds_netcdf_to_pandas_xarray():
     collection_id = "satellite-methane"
     request = {
         "format": "zip",
         "processing_level": "level_2",
         "variable": "xch4",
         "sensor_and_algorithm": "merged_emma",
```

### Comparing `earthkit-data-0.6.0/tests/sources/test_ecmwf_open_data.py` & `earthkit_data-0.7.0/tests/sources/test_wekeo.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,37 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import pytest
 
 from earthkit.data import from_source
-from earthkit.data.testing import NO_EOD
+from earthkit.data.testing import NO_HDA
 
 
 @pytest.mark.long_test
 @pytest.mark.download
-@pytest.mark.skipif(NO_EOD, reason="No access to EOD")
-def test_eod():
-    ds = from_source(
-        "ecmwf-open-data",
-        param=["2t", "msl"],
-        levtype="sfc",
+@pytest.mark.skipif(NO_HDA, reason="No access to WEKEO")
+@pytest.mark.parametrize("prompt", [True, False])
+def test_wekeo_download(prompt):
+    s = from_source(
+        "wekeo",
+        "EO:CLMS:DAT:CGLS_GLOBAL_NDVI300_V1_333M",
+        prompt=prompt,
+        request={
+            "datasetId": "EO:CLMS:DAT:CGLS_GLOBAL_NDVI300_V1_333M",
+            "dateRangeSelectValues": [
+                {
+                    "name": "dtrange",
+                    "start": "2014-01-01T00:00:00.000Z",
+                    "end": "2014-01-01T23:59:59.999Z",
+                }
+            ],
+        },
     )
-    assert len(ds) == 2
-    assert ds.path
+    assert len(s) == 1
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/sources/test_fdb.py` & `earthkit_data-0.7.0/tests/sources/test_fdb.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_list_of_dicts.py` & `earthkit_data-0.7.0/tests/sources/test_list_of_dicts.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_mars.py` & `earthkit_data-0.7.0/tests/sources/test_mars.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from earthkit.data import from_source
 from earthkit.data.testing import NO_MARS
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_MARS, reason="No access to MARS")
-def test_mars_grib_1():
+@pytest.mark.parametrize("prompt", [True, False])
+def test_mars_grib_1_prompt(prompt):
     s = from_source(
         "mars",
         param=["2t", "msl"],
         levtype="sfc",
         area=[50, -50, 20, 50],
         grid=[2, 2],
+        prompt=prompt,
         date="2023-05-10",
     )
     assert len(s) == 2
 
 
 @pytest.mark.long_test
 @pytest.mark.download
```

### Comparing `earthkit-data-0.6.0/tests/sources/test_multi.py` & `earthkit_data-0.7.0/tests/sources/test_multi.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_polytope.py` & `earthkit_data-0.7.0/tests/sources/test_polytope.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_url.py` & `earthkit_data-0.7.0/tests/sources/test_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,16 +192,18 @@
 
 def test_url_netcdf_source_save():
     ds = from_source(
         "url",
         earthkit_remote_test_data_file("examples/test.nc"),
     )
 
-    tmp = temp_file()
-    ds.save(tmp.path)
-    assert os.path.exists(tmp.path)
+    with temp_file() as tmp:
+        ds.save(tmp)
+        assert os.path.exists(tmp)
+        ds_saved = from_source("file", tmp)
+        assert len(ds_saved) == 2
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/sources/test_url_pattern.py` & `earthkit_data-0.7.0/tests/sources/test_url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/sources/test_wekeocds.py` & `earthkit_data-0.7.0/tests/sources/test_wekeocds.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 from earthkit.data import from_source
 from earthkit.data.testing import NO_HDA
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_HDA, reason="No access to WEKEO")
-def test_wekeo_grib_1():
+@pytest.mark.parametrize("prompt", [True, False])
+def test_wekeo_grib_1_prompt(prompt):
     s = from_source(
         "wekeocds",
         "EO:ECMWF:DAT:REANALYSIS_ERA5_SINGLE_LEVELS",
         variable=["2m_temperature", "mean_sea_level_pressure"],
         product_type=["reanalysis"],
         year=["2012"],
         month=["12"],
         day=["12"],
         time=["13:00"],
+        prompt=prompt,
         format="grib",
     )
     assert len(s) == 2
 
 
 @pytest.mark.long_test
 @pytest.mark.download
```

### Comparing `earthkit-data-0.6.0/tests/translators/test_translators.py` & `earthkit_data-0.7.0/tests/translators/test_translators.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from earthkit.data import from_source, transform, translators, wrappers
+from earthkit.data.testing import earthkit_test_data_file
 from earthkit.data.translators import ndarray as ndtranslator
 from earthkit.data.translators import pandas as pdtranslator
 from earthkit.data.translators import string as strtranslator
 from earthkit.data.translators import xarray as xrtranslator
 
 LOG = logging.getLogger(__name__)
 
@@ -129,15 +130,15 @@
     # Check that public API method transforms to correct type (back to original)
     transformed = transform(gpd.GeoDataFrame(), gpd.GeoDataFrame)
     assert isinstance(transformed, gpd.GeoDataFrame)
 
 
 def test_transform_from_grib_file():
     # transform grib-based data object
-    f = from_source("file", "tests/data/test_single.grib")
+    f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
     # np.ndarray
     transformed = transform(f, np.ndarray)
     assert isinstance(transformed, np.ndarray)
 
     # xr.DataArray
     transformed = transform(f, xr.DataArray)
```

### Comparing `earthkit-data-0.6.0/tests/utils/test_bbox.py` & `earthkit_data-0.7.0/tests/utils/test_bbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,11 +246,18 @@
 def test_bbox_union_with():
     b1 = BoundingBox(north=50, west=-20, south=-30, east=40)
     b2 = BoundingBox(north=60, west=-10, south=-40, east=55)
     b = b1.union_with(b2)
     assert b == BoundingBox(north=60, west=-20, south=-40, east=55)
 
 
+def test_bbox_make_invalid():
+    import numpy as np
+
+    b = BoundingBox.make_invalid()
+    assert b.as_tuple() == (np.nan, np.nan, np.nan, np.nan)
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main(__file__)
```

### Comparing `earthkit-data-0.6.0/tests/utils/test_dates.py` & `earthkit_data-0.7.0/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/utils/test_download_examples.py` & `earthkit_data-0.7.0/tests/utils/test_download_examples.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/utils/test_interval.py` & `earthkit_data-0.7.0/tests/utils/test_interval.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/utils/test_module_inputs_wrapper.py` & `earthkit_data-0.7.0/tests/utils/test_module_inputs_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from earthkit.data import from_object, from_source
 from earthkit.data.readers import Reader
+from earthkit.data.testing import earthkit_test_data_file
 from earthkit.data.utils import module_inputs_wrapper
 
 from . import dummy_module
 from .dummy_module import XR_TYPES
 
 TEST_NP = np.arange(10)
 TEST_NP2 = np.arange(10)
@@ -54,33 +55,33 @@
 WRAPPED_DUMMY_MODULE = module_inputs_wrapper.transform_module_inputs(
     dummy_module,
 )
 
 
 def test_transform_function_inputs_reader_to_xarray():
     # Check EK GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     ek_reader_result = WRAPPED_XR_ONES_LIKE(EK_GRIB_READER)
     # Will return a DataSet becuase that is first value in kwarg_types
     assert isinstance(ek_reader_result, xr.Dataset)
     assert ek_reader_result.equals(xr.ones_like(EK_GRIB_READER.to_xarray()))
 
 
 def test_transform_function_inputs_reader_to_xarray_typesetting():
     # Check EK GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     ek_reader_result = WRAPPED_XR_ONES_LIKE_TYPE_SETTING(EK_GRIB_READER)
     # Will return a dataarray because that is first value in type-set Union
     assert isinstance(ek_reader_result, xr.DataArray)
     assert ek_reader_result.equals(xr.ones_like(EK_GRIB_READER.to_xarray().t2m))
 
 
 def test_transform_module_inputs_reader_to_xarray():
     # Check EK GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     ek_reader_result = WRAPPED_DUMMY_MODULE.xarray_ones_like(EK_GRIB_READER)
     # Data array because type-setting of function has dataarray first
     assert isinstance(ek_reader_result, xr.DataArray)
     assert ek_reader_result.equals(xr.ones_like(EK_GRIB_READER.to_xarray()).t2m)
 
 
 def test_transform_function_inputs_wrapper_to_xarray():
@@ -104,30 +105,30 @@
     ek_wrapper_result = WRAPPED_DUMMY_MODULE.xarray_ones_like(EK_NUMPY_WRAPPER)
     assert isinstance(ek_wrapper_result, xr.DataArray)
     assert ek_wrapper_result.equals(xr.ones_like(TEST_DA))
 
 
 def test_transform_function_inputs_reader_to_numpy():
     # Test with Earthkit.data GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     assert WRAPPED_NP_MEAN(EK_GRIB_READER) == np.mean(EK_GRIB_READER.to_numpy())
     assert isinstance(WRAPPED_NP_MEAN(EK_GRIB_READER), np.float64)
 
 
 def test_transform_function_inputs_reader_to_numpy_typesetting():
     # Test with Earthkit.data GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     result = WRAPPED_NP_MEAN_TYPE_SETTING(EK_GRIB_READER)
     assert result == np.mean(EK_GRIB_READER.to_numpy())
     assert isinstance(result, np.float64)
 
 
 def test_transform_module_inputs_reader_to_numpy():
     # Test with Earthkit.data GribReader object
-    EK_GRIB_READER = from_source("file", "tests/data/test_single.grib")
+    EK_GRIB_READER = from_source("file", earthkit_test_data_file("test_single.grib"))
     result = WRAPPED_DUMMY_MODULE.numpy_mean(EK_GRIB_READER)
     assert result == np.mean(EK_GRIB_READER.to_numpy())
     assert isinstance(result, np.float64)
 
 
 def test_transform_function_inputs_wrapper_to_numpy():
     # Test with Earthkit.data XarrayWrapper object
```

### Comparing `earthkit-data-0.6.0/tests/utils/test_projections.py` & `earthkit_data-0.7.0/tests/utils/test_projections.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,24 @@
         "false_easting": 4321000.0,
     }
     assert projection.globe == {
         "ellipse": "GRS80",
     }
 
 
+def test_from_proj_string_lcc():
+    proj_string = "+proj=lcc +lon_0=-90 +lat_1=33 +lat_2=45"
+    projection = projections.Projection.from_proj_string(proj_string)
+    assert isinstance(projection, projections.LambertConformal)
+    assert projection.parameters == {
+        "central_longitude": -90.0,
+        "standard_parallels": (33.0, 45.0),
+    }
+
+
 def test_from_cf_grid_mapping_aea():
     grid_mapping = {
         "grid_mapping_name": "albers_conical_equal_area",
         "standard_parallel": 40,
         "longitude_of_central_meridian": 10,
     }
     projection = projections.Projection.from_cf_grid_mapping(**grid_mapping)
```

### Comparing `earthkit-data-0.6.0/tests/wrappers/test_ndarray.py` & `earthkit_data-0.7.0/tests/wrappers/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/wrappers/test_pandas.py` & `earthkit_data-0.7.0/tests/wrappers/test_pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/wrappers/test_string.py` & `earthkit_data-0.7.0/tests/wrappers/test_string.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.6.0/tests/wrappers/test_xarray.py` & `earthkit_data-0.7.0/tests/wrappers/test_xarray.py`

 * *Files identical despite different names*

