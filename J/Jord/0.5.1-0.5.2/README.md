# Comparing `tmp/jord-0.5.1.tar.gz` & `tmp/jord-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jord-0.5.1.tar", last modified: Tue Apr 16 07:37:18 2024, max compression
+gzip compressed data, was "jord-0.5.2.tar", last modified: Wed Apr 17 16:56:45 2024, max compression
```

## Comparing `jord-0.5.1.tar` & `jord-0.5.2.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.920349 jord-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-16 07:37:15.000000 jord-0.5.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 07:37:15.000000 jord-0.5.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 07:37:15.000000 jord-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 07:37:15.000000 jord-0.5.1/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-16 07:37:15.000000 jord-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 07:37:15.000000 jord-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-16 07:37:18.920349 jord-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-16 07:37:15.000000 jord-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-16 07:37:15.000000 jord-0.5.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 07:37:15.000000 jord-0.5.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 07:37:15.000000 jord-0.5.1/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-16 07:37:15.000000 jord-0.5.1/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-16 07:37:15.000000 jord-0.5.1/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-16 07:37:15.000000 jord-0.5.1/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 07:37:15.000000 jord-0.5.1/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3476 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/actions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1933 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23854 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 07:37:15.000000 jord-0.5.1/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27412 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9931 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-16 07:37:15.000000 jord-0.5.1/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-16 07:37:15.000000 jord-0.5.1/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 07:37:15.000000 jord-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 07:37:15.000000 jord-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 07:37:18.920349 jord-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-16 07:37:15.000000 jord-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 07:37:15.000000 jord-0.5.1/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-16 07:37:15.000000 jord-0.5.1/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-16 07:37:15.000000 jord-0.5.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.985396 jord-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.961396 jord-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-17 16:56:41.000000 jord-0.5.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 16:56:41.000000 jord-0.5.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 16:56:41.000000 jord-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:41.000000 jord-0.5.2/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-17 16:56:45.000000 jord-0.5.2/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-17 16:56:45.000000 jord-0.5.2/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:56:45.000000 jord-0.5.2/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-17 16:56:45.000000 jord-0.5.2/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 16:56:45.000000 jord-0.5.2/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 16:56:41.000000 jord-0.5.2/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-17 16:56:41.000000 jord-0.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 16:56:41.000000 jord-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-17 16:56:45.985396 jord-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-17 16:56:41.000000 jord-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-17 16:56:41.000000 jord-0.5.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.961396 jord-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 16:56:41.000000 jord-0.5.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.961396 jord-0.5.2/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 16:56:41.000000 jord-0.5.2/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-17 16:56:41.000000 jord-0.5.2/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.961396 jord-0.5.2/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:41.000000 jord-0.5.2/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-17 16:56:41.000000 jord-0.5.2/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.961396 jord-0.5.2/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-17 16:56:41.000000 jord-0.5.2/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-04-17 16:56:41.000000 jord-0.5.2/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-17 16:56:41.000000 jord-0.5.2/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 16:56:41.000000 jord-0.5.2/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.965396 jord-0.5.2/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 16:56:41.000000 jord-0.5.2/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-17 16:56:41.000000 jord-0.5.2/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-17 16:56:41.000000 jord-0.5.2/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-17 16:56:41.000000 jord-0.5.2/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.969396 jord-0.5.2/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.969396 jord-0.5.2/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.969396 jord-0.5.2/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.973396 jord-0.5.2/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/randomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.973396 jord-0.5.2/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.973396 jord-0.5.2/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.973396 jord-0.5.2/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.973396 jord-0.5.2/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-17 16:56:41.000000 jord-0.5.2/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 16:56:41.000000 jord-0.5.2/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-17 16:56:41.000000 jord-0.5.2/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27412 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-17 16:56:41.000000 jord-0.5.2/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-17 16:56:41.000000 jord-0.5.2/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-17 16:56:41.000000 jord-0.5.2/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:41.000000 jord-0.5.2/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 16:56:41.000000 jord-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 16:56:41.000000 jord-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 16:56:45.985396 jord-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-17 16:56:41.000000 jord-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:45.977396 jord-0.5.2/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 16:56:41.000000 jord-0.5.2/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-17 16:56:41.000000 jord-0.5.2/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-17 16:56:41.000000 jord-0.5.2/tests/test_sanity.py
```

### Comparing `jord-0.5.1/.github/CODE_OF_CONDUCT.md` & `jord-0.5.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/.github/CONTRIBUTING.md` & `jord-0.5.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/Jord.egg-info/PKG-INFO` & `jord-0.5.2/Jord.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.1
+Version: 0.5.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -22,99 +22,99 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: apppath>=1.0.2
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
-Requires-Dist: pyzmq
-Requires-Dist: sorcery
-Requires-Dist: sympy
-Requires-Dist: tqdm
+Requires-Dist: pyzmq>=1.1.1
+Requires-Dist: sorcery>=0.2.0
+Requires-Dist: sympy>=1.1.1
+Requires-Dist: tqdm>=1.1.1
 Requires-Dist: warg>=1.1.6
-Provides-Extra: dev
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: sympy; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: pyzmq; extra == "dev"
-Requires-Dist: sorcery; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: tqdm; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
+Provides-Extra: q
+Requires-Dist: PySide2; extra == "q"
+Provides-Extra: samples
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Provides-Extra: fiona
+Requires-Dist: fiona>=1.1.1; extra == "fiona"
+Provides-Extra: gdal
+Provides-Extra: tests
+Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest>=4.4.1; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: pyproj; extra == "shapely"
 Requires-Dist: shapely; extra == "shapely"
-Provides-Extra: q
-Requires-Dist: pyqt5-tools; extra == "q"
-Provides-Extra: setup
+Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
+Provides-Extra: dev
+Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: furo; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Provides-Extra: pil
+Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
-Provides-Extra: pil
-Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: fiona
-Requires-Dist: fiona; extra == "fiona"
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: samples
-Provides-Extra: gdal
-Provides-Extra: extra
+Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pyproj; extra == "all"
 Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: pyqt5-tools; extra == "all"
-Requires-Dist: fiona; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: networkx; extra == "all"
-Requires-Dist: sympy; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: pyzmq; extra == "all"
-Requires-Dist: sorcery; extra == "all"
-Requires-Dist: shapely; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: networkx; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: draugr>=1.0.9; extra == "all"
 Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: tqdm; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.1/Jord.egg-info/SOURCES.txt` & `jord-0.5.2/Jord.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 jord/qgis_utilities/helpers/actions.py
 jord/qgis_utilities/helpers/drawing.py
 jord/qgis_utilities/helpers/environment.py
 jord/qgis_utilities/helpers/groups.py
 jord/qgis_utilities/helpers/logging.py
 jord/qgis_utilities/helpers/models.py
 jord/qgis_utilities/helpers/progress_bar.py
+jord/qgis_utilities/helpers/randomize.py
 jord/qgis_utilities/helpers/sessions.py
 jord/qgis_utilities/helpers/signals.py
 jord/qgis_utilities/helpers/timestamp.py
 jord/qgis_utilities/numpy_utilities/README.md
 jord/qgis_utilities/numpy_utilities/__init__.py
 jord/qgis_utilities/numpy_utilities/conversion.py
 jord/qgis_utilities/numpy_utilities/data_type.py
```

### Comparing `jord-0.5.1/LICENSE.md` & `jord-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/PKG-INFO` & `jord-0.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.1
+Version: 0.5.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -22,99 +22,99 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: apppath>=1.0.2
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
-Requires-Dist: pyzmq
-Requires-Dist: sorcery
-Requires-Dist: sympy
-Requires-Dist: tqdm
+Requires-Dist: pyzmq>=1.1.1
+Requires-Dist: sorcery>=0.2.0
+Requires-Dist: sympy>=1.1.1
+Requires-Dist: tqdm>=1.1.1
 Requires-Dist: warg>=1.1.6
-Provides-Extra: dev
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: sympy; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: pyzmq; extra == "dev"
-Requires-Dist: sorcery; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: tqdm; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
+Provides-Extra: q
+Requires-Dist: PySide2; extra == "q"
+Provides-Extra: samples
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Provides-Extra: fiona
+Requires-Dist: fiona>=1.1.1; extra == "fiona"
+Provides-Extra: gdal
+Provides-Extra: tests
+Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest>=4.4.1; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: pyproj; extra == "shapely"
 Requires-Dist: shapely; extra == "shapely"
-Provides-Extra: q
-Requires-Dist: pyqt5-tools; extra == "q"
-Provides-Extra: setup
+Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
+Provides-Extra: dev
+Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: furo; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Provides-Extra: pil
+Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
-Provides-Extra: pil
-Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: fiona
-Requires-Dist: fiona; extra == "fiona"
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: samples
-Provides-Extra: gdal
-Provides-Extra: extra
+Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pyproj; extra == "all"
 Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: pyqt5-tools; extra == "all"
-Requires-Dist: fiona; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: networkx; extra == "all"
-Requires-Dist: sympy; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: pyzmq; extra == "all"
-Requires-Dist: sorcery; extra == "all"
-Requires-Dist: shapely; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: networkx; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: draugr>=1.0.9; extra == "all"
 Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: tqdm; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.1/README.md` & `jord-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/SECURITY.md` & `jord-0.5.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/__init__.py` & `jord-0.5.2/jord/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `jord-0.5.1/jord/fiona_utilities/deserialise.py` & `jord-0.5.2/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/__init__.py` & `jord-0.5.2/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/cloning.py` & `jord-0.5.2/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/context.py` & `jord-0.5.2/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/conversion.py` & `jord-0.5.2/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/error_handling.py` & `jord-0.5.2/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/importing.py` & `jord-0.5.2/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/gdal_utilities/persistence.py` & `jord-0.5.2/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geojson_utilities/geometry_types.py` & `jord-0.5.2/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geometric_analysis/center_line.py` & `jord-0.5.2/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geometric_analysis/intersections.py` & `jord-0.5.2/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.5.2/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.5.2/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.5.2/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/networkx_utilities/construction.py` & `jord-0.5.2/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/__init__.py` & `jord-0.5.2/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/categorisation.py` & `jord-0.5.2/jord/qgis_utilities/categorisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import random
 from itertools import cycle
 from typing import Callable, Generator, Iterable, Sized
 
-from PyQt5.Qt import QColor
+# noinspection PyUnresolvedReferences
+from qgis.PyQt.QtGui import QColor
 
 # noinspection PyUnresolvedReferences
 from qgis.core import (
     QgsCategorizedSymbolRenderer,
     QgsRendererCategory,
     QgsSymbol,
     QgsVectorLayer,
```

### Comparing `jord-0.5.1/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.5.2/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.5.2/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/data_provider.py` & `jord-0.5.2/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/enums.py` & `jord-0.5.2/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.5.2/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/geometry_types.py` & `jord-0.5.2/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/actions.py` & `jord-0.5.2/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/drawing.py` & `jord-0.5.2/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/environment.py` & `jord-0.5.2/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/logging.py` & `jord-0.5.2/jord/qgis_utilities/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/models.py` & `jord-0.5.2/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.5.2/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/sessions.py` & `jord-0.5.2/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/signals.py` & `jord-0.5.2/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.5.2/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/layer_creation.py` & `jord-0.5.2/jord/qgis_utilities/layer_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
         fields = None
 
     if categorise_by_attribute and fields:
         assert (
             categorise_by_attribute in fields
         ), f"{categorise_by_attribute} was not found in {fields}"
 
-    if not isinstance(qgis_instance_handle, QgsProject):
-        qgis_project = qgis_instance_handle.qgis_project
-    elif qgis_instance_handle is None:
+    if qgis_instance_handle is None:
         qgis_project = QgsProject.instance()
+    elif not isinstance(qgis_instance_handle, QgsProject):
+        qgis_project = qgis_instance_handle.qgis_project
     else:
         qgis_project = qgis_instance_handle
 
     if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
         for g in geom.asGeometryCollection():  # TODO: Look into recursion?
             uri = json.loads(g.asJson())["type"]
             if uri is None:
@@ -425,18 +425,18 @@
     if categorise_by_attribute:
         categorise_layer(layer, categorise_by_attribute)
 
     layer.commitChanges()
     layer.updateFields()
     layer.updateExtents()
 
-    if not isinstance(qgis_instance_handle, QgsProject):
-        qgis_project = qgis_instance_handle.qgis_project
-    elif qgis_instance_handle is None:
+    if qgis_instance_handle is None:
         qgis_project = QgsProject.instance()
+    elif not isinstance(qgis_instance_handle, QgsProject):
+        qgis_project = qgis_instance_handle.qgis_project
     else:
         qgis_project = qgis_instance_handle
 
     if group:
         qgis_project.addMapLayer(layer, False)
         group.insertLayer(0, layer)
     else:
```

### Comparing `jord-0.5.1/jord/qgis_utilities/layer_serialisation.py` & `jord-0.5.2/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.5.2/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.5.2/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.5.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/styles.py` & `jord-0.5.2/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qgis_utilities/styling.py` & `jord-0.5.2/jord/qgis_utilities/styling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import logging
 from typing import Mapping
 
-from PyQt5.Qt import QColor
+# noinspection PyUnresolvedReferences
+from qgis.PyQt.QtGui import QColor
 
 # noinspection PyUnresolvedReferences
 from qgis.core import (
     QgsCategorizedSymbolRenderer,
     QgsLineSymbol,
     QgsRendererCategory,
     QgsSymbol,
```

### Comparing `jord-0.5.1/jord/qlive_utilities/client.py` & `jord-0.5.2/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qlive_utilities/clients/auto.py` & `jord-0.5.2/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qlive_utilities/procedures.py` & `jord-0.5.2/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qlive_utilities/serialisation.py` & `jord-0.5.2/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qlive_utilities/uri_utilities.py` & `jord-0.5.2/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/qt_utilities/enums.py` & `jord-0.5.2/jord/qt_utilities/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "FocusReasonEnum",
     "ColorEnum",
     "WindowModalityEnum",
     "AlignmentFlag",
 ]
 
 try:
+
     from PyQt6.QtCore import Qt
 
     class AlignmentFlag(Flag):
         """
         Alignment
         """
```

### Comparing `jord-0.5.1/jord/shapely_utilities/__init__.py` & `jord-0.5.2/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/base.py` & `jord-0.5.2/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/clamp.py` & `jord-0.5.2/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/geometry_types.py` & `jord-0.5.2/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/grouping.py` & `jord-0.5.2/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/lines.py` & `jord-0.5.2/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/mirroring.py` & `jord-0.5.2/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/morphology.py` & `jord-0.5.2/jord/shapely_utilities/morphology.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,49 +5,53 @@
 from shapely.geometry.base import BaseGeometry
 
 __all__ = ["closing", "opening", "erode", "erosion", "dilate", "dilation", "close"]
 
 from warg import passes_kws_to
 
 FALLBACK_CAPSTYLE = shapely.BufferCapStyle.round  # CAN BE OVERRIDDEN
+FALLBACK_JOINSTYLE = shapely.BufferCapStyle.round  # CAN BE OVERRIDDEN
 
 
 @passes_kws_to(shapely.geometry.base.BaseGeometry.buffer)
 def morphology_buffer(
     geom: BaseGeometry,
     distance: float = 1e-7,
     cap_style: shapely.BufferCapStyle = shapely.BufferCapStyle.flat,
     join_style: shapely.BufferJoinStyle = shapely.BufferJoinStyle.mitre,
     **kwargs
 ):
     if distance == 0:
         if isinstance(geom, shapely.GeometryCollection):
             return shapely.GeometryCollection(
                 [
-                    dilation(
+                    morphology_buffer(
                         g,
                         distance=distance,
                         cap_style=cap_style,
                         join_style=join_style,
                         **kwargs
                     )
                     for g in geom.geoms
                 ]
             )
 
-        if not isinstance(geom, (shapely.Polygon, shapely.MultiPolygon)):
+        if not isinstance(
+            geom, (shapely.Polygon, shapely.MultiPolygon)
+        ):  # So if line(s) or point(s)
             return geom
 
     if (
         isinstance(geom, shapely.Point) and cap_style == shapely.BufferCapStyle.flat
     ):  # parameter NONSENSE, probably not what is intended
         cap_style = FALLBACK_CAPSTYLE
+        join_style = FALLBACK_JOINSTYLE
 
     return geom.buffer(
-        distance=-distance, cap_style=cap_style, join_style=join_style, **kwargs
+        distance=distance, cap_style=cap_style, join_style=join_style, **kwargs
     )
 
 
 @passes_kws_to(morphology_buffer)
 def erosion(geom: BaseGeometry, distance: float = 1e-7, **kwargs) -> BaseGeometry:
     """
 
@@ -57,21 +61,15 @@
     :param geom: The geometry to be eroded
     :return: The eroded geometry
     """
     return morphology_buffer(geom=geom, distance=-distance, **kwargs)
 
 
 @passes_kws_to(morphology_buffer)
-def dilation(
-    geom: BaseGeometry,
-    distance: float = 1e-7,
-    cap_style: shapely.BufferCapStyle = shapely.BufferCapStyle.flat,
-    join_style: shapely.BufferJoinStyle = shapely.BufferJoinStyle.mitre,
-    **kwargs
-) -> BaseGeometry:
+def dilation(geom: BaseGeometry, distance: float = 1e-7, **kwargs) -> BaseGeometry:
     """
 
     :param cap_style:
     :param join_style:
     :param geom: The geometry to be dilated
     :param distance: Dilation amount
     :return: The dilated geometry
@@ -297,10 +295,15 @@
         matplotlib.pyplot.show()
 
     def ahfuas3232hdu():
         lr = LinearRing([(-1, -1), (1, 1), (1, 1), (1, -1), (-1, -1)])
         print(dilate(lr))
         print(lr.buffer(0))
 
-    ahfuas3232hdu()
+    def simple_dilate_example():
+        print(dilate(shapely.Point(0, 0)))
+        print(dilate(shapely.Point(0, 0), distance=0))
+
+    simple_dilate_example()
+    # ahfuas3232hdu()
     # ahfuashdu()
     # aishdjauisd()
```

### Comparing `jord-0.5.1/jord/shapely_utilities/points.py` & `jord-0.5.2/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/polygons.py` & `jord-0.5.2/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/projection.py` & `jord-0.5.2/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/rings.py` & `jord-0.5.2/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/selection.py` & `jord-0.5.2/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/jord/shapely_utilities/transformation.py` & `jord-0.5.2/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/setup.py` & `jord-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.1/tests/test_import.py` & `jord-0.5.2/tests/test_import.py`

 * *Files identical despite different names*

