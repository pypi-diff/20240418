# Comparing `tmp/cwapi3d-30.443.9.tar.gz` & `tmp/cwapi3d-30.444.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-30.443.9.tar", last modified: Wed Mar 20 19:10:03 2024, max compression
+gzip compressed data, was "cwapi3d-30.444.0.tar", last modified: Thu Apr 18 12:39:37 2024, max compression
```

## Comparing `cwapi3d-30.443.9.tar` & `cwapi3d-30.444.0.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.425593 cwapi3d-30.443.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.425593 cwapi3d-30.443.9/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    33833 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.425593 cwapi3d-30.443.9/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.433594 cwapi3d-30.443.9/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/attribute_display_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/btl_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/camera_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/coordinate_system_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/division_zone_direction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/edge_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/element_grouping_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/element_module_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/element_module_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/extended_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/facet_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/hundegger_machine_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_2x3_element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_element_combine_behaviour.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_options_aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_options_level_of_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_options_project_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/ifc_options_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/import_3dc_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/layer_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/node_symbol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/point_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/polygon_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/process_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/projection_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/rhino_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/shortcut_key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/shortcut_key_modifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/text_element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/text_object_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/vertex_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/cadwork/weinmann_mfb_version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.433594 cwapi3d-30.443.9/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-20 19:10:03.000000 cwapi3d-30.443.9/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-20 19:10:03.000000 cwapi3d-30.443.9/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:10:03.000000 cwapi3d-30.443.9/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-20 19:10:03.000000 cwapi3d-30.443.9/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.433594 cwapi3d-30.443.9/src/dimension_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/dimension_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    37247 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    16437 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/multi_layer_cover_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/multi_layer_cover_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:10:03.437594 cwapi3d-30.443.9/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-03-20 19:09:57.000000 cwapi3d-30.443.9/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.176113 cwapi3d-30.444.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.180112 cwapi3d-30.444.0/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    34319 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.180112 cwapi3d-30.444.0/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/attribute_display_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/btl_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/camera_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/coordinate_system_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/division_zone_direction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/edge_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_grouping_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_module_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_module_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/extended_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/facet_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/hundegger_machine_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_2x3_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_element_combine_behaviour.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_level_of_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_project_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35586 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_predefined_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/import_3dc_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/layer_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/node_symbol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/point_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/polygon_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/process_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/projection_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/rhino_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/shortcut_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/shortcut_key_modifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/standard_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/text_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/text_object_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/vertex_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/weinmann_mfb_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/window_geometry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/dimension_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/dimension_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    40948 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/multi_layer_cover_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/multi_layer_cover_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    17693 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-30.443.9/LICENSE` & `cwapi3d-30.444.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/PKG-INFO` & `cwapi3d-30.444.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 30.443.9
+Version: 30.444.0
 Summary: Python bindings for CwAPI3D
 Author-email: Cadwork <it@cadwork.ca>
 License: MIT License
         
         Copyright (c) 2024 Cadwork
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cwapi3d-30.443.9/README.md` & `cwapi3d-30.444.0/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/pyproject.toml` & `cwapi3d-30.444.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cwapi3d"
-version = "30.443.9"
+version = "30.444.0"
 authors = [{ name = "Cadwork", email = "it@cadwork.ca" }]
 requires-python = ">= 3.10"
 description = 'Python bindings for CwAPI3D'
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["cadwork"]
 classifiers = [
```

### Comparing `cwapi3d-30.443.9/src/attribute_controller/__init__.pyi` & `cwapi3d-30.444.0/src/attribute_controller/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,1932 +1,1783 @@
 from typing import List
 from cadwork import attribute_display_settings
 from cadwork import element_grouping_type
 from cadwork import element_type
 from cadwork import extended_settings
 from cadwork import process_type
 
-
 def get_last_error(error_code: int) -> str:
     """Gets the last error
 
     Parameters:
         error_code: error_code
 
     Returns:
         error string
     """
 
-
 def set_name(element_id_list: List[int], name: str) -> None:
     """Sets the element name
 
     Parameters:
         element_id_list: element_id_list
         name: name
 
     Returns:
         None
     """
 
-
 def set_group(element_id_list: List[int], group: str) -> None:
     """Sets the element group
 
     Parameters:
         element_id_list: element_id_list
         group: group
 
     Returns:
         None
     """
 
-
 def set_subgroup(element_id_list: List[int], subgroup: str) -> None:
     """Sets the element subgroup
 
     Parameters:
         element_id_list: element_id_list
         subgroup: subgroup
 
     Returns:
         None
     """
 
-
 def set_comment(element_id_list: List[int], comment: str) -> None:
     """Sets the element comment
 
     Parameters:
         element_id_list: element_id_list
         comment: comment
 
     Returns:
         None
     """
 
-
 def set_user_attribute(element_id_list: List[int], number: int, user_attribute: str) -> None:
     """Sets the element user attribute
 
     Parameters:
         element_id_list: element_id_list
         number: number
         user_attribute: user_attribute
 
     Returns:
         None
     """
 
-
 def set_sku(element_id_list: List[int], sku: str) -> None:
     """Sets the element SKU
 
     Parameters:
         element_id_list: element_id_list
         sku: sku
 
     Returns:
         None
     """
 
-
 def set_production_number(element_id_list: List[int], production_number: int) -> None:
     """Sets the element production number
 
     Parameters:
         element_id_list: element_id_list
         production_number: production_number
 
     Returns:
         None
     """
 
-
 def set_part_number(element_id_list: List[int], part_number: int) -> None:
     """Sets the element part number
 
     Parameters:
         element_id_list: element_id_list
         part_number: part_number
 
     Returns:
         None
     """
 
-
 def set_additional_data(element_id_list: List[int], data_id: str, data_text: str) -> None:
     """Sets the element additional data
 
     Parameters:
         element_id_list: element_id_list
         data_id: data_id
         data_text: data_text
 
     Returns:
         None
     """
 
-
 def delete_additional_data(element_id_list: List[int], data_id: str) -> None:
     """Deletes the element additional data
 
     Parameters:
         element_id_list: element_id_list
         data_id: data_id
 
     Returns:
         None
     """
 
-
 def set_user_attribute_name(number: int, user_attribute_name: str) -> None:
     """Sets the user attribute name
 
     Parameters:
         number: number
         user_attribute_name: user_attribute_name
 
     Returns:
         None
     """
 
-
 def set_process_type_and_extended_settings_from_name(element_id_list: List[int]) -> None:
     """Sets the element process type and extended settings from the element name
 
     Parameters:
         element_id_list: element_id_list
 
     Returns:
         None
     """
 
-
 def set_name_process_type(name: str, process_type: None) -> None:
     """Sets the process type for an element name
 
     Parameters:
         name: name
         process_type: process_type
 
     Returns:
         None
     """
 
-
 def set_name_extended_settings(name: str, extended_settings: None) -> None:
     """Sets the extended settings for an element name
 
     Parameters:
         name: name
         extended_settings: extended_settings
 
     Returns:
         None
     """
 
-
 def set_output_type(element_id_list: List[int], process_type: None) -> None:
     """Sets the element output type
 
     Parameters:
         element_id_list: element_id_list
         process_type: process_type
 
     Returns:
         None
     """
 
-
 def set_extended_settings(element_id_list: List[int], extended_settings: None) -> None:
     """Sets the element extended settings
 
     Parameters:
         element_id_list: element_id_list
         extended_settings: extended_settings
 
     Returns:
         None
     """
 
-
 def set_wall(a0: List[int]) -> None:
     """set wall
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_floor(a0: List[int]) -> None:
     """set floor
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_opening(element_id_list: List[int]) -> None:
     """Sets the element to opening
 
     Parameters:
         element_id_list: element_id_list
 
     Returns:
         None
     """
 
-
 def set_fastening_attribute(element_id_list: List[int], value: str) -> None:
     """Sets the element fastening attribute
 
     Parameters:
         element_id_list: element_id_list
         value: value
 
     Returns:
         None
     """
 
-
 def set_element_material(element_id_list: List[int], material: int) -> None:
     """Sets the element material
 
     Parameters:
         element_id_list: element_id_list
         material: material
 
     Returns:
         None
     """
 
-
 def set_assembly_number(element_id_list: List[int], assembly_number: str) -> None:
     """set assembly number
 
     Parameters:
         element_id_list: element_id_list
         assembly_number: assembly_number
 
     Returns:
         None
     """
 
-
 def set_list_quantity(element_id_list: List[int], list_quantity: int) -> None:
     """set list quantity
 
     Parameters:
         element_id_list: element_id_list
         list_quantity: list_quantity
 
     Returns:
         None
     """
 
-
 def set_layer_settings(element_id_list: List[int], layer_settings: None) -> None:
     """set layer settings
 
     Parameters:
         element_id_list: element_id_list
         layer_settings: layer_settings
 
     Returns:
         None
     """
 
-
 def set_ignore_in_vba_calculation(elements: List[int], ignore: bool) -> None:
     """Sets if the element should be ignored in VBA Calculation
 
     Parameters:
         elements: elements
         ignore: ignore
 
     Returns:
         None
     """
 
-
 def clear_errors() -> None:
     """clear errors
 
     Returns:
         None
     """
 
-
 def set_reference_wall_2dc(elements: List[int], _2dc_file_path: str) -> None:
     """Applies a new 2dc reference wall to an element
 
     Parameters:
         elements: elements
         _2dc_file_path: _2dc_file_path
 
     Returns:
         None
     """
 
-
 def get_user_attribute_count() -> int:
     """get user attribute count
 
     Returns:
         int
     """
 
-
 def set_standard_part(elements: List[int]) -> None:
     """Sets covers (wall,opening or floor) to standard part.
 
     Parameters:
         elements: elements
 
     Returns:
         None
     """
 
-
 def set_solid_wall(elements: List[int]) -> None:
     """Sets elements to solid wall.
 
     Parameters:
         elements: elements
 
     Returns:
         None
     """
 
-
 def set_log_wall(elements: List[int]) -> None:
     """Sets elements to log wall.
 
     Parameters:
         elements: elements
 
     Returns:
         None
     """
 
-
 def set_solid_floor(elements: List[int]) -> None:
     """Sets elements to solid floor.
 
     Parameters:
         elements: elements
 
     Returns:
         None
     """
 
-
 def set_roof(a0: List[int]) -> None:
     """set roof
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_solid_roof(elements: List[int]) -> None:
     """Sets elements to solid roof cover.
 
     Parameters:
         elements: elements
 
     Returns:
         None
     """
 
-
 def get_node_symbol(element: int) -> int:
     """get node symbol
 
     Parameters:
         element: element
 
     Returns:
         int
     """
 
-
 def set_node_symbol(elements: List[int], symbol: int) -> None:
     """set node symbol
 
     Parameters:
         elements: elements
         symbol: symbol
 
     Returns:
         None
     """
 
-
 def enable_attribute_display() -> None:
     """enable attribute display
 
     Returns:
         None
     """
 
-
 def disable_attribute_display() -> None:
     """disable attribute display
 
     Returns:
         None
     """
 
-
 def is_attribute_display_enabled() -> bool:
     """is attribute display enabled
 
     Returns:
         bool
     """
 
-
 def update_auto_attribute() -> None:
     """update auto attribute
 
     Returns:
         None
     """
 
-
 def set_additional_guid(a0: List[int], a1: str, a2: str) -> None:
     """set additional guid
 
     Parameters:
         a0: a0
         a1: a1
         a2: a2
 
     Returns:
         None
     """
 
-
 def add_item_to_group_list(a0: str) -> None:
     """add item to group list
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def add_item_to_subgroup_list(a0: str) -> None:
     """add item to subgroup list
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def add_item_to_comment_list(a0: str) -> None:
     """add item to comment list
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def add_item_to_sku_list(a0: str) -> None:
     """add item to sku list
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def add_item_to_user_attribute_list(a0: int, a1: str) -> None:
     """add item to user attribute list
 
     Parameters:
         a0: a0
         a1: a1
 
     Returns:
         None
     """
 
-
 def set_container_number(a0: List[int], a1: int) -> None:
     """set container number
 
     Parameters:
         a0: a0
         a1: a1
 
     Returns:
         None
     """
 
-
 def get_name_list_items() -> List[str]:
     """get name list items
 
     Returns:
         List[str]
     """
 
-
 def add_item_to_name_list(a0: str) -> None:
     """add item to name list
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def delete_item_from_comment_list(a0: str) -> bool:
     """delete item from comment list
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def delete_item_from_group_list(a0: str) -> bool:
     """delete item from group list
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def delete_item_from_sku_list(a0: str) -> bool:
     """delete item from sku list
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def delete_item_from_subgroup_list(a0: str) -> bool:
     """delete item from subgroup list
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def delete_item_from_user_attribute_list(a0: int, a1: str) -> bool:
     """delete item from user attribute list
 
     Parameters:
         a0: a0
         a1: a1
 
     Returns:
         bool
     """
 
-
 def set_attribute_display_settings_for_2d(a0: attribute_display_settings) -> None:
     """set attribute display settings for 2d
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_2d_with_layout(a0: attribute_display_settings) -> None:
     """set attribute display settings for 2d with layout
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_2d_without_layout(a0: attribute_display_settings) -> None:
     """set attribute display settings for 2d without layout
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_3d(a0: attribute_display_settings) -> None:
     """set attribute display settings for 3d
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_container(a0: attribute_display_settings) -> None:
     """set attribute display settings for container
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_export_solid(a0: attribute_display_settings) -> None:
     """set attribute display settings for export solid
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_framed_wall_axis(a0: attribute_display_settings) -> None:
     """set attribute display settings for framed wall axis
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_framed_wall_beam(a0: attribute_display_settings) -> None:
     """set attribute display settings for framed wall beam
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_framed_wall_opening(a0: attribute_display_settings) -> None:
     """set attribute display settings for framed wall opening
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_framed_wall_panel(a0: attribute_display_settings) -> None:
     """set attribute display settings for framed wall panel
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_log_wall_axis(a0: attribute_display_settings) -> None:
     """set attribute display settings for log wall axis
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_log_wall_beam(a0: attribute_display_settings) -> None:
     """set attribute display settings for log wall beam
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_log_wall_opening(a0: attribute_display_settings) -> None:
     """set attribute display settings for log wall opening
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_log_wall_panel(a0: attribute_display_settings) -> None:
     """set attribute display settings for log wall panel
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_machine(a0: attribute_display_settings) -> None:
     """set attribute display settings for machine
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_nesting_element(a0: attribute_display_settings) -> None:
     """set attribute display settings for nesting element
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_nesting_volume(a0: attribute_display_settings) -> None:
     """set attribute display settings for nesting volume
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_solid_wall_axis(a0: attribute_display_settings) -> None:
     """set attribute display settings for solid wall axis
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_solid_wall_beam(a0: attribute_display_settings) -> None:
     """set attribute display settings for solid wall beam
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_solid_wall_opening(a0: attribute_display_settings) -> None:
     """set attribute display settings for solid wall opening
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_attribute_display_settings_for_solid_wall_panel(a0: attribute_display_settings) -> None:
     """set attribute display settings for solid wall panel
 
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
-
 def set_framed_floor(element_id_list: List[int]) -> None:
     """Sets the elements to framed floor
 
     Parameters:
         element_id_list: element_id_list
 
     Returns:
         None
     """
 
-
 def set_framed_roof(element_id_list: List[int]) -> None:
     """Sets the elements to framed roof
 
     Parameters:
         element_id_list: element_id_list
 
     Returns:
         None
     """
 
-
 def set_framed_wall(element_id_list: List[int]) -> None:
     """Sets the element to framed wall
 
     Parameters:
         element_id_list: element_id_list
 
     Returns:
         None
     """
 
-
 def get_name_list_items_by_element_type(a0: element_type) -> List[str]:
     """get name list items by element type
 
     Parameters:
         a0: a0
 
     Returns:
         List[str]
     """
 
-
 def get_name(element_id: int) -> str:
     """Gets the element name
 
     Parameters:
         element_id: element_id
 
     Returns:
         element name
     """
 
-
 def get_group(element_id: int) -> str:
     """Gets the element group
 
     Parameters:
         element_id: element_id
 
     Returns:
         element group
     """
 
-
 def get_subgroup(element_id: int) -> str:
     """Gets the element subgroup
 
     Parameters:
         element_id: element_id
 
     Returns:
         element subgroup
     """
 
-
 def get_comment(element_id: int) -> str:
     """Gets the element comment
 
     Parameters:
         element_id: element_id
 
     Returns:
         element comment
     """
 
-
 def get_user_attribute(element_id: int, number: int) -> str:
     """Gets the element user attribute
 
     Parameters:
         element_id: element_id
         number: number
 
     Returns:
         element user attribute
     """
 
-
 def get_sku(element_id: int) -> str:
     """Gets the element SKU
 
     Parameters:
         element_id: element_id
 
     Returns:
         element SKU
     """
 
-
 def get_production_number(element_id: int) -> int:
     """Gets the element production number
 
     Parameters:
         element_id: element_id
 
     Returns:
         element production number
     """
 
-
 def get_part_number(element_id: int) -> int:
     """Gets the element part number
 
     Parameters:
         element_id: element_id
 
     Returns:
         element part number
     """
 
-
 def get_additional_data(element_id: int, data_id: str) -> str:
     """Gets the element additional data
 
     Parameters:
         element_id: element_id
         data_id: data_id
 
     Returns:
         element additional data
     """
 
-
 def get_user_attribute_name(number: int) -> str:
     """Gets the user attribute name
 
     Parameters:
         number: number
 
     Returns:
         user attribute name
     """
 
-
 def get_wall_situation(element_id: int) -> str:
     """Gets the element wall situation
 
     Parameters:
         element_id: element_id
 
     Returns:
         element wall situation
     """
 
-
 def get_element_material_name(element_id: int) -> str:
     """Gets the element material name
 
     Parameters:
         element_id: element_id
 
     Returns:
         element material name
     """
 
-
 def get_prefab_layer(element_id: int) -> str:
     """Gets the element prefab layer
 
     Parameters:
         element_id: element_id
 
     Returns:
         element prefab layer
     """
 
-
 def get_machine_calculation_set(element_id: int) -> str:
     """Gets the element machine calculation set
 
     Parameters:
         element_id: element_id
 
     Returns:
         element machine calculation set
     """
 
-
 def get_cutting_set(element_id: int) -> str:
     """Gets the element cutting set
 
     Parameters:
         element_id: element_id
 
     Returns:
         element cutting set
     """
 
-
 def get_name_process_type(name: str) -> process_type:
     """Gets the process type for an element name
 
     Parameters:
         name: name
 
     Returns:
         process type
     """
 
-
 def get_name_extended_settings(name: str) -> extended_settings:
     """Gets the extended settings for an element name
 
     Parameters:
         name: name
 
     Returns:
         extended settings
     """
 
-
 def get_output_type(element_id: int) -> process_type:
     """Gets the element output type
 
     Parameters:
         element_id: element_id
 
     Returns:
         element output type
     """
 
-
 def get_extended_settings(element_id: int) -> extended_settings:
     """Gets the element extended settings
 
     Parameters:
         element_id: element_id
 
     Returns:
         element extended settings
     """
 
-
 def get_element_type(element_id: int) -> element_type:
     """Gets the element type
 
     Parameters:
         element_id: element_id
 
     Returns:
         element type
     """
 
-
 def get_fastening_attribute(element_id: int) -> str:
     """Get the element fastening attribute
 
     Parameters:
         element_id: element_id
 
     Returns:
         element fastening attribute
     """
 
-
 def get_assembly_number(element_id: int) -> str:
     """get assembly number
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def get_list_quantity(element_id: int) -> int:
     """get list quantity
 
     Parameters:
         element_id: element_id
 
     Returns:
         int
     """
 
-
 def get_ignore_in_vba_calculation(element: int) -> bool:
     """get ignore in vba calculation
 
     Parameters:
         element: element
 
     Returns:
         bool
     """
 
-
 def get_standard_element_name(element_id: int) -> str:
     """get standard element name
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def get_steel_shape_name(element_id: int) -> str:
     """get steel shape name
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def is_beam(element_id: int) -> bool:
     """Tests if element is beam
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element beam
     """
 
-
 def is_panel(element_id: int) -> bool:
     """Tests if element is panel
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element panel
     """
 
-
 def is_opening(element_id: int) -> bool:
     """Tests if element is opening
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element opening
     """
 
-
 def is_wall(element_id: int) -> bool:
     """Tests if element is wall
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element wall
     """
 
-
 def is_floor(element_id: int) -> bool:
     """Tests if element is floor
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element floor
     """
 
-
 def is_roof(element_id: int) -> bool:
     """Tests if element is roof
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element roof
     """
 
-
 def is_metal(element_id: int) -> bool:
     """Tests if element is metal
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element metal
     """
 
-
 def is_export_solid(element_id: int) -> bool:
     """Tests if element is export solid
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element export solid
     """
 
-
 def is_container(element_id: int) -> bool:
     """Tests if element is container
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element container
     """
 
-
 def is_connector_axis(element_id: int) -> bool:
     """Tests if element is connector axis
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element connector axis
     """
 
-
 def is_drilling(element_id: int) -> bool:
     """Tests if element is drilling
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element drilling
     """
 
-
 def is_node(element_id: int) -> bool:
     """Tests if element is node
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element node
     """
 
-
 def is_auxiliary(element_id: int) -> bool:
     """Tests if element is auxiliary
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element auxiliary
     """
 
-
 def is_roof_surface(element_id: int) -> bool:
     """Tests if the element is roof surface
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element roof surface
     """
 
-
 def is_caddy_object(element_id: int) -> bool:
     """Tests if the element is caddy object
 
     Parameters:
         element_id: element_id
 
     Returns:
         is element caddy object
     """
 
-
 def is_envelope(element_id: int) -> bool:
     """is envelope
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_architecture_wall_2dc(element: int) -> bool:
     """Tests if the element has a 2dc reference wall
 
     Parameters:
         element: element
 
     Returns:
         is architecturewall 2dc
     """
 
-
 def is_architecture_wall_xml(element: int) -> bool:
     """Tests if the element has a xml reference wall
 
     Parameters:
         element: element
 
     Returns:
         is architecturewall xml
     """
 
-
 def is_surface(element_id: int) -> bool:
     """Tests if the element is a Surface
 
     Parameters:
         element_id: element_id
 
     Returns:
         is Surface
     """
 
-
 def is_line(element_id: int) -> bool:
     """Tests if the element is a Line
 
     Parameters:
         element_id: element_id
 
     Returns:
         is Line
     """
 
-
 def get_auto_attribute(element_id: int, number: int) -> str:
     """get auto attribute
 
     Parameters:
         element_id: element_id
         number: number
 
     Returns:
         str
     """
 
-
 def get_auto_attribute_name(number: int) -> str:
     """get auto attribute name
 
     Parameters:
         number: number
 
     Returns:
         str
     """
 
-
 def is_framed_wall(element_id: int) -> bool:
     """is framed wall
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_solid_wall(element_id: int) -> bool:
     """is solid wall
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_log_wall(element_id: int) -> bool:
     """is log wall
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_framed_floor(element_id: int) -> bool:
     """is framed floor
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_solid_floor(element_id: int) -> bool:
     """is solid floor
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_framed_roof(element_id: int) -> bool:
     """is framed roof
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def is_solid_roof(element_id: int) -> bool:
     """is solid roof
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def get_additional_guid(a0: int, a1: str) -> str:
     """get additional guid
 
     Parameters:
         a0: a0
         a1: a1
 
     Returns:
         str
     """
 
-
 def get_prefab_layer_all_assigned(a0: int) -> List[int]:
     """get prefab layer all assigned
 
     Parameters:
         a0: a0
 
     Returns:
         List[int]
     """
 
-
 def get_prefab_layer_with_dimensions(a0: int) -> List[int]:
     """get prefab layer with dimensions
 
     Parameters:
         a0: a0
 
     Returns:
         List[int]
     """
 
-
 def get_prefab_layer_without_dimensions(a0: int) -> List[int]:
     """get prefab layer without dimensions
 
     Parameters:
         a0: a0
 
     Returns:
         List[int]
     """
 
-
 def is_nesting_parent(a0: int) -> bool:
     """is nesting parent
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def is_nesting_raw_part(a0: int) -> bool:
     """is nesting raw part
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def get_container_number(a0: int) -> int:
     """get container number
 
     Parameters:
         a0: a0
 
     Returns:
         int
     """
 
-
 def get_container_number_with_prefix(a0: int) -> str:
     """get container number with prefix
 
     Parameters:
         a0: a0
 
     Returns:
         str
     """
 
-
 def get_group_list_items() -> List[str]:
     """get group list items
 
     Returns:
         List[str]
     """
 
-
 def get_subgroup_list_items() -> List[str]:
     """get subgroup list items
 
     Returns:
         List[str]
     """
 
-
 def get_comment_list_items() -> List[str]:
     """get comment list items
 
     Returns:
         List[str]
     """
 
-
 def get_sku_list_items() -> List[str]:
     """get sku list items
 
     Returns:
         List[str]
     """
 
-
 def get_user_attribute_list_items(a0: int) -> List[str]:
     """get user attribute list items
 
     Parameters:
         a0: a0
 
     Returns:
         List[str]
     """
 
-
 def is_circular_mep(a0: int) -> bool:
     """is circular mep
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def is_rectangular_mep(a0: int) -> bool:
     """is rectangular mep
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def get_machine_calculation_state(a0: int) -> str:
     """get machine calculation state
 
     Parameters:
         a0: a0
 
     Returns:
         str
     """
 
-
 def get_machine_calculation_set_machine_type(a0: int) -> str:
     """get machine calculation set machine type
 
     Parameters:
         a0: a0
 
     Returns:
         str
     """
 
-
 def is_btl_processing_group(a0: int) -> bool:
     """is btl processing group
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def is_hundegger_processing_group(a0: int) -> bool:
     """is hundegger processing group
 
     Parameters:
         a0: a0
 
     Returns:
         bool
     """
 
-
 def get_element_grouping_type() -> element_grouping_type:
     """Get the element grouping type (group, subgroup)
 
     Returns:
         element grouping type
     """
 
-
 def set_element_grouping_type(element_grouping_type: element_grouping_type) -> None:
     """Set the element grouping type (group, subgroup)
 
     Parameters:
         element_grouping_type: element_grouping_type
 
     Returns:
         None
     """
 
-
 def get_associated_nesting_name(element_id: int) -> str:
     """get associated nesting name
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def get_associated_nesting_number(element_id: int) -> str:
     """get associated nesting number
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def get_attribute_display_settings_for_2d() -> attribute_display_settings:
     """get attribute display settings for 2d
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_2d_with_layout() -> attribute_display_settings:
     """get attribute display settings for 2d with layout
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_2d_without_layout() -> attribute_display_settings:
     """get attribute display settings for 2d without layout
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_3d() -> attribute_display_settings:
     """get attribute display settings for 3d
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_container() -> attribute_display_settings:
     """get attribute display settings for container
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_export_solid() -> attribute_display_settings:
     """get attribute display settings for export solid
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_framed_wall_axis() -> attribute_display_settings:
     """get attribute display settings for framed wall axis
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_framed_wall_beam() -> attribute_display_settings:
     """get attribute display settings for framed wall beam
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_framed_wall_opening() -> attribute_display_settings:
     """get attribute display settings for framed wall opening
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_framed_wall_panel() -> attribute_display_settings:
     """get attribute display settings for framed wall panel
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_log_wall_axis() -> attribute_display_settings:
     """get attribute display settings for log wall axis
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_log_wall_beam() -> attribute_display_settings:
     """get attribute display settings for log wall beam
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_log_wall_opening() -> attribute_display_settings:
     """get attribute display settings for log wall opening
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_log_wall_panel() -> attribute_display_settings:
     """get attribute display settings for log wall panel
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_machine() -> attribute_display_settings:
     """get attribute display settings for machine
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_nesting_element() -> attribute_display_settings:
     """get attribute display settings for nesting element
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_nesting_volume() -> attribute_display_settings:
     """get attribute display settings for nesting volume
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_solid_wall_axis() -> attribute_display_settings:
     """get attribute display settings for solid wall axis
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_solid_wall_beam() -> attribute_display_settings:
     """get attribute display settings for solid wall beam
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_solid_wall_opening() -> attribute_display_settings:
     """get attribute display settings for solid wall opening
 
     Returns:
         attribute_display_settings
     """
 
-
 def get_attribute_display_settings_for_solid_wall_panel() -> attribute_display_settings:
     """get attribute display settings for solid wall panel
 
     Returns:
         attribute_display_settings
     """
 
-
 def is_processing(element_id: int) -> bool:
     """is processing
 
     Parameters:
         element_id: element_id
 
     Returns:
         bool
     """
 
-
 def delete_user_attribute(number: int) -> bool:
     """Delete user attribute from attribute list. The attribute is only deleted when the attribute is not used.
 
     Parameters:
         number: number
 
     Returns:
         bool deletion successfully
     """
+
+def is_attribute_visible_in_modify_window(number: int) -> bool:
+    """is attribute visible in modify window
+
+    Parameters:
+        number: number
+
+    Returns:
+        bool
+    """
+
+def set_attribute_visibility_in_modify_window(number: int, visibility: bool) -> None:
+    """set attribute visibility in modify window
+
+    Parameters:
+        number: number
+        visibility: visibility
+
+    Returns:
+        None
+    """
+
+def set_cutting_set(element_id_list: List[int], cutting_set_name: str) -> bool:
+    """set cutting set
+
+    Parameters:
+        element_id_list: element_id_list
+        cutting_set_name: cutting_set_name
+
+    Returns:
+        bool
+    """
```

### Comparing `cwapi3d-30.443.9/src/bim_controller/__init__.pyi` & `cwapi3d-30.444.0/src/bim_controller/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,326 +1,320 @@
 from typing import List
 from cadwork import ifc_2x3_element_type
 from cadwork import ifc_options
-
+from cadwork import ifc_predefined_type
 
 def get_last_error(a0: int) -> str:
     """get last error
 
     Parameters:
         a0: a0
 
     Returns:
         str
     """
 
-
 def get_ifc_guid(element_id: int) -> str:
     """get ifc guid
 
     Parameters:
         element_id: element_id
 
     Returns:
         str
     """
 
-
 def clear_errors() -> None:
     """clear errors
 
     Returns:
         None
     """
 
-
 def get_ifc2x3_element_type(element_id: int) -> ifc_2x3_element_type:
     """get ifc2x3 element type
 
     Parameters:
         element_id: element_id
 
     Returns:
         ifc_2x3_element_type
     """
 
-
 def set_ifc2x3_element_type(element_i_ds: List[int], element_type: None) -> None:
     """set ifc2x3 element type
 
     Parameters:
         element_i_ds: element_i_ds
         element_type: element_type
 
     Returns:
         None
     """
 
-
 def import_ifc_as_graphical_object(file_path: str) -> bool:
     """import ifc as graphical object
 
     Parameters:
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def import_bcf(file_path: str) -> bool:
     """import bcf
 
     Parameters:
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def export_bcf(file_path: str) -> bool:
     """export bcf
 
     Parameters:
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def export_ifc(element_i_ds: List[int], file_path: str) -> bool:
     """export ifc
 
     Parameters:
         element_i_ds: element_i_ds
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def import_ifc_return_exchange_objects(file_path: str) -> List[int]:
     """imports an IFC File and returns the ids of the Exchange Objects
 
     Parameters:
         file_path: file_path
 
     Returns:
         List[int]
     """
 
-
 def set_storey_height(building: str, storey: str, height: float) -> None:
     """set storey height
 
     Parameters:
         building: building
         storey: storey
         height: height
 
     Returns:
         None
     """
 
-
 def convert_exchange_objects(exchange_objects: List[int]) -> List[int]:
     """converts a list of Exchange Objects to Cadwork Elements
 
     Parameters:
         exchange_objects: exchange_objects
 
     Returns:
         List[int]
     """
 
-
 def export_ifc2x3_silently(element_i_ds: List[int], file_path: str) -> bool:
     """export ifc2x3 silently
 
     Parameters:
         element_i_ds: element_i_ds
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def export_ifc4_silently(element_i_ds: List[int], file_path: str) -> bool:
     """export ifc4 silently
 
     Parameters:
         element_i_ds: element_i_ds
         file_path: file_path
 
     Returns:
         bool
     """
 
-
 def export_ifc2x3_silently_with_options(element_i_ds: List[int], file_path: str, options: ifc_options) -> bool:
     """export ifc2x3 silently with options
 
     Parameters:
         element_i_ds: element_i_ds
         file_path: file_path
         options: options
 
     Returns:
         bool
     """
 
-
 def export_ifc4_silently_with_options(element_i_ds: List[int], file_path: str, options: ifc_options) -> bool:
     """export ifc4 silently with options
 
     Parameters:
         element_i_ds: element_i_ds
         file_path: file_path
         options: options
 
     Returns:
         bool
     """
 
-
 def update_bmt_structure_created_elements(element_i_ds: List[int]) -> None:
     """This function takes the specified elements and inserts them into the BMT structure and adds them to the active building and storey.
 
     Parameters:
         element_i_ds: element_i_ds
 
     Returns:
         None
     """
 
-
 def update_bmt_structure_building_storey(element_i_ds: List[int]) -> None:
     """This function takes the specified elements and inserts them into the BMT structure and adds them to the assigned Building and Storey.
 
     Parameters:
         element_i_ds: element_i_ds
 
     Returns:
         None
     """
 
-
 def get_ifc_options() -> ifc_options:
     """Get the IfcOptions with the settings used in the document // *
 
     Returns:
         IfcOptions //
     """
 
-
 def set_building_and_storey(element_id_list: List[int], building: str, storey: str) -> None:
     """set building and storey
 
     Parameters:
         element_id_list: element_id_list
         building: building
         storey: storey
 
     Returns:
         None
     """
 
-
 def get_building(element: int) -> str:
     """get building
 
     Parameters:
         element: element
 
     Returns:
         str
     """
 
-
 def get_storey(element: int) -> str:
     """get storey
 
     Parameters:
         element: element
 
     Returns:
         str
     """
 
-
 def get_storey_height(building: str, storey: str) -> float:
     """get storey height
 
     Parameters:
         building: building
         storey: storey
 
     Returns:
         float
     """
 
-
 def get_ifc2x3_element_type_string(element_type: None) -> str:
     """get ifc2x3 element type string
 
     Parameters:
         element_type: element_type
 
     Returns:
         str
     """
 
-
 def get_ifc2x3_element_type_display_string(element_type: None) -> str:
     """get ifc2x3 element type display string
 
     Parameters:
         element_type: element_type
 
     Returns:
         str
     """
 
-
 def get_all_buildings() -> List[str]:
     """get all buildings
 
     Returns:
         List[str]
     """
 
-
 def get_all_storeys(building: str) -> List[str]:
     """get all storeys
 
     Parameters:
         building: building
 
     Returns:
         List[str]
     """
 
-
 def get_element_id_from_base64_ifc_guid(a1: str) -> int:
     """get element id from base64 ifc guid
 
     Parameters:
         a1: a1
 
     Returns:
         int
     """
 
-
 def get_ifc_base64_guid(element_id: int) -> str:
     """Get IFC base64 Guid from element ID
 
     Parameters:
         element_id: element_id
 
     Returns:
         The IFC GUID in base64 string format ("28kif20KPEuBjk2m1N3ep$").
     """
+
+def get_ifc_predefined_type(element_id: int) -> 'ifc_predefined_type':
+    """Get the IfcPredefinedType of an element.
+
+    Parameters:
+        element_id: element_id
+
+    Returns:
+        IfcPredefinedType Wrapper
+    """
+
+def set_ifc_predefined_type(element_i_ds: List[int], predefined_type: None) -> None:
+    """Set a predefined type to elements. Attention, if you change the PredefinedType of the elements, you are responsible for ensuring that valid types are set
+
+    Parameters:
+        element_i_ds: element_i_ds
+        predefined_type: predefined_type
+
+    Returns:
+        None
+    """
+
```

### Comparing `cwapi3d-30.443.9/src/cadwork/attribute_display_settings.pyi` & `cwapi3d-30.444.0/src/cadwork/attribute_display_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/btl_version.pyi` & `cwapi3d-30.444.0/src/cadwork/btl_version.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/camera_data.pyi` & `cwapi3d-30.444.0/src/cadwork/camera_data.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/element_module_detail.pyi` & `cwapi3d-30.444.0/src/cadwork/element_module_detail.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/element_module_properties.pyi` & `cwapi3d-30.444.0/src/cadwork/element_module_properties.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/element_type.pyi` & `cwapi3d-30.444.0/src/cadwork/element_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/extended_settings.pyi` & `cwapi3d-30.444.0/src/cadwork/extended_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/facet_list.pyi` & `cwapi3d-30.444.0/src/cadwork/facet_list.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/hundegger_machine_type.pyi` & `cwapi3d-30.444.0/src/cadwork/hundegger_machine_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_2x3_element_type.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_2x3_element_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_options.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_options_aggregation.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_options_aggregation.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_options_level_of_detail.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_options_level_of_detail.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_options_project_data.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_options_project_data.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/ifc_options_properties.pyi` & `cwapi3d-30.444.0/src/cadwork/ifc_options_properties.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/import_3dc_options.pyi` & `cwapi3d-30.444.0/src/cadwork/import_3dc_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/layer_settings.pyi` & `cwapi3d-30.444.0/src/cadwork/layer_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/point_3d.pyi` & `cwapi3d-30.444.0/src/cadwork/point_3d.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 class point_3d:
+
+    def __init__(self, x: float, y: float, z: float) -> None: ...
     
     def dot(self, p: 'point_3d') -> float:
         """dot
 
         Parameters:
             p: p
```

### Comparing `cwapi3d-30.443.9/src/cadwork/process_type.pyi` & `cwapi3d-30.444.0/src/cadwork/process_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/rhino_options.pyi` & `cwapi3d-30.444.0/src/cadwork/rhino_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cadwork/text_object_options.pyi` & `cwapi3d-30.444.0/src/cadwork/text_object_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/connector_axis_controller/__init__.pyi` & `cwapi3d-30.444.0/src/connector_axis_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-30.444.0/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 30.443.9
+Version: 30.444.0
 Summary: Python bindings for CwAPI3D
 Author-email: Cadwork <it@cadwork.ca>
 License: MIT License
         
         Copyright (c) 2024 Cadwork
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cwapi3d-30.443.9/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-30.444.0/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 src/cadwork/ifc_2x3_element_type.pyi
 src/cadwork/ifc_element_combine_behaviour.pyi
 src/cadwork/ifc_options.pyi
 src/cadwork/ifc_options_aggregation.pyi
 src/cadwork/ifc_options_level_of_detail.pyi
 src/cadwork/ifc_options_project_data.pyi
 src/cadwork/ifc_options_properties.pyi
+src/cadwork/ifc_predefined_type.pyi
 src/cadwork/import_3dc_options.pyi
 src/cadwork/layer_settings.pyi
 src/cadwork/node_symbol.pyi
 src/cadwork/point_3d.pyi
 src/cadwork/polygon_list.pyi
 src/cadwork/process_type.pyi
 src/cadwork/projection_type.pyi
 src/cadwork/rhino_options.pyi
 src/cadwork/shortcut_key.pyi
 src/cadwork/shortcut_key_modifier.pyi
+src/cadwork/standard_element_type.pyi
 src/cadwork/text_element_type.pyi
 src/cadwork/text_object_options.pyi
 src/cadwork/vertex_list.pyi
 src/cadwork/weinmann_mfb_version.pyi
+src/cadwork/window_geometry.pyi
 src/connector_axis_controller/__init__.pyi
 src/cwapi3d.egg-info/PKG-INFO
 src/cwapi3d.egg-info/SOURCES.txt
 src/cwapi3d.egg-info/dependency_links.txt
 src/cwapi3d.egg-info/top_level.txt
 src/dimension_controller/__init__.pyi
 src/element_controller/__init__.pyi
```

### Comparing `cwapi3d-30.443.9/src/dimension_controller/__init__.pyi` & `cwapi3d-30.444.0/src/dimension_controller/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -152,7 +152,60 @@
     Parameters:
         element: element
 
     Returns:
         double
     """
 
+from cadwork import point_3d
+
+def get_distance(element: int) -> point_3d:
+    """Get the distance to the dimension reference point. The point is in the plane of the dimensioning.
+
+    Parameters:
+        element: element
+
+    Returns:
+        point_3d
+    """
+
+def get_plane_normal(element: int) -> point_3d:
+    """Get the plane normal
+
+    Parameters:
+        element: element
+
+    Returns:
+        normal
+    """
+
+def get_plane_xl(element: int) -> point_3d:
+    """Get the plane x direction
+
+    Parameters:
+        element: element
+
+    Returns:
+        x direction
+    """
+
+def get_segment_count(element: int) -> int:
+    """Get count of segments
+
+    Parameters:
+        element: element
+
+    Returns:
+        segment count
+    """
+
+def get_segment_distance(element: int, segment_index: int) -> float:
+    """Get the distance from the anchor point to the dimension segment
+
+    Parameters:
+        element: element
+        segment_index: segment_index
+
+    Returns:
+        distance
+    """
+
```

### Comparing `cwapi3d-30.443.9/src/element_controller/__init__.pyi` & `cwapi3d-30.444.0/src/element_controller/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from cadwork import edge_list
 from cadwork import element_module_properties
 from cadwork import facet_list
 from cadwork import point_3d
 from cadwork import text_object_options
+from cadwork import coordinate_system_data
 
 def get_last_error(error_code: int) -> str:
     """Gets the last error
 
     Parameters:
         error_code: error_code
 
@@ -1772,7 +1773,155 @@
         zl: zl
         text_options: text_options
 
     Returns:
         int
     """
 
+def convert_surfaces_to_roof_surfaces(elements: List[int], roof_name: str) -> None:
+    """converts surfaces to roof surfaces
+
+    Parameters:
+        elements: elements
+        roof_name: roof_name
+
+    Returns:
+        None
+    """
+
+def start_standard_element_dialog(standard_element_type: None) -> str:
+    """Starts the standard element dialogue based on the chosen element type
+
+    Parameters:
+        standard_element_type: standard_element_type
+
+    Returns:
+        Returns guid of selected standard element if item is valid, else null
+    """
+
+def remove_standard_connector_axis(a0: str) -> None:
+    """remove standard connector axis
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        None
+    """
+
+def remove_standard_beam(guid: str) -> None:
+    """remove standard beam
+
+    Parameters:
+        guid: guid
+
+    Returns:
+        None
+    """
+
+def remove_standard_panel(guid: str) -> None:
+    """remove standard panel
+
+    Parameters:
+        guid: guid
+
+    Returns:
+        None
+    """
+
+def remove_standard_container(guid: str) -> None:
+    """remove standard container
+
+    Parameters:
+        guid: guid
+
+    Returns:
+        None
+    """
+
+def remove_standard_export_solid(guid: str) -> None:
+    """remove standard export solid
+
+    Parameters:
+        guid: guid
+
+    Returns:
+        None
+    """
+
+def get_user_element_ids_with_count(count: int) -> List[int]:
+    """get user element ids with count
+
+    Parameters:
+        count: count
+
+    Returns:
+        List[int]
+    """
+
+def cut_scarf_straight(elements: List[int], length: float, depth: float, clearance_length: float, clearance_depth: float, clearance_hook: float, drilling_count: int, drilling_diameter: float, drilling_tolerance: float) -> None:
+    """cut scarf straight
+
+    Parameters:
+        elements: elements
+        length: length
+        depth: depth
+        clearance_length: clearance_length
+        clearance_depth: clearance_depth
+        clearance_hook: clearance_hook
+        drilling_count: drilling_count
+        drilling_diameter: drilling_diameter
+        drilling_tolerance: drilling_tolerance
+
+    Returns:
+        None
+    """
+
+def cut_scarf_diagonal(elements: List[int], length: float, depth: float, clearance_length: float, clearance_depth: float, drilling_count: int, drilling_diameter: float, drilling_tolerance: float) -> None:
+    """cut scarf diagonal
+
+    Parameters:
+        elements: elements
+        length: length
+        depth: depth
+        clearance_length: clearance_length
+        clearance_depth: clearance_depth
+        drilling_count: drilling_count
+        drilling_diameter: drilling_diameter
+        drilling_tolerance: drilling_tolerance
+
+    Returns:
+        None
+    """
+
+def cut_scarf_with_wedge(elements: List[int], length: float, depth: float, clearance_length: float, clearance_depth: float, wedge_width: float, drilling_count: int, drilling_diameter: float, drilling_tolerance: float) -> None:
+    """cut scarf with wedge
+
+    Parameters:
+        elements: elements
+        length: length
+        depth: depth
+        clearance_length: clearance_length
+        clearance_depth: clearance_depth
+        wedge_width: wedge_width
+        drilling_count: drilling_count
+        drilling_diameter: drilling_diameter
+        drilling_tolerance: drilling_tolerance
+
+    Returns:
+        None
+    """
+
+def cut_beam_end_profile(elements: List[int], profile_name: str, on_start_face: bool, on_end_face: bool) -> None:
+    """cut beam end profile
+
+    Parameters:
+        elements: elements
+        profile_name: profile_name
+        on_start_face: on_start_face
+        on_end_face: on_end_face
+
+    Returns:
+        None
+    """
+
+
```

### Comparing `cwapi3d-30.443.9/src/endtype_controller/__init__.pyi` & `cwapi3d-30.444.0/src/endtype_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/file_controller/__init__.pyi` & `cwapi3d-30.444.0/src/file_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/list_controller/__init__.pyi` & `cwapi3d-30.444.0/src/list_controller/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -139,7 +139,30 @@
         a2: a2
         a3: a3
 
     Returns:
         None
     """
 
+def export_cover_list(element_id_list: List[int], file_path: str) -> None:
+    """Exports a Wall/Roof/Floor list
+
+    Parameters:
+        element_id_list: element_id_list
+        file_path: file_path
+
+    Returns:
+        None
+    """
+
+def export_cover_list_with_settings(element_id_list: List[int], file_path: str, settings_file_path: str) -> None:
+    """Exports a Wall/Roof/Floor list with settings file
+
+    Parameters:
+        element_id_list: element_id_list
+        file_path: file_path
+        settings_file_path: settings_file_path
+
+    Returns:
+        None
+    """
+
```

### Comparing `cwapi3d-30.443.9/src/machine_controller/__init__.pyi` & `cwapi3d-30.444.0/src/machine_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/material_controller/__init__.pyi` & `cwapi3d-30.444.0/src/material_controller/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -550,7 +550,301 @@
     Parameters:
         group: group
 
     Returns:
         parent group name
     """
 
+def get_material_color_assignment_for_nodes(a0: int) -> int:
+    """get material color assignment for nodes
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_nodes(a0: int, a1: int) -> None:
+    """set material color assignment for nodes
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_standard_axes(a0: int) -> int:
+    """get material color assignment for standard axes
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_standard_axes(a0: int, a1: int) -> None:
+    """set material color assignment for standard axes
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_drillings(a0: int) -> int:
+    """get material color assignment for drillings
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_drillings(a0: int, a1: int) -> None:
+    """set material color assignment for drillings
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_mep_axes(a0: int) -> int:
+    """get material color assignment for mep axes
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_mep_axes(a0: int, a1: int) -> None:
+    """set material color assignment for mep axes
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_beams(a0: int) -> int:
+    """get material color assignment for beams
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_beams(a0: int, a1: int) -> None:
+    """set material color assignment for beams
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_panels(a0: int) -> int:
+    """get material color assignment for panels
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_panels(a0: int, a1: int) -> None:
+    """set material color assignment for panels
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_auxiliary_elements(a0: int) -> int:
+    """get material color assignment for auxiliary elements
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_auxiliary_elements(a0: int, a1: int) -> None:
+    """set material color assignment for auxiliary elements
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_material_color_assignment_for_surfaces(a0: int) -> int:
+    """get material color assignment for surfaces
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_material_color_assignment_for_surfaces(a0: int, a1: int) -> None:
+    """set material color assignment for surfaces
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_color(a0: int) -> int:
+    """get texture color
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_texture_color(a0: int, a1: int) -> None:
+    """set texture color
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_transparency(a0: int) -> int:
+    """get texture transparency
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        int
+    """
+
+def set_texture_transparency(a0: int, a1: int) -> None:
+    """set texture transparency
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_rotation_angle(a0: int) -> float:
+    """get texture rotation angle
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        float
+    """
+
+def set_texture_rotation_angle(a0: int, a1: float) -> None:
+    """set texture rotation angle
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_length_alignment(a0: int) -> bool:
+    """get texture length alignment
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        bool
+    """
+
+def set_texture_length_alignment(a0: int, a1: bool) -> None:
+    """set texture length alignment
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_zoom_x(a0: int) -> float:
+    """get texture zoom x
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        float
+    """
+
+def set_texture_zoom_x(a0: int, a1: float) -> None:
+    """set texture zoom x
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
+def get_texture_zoom_y(a0: int) -> float:
+    """get texture zoom y
+
+    Parameters:
+        a0: a0
+
+    Returns:
+        float
+    """
+
+def set_texture_zoom_y(a0: int, a1: float) -> None:
+    """set texture zoom y
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        None
+    """
+
```

### Comparing `cwapi3d-30.443.9/src/multi_layer_cover_controller/__init__.pyi` & `cwapi3d-30.444.0/src/multi_layer_cover_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/roof_controller/__init__.pyi` & `cwapi3d-30.444.0/src/roof_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/scene_controller/__init__.pyi` & `cwapi3d-30.444.0/src/scene_controller/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -113,7 +113,72 @@
     Parameters:
         a0: a0
 
     Returns:
         None
     """
 
+def is_scene_present(name: str) -> bool:
+    """Queries of scene with name is present
+
+    Parameters:
+        name: name
+
+    Returns:
+        presence of scene
+    """
+
+def set_group_tab_color(scene_group_name: str, red: int, green: int, blue: int) -> None:
+    """set group tab color
+
+    Parameters:
+        scene_group_name: scene_group_name
+        red: red
+        green: green
+        blue: blue
+
+    Returns:
+        None
+    """
+
+def rename_scene_group(old_name: str, new_name: str) -> None:
+    """rename scene group
+
+    Parameters:
+        old_name: old_name
+        new_name: new_name
+
+    Returns:
+        None
+    """
+
+def get_group_index_by_name(scene_group_name: str) -> int:
+    """get group index by name
+
+    Parameters:
+        scene_group_name: scene_group_name
+
+    Returns:
+        int
+    """
+
+def rename_scene_group_by_index(group_index: int, new_name: str) -> None:
+    """rename scene group by index
+
+    Parameters:
+        group_index: group_index
+        new_name: new_name
+
+    Returns:
+        None
+    """
+
+def group_scences_with_name(a0: List[str], a1: str) -> int:
+    """group scences with name
+
+    Parameters:
+        a0: a0
+        a1: a1
+
+    Returns:
+        int
+    """
```

### Comparing `cwapi3d-30.443.9/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-30.444.0/src/shop_drawing_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.443.9/src/utility_controller/__init__.pyi` & `cwapi3d-30.444.0/src/utility_controller/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List
+from typing import Tuple
 from cadwork import point_3d
+from cadwork import window_geometry
 
 def get_last_error(error_code: int) -> str:
     """Gets the last error
 
     Parameters:
         error_code: error_code
 
@@ -1034,10 +1036,24 @@
         snapshot
     """
 
 def get_3d_gui_upper_left_screen_coordinates() -> Tuple[int, int]:
     """get 3d gui upper left screen coordinates
 
     Returns:
-        Tuple[int, int]
+        coordinates of the upper left corner of the 3D GUI
+    """
+
+def get_3d_main_window_geometry() -> 'window_geometry':
+    """get 3d main window geometry
+
+    Returns:
+        window geometry
+    """
+
+def get_project_data_keys() -> List[str]:
+    """get project data keys
+
+    Returns:
+        List[str]
     """
```

### Comparing `cwapi3d-30.443.9/src/visualization_controller/__init__.pyi` & `cwapi3d-30.444.0/src/visualization_controller/__init__.pyi`

 * *Files identical despite different names*

