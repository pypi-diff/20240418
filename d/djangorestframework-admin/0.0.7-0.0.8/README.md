# Comparing `tmp/djangorestframework-admin-0.0.7.tar.gz` & `tmp/djangorestframework-admin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-admin-0.0.7.tar", last modified: Wed Apr  3 05:55:50 2024, max compression
+gzip compressed data, was "djangorestframework-admin-0.0.8.tar", last modified: Thu Apr 18 03:38:40 2024, max compression
```

## Comparing `djangorestframework-admin-0.0.7.tar` & `djangorestframework-admin-0.0.8.tar`

### file list

```diff
@@ -1,118 +1,140 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.306277 djangorestframework-admin-0.0.7/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-12-22 08:20:25.000000 djangorestframework-admin-0.0.7/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/MANIFEST.in
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1969 2024-04-03 05:55:50.302259 djangorestframework-admin-0.0.7/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.018309 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1969 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3968 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      130 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/top_level.txt
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.034698 djangorestframework-admin-0.0.7/rest_framework_admin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      389 2024-04-03 05:38:11.000000 djangorestframework-admin-0.0.7/rest_framework_admin/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.134384 djangorestframework-admin-0.0.7/rest_framework_admin/auth/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      270 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.236485 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1186 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      406 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/exceptions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      983 2024-04-03 05:37:26.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/middlewares.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      669 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.267275 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1168 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/blacklist.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1930 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.304322 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1682 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      164 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3109 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/tests.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      837 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.364329 djangorestframework-admin-0.0.7/rest_framework_admin/doc/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.376794 djangorestframework-admin-0.0.7/rest_framework_admin/doc/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       60 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      790 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.525240 djangorestframework-admin-0.0.7/rest_framework_admin/role/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1506 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2266 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/filters.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.601288 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13635 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0001_initial.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1308 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0002_create_role.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1097 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0003_create_user_role_rel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      901 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0004_delete_useless_table.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7893 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1446 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8745 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2530 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/services.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1415 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5452 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.741956 djangorestframework-admin-0.0.7/rest_framework_admin/system/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      290 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      191 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      477 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      410 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      551 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1567 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      527 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/tests.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      807 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4468 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.892949 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      256 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      718 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      759 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/filters.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.946968 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6632 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0001_initial.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1313 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0002_create_role.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1164 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1195 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3319 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      834 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2082 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/views.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1287 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.113170 djangorestframework-admin-0.0.7/rest_framework_admin/user/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      320 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      655 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      736 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/filters.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.238052 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      751 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1156 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1193 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2919 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      826 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2134 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.291381 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11732 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0001_initial.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1528 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0002_create_user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6331 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5543 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      915 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3174 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/views.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-03 05:55:50.306277 djangorestframework-admin-0.0.7/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3395 2024-03-25 06:23:56.000000 djangorestframework-admin-0.0.7/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.763435 djangorestframework-admin-0.0.8/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1086 2024-04-18 03:25:05.000000 djangorestframework-admin-0.0.8/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/MANIFEST.in
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2710 2024-04-18 03:38:40.762307 djangorestframework-admin-0.0.8/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1841 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.072128 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2710 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4595 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/not-zip-safe
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      130 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-04-18 03:38:38.000000 djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/top_level.txt
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.099707 djangorestframework-admin-0.0.8/rest_framework_admin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      389 2024-04-18 03:34:30.000000 djangorestframework-admin-0.0.8/rest_framework_admin/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.226741 djangorestframework-admin-0.0.8/rest_framework_admin/auth/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      270 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.370628 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1186 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      406 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/exceptions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      983 2024-04-03 05:37:26.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/middlewares.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-04-16 05:15:10.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      669 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.414342 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/utils/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1168 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/utils/blacklist.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1930 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.461603 djangorestframework-admin-0.0.8/rest_framework_admin/auth/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/model/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1682 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/model/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      164 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2919 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/tests.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1391 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/auth/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.540805 djangorestframework-admin-0.0.8/rest_framework_admin/doc/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.540805 djangorestframework-admin-0.0.8/rest_framework_admin/doc/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       60 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      790 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/doc/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.607040 djangorestframework-admin-0.0.8/rest_framework_admin/group/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/group/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      371 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/group/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      545 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/group/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      975 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/group/serializers.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.762831 djangorestframework-admin-0.0.8/rest_framework_admin/role/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      383 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1341 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.802828 djangorestframework-admin-0.0.8/rest_framework_admin/role/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13167 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7822 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/models.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:39.922915 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      572 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      716 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      474 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      431 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      523 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      979 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permission/views.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1164 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8863 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2492 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/services.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1363 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5392 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/role/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.133506 djangorestframework-admin-0.0.8/rest_framework_admin/system/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      290 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      191 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      477 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      410 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      569 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1567 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      527 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/tests.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      807 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4468 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/system/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.268878 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      256 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      115 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      755 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.302331 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6896 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1145 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1863 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3641 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      523 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      867 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2412 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tenant/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.319237 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.350556 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/role/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/role/0002_delete_useless_table.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/role/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.365256 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/user/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/tmp/user/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1287 2024-04-15 03:19:46.000000 djangorestframework-admin-0.0.8/rest_framework_admin/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.521757 djangorestframework-admin-0.0.8/rest_framework_admin/user/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      320 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      811 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      732 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.632617 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      670 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1469 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1532 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      859 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/group/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.697360 djangorestframework-admin-0.0.8/rest_framework_admin/user/me/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/me/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2970 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/me/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      546 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/me/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2807 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/me/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:38:40.744886 djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11705 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1528 2024-04-10 09:41:59.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/0002_create_user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7483 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1897 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5875 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1042 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3019 2024-04-18 03:25:06.000000 djangorestframework-admin-0.0.8/rest_framework_admin/user/views.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-18 03:38:40.763435 djangorestframework-admin-0.0.8/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3395 2024-03-25 06:23:56.000000 djangorestframework-admin-0.0.8/setup.py
```

### Comparing `djangorestframework-admin-0.0.7/LICENSE` & `djangorestframework-admin-0.0.8/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Copyright (c) 2023 iamfengdy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+furnished to do so, member to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/SOURCES.txt` & `djangorestframework-admin-0.0.8/djangorestframework_admin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,31 +31,39 @@
 rest_framework_admin/auth/model/backends.py
 rest_framework_admin/doc/__init__.py
 rest_framework_admin/doc/admin.py
 rest_framework_admin/doc/apps.py
 rest_framework_admin/doc/models.py
 rest_framework_admin/doc/urls.py
 rest_framework_admin/doc/migrations/__init__.py
+rest_framework_admin/group/__init__.py
+rest_framework_admin/group/filters.py
+rest_framework_admin/group/models.py
+rest_framework_admin/group/serializers.py
 rest_framework_admin/role/__init__.py
 rest_framework_admin/role/admin.py
 rest_framework_admin/role/apps.py
 rest_framework_admin/role/configs.py
 rest_framework_admin/role/filters.py
 rest_framework_admin/role/models.py
 rest_framework_admin/role/permissions.py
 rest_framework_admin/role/serializers.py
 rest_framework_admin/role/services.py
 rest_framework_admin/role/settings.py
 rest_framework_admin/role/urls.py
 rest_framework_admin/role/views.py
 rest_framework_admin/role/migrations/0001_initial.py
-rest_framework_admin/role/migrations/0002_create_role.py
-rest_framework_admin/role/migrations/0003_create_user_role_rel.py
-rest_framework_admin/role/migrations/0004_delete_useless_table.py
 rest_framework_admin/role/migrations/__init__.py
+rest_framework_admin/role/permission/__init__.py
+rest_framework_admin/role/permission/filters.py
+rest_framework_admin/role/permission/models.py
+rest_framework_admin/role/permission/permissions.py
+rest_framework_admin/role/permission/serializers.py
+rest_framework_admin/role/permission/urls.py
+rest_framework_admin/role/permission/views.py
 rest_framework_admin/system/__init__.py
 rest_framework_admin/system/apps.py
 rest_framework_admin/system/configs.py
 rest_framework_admin/system/filters.py
 rest_framework_admin/system/models.py
 rest_framework_admin/system/permissions.py
 rest_framework_admin/system/serializers.py
@@ -67,19 +75,23 @@
 rest_framework_admin/tenant/admin.py
 rest_framework_admin/tenant/apps.py
 rest_framework_admin/tenant/configs.py
 rest_framework_admin/tenant/filters.py
 rest_framework_admin/tenant/models.py
 rest_framework_admin/tenant/permissions.py
 rest_framework_admin/tenant/serializers.py
+rest_framework_admin/tenant/settings.py
 rest_framework_admin/tenant/urls.py
 rest_framework_admin/tenant/views.py
 rest_framework_admin/tenant/migrations/0001_initial.py
-rest_framework_admin/tenant/migrations/0002_create_role.py
 rest_framework_admin/tenant/migrations/__init__.py
+rest_framework_admin/tmp/__init__.py
+rest_framework_admin/tmp/role/0002_delete_useless_table.py
+rest_framework_admin/tmp/role/__init__.py
+rest_framework_admin/tmp/user/__init__.py
 rest_framework_admin/user/__init__.py
 rest_framework_admin/user/admin.py
 rest_framework_admin/user/apps.py
 rest_framework_admin/user/configs.py
 rest_framework_admin/user/filters.py
 rest_framework_admin/user/models.py
 rest_framework_admin/user/permissions.py
@@ -90,10 +102,14 @@
 rest_framework_admin/user/group/__init__.py
 rest_framework_admin/user/group/filters.py
 rest_framework_admin/user/group/models.py
 rest_framework_admin/user/group/permissions.py
 rest_framework_admin/user/group/serializers.py
 rest_framework_admin/user/group/urls.py
 rest_framework_admin/user/group/views.py
+rest_framework_admin/user/me/__init__.py
+rest_framework_admin/user/me/serializers.py
+rest_framework_admin/user/me/urls.py
+rest_framework_admin/user/me/views.py
 rest_framework_admin/user/migrations/0001_initial.py
 rest_framework_admin/user/migrations/0002_create_user.py
 rest_framework_admin/user/migrations/__init__.py
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/backends.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/middlewares.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/middlewares.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/blacklist.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/utils/blacklist.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/views.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/jwt/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/backends.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/model/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,22 +69,17 @@
 
     nickname = serializers.CharField(
         required=False,
         allow_blank=True,
         allow_null=True,
         help_text='昵称')
 
-    is_staff = serializers.BooleanField(
-        required=False,
-        default=False,
-        help_text='是否为员工，默认为False, 为True时需要手动激活')
-
     class Meta:
         model = User
-        fields = ('id', 'username', 'password', 'email', 'telephone', 'nickname', 'is_staff',
+        fields = ('id', 'username', 'password', 'email', 'telephone', 'nickname',
                   'create_datetime')
         read_only_fields = ('id', 'create_datetime')
 
     def create(self, validated_data):
         if validated_data.get('is_staff', False):
             # 如果非用户，则需要管理员手动激活
             validated_data['is_active'] = False
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/settings.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/auth/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/doc/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/doc/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/filters.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/filters.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,64 +6,42 @@
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
 from django_filters import rest_framework as filters
 
-from rest_framework_admin.role.configs import SubjectTypeEnum
-from rest_framework_admin.role.models import Role, RolePermissionRel, RoleSubjectRel, Permission
-
-
-class PermissionFilter(filters.FilterSet):
-    name = filters.CharFilter(lookup_expr='icontains')
-
-    class Meta:
-        model = Permission
-        fields = ['name']
+from rest_framework_admin.role.configs import MemberTypeEnum
+from rest_framework_admin.role.models import Role, RolePermissionRel, RoleMemberRel, Permission
 
 
 class RoleFilter(filters.FilterSet):
     name = filters.CharFilter(lookup_expr='icontains')
     code = filters.CharFilter(lookup_expr='icontains')
     type = filters.CharFilter(method='filter_by_type')
-    user_id = filters.CharFilter(method='filter_by_user_id')
-    group_id = filters.CharFilter(method='filter_by_group_id')
-    # permission_id = filters.CharFilter(method='filter_by_group_id')
 
     class Meta:
         model = Role
-        fields = ['name', 'code', 'type', 'user_id', 'group_id']
+        fields = ['name', 'code', 'type']
 
     def filter_by_type(self, queryset, name, value):
         return queryset.filter(type__in=value.split(','))
 
-    def filter_by_user_id(self, queryset, name, value):
-        queryset = queryset.filter(
-            subject_rels__subject_id=value, subject_rels__type=SubjectTypeEnum.user.name)
-        return Role.filter_by_valid(queryset, is_valid=True)
-
-    def filter_by_group_id(self, queryset, name, value):
-        queryset = queryset.filter(
-            subject_rels__subject_id=value, subject_rels__type=SubjectTypeEnum.user_group.name).all()
-        return Role.filter_by_valid(queryset, is_valid=True)
-
 
-class RoleRelatedPermissionFilter(filters.FilterSet):
+class RolePermissionRelFilter(filters.FilterSet):
     id = filters.CharFilter(field_name='permission_id')
-
     name = filters.CharFilter(
         lookup_expr='icontains',
         field_name='permission__name')
 
     class Meta:
         model = RolePermissionRel
         fields = ['id', 'name']
 
 
-class RoleRelatedSubjectFilter(filters.FilterSet):
-    id = filters.CharFilter(field_name='subject_id')
-    type = filters.CharFilter(field_name='subject_type')
+class RoleMemberRelFilter(filters.FilterSet):
+    id = filters.CharFilter(field_name='member_id')
+    type = filters.CharFilter(field_name='member_type')
 
     class Meta:
-        model = RoleSubjectRel
+        model = RoleMemberRel
         fields = ['id', 'type']
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0001_initial.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.13 on 2024-03-31 08:16
+# Generated by Django 4.1.13 on 2024-04-15 08:53
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import shortcut_util.unique
 
 
@@ -44,18 +44,14 @@
                 (
                     "delete_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="删除时间"),
                 ),
                 ("content_type", models.CharField(max_length=64, verbose_name="内容类型")),
                 ("action", models.CharField(max_length=64, verbose_name="动作")),
                 (
-                    "scope_type",
-                    models.CharField(help_text="范围类型", max_length=32, null=True),
-                ),
-                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -78,15 +74,15 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "权限表",
-                "db_table": "admin_role_permission",
+                "db_table": "role_permission",
                 "unique_together": {("content_type", "action")},
             },
         ),
         migrations.CreateModel(
             name="Role",
             fields=[
                 (
@@ -119,18 +115,14 @@
                 ("code", models.CharField(max_length=64, verbose_name="编码")),
                 ("type", models.CharField(max_length=32, verbose_name="类型")),
                 (
                     "weight",
                     models.PositiveSmallIntegerField(verbose_name="权重，值越高优先级越高，即权限越大"),
                 ),
                 (
-                    "scope_type",
-                    models.CharField(help_text="范围类型", max_length=32, null=True),
-                ),
-                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -143,15 +135,15 @@
                         related_name="deleted_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "角色表",
-                "db_table": "admin_role",
+                "db_table": "role",
             },
         ),
         migrations.CreateModel(
             name="RolePermissionRel",
             fields=[
                 (
                     "id",
@@ -198,21 +190,23 @@
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "permission",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
+                        related_name="role_rels",
                         to="admin_role.permission",
                     ),
                 ),
                 (
                     "role",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
+                        related_name="permission_rels",
                         to="admin_role.role",
                     ),
                 ),
                 (
                     "update_user",
                     models.ForeignKey(
                         blank=True,
@@ -221,15 +215,15 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "角色权限关联表",
-                "db_table": "admin_role_permission_rel",
+                "db_table": "role_permission_rel",
                 "unique_together": {("role", "permission")},
             },
         ),
         migrations.AddField(
             model_name="role",
             name="permissions",
             field=models.ManyToManyField(
@@ -246,15 +240,15 @@
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="updated_%(app_label)s_%(class)ss",
                 to=settings.AUTH_USER_MODEL,
             ),
         ),
         migrations.CreateModel(
-            name="RoleSubjectRel",
+            name="RoleMemberRel",
             fields=[
                 (
                     "id",
                     models.CharField(
                         default=shortcut_util.unique.uuid_id,
                         max_length=32,
                         primary_key=True,
@@ -276,30 +270,23 @@
                     models.CharField(blank=True, max_length=256, verbose_name="描述"),
                 ),
                 (
                     "delete_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="删除时间"),
                 ),
                 (
-                    "subject_id",
+                    "member_id",
                     models.CharField(help_text="主体id，用户id/组id", max_length=32),
                 ),
-                (
-                    "subject_type",
-                    models.CharField(help_text="主体类型，用户/组", max_length=32),
-                ),
+                ("member_type", models.CharField(help_text="主体类型，用户/组", max_length=32)),
                 (
                     "expire_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="过期时间"),
                 ),
                 (
-                    "scope_id",
-                    models.CharField(help_text="范围id", max_length=32, null=True),
-                ),
-                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -313,15 +300,15 @@
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "role",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
-                        related_name="subject_rels",
+                        related_name="member_rels",
                         to="admin_role.role",
                     ),
                 ),
                 (
                     "update_user",
                     models.ForeignKey(
                         blank=True,
@@ -329,13 +316,13 @@
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
-                "verbose_name": "角色主体表",
-                "db_table": "admin_role_subject_rel",
-                "unique_together": {("subject_id", "role", "subject_type")},
+                "verbose_name": "角色成员关联表",
+                "db_table": "role_member_rel",
+                "unique_together": {("member_id", "role", "member_type")},
             },
         ),
     ]
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0002_create_role.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/0002_create_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 #!/usr/bin/python
 # -*- coding:utf-8 -*-
 # Email:iamfengdy@126.com
 # DateTime:2023/11/21
 # Tool:PyCharm
 
-""" 创建角色 """
+""" 创建默认用户 """
 __version__ = '0.0.1'
 __history__ = """"""
 __all__ = []
 
 
+from django.contrib.auth import get_user_model
+from django.contrib.auth.hashers import make_password
 from django.db import migrations
 
-from rest_framework_admin.role.configs import DefaultRoleEnum, DEFAULT_ROLE_DATA
+from rest_framework_admin.user.configs import DefaultUserEnum
 
 
 def forwards_func(apps, schema_editor):
     # We get the model from the versioned app registry;
     # if we directly import it, it'll be the wrong version
-    Role = apps.get_model("admin_role", "Role")
+    # User = apps.get_model("user", "User")
+    User = get_user_model()
     db_alias = schema_editor.connection.alias
-    roles = []
-    for role_enum in DefaultRoleEnum:
-        data = role_enum.value._asdict()
-        data.update(DEFAULT_ROLE_DATA)
-        roles.append(Role(**data))
-    Role.objects.using(db_alias).bulk_create(roles)
+    users = []
+    for user_enum in DefaultUserEnum:
+        users.append(
+            User(
+                username=user_enum.name,
+                password=make_password(f"{user_enum.name}@2023"),
+                **user_enum.value._asdict()))
+    User.objects.using(db_alias).bulk_create(users)
 
 
 def reverse_func(apps, schema_editor):
-    Role = apps.get_model("admin_role", "Role")
+    # so reverse_func() should delete them.
+    # User = apps.get_model("user", "User")
+    User = get_user_model()
     db_alias = schema_editor.connection.alias
-    role_ids = [_.value.id for _ in DefaultRoleEnum]
-    Role.objects.using(db_alias).filter(id__in=role_ids).delete()
+    user_ids = [_.value.id for _ in DefaultUserEnum]
+    User.objects.using(db_alias).filter(id__in=user_ids).delete()
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('admin_role', '0001_initial'),
-        ('admin_user', '0002_create_user')
+        ('admin_user', '0001_initial')
     ]
 
     operations = [
         migrations.RunPython(forwards_func, reverse_func),
     ]
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0004_delete_useless_table.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tmp/role/0002_delete_useless_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('admin_role', '0003_create_user_role_rel'),
-        ('auth', '0012_alter_user_first_name_max_length'),
+        ('admin_role', '0001_initial'),
     ]
 
     operations = [
         # FIXME(fengdy): auth模块会发出信号，信号接收者会使用如下表
         # migrations.RunSQL('DROP TABLE IF EXISTS auth_group_permissions;'),
         # migrations.RunSQL('DROP TABLE IF EXISTS auth_group;'),
         # migrations.RunSQL('DROP TABLE IF EXISTS auth_permission;'),
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/permissions.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/permissions.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,44 +7,34 @@
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
 from rest_framework import permissions
 
 
-class PermissionModelPermission(permissions.BasePermission):
-    def has_permission(self, request, view):
-        return request.user.is_admin()
-
-    def has_object_permission(self, request, view, obj):
-        return request.user.is_admin()
-
-
 class RoleModelPermission(permissions.BasePermission):
     def has_permission(self, request, view):
-        if view.action in ('selection', ):
-            return True
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
     def has_object_permission(self, request, view, obj):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
 
-class RoleRelatedPermissionModelPermission(permissions.BasePermission):
+class RolePermissionRelModelPermission(permissions.BasePermission):
     def has_permission(self, request, view):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
     def has_object_permission(self, request, view, obj):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
 
-class RoleRelatedSubjectModelPermission(permissions.BasePermission):
+class RoleMemberRelModelPermission(permissions.BasePermission):
     def has_permission(self, request, view):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
     def has_object_permission(self, request, view, obj):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
 
 
-class SubjectListPermission(permissions.BasePermission):
+class MemberListPermission(permissions.BasePermission):
     def has_permission(self, request, view):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,156 +4,160 @@
 # DateTime:2023/11/17
 # Tool:PyCharm
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
+from django.contrib.auth import get_user_model
 from drf_spectacular.utils import extend_schema_field
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 
-from rest_framework_admin.role.configs import RoleTypeEnum, SubjectTypeEnum
+from rest_framework_admin.role.configs import RoleTypeEnum, MemberTypeEnum
 from rest_framework_admin.role.models import Permission
-from rest_framework_admin.role.models import Role, RoleSubjectRel, RolePermissionRel
-from rest_framework_admin.user.models import Group, User
+from rest_framework_admin.role.models import Role, RoleMemberRel, RolePermissionRel
+from rest_framework_admin.user.group.models import Group
 from rest_framework_admin.user.serializers import UserModelSerializer
 from rest_framework_util.serializers import BaseModelSerializer, RelatedUserModelSerializer, BaseSwitchModelSerializer, \
     BaseSelectionModelSerializer, BaseRelModelSerializer
 
 
-class PermissionModelSerializer(BaseModelSerializer):
-    class Meta(BaseModelSerializer.Meta):
-        model = Permission
-
-
 class RoleModelSerializer(BaseModelSerializer):
     type = serializers.ChoiceField(
         [RoleTypeEnum.custom.name])
     name = serializers.CharField(max_length=64)
     code = serializers.CharField(max_length=64)
-    subject_count = serializers.SerializerMethodField(help_text='主体个数统计')
+    member_count = serializers.SerializerMethodField(help_text='主体个数统计')
     weight = serializers.IntegerField(
         required=False,
         help_text='权重，值越高优先级越高，即权限越大',
         min_value=1,
         max_value=100)
 
     class Meta(BaseModelSerializer.Meta):
         model = Role
         fields = BaseModelSerializer.Meta.fields + \
-            ('code', 'subject_count', 'type', 'weight')
+            ('code', 'member_count', 'type', 'weight')
         validators = []
 
     @extend_schema_field({'type': 'object',
                           'properties': {'all': {'type': 'int',
                                                  'description': '所有主体个数'},
                                          '{key}': {'type': 'int',
                                                    'description': '个数,{key}为主体类型'}}})
-    def get_subject_count(self, obj):
-        data = {'all': obj.subject_rels.count()}
-        for enum in SubjectTypeEnum:
-            data[enum.name] = obj.subject_rels.filter(
-                subject_type=enum.name).count()
+    def get_member_count(self, obj):
+        data = {'all': obj.member_rels.count()}
+        for enum in MemberTypeEnum:
+            data[enum.name] = obj.member_rels.filter(
+                member_type=enum.name).count()
         return data
 
 
-class RelatedRoleSubjectRelModelSerializer(BaseRelModelSerializer):
+class RelatedRoleMemberRelModelSerializer(BaseRelModelSerializer):
     """ 关联的角色 """
     id = serializers.CharField(source='role_id', read_only=True)
     code = serializers.SlugRelatedField(
         source='role', slug_field='code', read_only=True)
     name = serializers.SlugRelatedField(
         source='role', slug_field='name', read_only=True)
     create_user = RelatedUserModelSerializer(help_text='绑定用户与角色的人员')
 
     class Meta(BaseRelModelSerializer.Meta):
-        model = RoleSubjectRel
+        model = RoleMemberRel
         fields = BaseRelModelSerializer.Meta.fields + ('code', 'name')
 
 
 class SwitchRoleModelSerializer(BaseSwitchModelSerializer):
 
     class Meta(BaseSwitchModelSerializer.Meta):
         model = Role
 
 
-class SelectionRoleModelSerializer(BaseSelectionModelSerializer):
+class SelectRoleModelSerializer(BaseSelectionModelSerializer):
     class Meta(BaseSelectionModelSerializer.Meta):
         model = Role
         fields = BaseSelectionModelSerializer.Meta.fields + ('type', )
 
 
-class RoleRelatedPermissionModelSerializer(BaseRelModelSerializer):
+class RolePermissionRelModelSerializer(BaseRelModelSerializer):
     id = serializers.CharField(source='permission_id')
     name = serializers.CharField(source='permission__name')
+
+    class Meta(BaseRelModelSerializer.Meta):
+        model = RolePermissionRel
+        fields = BaseRelModelSerializer.Meta.fields + ('id', 'name')
+
+
+class CreateRolePermissionRelModelSerializer(BaseRelModelSerializer):
     permission_ids = serializers.ListField(
         min_length=1,
         max_length=10,
         write_only=True,
         child=serializers.PrimaryKeyRelatedField(queryset=Permission.objects.all()))
 
-    class Meta(BaseRelModelSerializer.Meta):
+    class Meta:
         model = RolePermissionRel
-        fields = BaseRelModelSerializer.Meta.fields + ('permission_ids', )
+        fields = ('permission_ids', )
 
     def create(self, validated_data):
         for permission in validated_data.pop('permission_ids'):
-            if not RolePermissionRel.objects.filter(
+            if RolePermissionRel.objects.filter(
                     permission_id=permission.id,
                     role_id=validated_data['role_id']).exists():
-                validated_data['permission_id'] = permission.id
-                instance = super().create(validated_data)
+                raise ValidationError(_(f'权限【{permission.name}】已关联'))
+            validated_data['permission_id'] = permission.id
+            instance = super().create(validated_data)
         return instance
 
 
-class RoleRelatedSubjectModelSerializer(BaseRelModelSerializer):
-    id = serializers.CharField(source='subject_id')
+class RoleMemberRelModelSerializer(BaseRelModelSerializer):
+    id = serializers.CharField(source='member_id')
     type = serializers.ChoiceField(
-        [enum.name for enum in SubjectTypeEnum], source='subject_type')
+        [enum.name for enum in MemberTypeEnum], source='member_type')
     name = serializers.SerializerMethodField()
-    subject_ids = serializers.ListField(
+    member_ids = serializers.ListField(
         min_length=1,
         max_length=10,
         write_only=True,
         child=serializers.CharField(max_length=32, min_length=32))
 
     class Meta(BaseRelModelSerializer.Meta):
-        model = RoleSubjectRel
-        fields = BaseRelModelSerializer.Meta.fields + ('subject_ids', )
+        model = RoleMemberRel
+        fields = BaseRelModelSerializer.Meta.fields + ('member_ids', )
 
     def get_name(self, obj):
-        return obj.subject.name
+        return obj.member.name
 
     def create(self, validated_data):
-        subject_type = validated_data['type']
-        for subject_id in validated_data.pop('subject_ids'):
-            if subject_type == SubjectTypeEnum.user_group.name:
-                enum = SubjectTypeEnum.user_group
+        member_type = validated_data['type']
+        for member_id in validated_data.pop('member_ids'):
+            if member_type == MemberTypeEnum.group.name:
+                enum = MemberTypeEnum.group
                 model = Group
             else:
-                enum = SubjectTypeEnum.user
-                model = User
-            if not model.objects.filter(pk=subject_id).exists():
+                enum = MemberTypeEnum.user
+                model = get_user_model()
+            if not model.objects.filter(pk=member_id).exists():
                 raise ValidationError(
-                    _(f'[{enum.value}]类型实体[id={subject_id}]不存在'))
-            if not RoleSubjectRel.objects.filter(
-                    subject_id=subject_id,
-                    subject_type=subject_type,
+                    _(f'[{enum.value}]类型实体[id={member_id}]不存在'))
+            if not RoleMemberRel.objects.filter(
+                    member_id=member_id,
+                    member_type=member_type,
                     role_id=validated_data['role_id']).exists():
-                validated_data['subject_id'] = subject_id
+                validated_data['member_id'] = member_id
                 instance = super().create(validated_data)
         return instance
 
 
 # ========== 主体 ==========
 
 
-class SubjectListSerializer(serializers.Serializer):
+class MemberListSerializer(serializers.Serializer):
     id = serializers.CharField()
     description = serializers.CharField()
     is_active = serializers.BooleanField()
     type = serializers.CharField()
     create_ts = serializers.SerializerMethodField()
     #
     username = serializers.SerializerMethodField()
@@ -186,16 +190,16 @@
             'description',
             'user_count',
             'create_ts']))
 
     def __get_obj(self, obj):
         key = '_obj_instance__'
         if key not in obj:
-            if obj["type"] == SubjectTypeEnum.user.name:
-                model = User
+            if obj["type"] == MemberTypeEnum.user.name:
+                model = get_user_model()
             else:
                 model = Group
             obj[key] = model.objects.get(pk=obj["id"])
         return obj[key]
 
     def get_create_ts(self, obj):
         instance = self.__get_obj(obj)
@@ -227,10 +231,10 @@
 
     def get_expire_ts(self, obj):
         instance = self.__get_obj(obj)
         return getattr(instance, 'expire_ts', None)
 
     def get_role(self, obj):
         instance = self.__get_obj(obj)
-        if obj['type'] == SubjectTypeEnum.user.name:
+        if obj['type'] == MemberTypeEnum.user.name:
             return UserModelSerializer(context=self.context).get_role(instance)
         return None
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/services.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/services.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/python
 # -*- coding:utf-8 -*-
 # Email:iamfengdy@126.com
 # DateTime:2024/3/6
-from rest_framework_admin.role.configs import SubjectTypeEnum
-from rest_framework_admin.role.models import Role, RoleSubjectRel
+from rest_framework_admin.role.configs import MemberTypeEnum
+from rest_framework_admin.role.models import Role, RoleMemberRel
 from rest_framework_util.services import BaseService
 
 
 class UserService(BaseService):
     """ 用户角色服务 """
 
     def filter_roles(self, is_valid=None):
         """ 过滤直接绑定的角色 """
-        return Role.filter_by_subject(
-            self.id, SubjectTypeEnum.user.name, is_valid=is_valid)
+        return Role.filter_by_member(
+            self.id, MemberTypeEnum.user.name, is_valid=is_valid)
 
     def save_roles(self, role_ids, **kwargs):
-        RoleSubjectRel.save_by_subject(
-            self.id, role_ids, SubjectTypeEnum.user.name, **kwargs)
+        RoleMemberRel.save_by_member(
+            self.id, role_ids, MemberTypeEnum.user.name, **kwargs)
 
     def delete_roles(self, role_ids):
-        RoleSubjectRel.delete_by_subject(
-            self.id, role_ids, SubjectTypeEnum.user.name)
+        RoleMemberRel.delete_by_member(
+            self.id, role_ids, MemberTypeEnum.user.name)
 
     def filter_group_roles(self, is_valid=None):
         """ 过滤通过组绑定的角色 """
         queryset = Role.objects.none()
         for group in self.groups.all():
             queryset = queryset | group.filter_roles(is_valid=is_valid)
         return queryset
@@ -43,27 +43,27 @@
         return queryset
 
     def get_max_role_rel(self):
         """ 获取最大的角色rel """
         role = self.filter_all_roles(is_valid=True).order_by('-weight').first()
         if not role:
             return None
-        rel = RoleSubjectRel.objects.get(
-            subject_id=role.subject_id,
-            subject_type=SubjectTypeEnum.user.name,
+        rel = RoleMemberRel.objects.get(
+            member_id=role.member_id,
+            member_type=MemberTypeEnum.user.name,
             role_id=role.id)
         return rel
 
 
 class UserGroupService(BaseService):
     def filter_roles(self, is_valid=None):
         """ 过滤直接绑定的角色 """
-        return Role.filter_by_subject(
-            self.id, SubjectTypeEnum.user_group.name, is_valid=is_valid)
+        return Role.filter_by_member(
+            self.id, MemberTypeEnum.group.name, is_valid=is_valid)
 
     def save_roles(self, role_ids, **kwargs):
-        RoleSubjectRel.save_by_subject(
-            self.id, role_ids, SubjectTypeEnum.user_group.name, **kwargs)
+        RoleMemberRel.save_by_member(
+            self.id, role_ids, MemberTypeEnum.group.name, **kwargs)
 
     def delete_roles(self, role_ids):
-        RoleSubjectRel.delete_by_subject(
-            self.id, role_ids, SubjectTypeEnum.user_group.name)
+        RoleMemberRel.delete_by_member(
+            self.id, role_ids, MemberTypeEnum.group.name)
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/settings.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,42 +9,38 @@
 __history__ = """"""
 __all__ = ['urlpatterns']
 
 from django.urls import path, include, re_path
 from rest_framework import routers
 
 from rest_framework_admin.role import views
-
-
-permission_router = routers.DefaultRouter()
-permission_router.register(r'^permissions', views.PermissionViewSet)
-
+from rest_framework_admin.role.permission.urls import urlpatterns as permission_urlpatterns
+from rest_framework_util.routers import RelDefaultRouter
 
 role_router = routers.DefaultRouter()
 role_router.register(r'^roles', views.RoleModelViewSet)
 
-role_related_permission_router = routers.DefaultRouter()
-role_related_permission_router.register(
+role_permission_rel_router = RelDefaultRouter()
+role_permission_rel_router.register(
     r'^permissions',
-    views.RoleRelatedPermissionModelViewSet,
-    basename='role_related_permission_router')
+    views.RolePermissionRelModelViewSet,
+    basename='role_permission_rel_router')
 
-role_related_subject_router = routers.DefaultRouter()
-role_related_subject_router.register(
-    r'^subjects',
-    views.RoleRelatedSubjectModelViewSet,
-    basename='role_related_subject_router')
+role_member_rel_router = RelDefaultRouter()
+role_member_rel_router.register(
+    r'^members',
+    views.RoleMemberRelModelViewSet,
+    basename='role_member_rel_router')
 
 
 urlpatterns = [
-    path(r'', include(permission_router.urls)),
     path(r'', include(role_router.urls)),
     re_path(
         r'roles/(?P<role_id>[a-z0-9A-Z\-]{32})/',
         include(
-            role_related_permission_router.urls)),
+            role_permission_rel_router.urls)),
     re_path(
         r'roles/(?P<role_id>[a-z0-9A-Z\-]{32})/',
         include(
-            role_related_subject_router.urls)),
-    re_path(r'^subjects/$', views.SubjectListAPIView.as_view()),
-]
+            role_member_rel_router.urls)),
+    re_path(r'^members/$', views.MemberListAPIView.as_view()),
+] + permission_urlpatterns
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/role/views.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,110 @@
+from django.contrib.auth import get_user_model
 from django.db.models import F, Value, CharField, Q
 
 # Create your views here.
 from drf_spectacular.utils import extend_schema_view, extend_schema
 from rest_framework import viewsets
 from rest_framework.generics import ListAPIView
 
-from rest_framework_admin.role.configs import SubjectTypeEnum
 from rest_framework_admin.role import serializers
-from rest_framework_admin.role.filters import RoleFilter, RoleRelatedPermissionFilter, RoleRelatedSubjectFilter, \
-    PermissionFilter
-from rest_framework_admin.role.models import Role, RolePermissionRel, RoleSubjectRel, Permission
-from rest_framework_admin.role.permissions import RoleModelPermission, RoleRelatedPermissionModelPermission, \
-    RoleRelatedSubjectModelPermission, SubjectListPermission, PermissionModelPermission
-from rest_framework_admin.role.serializers import PermissionModelSerializer
-from rest_framework_admin.user.models import User, Group
+from rest_framework_admin.role.configs import MemberTypeEnum
+from rest_framework_admin.role.filters import RoleFilter, RolePermissionRelFilter, RoleMemberRelFilter
+from rest_framework_admin.role.models import Role, RolePermissionRel, RoleMemberRel
+from rest_framework_admin.role.permissions import RoleModelPermission, RolePermissionRelModelPermission, \
+    RoleMemberRelModelPermission, MemberListPermission
+from rest_framework_admin.user.group.models import Group
 from rest_framework_util.exceptions import HTTP403
 from rest_framework_util.viewsets import BaseModeViewSet, BaseRelModelViewSet
 
 
-@extend_schema_view()
-class PermissionViewSet(viewsets.ReadOnlyModelViewSet):
-    """ 权限 """
-    queryset = Permission.objects.filter().order_by('-create_datetime').all()
-    serializer_class = PermissionModelSerializer
-    filterset_class = PermissionFilter
-    search_fields = ['name']
-    ordering_fields = ['name', 'create_datetime']
-    permission_classes = (PermissionModelPermission, )
-
-    def perform_create(self, serializer):
-        serializer.save(create_user_id=self.request.user.id)
-
-
 @extend_schema_view(
-    switch=extend_schema(summary='启用、禁用')
+    list=extend_schema(summary='搜索角色'),
+    create=extend_schema(summary='增加角色'),
+    retrieve=extend_schema(summary='查询角色'),
+    partial_update=extend_schema(summary='更新角色'),
+    destroy=extend_schema(summary='删除角色'),
+    switch=extend_schema(summary='启用、禁用'),
+    select=extend_schema(summary='搜索选择列表')
 )
 class RoleModelViewSet(BaseModeViewSet):
-    """ 角色 """
+    """ 角色管理 """
     queryset = Role.objects.filter().order_by('-create_datetime').all()
     serializer_class = serializers.RoleModelSerializer
     serializer_module = serializers
     filterset_class = RoleFilter
     search_fields = ['name', 'code']
     ordering_fields = ['name', 'create_datetime']
     permission_classes = (RoleModelPermission, )
 
     def perform_destroy(self, instance):
-        if instance.subject_rels.exists():
-            raise HTTP403('存在关联主体，不允许删除')
-        if instance.permissions.exists():
-            raise HTTP403('存在关联权限，不允许删除')
         instance.delete(delete_user_id=self.request.user.id)
 
 
-@extend_schema_view()
-class RoleRelatedPermissionModelViewSet(BaseRelModelViewSet):
+@extend_schema_view(
+    list=extend_schema(summary='搜索权限'),
+    create=extend_schema(summary='批量增加权限'),
+    update=extend_schema(summary='全量更新权限'),
+    destroy=extend_schema(summary='批量删除权限'),
+)
+class RolePermissionRelModelViewSet(BaseRelModelViewSet):
     """ 角色关联的权限管理 """
     parent_model = Role
     lookup_field = 'permission_id'
     queryset = RolePermissionRel.objects.all()
-    serializer_class = serializers.RoleRelatedPermissionModelSerializer
-    filterset_class = RoleRelatedPermissionFilter
+    serializer_class = serializers.RolePermissionRelModelSerializer
+    filterset_class = RolePermissionRelFilter
     search_fields = ['permission__name', 'permission__description']
     ordering_fields = [
         'create_datetime',
         'permission__name',
         'permission__create_datetime']
     ordering = ['-create_datetime']
-    permission_classes = (RoleRelatedPermissionModelPermission, )
+    permission_classes = (RolePermissionRelModelPermission, )
 
 
-@extend_schema_view()
-class RoleRelatedSubjectModelViewSet(BaseRelModelViewSet):
-    """ 角色关联的实体管理 """
+@extend_schema_view(
+    list=extend_schema(summary='搜索成员'),
+    create=extend_schema(summary='批量增加成员'),
+    update=extend_schema(summary='全量更新成员'),
+    destroy=extend_schema(summary='批量删除成员'),
+)
+class RoleMemberRelModelViewSet(BaseRelModelViewSet):
+    """ 角色关联的成员管理 """
     parent_model = Role
-    lookup_field = 'subject_id'
-    queryset = RoleSubjectRel.objects.all()
-    serializer_class = serializers.RoleRelatedPermissionModelSerializer
-    filterset_class = RoleRelatedSubjectFilter
+    lookup_field = 'member_id'
+    queryset = RoleMemberRel.objects.all()
+    serializer_class = serializers.RoleMemberRelModelSerializer
+    filterset_class = RoleMemberRelFilter
     search_fields = []
     ordering_fields = [
         'create_datetime',
         'type']
     ordering = ['-create_datetime']
-    permission_classes = (RoleRelatedSubjectModelPermission, )
+    permission_classes = (RoleMemberRelModelPermission, )
 
 
-@extend_schema_view()
-class SubjectListAPIView(ListAPIView):
-    """ 角色主体列表 """
-    serializer_class = serializers.SubjectListSerializer
+@extend_schema_view(
+    get=extend_schema(summary='搜索可赋予角色的成员列表'),
+)
+class MemberListAPIView(ListAPIView):
+    """ 成员列表 """
+    serializer_class = serializers.MemberListSerializer
     filterset_class = None
     search_fields = []
     ordering_fields = ['name', 'type']
     ordering = ['name']
-    permission_classes = (SubjectListPermission,)
+    permission_classes = (MemberListPermission,)
 
     def get_queryset(self):
-        user_queryset = User.objects.filter(is_active=True).annotate(
-            name=F('username')).annotate(type=Value(SubjectTypeEnum.user.name, output_field=CharField(max_length=8)))
+        user_queryset = get_user_model().objects.filter(is_active=True).annotate(
+            name=F('username')).annotate(type=Value(MemberTypeEnum.user.name, output_field=CharField(max_length=8)))
         group_queryset = Group.objects.filter(is_active=True).annotate(
             type=Value(
-                SubjectTypeEnum.user_group.name,
+                MemberTypeEnum.group.name,
                 output_field=CharField(
                     max_length=8)))
         name = self.request.query_params.get('name', None) or None
         if not name:
             name = self.request.query_params.get('search', None) or None
         if name is not None:
             user_queryset = user_queryset.filter(Q(realname__icontains=name) | Q(
@@ -117,16 +116,16 @@
             'is_active',
             'description',
             'create_datetime',
             'name',
             'type']
         user_queryset = user_queryset.values(*keys)
         group_queryset = group_queryset.values(*keys)
-        subject_type = self.request.query_params.get('type', None) or None
-        if subject_type == SubjectTypeEnum.user.name:
+        member_type = self.request.query_params.get('type', None) or None
+        if member_type == MemberTypeEnum.user.name:
             return user_queryset
-        elif subject_type == SubjectTypeEnum.user_group.name:
+        elif member_type == MemberTypeEnum.group.name:
             return group_queryset
         else:
             queryset = user_queryset.union(
                 group_queryset, all=True)
         return queryset
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/system/permissions.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/system/permissions.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 from rest_framework import permissions
 
 
 class ConfigPermission(permissions.BasePermission):
     def has_permission(self, request, view):
         if view.action in ('selection',):
             return True
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner()
 
     def has_object_permission(self, request, view, obj):
-        return request.user.is_admin()
+        return request.user.is_admin_or_owner()
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/system/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/system/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/system/settings.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/system/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/system/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/system/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/system/views.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/system/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/filters.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name = filters.CharFilter(lookup_expr='icontains')
 
     class Meta:
         model = Tenant
         fields = ['name']
 
 
-class TenantRelatedUserFilter(filters.FilterSet):
+class TenantUserRelFilter(filters.FilterSet):
     id = filters.CharFilter(field_name='user_id')
 
     name = filters.CharFilter(
         lookup_expr='icontains',
         field_name='user__username')
 
     class Meta:
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0001_initial.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.13 on 2024-03-31 08:16
+# Generated by Django 4.1.13 on 2024-04-15 08:53
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import shortcut_util.unique
 
 
@@ -74,15 +74,15 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "租户表",
-                "db_table": "admin_tenant",
+                "db_table": "tenant",
             },
         ),
         migrations.CreateModel(
             name="TenantUserRel",
             fields=[
                 (
                     "id",
@@ -108,14 +108,21 @@
                     models.CharField(blank=True, max_length=256, verbose_name="描述"),
                 ),
                 (
                     "delete_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="删除时间"),
                 ),
                 (
+                    "role",
+                    models.CharField(
+                        choices=[("owner", "创建者"), ("admin", "管理员"), ("member", "成员")],
+                        max_length=32,
+                    ),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -152,15 +159,15 @@
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "租户用户关联表",
-                "db_table": "admin_tenant_user_rel",
+                "db_table": "tenant_user_rel",
                 "unique_together": {("user", "tenant", "delete_datetime")},
             },
         ),
         migrations.AddField(
             model_name="tenant",
             name="user_rels",
             field=models.ManyToManyField(
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0002_create_role.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/auth/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 #!/usr/bin/python
 # -*- coding:utf-8 -*-
 # Email:iamfengdy@126.com
-# DateTime:2023/11/21
+# DateTime:2024/1/2
 # Tool:PyCharm
 
-""" 创建角色 """
+"""  """
 __version__ = '0.0.1'
 __history__ = """"""
 __all__ = []
 
-
-from django.db import migrations
-
-from rest_framework_admin.tenant.configs import DefaultRoleEnum, DEFAULT_ROLE_DATA
-
-
-def forwards_func(apps, schema_editor):
-    # We get the model from the versioned app registry;
-    # if we directly import it, it'll be the wrong version
-    Role = apps.get_model("admin_role", "Role")
-    db_alias = schema_editor.connection.alias
-    roles = []
-    for role_enum in DefaultRoleEnum:
-        data = role_enum.value._asdict()
-        data.update(DEFAULT_ROLE_DATA)
-        roles.append(Role(**data))
-    Role.objects.using(db_alias).bulk_create(roles)
-
-
-def reverse_func(apps, schema_editor):
-    Role = apps.get_model("admin_role", "Role")
-    db_alias = schema_editor.connection.alias
-    role_ids = [_.value.id for _ in DefaultRoleEnum]
-    Role.objects.using(db_alias).filter(id__in=role_ids).delete()
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('admin_tenant', '0001_initial'),
-        ('admin_role', '0002_create_role'),
-    ]
-
-    operations = [
-        migrations.RunPython(forwards_func, reverse_func),
-    ]
+from django.core.mail import send_mail
+from drf_spectacular.utils import extend_schema_view, extend_schema
+from rest_framework.generics import RetrieveAPIView, CreateAPIView
+
+from rest_framework_admin import logger
+from rest_framework_admin.auth.serializers import AuthMeUserModelSerializer, RegisterUserModelSerializer
+
+
+@extend_schema_view(
+    get=extend_schema(summary='用户自查')
+)
+class AuthMeRetrieveAPIView(RetrieveAPIView):
+    serializer_class = AuthMeUserModelSerializer
+
+    def get_object(self):
+        return self.request.user
+
+
+@extend_schema_view(
+    post=extend_schema(summary='用户注册')
+)
+class AuthRegisterCreateAPIView(CreateAPIView):
+    serializer_class = RegisterUserModelSerializer
+
+    def perform_create(self, serializer):
+        instance = serializer.save()
+        try:
+            send_mail(
+                '【Admin】注册成功',
+                f'您的账户名为{instance.username}，默认密码为，请登录更改密码！',
+                None,
+                [instance.email])
+        except BaseException:
+            logger.exception(
+                f'cannot send email to registered user. email={instance.email}')
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/models.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from django.contrib.auth import get_user_model
 from django.db import models
 
+from rest_framework_admin.user.models import BaseUserRel
 from rest_framework_util.db.models.base import BaseModel, BaseRelModel
 
 
 # Create your models here.
 class Tenant(BaseModel):
     code = models.CharField('编码', max_length=64)
     config = models.JSONField('配置')
 
     user_rels = models.ManyToManyField(
         get_user_model(), through='TenantUserRel', through_fields=(
             'tenant', 'user'), related_name='tenant_rels')
 
     class Meta:
-        db_table = 'admin_tenant'
+        db_table = 'tenant'
         verbose_name = '租户表'
 
     def extended_strs(self):
         return [f'code={self.code}']
 
     @property
     def user_count(self):
         return self.user_rels.count()
 
 
-class TenantUserRel(BaseRelModel):
-    user = models.ForeignKey(get_user_model(), models.CASCADE)
+class TenantUserRel(BaseUserRel):
     tenant = models.ForeignKey(Tenant, models.CASCADE)
 
     class Meta:
-        db_table = 'admin_tenant_user_rel'
+        db_table = 'tenant_user_rel'
         verbose_name = '租户用户关联表'
         unique_together = ('user', 'tenant', 'delete_datetime')
 
     def extended_strs(self):
         return [f'tenant_id={self.tenant.id})', f'user_id={self.user.id}']
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # Tool:PyCharm
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
 from rest_framework import serializers
+from rest_framework.exceptions import ValidationError
 from rest_framework.validators import UniqueValidator
+from django.utils.translation import gettext_lazy as _
 
-from rest_framework_admin.role.configs import SubjectTypeEnum
-from rest_framework_admin.role.models import RoleSubjectRel, Role
-from rest_framework_admin.tenant.configs import DefaultRoleEnum
+from rest_framework_admin.user.configs import MemberRoleEnum
 from rest_framework_admin.user.models import User
 from rest_framework_util.serializers import (
     BaseSwitchModelSerializer,
     BaseModelSerializer,
     BaseRelatedModelSerializer,
     BaseSelectionModelSerializer,
     BaseRelModelSerializer)
@@ -37,46 +37,39 @@
             ('user_count', 'config')
 
     def create(self, validated_data):
         instance = super().create(validated_data)
         rel = TenantUserRel(
             user=instance.create_user,
             tenant=instance,
-            create_user=instance.create_user
+            create_user=instance.create_user,
+            role=MemberRoleEnum.owner.name
         )
         rel.save()
-        role_rel = RoleSubjectRel(
-            subject_id=instance.create_user.id,
-            subject_type=SubjectTypeEnum.user.name,
-            role=Role.objects.get(id=DefaultRoleEnum.owner.value.id),
-            scope_id=instance.id,
-            create_user=instance.create_user
-        )
-        role_rel.save()
         return instance
 
 
 class RelatedTenantModelSerializer(BaseRelatedModelSerializer):
     class Meta(BaseRelatedModelSerializer.Meta):
         model = Tenant
 
 
 class SwitchTenantModelSerializer(BaseSwitchModelSerializer):
 
     class Meta(BaseSwitchModelSerializer.Meta):
         model = Tenant
 
 
-class SelectionTenantModelSerializer(BaseSelectionModelSerializer):
+class SelectTenantModelSerializer(BaseSelectionModelSerializer):
 
     class Meta(BaseSelectionModelSerializer.Meta):
         model = Tenant
 
 
-class TenantRelatedUserModelSerializer(BaseRelModelSerializer):
+class TenantUserRelModelSerializer(BaseRelModelSerializer):
     id = serializers.CharField(source='user_id', read_only=True)
     name = serializers.CharField(source='user__username', read_only=True)
     user_ids = serializers.ListField(
         min_length=1,
         max_length=10,
         write_only=True,
         child=serializers.PrimaryKeyRelatedField(queryset=User.objects.all()))
@@ -91,7 +84,24 @@
             instance = TenantUserRel.objects.filter(
                 user_id=user.id,
                 tenant_id=validated_data['tenant_id']).first()
             if instance is None:
                 validated_data['user_id'] = user.id
                 instance = super().create(validated_data)
         return instance
+
+
+class DestroyTenantUserRelModelSerializer(serializers.Serializer):
+    user_ids = serializers.ListField(
+        min_length=1,
+        max_length=10,
+        write_only=True,
+        child=serializers.PrimaryKeyRelatedField(queryset=User.objects.all()))
+
+    def validate_user_ids(self, users):
+        user_ids = []
+        tenant = self.context['view'].get_parent_object()
+        for user in users:
+            if tenant.user_rels.filter(user_id=user.id).exists():
+                raise ValidationError(_(f'用户【{user.name}】未加入空间'))
+            user_ids.append(user.id)
+        return user_ids
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 __history__ = """"""
 __all__ = ['urlpatterns']
 
 from django.urls import path, include, re_path
 from rest_framework import routers
 
 from rest_framework_admin.tenant import views
+from rest_framework_util.routers import RelDefaultRouter
 
 tenant_router = routers.DefaultRouter()
 tenant_router.register(r'^tenants', views.TenantModelViewSet)
 
-tenant_related_user_router = routers.DefaultRouter()
-tenant_related_user_router.register(
+tenant_user_rel_router = RelDefaultRouter()
+tenant_user_rel_router.register(
     r'^users',
-    views.TenantRelatedUserModelViewSet,
-    basename='tenant_related_user_router')
+    views.TenantUserRelModelViewSet,
+    basename='tenant_user_rel_router')
 
 
 urlpatterns = [
     path(r'', include(tenant_router.urls)),
     re_path(
         r'tenants/(?P<tenant_id>[a-z0-9A-Z\-]{32})/',
         include(
-            tenant_related_user_router.urls)),
+            tenant_user_rel_router.urls)),
 ]
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/tenant/views.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/tenant/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Create your views here.
 from drf_spectacular.utils import extend_schema_view, extend_schema
 from django.utils.translation import gettext_lazy as _
+from rest_framework import mixins
 from rest_framework.decorators import action
 from rest_framework.response import Response
 
 from rest_framework_admin.tenant import serializers
-from rest_framework_admin.tenant.filters import TenantFilter, TenantRelatedUserFilter
+from rest_framework_admin.tenant.filters import TenantFilter, TenantUserRelFilter
 from rest_framework_admin.tenant.models import Tenant, TenantUserRel
-from rest_framework_admin.tenant.permissions import TenantModelPermission, TenantRelatedUserModelPermission
+from rest_framework_admin.tenant.permissions import TenantModelPermission, TenantUserRelModelPermission
 from rest_framework_admin.tenant.serializers import TenantModelSerializer
 from rest_framework_util.exceptions import HTTP403
-from rest_framework_util.viewsets import BaseModeViewSet, BaseRelModelViewSet
+from rest_framework_util.mixins import CreateRelModelMixin, DestroyRelModelMixin
+from rest_framework_util.viewsets import BaseModeViewSet, BaseRelModelViewSet, GenericRelViewSet
 
 
 @extend_schema_view(
     switch=extend_schema(summary='启用、禁用'),
 )
 class TenantModelViewSet(BaseModeViewSet):
     """ 租户管理 """
@@ -23,27 +25,32 @@
     serializer_module = serializers
     filterset_class = TenantFilter
     search_fields = ['id', 'name']
     ordering_fields = ['name', 'create_datetime']
     permission_classes = (TenantModelPermission,)
 
     def perform_destroy(self, instance):
-        if instance.user_rels.exists():
-            raise HTTP403(_('存在关联用户，不允许删除'))
         instance.delete(delete_user_id=self.request.user.id)
 
 
-@extend_schema_view()
-class TenantRelatedUserModelViewSet(BaseRelModelViewSet):
+@extend_schema_view(
+    list=extend_schema(summary='搜索用户'),
+    create=extend_schema(summary='批量增加用户'),
+    destroy=extend_schema(summary='批量删除用户'),
+)
+class TenantUserRelModelViewSet(mixins.ListModelMixin,
+                                CreateRelModelMixin,
+                                DestroyRelModelMixin,
+                                GenericRelViewSet):
     """ 关联的用户管理 """
     parent_model = Tenant
     lookup_field = 'user_id'
     queryset = TenantUserRel.objects.all()
-    serializer_class = serializers.TenantRelatedUserModelSerializer
-    filterset_class = TenantRelatedUserFilter
+    serializer_class = serializers.TenantUserRelModelSerializer
+    filterset_class = TenantUserRelFilter
     search_fields = ['user__username', 'user__nickname']
     ordering_fields = [
         'create_datetime',
         'user__username',
         'user__create_datetime']
     ordering = ['-create_datetime']
-    permission_classes = (TenantRelatedUserModelPermission,)
+    permission_classes = (TenantUserRelModelPermission,)
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/filters.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
 from django_filters import rest_framework as filters
 
-from rest_framework_admin.user.models import User, UserGroupRel
+from rest_framework_admin.user.models import User, GroupUserRel
 
 
 class UserFilter(filters.FilterSet):
     is_active = filters.BooleanFilter()
 
     class Meta:
         model = User
         fields = ['is_active']
 
 
-class UserRelatedGroupFilter(filters.FilterSet):
+class GroupUserRelFilter(filters.FilterSet):
     id = filters.CharFilter(field_name='group_id')
 
     name = filters.CharFilter(
         lookup_expr='icontains',
         field_name='group__name')
 
     class Meta:
-        model = UserGroupRel
+        model = GroupUserRel
         fields = ['id', 'name']
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/filters.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/group/filters.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,23 @@
 # Tool:PyCharm
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 
 from django_filters import rest_framework as filters
+from rest_framework_admin.group.filters import BaseGroupFilter
+from rest_framework_admin.user.group.models import Group, GroupUserRel
 
-from rest_framework_admin.user.models import Group, UserGroupRel
 
+class GroupFilter(BaseGroupFilter):
 
-class GroupFilter(filters.FilterSet):
-    name = filters.CharFilter(lookup_expr='icontains')
-
-    class Meta:
+    class Meta(BaseGroupFilter.Meta):
         model = Group
-        fields = ['name']
 
 
-class GroupRelatedUserFilter(filters.FilterSet):
-    id = filters.CharFilter(field_name='user_id')
-
-    name = filters.CharFilter(
-        lookup_expr='icontains',
-        field_name='user__username')
+class GroupUserRelFilter(filters.FilterSet):
+    name = filters.CharFilter(field_name='user__name', lookup_expr='icontains')
 
     class Meta:
-        model = UserGroupRel
-        fields = ['id', 'name']
+        model = GroupUserRel
+        fields = ['name']
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/models.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/group/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,46 @@
 # -*- coding:utf-8 -*-
 # Email:iamfengdy@126.com
 # DateTime:2023/11/16
 # Tool:PyCharm
 from django.contrib.auth import get_user_model
 from django.db import models
 
-
+from rest_framework_admin.user.configs import MemberRoleEnum
 from rest_framework_util.db.models.base import BaseModel, BaseRelModel
 
 
 class Group(BaseModel):
-    user_rels = models.ManyToManyField(
-        get_user_model(), through='UserGroupRel', through_fields=(
-            'group', 'user'), related_name='group_rels')
+    users = models.ManyToManyField(
+        get_user_model(), through='GroupUserRel', through_fields=(
+            'group', 'user'), related_name='groups')
     expire_datetime = models.DateTimeField('过期时间', blank=True, null=True)
 
     class Meta:
-        db_table = 'admin_user_group'
+        db_table = 'user_group'
         verbose_name = '用户组表'
 
     @property
     def user_count(self):
         return self.user_rels.count()
 
 
-class UserGroupRel(BaseRelModel):
-    user = models.ForeignKey(get_user_model(), models.CASCADE)
-    group = models.ForeignKey(Group, models.CASCADE)
+class GroupUserRel(BaseRelModel):
+    user = models.ForeignKey(
+        get_user_model(),
+        models.CASCADE,
+        related_name='group_rel')
+    group = models.ForeignKey(Group, models.CASCADE, related_name='user_rel')
+    role = models.CharField(
+        max_length=32,
+        choices=[
+            (_.name,
+             _.value) for _ in MemberRoleEnum],
+        default=MemberRoleEnum.member.name)
 
     class Meta:
-        db_table = 'admin_user_group_rel'
+        db_table = 'user_group_user_rel'
         verbose_name = '用户组关联表'
         unique_together = ('user', 'group', 'delete_datetime')
 
     def extended_strs(self):
         return [f'user_id={self.user.id}', f'group_id={self.group.id})']
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/group/serializers.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,83 +3,123 @@
 # Email:iamfengdy@126.com
 # DateTime:2023/11/17
 # Tool:PyCharm
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
-
+from django.utils.translation import gettext_lazy as _
 from drf_spectacular.types import OpenApiTypes
 from drf_spectacular.utils import extend_schema_field
 from rest_framework import serializers
+from rest_framework.exceptions import ValidationError
 from rest_framework.validators import UniqueValidator
 
-from rest_framework_admin.user.models import User, Group, UserGroupRel
+from rest_framework_admin.group.serializers import BaseGroupModelSerializer
+from rest_framework_admin.user.configs import MemberRoleEnum
+from rest_framework_admin.user.group.models import Group, GroupUserRel
+from rest_framework_admin.user.models import User
 from rest_framework_util.serializers import (
     BaseSwitchModelSerializer,
     BaseModelSerializer,
     BaseRelatedModelSerializer,
     BaseSelectionModelSerializer,
     BaseRelModelSerializer)
 
 
-class GroupModelSerializer(BaseModelSerializer, serializers.ModelSerializer):
+class GroupModelSerializer(BaseGroupModelSerializer):
     name = serializers.CharField(
         max_length=64, validators=[
             UniqueValidator(
                 queryset=Group.objects.filter())])
     user_count = serializers.IntegerField(
         help_text='用户个数', read_only=True)
-    expire_ts = serializers.SerializerMethodField()
-    expire_datetime = serializers.DateTimeField(
-        input_formats='%Y%m%d%H%M', required=False)
 
-    class Meta(BaseModelSerializer.Meta):
+    class Meta(BaseGroupModelSerializer.Meta):
         model = Group
-        fields = BaseModelSerializer.Meta.fields + \
-            ('user_count', 'expire_datetime', 'expire_ts')
-
-    @extend_schema_field(OpenApiTypes.INT)
-    def get_expire_ts(self, obj):
-        return self.get_ts_by_field(obj, 'expire_datetime')
+        fields = BaseGroupModelSerializer.Meta.fields + \
+            ('user_count', )
 
 
 class RelatedGroupModelSerializer(BaseRelatedModelSerializer):
     class Meta(BaseRelatedModelSerializer.Meta):
-        model = Group
+        model = GroupUserRel
 
 
 class SwitchGroupModelSerializer(BaseSwitchModelSerializer):
 
     class Meta(BaseSwitchModelSerializer.Meta):
-        model = Group
+        model = GroupUserRel
 
 
-class SelectionGroupModelSerializer(BaseSelectionModelSerializer):
+class SelectGroupModelSerializer(BaseSelectionModelSerializer):
 
     class Meta(BaseSelectionModelSerializer.Meta):
-        model = Group
+        model = GroupUserRel
 
 
-class GroupRelatedUserModelSerializer(BaseRelModelSerializer):
+class GroupUserRelModelSerializer(BaseRelModelSerializer):
     id = serializers.CharField(source='user_id', read_only=True)
     name = serializers.CharField(source='user__username', read_only=True)
+    role = serializers.ChoiceField(
+        choices=[
+            MemberRoleEnum.admin.name,
+            MemberRoleEnum.member.name],
+        read_only=True)
+
+    class Meta(BaseModelSerializer.Meta):
+        model = GroupUserRel
+        fields = BaseModelSerializer.Meta.fields + ('role', )
+        read_only_fields = fields
+
+
+class CreateGroupUserRelModelSerializer(BaseRelModelSerializer):
     user_ids = serializers.ListField(
         min_length=1,
         max_length=10,
         write_only=True,
-        child=serializers.PrimaryKeyRelatedField(queryset=User.objects.all()))
+        child=serializers.PrimaryKeyRelatedField(
+            queryset=User.objects.filter(
+                role__in=[_.name for _ in MemberRoleEnum])))
+    role = serializers.ChoiceField(
+        choices=[
+            MemberRoleEnum.admin.name,
+            MemberRoleEnum.member.name],
+        read_only=True)
 
     class Meta(BaseModelSerializer.Meta):
-        model = UserGroupRel
-        fields = BaseModelSerializer.Meta.fields + ('user_ids', )
+        model = GroupUserRel
+        fields = BaseModelSerializer.Meta.fields + ('user_ids', 'role')
         read_only_fields = BaseModelSerializer.Meta.read_only_fields
 
     def create(self, validated_data):
         for user in validated_data.pop('user_ids'):
-            instance = UserGroupRel.objects.filter(
+            if GroupUserRel.objects.filter(
                     user_id=user.id,
-                    group_id=validated_data['group_id']).first()
-            if instance is None:
-                validated_data['user_id'] = user.id
-                instance = super().create(validated_data)
+                    group_id=validated_data['group_id']).exists():
+                raise ValidationError(_(f'用户【{user.name}】已加入组'))
+            validated_data['user_id'] = user.id
+            instance = super().create(validated_data)
         return instance
+
+
+class DestroyGroupUserRelModelSerializer(BaseRelModelSerializer):
+    user_ids = serializers.ListField(
+        min_length=1,
+        max_length=10,
+        write_only=True,
+        child=serializers.PrimaryKeyRelatedField(
+            queryset=User.objects.filter(
+                role__in=[_.name for _ in MemberRoleEnum])))
+
+    class Meta:
+        model = GroupUserRel
+        fields = ('user_ids', )
+
+    def validate_user_ids(self, users):
+        user_ids = []
+        group = self.context['view'].get_parent_object()
+        for user in users:
+            if group.user_rels.filter(user_id=user.id).exists():
+                raise ValidationError(_(f'用户【{user.name}】未加入组'))
+            user_ids.append(user.id)
+        return user_ids
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/group/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 __history__ = """"""
 __all__ = ['urlpatterns']
 
 from django.urls import path, include, re_path
 from rest_framework import routers
 
 from rest_framework_admin.user.group import views
+from rest_framework_util.routers import RelDefaultRouter
 
 group_router = routers.DefaultRouter()
 group_router.register(r'^groups', views.GroupModelViewSet)
 
-group_related_user_router = routers.DefaultRouter()
-group_related_user_router.register(
+group_user_rel_router = RelDefaultRouter()
+group_user_rel_router.register(
     r'^users',
-    views.GroupRelatedUserModelViewSet,
-    basename='group_related_user_router')
+    views.GroupUserRelModelViewSet,
+    basename='group_user_rel_router')
 
 
 urlpatterns = [
     path(r'', include(group_router.urls)),
     re_path(
         r'groups/(?P<group_id>[a-z0-9A-Z\-]{32})/',
         include(
-            group_related_user_router.urls)),
+            group_user_rel_router.urls)),
 ]
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/views.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/group/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 # Create your views here.
 from drf_spectacular.utils import extend_schema_view, extend_schema
 from django.utils.translation import gettext_lazy as _
 
 from rest_framework_admin.user.group import serializers
-from rest_framework_admin.user.group.filters import GroupFilter, GroupRelatedUserFilter
-from rest_framework_admin.user.group.models import Group, UserGroupRel
-from rest_framework_admin.user.group.permissions import GroupModelPermission
+from rest_framework_admin.user.group.filters import GroupFilter, GroupUserRelFilter
+from rest_framework_admin.user.group.models import Group, GroupUserRel
+from rest_framework_admin.user.group.permissions import GroupModelPermission, GroupUserRelModelPermission
 from rest_framework_admin.user.group.serializers import GroupModelSerializer
-from rest_framework_admin.user.permissions import UserModelPermission
 from rest_framework_util.exceptions import HTTP403
 from rest_framework_util.viewsets import BaseModeViewSet, BaseRelModelViewSet
 
 
 @extend_schema_view(
     switch=extend_schema(summary='启用、禁用'),
 )
 class GroupModelViewSet(BaseModeViewSet):
     """ 组管理 """
     queryset = Group.objects.filter().order_by('-create_datetime').all()
     serializer_class = GroupModelSerializer
     serializer_module = serializers
     filterset_class = GroupFilter
-    search_fields = ['id', 'name']
+    search_fields = ['name']
     ordering_fields = ['name', 'create_datetime']
     permission_classes = (GroupModelPermission,)
 
+    def get_queryset(self):
+        if self.request.user.is_admin_or_owner:
+            queryset = super().get_queryset()
+        else:
+            queryset = self.request.user.groups
+        return queryset
+
     def perform_destroy(self, instance):
-        if instance.user_rels.exists():
-            raise HTTP403(_('存在关联用户，不允许删除'))
-        if instance.filter_roles().exists():
-            raise HTTP403(_('存在关联角色，不允许删除'))
+        # TODO(fengdy): 关联角色限制
         instance.delete(delete_user_id=self.request.user.id)
 
 
-@extend_schema_view()
-class GroupRelatedUserModelViewSet(BaseRelModelViewSet):
+@extend_schema_view(
+    list=extend_schema(summary='搜索用户'),
+    create=extend_schema(summary='批量增加用户'),
+    update=extend_schema(summary='全量更新用户'),
+    destroy=extend_schema(summary='批量删除用户'),
+)
+class GroupUserRelModelViewSet(BaseRelModelViewSet):
     """ 组关联的用户管理 """
     parent_model = Group
     lookup_field = 'user_id'
-    queryset = UserGroupRel.objects.all()
-    serializer_class = serializers.GroupRelatedUserModelSerializer
-    filterset_class = GroupRelatedUserFilter
+    queryset = GroupUserRel.objects.all()
+    serializer_class = serializers.GroupUserRelModelSerializer
+    serializer_module = serializers
+    filterset_class = GroupUserRelFilter
     search_fields = ['user__username', 'user__nickname']
     ordering_fields = [
         'create_datetime',
         'user__username',
         'user__create_datetime']
     ordering = ['-create_datetime']
-    permission_classes = (UserModelPermission,)
+    permission_classes = (GroupUserRelModelPermission,)
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0001_initial.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.13 on 2024-03-31 08:16
+# Generated by Django 4.1.13 on 2024-04-12 06:36
 
 from django.conf import settings
 import django.contrib.auth.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import rest_framework_util.db.models.manager
 import shortcut_util.unique
@@ -64,46 +64,37 @@
                     "nickname",
                     models.CharField(
                         blank=True, max_length=64, null=True, verbose_name="昵称"
                     ),
                 ),
                 ("email", models.EmailField(max_length=254, verbose_name="邮箱")),
                 (
-                    "is_staff",
-                    models.BooleanField(
-                        default=False,
-                        help_text="Designates whether the user can log into this admin site.",
-                        verbose_name="是否为员工",
-                    ),
-                ),
-                (
-                    "is_superuser",
-                    models.BooleanField(
-                        default=False,
-                        help_text="Designates that this user has all permissions without explicitly assigning them.",
-                        verbose_name="是否为超级管理员",
-                    ),
-                ),
-                (
                     "last_login",
                     models.DateTimeField(blank=True, null=True, verbose_name="最后登录时间"),
                 ),
                 (
-                    "telephone",
+                    "phone",
                     models.CharField(
                         blank=True, max_length=64, null=True, verbose_name="电话"
                     ),
                 ),
                 (
                     "avatar",
                     models.CharField(
                         blank=True, max_length=256, null=True, verbose_name="头像"
                     ),
                 ),
                 (
+                    "role",
+                    models.CharField(
+                        choices=[("owner", "创建者"), ("admin", "管理员"), ("member", "成员")],
+                        max_length=32,
+                    ),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
@@ -128,15 +119,15 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "user",
-                "db_table": "admin_user",
+                "db_table": "user",
             },
             managers=[
                 ("objects", rest_framework_util.db.models.manager.UserModelManager()),
             ],
         ),
         migrations.CreateModel(
             name="Group",
@@ -199,19 +190,19 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "用户组表",
-                "db_table": "admin_user_group",
+                "db_table": "user_group",
             },
         ),
         migrations.CreateModel(
-            name="UserGroupRel",
+            name="GroupUserRel",
             fields=[
                 (
                     "id",
                     models.CharField(
                         default=shortcut_util.unique.uuid_id,
                         max_length=32,
                         primary_key=True,
@@ -233,14 +224,22 @@
                     models.CharField(blank=True, max_length=256, verbose_name="描述"),
                 ),
                 (
                     "delete_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="删除时间"),
                 ),
                 (
+                    "role",
+                    models.CharField(
+                        choices=[("owner", "创建者"), ("admin", "管理员"), ("member", "成员")],
+                        default="member",
+                        max_length=32,
+                    ),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -254,14 +253,15 @@
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "group",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
+                        related_name="user_rel",
                         to="admin_user.group",
                     ),
                 ),
                 (
                     "update_user",
                     models.ForeignKey(
                         blank=True,
@@ -271,27 +271,28 @@
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
+                        related_name="group_rel",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "用户组关联表",
-                "db_table": "admin_user_group_rel",
+                "db_table": "user_group_user_rel",
                 "unique_together": {("user", "group", "delete_datetime")},
             },
         ),
         migrations.AddField(
             model_name="group",
-            name="user_rels",
+            name="users",
             field=models.ManyToManyField(
-                related_name="group_rels",
-                through="admin_user.UserGroupRel",
+                related_name="groups",
+                through="admin_user.GroupUserRel",
                 to=settings.AUTH_USER_MODEL,
             ),
         ),
     ]
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/models.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 # -*- coding:utf-8 -*-
 # Email:iamfengdy@126.com
 # DateTime:2023/11/16
 # Tool:PyCharm
 __all__ = [
     'User',
     'Group',
-    'UserGroupRel'
+    'GroupUserRel'
 ]
 import unicodedata
 
 from django.conf import settings
 from django.contrib.auth import password_validation
 from django.contrib.auth.hashers import make_password, check_password
 from django.contrib.auth.validators import UnicodeUsernameValidator
 from django.db import models
 
 # Create your models here.
 from django.utils.crypto import salted_hmac
 from django.utils.translation import gettext_lazy as _
 
-from rest_framework_util.db.models.base import BaseModel
+from rest_framework_admin.user.configs import MemberRoleEnum
+from rest_framework_util.db.models.base import BaseModel, BaseRelModel
 from rest_framework_util.db.models.manager import UserModelManager
 
 
 class User(BaseModel):
     username = models.CharField(
         '用户名',
         max_length=32,
@@ -35,50 +36,40 @@
             'unique': _("A user with that username already exists."),
         },
         unique=True,
     )
     password = models.CharField('密码', max_length=128)
     nickname = models.CharField('昵称', max_length=64, blank=True, null=True)
     email = models.EmailField('邮箱')
-    is_staff = models.BooleanField(
-        '是否为员工',
-        default=False,
-        help_text=_(
-            'Designates whether the user can log into this admin site.'),
-    )
-    is_superuser = models.BooleanField(
-        '是否为超级管理员',
-        default=False,
-        help_text=_(
-            'Designates that this user has all permissions without '
-            'explicitly assigning them.'
-        ),
-    )
     last_login = models.DateTimeField('最后登录时间', blank=True, null=True)
-    telephone = models.CharField('电话', max_length=64, blank=True, null=True)
+    phone = models.CharField('电话', max_length=64, blank=True, null=True)
     avatar = models.CharField('头像', max_length=256, null=True, blank=True)
     create_user = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         models.RESTRICT,
         related_name="created_%(app_label)s_%(class)ss",
         blank=True, null=True
     )
+    role = models.CharField(
+        max_length=32,
+        choices=[(_.name, _.value) for _ in MemberRoleEnum],
+        null=True)
     EMAIL_FIELD = 'email'
     USERNAME_FIELD = 'username'
     REQUIRED_FIELDS = ['email']
 
     objects = UserModelManager()
 
     # Stores the raw password if set_password() is called so that it can
     # be passed to password_changed() after the model is saved.
     _password = None
 
     class Meta:
         verbose_name = _('user')
-        db_table = 'admin_user'
+        db_table = 'user'
 
     def get_username(self):
         """Return the username for this User."""
         return getattr(self, self.USERNAME_FIELD)
 
     def __str__(self):
         return f'User(id={self.id}, username={self.get_username()})'
@@ -157,26 +148,73 @@
     def is_authenticated(self):
         """
         Always return True. This is a way to tell if the user has been
         authenticated in templates.
         """
         return True
 
-    def is_admin(self):
-        """ 管理员或者超级管理员 """
-        # TODO(fengdy): 管理员怎么定义
-        if not self.is_staff:
-            return False
-        if self.is_superuser:
-            return True
-        from rest_framework_admin.role.models import Role
-        from rest_framework_admin.role.configs import DefaultRoleEnum
-        for role_enum in (DefaultRoleEnum.owner, DefaultRoleEnum.admin):
-            role = Role.objects.get(id=role_enum.value.id)
-            role_rel_query = role.filter_users(
-                is_valid=True)
-            if role_rel_query.exists():
-                return True
-        return False
+    @property
+    def is_staff(self):
+        return self.role in MemberRoleEnum._member_names_
+
+    @property
+    def is_admin_or_owner(self):
+        """ 管理员或者创建者 """
+        return MemberRoleEnum.is_admin_or_owner(self.role)
+
+    @property
+    def current_tenant(self):
+        if hasattr(self, '_current_tenant'):
+            return self._current_tenant
+        from rest_framework_admin.tenant.models import TenantUserRel
+        rel_query = TenantUserRel.objects.filter(user_id=self.id)
+        if rel_query.filter(is_current=True).first():
+            rel = rel_query.filter(is_current=True).first()
+        else:
+            rel = rel_query.first()
+        self.current_tenant_id = rel.tenant_id if rel else None
+        return self._current_tenant
+
+    @current_tenant.setter
+    def current_tenant(self, value):
+        from rest_framework_admin.tenant.models import TenantUserRel
+        tenant = value
+        rel = TenantUserRel.objects.filter(
+            tenant_id=tenant.id, user_id=self.id).first()
+        if rel:
+            tenant.current_role = rel.role
+        else:
+            tenant = None
+        self._current_tenant = tenant
+
+    @property
+    def current_tenant_id(self):
+        return self._current_tenant.id
+
+    @current_tenant_id.setter
+    def current_tenant_id(self, value):
+        try:
+            from rest_framework_admin.tenant.models import TenantUserRel
+            rel = TenantUserRel.objects.filter(
+                tenant_id=value, user_id=self.id).first()
+            if rel:
+                tenant = rel.tenant
+                tenant.current_role = rel.role
+            else:
+                tenant = None
+        except BaseException:
+            tenant = None
+
+        self._current_tenant = tenant
+
+
+class BaseUserRel(BaseRelModel):
+    user = models.ForeignKey(User, models.CASCADE)
+    role = models.CharField(
+        max_length=32,
+        choices=[(_.name, _.value) for _ in MemberRoleEnum])
+
+    class Meta:
+        abstract = True
 
 
-from rest_framework_admin.user.group.models import Group, UserGroupRel
+from rest_framework_admin.user.group.models import Group, GroupUserRel
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/serializers.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,113 +10,121 @@
 
 from django.contrib.auth import password_validation
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 from rest_framework.validators import UniqueValidator
 
-from rest_framework_admin.user.models import User, Group, UserGroupRel
+from rest_framework_admin.user.configs import MemberRoleEnum
+from rest_framework_admin.user.group.models import Group
+from rest_framework_admin.user.models import User, GroupUserRel
 from rest_framework_util.serializers import BaseSwitchModelSerializer, BaseModelSerializer, BaseSelectionModelSerializer, BaseRelModelSerializer
 
 
 class UserModelSerializer(BaseModelSerializer):
     username = serializers.CharField(
+        write_only=True,
         help_text='账户（不允许更新）',
         validators=(
             UniqueValidator(
                 queryset=User.objects.filter()),))
     password = serializers.CharField(
         help_text='密码（不允许更新）',
         write_only=True, validators=[
             password_validation.validate_password])
-    is_staff = serializers.BooleanField(
-        required=False,
-        default=True,
-        help_text='是否为员工，默认为True')
     is_active = serializers.BooleanField(
         required=False,
         default=True,
         help_text='是否激活，默认为True')
-    is_superuser = serializers.BooleanField(
-        required=False,
-        default=False,
-        help_text='是否为超级用户，默认为False')
     description = serializers.CharField(
         required=False, allow_blank=True, allow_null=True, help_text='描述')
-    telephone = serializers.CharField(
-        required=False, allow_blank=True, allow_null=True, help_text='电话')
-    name = serializers.CharField(
-        help_text='真实姓名',
-        read_only=True)
+    phone = serializers.CharField(
+        required=False,
+        write_only=True,
+        help_text='电话')
+    name = serializers.CharField(read_only=True)
     nickname = serializers.CharField(
         required=False,
         allow_blank=True,
         allow_null=True,
         help_text='昵称')
     email = serializers.EmailField(
         required=False,
         allow_blank=True,
         allow_null=True,
         help_text='邮箱')
+    role = serializers.ChoiceField(
+        [_.name for _ in MemberRoleEnum], default=None, required=False, allow_null=True)
     # avatar = ImageOrCharField(
     #     max_length=256,
     #     required=False,
     #     allow_blank=True,
     #     allow_null=True)
+    # TODO(fengdy): 头像
+    is_staff = serializers.BooleanField(read_only=True)
 
     class Meta:
         model = User
-        read_only_fields = ('create_datetime', 'id', 'last_login')
+        read_only_fields = ('create_datetime', 'id', 'last_login', 'is_staff')
         exclude = ('delete_user', 'delete_datetime')
 
     def create(self, validated_data):
         user = User(**validated_data)
         user.set_password(user.password)
         user.save()
         return user
 
-    def update(self, instance, validated_data):
-        validated_data.pop('username', None)
-        validated_data.pop('password', None)
-        instance = super().update(instance, validated_data)
-        return instance
-
 
-class SwitchUserModelSerializer(BaseSwitchModelSerializer):
+class PartialUpdateUserModelSerializer(serializers.ModelSerializer):
+    username = serializers.CharField(
+        required=False,
+        validators=(
+            UniqueValidator(
+                queryset=User.objects.filter()),),
+        write_only=True)
+    role = serializers.ChoiceField(
+        [MemberRoleEnum.admin.name, MemberRoleEnum.member.name],
+        required=False)
+    description = serializers.CharField(
+        required=False, allow_blank=True, allow_null=True, help_text='描述')
+    phone = serializers.CharField(
+        required=False,
+        help_text='电话')
+    nickname = serializers.CharField(
+        required=False,
+        help_text='昵称')
+    email = serializers.EmailField(
+        required=False,
+        help_text='邮箱')
+    # TODO(fengdy): 头像
 
-    class Meta(BaseSwitchModelSerializer.Meta):
+    class Meta:
         model = User
+        fields = (
+            'id',
+            'username',
+            'description',
+            'nickname',
+            'phone',
+            'email',
+            'role')
+
+    def validate_role(self, value):
+        if not self.instance.is_staff:
+            raise ValidationError(_('仅允许内部员工更新'))
+        return value
 
 
-class UpdatePasswordUserModelSerializer(serializers.ModelSerializer):
-    """ 用户更新密码 """
-    old_password = serializers.CharField(help_text='旧密码', write_only=True)
-    new_password = serializers.CharField(
-        help_text='新密码',
-        write_only=True, validators=[
-            password_validation.validate_password])
+class SwitchUserModelSerializer(BaseSwitchModelSerializer):
 
-    class Meta:
+    class Meta(BaseSwitchModelSerializer.Meta):
         model = User
-        fields = ('old_password', 'new_password')
-
-    def validate_old_password(self, value):
-        if not self.instance.check_password(value):
-            raise ValidationError(_('密码错误，请确认'))
-        return value
-
-    def update(self, instance, validated_data):
-        new_password = validated_data.pop('new_password')
-        instance.set_password(new_password)
-        instance = super().update(instance, validated_data)
-        return instance
 
 
-class UpdateUserPasswordUserModelSerializer(serializers.ModelSerializer):
-    """ 更新用户密码 """
+class UpdatePasswordUserModelSerializer(serializers.ModelSerializer):
     new_password = serializers.CharField(
         help_text='新密码',
         write_only=True, validators=[
             password_validation.validate_password])
 
     class Meta:
         model = User
@@ -125,34 +133,43 @@
     def update(self, instance, validated_data):
         new_password = validated_data.pop('new_password')
         instance.set_password(new_password)
         instance = super().update(instance, validated_data)
         return instance
 
 
-class SelectionUserModelSerializer(BaseSelectionModelSerializer):
+class SelectUserModelSerializer(BaseSelectionModelSerializer):
 
     class Meta(BaseSelectionModelSerializer.Meta):
         model = User
 
 
-class UserRelatedGroupModelSerializer(BaseRelModelSerializer):
+class GroupUserRelModelSerializer(BaseRelModelSerializer):
     id = serializers.CharField(source='group_id', read_only=True)
     name = serializers.CharField(source='group__name', read_only=True)
+
+    class Meta(BaseRelModelSerializer.Meta):
+        model = GroupUserRel
+
+
+class DestroyGroupUserRelModelSerializer(BaseRelModelSerializer):
     group_ids = serializers.ListField(
         min_length=1,
         max_length=10,
         write_only=True,
         child=serializers.PrimaryKeyRelatedField(queryset=Group.objects.all()))
 
-    class Meta(BaseRelModelSerializer.Meta):
-        model = UserGroupRel
-        fields = BaseRelModelSerializer.Meta.fields + ('group_ids', )
+    class Meta:
+        model = GroupUserRel
+        fields = ('group_ids', )
 
-    def create(self, validated_data):
-        for group in validated_data.pop('group_ids'):
-            if not UserGroupRel.objects.filter(
-                    group_id=group.id,
-                    user_id=validated_data['user_id']).exists():
-                validated_data['group_id'] = group.id
-                instance = super().create(validated_data)
-        return instance
+    def validate_group_ids(self, groups):
+        group_ids = []
+        user = self.context['view'].get_parent_object()
+        for group in groups:
+            rel = user.group_rels.filter(group_id=group.id).first()
+            if not rel:
+                raise ValidationError(_(f'用户未加入组【{group.name}】'))
+            if rel.role == MemberRoleEnum.owner.name:
+                raise ValidationError(_(f'当前角色为组【{group.name}】创建者，禁止退出'))
+            group_ids.append(group.id)
+        return group_ids
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/settings.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/role/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 }
 
 IMPORT_STRINGS = [
     'UPLOAD_SETTINGS'
 ]
 
 api_settings = get_api_settings(
-    'ADMIN_USER',
+    'ADMIN_ROLE',
     defaults=DEFAULTS,
     import_strings=IMPORT_STRINGS)
```

### Comparing `djangorestframework-admin-0.0.7/rest_framework_admin/user/urls.py` & `djangorestframework-admin-0.0.8/rest_framework_admin/user/urls.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 __all__ = ['urlpatterns']
 
 from django.urls import path, include, re_path
 from rest_framework import routers
 
 from rest_framework_admin.user import views
 from rest_framework_admin.user.group.urls import urlpatterns as group_urlpatterns
+from rest_framework_admin.user.me.urls import urlpatterns as me_urlpatterns
+from rest_framework_util.routers import RelDefaultRouter
 
 user_router = routers.DefaultRouter()
 user_router.register(r'^users', views.UserModelViewSet)
 
-user_related_group_router = routers.DefaultRouter()
-user_related_group_router.register(
+group_user_rel_router = RelDefaultRouter()
+group_user_rel_router.register(
     r'^groups',
-    views.UserRelatedGroupModelViewSet,
-    basename='user_related_group_router')
+    views.GroupUserRelModelViewSet,
+    basename='group_user_rel_router')
 
 urlpatterns = [
     path(r'', include(user_router.urls)),
     re_path(
         r'users/(?P<user_id>[a-z0-9A-Z\-]{32})/',
         include(
-            user_related_group_router.urls)),
-] + group_urlpatterns
+            group_user_rel_router.urls)),
+] + group_urlpatterns + me_urlpatterns
```

### Comparing `djangorestframework-admin-0.0.7/setup.py` & `djangorestframework-admin-0.0.8/setup.py`

 * *Files identical despite different names*

