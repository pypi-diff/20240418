# Comparing `tmp/dbt-materialize-1.7.5.tar.gz` & `tmp/dbt-materialize-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.7.5.tar", last modified: Fri Mar 15 17:54:49 2024, max compression
+gzip compressed data, was "dbt-materialize-1.7.6.tar", last modified: Thu Apr 18 14:01:05 2024, max compression
```

## Comparing `dbt-materialize-1.7.5.tar` & `dbt-materialize-1.7.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/
--rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/MANIFEST.in
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/README.md
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/exceptions.py
--rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize   (993)     8504 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/catalog.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/columns.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_await.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)    12165 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_init.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     6074 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5847 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_promote.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/freshness.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/materializedview.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1965 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2011 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/materialize/macros/tests/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/tests/helpers.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/await_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/ci_utils.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/exists.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/generate_cluster_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/generate_schema_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/is_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/listagg.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/profile_template.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/materialize/sample_profiles.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/starter_project/
--rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.782899 dbt-materialize-1.7.5/dbt/include/starter_project/models/
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/
--rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/fraud_activity.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/funds_movement.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/sources/
--rw-r--r--   0 materialize  (2000) materialize   (993)      900 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/sources/auction.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/sources/sources.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/dbt/include/starter_project/models/example/winning_bids.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-03-15 17:54:49.000000 dbt-materialize-1.7.5/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-03-15 17:54:49.000000 dbt-materialize-1.7.5/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-03-15 17:54:49.000000 dbt-materialize-1.7.5/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-03-15 17:54:49.000000 dbt-materialize-1.7.5/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-03-15 17:54:49.000000 dbt-materialize-1.7.5/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/pyproject.toml
--rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-03-15 17:54:49.792900 dbt-materialize-1.7.5/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-03-15 17:52:34.000000 dbt-materialize-1.7.5/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/MANIFEST.in
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/README.md
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/exceptions.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/catalog.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/columns.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_await.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)    12165 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_init.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6074 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_promote.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/freshness.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materializedview.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/helpers.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/await_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/ci_utils.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/exists.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_cluster_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_schema_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/is_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/listagg.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/profile_template.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/sample_profiles.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/include/starter_project/models/
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/fraud_activity.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/funds_movement.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      900 2024-04-18 13:58:48.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/auction.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/sources.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/winning_bids.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/pyproject.toml
+-rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/setup.py
```

### Comparing `dbt-materialize-1.7.5/PKG-INFO` & `dbt-materialize-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.5
+Version: 1.7.6
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.5/README.md` & `dbt-materialize-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/__init__.py` & `dbt-materialize-1.7.6/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/__init__.py` & `dbt-materialize-1.7.6/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.7.5"
+version = "1.7.6"
```

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/exceptions.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.7.6/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/__init__.py` & `dbt-materialize-1.7.6/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/__init__.py` & `dbt-materialize-1.7.6/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.7.6/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/adapters.sql`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,48 @@
     {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
       {{exceptions.warn("Model contracts cannot be enforced for custom materializations (see dbt-core #7213)")}}
     {%- endif %}
     {{ sql }}
 {%- endmacro %}
 
+{% macro materialize__create_source(relation, sql) -%}
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config.enforced %}
+    {{exceptions.warn("Model contracts cannot be enforced for custom materializations (see dbt-core #7213)")}}
+  {%- endif %}
+
+  {%- set cluster = generate_cluster_name(config.get('cluster', target.cluster)) -%}
+
+  create source {{ relation }}
+  {% if cluster %}
+    in cluster {{ cluster }}
+  {% endif %}
+
+  {{ sql }}
+  ;
+  {%- endmacro %}
+
+{% macro materialize__create_sink(relation, sql) -%}
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config.enforced %}
+    {{exceptions.warn("Model contracts cannot be enforced for custom materializations (see dbt-core #7213)")}}
+  {%- endif %}
+
+  {%- set cluster = generate_cluster_name(config.get('cluster', target.cluster)) -%}
+
+  create sink {{ relation }}
+  {% if cluster %}
+    in cluster {{ cluster }}
+  {% endif %}
+
+  {{ sql }}
+  ;
+  {%- endmacro %}
+
 {% macro materialize__rename_relation(from_relation, to_relation) -%}
   {% set target_name = adapter.quote_as_configured(to_relation.identifier, 'identifier') %}
   {% call statement('rename_relation') -%}
     {% if relation.type == 'view' %}
       alter view {{ from_relation }} rename to {{ target_name }}
     {% else %}
       alter materialized view {{ from_relation }} rename to {{ target_name }}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/columns.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_await.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_await.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_cleanup.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_cleanup.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_init.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_init.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/deploy/deploy_promote.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_promote.sql`

 * *Files 9% similar despite different names*

```diff
@@ -52,36 +52,36 @@
     {% set deploy_schema = schema ~ "_dbt_deploy" %}
     {% if not schema_exists(schema) %}
         {{ exceptions.raise_compiler_error("Production schema " ~ schema ~ " does not exist") }}
     {% endif %}
     {% if not schema_exists(deploy_schema) %}
         {{ exceptions.raise_compiler_error("Deployment schema " ~ deploy_schema ~ " does not exist") }}
     {% endif %}
-    {% if schema_contains_sources_or_sinks(deploy_schema) %}
+    {% if schema_contains_sinks(deploy_schema) %}
         {{ exceptions.raise_compiler_error("""
-        Deployment schema " ~ deploy_schema ~ " contains sources or sinks. This is not currently
-        supported by dbt run-operation deploy_promote.
+        Deployment schema " ~ deploy_schema ~ " contains sinks. This is not currently
+        supported by the deploy_promote macro.
 
         If this feature is important to you, please reach out!
         """) }}
     {% endif %}
 {% endfor %}
 
 {% for cluster in clusters %}
     {% set deploy_cluster = cluster ~ "_dbt_deploy" %}
     {% if not cluster_exists(cluster) %}
         {{ exceptions.raise_compiler_error("Production cluster " ~ cluster ~ " does not exist") }}
     {% endif %}
     {% if not cluster_exists(deploy_cluster) %}
         {{ exceptions.raise_compiler_error("Deployment cluster " ~ deploy_cluster ~ " does not exist") }}
     {% endif %}
-    {% if cluster_contains_sources_or_sinks(deploy_cluster) %}
+    {% if cluster_contains_sinks(deploy_cluster) %}
         {{ exceptions.raise_compiler_error("""
-        Deployment cluster " ~ deploy_cluster ~ " contains sources or sinks. This is not currently
-        supported by dbt run-operation deploy_promote.
+        Deployment cluster " ~ deploy_cluster ~ " contains sinks. This is not currently
+        supported by the deploy_promote macro.
 
         If this feature is important to you, please reach out!
         """) }}
     {% endif %}
 {% endfor %}
 
 {% if wait %}
@@ -103,53 +103,33 @@
     ALTER CLUSTER {{ adapter.quote(cluster) }} SWAP WITH {{ adapter.quote(deploy_cluster) }};
 {% endfor %}
 
 COMMIT;
 {%- endcall %}
 {% endmacro %}
 
-{% macro cluster_contains_sources_or_sinks(cluster) %}
+{% macro cluster_contains_sinks(cluster) %}
     {% set query %}
-        WITH sources_and_sinks AS (
-            SELECT cluster_id
-            FROM mz_sources
-
-            UNION ALL
-
-            SELECT cluster_id
-            FROM mz_sinks
-        )
-
         SELECT count(*) > 0
-        FROM sources_and_sinks
-        JOIN mz_clusters ON sources_and_sinks.cluster_id = mz_clusters.id
+        FROM mz_sinks
+        JOIN mz_clusters ON mz_sinks.cluster_id = mz_clusters.id
         WHERE mz_clusters.name = {{ dbt.string_literal(cluster) }}
     {% endset %}
 
     {% set count = run_query(query) %}
     {% if execute %}
         {{ return(count.rows[0][0]) }}
     {% endif %}
 {% endmacro %}
 
-{% macro schema_contains_sources_or_sinks(schema) %}
+{% macro schema_contains_sinks(schema) %}
     {% set query %}
-        WITH sources_and_sinks AS (
-            SELECT schema_id
-            FROM mz_sources
-
-            UNION ALL
-
-            SELECT schema_id
-            FROM mz_sinks
-        )
-
         SELECT count(*) > 0
-        FROM sources_and_sinks
-        JOIN mz_schemas ON sources_and_sinks.schema_id = mz_schemas.id
+        FROM mz_sinks
+        JOIN mz_schemas ON mz_sinks.schema_id = mz_schemas.id
         JOIN mz_databases ON mz_schemas.database_id = mz_databases.id
         WHERE mz_schemas.name = {{ dbt.string_literal(schema) }}
             AND mz_databases.name = current_database()
     {% endset %}
 
     {% set count = run_query(query) %}
     {% if execute %}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/freshness.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/materializedview.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     {{ adapter.drop_relation(old_relation) }}
   {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% call statement('main') -%}
-    {{ materialize__create_arbitrary_object(sql) }}
+    {{ materialize__create_sink(target_relation, sql) }}
   {%- endcall %}
 
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/table.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+-- Copyright 2020 Josh Wills. All rights reserved.
 -- Copyright Materialize, Inc. and contributors. All rights reserved.
 --
 -- Licensed under the Apache License, Version 2.0 (the "License");
 -- you may not use this file except in compliance with the License.
 -- You may obtain a copy of the License in the LICENSE file at the
 -- root of this repository, or online at
 --
@@ -9,41 +10,34 @@
 --
 -- Unless required by applicable law or agreed to in writing, software
 -- distributed under the License is distributed on an "AS IS" BASIS,
 -- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 -- See the License for the specific language governing permissions and
 -- limitations under the License.
 
-{% materialization source, adapter='materialize' %}
-  {% if var('deploy', False) %}
-      {{ exceptions.CompilationError(
-        """
-        dbt-materialize does not support deployments for sources.
-        """
-    )}}
-  {% endif %}
-
+{% materialization table, adapter='materialize' %}
   {%- set identifier = model['alias'] -%}
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
-                                                type='source') -%}
+                                                type='materialized_view') -%}
 
   {% if old_relation %}
     {{ adapter.drop_relation(old_relation) }}
   {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% call statement('main') -%}
-    {{ materialize__create_arbitrary_object(sql) }}
+    -- Creates a materialized view, not a table, in Materialize
+    {{ materialize__create_materialized_view_as(target_relation, sql) }}
   {%- endcall %}
 
   {{ create_indexes(target_relation) }}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/view.sql`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 --
 -- Unless required by applicable law or agreed to in writing, software
 -- distributed under the License is distributed on an "AS IS" BASIS,
 -- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 -- See the License for the specific language governing permissions and
 -- limitations under the License.
 
-{% materialization table, adapter='materialize' %}
+{% materialization view, adapter='materialize' %}
   {%- set identifier = model['alias'] -%}
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
-                                                type='materialized_view') -%}
+                                                type='view') -%}
 
   {% if old_relation %}
     {{ adapter.drop_relation(old_relation) }}
   {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% call statement('main') -%}
-    -- Creates a materialized view, not a table, in Materialize
-    {{ materialize__create_materialized_view_as(target_relation, sql) }}
+    {{ materialize__create_view_as(target_relation, sql) }}
   {%- endcall %}
 
   {{ create_indexes(target_relation) }}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/source.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
--- Copyright 2020 Josh Wills. All rights reserved.
 -- Copyright Materialize, Inc. and contributors. All rights reserved.
 --
 -- Licensed under the Apache License, Version 2.0 (the "License");
 -- you may not use this file except in compliance with the License.
 -- You may obtain a copy of the License in the LICENSE file at the
 -- root of this repository, or online at
 --
@@ -10,33 +9,33 @@
 --
 -- Unless required by applicable law or agreed to in writing, software
 -- distributed under the License is distributed on an "AS IS" BASIS,
 -- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 -- See the License for the specific language governing permissions and
 -- limitations under the License.
 
-{% materialization view, adapter='materialize' %}
+{% materialization source, adapter='materialize' %}
   {%- set identifier = model['alias'] -%}
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
-                                                type='view') -%}
+                                                type='source') -%}
 
   {% if old_relation %}
     {{ adapter.drop_relation(old_relation) }}
   {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% call statement('main') -%}
-    {{ materialize__create_view_as(target_relation, sql) }}
+    {{ materialize__create_source(target_relation, sql) }}
   {%- endcall %}
 
   {{ create_indexes(target_relation) }}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/tests/helpers.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/await_cluster_ready.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/await_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/ci_utils.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/ci_utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/exists.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/exists.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/generate_cluster_name.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_cluster_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/generate_schema_name.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/is_cluster_ready.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/is_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/profile_template.yml` & `dbt-materialize-1.7.6/dbt/include/materialize/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/materialize/sample_profiles.yml` & `dbt-materialize-1.7.6/dbt/include/materialize/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/dbt_project.yml` & `dbt-materialize-1.7.6/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/fraud_activity.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/fraud_activity.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/funds_movement.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/funds_movement.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/my_first_dbt_model.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_first_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/my_second_dbt_model.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_second_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/schema.yml` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/sources/auction.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/auction.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/sources/sources.yml` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/sources.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt/include/starter_project/models/example/winning_bids.sql` & `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/winning_bids.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.7.6/dbt_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.5
+Version: 1.7.6
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.5/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.7.6/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.5/setup.py` & `dbt-materialize-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 README = Path(__file__).parent / "README.md"
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.7.5",
+    version="1.7.6",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
```

