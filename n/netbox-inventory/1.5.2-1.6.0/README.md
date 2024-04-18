# Comparing `tmp/netbox-inventory-1.5.2.tar.gz` & `tmp/netbox_inventory-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.5.2.tar", last modified: Fri Dec 22 07:46:33 2023, max compression
+gzip compressed data, was "netbox_inventory-1.6.0.tar", last modified: Thu Apr 18 14:53:17 2024, max compression
```

## Comparing `netbox-inventory-1.5.2.tar` & `netbox_inventory-1.6.0.tar`

### file list

```diff
@@ -1,116 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.387103 netbox-inventory-1.5.2/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.391103 netbox-inventory-1.5.2/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.391103 netbox-inventory-1.5.2/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/forms/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.391103 netbox-inventory-1.5.2/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/0005_delivery_asset_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18811 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.383103 netbox-inventory-1.5.2/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.395103 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_reassign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/delivery.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.395103 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.395103 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.399103 netbox-inventory-1.5.2/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.399103 netbox-inventory-1.5.2/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.399103 netbox-inventory-1.5.2/netbox_inventory/tests/delivery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/delivery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/delivery/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/delivery/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.399103 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.399103 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2023-12-22 07:46:33.000000 netbox-inventory-1.5.2/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-12-22 07:46:33.000000 netbox-inventory-1.5.2/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 07:46:33.000000 netbox-inventory-1.5.2/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 07:46:33.000000 netbox-inventory-1.5.2/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-22 07:46:24.000000 netbox-inventory-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 07:46:33.403103 netbox-inventory-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.580691 netbox_inventory-1.6.0/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.580691 netbox_inventory-1.6.0/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21988 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.572691 netbox_inventory-1.6.0/netbox_inventory/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/management/commands/check_asset_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0006_purchase_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18925 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.572691 netbox_inventory-1.6.0/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/delivery.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/setup.cfg
```

### Comparing `netbox-inventory-1.5.2/LICENSE` & `netbox_inventory-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/PKG-INFO` & `netbox_inventory-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.5.2
+Version: 1.6.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,23 +67,24 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.5.x to work. Older versions of the plugin
+This plugin requires netbox version 3.7.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
 |       3.5      | 1.3.x & 1.4.x  |
 |       3.6      |      1.5.x     |
+|       3.7      |      1.6.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.5.2/README.md` & `netbox_inventory-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,24 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.5.x to work. Older versions of the plugin
+This plugin requires netbox version 3.7.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
 |       3.5      | 1.3.x & 1.4.x  |
 |       3.6      |      1.5.x     |
+|       3.7      |      1.6.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/__init__.py` & `netbox_inventory-1.6.0/netbox_inventory/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     name = 'netbox_inventory'
     verbose_name = 'NetBox Inventory'
     version = __version__
     description = 'Inventory asset management in NetBox'
     author = 'Matej Vadnjal'
     author_email = 'matej.vadnjal@arnes.si'
     base_url = 'inventory'
-    min_version = '3.6.0'
+    min_version = '3.7.0'
     default_settings = {
         'top_level_menu': True,
         'used_status_name': 'used',
         'stored_status_name': 'stored',
         'sync_hardware_serial_asset_tag': False,
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/analyzers.py` & `netbox_inventory-1.6.0/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/api/nested_serializers.py` & `netbox_inventory-1.6.0/netbox_inventory/api/nested_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:purchase-detail'
     )
     supplier = NestedSupplierSerializer(read_only=True)
 
     class Meta:
         model = Purchase
-        fields = ('id', 'url', 'display', 'supplier', 'name', 'date')
+        fields = ('id', 'url', 'display', 'supplier', 'name', 'status', 'date')
 
 
 class NestedDeliverySerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:delivery-detail'
     )
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/api/serializers.py` & `netbox_inventory-1.6.0/netbox_inventory/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     supplier = NestedSupplierSerializer()
     asset_count = serializers.IntegerField(read_only=True)
     delivery_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = Purchase
         fields = (
-            'id', 'url', 'display', 'supplier', 'name', 'date', 'description',
+            'id', 'url', 'display', 'supplier', 'name', 'status', 'date', 'description',
             'comments', 'tags', 'custom_fields', 'created', 'last_updated',
             'asset_count', 'delivery_count',
         )
 
 
 class DeliverySerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/api/urls.py` & `netbox_inventory-1.6.0/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/api/views.py` & `netbox_inventory-1.6.0/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/filtersets.py` & `netbox_inventory-1.6.0/netbox_inventory/filtersets.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dcim.filtersets import DeviceFilterSet, InventoryItemFilterSet, ModuleFilterSet
 from dcim.models import Manufacturer, DeviceType, ModuleType, Site, Location
 from netbox.filtersets import NetBoxModelFilterSet
 from utilities import filters
 from tenancy.filtersets import ContactModelFilterSet
 from tenancy.models import Contact, Tenant
-from .choices import HardwareKindChoices, AssetStatusChoices
+from .choices import HardwareKindChoices, AssetStatusChoices, PurchaseStatusChoices
 from .models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from .utils import query_located, get_asset_custom_fields_search_filters
 
 
 class AssetFilterSet(NetBoxModelFilterSet):
     status = django_filters.MultipleChoiceFilter(
         choices=AssetStatusChoices,
@@ -327,14 +327,17 @@
 
 class PurchaseFilterSet(NetBoxModelFilterSet):
     supplier_id = django_filters.ModelMultipleChoiceFilter(
         field_name='supplier',
         queryset=Supplier.objects.all(),
         label='Supplier (ID)',
     )
+    status = django_filters.MultipleChoiceFilter(
+        choices=PurchaseStatusChoices,
+    )
     date = django_filters.DateFromToRangeFilter()
 
     class Meta:
         model = Purchase
         fields = (
             'id', 'supplier', 'name', 'date', 'description'
         )
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/assign.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/bulk.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/bulk.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelBulkEditForm, NetBoxModelImportForm
 from utilities.forms import add_blank_choice
 from utilities.forms.fields import (
     CommentField, CSVChoiceField, CSVModelChoiceField,
     DynamicModelChoiceField
 )
+from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact, Tenant
-from ..choices import AssetStatusChoices, HardwareKindChoices
+from ..choices import AssetStatusChoices, HardwareKindChoices, PurchaseStatusChoices
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_plugin_setting
 
 __all__ = (
     'AssetBulkEditForm',
     'AssetImportForm',
     'SupplierImportForm',
@@ -70,19 +71,23 @@
         required=not Asset._meta.get_field('purchase').blank,
     )
     delivery = DynamicModelChoiceField(
         queryset=Delivery.objects.all(),
         help_text=Asset._meta.get_field('delivery').help_text,
         required=not Asset._meta.get_field('delivery').blank,
     )
-    warranty_start = forms.CharField(
+    warranty_start = forms.DateField(
+        label='Warranty start',
         required=False,
+        widget=DatePicker()
     )
-    warranty_end = forms.CharField(
+    warranty_end = forms.DateField(
+        label='Warranty end',
         required=False,
+        widget=DatePicker()
     )
     tenant = DynamicModelChoiceField(
         queryset=Tenant.objects.all(),
         help_text=Asset._meta.get_field('tenant').help_text,
         required=not Asset._meta.get_field('tenant').blank,
     )
     contact = DynamicModelChoiceField(
@@ -177,14 +182,19 @@
         help_text='Purchase through which this asset was purchased. See "Import settings" for more info.',
         required=False,
     )
     purchase_date = forms.DateField(
         help_text='Date when this purchase was made.',
         required=False,
     )
+    purchase_status = CSVChoiceField(
+        choices=PurchaseStatusChoices,
+        help_text='Status of purchase',
+        required=False
+    )
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
         to_field_name='name',
         help_text='Legal entity this purchase was made from. Required if a new purchase is given.',
         required=False,
     )
     tenant = CSVModelChoiceField(
@@ -202,16 +212,16 @@
 
     class Meta:
         model = Asset
         fields = (
             'name', 'asset_tag', 'serial', 'status',
             'hardware_kind', 'manufacturer', 'model_name', 'part_number',
             'model_comments', 'storage_site', 'storage_location',
-            'owner', 'supplier', 'purchase', 'purchase_date', 'delivery',
-            'delivery_date', 'receiving_contact', 'warranty_start',
+            'owner', 'supplier', 'purchase', 'purchase_date', 'purchase_status',
+            'delivery', 'delivery_date', 'receiving_contact', 'warranty_start',
             'warranty_end', 'comments', 'tenant', 'contact', 'tags',
         )
 
     def clean_model_name(self):
         hardware_kind = self.cleaned_data.get('hardware_kind')
         manufacturer = self.cleaned_data.get('manufacturer')
         model = self.cleaned_data.get('model_name')
@@ -294,15 +304,18 @@
         try:
             # handle creating related resources if they don't exist and enabled in settings
             if (get_plugin_setting('asset_import_create_purchase')
                 and self.data.get('purchase') and self.data.get('supplier')):
                 purchase, _ = Purchase.objects.get_or_create(
                     name=self.data.get('purchase'),
                     supplier=self._get_or_create_related('supplier'),
-                    defaults={'date': self._get_clean_value('purchase_date')}
+                    defaults={
+                        'date': self._get_clean_value('purchase_date'),
+                        'status': self._get_clean_value('purchase_status'),
+                    }
                 )
                 if self.data.get('delivery'):
                     Delivery.objects.get_or_create(
                         name=self.data.get('delivery'),
                         purchase=purchase,
                         defaults={
                             'date': self._get_clean_value('delivery_date'),
@@ -422,25 +435,36 @@
 class PurchaseImportForm(NetBoxModelImportForm):
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
         to_field_name='name',
         help_text='Legal entity this purchase was made at. It must exist when importing.',
         required=True,
     )
-    
+    status = CSVChoiceField(
+        choices=PurchaseStatusChoices,
+        help_text='Status of purchase',
+    )
+
     class Meta:
         model = Purchase
         fields = (
-            'name', 'date', 'supplier', 'description', 'comments', 'tags'
+            'name', 'date', 'status', 'supplier', 'description', 'comments', 'tags'
         )
 
 
 class PurchaseBulkEditForm(NetBoxModelBulkEditForm):
-    date = forms.CharField(
+    status = forms.ChoiceField(
+        choices=add_blank_choice(PurchaseStatusChoices),
+        required=False,
+        initial='',
+    )
+    date = forms.DateField(
+        label='Date',
         required=False,
+        widget=DatePicker()
     )
     supplier = DynamicModelChoiceField(
         queryset=Supplier.objects.all(),
         required=False,
         label='Supplier',
     )
     description = forms.CharField(
@@ -448,15 +472,15 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = Purchase
     fieldsets = (
-        ('General', ('date', 'supplier', 'description',)),
+        ('General', ('date', 'status', 'supplier', 'description',)),
     )
     nullable_fields = ('date', 'description',)
 
 
 class DeliveryImportForm(NetBoxModelImportForm):
     purchase = CSVModelChoiceField(
         queryset=Purchase.objects.all(),
@@ -475,16 +499,18 @@
         model = Delivery
         fields = (
             'name', 'date', 'purchase', 'receiving_contact', 'description', 'comments', 'tags'
         )
 
 
 class DeliveryBulkEditForm(NetBoxModelBulkEditForm):
-    date = forms.CharField(
+    date = forms.DateField(
+        label='Date',
         required=False,
+        widget=DatePicker()
     )
     purchase = DynamicModelChoiceField(
         queryset=Purchase.objects.all(),
         required=False,
         label='Purchase',
     )
     receiving_contact = DynamicModelChoiceField(
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/bulk_add.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/create.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/filters.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dcim.models import Device, DeviceType, Manufacturer, ModuleType, Site, Location, Rack
 from netbox.forms import NetBoxModelFilterSetForm
 from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
 from utilities.forms.fields import DynamicModelMultipleChoiceField, TagFilterField
 from utilities.forms.widgets import DatePicker
 from tenancy.forms import ContactModelFilterForm
 from tenancy.models import Contact, Tenant
-from ..choices import HardwareKindChoices, AssetStatusChoices
+from ..choices import HardwareKindChoices, AssetStatusChoices, PurchaseStatusChoices
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
 __all__ = (
     'AssetFilterForm',
     'SupplierFilterForm',
     'PurchaseFilterForm',
@@ -251,22 +251,26 @@
     tag = TagFilterField(model)
 
 
 class PurchaseFilterForm(NetBoxModelFilterSetForm):
     model = Purchase
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
-        ('Purchase', ('supplier_id', 'date_after', 'date_before')),
+        ('Purchase', ('supplier_id', 'status', 'date_after', 'date_before')),
     )
 
     supplier_id = DynamicModelMultipleChoiceField(
         queryset=Supplier.objects.all(),
         required=False,
         label='Supplier',
     )
+    status = forms.MultipleChoiceField(
+        choices=PurchaseStatusChoices,
+        required=False,
+    )
     date_after = forms.DateField(
         required=False,
         label='Purchased on or after',
         widget=DatePicker,
     )
     date_before = forms.DateField(
         required=False,
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/models.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,21 +225,22 @@
             'tags',
         )
 
 
 class PurchaseForm(NetBoxModelForm):
     comments = CommentField()
 
-    fieldsets = (('Purchase', ('supplier', 'name', 'date', 'description', 'tags')),)
+    fieldsets = (('Purchase', ('supplier', 'name', 'status', 'date', 'description', 'tags')),)
 
     class Meta:
         model = Purchase
         fields = (
             'supplier',
             'name',
+            'status',
             'date',
             'description',
             'comments',
             'tags',
         )
         widgets = {
             'date': DatePicker(),
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/forms/reassign.py` & `netbox_inventory-1.6.0/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/graphql.py` & `netbox_inventory-1.6.0/netbox_inventory/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/migrations/0001_initial_prod.py` & `netbox_inventory-1.6.0/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox_inventory-1.6.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox_inventory-1.6.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/migrations/0005_delivery_asset_delivery.py` & `netbox_inventory-1.6.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/models.py` & `netbox_inventory-1.6.0/netbox_inventory/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from datetime import date
 
-from django.contrib.contenttypes.fields import GenericRelation
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
 
 from netbox.models import NetBoxModel, NestedGroupModel
-from .choices import HardwareKindChoices, AssetStatusChoices
+from netbox.models.features import ContactsMixin, ImageAttachmentsMixin
+from .choices import HardwareKindChoices, AssetStatusChoices, PurchaseStatusChoices
 from .utils import asset_clear_old_hw, asset_set_new_hw, get_prechange_field, get_plugin_setting, get_status_for
 
 
-class Asset(NetBoxModel):
+class Asset(NetBoxModel, ImageAttachmentsMixin):
     """
     An Asset represents a piece of hardware we want to keep track of. It has a
     make (model, part number) that is one of: Device Type, Module Type or
     InventoryItem Type.
 
     Asset must have a serial number, can have an asset tag (inventory number). It
     must have one of DeviceType, ModuleType or InventoryItemType. It can have a
@@ -179,18 +179,14 @@
         verbose_name='Warranty End',
     )
 
     comments = models.TextField(
         blank=True
     )
 
-    images = GenericRelation(
-        to='extras.ImageAttachment'
-    )
-
     clone_fields = [
         'name', 'asset_tag', 'status', 'device_type', 'module_type',
         'inventoryitem_type', 'owner', 'purchase', 'delivery',
         'warranty_start', 'warranty_end', 'tenant', 'contact', 'storage_location',
         'comments'
     ]
 
@@ -384,15 +380,15 @@
             ('device_type', 'serial'),
             ('module_type', 'serial'),
             ('inventoryitem_type', 'serial'),
             ('owner', 'asset_tag'),
         )
 
 
-class Supplier(NetBoxModel):
+class Supplier(NetBoxModel, ContactsMixin):
     """
     Supplier is a legal entity that sold some assets that we keep track of.
     This can be the same entity as Manufacturer or a separate one. However
     netbox_inventory keeps track of Suppliers separate from Manufacturers.
     """
     name = models.CharField(
         max_length=100,
@@ -402,17 +398,14 @@
         max_length=100,
         unique=True
     )
     description = models.CharField(
         max_length=200,
         blank=True
     )
-    contacts = GenericRelation(
-        to='tenancy.ContactAssignment'
-    )
     comments = models.TextField(
         blank=True
     )
 
     clone_fields = [
         'description', 'comments'
     ]
@@ -438,37 +431,45 @@
         help_text='Legal entity this purchase was made at',
         to='netbox_inventory.Supplier',
         on_delete=models.PROTECT,
         related_name='purchases',
         blank=False,
         null=False,
     )
+    status = models.CharField(
+        max_length=30,
+        choices=PurchaseStatusChoices,
+        help_text='Status of purchase',
+    )
     date = models.DateField(
         help_text='Date when this purchase was made',
         blank=True,
         null=True,
     )
     description = models.CharField(
         max_length=200,
         blank=True
     )
     comments = models.TextField(
         blank=True
     )
 
     clone_fields = [
-        'supplier', 'date', 'description', 'comments'
+        'supplier', 'date', 'status', 'description', 'comments'
     ]
 
     class Meta:
         ordering = ['supplier', 'name']
         unique_together = (
             ('supplier', 'name'),
         )
 
+    def get_status_color(self):
+        return PurchaseStatusChoices.colors.get(self.status)
+
     def __str__(self):
         return f'{self.supplier} {self.name}'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:purchase', args=[self.pk])
 
 
@@ -524,15 +525,15 @@
     def __str__(self):
         return f'{self.purchase} {self.name}'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:delivery', args=[self.pk])
 
 
-class InventoryItemType(NetBoxModel):
+class InventoryItemType(NetBoxModel, ImageAttachmentsMixin):
     """
     Inventory Item Type is a model (make, part number) of an Inventory Item. In
     that it is simmilar to Device Type or Module Type.
     """
     manufacturer = models.ForeignKey(
         to='dcim.Manufacturer',
         on_delete=models.PROTECT,
@@ -557,17 +558,14 @@
         blank=True,
         null=True,
         verbose_name='Inventory Item Group',
     )
     comments = models.TextField(
         blank=True
     )
-    images = GenericRelation(
-        to='extras.ImageAttachment'
-    )
 
     clone_fields = [
         'manufacturer',
     ]
 
     class Meta:
         ordering = ['manufacturer', 'model']
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/navigation.py` & `netbox_inventory-1.6.0/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/search.py` & `netbox_inventory-1.6.0/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/signals.py` & `netbox_inventory-1.6.0/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tables.py` & `netbox_inventory-1.6.0/netbox_inventory/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,15 @@
 class PurchaseTable(NetBoxTable):
     supplier = tables.Column(
         linkify=True,
     )
     name = tables.Column(
         linkify=True,
     )
+    status = columns.ChoiceFieldColumn()
     delivery_count = columns.LinkedCountColumn(
         viewname='plugins:netbox_inventory:delivery_list',
         url_params={'purchase_id': 'pk'},
         verbose_name='Deliveries',
     )
     asset_count = columns.LinkedCountColumn(
         viewname='plugins:netbox_inventory:asset_list',
@@ -328,14 +329,15 @@
     class Meta(NetBoxTable.Meta):
         model = Purchase
         fields = (
             'pk',
             'id',
             'name',
             'supplier',
+            'status',
             'date',
             'description',
             'comments',
             'delivery_count',
             'asset_count',
             'tags',
             'created',
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/template_content.py` & `netbox_inventory-1.6.0/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/delivery.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/delivery.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
               <td>{{ object.name }}</td>
             </tr>
             <tr>
               <th scope="row">Supplier</th>
               <td>{{ object.supplier|linkify }}</td>
             </tr>
             <tr>
+              <th scope="row">Status</th>
+              <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
+            </tr>
+            <tr>
               <th scope="row">Date</th>
               <td>{{ object.date|annotated_date|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Description</th>
               <td>{{ object.description|placeholder }}</td>
             </tr>
```

#### html2text {}

```diff
@@ -2,14 +2,16 @@
 load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
 }}
 _{_{_ _o_b_j_e_c_t_._s_u_p_p_l_i_e_r_ _}_}
 {% endblock %} {% block content %}
 **** PPuurrcchhaassee ****
 NNaammee        {{ object.name }}
 SSuupppplliieerr    {{ object.supplier|linkify }}
+SSttaattuuss      {% badge object.get_status_display bg_color=object.get_status_color
+            %}
 DDaattee        {{ object.date|annotated_date|placeholder }}
 DDeessccrriippttiioonn {{ object.description|placeholder }}
 DDeelliivveerriieess  _{_{_ _d_e_l_i_v_e_r_y___c_o_u_n_t_ _}_}
 AAsssseettss      _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         inventoryitem_type1 = InventoryItemType.objects.create(model='II Type 1', manufacturer=manufacturer)
         site1 = Site.objects.create(name='Site 1', slug='site1')
         role1 = DeviceRole.objects.create(name='Device Role 1', slug='devicerole1')
         cls.device1 = Device.objects.create(name='Device 1', role=role1, device_type=device_type1, site=site1, status='active')
         cls.device2 = Device.objects.create(name='Device 2', role=role1, device_type=device_type2, site=site1, status='active')
         cls.inventoryitem1 = InventoryItem.objects.create(device=cls.device1, name='II 1')
         supplier1 = Supplier.objects.create(name='Supplier1', slug='supplier1')
-        cls.purchase1 = Purchase.objects.create(name='Purchase1', supplier=supplier1)
+        cls.purchase1 = Purchase.objects.create(name='Purchase1', supplier=supplier1, status='closed')
         cls.delivery1 = Delivery.objects.create(name='Delivery1', purchase=cls.purchase1)
 
         Asset.objects.create(name='Asset 1', serial='asset1', device_type=device_type1)
         Asset.objects.create(name='Asset 2', serial='asset2', device_type=device_type1)
         Asset.objects.create(name='Asset 3', serial='asset3', device_type=device_type1)
 
         cls.create_data = [
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_models.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         self.supplier1 = Supplier.objects.create(
             name='Supplier1',
             slug='supplier1',
         )
         self.purchase1 = Purchase.objects.create(
             name='Purchase1',
             supplier=self.supplier1,
+            status='closed',
         )
         self.purchase2 = Purchase.objects.create(
             name='Purchase2',
             supplier=self.supplier1,
+            status='closed',
         )
         self.delivery1 = Delivery.objects.create(
             name='Delivery1',
             purchase=self.purchase1,
         )
         self.site1 = Site.objects.create(
             name='site1',
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,20 @@
         supplier1 = Supplier.objects.create(
             name='Supplier1',
             slug='supplier1',
         )
         purchase1 = Purchase.objects.create(
             name='Purchase1',
             supplier=supplier1,
+            status='closed',
         )
         purchase2 = Purchase.objects.create(
             name='Purchase2',
             supplier=supplier1,
+            status='closed',
         )
         delivery1 = Delivery.objects.create(
             name='the_delivery',
             purchase=purchase1,
         )
         delivery2 = Delivery.objects.create(
             name='the_delivery',
@@ -163,14 +165,15 @@
         supplier1 = Supplier.objects.create(
             name='Supplier1-autoset',
             slug='supplier1-autoset',
         )
         purchase1 = Purchase.objects.create(
             name='Purchase1-autoset',
             supplier=supplier1,
+            status='closed',
         )
         delivery1 = Delivery.objects.create(
             name='Delivery1-autoset',
             purchase=purchase1,
         )
 
         form_data = {
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views_create.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/custom.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/delivery/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     bulk_update_data = {
         'description': 'new description',
     }
 
     @classmethod
     def setUpTestData(cls) -> None:
         supplier1 = Supplier.objects.create(name='Supplier1', slug='supplier1')
-        purchase1 = Purchase.objects.create(name='Purchase1', supplier=supplier1)
+        purchase1 = Purchase.objects.create(name='Purchase1', supplier=supplier1, status='closed')
         Delivery.objects.create(name='Delivery 1', purchase=purchase1)
         Delivery.objects.create(name='Delivery 2', purchase=purchase1)
         Delivery.objects.create(name='Delivery 3', purchase=purchase1)
         cls.create_data = [
             {
                 'name': 'Delivery 4',
                 'purchase': purchase1.pk,
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/delivery/test_views.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,18 +21,20 @@
         supplier2 = Supplier.objects.create(
             name='Supplier 2',
             slug='supplier2',
         )
         purchase1 = Purchase.objects.create(
             name='Purchase 1',
             supplier=supplier1,
+            status='closed',
         )
         purchase2 = Purchase.objects.create(
             name='Purchase 1',
             supplier=supplier2,
+            status='closed',
         )
         delivery1 = Delivery.objects.create(
             name='Delivery 1',
             purchase=purchase1,
         )
         delivery2 = Delivery.objects.create(
             name='Delivery 2',
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/purchase/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,33 +7,36 @@
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
         APIViewTestCases.UpdateObjectViewTestCase,
         APIViewTestCases.DeleteObjectViewTestCase):
     model = Purchase
-    brief_fields = ['date', 'display', 'id', 'name', 'supplier', 'url']
+    brief_fields = ['date', 'display', 'id', 'name', 'status', 'supplier', 'url']
 
     bulk_update_data = {
         'description': 'new description',
     }
 
     @classmethod
     def setUpTestData(cls) -> None:
         supplier1 = Supplier.objects.create(name='Supplier 1')
-        Purchase.objects.create(name='Purchase 1', supplier=supplier1)
-        Purchase.objects.create(name='Purchase 2', supplier=supplier1)
-        Purchase.objects.create(name='Purchase 3', supplier=supplier1)
+        Purchase.objects.create(name='Purchase 1', supplier=supplier1, status='closed')
+        Purchase.objects.create(name='Purchase 2', supplier=supplier1, status='closed')
+        Purchase.objects.create(name='Purchase 3', supplier=supplier1, status='closed')
         cls.create_data = [
             {
                 'name': 'Purchase 4',
                 'supplier': supplier1.pk,
+                'status': 'closed',
             },
             {
                 'name': 'Purchase 5',
                 'supplier': supplier1.pk,
+                'status': 'closed',
             },
             {
                 'name': 'Purchase 6',
                 'supplier': supplier1.pk,
+                'status': 'closed',
             },
         ]
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/purchase/test_views.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,38 +21,43 @@
         supplier2 = Supplier.objects.create(
             name='Supplier 2',
             slug='supplier2',
         )
         purchase1 = Purchase.objects.create(
             name='Purchase 1',
             supplier=supplier1,
+            status='closed',
         )
         purchase2 = Purchase.objects.create(
             name='Purchase 2',
             supplier=supplier1,
+            status='closed',
         )
         purchase3 = Purchase.objects.create(
             name='Purchase 3',
             supplier=supplier1,
+            status='closed',
         )
         cls.form_data = {
             'name': 'Purchase',
             'supplier': supplier1.pk,
             'description': 'Purchase description',
+            'status': 'open',
             'date': datetime.date(day=1, month=1, year=2023),
         }
         cls.csv_data = (
-            'name,supplier,date',
-            f'Purchase 4,{supplier1.name},2023-03-26',
-            f'Purchase 5,{supplier1.name},2023-03-26',
-            f'Purchase 6,{supplier1.name},2023-03-26',
+            'name,supplier,date,status',
+            f'Purchase 4,{supplier1.name},2023-03-26,open',
+            f'Purchase 5,{supplier1.name},2023-03-26,open',
+            f'Purchase 6,{supplier1.name},2023-03-26,open',
         )
         cls.csv_update_data = (
-            'id,description,supplier',
-            f'{purchase1.pk},description 1,{supplier2.name}',
-            f'{purchase2.pk},description 2,{supplier2.name}',
-            f'{purchase3.pk},description 3,{supplier2.name}',
+            'id,description,supplier,status',
+            f'{purchase1.pk},description 1,{supplier2.name},closed',
+            f'{purchase2.pk},description 2,{supplier2.name},closed',
+            f'{purchase3.pk},description 3,{supplier2.name},closed',
         )
         cls.bulk_edit_data = {
             'description': 'bulk description',
             'date': datetime.date(day=1, month=1, year=2022),
+            'status': 'partial',
         }
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/settings.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/supplier/test_api.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/tests/test_load.py` & `netbox_inventory-1.6.0/netbox_inventory/tests/test_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from django.urls import reverse
 from django.test import SimpleTestCase
 
 from netbox_inventory import __version__
 from netbox_inventory.tests.custom import APITestCase
 
 
-class NetboxDnsVersionTestCase(SimpleTestCase):
+class NetboxInventoryVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.5.2"
+        assert __version__ == "1.6.0"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory/urls.py` & `netbox_inventory-1.6.0/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/utils.py` & `netbox_inventory-1.6.0/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/asset.py` & `netbox_inventory-1.6.0/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/asset_assign.py` & `netbox_inventory-1.6.0/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/asset_create.py` & `netbox_inventory-1.6.0/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/asset_reassign.py` & `netbox_inventory-1.6.0/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/delivery.py` & `netbox_inventory-1.6.0/netbox_inventory/views/delivery.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/inventoryitem_group.py` & `netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/inventoryitem_type.py` & `netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/purchase.py` & `netbox_inventory-1.6.0/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/supplier.py` & `netbox_inventory-1.6.0/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory/views/tabs.py` & `netbox_inventory-1.6.0/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.5.2/netbox_inventory.egg-info/PKG-INFO` & `netbox_inventory-1.6.0/netbox_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.5.2
+Version: 1.6.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,23 +67,24 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.5.x to work. Older versions of the plugin
+This plugin requires netbox version 3.7.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
 |       3.5      | 1.3.x & 1.4.x  |
 |       3.6      |      1.5.x     |
+|       3.7      |      1.6.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.5.2/netbox_inventory.egg-info/SOURCES.txt` & `netbox_inventory-1.6.0/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 netbox_inventory/forms/assign.py
 netbox_inventory/forms/bulk.py
 netbox_inventory/forms/bulk_add.py
 netbox_inventory/forms/create.py
 netbox_inventory/forms/filters.py
 netbox_inventory/forms/models.py
 netbox_inventory/forms/reassign.py
+netbox_inventory/management/commands/check_asset_tags.py
 netbox_inventory/migrations/0001_initial_prod.py
 netbox_inventory/migrations/0002_alter_asset_serial.py
 netbox_inventory/migrations/0003_add_inventoryitemgroup.py
 netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
 netbox_inventory/migrations/0005_delivery_asset_delivery.py
+netbox_inventory/migrations/0006_purchase_status.py
 netbox_inventory/migrations/__init__.py
 netbox_inventory/templates/netbox_inventory/asset.html
 netbox_inventory/templates/netbox_inventory/asset_assign.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
 netbox_inventory/templates/netbox_inventory/asset_create.html
 netbox_inventory/templates/netbox_inventory/asset_edit.html
```

### Comparing `netbox-inventory-1.5.2/pyproject.toml` & `netbox_inventory-1.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

