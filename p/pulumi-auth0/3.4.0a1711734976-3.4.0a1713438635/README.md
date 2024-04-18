# Comparing `tmp/pulumi_auth0-3.4.0a1711734976.tar.gz` & `tmp/pulumi_auth0-3.4.0a1713438635.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_auth0-3.4.0a1711734976.tar", last modified: Fri Mar 29 18:19:15 2024, max compression
+gzip compressed data, was "pulumi_auth0-3.4.0a1713438635.tar", last modified: Thu Apr 18 11:12:34 2024, max compression
```

## Comparing `pulumi_auth0-3.4.0a1711734976.tar` & `pulumi_auth0-3.4.0a1713438635.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:19:15.923539 pulumi_auth0-3.4.0a1711734976/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-29 18:19:15.923539 pulumi_auth0-3.4.0a1711734976/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:19:15.919538 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   363424 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/branding.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)   104995 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24449 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:19:15.923539 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    43140 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)    20422 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/custom_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/email_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/email_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    27341 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_signing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    31395 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)    18375 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14807 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    14580 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_members.py
--rw-r--r--   0 runner    (1001) docker     (127)   528561 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt_custom_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt_partials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35511 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13051 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/rule_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    50856 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/trigger_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54816 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:19:15.923539 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-29 18:19:15.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-29 18:19:15.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:19:15.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 18:19:15.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 18:19:15.000000 pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-29 18:19:09.000000 pulumi_auth0-3.4.0a1711734976/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 18:19:15.923539 pulumi_auth0-3.4.0a1711734976/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   363424 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104995 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24449 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43140 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20422 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/custom_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/email_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/email_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27341 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_signing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31395 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18375 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14807 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14580 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)   528561 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt_custom_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt_partials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35511 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13051 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/rule_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50856 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/trigger_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54816 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 11:12:34.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-18 11:12:34.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:12:34.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 11:12:34.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 11:12:34.000000 pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 11:12:28.000000 pulumi_auth0-3.4.0a1713438635/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:12:34.651615 pulumi_auth0-3.4.0a1713438635/setup.cfg
```

### Comparing `pulumi_auth0-3.4.0a1711734976/PKG-INFO` & `pulumi_auth0-3.4.0a1713438635/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1711734976
+Version: 3.4.0a1713438635
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1711734976/README.md` & `pulumi_auth0-3.4.0a1713438635/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/__init__.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/_inputs.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/_utilities.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/action.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/attack_protection.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/branding.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/branding_theme.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client_credentials.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/client_grant.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/client_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/__init__.pyi` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/config/vars.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection_client.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/connection_clients.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/connection_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/custom_domain.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/custom_domain_verification.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/custom_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/email_provider.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/email_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/email_template.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/email_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_attack_protection.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_branding.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_branding_theme.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_client.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_connection.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_custom_domain.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_organization.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_pages.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_resource_server.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_role.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_signing_keys.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_signing_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_tenant.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/get_user.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/guardian.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/guardian.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/hook.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/log_stream.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_connection.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_connections.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member_role.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_member_roles.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_member_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/organization_members.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/organization_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/outputs.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/pages.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt_custom_text.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt_custom_text.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/prompt_partials.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/prompt_partials.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/provider.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server_scope.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/resource_server_scopes.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/resource_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role_permission.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/role_permissions.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/role_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/rule.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/rule_config.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/rule_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/tenant.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/trigger_action.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/trigger_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/trigger_actions.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_permission.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_permissions.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_role.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0/user_roles.py` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/PKG-INFO` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1711734976
+Version: 3.4.0a1713438635
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1711734976/pulumi_auth0.egg-info/SOURCES.txt` & `pulumi_auth0-3.4.0a1713438635/pulumi_auth0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1711734976/pyproject.toml` & `pulumi_auth0-3.4.0a1713438635/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_auth0"
   description = "A Pulumi package for creating and managing auth0 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "auth0"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1711734976"
+  version = "3.4.0a1713438635"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-auth0"
 
 [build-system]
```

