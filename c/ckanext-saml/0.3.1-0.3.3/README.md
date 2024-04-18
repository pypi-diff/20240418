# Comparing `tmp/ckanext-saml-0.3.1.tar.gz` & `tmp/ckanext_saml-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-saml-0.3.1.tar", last modified: Mon Apr 24 12:29:21 2023, max compression
+gzip compressed data, was "ckanext_saml-0.3.3.tar", last modified: Thu Apr 18 16:35:15 2024, max compression
```

## Comparing `ckanext-saml-0.3.1.tar` & `ckanext_saml-0.3.3.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      199 2023-04-11 20:10:06.000000 ckanext-saml-0.3.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6376 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       91 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2949 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2313 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      693 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1201 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/logic/action.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/saml/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/migration/saml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      794 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       50 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      829 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/model/user.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1823 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/saml/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/templates/admin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      166 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/templates/admin/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/templates/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3663 2023-04-24 12:27:53.000000 ckanext-saml-0.3.1/ckanext/saml/templates/user/edit_user_form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/templates/user/login.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      242 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1177 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/tests/model/test_user.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1358 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/tests/test_helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       94 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1785 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/views/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/views/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9866 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/views/saml.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/ckanext_saml.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1405 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       68 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1664 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.284993 ckanext_saml-0.3.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      199 2024-04-18 16:34:16.000000 ckanext_saml-0.3.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7163 2024-04-18 16:35:15.284993 ckanext_saml-0.3.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6376 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.274993 ckanext_saml-0.3.3/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.278326 ckanext_saml-0.3.3/ckanext/saml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       91 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2949 2024-04-18 16:34:16.000000 ckanext_saml-0.3.3/ckanext/saml/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2313 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      693 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.278326 ckanext_saml-0.3.3/ckanext/saml/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1639 2024-04-18 16:34:16.000000 ckanext_saml-0.3.3/ckanext/saml/logic/action.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.274993 ckanext_saml-0.3.3/ckanext/saml/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.278326 ckanext_saml-0.3.3/ckanext/saml/migration/saml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.278326 ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      794 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       50 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      829 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/model/user.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1823 2024-04-18 16:34:16.000000 ckanext_saml-0.3.3/ckanext/saml/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.274993 ckanext_saml-0.3.3/ckanext/saml/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/templates/admin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      166 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/templates/admin/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/templates/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/templates/user/login.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      242 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1177 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/model/test_user.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1358 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/test_helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       94 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1785 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.281659 ckanext_saml-0.3.3/ckanext/saml/views/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/ckanext/saml/views/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9941 2024-04-18 16:34:18.000000 ckanext_saml-0.3.3/ckanext/saml/views/saml.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-18 16:35:15.284993 ckanext_saml-0.3.3/ckanext_saml.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7163 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1357 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       68 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-18 16:35:15.000000 ckanext_saml-0.3.3/ckanext_saml.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1664 2024-04-18 16:35:15.284993 ckanext_saml-0.3.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2024-02-26 12:57:44.000000 ckanext_saml-0.3.3/setup.py
```

### Comparing `ckanext-saml-0.3.1/LICENSE` & `ckanext_saml-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/PKG-INFO` & `ckanext_saml-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: ckanext-saml
-Version: 0.3.1
+Version: 0.3.3
 Home-page: https://github.com/DataShades/ckanext-saml
 Author: Yan Rudendo
 Author-email: yan.rudenko@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: adfs
 License-File: LICENSE
+Requires-Dist: python3-saml
+Requires-Dist: typing-extensions
+Requires-Dist: ckanext-toolbelt
+Provides-Extra: adfs
+Requires-Dist: lxml==4.6.4; extra == "adfs"
 
 # ckanext-saml
 
 Adds an ability to login from other source (known as
 [IdP](https://en.wikipedia.org/wiki/Identity_provider_(SAML))) using
 [SAML2](https://en.wikipedia.org/wiki/SAML_2.0) standard. Your instance is
 presented as the [SP](https://en.wikipedia.org/wiki/Service_provider_(SAML)).
```

### Comparing `ckanext-saml-0.3.1/README.md` & `ckanext_saml-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/config.py` & `ckanext_saml-0.3.3/ckanext/saml/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/helpers.py` & `ckanext_saml-0.3.3/ckanext/saml/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/interfaces.py` & `ckanext_saml-0.3.3/ckanext/saml/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/migration/saml/alembic.ini` & `ckanext_saml-0.3.3/ckanext/saml/migration/saml/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/migration/saml/env.py` & `ckanext_saml-0.3.3/ckanext/saml/migration/saml/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py` & `ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py` & `ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py` & `ckanext_saml-0.3.3/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/model/user.py` & `ckanext_saml-0.3.3/ckanext/saml/model/user.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/plugin.py` & `ckanext_saml-0.3.3/ckanext/saml/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/tests/model/test_user.py` & `ckanext_saml-0.3.3/ckanext/saml/tests/model/test_user.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/tests/test_helpers.py` & `ckanext_saml-0.3.3/ckanext/saml/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/utils.py` & `ckanext_saml-0.3.3/ckanext/saml/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.1/ckanext/saml/views/saml.py` & `ckanext_saml-0.3.3/ckanext/saml/views/saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,18 @@
             redirect = (
                 saml_relaystate
                 if saml_relaystate
                 else _destination()
             )
             if tk.request.args.get("redirect"):
                 redirect = tk.request.args.get("redirect")
+
+            if tk.g.user:
+                return h.redirect_to(redirect)
+
             log.info("Redirect to SAML IdP.")
             return h.redirect_to(auth.login(return_to=redirect))
         else:
             log.warning(
                 "No arguments been provided in this URL. If you want to make"
                 " auth request to SAML IdP point, please provide '?sso=true'"
                 " at the end of the URL."
```

### Comparing `ckanext-saml-0.3.1/ckanext_saml.egg-info/PKG-INFO` & `ckanext_saml-0.3.3/ckanext_saml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: ckanext-saml
-Version: 0.3.1
+Version: 0.3.3
 Home-page: https://github.com/DataShades/ckanext-saml
 Author: Yan Rudendo
 Author-email: yan.rudenko@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: adfs
 License-File: LICENSE
+Requires-Dist: python3-saml
+Requires-Dist: typing-extensions
+Requires-Dist: ckanext-toolbelt
+Provides-Extra: adfs
+Requires-Dist: lxml==4.6.4; extra == "adfs"
 
 # ckanext-saml
 
 Adds an ability to login from other source (known as
 [IdP](https://en.wikipedia.org/wiki/Identity_provider_(SAML))) using
 [SAML2](https://en.wikipedia.org/wiki/SAML_2.0) standard. Your instance is
 presented as the [SP](https://en.wikipedia.org/wiki/Service_provider_(SAML)).
```

### Comparing `ckanext-saml-0.3.1/ckanext_saml.egg-info/SOURCES.txt` & `ckanext_saml-0.3.3/ckanext_saml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 ckanext/saml/migration/saml/script.py.mako
 ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py
 ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py
 ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py
 ckanext/saml/model/__init__.py
 ckanext/saml/model/user.py
 ckanext/saml/templates/admin/base.html
-ckanext/saml/templates/user/edit_user_form.html
 ckanext/saml/templates/user/login.html
 ckanext/saml/tests/__init__.py
 ckanext/saml/tests/conftest.py
 ckanext/saml/tests/test_helpers.py
 ckanext/saml/tests/test_plugin.py
 ckanext/saml/tests/model/__init__.py
 ckanext/saml/tests/model/test_user.py
```

### Comparing `ckanext-saml-0.3.1/setup.cfg` & `ckanext_saml-0.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-saml
-version = 0.3.1
+version = 0.3.3
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-saml
 author = Yan Rudendo
 author_email = yan.rudenko@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-saml-0.3.1/setup.py` & `ckanext_saml-0.3.3/setup.py`

 * *Files identical despite different names*

