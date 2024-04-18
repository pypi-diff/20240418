# Comparing `tmp/nsj_rest_lib-2.6.3.tar.gz` & `tmp/nsj_rest_lib-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-2.6.3.tar", last modified: Mon Mar  4 22:28:12 2024, max compression
+gzip compressed data, was "nsj_rest_lib-2.6.4.tar", last modified: Thu Apr 18 14:26:57 2024, max compression
```

## Comparing `nsj_rest_lib-2.6.3.tar` & `nsj_rest_lib-2.6.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/
--rw-r--r--   0 sergio    (1000) sergio    (1000)    23835 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    22979 2024-03-04 21:52:29.000000 nsj_rest_lib-2.6.3/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.613180 nsj_rest_lib-2.6.3/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.613180 nsj_rest_lib-2.6.3/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.613180 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/constants.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2023-08-20 19:12:24.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.613180 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1419 2023-10-05 17:46:49.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10906 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/dto.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/entity.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_left_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7389 2024-03-04 22:23:16.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dto/after_insert_update_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16234 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    55777 2024-03-04 17:44:01.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      842 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/util/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/util/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/util/join_aux.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/util/type_validator_util.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/validate_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib/wsgi.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-03-04 22:28:12.617179 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)    23835 2024-03-04 22:28:12.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2063 2024-03-04 22:28:12.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-03-04 22:28:12.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-03-04 22:28:12.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-03-04 22:28:12.000000 nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4082 2024-03-19 17:07:11.000000 nsj_rest_lib-2.6.4/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/constants.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2023-08-20 19:12:24.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1419 2023-10-05 17:46:49.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10906 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/dto.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/entity.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_left_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7331 2024-03-05 22:27:27.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/after_insert_update_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16234 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    55849 2024-04-18 14:26:34.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      845 2024-03-06 20:26:30.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/join_aux.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/type_validator_util.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/validate_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/wsgi.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2063 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-2.6.3/setup.cfg` & `nsj_rest_lib-2.6.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 2.6.3
+version = 2.6.4
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/decorator/entity.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/entity.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_left_join_field.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_left_join_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/descriptor/dto_sql_join_field.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_sql_join_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 
 class DTOJoinFieldType:
     LEFT = "left"
     INNER = "inner"
     FULL = "full outer"
 
 
-# TODO Adicionar suporte a esse tipo de field no GET (GET ONE e não GET LIST)
 # TODO Adicionar suporte ao search
-# TODO Implementar o filters abaixo
+# TODO Implementar o filters comentado no construtor
 # TODO Pensar em como ordenar os joins (quando tiver um left no meio, pode ser útil)
 # TODO Pensar em como passar mais condições dentro do ON
 # TODO Pensar em como usar um só entity (e não precisar de um com os campos que vem da outra entidade)
-# TODO Verificar se ficou a abstração pelo DTO (porque o join ficou bem distante do natural em SQL)
+# TODO Verificar se ficou boa a abstração pelo DTO (porque o join ficou bem distante do natural em SQL)
 
 
 class DTOSQLJoinField:
     _ref_counter = 0
 
     def __init__(
         self,
```

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/service_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1425,14 +1425,15 @@
                     )
 
                 # Copiando os campos necessários
                 for field in fields_necessarios:
                     # Recuperando a configuração do campo left join
                     left_join_field: DTOLeftJoinField = dto.left_join_fields_map[field]
 
-                    # Recuperando o valor da propriedade no DTO relacionado
-                    field_value = getattr(
-                        related_dto, left_join_field.related_dto_field
-                    )
+                    if related_dto is not None:
+                        # Recuperando o valor da propriedade no DTO relacionado
+                        field_value = getattr(
+                            related_dto, left_join_field.related_dto_field
+                        )
 
-                    # Gravando o valor no DTO de interesse
-                    setattr(dto, field, field_value)
+                        # Gravando o valor no DTO de interesse
+                        setattr(dto, field, field_value)
```

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/util/type_validator_util.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/type_validator_util.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.3/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*
