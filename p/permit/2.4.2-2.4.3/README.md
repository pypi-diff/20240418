# Comparing `tmp/permit-2.4.2.tar.gz` & `tmp/permit-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.4.2.tar", last modified: Wed Apr 17 08:52:57 2024, max compression
+gzip compressed data, was "permit-2.4.3.tar", last modified: Thu Apr 18 17:29:07 2024, max compression
```

## Comparing `permit-2.4.2.tar` & `permit-2.4.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 08:51:54.000000 permit-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 08:51:54.000000 permit-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 08:52:57.197205 permit-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 08:51:54.000000 permit-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.193205 permit-2.4.2/permit/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 08:51:54.000000 permit-2.4.2/permit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/permit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/condition_set_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/condition_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/relationship_tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_action_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resource_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/sync_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-17 08:51:54.000000 permit-2.4.2/permit/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-17 08:51:54.000000 permit-2.4.2/permit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/permit/enforcement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:51:54.000000 permit-2.4.2/permit/enforcement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-17 08:51:54.000000 permit-2.4.2/permit/enforcement/enforcer.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-17 08:51:54.000000 permit-2.4.2/permit/enforcement/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-17 08:51:54.000000 permit-2.4.2/permit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 08:51:54.000000 permit-2.4.2/permit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/permit/pdp_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:51:54.000000 permit-2.4.2/permit/pdp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 08:51:54.000000 permit-2.4.2/permit/pdp_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 08:51:54.000000 permit-2.4.2/permit/pdp_api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 08:51:54.000000 permit-2.4.2/permit/pdp_api/pdp_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-17 08:51:54.000000 permit-2.4.2/permit/pdp_api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-17 08:51:54.000000 permit-2.4.2/permit/permit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-17 08:51:54.000000 permit-2.4.2/permit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/permit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/pydantic_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-17 08:51:54.000000 permit-2.4.2/permit/utils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.193205 permit-2.4.2/permit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 08:52:57.000000 permit-2.4.2/permit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 08:52:57.000000 permit-2.4.2/permit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:52:57.000000 permit-2.4.2/permit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 08:52:57.000000 permit-2.4.2/permit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 08:52:57.000000 permit-2.4.2/permit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 08:51:54.000000 permit-2.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:52:57.197205 permit-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 08:52:55.000000 permit-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:52:57.197205 permit-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:51:54.000000 permit-2.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-17 08:51:54.000000 permit-2.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-17 08:51:54.000000 permit-2.4.2/tests/test_abac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-17 08:51:54.000000 permit-2.4.2/tests/test_abac_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-17 08:51:54.000000 permit-2.4.2/tests/test_rbac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 08:51:54.000000 permit-2.4.2/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-17 08:51:54.000000 permit-2.4.2/tests/test_rebac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-17 08:51:54.000000 permit-2.4.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 17:27:48.000000 permit-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 17:27:48.000000 permit-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 17:29:07.105849 permit-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 17:27:48.000000 permit-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.097849 permit-2.4.3/permit/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 17:27:48.000000 permit-2.4.3/permit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/condition_set_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/condition_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/relationship_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_action_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/sync_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-18 17:27:48.000000 permit-2.4.3/permit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/enforcement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/enforcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-18 17:27:48.000000 permit-2.4.3/permit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 17:27:48.000000 permit-2.4.3/permit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/pdp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/pdp_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-18 17:27:48.000000 permit-2.4.3/permit/permit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-18 17:27:48.000000 permit-2.4.3/permit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/permit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/pydantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.097849 permit-2.4.3/permit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 17:27:48.000000 permit-2.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:29:07.105849 permit-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 17:29:05.000000 permit-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-18 17:27:48.000000 permit-2.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_abac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_abac_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rbac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rebac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-18 17:27:48.000000 permit-2.4.3/tests/utils.py
```

### Comparing `permit-2.4.2/LICENSE` & `permit-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/api_client.py` & `permit-2.4.3/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/base.py` & `permit-2.4.3/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/condition_set_rules.py` & `permit-2.4.3/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/condition_sets.py` & `permit-2.4.3/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/context.py` & `permit-2.4.3/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/deprecated.py` & `permit-2.4.3/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/elements.py` & `permit-2.4.3/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/environments.py` & `permit-2.4.3/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/models.py` & `permit-2.4.3/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/projects.py` & `permit-2.4.3/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/relationship_tuples.py` & `permit-2.4.3/permit/api/relationship_tuples.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_action_groups.py` & `permit-2.4.3/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_actions.py` & `permit-2.4.3/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_attributes.py` & `permit-2.4.3/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_instances.py` & `permit-2.4.3/permit/api/resource_instances.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_relations.py` & `permit-2.4.3/permit/api/resource_relations.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resource_roles.py` & `permit-2.4.3/permit/api/resource_roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/resources.py` & `permit-2.4.3/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/role_assignments.py` & `permit-2.4.3/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/roles.py` & `permit-2.4.3/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/sync_api_client.py` & `permit-2.4.3/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/tenants.py` & `permit-2.4.3/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/api/users.py` & `permit-2.4.3/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/config.py` & `permit-2.4.3/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/enforcement/enforcer.py` & `permit-2.4.3/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/enforcement/interfaces.py` & `permit-2.4.3/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/exceptions.py` & `permit-2.4.3/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/pdp_api/base.py` & `permit-2.4.3/permit/pdp_api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/pdp_api/models.py` & `permit-2.4.3/permit/pdp_api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/pdp_api/pdp_api_client.py` & `permit-2.4.3/permit/pdp_api/pdp_api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from permit.utils.sync import SyncClass
 
 from ..config import PermitConfig
 from .role_assignments import RoleAssignmentsApi
 
 
+class SyncRoleAssignmentsApi(RoleAssignmentsApi, metaclass=SyncClass):
+    pass
+
+
 class PermitPdpApiClient:
     def __init__(self, config: PermitConfig):
         """
         Constructs a new instance of the PdpApiClient class with the specified SDK configuration.
 
         Args:
             config: The configuration for the Permit SDK.
@@ -22,9 +26,14 @@
         self._role_assignments = RoleAssignmentsApi(config)
 
     @property
     def role_assignments(self) -> RoleAssignmentsApi:
         return self._role_assignments
 
 
-class SyncPDPApi(PermitPdpApiClient, metaclass=SyncClass):
-    pass
+class SyncPDPApi(PermitPdpApiClient):
+    def __init__(self, config: PermitConfig):
+        self._role_assignments = SyncRoleAssignmentsApi(config)
+
+    @property
+    def role_assignments(self) -> SyncRoleAssignmentsApi:
+        return self._role_assignments
```

### Comparing `permit-2.4.2/permit/pdp_api/role_assignments.py` & `permit-2.4.3/permit/pdp_api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/permit.py` & `permit-2.4.3/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/sync.py` & `permit-2.4.3/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/utils/context.py` & `permit-2.4.3/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/utils/deprecation.py` & `permit-2.4.3/permit/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/permit/utils/sync.py` & `permit-2.4.3/permit/utils/sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,13 +27,17 @@
 
         for name in dir(class_obj):
             if name.startswith("_"):
                 # do not monkey-patch protected or private method
                 continue
 
             attr = getattr(class_obj, name)
-
-            if callable(attr) and iscoroutine_func(attr):
+            if attr.__class__.__name__ in ("cython_function_or_method", "function"):
+                # Handle cython method
+                is_coroutine = True
+            else:
+                is_coroutine = iscoroutine_func(attr)
+            if callable(attr) and is_coroutine:
                 # monkey-patch public method using async_to_sync decorator
                 setattr(class_obj, name, async_to_sync(attr))
 
         return class_obj
```

### Comparing `permit-2.4.2/permit.egg-info/SOURCES.txt` & `permit-2.4.3/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/setup.py` & `permit-2.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 
 setup(
     name="permit",
-    version="v2.4.2",
+    version="v2.4.3",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.4.2/tests/conftest.py` & `permit-2.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/tests/test_abac_e2e.py` & `permit-2.4.3/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/tests/test_abac_pdp.py` & `permit-2.4.3/tests/test_abac_pdp.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/tests/test_rbac_e2e.py` & `permit-2.4.3/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.2/tests/test_rbac_e2e_sync.py` & `permit-2.4.3/tests/test_rbac_e2e_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 
 import pytest
 from loguru import logger
 
 from permit import RoleAssignmentRead
 from permit.exceptions import PermitApiError, PermitConnectionError
+from permit.pdp_api.models import RoleAssignment
 from permit.sync import Permit as SyncPermit
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
@@ -212,14 +213,24 @@
                     "user": user.key,
                     "action": "create",
                     "resource": {"type": document.key, "tenant": tenant.key},
                 },
             ]
         ) == [True, True, False]
 
+        logger.info("testing list role assignments")
+        assignments_returned: List[
+            RoleAssignment
+        ] = permit.pdp_api.role_assignments.list()
+        assert len(assignments_returned) == 1
+        assert assignments_returned[0].user == user.key
+        assert assignments_returned[0].role == viewer.key
+        assert assignments_returned[0].tenant == tenant.key
+        print_break()
+
         logger.info("changing the user roles")
 
         # change the user role - assign admin role
         permit.api.users.assign_role(
             {
                 "user": user.key,
                 "role": admin.key,
```

### Comparing `permit-2.4.2/tests/test_rebac_e2e.py` & `permit-2.4.3/tests/test_rebac_e2e.py`

 * *Files identical despite different names*

