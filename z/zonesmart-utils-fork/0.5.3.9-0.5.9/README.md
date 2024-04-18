# Comparing `tmp/zonesmart-utils-fork-0.5.3.9.tar.gz` & `tmp/zonesmart-utils-fork-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zonesmart-utils-fork-0.5.3.9.tar", last modified: Mon Jan 15 17:19:13 2024, max compression
+gzip compressed data, was "zonesmart-utils-fork-0.5.9.tar", last modified: Thu Apr 18 02:13:34 2024, max compression
```

## Comparing `zonesmart-utils-fork-0.5.3.9.tar` & `zonesmart-utils-fork-0.5.9.tar`

### file list

```diff
@@ -1,354 +1,360 @@
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.888841 zonesmart-utils-fork-0.5.3.9/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      204 2024-01-15 17:19:13.888841 zonesmart-utils-fork-0.5.3.9/PKG-INFO
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        9 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/README.md
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/pyproject.toml
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      209 2024-01-15 17:19:13.888841 zonesmart-utils-fork-0.5.3.9/setup.cfg
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      542 2024-01-15 17:19:11.000000 zonesmart-utils-fork-0.5.3.9/setup.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.852841 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      204 2024-01-15 17:19:13.000000 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/PKG-INFO
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    11046 2024-01-15 17:19:13.000000 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/SOURCES.txt
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        1 2024-01-15 17:19:13.000000 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/dependency_links.txt
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      388 2024-01-15 17:19:13.000000 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/requires.txt
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        9 2024-01-15 17:19:13.000000 zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/top_level.txt
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.856841 zonesmart-utils-fork-0.5.3.9/zs_utils/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.856841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.856841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2193 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.856841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      209 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      609 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1352 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/dropshipping.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      360 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/freight_template.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      995 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/logistics.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      162 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/merchant.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1071 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4000 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/product.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      223 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/service_template.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.856841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      503 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      112 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1098 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1038 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/chat.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1720 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2966 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/product.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2918 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/shipment.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5219 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/actions.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      124 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/apps.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3497 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/base_action.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      423 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/base_api.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/core.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/migrations/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1771 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/migrations/0001_initial.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/migrations/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1681 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/models.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4718 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/services.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      548 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      154 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      356 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/account.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1323 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/connection.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      354 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/label.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      354 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/lists.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1803 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      515 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/rate.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1511 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/status.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      120 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/apps.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    20998 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/base_action.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5542 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/base_api.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      980 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/constants.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       24 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       50 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3190 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/new_api.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2824 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/trading_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      118 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.860841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       71 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      701 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/catalog.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/identity.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2946 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/taxonomy.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      664 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/developer.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/post_order.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      126 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      113 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      275 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/base.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1858 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/payment_policy.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1828 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/return_policy.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)       88 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     4167 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3281 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1085 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3082 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/item.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1707 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/item_group.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      299 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/listing.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2284 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/location.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2644 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/offer.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1232 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/metadata.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      641 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/negotiation.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      260 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2952 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/best_offer.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2081 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/billing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1185 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      738 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/details.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      505 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/feedback.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      836 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/image.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      334 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/limits.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1823 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/listing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7317 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/messages.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5466 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/notifications.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      426 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/store.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.864841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      241 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      736 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/aspect_enums.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1389 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/common_enums.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2791 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/listing_enums.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1060 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/message_enums.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1571 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/notification_enums.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3189 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/order_enums.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1745 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/policy_enums.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5709 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      109 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      990 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1429 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2627 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      538 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     4809 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/sftp_get.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2153 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/sftp_put.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1535 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/model.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3163 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/oauth_client.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/utils/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       28 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/utils/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      873 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/utils/custom_quote.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1174 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.868841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      259 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       68 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1070 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/shop.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      795 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/shop_section.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      271 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/user.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      395 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/carrier.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      718 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/category.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       44 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2270 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/image.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/listing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1466 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/receipt.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2168 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2233 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile_destination.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1927 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile_upgrade.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      713 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/transaction.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      519 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       90 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1566 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/pickup.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      337 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/rate.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      692 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/shipment.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      256 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/tracking.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      724 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/filters.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      549 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       90 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      215 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      541 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      467 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/policy.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      555 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/product.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1672 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/constants.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7685 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/services.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/migrations/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4222 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/migrations/0001_initial.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/migrations/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2219 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/models.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.872841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1002 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      157 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      593 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/act.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      894 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1532 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/chat.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2832 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/listing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      238 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/report.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3197 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/shipment.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      301 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/warehouse.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      956 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/serializers.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3801 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/services.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      444 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       67 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      328 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/carrier.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      559 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/rate.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      938 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/shipment.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      734 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/account/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       44 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/account/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      527 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/account/location.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      364 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/account/shop.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       92 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1957 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/image.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      903 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/inventory.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2938 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/product.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1680 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/variant.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2918 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1872 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/shipment.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1410 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/webhook.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/utils/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       31 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/utils/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      683 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/utils/response_keeper.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      468 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/views.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      971 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.876841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       93 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1815 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3266 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/listing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4213 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1143 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/warehouse.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      813 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/base_api.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       64 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      340 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/listing.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4417 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/order.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3269 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/shop.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3054 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/base_action.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5654 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/constants.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       87 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3009 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_create.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      590 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_get.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2233 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_refund.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7230 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/services.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2436 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/views.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      662 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/captcha.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     8147 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/compare_data.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3615 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/currency_converter.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/data/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/__init__.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      137 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)    14709 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/country.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)    14881 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/currency.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      739 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/files.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7295 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/language.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      839 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/unit.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1682 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/usa_state.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3070 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/dict_converter.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6562 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/exceptions.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1398 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/file_io.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      729 2023-12-20 10:54:45.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/file_utils.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      866 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/function_timeout.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      732 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/get_file_extension.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      331 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/html_utils.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2802 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/import_utils.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1889 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/inspect_func.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4053 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/json_utils.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      652 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/permissions.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      968 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/s3_storage_backend.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.880841 zonesmart-utils-fork-0.5.3.9/zs_utils/support/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1285 2024-01-15 14:15:06.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      198 2024-01-09 16:21:55.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/apps.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1143 2024-01-15 14:25:16.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/constants.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5369 2024-01-15 17:18:23.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/models.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2367 2024-01-15 13:38:54.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/serializers.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     9677 2024-01-15 12:23:47.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/services.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      120 2023-12-05 19:50:01.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/signals.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6616 2024-01-15 13:45:52.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/support/views.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2401 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/time_utils.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2285 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/transliterate.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)       47 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/__init__.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1531 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/converter.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3855 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/data.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      615 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/exceptions.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1984 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/parser.py
--rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     6952 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/units.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/user/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/user/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/user/apps.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/user/migrations/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/user/migrations/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2469 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/user/models.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      626 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/user/utils.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/views/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       42 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/views/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6117 2024-01-09 07:43:55.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/views/core.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7394 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/views/mixins.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7453 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/consumer.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1919 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/middleware.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2419 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/services.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      667 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/tasks.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4325 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/xml_parser.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.884841 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       65 2024-01-09 07:43:55.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      277 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/exceptions.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.888841 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1064 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4895 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/abstract.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2101 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/age.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      982 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/category.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1583 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/condition.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2214 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/currency.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1352 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/dimensions.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1229 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/feed.py
-drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-01-15 17:19:13.888841 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      103 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/__init__.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1318 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      600 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/options.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      251 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/outlets.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      310 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/year.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1427 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/gift.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    30099 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/offers.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1084 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/option.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1051 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/outlet.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1231 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/parameter.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1592 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/price.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5740 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/promo.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     8300 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/shop.py
--rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1321 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/yml.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      202 2024-04-18 02:13:34.843135 zonesmart-utils-fork-0.5.9/PKG-INFO
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        9 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/README.md
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/pyproject.toml
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      209 2024-04-18 02:13:34.843135 zonesmart-utils-fork-0.5.9/setup.cfg
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      540 2024-04-18 02:06:47.000000 zonesmart-utils-fork-0.5.9/setup.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.807134 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      202 2024-04-18 02:13:34.000000 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    11222 2024-04-18 02:13:34.000000 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        1 2024-04-18 02:13:34.000000 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      413 2024-04-18 02:13:34.000000 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/requires.txt
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        9 2024-04-18 02:13:34.000000 zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/top_level.txt
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.807134 zonesmart-utils-fork-0.5.9/zs_utils/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.811134 zonesmart-utils-fork-0.5.9/zs_utils/api/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.811134 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2193 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.811134 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      209 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      609 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1352 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/dropshipping.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      360 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/freight_template.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      995 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/logistics.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      162 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/merchant.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1071 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4000 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/product.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      223 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/service_template.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.811134 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      503 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.811134 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      112 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1098 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1038 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/chat.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1720 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2966 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/product.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2918 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/shipment.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5219 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/actions.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      124 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/apps.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3497 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/base_action.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      423 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/base_api.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/core.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/migrations/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1771 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/migrations/0001_initial.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/migrations/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1681 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/models.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4718 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/services.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      548 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      154 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      356 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/account.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1323 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/connection.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      354 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/label.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      354 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/lists.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1803 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      515 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/rate.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1511 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/status.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      120 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/apps.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    21005 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/base_action.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5542 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/base_api.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      980 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/constants.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       24 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       50 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3190 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/new_api.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2824 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/trading_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      118 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       71 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      701 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/catalog.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/identity.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2946 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/taxonomy.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      664 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/developer.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1368 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/post_order.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      126 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.815135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      113 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      275 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/base.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1858 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/payment_policy.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1828 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/return_policy.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.819135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)       88 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     4167 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3281 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1085 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.819135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3082 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/item.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1707 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/item_group.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      299 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/listing.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2284 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/location.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2644 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/offer.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1232 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/metadata.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      641 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/negotiation.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.819135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      260 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2952 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/best_offer.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2081 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/billing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1185 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      738 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/details.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      505 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/feedback.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      836 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/image.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      334 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/limits.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1823 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/listing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7317 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/messages.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5466 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/notifications.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      426 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/store.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.819135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.819135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      241 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      736 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/aspect_enums.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1389 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/common_enums.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2791 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/listing_enums.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1060 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/message_enums.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1571 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/notification_enums.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3189 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/order_enums.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1745 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/policy_enums.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5709 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      109 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      990 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1429 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2627 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      538 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     4809 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/sftp_get.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     2153 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/sftp_put.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1535 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/model.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3163 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/oauth_client.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/utils/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       28 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/utils/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      873 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/utils/custom_quote.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1174 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      259 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       68 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1070 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/shop.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      795 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/shop_section.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      271 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/user.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      395 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/carrier.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      718 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/category.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       44 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2270 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/image.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7978 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/listing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1466 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/receipt.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2168 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2233 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile_destination.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1927 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile_upgrade.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      713 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/transaction.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.823135 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      519 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       90 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1566 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/pickup.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      337 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/rate.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      692 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/shipment.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      256 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/tracking.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      724 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/filters.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      549 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       90 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      215 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      541 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      467 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/policy.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      555 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/product.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1589 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/constants.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7658 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/services.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/migrations/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4222 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/migrations/0001_initial.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/migrations/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2219 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/models.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1002 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      157 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      593 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/act.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      954 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1532 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/chat.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2832 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/listing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      238 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/report.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3197 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/shipment.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      301 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/warehouse.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      956 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/serializers.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3801 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/services.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      444 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       67 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      328 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/carrier.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      559 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/rate.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      938 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/shipment.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.827134 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      734 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/account/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       44 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/account/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      527 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/account/location.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      364 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/account/shop.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       92 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1957 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/image.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      903 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/inventory.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2938 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/product.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1680 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/variant.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2918 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1872 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/shipment.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1410 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/webhook.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/utils/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       31 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/utils/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      683 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/utils/response_keeper.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      468 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/views.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      971 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      114 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1540 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2605 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/listing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4213 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      762 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/price.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1143 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/warehouse.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      813 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/base_api.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       64 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      340 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/listing.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4417 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/order.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3269 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/shop.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.831135 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3054 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/base_action.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5654 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/constants.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       87 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3009 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_create.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      590 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_get.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2233 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_refund.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7230 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/services.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2436 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/views.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      662 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/captcha.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     8147 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/compare_data.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3615 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/currency_converter.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/data/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/__init__.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      137 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)    14709 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/country.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)    14881 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/currency.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      739 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/files.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7295 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/language.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      839 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/unit.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1682 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/data/enums/usa_state.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     3070 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/dict_converter.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6666 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/exceptions.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1398 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/file_io.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      729 2024-04-17 02:16:33.000000 zonesmart-utils-fork-0.5.9/zs_utils/file_utils.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      866 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/function_timeout.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      732 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/get_file_extension.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      331 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/html_utils.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2802 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/import_utils.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1889 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/inspect_func.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4053 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/json_utils.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1047 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/permissions.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      968 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/s3_storage_backend.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/support/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-17 02:16:33.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      198 2024-04-17 02:16:33.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/apps.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1951 2024-04-17 23:11:35.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/constants.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1999 2024-04-18 02:01:18.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/filters.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/support/migrations/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6680 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/migrations/0001_initial.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/migrations/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4882 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/models.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2040 2024-04-17 02:16:33.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/serializers.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     8737 2024-04-17 02:22:29.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/services.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      120 2024-04-17 02:16:33.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/signals.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      558 2024-04-17 02:20:32.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/urls.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4933 2024-04-18 02:01:18.000000 zonesmart-utils-fork-0.5.9/zs_utils/support/views.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2401 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/time_utils.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2285 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/transliterate.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)       47 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/__init__.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1531 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/converter.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     3855 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/data.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)      615 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/exceptions.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     1984 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/parser.py
+-rwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)     6952 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/units.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.835135 zonesmart-utils-fork-0.5.9/zs_utils/user/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/user/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      114 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/user/apps.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/user/migrations/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/user/migrations/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2469 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/user/models.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      626 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/user/utils.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/views/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       42 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/views/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     6117 2024-01-09 07:43:55.000000 zonesmart-utils-fork-0.5.9/zs_utils/views/core.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7394 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/views/mixins.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/websocket/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)        0 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/websocket/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     7453 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/websocket/consumer.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1919 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/websocket/middleware.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2419 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/websocket/services.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      667 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/websocket/tasks.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4325 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/xml_parser.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)       65 2024-01-09 07:43:55.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      277 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/exceptions.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1064 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     4895 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/abstract.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2101 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/age.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      982 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/category.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1583 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/condition.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     2214 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/currency.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1352 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/dimensions.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1229 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/feed.py
+drwxrwxr-x   0 hashbrown  (1000) hashbrown  (1000)        0 2024-04-18 02:13:34.839135 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      103 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/__init__.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1318 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      600 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/options.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      251 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/outlets.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)      310 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/year.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1427 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/gift.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)    30099 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/offers.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1084 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/option.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1051 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/outlet.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1231 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/parameter.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1592 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/price.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     5740 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/promo.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     8300 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/shop.py
+-rw-rw-r--   0 hashbrown  (1000) hashbrown  (1000)     1321 2023-12-05 19:50:25.000000 zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/yml.py
```

### Comparing `zonesmart-utils-fork-0.5.3.9/setup.py` & `zonesmart-utils-fork-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
             if line:
                 reqs.append(line)
     return reqs
 
 
 setup(
     name="zonesmart-utils-fork",
-    version="0.5.3.9",
+    version="0.5.9",
     author="Zonesmart",
     author_email="e.beliakov@dev.kokoc.com",
     packages=find_packages(include=["zs_utils", "zs_utils.*"]),
     install_requires=parse_requirements(),
 )
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zonesmart_utils_fork.egg-info/SOURCES.txt` & `zonesmart-utils-fork-0.5.9/zonesmart_utils_fork.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 zs_utils/api/utils/response_keeper.py
 zs_utils/api/wildberries/__init__.py
 zs_utils/api/wildberries/base_api.py
 zs_utils/api/wildberries/core/__init__.py
 zs_utils/api/wildberries/core/category.py
 zs_utils/api/wildberries/core/listing.py
 zs_utils/api/wildberries/core/order.py
+zs_utils/api/wildberries/core/price.py
 zs_utils/api/wildberries/core/warehouse.py
 zs_utils/api/yandex_market/__init__.py
 zs_utils/api/yandex_market/base_api.py
 zs_utils/api/yandex_market/core/__init__.py
 zs_utils/api/yandex_market/core/listing.py
 zs_utils/api/yandex_market/core/order.py
 zs_utils/api/yandex_market/core/shop.py
@@ -236,19 +237,23 @@
 zs_utils/data/enums/files.py
 zs_utils/data/enums/language.py
 zs_utils/data/enums/unit.py
 zs_utils/data/enums/usa_state.py
 zs_utils/support/__init__.py
 zs_utils/support/apps.py
 zs_utils/support/constants.py
+zs_utils/support/filters.py
 zs_utils/support/models.py
 zs_utils/support/serializers.py
 zs_utils/support/services.py
 zs_utils/support/signals.py
+zs_utils/support/urls.py
 zs_utils/support/views.py
+zs_utils/support/migrations/0001_initial.py
+zs_utils/support/migrations/__init__.py
 zs_utils/unit_converter/__init__.py
 zs_utils/unit_converter/converter.py
 zs_utils/unit_converter/data.py
 zs_utils/unit_converter/exceptions.py
 zs_utils/unit_converter/parser.py
 zs_utils/unit_converter/units.py
 zs_utils/user/__init__.py
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/dropshipping.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/dropshipping.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/logistics.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/logistics.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress/core/product.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/chat.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/chat.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/product.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/aliexpress_russia/core/shipment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/aliexpress_russia/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/actions.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/actions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/base_action.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/base_action.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/core.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/core.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/migrations/0001_initial.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/models.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/amocrm/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/amocrm/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/connection.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/connection.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/rate.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/rate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/apiship/core/status.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/apiship/core/status.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/base_action.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/base_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
         if self.instance:
             self.instance.incr_request_counter()
 
     def response_is_success(
         self,
         results: dict,
         response: requests.Response,
-        exception: CustomException = None,
+        exception: CustomException | None = None,
     ) -> bool:
         """
         Проверка, что запрос успешный
         """
         if exception is not None:
             return False
         if response is not None:
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/constants.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/constants.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/new_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/new_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/base_api/trading_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/base_api/trading_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/catalog.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/catalog.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/commerce/taxonomy.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/commerce/taxonomy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/developer.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/developer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/post_order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/post_order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/payment_policy.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/payment_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/account/return_policy.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/account/return_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/item.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/item.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/item_group.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/item_group.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/location.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/location.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/inventory/offer.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/inventory/offer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/metadata.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/metadata.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/sell/negotiation.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/sell/negotiation.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/best_offer.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/best_offer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/billing.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/billing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/details.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/details.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/image.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/listing.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/listing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/messages.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/messages.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/core/trading/notifications.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/core/trading/notifications.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/aspect_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/aspect_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/common_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/common_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/listing_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/listing_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/message_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/message_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/notification_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/notification_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/order_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/order_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/policy_enums.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/policy_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/sftp_get.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/sftp_get.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/mip/sftp_put.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/mip/sftp_put.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/model.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/model.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/oauth/oauth_client.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/oauth/oauth_client.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ebay/utils/custom_quote.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ebay/utils/custom_quote.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/shop.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/account/shop_section.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/account/shop_section.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/image.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/listing/listing.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/listing/listing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/receipt.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/receipt.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile_destination.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile_destination.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/shipping_profile_upgrade.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/shipping_profile_upgrade.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/etsy/core/transaction.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/etsy/core/transaction.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/pickup.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/pickup.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/fedex/core/shipment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/fedex/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/filters.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/filters.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/insales/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/insales/core/product.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/insales/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/constants.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from model_utils import Choices
 
 
-CRM_CATEGORIES = Choices(
-    ("22", "LANDING", "New отдел продаж"),
-)
-
 CRM_LANDING_STAGES = Choices(
     ("C22:UC_GR0G8F", "NEW", "Обработка"),
     ("C22:UC_44PJ08", "IDENTIFY_NEEDS", "Выявление потребностей"),
     ("C22:NEW", "BRIEFING", "Брифинг"),
     ("C22:PREPARATION", "PREPARING", "Подготовка стратегии / КП"),
     ("C22:PREPAYMENT_INVOIC", "PRESENTED", "Стратегия / КП - отправлено (презентовано)"),
     ("C22:EXECUTING", "NEGOTIATION", "Переговоры по КП"),
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/kokoc_crm/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/kokoc_crm/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,14 @@
         parsed_url = urlparse(url=url)
         return {k: v for k, v in parse_qsl(qs=parsed_url.query) if k.startswith("utm_")}
 
     @classmethod
     def create_deal(
         cls,
         title: str,
-        category: str,
         stage: str,
         contact_id: int = None,
         comment: str = None,
         source: str = None,
         assigned_by: str = "2806",
         department: str = "9923",
         utm_params: dict = None,
@@ -158,15 +157,15 @@
                 ]
             }
         else:
             utm_params = {}
         params = {
             "fields": {
                 "TITLE": title,
-                "CATEGORY_ID": category,
+                "CATEGORY_ID": "22",
                 "STAGE_ID": stage,
                 "CONTACT_ID": contact_id,
                 "COMMENTS": comment,
                 "UF_CRM_DEAL_AMO_OKDUOUUHNSIOPEJZ": source,
                 "ASSIGNED_BY_ID": assigned_by,
                 "UF_DEPARTMENT": department,
                 **utm_params,
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/migrations/0001_initial.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/models.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/act.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/act.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/chat.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/chat.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/listing.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/listing.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 
     resource_method = "v1/product/import/info"
     required_params = ["task_id"]
 
 
 class OzonCreateProductAPI(OzonAPI):
     """
-    Docs: https://docs.ozon.ru/api/seller/#operation/ProductAPI_ImportProductsV2
+    Docs: https://docs.ozon.ru/api/seller/#operation/ProductAPI_ImportProductsV3
     """
 
-    resource_method = "v2/product/import"
+    resource_method = "v3/product/import"
     required_params = ["items"]
 
 
 class OzonUpdateProductStocksAPI(OzonAPI):
     resource_method = "v1/product/import/stocks"
     required_params = ["stocks"]
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/ozon/core/shipment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/ozon/core/shipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 class OzonCreateFBSShipmentAPI(OzonAPI):
     """
     Docs: https://docs.ozon.ru/api/seller/#operation/PostingAPI_ShipFbsPostingV3
     """
 
-    resource_method = "v3/posting/fbs/ship"
+    resource_method = "v4/posting/fbs/ship"
     required_params = [
         "packages",
         "posting_number",
     ]
     allowed_params = ["with"]
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/serializers.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/rate.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/rate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shipstation/core/shipment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shipstation/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/account/location.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/account/location.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/image.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/inventory.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/inventory.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/product.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/listing/variant.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/listing/variant.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/shipment.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/shopify/core/webhook.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/shopify/core/webhook.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/utils/response_keeper.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/utils/response_keeper.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/category.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 from zs_utils.api.wildberries.base_api import WildberriesAPI
 
 
 class GetWildberriesCategoryList(WildberriesAPI):
     """
-    Docs: https://openapi.wildberries.ru/#tag/Kontent-Konfigurator/paths/~1content~1v1~1object~1all/get
+    Docs: https://openapi.wb.ru/content/api/ru/#tag/Konfigurator/paths/~1content~1v2~1object~1all/get
     """
 
     http_method = "GET"
-    resource_method = "content/v1/object/all"
-    allowed_params = ["name", "top"]
+    resource_method = "content/v2/object/all"
+    allowed_params = ["name", "limit", "offset", "parentID"]
 
 
 class GetWildberriesCategoryParentList(WildberriesAPI):
     """
-    Docs: https://openapi.wildberries.ru/#tag/Kontent-Konfigurator/paths/~1content~1v1~1object~1parent~1all/get
+    Docs: https://openapi.wb.ru/content/api/ru/#tag/Konfigurator/paths/~1content~1v2~1object~1parent~1all/get
     """
 
     http_method = "GET"
-    resource_method = "content/v1/object/parent/all"
+    resource_method = "content/v2/object/parent/all"
 
 
 class GetWildberriesCategoryAttributes(WildberriesAPI):
     """
-    Docs: https://openapi.wildberries.ru/#tag/Kontent-Konfigurator/paths/~1content~1v1~1object~1characteristics~1%7BobjectName%7D/get
+    Docs: https://openapi.wb.ru/content/api/ru/#tag/Konfigurator/paths/~1content~1v2~1object~1charcs~1%7BsubjectId%7D/get
     """
 
     http_method = "GET"
-    resource_method = "content/v1/object/characteristics/{objectName}"
-    required_params = ["objectName"]
+    resource_method = "content/v2/object/charcs/{subjectId}"
+    required_params = ["subjectId"]
 
 
 class GetWildberriesAttributeValues(WildberriesAPI):
     """
     Docs: https://openapi.wildberries.ru/#tag/Kontent-Konfigurator/paths/~1content~1v1~1directory~1colors/get
     Значения dictionary_name:
     - colors (Цвет)
     - kinds (Пол)
     - countries (Страна производства)
-    - collections (Коллекции)
     - seasons (Сезон)
-    - contents (Комплектация)
-    - consists (Состав)
-    - brands (Бренд)
     - tnved (ТНВЭД)
     """
 
     http_method = "GET"
-    resource_method = "content/v1/directory/{dictionary_name}"
+    resource_method = "content/v2/directory/{dictionary_name}"
     required_params = []
     allowed_params = [
-        "top",  # кроме colors, kinds, countries, seasons
-        "pattern",  # кроме colors, kinds, countries, seasons
-        "objectName",  # только tnved
-        "tnvedsLike",  # только tnved
+        "search",  # только tnved
+        "subjectID",  # только tnved
     ]
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/wildberries/core/warehouse.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/wildberries/core/warehouse.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/base_api.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/order.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yandex_market/core/shop.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yandex_market/core/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/base_action.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/base_action.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/constants.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/constants.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_create.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_create.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_get.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_get.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/core/payment_refund.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/core/payment_refund.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/api/yookassa/views.py` & `zonesmart-utils-fork-0.5.9/zs_utils/api/yookassa/views.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/captcha.py` & `zonesmart-utils-fork-0.5.9/zs_utils/captcha.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/compare_data.py` & `zonesmart-utils-fork-0.5.9/zs_utils/compare_data.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/currency_converter.py` & `zonesmart-utils-fork-0.5.9/zs_utils/currency_converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/country.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/country.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/currency.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/files.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/files.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/language.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/language.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/unit.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/unit.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/data/enums/usa_state.py` & `zonesmart-utils-fork-0.5.9/zs_utils/data/enums/usa_state.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/dict_converter.py` & `zonesmart-utils-fork-0.5.9/zs_utils/dict_converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/exceptions.py` & `zonesmart-utils-fork-0.5.9/zs_utils/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             message += str(self.message)
         elif self.messages:
             message += "; ".join(self.messages)
 
         if self.message_dict:
             message += "\n" + pretty_json(data=self.message_dict)
 
+        if (not message) and (self.response_code):
+            message = f"Code: {self.response_code}"
+
         return message
 
     def __repr__(self) -> str:
         val = ""
         if self.messages:
             val = f"messages={self.messages}"
         elif self.message:
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/file_io.py` & `zonesmart-utils-fork-0.5.9/zs_utils/file_io.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/file_utils.py` & `zonesmart-utils-fork-0.5.9/zs_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/function_timeout.py` & `zonesmart-utils-fork-0.5.9/zs_utils/function_timeout.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/get_file_extension.py` & `zonesmart-utils-fork-0.5.9/zs_utils/get_file_extension.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/import_utils.py` & `zonesmart-utils-fork-0.5.9/zs_utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/inspect_func.py` & `zonesmart-utils-fork-0.5.9/zs_utils/inspect_func.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/json_utils.py` & `zonesmart-utils-fork-0.5.9/zs_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/permissions.py` & `zonesmart-utils-fork-0.5.9/zs_utils/permissions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from rest_framework.request import Request
 from rest_framework.permissions import BasePermission, AllowAny
 
 from django.contrib.auth.models import AnonymousUser
 
 
 __all__ = [
-    "UserHasAccess",
+    "UserHasAccess", "StaffPermission"
 ]
 
 
 class UserHasAccess(BasePermission):
     def user_has_access(self, user) -> bool:
         return True
 
@@ -17,7 +17,19 @@
         if getattr(view, "ignore_has_access", False) or (AllowAny in view.permission_classes):
             return True
         return (
             bool(request.user)
             and (not isinstance(request.user, AnonymousUser))
             and self.user_has_access(user=request.user)
         )
+
+
+class StaffPermission(BasePermission):
+    """
+    Права для сотрудников.
+    """
+
+    def has_permission(self, request: Request, view) -> bool:
+        return request.user and getattr(request.user, "is_staff", False)
+
+    def has_object_permission(self, request: Request, view, obj) -> bool:
+        return self.has_permission(request=request, view=view)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/s3_storage_backend.py` & `zonesmart-utils-fork-0.5.9/zs_utils/s3_storage_backend.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/support/constants.py` & `zonesmart-utils-fork-0.5.9/zs_utils/support/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from model_utils import Choices
 
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 
 
-SUPPORT_TICKET_QUESTION_TYPES = getattr(settings, "SUPPORT_TICKET_QUESTION_TYPES")
-SUPPORT_TICKET_DEFAULT_QUESTION_TYPE = getattr(settings, "SUPPORT_TICKET_DEFAULT_QUESTION_TYPE")
+SUPPORT_TICKET_QUESTION_TYPES = getattr(
+    settings,
+    "SUPPORT_TICKET_QUESTION_TYPES",
+    Choices(
+        ("BASIC", _("Общий вопрос")),
+        ("INTERFACE", _("Интерфейс")),
+        ("TECHNICAL", _("Технический")),
+        ("BILLING", _("Счет")),
+    )
+)
 
 SUPPORT_TICKET_STATUSES = Choices(
     ("PENDING", _("Ожидает рассмотрения")),
     ("OPEN", _("Открыто")),
     ("CLOSED_BY_USER", _("Закрыто пользователем")),
     ("CLOSED_BY_MANAGER", _("Закрыто менеджером")),
     ("CLOSED_AUTO", _("Закрыто из-за отсутствия активности")),
@@ -21,9 +29,20 @@
 
 SUPPORT_TICKET_CLIENT_STATUSES = Choices(
     ("PENDING", _("В работе")),
     ("RESPONDED", _("Получен ответ")),
     ("CLOSED", _("Закрыто")),
 )
 
+SUPPORT_TICKET_MESSAGES = Choices(
+    ("OPEN", _("Заявка взята в обработку оператором.")),
+    ("CLOSED_AUTO", _("Заявка автоматически закрыта после длительного отсутствия активности.")),
+    ("CLOSED_BY_USER", _("Заявка закрыта пользователем.")),
+    ("CLOSED_BY_MANAGER", _("Заявка закрыта оператором.")),
+    ("REOPEN", _("Заявка повторно открыта.")),
+)
+
+SUPPORT_TICKET_MESSAGE_SIGNATURE = getattr(settings, "SUPPORT_TICKET_MESSAGE_SIGNATURE", "")
+
 MAX_OPEN_TICKET = getattr(settings, "MAX_OPEN_TICKET", 10)
 MAX_TEXT_LENGTH = getattr(settings, "MAX_TEXT_LENGTH", 1500)
+AUTO_CLOSE_TICKET_AFTER = getattr(settings, "AUTO_CLOSE_TICKET_AFTER", 2)
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/support/models.py` & `zonesmart-utils-fork-0.5.9/zs_utils/support/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,40 +3,35 @@
 from django.contrib.auth import get_user_model
 
 from zs_utils.file_utils import get_support_file_upload_path
 from zs_utils.support import constants
 
 
 __all__ = [
-    "BaseSupportTicket",
-    "BaseSupportTicketMessage",
-    "BaseSupportTicketMessageFile",
+    "SupportTicket",
+    "SupportTicketMessage",
+    "SupportTicketMessageFile",
 ]
 
 User = get_user_model()
 
 
-class BaseSupportTicket(TimeStampedModel, UUIDModel):
+class SupportTicket(TimeStampedModel, UUIDModel):
     """
     Данные тикета (запросов в поддержку)
     """
     number = models.TextField(verbose_name="Номер обращения")
     subject = models.CharField(max_length=300, verbose_name="Тема")
     status = models.TextField(choices=constants.SUPPORT_TICKET_STATUSES, verbose_name="Статус")
-    question_type = models.TextField(
-        verbose_name="Тип вопроса",
-        choices=constants.SUPPORT_TICKET_QUESTION_TYPES,
-        default=constants.SUPPORT_TICKET_DEFAULT_QUESTION_TYPE,
-    )
+    question_type = models.TextField(verbose_name="Тип вопроса")
     user = models.ForeignKey(User, on_delete=models.CASCADE, related_name="tickets", verbose_name="Создатель")
     manager = models.ForeignKey(User, blank=True, null=True, on_delete=models.SET_NULL, verbose_name="Менеджер")
 
     class Meta:
         ordering = ["-created"]
-        app_label = "support"
 
     @property
     def client_status(self) -> constants.SUPPORT_TICKET_CLIENT_STATUSES:
         if self.status in constants.SUPPORT_TICKET_ACTIVE_STATUSES:
             if self.manager:
                 last_message = self.last_message
                 if last_message and (last_message.sender == self.manager):
@@ -66,36 +61,24 @@
     @property
     def last_message(self):
         """
         Последнее сообщение в данном обращении
         """
         return self.messages.filter(is_system=False).order_by("-created").first()
 
-    @property
-    def all_users(self) -> set:
-        """
-        Получение всех пользователей, которые участвуют в обращении
-        """
-        res = set(self.messages.values_list("sender", flat=True))
-        if self.user_id not in res:
-            res.append(self.user_id)
-        if self.manager_id and (self.manager_id not in res):
-            res.append(self.manager_id)
-        return res
-
 
-class BaseSupportTicketMessage(TimeStampedModel, UUIDModel):
+class SupportTicketMessage(TimeStampedModel, UUIDModel):
     """
     Данные сообщения тикета
     """
     text = models.TextField(max_length=constants.MAX_TEXT_LENGTH, null=True, verbose_name="Сообщение")
     is_system = models.BooleanField(verbose_name="Системное сообщение")
     is_viewed = models.BooleanField(default=False, verbose_name="Просмотрено получателем")
     ticket = models.ForeignKey(
-        "BaseSupportTicket",
+        "SupportTicket",
         on_delete=models.CASCADE,
         related_name="messages",
         related_query_name="message",
         verbose_name="Тикет",
     )
     sender = models.ForeignKey(
         to=User,
@@ -103,22 +86,21 @@
         null=True,
         on_delete=models.SET_NULL,
         verbose_name="Автор сообщения",
     )
 
     class Meta:
         ordering = ["-created"]
-        app_label = "support"
 
     @property
     def is_from_manager(self) -> bool:
         """
         Сообщение от менеджера
         """
-        return self.sender.is_staff
+        return self.ticket.manager and (self.sender == self.ticket.manager)
 
     @property
     def is_from_client(self) -> bool:
         """
         Сообщение от пользователя
         """
         return self.sender == self.ticket.user
@@ -130,31 +112,36 @@
         """
         if self.sender == self.ticket.user:
             return self.ticket.manager
         else:
             return self.ticket.user
 
 
-class BaseSupportTicketMessageFile(UUIDModel):
+class SupportTicketMessageFile(UUIDModel):
     """
     Данные прикреплённого файла к сообщению тикета
     """
     file = models.FileField(upload_to=get_support_file_upload_path, verbose_name="Приложенный файл")
     ticket_message = models.ForeignKey(
-        "BaseSupportTicketMessage",
+        "SupportTicketMessage",
         on_delete=models.CASCADE,
         related_name="files",
         related_query_name="file",
         verbose_name="Сообщение",
         null=True,
         blank=True,
     )
-
-    class Meta:
-        app_label = "support"
+    user = models.ForeignKey(
+        User,
+        on_delete=models.CASCADE,
+        related_name="+",
+        verbose_name="Пользователь",
+        null=True,
+        blank=True,
+    )
 
     @property
     def is_used(self) -> bool:
         if not self.ticket_message:
             raise NotImplemented
         return bool(self.ticket_message_id)
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/support/serializers.py` & `zonesmart-utils-fork-0.5.9/zs_utils/support/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 
+from zs_utils.support import models
+
 
 __all__ = [
     "CommonSupportTicketSerializer",
     "CommonCreateSupportTicketSerializer",
     "CommonSupportTicketMessageSerializer",
     "CommonCreateSupportTicketMessageSerializer",
     "CommonSupportTicketMessageFileSerializer",
@@ -12,14 +14,15 @@
 
 
 class CommonSupportTicketSerializer(serializers.ModelSerializer):
     user = None
     manager = None
 
     class Meta:
+        model = models.SupportTicket
         fields = [
             "id",
             "number",
             "created",
             "user",
             "manager",
             "status",
@@ -27,25 +30,27 @@
             "subject",
             "unread_messages",
         ]
 
 
 class CommonCreateSupportTicketSerializer(serializers.ModelSerializer):
     class Meta:
+        model = models.SupportTicket
         fields = [
             "question_type",
             "subject",
         ]
 
 
 class CommonSupportTicketMessageSerializer(serializers.ModelSerializer):
     sender = None
     files = None
 
     class Meta:
+        model = models.SupportTicketMessage
         fields = [
             "id",
             "created",
             "ticket",
             "sender",
             "text",
             "files",
@@ -54,37 +59,24 @@
         ]
 
 
 class CommonCreateSupportTicketMessageSerializer(serializers.Serializer):
     text = serializers.CharField(required=False, allow_null=True)
     files = None
 
-    @staticmethod
-    def get_signature():
-        return ""
-
-    @classmethod
-    def get_support_ticket(cls):
-        raise NotImplementedError("В сериализаторе должен быть определён метод получения модели SupportTicket")
-
     def to_internal_value(self, data):
-        signature = self.get_signature()
-        if signature:
-            user = self.get_support_ticket().objects.get(id=data["ticket"]).user.id
-            if data.get("text") and (data["sender"] != user):
-                data["text"] += signature
-
         data = super().to_internal_value(data)
 
         if not (data.get("text") or data.get("files")):
             raise ValidationError({"text": "Обязательное поле, если не задано поле 'files'."})
 
         return data
 
 
 class CommonSupportTicketMessageFileSerializer(serializers.ModelSerializer):
     class Meta:
+        model = models.SupportTicketMessageFile
         fields = [
             "id",
             "ticket_message",
             "file",
         ]
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/support/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/support/services.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from django.utils import timezone
-from django.utils.translation import gettext as _
-from django.conf import settings
 from django.db import transaction
 
 
 from zs_utils.exceptions import CustomException
 from zs_utils.support import constants, models, signals
 
 
@@ -16,36 +14,24 @@
 
 class SupportTicketServiceException(CustomException):
     pass
 
 
 class CommonSupportTicketService:
     """
-    Сервис для работы с тикетами (AbstractSupportTicket)
+    Сервис для работы с тикетами (SupportTicket)
     """
     @classmethod
-    def get_support_ticket(cls):
-        raise NotImplementedError("В сервисе должен быть определён метод получения модели SupportTicket")
-
-    @classmethod
-    def get_support_ticket_message(cls):
-        raise NotImplementedError("В сервисе должен быть определён метод получения модели SupportTicketMessage")
-
-    @classmethod
-    def get_support_ticket_message_file(cls):
-        raise NotImplementedError("В сервисе должен быть определён метод получения модели SupportTicketMessageFile")
-
-    @classmethod
     def max_active_tickets_opened(cls, user) -> bool:
         """
         Проверка, что было открыто максимальное кол-во тикетов для пользователя user
         """
         return (
             constants.MAX_OPEN_TICKET
-            <= cls.get_support_ticket().objects.filter(
+            <= models.SupportTicket.objects.filter(
                 user=user, status__in=constants.SUPPORT_TICKET_ACTIVE_STATUSES_LIST
             ).count()
         )
 
     @classmethod
     def check_user_can_open_new_ticket(cls, user) -> None:
         """
@@ -66,99 +52,98 @@
 
     @classmethod
     def create_ticket(
         cls,
         user,
         question_type: constants.SUPPORT_TICKET_QUESTION_TYPES,
         subject: str,
-    ) -> models.AbstractSupportTicket:
+    ) -> models.SupportTicket:
         cls.check_user_can_open_new_ticket(user=user)
 
-        return cls.get_support_ticket().objects.create(
+        return models.SupportTicket.objects.create(
             user=user,
             status=constants.SUPPORT_TICKET_STATUSES.PENDING,
             number=cls._generate_ticket_number(user=user),
             question_type=question_type,
             subject=subject,
         )
 
     @classmethod
     def create_ticket_message(
         cls,
-        ticket: models.AbstractSupportTicket,
+        ticket: models.SupportTicket,
         sender,
         is_system: bool,
         text: str = None,
-        files: list[models.AbstractSupportTicketMessageFile] = None,
-        **kwargs,
-    ) -> models.AbstractSupportTicketMessage:
+        files: list[models.SupportTicketMessageFile] = None,
+    ) -> models.SupportTicketMessage:
+        """
+        Создание сообщения тикета и вложений
+        """
         assert text or files, "Необходимо задать текст или файлы"
         if is_system:
             assert text and (not files), "Системное сообщение может быть только текстовым"
             assert not sender, "У системного сообщения не может быть отправителя"
         else:
             assert sender, "У пользовательского сообщения должен быть отправитель"
 
             if not ticket.is_active:
                 raise SupportTicketServiceException(message="Заявка закрыта.")
             if sender not in [ticket.user, ticket.manager]:
                 raise SupportTicketServiceException(message="Нельзя написать сообщение в чужую заявку.")
 
+        signature = constants.SUPPORT_TICKET_MESSAGE_SIGNATURE
+        if signature and text and (sender == ticket.manager):
+            text += signature
+
         prev_ticket_client_status = ticket.client_status
 
         with transaction.atomic():
-            ticket_message = cls.get_support_ticket_message().objects.create(
+            ticket_message = models.SupportTicketMessage.objects.create(
                 ticket=ticket,
                 text=text,
                 sender=sender,
                 is_system=is_system,
                 is_viewed=is_system,
             )
             if files:
-                cls.get_support_ticket_message_file().objects.filter(
-                    user=sender, id__in=[file.id for file in files]
+                models.SupportTicketMessageFile.objects.filter(
+                    id__in=[file.id for file in files]
                 ).update(ticket_message=ticket_message)
 
-        extra_fields = {}
-        if "event" in kwargs:
-            extra_fields["event"] = kwargs["event"]
-
         signals.support_ticket_message_created.send(
-            sender=None,
-            ticket_message=ticket_message,
-            prev_ticket_client_status=prev_ticket_client_status,
-            **extra_fields,
+            sender=None, ticket_message=ticket_message, prev_ticket_client_status=prev_ticket_client_status
         )
 
         return ticket_message
 
     @classmethod
     def create_system_message_after_status_change(
         cls,
-        ticket: models.AbstractSupportTicket,
+        ticket: models.SupportTicket,
         prev_status: constants.SUPPORT_TICKET_STATUSES,
-    ) -> models.AbstractSupportTicketMessage:
+    ) -> models.SupportTicketMessage:
         """
-        Создания системного сообщения для тикета ticket после изменения его статуса
+        Создание системного сообщения для тикета ticket после изменения его статуса
         """
         new_status = ticket.status
         text = None
 
         if prev_status in constants.SUPPORT_TICKET_ACTIVE_STATUSES:
             if new_status == constants.SUPPORT_TICKET_STATUSES.OPEN:
-                text = _("Заявка взята в обработку оператором: {manager}.").format(manager=ticket.manager)
+                text = constants.SUPPORT_TICKET_MESSAGES.OPEN
             elif new_status == constants.SUPPORT_TICKET_STATUSES.CLOSED_AUTO:
-                text = _("Заявка автоматически закрыта после длительного отсутствия активности.")
+                text = constants.SUPPORT_TICKET_MESSAGES.CLOSED_AUTO
             elif new_status == constants.SUPPORT_TICKET_STATUSES.CLOSED_BY_USER:
-                text = _("Заявка закрыта пользователем.")
+                text = constants.SUPPORT_TICKET_MESSAGES.CLOSED_BY_USER
             elif new_status == constants.SUPPORT_TICKET_STATUSES.CLOSED_BY_MANAGER:
-                text = _("Заявка закрыта оператором.")
+                text = constants.SUPPORT_TICKET_MESSAGES.CLOSED_BY_MANAGER
         else:
             if new_status == constants.SUPPORT_TICKET_STATUSES.OPEN:
-                text = _("Заявка повторно открыта.")
+                text = constants.SUPPORT_TICKET_MESSAGES.REOPEN
 
         if not text:
             raise NotImplementedError(f"Сообщение для смены статуса '{prev_status}' -> '{new_status}' неопределено.")
 
         return cls.create_ticket_message(ticket=ticket, text=text, sender=None, is_system=True)
 
     @classmethod
@@ -215,19 +200,19 @@
 
     @classmethod
     def close_inactive_tickets(cls) -> None:
         """
         Закрытие всех неактивных обращений в поддержку после settings.AUTO_CLOSE_TICKET_AFTER
         """
         now = timezone.now()
-        for ticket in cls.get_support_ticket().objects.filter(
+        for ticket in models.SupportTicket.objects.filter(
                 status=constants.SUPPORT_TICKET_ACTIVE_STATUSES.OPEN
         ):
             if ticket.manager:
                 last_message = ticket.last_message
                 # Последнее сообщение отправлено больше заданного кол-ва дней назад
                 if (
                     last_message
                     and (last_message.sender == ticket.manager)
-                    and (now > last_message.created + timezone.timedelta(days=settings.AUTO_CLOSE_TICKET_AFTER))
+                    and (now > last_message.created + timezone.timedelta(days=constants.AUTO_CLOSE_TICKET_AFTER))
                 ):
                     cls.set_ticket_status(ticket=ticket, status=constants.SUPPORT_TICKET_STATUSES.CLOSED_AUTO)
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/support/views.py` & `zonesmart-utils-fork-0.5.9/zs_utils/views/mixins.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,215 @@
-from django.db import transaction
-from django.db.models import Q
+from distutils.util import strtobool
+from rest_framework import status
 from rest_framework.decorators import action
-from rest_framework.parsers import MultiPartParser
-
-from zs_utils.support import constants
-from zs_utils.views import CustomModelViewSet
+from rest_framework.response import Response
+from rest_framework.exceptions import ValidationError
+from rest_framework.views import View
+from rest_framework.serializers import Serializer
+
+from django.conf import settings
+from django.contrib.auth.models import AnonymousUser
+from django.contrib.auth import get_user_model
+from django.utils.translation import gettext as _
 
 
 __all__ = [
-    "BaseSupportTicketView",
-    "BaseSupportTicketMessageView",
-    "BaseSupportTicketMessageFileView",
+    "AdminModeViewMixin",
+    "ResponseShortcutsViewMixin",
+    "DataValidationViewMixin",
+    "OnlyInstanceViewMixin",
+    "NearbyIdsViewMixin",
 ]
 
 
-class BaseSupportTicketView(CustomModelViewSet):
-    """
-    Абстрактный View для создания и просмотра тикетов (SupportTicket)
-    """
-    not_allowed_actions = [
-        "destroy",
-        "update",
-        "partial_update",
-    ]
-    staff_permission_classes = []
-
-    @classmethod
-    def get_support_ticket_service(cls):
-        raise NotImplementedError("В отображении должен быть определён метод получения модели SupportTicketService")
-
-    @classmethod
-    def get_create_support_ticket_serializer(cls):
-        raise NotImplementedError(
-            "В отображении должен быть определён метод получения модели CreateSupportTicketSerializer"
-        )
+class AdminModeViewMixin(View):
+    def _user_is_staff(self, user: settings.AUTH_USER_MODEL) -> bool:
+        return user.is_staff
 
-    def limit_queryset(self, queryset):
+    @property
+    def admin_mode(self) -> bool:
         """
-        Фильтрация QuerySet относительно роли пользователя
+        Включен режим администратора
         """
-        user = self.get_user()
-
-        if user.is_admin(user=user):
-            return queryset
-        elif user.is_staff(user=user):
-            return queryset.filter(Q(manager=user) | Q(status=constants.SUPPORT_TICKET_STATUSES.PENDING))
+        if not getattr(self, "_admin_mode", None):
+            return self._user_is_staff(user=self.request.user) and bool(
+                strtobool(self.request.GET.get("admin_mode", "false"))
+            )
+        return self._admin_mode
 
-        return super().limit_queryset(queryset)
+    @admin_mode.setter
+    def admin_mode(self, value: bool) -> None:
+        """
+        Установка значения для режима администрации
+        """
+        self._admin_mode = value
 
-    @action(detail=True, methods=["POST"])
-    def close(self, request, *args, **kwargs):
+    @property
+    def no_limit(self) -> bool:
         """
-        Закрытие тикета
+        Включён режим без ограничений
         """
-        self.get_support_ticket_service().close_ticket(user=self.get_user(), ticket=self.get_object())
-        return self.build_response()
+        if not getattr(self, "_no_limit", None):
+            self._no_limit = self.admin_mode and bool(strtobool(self.request.GET.get("no_limit", "false")))
+        return self._no_limit
 
-    def create(self, request, *args, **kwargs):
-        data = self.get_validated_data(serializer_class=self.get_create_support_ticket_serializer())
-        message = data.pop("message") if "message" in data else None
-        user = self.get_user()
-        with transaction.atomic():
-            instance = self.get_support_ticket_service().create_ticket(user=user, **data)
-            if message:
-                self.get_support_ticket_service().create_ticket_message(
-                    ticket=instance, sender=user, is_system=False, **message
-                )
-        return self.build_response(data=self.serializer_class(instance).data)
+    @no_limit.setter
+    def no_limit(self, value) -> None:
+        """
+        Установка значения для режима без ограничений
+        """
+        self._no_limit = value
 
-    @action(detail=True, methods=["POST"], permission_classes=staff_permission_classes)
-    def take_to_work(self, request, *args, **kwargs):
+    def get_user(self):
         """
-        Взятие тикета в работу (для staff пользователей)
+        Получение пользователя user.
+        В режиме администрации можно указывать любого пользователя и действовать от его лица
         """
-        if not self.staff_permission_classes:
-            raise NotImplementedError("В сервисе должен быть определён staff_permission_classes")
+        if self.admin_mode:
+            user_id = self.request.GET.get("user_id")
+            if user_id:
+                User = get_user_model()
+                try:
+                    return User.objects.get(id=user_id)
+                except User.DoesNotExist:
+                    raise ValidationError({"user_id": _("Пользователь не найден.")})
+
+        user = self.request.user
+        if isinstance(user, AnonymousUser):
+            user = None
 
-        self.get_support_ticket_service().take_ticket(manager=self.get_user(), ticket=self.get_object())
-        return self.build_response()
+        return user
 
-    @action(detail=True, methods=["POST"])
-    def reopen(self, request, *args, **kwargs):
+
+class OnlyInstanceViewMixin(View):
+    """
+    View-mixin для работы с единичными объектами (к пример у User лишь один объект настроек UserSettings)
+    """
+
+    def get_object(self):
         """
-        Открыть закрытый тикет
+        Получение единственного объекта
         """
-        self.get_support_ticket_service().reopen_ticket(user=self.get_user(), ticket=self.get_object())
-        return self.build_response()
-
-    @action(detail=True, methods=["POST"])
-    def set_viewed(self, request, *args, **kwargs):
-        self.get_support_ticket_service().set_ticket_viewed(user=self.get_user(), ticket=self.get_object())
-        return self.build_response()
+        return self.get_queryset().first()
 
-    @action(detail=False, methods=["GET"])
-    def get_metadata(self, request, *args, **kwargs):
+    def list(self, request, *args, **kwargs):
         """
-        Получение метаданных тикета (возможные статусы и тип вопроса)
+        Замена отдачи списка объектов на единичный объект
         """
-        data = {
-            "status": constants.SUPPORT_TICKET_STATUSES,
-            "question_type": constants.SUPPORT_TICKET_QUESTION_TYPES,
-        }
+        if getattr(self, "no_limit", False):
+            return super().list(request, *args, **kwargs)
+
+        instance = self.get_object()
+        if instance:
+            data = self.get_serializer(instance).data
+        else:
+            data = {}
+
         return self.build_response(data=data)
 
+    @action(detail=False, methods=["PUT", "PATCH"])
+    def alter(self, request, *args, **kwargs):
+        """
+        Обновление объекта
+        """
+        instance = self.get_object()
+
+        serializer = self.get_serializer(instance=instance, data=request.data)
+        serializer.is_valid(raise_exception=True)
+        instance = serializer.save()
 
-class BaseSupportTicketMessageView(CustomModelViewSet):
+        retrieve_serializer = self.serializer_classes.get(
+            "retrieve", self.serializer_classes.get("default", self.serializer_class)
+        )
+        return self.build_response(data=retrieve_serializer(instance=instance).data)
+
+
+class NearbyIdsViewMixin(View):
     """
-    Абстрактный View для создания/удаления/обновления/просмотра сообщений тикета (SupportTicketMessage)
+    View-mixin для получения соседних идентификаторов
     """
-    not_allowed_actions = [
-        "update",
-        "partial_update",
-        "destroy",
-    ]
-
-    @classmethod
-    def get_support_ticket(cls):
-        raise NotImplementedError("В отображении должен быть определён метод получения модели SupportTicket")
-
-    @classmethod
-    def get_support_ticket_service(cls):
-        raise NotImplementedError("В отображении должен быть определён метод получения модели SupportTicketService")
-
-    @classmethod
-    def get_create_support_ticket_message_serializer(cls):
-        raise NotImplementedError(
-            "В отображении должен быть определён метод получения модели CreateSupportTicketMessageSerializer"
-        )
 
-    def get_queryset_filter_kwargs(self) -> dict:
-        return {"ticket": self.kwargs["ticket_id"]}
+    @action(detail=True, methods=["GET"])
+    def get_nearby_ids(self, request, *args, **kwargs):
+        """
+        Получение соседних идентификаторов относительно переданного объекта
+        """
+        if hasattr(self, "actions_for_filterset_class"):
+            if self.actions_for_filterset_class != "__all__":
+                self.actions_for_filterset_class += ["get_nearby_ids"]
 
-    def create(self, request, *args, **kwargs):
+        qs = self.filter_queryset(self.get_queryset())
+        ids = list(qs.values_list(self.lookup_field, flat=True))
+        obj_id = getattr(self.get_object(), self.lookup_field)
+        obj_index = ids.index(obj_id)
+        prev_id = ids[obj_index - 1] if (obj_index - 1 >= 0) else None
+        next_id = ids[obj_index + 1] if (obj_index + 1 <= qs.count() - 1) else None
+
+        return Response({"prev_id": prev_id, "next_id": next_id}, status=status.HTTP_200_OK)
+
+
+class ResponseShortcutsViewMixin(View):
+    def build_response(
+        self,
+        message: str = None,
+        data: dict = None,
+        status_code: int = status.HTTP_200_OK,
+        **kwargs,
+    ) -> Response:
         """
-        Подстановка тикета SupportTicket.id и пользователя (отправителя) при создании нового сообщения
+        Создать ответ с переданным сообщением или данными. (Положительный по умолчанию)
         """
-        data = self.get_validated_data(serializer_class=self.get_create_support_ticket_message_serializer())
-        instance = self.get_support_ticket_service().create_ticket_message(
-            ticket=self.get_support_ticket().objects.get(id=kwargs["ticket_id"]),
-            sender=self.get_user(),
-            is_system=False,
-            **data,
+
+        if not data:
+            if message:
+                data = {"message": message}
+        elif message:
+            if isinstance(data, dict):
+                data = {"message": message, **data}
+            else:
+                data = {"message": message, "data": data}
+
+        return Response(data=data, status=status_code)
+
+    def build_error_response(
+        self,
+        message: str = None,
+        data: dict = None,
+        status_code: int = status.HTTP_400_BAD_REQUEST,
+        **kwargs,
+    ) -> Response:
+        """
+        Создать ответ с ошибкой с переданным сообщением или данными
+        """
+        return self.build_response(
+            message=message,
+            data=data,
+            status_code=status_code,
+            **kwargs,
         )
-        return self.build_response(data=self.serializer_class(instance).data)
 
 
-class BaseSupportTicketMessageFileView(CustomModelViewSet):
-    """
-    Абстрактный View для создания/удаления/обновления/просмотра файлов сообщений (SupportTicketMessageFile)
-    """
-    parser_classes = (MultiPartParser,)
-    not_allowed_actions = [
-        "update",
-        "partial_update",
-        "destroy",
-    ]
-
-    def get_queryset_filter_kwargs(self) -> dict:
-        return {"user": self.get_user()}
-
-    def create(self, request, *args, **kwargs):
-        request.data.update({"user": self.get_user().id})
-        return super().create(request, *args, **kwargs)
+class DataValidationViewMixin(View):
+    def validate_data(self, serializer_class: Serializer, data: dict = None) -> Serializer:
+        """
+        Валидация данных по переданному сериализатору
+        """
+
+        if not data:
+            data = {}
+            if isinstance(self.request.data, dict):
+                data.update(self.request.data)
+            data.update(self.request.GET.dict())
+
+        serializer = serializer_class(data=data)
+        serializer.is_valid(raise_exception=True)
+        return serializer
+
+    def get_validated_data(self, serializer_class, data: dict = None) -> dict:
+        """
+        Получение провалидированных данных по переданному сериализатору
+        """
+        serializer = self.validate_data(
+            serializer_class=serializer_class,
+            data=data,
+        )
+        return serializer.validated_data
```

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/time_utils.py` & `zonesmart-utils-fork-0.5.9/zs_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/transliterate.py` & `zonesmart-utils-fork-0.5.9/zs_utils/transliterate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/converter.py` & `zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/data.py` & `zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/data.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/exceptions.py` & `zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/exceptions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/parser.py` & `zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/parser.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/unit_converter/units.py` & `zonesmart-utils-fork-0.5.9/zs_utils/unit_converter/units.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/user/models.py` & `zonesmart-utils-fork-0.5.9/zs_utils/user/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/user/utils.py` & `zonesmart-utils-fork-0.5.9/zs_utils/user/utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/views/core.py` & `zonesmart-utils-fork-0.5.9/zs_utils/views/core.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/consumer.py` & `zonesmart-utils-fork-0.5.9/zs_utils/websocket/consumer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/middleware.py` & `zonesmart-utils-fork-0.5.9/zs_utils/websocket/middleware.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/services.py` & `zonesmart-utils-fork-0.5.9/zs_utils/websocket/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/websocket/tasks.py` & `zonesmart-utils-fork-0.5.9/zs_utils/websocket/tasks.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/xml_parser.py` & `zonesmart-utils-fork-0.5.9/zs_utils/xml_parser.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/__init__.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/abstract.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/abstract.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/age.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/age.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/category.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/condition.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/condition.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/currency.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/dimensions.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/dimensions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/feed.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/feed.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/fields/options.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/fields/options.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/gift.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/gift.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/offers.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/offers.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/option.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/option.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/outlet.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/outlet.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/parameter.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/parameter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/price.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/price.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/promo.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/promo.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/models/shop.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/models/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-fork-0.5.3.9/zs_utils/yandex_market_language/yml.py` & `zonesmart-utils-fork-0.5.9/zs_utils/yandex_market_language/yml.py`

 * *Files identical despite different names*

