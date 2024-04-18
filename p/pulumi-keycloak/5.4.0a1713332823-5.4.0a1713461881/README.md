# Comparing `tmp/pulumi_keycloak-5.4.0a1713332823.tar.gz` & `tmp/pulumi_keycloak-5.4.0a1713461881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.4.0a1713332823.tar", last modified: Wed Apr 17 05:59:21 2024, max compression
+gzip compressed data, was "pulumi_keycloak-5.4.0a1713461881.tar", last modified: Thu Apr 18 17:41:39 2024, max compression
```

## Comparing `pulumi_keycloak-5.4.0a1713332823.tar` & `pulumi_keycloak-5.4.0a1713461881.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.649077 pulumi_keycloak-5.4.0a1713332823/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-17 05:59:21.649077 pulumi_keycloak-5.4.0a1713332823/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.633077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91136 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.637077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23414 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.637077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22921 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24066 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22483 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    26906 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    38664 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24616 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.637077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/custom_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    45018 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18611 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14490 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46697 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    32408 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    89276 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.641077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70210 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    82524 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.645077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28803 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (127)    90703 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21986 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31435 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31053 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    38993 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31198 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    34306 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30599 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    82512 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18366 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    25256 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19137 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.649077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    71743 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)   101072 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28415 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20640 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24612 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:21.649077 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-17 05:59:21.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-17 05:59:21.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:59:21.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:59:21.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 05:59:21.000000 pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 05:59:15.000000 pulumi_keycloak-5.4.0a1713332823/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:59:21.649077 pulumi_keycloak-5.4.0a1713332823/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91136 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24684 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23414 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23287 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26780 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38724 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20514 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24704 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.285069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/custom_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45150 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46827 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32560 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89338 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.285069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70182 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82528 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.293069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29119 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19279 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90769 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22120 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15773 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23154 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26636 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35520 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36474 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39329 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31502 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34658 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30939 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82512 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18452 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18252 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17424 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.293069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63709 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24405 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101076 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28553 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20651 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17054 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/setup.cfg
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/PKG-INFO` & `pulumi_keycloak-5.4.0a1713461881/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1713332823
+Version: 5.4.0a1713461881
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/README.md` & `pulumi_keycloak-5.4.0a1713461881/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,18 +294,19 @@
         ### Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        test_mapper = keycloak.AttributeImporterIdentityProviderMapper("testMapper",
-            attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
-            identity_provider_alias="idp_alias",
+        test_mapper = keycloak.AttributeImporterIdentityProviderMapper("test_mapper",
             realm="my-realm",
+            name="my-mapper",
+            identity_provider_alias="idp_alias",
+            attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
             user_attribute="lastName")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
@@ -349,18 +350,19 @@
         ### Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        test_mapper = keycloak.AttributeImporterIdentityProviderMapper("testMapper",
-            attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
-            identity_provider_alias="idp_alias",
+        test_mapper = keycloak.AttributeImporterIdentityProviderMapper("test_mapper",
             realm="my-realm",
+            name="my-mapper",
+            identity_provider_alias="idp_alias",
+            attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
             user_attribute="lastName")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,28 +371,30 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        oidc_attribute_to_role_identity_mapper = keycloak.AttributeToRoleIdentityMapper("oidcAttributeToRoleIdentityMapper",
+        oidc_attribute_to_role_identity_mapper = keycloak.AttributeToRoleIdentityMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="role-attribute",
+            identity_provider_alias=oidc.alias,
             role="my-realm-role",
             claim_name="my-claim",
             claim_value="my-value",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
@@ -442,28 +444,30 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        oidc_attribute_to_role_identity_mapper = keycloak.AttributeToRoleIdentityMapper("oidcAttributeToRoleIdentityMapper",
+        oidc_attribute_to_role_identity_mapper = keycloak.AttributeToRoleIdentityMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="role-attribute",
+            identity_provider_alias=oidc.alias,
             role="my-realm-role",
             claim_name="my-claim",
             claim_value="my-value",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,27 +288,27 @@
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         flow = keycloak.authentication.Flow("flow",
             realm_id=realm.id,
             alias="my-flow-alias")
         # first execution
-        execution_one = keycloak.authentication.Execution("executionOne",
+        execution_one = keycloak.authentication.Execution("execution_one",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="auth-cookie",
             requirement="ALTERNATIVE")
         # second execution
-        execution_two = keycloak.authentication.Execution("executionTwo",
+        execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
-        browser_authentication_binding = keycloak.authentication.Bindings("browserAuthenticationBinding",
+        browser_authentication_binding = keycloak.authentication.Bindings("browser_authentication_binding",
             realm_id=realm.id,
             browser_flow=flow.alias)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -351,27 +351,27 @@
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         flow = keycloak.authentication.Flow("flow",
             realm_id=realm.id,
             alias="my-flow-alias")
         # first execution
-        execution_one = keycloak.authentication.Execution("executionOne",
+        execution_one = keycloak.authentication.Execution("execution_one",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="auth-cookie",
             requirement="ALTERNATIVE")
         # second execution
-        execution_two = keycloak.authentication.Execution("executionTwo",
+        execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
-        browser_authentication_binding = keycloak.authentication.Bindings("browserAuthenticationBinding",
+        browser_authentication_binding = keycloak.authentication.Bindings("browser_authentication_binding",
             realm_id=realm.id,
             browser_flow=flow.alias)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param BindingsArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,21 +180,21 @@
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         flow = keycloak.authentication.Flow("flow",
             realm_id=realm.id,
             alias="my-flow-alias")
         # first execution
-        execution_one = keycloak.authentication.Execution("executionOne",
+        execution_one = keycloak.authentication.Execution("execution_one",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="auth-cookie",
             requirement="ALTERNATIVE")
         # second execution
-        execution_two = keycloak.authentication.Execution("executionTwo",
+        execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         ```
         <!--End PulumiCodeChooser -->
@@ -242,21 +242,21 @@
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         flow = keycloak.authentication.Flow("flow",
             realm_id=realm.id,
             alias="my-flow-alias")
         # first execution
-        execution_one = keycloak.authentication.Execution("executionOne",
+        execution_one = keycloak.authentication.Execution("execution_one",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="auth-cookie",
             requirement="ALTERNATIVE")
         # second execution
-        execution_two = keycloak.authentication.Execution("executionTwo",
+        execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/subflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/__init__.pyi` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,25 +202,26 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        oidc_custom_identity_provider_mapping = keycloak.CustomIdentityProviderMapping("oidcCustomIdentityProviderMapping",
+        oidc_custom_identity_provider_mapping = keycloak.CustomIdentityProviderMapping("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="email-attribute-importer",
+            identity_provider_alias=oidc.alias,
             identity_provider_mapper="%s-user-attribute-idp-mapper",
             extra_config={
                 "syncMode": "INHERIT",
                 "Claim": "my-email-claim",
                 "UserAttribute": "email",
             })
         ```
@@ -261,25 +262,26 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        oidc_custom_identity_provider_mapping = keycloak.CustomIdentityProviderMapping("oidcCustomIdentityProviderMapping",
+        oidc_custom_identity_provider_mapping = keycloak.CustomIdentityProviderMapping("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="email-attribute-importer",
+            identity_provider_alias=oidc.alias,
             identity_provider_mapper="%s-user-attribute-idp-mapper",
             extra_config={
                 "syncMode": "INHERIT",
                 "Claim": "my-email-claim",
                 "UserAttribute": "email",
             })
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_user_federation.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,20 +366,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        custom_user_federation = keycloak.CustomUserFederation("customUserFederation",
-            enabled=True,
+            realm="test",
+            enabled=True)
+        custom_user_federation = keycloak.CustomUserFederation("custom_user_federation",
+            name="custom",
+            realm_id=realm.id,
             provider_id="custom",
-            realm_id=realm.id)
+            enabled=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -427,20 +428,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        custom_user_federation = keycloak.CustomUserFederation("customUserFederation",
-            enabled=True,
+            realm="test",
+            enabled=True)
+        custom_user_federation = keycloak.CustomUserFederation("custom_user_federation",
+            name="custom",
+            realm_id=realm.id,
             provider_id="custom",
-            realm_id=realm.id)
+            enabled=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        group = keycloak.Group("group", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
         default = keycloak.DefaultGroups("default",
-            group_ids=[group.id],
-            realm_id=realm.id)
+            realm_id=realm.id,
+            group_ids=[group.id])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -140,20 +142,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        group = keycloak.Group("group", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
         default = keycloak.DefaultGroups("default",
-            group_ids=[group.id],
-            realm_id=realm.id)
+            realm_id=realm.id,
+            group_ids=[group.id])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        default_roles = keycloak.DefaultRoles("defaultRoles",
+        default_roles = keycloak.DefaultRoles("default_roles",
             realm_id=realm.id,
             default_roles=["uma_authorization"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -160,15 +160,15 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        default_roles = keycloak.DefaultRoles("defaultRoles",
+        default_roles = keycloak.DefaultRoles("default_roles",
             realm_id=realm.id,
             default_roles=["uma_authorization"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,30 +268,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
-            client_id="test-client",
-            realm_id=realm.id)
-        saml_hardcode_attribute_mapper = keycloak.GenericClientProtocolMapper("samlHardcodeAttributeMapper",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=realm.id,
+            client_id="test-client")
+        saml_hardcode_attribute_mapper = keycloak.GenericClientProtocolMapper("saml_hardcode_attribute_mapper",
+            realm_id=realm.id,
             client_id=saml_client.id,
+            name="tes-mapper",
+            protocol="saml",
+            protocol_mapper="saml-hardcode-attribute-mapper",
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
-            },
-            protocol="saml",
-            protocol_mapper="saml-hardcode-attribute-mapper",
-            realm_id=realm.id)
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -340,30 +341,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
-            client_id="test-client",
-            realm_id=realm.id)
-        saml_hardcode_attribute_mapper = keycloak.GenericClientProtocolMapper("samlHardcodeAttributeMapper",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=realm.id,
+            client_id="test-client")
+        saml_hardcode_attribute_mapper = keycloak.GenericClientProtocolMapper("saml_hardcode_attribute_mapper",
+            realm_id=realm.id,
             client_id=saml_client.id,
+            name="tes-mapper",
+            protocol="saml",
+            protocol_mapper="saml-hardcode-attribute-mapper",
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
-            },
-            protocol="saml",
-            protocol_mapper="saml-hardcode-attribute-mapper",
-            realm_id=realm.id)
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_role_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['GenericClientRoleMapperArgs', 'GenericClientRoleMapper']
+__all__ = ['GenericRoleMapperArgs', 'GenericRoleMapper']
 
 @pulumi.input_type
-class GenericClientRoleMapperArgs:
+class GenericRoleMapperArgs:
     def __init__(__self__, *,
                  realm_id: pulumi.Input[str],
                  role_id: pulumi.Input[str],
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a GenericClientRoleMapper resource.
+        The set of arguments for constructing a GenericRoleMapper resource.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         """
         pulumi.set(__self__, "realm_id", realm_id)
         pulumi.set(__self__, "role_id", role_id)
@@ -78,22 +78,22 @@
 
     @client_scope_id.setter
     def client_scope_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_scope_id", value)
 
 
 @pulumi.input_type
-class _GenericClientRoleMapperState:
+class _GenericRoleMapperState:
     def __init__(__self__, *,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GenericClientRoleMapper resources.
+        Input properties used for looking up and filtering GenericRoleMapper resources.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
@@ -149,28 +149,26 @@
         return pulumi.get(self, "role_id")
 
     @role_id.setter
     def role_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_id", value)
 
 
-class GenericClientRoleMapper(pulumi.CustomResource):
+class GenericRoleMapper(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        !> **WARNING:** This resource is deprecated and will be removed in the next major version. Please use `GenericRoleMapper` instead.
-
-        Allow for creating and managing a client's scope mappings within Keycloak.
+        Allow for creating and managing a client's or client scope's role mappings within Keycloak.
 
         By default, all the user role mappings of the user are added as claims within the token (OIDC) or assertion (SAML). When
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
@@ -183,20 +181,22 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericClientRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
@@ -205,34 +205,38 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_a = keycloak.openid.Client("clientA",
+        client_a = keycloak.openid.Client("client_a",
             realm_id=realm.id,
             client_id="client-a",
+            name="client-a",
             enabled=True,
             access_type="BEARER-ONLY",
             full_scope_allowed=False)
-        client_role_a = keycloak.Role("clientRoleA",
+        client_role_a = keycloak.Role("client_role_a",
             realm_id=realm.id,
             client_id=client_a.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b = keycloak.openid.Client("clientB",
+        client_b = keycloak.openid.Client("client_b",
             realm_id=realm.id,
             client_id="client-b",
+            name="client-b",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role_b = keycloak.Role("clientRoleB",
+        client_role_b = keycloak.Role("client_role_b",
             realm_id=realm.id,
             client_id=client_b.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b_role_mapper = keycloak.GenericClientRoleMapper("clientBRoleMapper",
+        client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
@@ -241,19 +245,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        realm_role = keycloak.Role("realmRole",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericClientRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
@@ -265,22 +272,26 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client.id,
+            name="my-client-role",
             description="My Client Role")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_b_role_mapper = keycloak.GenericClientRoleMapper("clientBRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -292,34 +303,32 @@
         - When mapping a role to a client scope, use the format `{{realmId}}/client-scope/{{clientScopeId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
         Example:
 
         bash
 
         ```sh
-        $ pulumi import keycloak:index/genericClientRoleMapper:GenericClientRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
+        $ pulumi import keycloak:index/genericRoleMapper:GenericRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GenericClientRoleMapperArgs,
+                 args: GenericRoleMapperArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        !> **WARNING:** This resource is deprecated and will be removed in the next major version. Please use `GenericRoleMapper` instead.
-
-        Allow for creating and managing a client's scope mappings within Keycloak.
+        Allow for creating and managing a client's or client scope's role mappings within Keycloak.
 
         By default, all the user role mappings of the user are added as claims within the token (OIDC) or assertion (SAML). When
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
@@ -332,20 +341,22 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericClientRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
@@ -354,34 +365,38 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_a = keycloak.openid.Client("clientA",
+        client_a = keycloak.openid.Client("client_a",
             realm_id=realm.id,
             client_id="client-a",
+            name="client-a",
             enabled=True,
             access_type="BEARER-ONLY",
             full_scope_allowed=False)
-        client_role_a = keycloak.Role("clientRoleA",
+        client_role_a = keycloak.Role("client_role_a",
             realm_id=realm.id,
             client_id=client_a.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b = keycloak.openid.Client("clientB",
+        client_b = keycloak.openid.Client("client_b",
             realm_id=realm.id,
             client_id="client-b",
+            name="client-b",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role_b = keycloak.Role("clientRoleB",
+        client_role_b = keycloak.Role("client_role_b",
             realm_id=realm.id,
             client_id=client_b.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b_role_mapper = keycloak.GenericClientRoleMapper("clientBRoleMapper",
+        client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
@@ -390,19 +405,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        realm_role = keycloak.Role("realmRole",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericClientRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
@@ -414,22 +432,26 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client.id,
+            name="my-client-role",
             description="My Client Role")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_b_role_mapper = keycloak.GenericClientRoleMapper("clientBRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -441,24 +463,24 @@
         - When mapping a role to a client scope, use the format `{{realmId}}/client-scope/{{clientScopeId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
         Example:
 
         bash
 
         ```sh
-        $ pulumi import keycloak:index/genericClientRoleMapper:GenericClientRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
+        $ pulumi import keycloak:index/genericRoleMapper:GenericRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
         ```
 
         :param str resource_name: The name of the resource.
-        :param GenericClientRoleMapperArgs args: The arguments to use to populate this resource's properties.
+        :param GenericRoleMapperArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GenericClientRoleMapperArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(GenericRoleMapperArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -470,59 +492,59 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GenericClientRoleMapperArgs.__new__(GenericClientRoleMapperArgs)
+            __props__ = GenericRoleMapperArgs.__new__(GenericRoleMapperArgs)
 
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["client_scope_id"] = client_scope_id
             if realm_id is None and not opts.urn:
                 raise TypeError("Missing required property 'realm_id'")
             __props__.__dict__["realm_id"] = realm_id
             if role_id is None and not opts.urn:
                 raise TypeError("Missing required property 'role_id'")
             __props__.__dict__["role_id"] = role_id
-        super(GenericClientRoleMapper, __self__).__init__(
-            'keycloak:index/genericClientRoleMapper:GenericClientRoleMapper',
+        super(GenericRoleMapper, __self__).__init__(
+            'keycloak:index/genericRoleMapper:GenericRoleMapper',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             client_id: Optional[pulumi.Input[str]] = None,
             client_scope_id: Optional[pulumi.Input[str]] = None,
             realm_id: Optional[pulumi.Input[str]] = None,
-            role_id: Optional[pulumi.Input[str]] = None) -> 'GenericClientRoleMapper':
+            role_id: Optional[pulumi.Input[str]] = None) -> 'GenericRoleMapper':
         """
-        Get an existing GenericClientRoleMapper resource's state with the given name, id, and optional extra
+        Get an existing GenericRoleMapper resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GenericClientRoleMapperState.__new__(_GenericClientRoleMapperState)
+        __props__ = _GenericRoleMapperState.__new__(_GenericRoleMapperState)
 
         __props__.__dict__["client_id"] = client_id
         __props__.__dict__["client_scope_id"] = client_scope_id
         __props__.__dict__["realm_id"] = realm_id
         __props__.__dict__["role_id"] = role_id
-        return GenericClientRoleMapper(resource_name, opts=opts, __props__=__props__)
+        return GenericRoleMapper(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Output[Optional[str]]:
         """
         The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         """
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,20 +276,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client = keycloak.saml.Client("samlClient",
+        saml_client = keycloak.saml.Client("saml_client",
             realm_id=realm.id,
             client_id="test-client")
-        saml_hardcode_attribute_mapper = keycloak.GenericProtocolMapper("samlHardcodeAttributeMapper",
+        saml_hardcode_attribute_mapper = keycloak.GenericProtocolMapper("saml_hardcode_attribute_mapper",
             realm_id=realm.id,
             client_id=saml_client.id,
+            name="test-mapper",
             protocol="saml",
             protocol_mapper="saml-hardcode-attribute-mapper",
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
@@ -341,20 +342,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client = keycloak.saml.Client("samlClient",
+        saml_client = keycloak.saml.Client("saml_client",
             realm_id=realm.id,
             client_id="test-client")
-        saml_hardcode_attribute_mapper = keycloak.GenericProtocolMapper("samlHardcodeAttributeMapper",
+        saml_hardcode_attribute_mapper = keycloak.GenericProtocolMapper("saml_hardcode_attribute_mapper",
             realm_id=realm.id,
             client_id=saml_client.id,
+            name="test-mapper",
             protocol="saml",
             protocol_mapper="saml-hardcode-attribute-mapper",
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['GenericRoleMapperArgs', 'GenericRoleMapper']
+__all__ = ['GenericClientRoleMapperArgs', 'GenericClientRoleMapper']
 
 @pulumi.input_type
-class GenericRoleMapperArgs:
+class GenericClientRoleMapperArgs:
     def __init__(__self__, *,
                  realm_id: pulumi.Input[str],
                  role_id: pulumi.Input[str],
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a GenericRoleMapper resource.
+        The set of arguments for constructing a GenericClientRoleMapper resource.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         """
         pulumi.set(__self__, "realm_id", realm_id)
         pulumi.set(__self__, "role_id", role_id)
@@ -78,22 +78,22 @@
 
     @client_scope_id.setter
     def client_scope_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_scope_id", value)
 
 
 @pulumi.input_type
-class _GenericRoleMapperState:
+class _GenericClientRoleMapperState:
     def __init__(__self__, *,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GenericRoleMapper resources.
+        Input properties used for looking up and filtering GenericClientRoleMapper resources.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
@@ -149,26 +149,28 @@
         return pulumi.get(self, "role_id")
 
     @role_id.setter
     def role_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_id", value)
 
 
-class GenericRoleMapper(pulumi.CustomResource):
+class GenericClientRoleMapper(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_scope_id: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Allow for creating and managing a client's or client scope's role mappings within Keycloak.
+        !> **WARNING:** This resource is deprecated and will be removed in the next major version. Please use `GenericRoleMapper` instead.
+
+        Allow for creating and managing a client's scope mappings within Keycloak.
 
         By default, all the user role mappings of the user are added as claims within the token (OIDC) or assertion (SAML). When
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
@@ -181,20 +183,22 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
@@ -203,34 +207,38 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_a = keycloak.openid.Client("clientA",
+        client_a = keycloak.openid.Client("client_a",
             realm_id=realm.id,
             client_id="client-a",
+            name="client-a",
             enabled=True,
             access_type="BEARER-ONLY",
             full_scope_allowed=False)
-        client_role_a = keycloak.Role("clientRoleA",
+        client_role_a = keycloak.Role("client_role_a",
             realm_id=realm.id,
             client_id=client_a.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b = keycloak.openid.Client("clientB",
+        client_b = keycloak.openid.Client("client_b",
             realm_id=realm.id,
             client_id="client-b",
+            name="client-b",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role_b = keycloak.Role("clientRoleB",
+        client_role_b = keycloak.Role("client_role_b",
             realm_id=realm.id,
             client_id=client_b.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b_role_mapper = keycloak.GenericRoleMapper("clientBRoleMapper",
+        client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
@@ -239,19 +247,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        realm_role = keycloak.Role("realmRole",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
@@ -263,22 +274,26 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client.id,
+            name="my-client-role",
             description="My Client Role")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_b_role_mapper = keycloak.GenericRoleMapper("clientBRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -290,32 +305,34 @@
         - When mapping a role to a client scope, use the format `{{realmId}}/client-scope/{{clientScopeId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
         Example:
 
         bash
 
         ```sh
-        $ pulumi import keycloak:index/genericRoleMapper:GenericRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
+        $ pulumi import keycloak:index/genericClientRoleMapper:GenericClientRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GenericRoleMapperArgs,
+                 args: GenericClientRoleMapperArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Allow for creating and managing a client's or client scope's role mappings within Keycloak.
+        !> **WARNING:** This resource is deprecated and will be removed in the next major version. Please use `GenericRoleMapper` instead.
+
+        Allow for creating and managing a client's scope mappings within Keycloak.
 
         By default, all the user role mappings of the user are added as claims within the token (OIDC) or assertion (SAML). When
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
@@ -328,20 +345,22 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
@@ -350,34 +369,38 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_a = keycloak.openid.Client("clientA",
+        client_a = keycloak.openid.Client("client_a",
             realm_id=realm.id,
             client_id="client-a",
+            name="client-a",
             enabled=True,
             access_type="BEARER-ONLY",
             full_scope_allowed=False)
-        client_role_a = keycloak.Role("clientRoleA",
+        client_role_a = keycloak.Role("client_role_a",
             realm_id=realm.id,
             client_id=client_a.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b = keycloak.openid.Client("clientB",
+        client_b = keycloak.openid.Client("client_b",
             realm_id=realm.id,
             client_id="client-b",
+            name="client-b",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role_b = keycloak.Role("clientRoleB",
+        client_role_b = keycloak.Role("client_role_b",
             realm_id=realm.id,
             client_id=client_b.id,
+            name="my-client-role",
             description="My Client Role")
-        client_b_role_mapper = keycloak.GenericRoleMapper("clientBRoleMapper",
+        client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
@@ -386,19 +409,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        realm_role = keycloak.Role("realmRole",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        client_role_mapper = keycloak.GenericRoleMapper("clientRoleMapper",
+        client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
@@ -410,22 +436,26 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client.id,
+            name="my-client-role",
             description="My Client Role")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_b_role_mapper = keycloak.GenericRoleMapper("clientBRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="my-client-scope")
+        client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -437,24 +467,24 @@
         - When mapping a role to a client scope, use the format `{{realmId}}/client-scope/{{clientScopeId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
         Example:
 
         bash
 
         ```sh
-        $ pulumi import keycloak:index/genericRoleMapper:GenericRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
+        $ pulumi import keycloak:index/genericClientRoleMapper:GenericClientRoleMapper client_role_mapper my-realm/client/23888550-5dcd-41f6-85ba-554233021e9c/scope-mappings/ce51f004-bdfb-4dd5-a963-c4487d2dec5b/ff3aa49f-bc07-4030-8783-41918c3614a3
         ```
 
         :param str resource_name: The name of the resource.
-        :param GenericRoleMapperArgs args: The arguments to use to populate this resource's properties.
+        :param GenericClientRoleMapperArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GenericRoleMapperArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(GenericClientRoleMapperArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -466,59 +496,59 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GenericRoleMapperArgs.__new__(GenericRoleMapperArgs)
+            __props__ = GenericClientRoleMapperArgs.__new__(GenericClientRoleMapperArgs)
 
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["client_scope_id"] = client_scope_id
             if realm_id is None and not opts.urn:
                 raise TypeError("Missing required property 'realm_id'")
             __props__.__dict__["realm_id"] = realm_id
             if role_id is None and not opts.urn:
                 raise TypeError("Missing required property 'role_id'")
             __props__.__dict__["role_id"] = role_id
-        super(GenericRoleMapper, __self__).__init__(
-            'keycloak:index/genericRoleMapper:GenericRoleMapper',
+        super(GenericClientRoleMapper, __self__).__init__(
+            'keycloak:index/genericClientRoleMapper:GenericClientRoleMapper',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             client_id: Optional[pulumi.Input[str]] = None,
             client_scope_id: Optional[pulumi.Input[str]] = None,
             realm_id: Optional[pulumi.Input[str]] = None,
-            role_id: Optional[pulumi.Input[str]] = None) -> 'GenericRoleMapper':
+            role_id: Optional[pulumi.Input[str]] = None) -> 'GenericClientRoleMapper':
         """
-        Get an existing GenericRoleMapper resource's state with the given name, id, and optional extra
+        Get an existing GenericClientRoleMapper resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         :param pulumi.Input[str] client_scope_id: The ID of the client scope this role mapper should be added to. Conflicts with `client_id`. This argument is required if `client_id` is not set.
         :param pulumi.Input[str] realm_id: The realm this role mapper exists within.
         :param pulumi.Input[str] role_id: The ID of the role to be added to this role mapper.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GenericRoleMapperState.__new__(_GenericRoleMapperState)
+        __props__ = _GenericClientRoleMapperState.__new__(_GenericClientRoleMapperState)
 
         __props__.__dict__["client_id"] = client_id
         __props__.__dict__["client_scope_id"] = client_scope_id
         __props__.__dict__["realm_id"] = realm_id
         __props__.__dict__["role_id"] = role_id
-        return GenericRoleMapper(resource_name, opts=opts, __props__=__props__)
+        return GenericClientRoleMapper(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Output[Optional[str]]:
         """
         The ID of the client this role mapper should be added to. Conflicts with `client_scope_id`. This argument is required if `client_scope_id` is not set.
         """
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_client_description_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
-    saml_client_client_description_converter = keycloak.get_client_description_converter_output(realm_id=realm.id,
+    saml_client = keycloak.get_client_description_converter_output(realm_id=realm.id,
         body=\"\"\"	<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
         <md:SPSSODescriptor AuthnRequestsSigned="false" WantAssertionsSigned="false" protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
             <md:KeyDescriptor use="signing">
     			<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
     				<ds:X509Data>
     					<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
     					CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
@@ -420,17 +420,17 @@
     			</ds:KeyInfo>
     		</md:KeyDescriptor>
     		<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
             <md:AssertionConsumerService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://localhost/acs/saml/" index="1"/>
         </md:SPSSODescriptor>
     </md:EntityDescriptor>
     \"\"\")
-    saml_client_client = keycloak.saml.Client("samlClientClient",
+    saml_client_client = keycloak.saml.Client("saml_client",
         realm_id=realm.id,
-        client_id=saml_client_client_description_converter.client_id)
+        client_id=saml_client.client_id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str body: The body of the request to convert.
     :param str realm_id: The realm to use for the client description converter API call.
     """
@@ -495,15 +495,15 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
-    saml_client_client_description_converter = keycloak.get_client_description_converter_output(realm_id=realm.id,
+    saml_client = keycloak.get_client_description_converter_output(realm_id=realm.id,
         body=\"\"\"	<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
         <md:SPSSODescriptor AuthnRequestsSigned="false" WantAssertionsSigned="false" protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
             <md:KeyDescriptor use="signing">
     			<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
     				<ds:X509Data>
     					<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
     					CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
@@ -524,17 +524,17 @@
     			</ds:KeyInfo>
     		</md:KeyDescriptor>
     		<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
             <md:AssertionConsumerService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://localhost/acs/saml/" index="1"/>
         </md:SPSSODescriptor>
     </md:EntityDescriptor>
     \"\"\")
-    saml_client_client = keycloak.saml.Client("samlClientClient",
+    saml_client_client = keycloak.saml.Client("saml_client",
         realm_id=realm.id,
-        client_id=saml_client_client_description_converter.client_id)
+        client_id=saml_client.client_id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str body: The body of the request to convert.
     :param str realm_id: The realm to use for the client description converter API call.
     """
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,15 +572,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.get_realm(realm="my-realm")
-    group = keycloak.Role("group", realm_id=data["keycloak_realm"]["id"])
+    # use the data source
+    group = keycloak.Role("group",
+        realm_id=id,
+        name="group")
     ```
     <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
 
@@ -688,15 +691,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.get_realm(realm="my-realm")
-    group = keycloak.Role("group", realm_id=data["keycloak_realm"]["id"])
+    # use the data source
+    group = keycloak.Role("group",
+        realm_id=id,
+        name="group")
     ```
     <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
+    # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     pulumi.export("keycloakUserId", default_admin_user.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
@@ -210,14 +211,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
+    # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     pulumi.export("keycloakUserId", default_admin_user.id)
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user_realm_roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,16 +84,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
+    # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
+    # use the keycloak_user_realm_roles data source to list role names
     user_realm_roles = keycloak.get_user_realm_roles(realm_id=master_realm.id,
         user_id=default_admin_user.id)
     pulumi.export("keycloakUserRoleNames", user_realm_roles.role_names)
     ```
     <!--End PulumiCodeChooser -->
 
 
@@ -124,16 +126,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
+    # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
+    # use the keycloak_user_realm_roles data source to list role names
     user_realm_roles = keycloak.get_user_realm_roles(realm_id=master_realm.id,
         user_id=default_admin_user.id)
     pulumi.export("keycloakUserRoleNames", user_realm_roles.role_names)
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,27 +162,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        parent_group = keycloak.Group("parentGroup", realm_id=realm.id)
-        child_group = keycloak.Group("childGroup",
+            realm="my-realm",
+            enabled=True)
+        parent_group = keycloak.Group("parent_group",
+            realm_id=realm.id,
+            name="parent-group")
+        child_group = keycloak.Group("child_group",
+            realm_id=realm.id,
             parent_id=parent_group.id,
-            realm_id=realm.id)
-        child_group_with_optional_attributes = keycloak.Group("childGroupWithOptionalAttributes",
+            name="child-group")
+        child_group_with_optional_attributes = keycloak.Group("child_group_with_optional_attributes",
+            realm_id=realm.id,
+            parent_id=parent_group.id,
+            name="child-group-with-optional-attributes",
             attributes={
                 "key1": "value1",
                 "key2": "value2",
-            },
-            parent_id=parent_group.id,
-            realm_id=realm.id)
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -231,27 +235,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        parent_group = keycloak.Group("parentGroup", realm_id=realm.id)
-        child_group = keycloak.Group("childGroup",
+            realm="my-realm",
+            enabled=True)
+        parent_group = keycloak.Group("parent_group",
+            realm_id=realm.id,
+            name="parent-group")
+        child_group = keycloak.Group("child_group",
+            realm_id=realm.id,
             parent_id=parent_group.id,
-            realm_id=realm.id)
-        child_group_with_optional_attributes = keycloak.Group("childGroupWithOptionalAttributes",
+            name="child-group")
+        child_group_with_optional_attributes = keycloak.Group("child_group_with_optional_attributes",
+            realm_id=realm.id,
+            parent_id=parent_group.id,
+            name="child-group-with-optional-attributes",
             attributes={
                 "key1": "value1",
                 "key2": "value2",
-            },
-            parent_id=parent_group.id,
-            realm_id=realm.id)
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_memberships.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,24 +127,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        group = keycloak.Group("group", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="my-user")
-        group_members = keycloak.GroupMemberships("groupMembers",
+        group_members = keycloak.GroupMemberships("group_members",
+            realm_id=realm.id,
             group_id=group.id,
-            members=[user.username],
-            realm_id=realm.id)
+            members=[user.username])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -187,24 +189,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        group = keycloak.Group("group", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="my-user")
-        group_members = keycloak.GroupMemberships("groupMembers",
+        group_members = keycloak.GroupMemberships("group_members",
+            realm_id=realm.id,
             group_id=group.id,
-            members=[user.username],
-            realm_id=realm.id)
+            members=[user.username])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,32 +149,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        realm_role = keycloak.Role("realmRole",
-            description="My Realm Role",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role",
+            description="My Realm Role")
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
-        group = keycloak.Group("group", realm_id=realm.id)
-        group_roles = keycloak.GroupRoles("groupRoles",
-            group_id=group.id,
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
+        group_roles = keycloak.GroupRoles("group_roles",
+            realm_id=realm.id,
+            group_id=group.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
         <!--End PulumiCodeChooser -->
 
@@ -224,32 +229,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        realm_role = keycloak.Role("realmRole",
-            description="My Realm Role",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role",
+            description="My Realm Role")
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
-        group = keycloak.Group("group", realm_id=realm.id)
-        group_roles = keycloak.GroupRoles("groupRoles",
-            group_id=group.id,
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
+        group = keycloak.Group("group",
+            realm_id=realm.id,
+            name="my-group")
+        group_roles = keycloak.GroupRoles("group_roles",
+            realm_id=realm.id,
+            group_id=group.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,24 +264,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com")
-        oidc_hardcoded_attribute_identity_provider_mapper = keycloak.HardcodedAttributeIdentityProviderMapper("oidcHardcodedAttributeIdentityProviderMapper",
+        oidc_hardcoded_attribute_identity_provider_mapper = keycloak.HardcodedAttributeIdentityProviderMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="hardcodedUserSessionAttribute",
+            identity_provider_alias=oidc.alias,
             attribute_name="attribute",
             attribute_value="value",
             user_session=True,
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
@@ -313,24 +314,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com")
-        oidc_hardcoded_attribute_identity_provider_mapper = keycloak.HardcodedAttributeIdentityProviderMapper("oidcHardcodedAttributeIdentityProviderMapper",
+        oidc_hardcoded_attribute_identity_provider_mapper = keycloak.HardcodedAttributeIdentityProviderMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="hardcodedUserSessionAttribute",
+            identity_provider_alias=oidc.alias,
             attribute_name="attribute",
             attribute_value="value",
             user_session=True,
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,27 +199,29 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        oidc_hardcoded_role_identity_mapper = keycloak.HardcodedRoleIdentityMapper("oidcHardcodedRoleIdentityMapper",
+        oidc_hardcoded_role_identity_mapper = keycloak.HardcodedRoleIdentityMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="hardcodedRole",
+            identity_provider_alias=oidc.alias,
             role="my-realm-role",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
         <!--End PulumiCodeChooser -->
 
@@ -247,27 +249,29 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        oidc_identity_provider = keycloak.oidc.IdentityProvider("oidcIdentityProvider",
+        oidc = keycloak.oidc.IdentityProvider("oidc",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com")
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
-        oidc_hardcoded_role_identity_mapper = keycloak.HardcodedRoleIdentityMapper("oidcHardcodedRoleIdentityMapper",
+        oidc_hardcoded_role_identity_mapper = keycloak.HardcodedRoleIdentityMapper("oidc",
             realm=realm.id,
-            identity_provider_alias=oidc_identity_provider.alias,
+            name="hardcodedRole",
+            identity_provider_alias=oidc.alias,
             role="my-realm-role",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,35 +230,36 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        token_exchange_realm = keycloak.Realm("tokenExchangeRealm",
+        token_exchange_realm = keycloak.Realm("token_exchange_realm",
             realm="token-exchange_destination_realm",
             enabled=True)
-        token_exchange_my_oidc_idp = keycloak.oidc.IdentityProvider("tokenExchangeMyOidcIdp",
+        token_exchange_my_oidc_idp = keycloak.oidc.IdentityProvider("token_exchange_my_oidc_idp",
             realm=token_exchange_realm.id,
             alias="myIdp",
             authorization_url="http://localhost:8080/auth/realms/someRealm/protocol/openid-connect/auth",
             token_url="http://localhost:8080/auth/realms/someRealm/protocol/openid-connect/token",
             client_id="clientId",
             client_secret="secret",
             default_scopes="openid")
-        token_exchange_webapp_client = keycloak.openid.Client("token-exchangeWebappClient",
+        token_exchange_webapp_client = keycloak.openid.Client("token-exchange_webapp_client",
             realm_id=token_exchange_realm.id,
+            name="webapp_client",
             client_id="webapp_client",
             client_secret="secret",
             description="a webapp client on the destination realm",
             access_type="CONFIDENTIAL",
             standard_flow_enabled=True,
             valid_redirect_uris=["http://localhost:8080/*"])
         #relevant part
-        oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidcIdpPermission",
+        oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidc_idp_permission",
             realm_id=token_exchange_realm.id,
             provider_alias=token_exchange_my_oidc_idp.alias,
             policy_type="client",
             clients=[token_exchange_webapp_client.id])
         ```
         <!--End PulumiCodeChooser -->
 
@@ -293,35 +294,36 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        token_exchange_realm = keycloak.Realm("tokenExchangeRealm",
+        token_exchange_realm = keycloak.Realm("token_exchange_realm",
             realm="token-exchange_destination_realm",
             enabled=True)
-        token_exchange_my_oidc_idp = keycloak.oidc.IdentityProvider("tokenExchangeMyOidcIdp",
+        token_exchange_my_oidc_idp = keycloak.oidc.IdentityProvider("token_exchange_my_oidc_idp",
             realm=token_exchange_realm.id,
             alias="myIdp",
             authorization_url="http://localhost:8080/auth/realms/someRealm/protocol/openid-connect/auth",
             token_url="http://localhost:8080/auth/realms/someRealm/protocol/openid-connect/token",
             client_id="clientId",
             client_secret="secret",
             default_scopes="openid")
-        token_exchange_webapp_client = keycloak.openid.Client("token-exchangeWebappClient",
+        token_exchange_webapp_client = keycloak.openid.Client("token-exchange_webapp_client",
             realm_id=token_exchange_realm.id,
+            name="webapp_client",
             client_id="webapp_client",
             client_secret="secret",
             description="a webapp client on the destination realm",
             access_type="CONFIDENTIAL",
             standard_flow_enabled=True,
             valid_redirect_uris=["http://localhost:8080/*"])
         #relevant part
-        oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidcIdpPermission",
+        oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidc_idp_permission",
             realm_id=token_exchange_realm.id,
             provider_alias=token_exchange_my_oidc_idp.alias,
             policy_type="client",
             clients=[token_exchange_webapp_client.id])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/custom_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/custom_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,30 +242,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        custom_mapper = keycloak.ldap.CustomMapper("customMapper",
-            realm_id=keycloak_ldap_user_federation["openldap"]["realm_id"],
-            ldap_user_federation_id=keycloak_ldap_user_federation["openldap"]["id"],
+        custom_mapper = keycloak.ldap.CustomMapper("custom_mapper",
+            name="custom-mapper",
+            realm_id=openldap["realmId"],
+            ldap_user_federation_id=openldap["id"],
             provider_id="custom-provider-registered-in-keycloak",
             provider_type="com.example.custom.ldap.mappers.CustomMapper",
             config={
                 "attribute.name": "name",
                 "attribute.value": "value",
             })
         ```
@@ -315,30 +317,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        custom_mapper = keycloak.ldap.CustomMapper("customMapper",
-            realm_id=keycloak_ldap_user_federation["openldap"]["realm_id"],
-            ldap_user_federation_id=keycloak_ldap_user_federation["openldap"]["id"],
+        custom_mapper = keycloak.ldap.CustomMapper("custom_mapper",
+            name="custom-mapper",
+            realm_id=openldap["realmId"],
+            ldap_user_federation_id=openldap["id"],
             provider_id="custom-provider-registered-in-keycloak",
             provider_type="com.example.custom.ldap.mappers.CustomMapper",
             config={
                 "attribute.name": "name",
                 "attribute.value": "value",
             })
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,33 +217,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldapFullNameMapper",
-            ldap_full_name_attribute="cn",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldap_full_name_mapper",
+            realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
-            realm_id=realm.id)
+            name="full-name-mapper",
+            ldap_full_name_attribute="cn")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -285,33 +287,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldapFullNameMapper",
-            ldap_full_name_attribute="cn",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldap_full_name_mapper",
+            realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
-            realm_id=realm.id)
+            name="full-name-mapper",
+            ldap_full_name_attribute="cn")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/group_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,39 +514,41 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_group_mapper = keycloak.ldap.GroupMapper("ldapGroupMapper",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_group_mapper = keycloak.ldap.GroupMapper("ldap_group_mapper",
+            realm_id=realm.id,
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="group-mapper",
+            ldap_groups_dn="dc=example,dc=org",
             group_name_ldap_attribute="cn",
             group_object_classes=["groupOfNames"],
-            ldap_groups_dn="dc=example,dc=org",
-            ldap_user_federation_id=ldap_user_federation.id,
-            memberof_ldap_attribute="memberOf",
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
-            realm_id=realm.id)
+            memberof_ldap_attribute="memberOf")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -600,39 +602,41 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_group_mapper = keycloak.ldap.GroupMapper("ldapGroupMapper",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_group_mapper = keycloak.ldap.GroupMapper("ldap_group_mapper",
+            realm_id=realm.id,
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="group-mapper",
+            ldap_groups_dn="dc=example,dc=org",
             group_name_ldap_attribute="cn",
             group_object_classes=["groupOfNames"],
-            ldap_groups_dn="dc=example,dc=org",
-            ldap_user_federation_id=ldap_user_federation.id,
-            memberof_ldap_attribute="memberOf",
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
-            realm_id=realm.id)
+            memberof_ldap_attribute="memberOf")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,31 +207,33 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin",
             sync_registrations=True)
-        assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assignBarToFoo",
+        assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assign_bar_to_foo",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-foo-to-bar",
             attribute_name="foo",
             attribute_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -274,31 +276,33 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin",
             sync_registrations=True)
-        assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assignBarToFoo",
+        assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assign_bar_to_foo",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-foo-to-bar",
             attribute_name="foo",
             attribute_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,31 +173,35 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        realm_group = keycloak.Group("realmGroup", realm_id=realm.id)
-        assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assignGroupToUsers",
+        realm_group = keycloak.Group("realm_group",
+            realm_id=realm.id,
+            name="my-group")
+        assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assign_group_to_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-group-to-users",
             group=realm_group.name)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
@@ -236,31 +240,35 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        realm_group = keycloak.Group("realmGroup", realm_id=realm.id)
-        assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assignGroupToUsers",
+        realm_group = keycloak.Group("realm_group",
+            realm_id=realm.id,
+            name="my-group")
+        assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assign_group_to_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-group-to-users",
             group=realm_group.name)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,30 +173,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assignAdminRoleToAllUsers",
+        assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assign_admin_role_to_all_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-admin-role-to-all-users",
             role="admin")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
@@ -236,30 +238,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assignAdminRoleToAllUsers",
+        assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assign_admin_role_to_all_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="assign-admin-role-to-all-users",
             role="admin")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,31 +145,33 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="ad",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="objectGUID",
             user_object_classes=[
                 "person",
                 "organizationalPerson",
                 "user",
             ],
             connection_url="ldap://my-ad-server",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msadLdsUserAccountControlMapper",
+        msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msad_lds_user_account_control_mapper",
             realm_id=realm.id,
-            ldap_user_federation_id=ldap_user_federation.id)
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="msad-lds-user-account-control-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
@@ -210,31 +212,33 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="ad",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="objectGUID",
             user_object_classes=[
                 "person",
                 "organizationalPerson",
                 "user",
             ],
             connection_url="ldap://my-ad-server",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msadLdsUserAccountControlMapper",
+        msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msad_lds_user_account_control_mapper",
             realm_id=realm.id,
-            ldap_user_federation_id=ldap_user_federation.id)
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="msad-lds-user-account-control-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,33 +170,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://my-ad-server",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="ad",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="objectGUID",
             user_object_classes=[
                 "person",
                 "organizationalPerson",
                 "user",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://my-ad-server",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="objectGUID")
-        msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msadUserAccountControlMapper",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msad_user_account_control_mapper",
+            realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
-            realm_id=realm.id)
+            name="msad-user-account-control-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -238,33 +240,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://my-ad-server",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="ad",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="objectGUID",
             user_object_classes=[
                 "person",
                 "organizationalPerson",
                 "user",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://my-ad-server",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="objectGUID")
-        msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msadUserAccountControlMapper",
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msad_user_account_control_mapper",
+            realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
-            realm_id=realm.id)
+            name="msad-user-account-control-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/role_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,30 +532,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        ldap_role_mapper = keycloak.ldap.RoleMapper("ldapRoleMapper",
+        ldap_role_mapper = keycloak.ldap.RoleMapper("ldap_role_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="role-mapper",
             ldap_roles_dn="dc=example,dc=org",
             role_name_ldap_attribute="cn",
             role_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             user_roles_retrieve_strategy="GET_ROLES_FROM_USER_MEMBEROF_ATTRIBUTE",
@@ -612,30 +614,32 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
             username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
             uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
-        ldap_role_mapper = keycloak.ldap.RoleMapper("ldapRoleMapper",
+        ldap_role_mapper = keycloak.ldap.RoleMapper("ldap_role_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
+            name="role-mapper",
             ldap_roles_dn="dc=example,dc=org",
             role_name_ldap_attribute="cn",
             role_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             user_roles_retrieve_strategy="GET_ROLES_FROM_USER_MEMBEROF_ATTRIBUTE",
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,34 +372,36 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldapUserAttributeMapper",
-            ldap_attribute="bar",
-            ldap_user_federation_id=ldap_user_federation.id,
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldap_user_attribute_mapper",
             realm_id=realm.id,
-            user_model_attribute="foo")
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="user-attribute-mapper",
+            user_model_attribute="foo",
+            ldap_attribute="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -450,34 +452,36 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_url="ldap://openldap",
-            rdn_ldap_attribute="cn",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
             realm_id=realm.id,
+            username_ldap_attribute="cn",
+            rdn_ldap_attribute="cn",
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
-        ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldapUserAttributeMapper",
-            ldap_attribute="bar",
-            ldap_user_federation_id=ldap_user_federation.id,
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin")
+        ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldap_user_attribute_mapper",
             realm_id=realm.id,
-            user_model_attribute="foo")
+            ldap_user_federation_id=ldap_user_federation.id,
+            name="user-attribute-mapper",
+            user_model_attribute="foo",
+            ldap_attribute="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_federation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,32 +1098,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
+            realm_id=realm.id,
             enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_timeout="5s",
-            connection_url="ldap://openldap",
-            enabled=True,
+            username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
-            read_timeout="10s",
-            realm_id=realm.id,
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin",
+            connection_timeout="5s",
+            read_timeout="10s")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -1221,32 +1222,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
+            realm="test",
+            enabled=True)
+        ldap_user_federation = keycloak.ldap.UserFederation("ldap_user_federation",
+            name="openldap",
+            realm_id=realm.id,
             enabled=True,
-            realm="test")
-        ldap_user_federation = keycloak.ldap.UserFederation("ldapUserFederation",
-            bind_credential="admin",
-            bind_dn="cn=admin,dc=example,dc=org",
-            connection_timeout="5s",
-            connection_url="ldap://openldap",
-            enabled=True,
+            username_ldap_attribute="cn",
             rdn_ldap_attribute="cn",
-            read_timeout="10s",
-            realm_id=realm.id,
+            uuid_ldap_attribute="entryDN",
             user_object_classes=[
                 "simpleSecurityObject",
                 "organizationalRole",
             ],
-            username_ldap_attribute="cn",
+            connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
-            uuid_ldap_attribute="entryDN")
+            bind_dn="cn=admin,dc=example,dc=org",
+            bind_credential="admin",
+            connection_timeout="5s",
+            read_timeout="10s")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,16 +809,16 @@
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         google = keycloak.oidc.GoogleIdentityProvider("google",
             realm=realm.id,
-            client_id=var["google_identity_provider_client_id"],
-            client_secret=var["google_identity_provider_client_secret"],
+            client_id=google_identity_provider_client_id,
+            client_secret=google_identity_provider_client_secret,
             trust_email=True,
             hosted_domain="example.com",
             sync_mode="IMPORT",
             extra_config={
                 "myCustomConfigKey": "myValue",
             })
         ```
@@ -879,16 +879,16 @@
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         google = keycloak.oidc.GoogleIdentityProvider("google",
             realm=realm.id,
-            client_id=var["google_identity_provider_client_id"],
-            client_secret=var["google_identity_provider_client_secret"],
+            client_id=google_identity_provider_client_id,
+            client_secret=google_identity_provider_client_secret,
             trust_email=True,
             hosted_domain="example.com",
             sync_mode="IMPORT",
             extra_config={
                 "myCustomConfigKey": "myValue",
             })
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1069,15 +1069,15 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_identity_provider = keycloak.oidc.IdentityProvider("realmIdentityProvider",
+        realm_identity_provider = keycloak.oidc.IdentityProvider("realm_identity_provider",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com",
             extra_config={
@@ -1148,15 +1148,15 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_identity_provider = keycloak.oidc.IdentityProvider("realmIdentityProvider",
+        realm_identity_provider = keycloak.oidc.IdentityProvider("realm_identity_provider",
             realm=realm.id,
             alias="my-idp",
             authorization_url="https://authorizationurl.com",
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com",
             extra_config={
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,44 +310,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            included_custom_audience="foo",
-            realm_id=realm.id)
+            name="audience-mapper",
+            included_custom_audience="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            included_custom_audience="foo",
-            realm_id=realm.id)
+            name="audience-mapper",
+            included_custom_audience="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -399,44 +404,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            included_custom_audience="foo",
-            realm_id=realm.id)
+            name="audience-mapper",
+            included_custom_audience="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            included_custom_audience="foo",
-            realm_id=realm.id)
+            name="audience-mapper",
+            included_custom_audience="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,38 +179,42 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
-            client_id=openid_client.id)
+            client_id=openid_client.id,
+            name="my-audience-resolve-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -260,38 +264,42 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
-            client_id=openid_client.id)
+            client_id=openid_client.id,
+            name="my-audience-resolve-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,38 +184,42 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
-            client_id=openid_client.id)
+            client_id=openid_client.id,
+            name="my-audience-resolve-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -265,38 +269,42 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audienceMapper",
+        audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
-            client_id=openid_client.id)
+            client_id=openid_client.id,
+            name="my-audience-resolve-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1169,21 +1169,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
@@ -1249,21 +1250,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,31 +110,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="CONFIDENTIAL",
+            realm_id=realm.id,
             client_id="test-client",
-            realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_default_scopes = keycloak.openid.ClientDefaultScopes("clientDefaultScopes",
+            access_type="CONFIDENTIAL")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        client_default_scopes = keycloak.openid.ClientDefaultScopes("client_default_scopes",
+            realm_id=realm.id,
             client_id=client.id,
             default_scopes=[
                 "profile",
                 "email",
                 "roles",
                 "web-origins",
                 client_scope.name,
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -161,31 +163,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="CONFIDENTIAL",
+            realm_id=realm.id,
             client_id="test-client",
-            realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_default_scopes = keycloak.openid.ClientDefaultScopes("clientDefaultScopes",
+            access_type="CONFIDENTIAL")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        client_default_scopes = keycloak.openid.ClientDefaultScopes("client_default_scopes",
+            realm_id=realm.id,
             client_id=client.id,
             default_scopes=[
                 "profile",
                 "email",
                 "roles",
                 "web-origins",
                 client_scope.name,
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,30 +110,32 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="CONFIDENTIAL",
+            realm_id=realm.id,
             client_id="test-client",
-            realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_optional_scopes = keycloak.openid.ClientOptionalScopes("clientOptionalScopes",
+            access_type="CONFIDENTIAL")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        client_optional_scopes = keycloak.openid.ClientOptionalScopes("client_optional_scopes",
+            realm_id=realm.id,
             client_id=client.id,
             optional_scopes=[
                 "address",
                 "phone",
                 "offline_access",
                 client_scope.name,
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -160,30 +162,32 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="CONFIDENTIAL",
+            realm_id=realm.id,
             client_id="test-client",
-            realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        client_optional_scopes = keycloak.openid.ClientOptionalScopes("clientOptionalScopes",
+            access_type="CONFIDENTIAL")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        client_optional_scopes = keycloak.openid.ClientOptionalScopes("client_optional_scopes",
+            realm_id=realm.id,
             client_id=client.id,
             optional_scopes=[
                 "address",
                 "phone",
                 "offline_access",
                 client_scope.name,
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,27 +272,29 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             client_id="openid_client",
+            name="openid_client",
             realm_id=realm.id,
             access_type="CONFIDENTIAL",
             service_accounts_enabled=True)
-        my_permission = keycloak.openid.ClientPermissions("myPermission",
+        my_permission = keycloak.openid.ClientPermissions("my_permission",
             realm_id=realm.id,
             client_id=openid_client.id)
         realm_management = keycloak.openid.get_client(realm_id="my-realm",
             client_id="realm-management")
-        token_exchange = keycloak.openid.ClientPolicy("tokenExchange",
+        token_exchange = keycloak.openid.ClientPolicy("token_exchange",
             resource_server_id=realm_management.id,
             realm_id=realm.id,
+            name="my-policy",
             logic="POSITIVE",
             decision_strategy="UNANIMOUS",
             clients=[openid_client.id])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -322,27 +324,29 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             client_id="openid_client",
+            name="openid_client",
             realm_id=realm.id,
             access_type="CONFIDENTIAL",
             service_accounts_enabled=True)
-        my_permission = keycloak.openid.ClientPermissions("myPermission",
+        my_permission = keycloak.openid.ClientPermissions("my_permission",
             realm_id=realm.id,
             client_id=openid_client.id)
         realm_management = keycloak.openid.get_client(realm_id="my-realm",
             client_id="realm-management")
-        token_exchange = keycloak.openid.ClientPolicy("tokenExchange",
+        token_exchange = keycloak.openid.ClientPolicy("token_exchange",
             resource_server_id=realm_management.id,
             realm_id=realm.id,
+            name="my-policy",
             logic="POSITIVE",
             decision_strategy="UNANIMOUS",
             clients=[openid_client.id])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client_scope = keycloak.openid.ClientScope("openidClientScope",
-            description="When requested, this scope will map a user's group memberships to a claim",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        openid_client_scope = keycloak.openid.ClientScope("openid_client_scope",
+            realm_id=realm.id,
+            name="groups",
+            description="When requested, this scope will map a user's group memberships to a claim")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -249,19 +250,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client_scope = keycloak.openid.ClientScope("openidClientScope",
-            description="When requested, this scope will map a user's group memberships to a claim",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        openid_client_scope = keycloak.openid.ClientScope("openid_client_scope",
+            realm_id=realm.id,
+            name="groups",
+            description="When requested, this scope will map a user's group memberships to a claim")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,19 +142,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_role = keycloak.Role("realmRole", realm_id=realm.id)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role")
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
+            name="client",
             service_accounts_enabled=True)
-        client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("clientServiceAccountRole",
+        client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("client_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client.service_account_user_id,
             role=realm_role.name)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -194,19 +197,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_role = keycloak.Role("realmRole", realm_id=realm.id)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role")
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
+            name="client",
             service_accounts_enabled=True)
-        client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("clientServiceAccountRole",
+        client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("client_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client.service_account_user_id,
             role=realm_role.name)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,24 +175,28 @@
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         # client1 provides a role to other clients
-        client1 = keycloak.openid.Client("client1", realm_id=realm.id)
-        client1_role = keycloak.Role("client1Role",
+        client1 = keycloak.openid.Client("client1",
+            realm_id=realm.id,
+            name="client1")
+        client1_role = keycloak.Role("client1_role",
             realm_id=realm.id,
             client_id=client1.id,
+            name="my-client1-role",
             description="A role that client1 provides")
         # client2 is assigned the role of client1
         client2 = keycloak.openid.Client("client2",
             realm_id=realm.id,
+            name="client2",
             service_accounts_enabled=True)
-        client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2ServiceAccountRole",
+        client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client2.service_account_user_id,
             client_id=client1.id,
             role=client1_role.name)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -235,24 +239,28 @@
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         # client1 provides a role to other clients
-        client1 = keycloak.openid.Client("client1", realm_id=realm.id)
-        client1_role = keycloak.Role("client1Role",
+        client1 = keycloak.openid.Client("client1",
+            realm_id=realm.id,
+            name="client1")
+        client1_role = keycloak.Role("client1_role",
             realm_id=realm.id,
             client_id=client1.id,
+            name="my-client1-role",
             description="A role that client1 provides")
         # client2 is assigned the role of client1
         client2 = keycloak.openid.Client("client2",
             realm_id=realm.id,
+            name="client2",
             service_accounts_enabled=True)
-        client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2ServiceAccountRole",
+        client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client2.service_account_user_id,
             client_id=client1.id,
             role=client1_role.name)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,42 +254,47 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        full_name_mapper = keycloak.openid.FullNameProtocolMapper("fullNameMapper",
+        full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="full-name-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        full_name_mapper = keycloak.openid.FullNameProtocolMapper("fullNameMapper",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="full-name-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -337,42 +342,47 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        full_name_mapper = keycloak.openid.FullNameProtocolMapper("fullNameMapper",
+        full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="full-name-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        full_name_mapper = keycloak.openid.FullNameProtocolMapper("fullNameMapper",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="full-name-mapper")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,14 +469,15 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.openid.get_client(realm_id="my-realm",
         client_id="realm-management")
+    # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
     <!--End PulumiCodeChooser -->
 
     ### Argument Reference
@@ -571,14 +572,15 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.openid.get_client(realm_id="my-realm",
         client_id="realm-management")
+    # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
     <!--End PulumiCodeChooser -->
 
     ### Argument Reference
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,35 +172,38 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
-    client_with_authz = keycloak.openid.Client("clientWithAuthz",
+    client_with_authz = keycloak.openid.Client("client_with_authz",
         client_id="client-with-authz",
+        name="client-with-authz",
         realm_id=realm.id,
         access_type="CONFIDENTIAL",
         service_accounts_enabled=True,
         authorization=keycloak.openid.ClientAuthorizationArgs(
             policy_enforcement_mode="ENFORCING",
         ))
     default_permission = keycloak.openid.get_client_authorization_policy_output(realm_id=realm.id,
         resource_server_id=client_with_authz.resource_server_id,
         name="Default Permission")
     resource = keycloak.openid.ClientAuthorizationResource("resource",
         resource_server_id=client_with_authz.resource_server_id,
+        name="authorization-resource",
         realm_id=realm.id,
         uris=["/endpoint/*"],
         attributes={
             "foo": "bar",
         })
     permission = keycloak.openid.ClientAuthorizationPermission("permission",
         resource_server_id=client_with_authz.resource_server_id,
         realm_id=realm.id,
+        name="authorization-permission",
         policies=[default_permission.id],
         resources=[resource.id])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the authorization policy.
@@ -246,35 +249,38 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
-    client_with_authz = keycloak.openid.Client("clientWithAuthz",
+    client_with_authz = keycloak.openid.Client("client_with_authz",
         client_id="client-with-authz",
+        name="client-with-authz",
         realm_id=realm.id,
         access_type="CONFIDENTIAL",
         service_accounts_enabled=True,
         authorization=keycloak.openid.ClientAuthorizationArgs(
             policy_enforcement_mode="ENFORCING",
         ))
     default_permission = keycloak.openid.get_client_authorization_policy_output(realm_id=realm.id,
         resource_server_id=client_with_authz.resource_server_id,
         name="Default Permission")
     resource = keycloak.openid.ClientAuthorizationResource("resource",
         resource_server_id=client_with_authz.resource_server_id,
+        name="authorization-resource",
         realm_id=realm.id,
         uris=["/endpoint/*"],
         attributes={
             "foo": "bar",
         })
     permission = keycloak.openid.ClientAuthorizationPermission("permission",
         resource_server_id=client_with_authz.resource_server_id,
         realm_id=realm.id,
+        name="authorization-permission",
         policies=[default_permission.id],
         resources=[resource.id])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the authorization policy.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,18 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     offline_access = keycloak.openid.get_client_scope(realm_id="my-realm",
         name="offline_access")
     # use the data source
-    audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+    audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
         realm_id=offline_access.realm_id,
         client_scope_id=offline_access.id,
+        name="audience-mapper",
         included_custom_audience="foo")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the client scope.
     :param str realm_id: The realm id.
@@ -154,17 +155,18 @@
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     offline_access = keycloak.openid.get_client_scope(realm_id="my-realm",
         name="offline_access")
     # use the data source
-    audience_mapper = keycloak.openid.AudienceProtocolMapper("audienceMapper",
+    audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
         realm_id=offline_access.realm_id,
         client_scope_id=offline_access.id,
+        name="audience-mapper",
         included_custom_audience="foo")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the client scope.
     :param str realm_id: The realm id.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,21 +164,22 @@
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     client = keycloak.openid.Client("client",
         realm_id=realm.id,
         client_id="client",
+        name="client",
         access_type="CONFIDENTIAL",
         service_accounts_enabled=True)
     service_account_user = keycloak.openid.get_client_service_account_user_output(realm_id=realm.id,
         client_id=client.id)
     offline_access = keycloak.get_role_output(realm_id=realm.id,
         name="offline_access")
-    service_account_user_roles = keycloak.UserRoles("serviceAccountUserRoles",
+    service_account_user_roles = keycloak.UserRoles("service_account_user_roles",
         realm_id=realm.id,
         user_id=service_account_user.id,
         role_ids=[offline_access.id])
     ```
     <!--End PulumiCodeChooser -->
 
 
@@ -227,21 +228,22 @@
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     client = keycloak.openid.Client("client",
         realm_id=realm.id,
         client_id="client",
+        name="client",
         access_type="CONFIDENTIAL",
         service_accounts_enabled=True)
     service_account_user = keycloak.openid.get_client_service_account_user_output(realm_id=realm.id,
         client_id=client.id)
     offline_access = keycloak.get_role_output(realm_id=realm.id,
         name="offline_access")
-    service_account_user_roles = keycloak.UserRoles("serviceAccountUserRoles",
+    service_account_user_roles = keycloak.UserRoles("service_account_user_roles",
         realm_id=realm.id,
         user_id=service_account_user.id,
         role_ids=[offline_access.id])
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,44 +303,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("groupMembershipMapper",
-            claim_name="groups",
+        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="group-membership-mapper",
+            claim_name="groups")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("groupMembershipMapper",
-            claim_name="groups",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="group-membership-mapper",
+            claim_name="groups")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -390,44 +395,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("groupMembershipMapper",
-            claim_name="groups",
+        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="group-membership-mapper",
+            claim_name="groups")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("groupMembershipMapper",
-            claim_name="groups",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="group-membership-mapper",
+            claim_name="groups")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,46 +359,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcodedClaimMapper",
-            claim_name="foo",
-            claim_value="bar",
+        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="hardcoded-claim-mapper",
+            claim_name="foo",
+            claim_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcodedClaimMapper",
-            claim_name="foo",
-            claim_value="bar",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="hardcoded-claim-mapper",
+            claim_name="foo",
+            claim_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -453,46 +458,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcodedClaimMapper",
-            claim_name="foo",
-            claim_value="bar",
+        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="hardcoded-claim-mapper",
+            claim_name="foo",
+            claim_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcodedClaimMapper",
-            claim_name="foo",
-            claim_value="bar",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="hardcoded-claim-mapper",
+            claim_name="foo",
+            claim_value="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,45 +203,54 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        role = keycloak.Role("role", realm_id=realm.id)
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        role = keycloak.Role("role",
+            realm_id=realm.id,
+            name="my-role")
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcodedRoleMapper",
-            client_id=openid_client.id,
+        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
+            client_id=openid_client.id,
+            name="hardcoded-role-mapper",
             role_id=role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        role = keycloak.Role("role", realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcodedRoleMapper",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        role = keycloak.Role("role",
             realm_id=realm.id,
+            name="my-role")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="hardcoded-role-mapper",
             role_id=role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
@@ -289,45 +298,54 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        role = keycloak.Role("role", realm_id=realm.id)
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        role = keycloak.Role("role",
+            realm_id=realm.id,
+            name="my-role")
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcodedRoleMapper",
-            client_id=openid_client.id,
+        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
+            client_id=openid_client.id,
+            name="hardcoded-role-mapper",
             role_id=role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        role = keycloak.Role("role", realm_id=realm.id)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcodedRoleMapper",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        role = keycloak.Role("role",
             realm_id=realm.id,
+            name="my-role")
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="hardcoded-role-mapper",
             role_id=role.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,23 +411,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        script_mapper = keycloak.openid.ScriptProtocolMapper("scriptMapper",
+        script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
@@ -435,18 +437,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        script_mapper = keycloak.openid.ScriptProtocolMapper("scriptMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -506,23 +511,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        script_mapper = keycloak.openid.ScriptProtocolMapper("scriptMapper",
+        script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
@@ -530,18 +537,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        script_mapper = keycloak.openid.ScriptProtocolMapper("scriptMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,46 +425,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("userAttributeMapper",
-            claim_name="bar",
-            client_id=openid_client.id,
+        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
-            user_attribute="foo")
+            client_id=openid_client.id,
+            name="test-mapper",
+            user_attribute="foo",
+            claim_name="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("userAttributeMapper",
-            claim_name="bar",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
-            user_attribute="foo")
+            name="test-client-scope")
+        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="test-mapper",
+            user_attribute="foo",
+            claim_name="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -522,46 +527,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("userAttributeMapper",
-            claim_name="bar",
-            client_id=openid_client.id,
+        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
-            user_attribute="foo")
+            client_id=openid_client.id,
+            name="test-mapper",
+            user_attribute="foo",
+            claim_name="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("userAttributeMapper",
-            claim_name="bar",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
-            user_attribute="foo")
+            name="test-client-scope")
+        user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="test-mapper",
+            user_attribute="foo",
+            claim_name="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,41 +443,46 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("userClientRoleMapper",
+        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="user-client-role-mapper",
             claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("userClientRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="user-client-role-mapper",
             claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
@@ -535,41 +540,46 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("userClientRoleMapper",
+        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="user-client-role-mapper",
             claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("userClientRoleMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="user-client-role-mapper",
             claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,46 +359,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("userPropertyMapper",
-            claim_name="email",
-            client_id=openid_client.id,
+        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
-            user_property="email")
+            client_id=openid_client.id,
+            name="test-mapper",
+            user_property="email",
+            claim_name="email")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("userPropertyMapper",
-            claim_name="email",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
-            user_property="email")
+            name="test-client-scope")
+        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="test-mapper",
+            user_property="email",
+            claim_name="email")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -453,46 +458,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("userPropertyMapper",
-            claim_name="email",
-            client_id=openid_client.id,
+        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
-            user_property="email")
+            client_id=openid_client.id,
+            name="test-mapper",
+            user_property="email",
+            claim_name="email")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("userPropertyMapper",
-            claim_name="email",
-            client_scope_id=client_scope.id,
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
-            user_property="email")
+            name="test-client-scope")
+        user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
+            realm_id=realm.id,
+            client_scope_id=client_scope.id,
+            name="test-mapper",
+            user_property="email",
+            claim_name="email")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,44 +401,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("userRealmRoleMapper",
-            claim_name="foo",
+        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="user-realm-role-mapper",
+            claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("userRealmRoleMapper",
-            claim_name="foo",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="user-realm-role-mapper",
+            claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -496,44 +501,49 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        openid_client = keycloak.openid.Client("openidClient",
-            access_type="CONFIDENTIAL",
+            realm="my-realm",
+            enabled=True)
+        openid_client = keycloak.openid.Client("openid_client",
+            realm_id=realm.id,
             client_id="test-client",
+            name="test client",
             enabled=True,
-            realm_id=realm.id,
+            access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("userRealmRoleMapper",
-            claim_name="foo",
+        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
+            realm_id=realm.id,
             client_id=openid_client.id,
-            realm_id=realm.id)
+            name="user-realm-role-mapper",
+            claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("userRealmRoleMapper",
-            claim_name="foo",
+            realm="my-realm",
+            enabled=True)
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="test-client-scope")
+        user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
+            realm_id=realm.id,
             client_scope_id=client_scope.id,
-            realm_id=realm.id)
+            name="user-realm-role-mapper",
+            claim_name="foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,23 +344,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("userSessionNoteMapper",
+        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("user_session_note_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
@@ -369,18 +371,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("userSessionNoteMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("user_session_note_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -437,23 +442,25 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        openid_client = keycloak.openid.Client("openidClient",
+        openid_client = keycloak.openid.Client("openid_client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
-        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("userSessionNoteMapper",
+        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("user_session_note_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
+            name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Client Scope)
@@ -462,18 +469,21 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        client_scope = keycloak.openid.ClientScope("clientScope", realm_id=realm.id)
-        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("userSessionNoteMapper",
+        client_scope = keycloak.openid.ClientScope("client_scope",
+            realm_id=realm.id,
+            name="client-scope")
+        user_session_note_mapper = keycloak.openid.UserSessionNoteProtocolMapper("user_session_note_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
+            name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,25 +216,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="test")
-        realm_events = keycloak.RealmEvents("realmEvents",
-            admin_events_details_enabled=True,
+        realm_events = keycloak.RealmEvents("realm_events",
+            realm_id=realm.id,
+            events_enabled=True,
+            events_expiration=3600,
             admin_events_enabled=True,
+            admin_events_details_enabled=True,
             enabled_event_types=[
                 "LOGIN",
                 "LOGOUT",
             ],
-            events_enabled=True,
-            events_expiration=3600,
-            events_listeners=["jboss-logging"],
-            realm_id=realm.id)
+            events_listeners=["jboss-logging"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -264,25 +264,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="test")
-        realm_events = keycloak.RealmEvents("realmEvents",
-            admin_events_details_enabled=True,
+        realm_events = keycloak.RealmEvents("realm_events",
+            realm_id=realm.id,
+            events_enabled=True,
+            events_expiration=3600,
             admin_events_enabled=True,
+            admin_events_details_enabled=True,
             enabled_event_types=[
                 "LOGIN",
                 "LOGOUT",
             ],
-            events_enabled=True,
-            events_expiration=3600,
-            events_listeners=["jboss-logging"],
-            realm_id=realm.id)
+            events_listeners=["jboss-logging"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystoreAesGenerated",
+        keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystore_aes_generated",
+            name="my-aes-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             secret_size=16)
         ```
         <!--End PulumiCodeChooser -->
@@ -288,15 +289,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystoreAesGenerated",
+        keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystore_aes_generated",
+            name="my-aes-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             secret_size=16)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystoreEcdsaGenerated",
+        keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystore_ecdsa_generated",
+            name="my-ecdsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             elliptic_curve_key="P-256")
         ```
         <!--End PulumiCodeChooser -->
@@ -288,15 +289,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystoreEcdsaGenerated",
+        keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystore_ecdsa_generated",
+            name="my-ecdsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             elliptic_curve_key="P-256")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystoreHmacGenerated",
+        keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystore_hmac_generated",
+            name="my-hmac-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="HS256",
             secret_size=64)
         ```
@@ -323,15 +324,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystoreHmacGenerated",
+        keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystore_hmac_generated",
+            name="my-hmac-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="HS256",
             secret_size=64)
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        java_keystore = keycloak.RealmKeystoreJavaGenerated("javaKeystore",
+        java_keystore = keycloak.RealmKeystoreJavaGenerated("java_keystore",
+            name="my-java-keystore",
             realm_id=realm.id,
             enabled=True,
             active=True,
             keystore="<path to your keystore>",
             keystore_password="<password for keystore>",
             key_alias="<alias for the private key>",
             key_password="<password for the private key>",
@@ -424,15 +425,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        java_keystore = keycloak.RealmKeystoreJavaGenerated("javaKeystore",
+        java_keystore = keycloak.RealmKeystoreJavaGenerated("java_keystore",
+            name="my-java-keystore",
             realm_id=realm.id,
             enabled=True,
             active=True,
             keystore="<path to your keystore>",
             keystore_password="<password for keystore>",
             key_alias="<alias for the private key>",
             key_password="<password for the private key>",
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystoreRsaGenerated",
+        keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystore_rsa_generated",
+            name="my-rsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="RS256",
             key_size=2048)
         ```
@@ -323,15 +324,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
-        keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystoreRsaGenerated",
+        keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystore_rsa_generated",
+            name="my-rsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="RS256",
             key_size=2048)
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             attributes={
                 "userProfileEnabled": True,
             })
         userprofile = keycloak.RealmUserProfile("userprofile",
-            realm_id=keycloak_realm["my_realm"]["id"],
+            realm_id=my_realm["id"],
             attributes=[
                 keycloak.RealmUserProfileAttributeArgs(
                     name="field1",
                     display_name="Field 1",
                     group="group1",
                     enabled_when_scopes=["offline_access"],
                     required_for_roles=["user"],
@@ -266,15 +266,15 @@
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             attributes={
                 "userProfileEnabled": True,
             })
         userprofile = keycloak.RealmUserProfile("userprofile",
-            realm_id=keycloak_realm["my_realm"]["id"],
+            realm_id=my_realm["id"],
             attributes=[
                 keycloak.RealmUserProfileAttributeArgs(
                     name="field1",
                     display_name="Field 1",
                     group="group1",
                     enabled_when_scopes=["offline_access"],
                     required_for_roles=["user"],
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/required_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,18 +240,19 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        required_action = keycloak.RequiredAction("requiredAction",
+        required_action = keycloak.RequiredAction("required_action",
             realm_id=realm.realm,
             alias="webauthn-register",
-            enabled=True)
+            enabled=True,
+            name="Webauthn Register")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realm}}/{{alias}}`.
 
@@ -289,18 +290,19 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        required_action = keycloak.RequiredAction("requiredAction",
+        required_action = keycloak.RequiredAction("required_action",
             realm_id=realm.realm,
             alias="webauthn-register",
-            enabled=True)
+            enabled=True,
+            name="Webauthn Register")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realm}}/{{alias}}`.
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/role.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/role.py`

 * *Files 11% similar despite different names*

```diff
@@ -194,76 +194,92 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        realm_role = keycloak.Role("realmRole",
-            description="My Realm Role",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role",
+            description="My Realm Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client role)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
+            realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Composite role)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        create_role = keycloak.Role("createRole", realm_id=realm.id)
-        read_role = keycloak.Role("readRole", realm_id=realm.id)
-        update_role = keycloak.Role("updateRole", realm_id=realm.id)
-        delete_role = keycloak.Role("deleteRole", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        # realm roles
+        create_role = keycloak.Role("create_role",
+            realm_id=realm.id,
+            name="create")
+        read_role = keycloak.Role("read_role",
+            realm_id=realm.id,
+            name="read")
+        update_role = keycloak.Role("update_role",
+            realm_id=realm.id,
+            name="update")
+        delete_role = keycloak.Role("delete_role",
+            realm_id=realm.id,
+            name="delete")
+        # client role
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
-        admin_role = keycloak.Role("adminRole",
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
+            realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
+        admin_role = keycloak.Role("admin_role",
+            realm_id=realm.id,
+            name="admin",
             composite_roles=[
                 "{keycloak_role.create_role.id}",
                 "{keycloak_role.read_role.id}",
                 "{keycloak_role.update_role.id}",
                 "{keycloak_role.delete_role.id}",
                 "{keycloak_role.client_role.id}",
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -306,76 +322,92 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        realm_role = keycloak.Role("realmRole",
-            description="My Realm Role",
-            realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        realm_role = keycloak.Role("realm_role",
+            realm_id=realm.id,
+            name="my-realm-role",
+            description="My Realm Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client role)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
+            realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage (Composite role)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        create_role = keycloak.Role("createRole", realm_id=realm.id)
-        read_role = keycloak.Role("readRole", realm_id=realm.id)
-        update_role = keycloak.Role("updateRole", realm_id=realm.id)
-        delete_role = keycloak.Role("deleteRole", realm_id=realm.id)
+            realm="my-realm",
+            enabled=True)
+        # realm roles
+        create_role = keycloak.Role("create_role",
+            realm_id=realm.id,
+            name="create")
+        read_role = keycloak.Role("read_role",
+            realm_id=realm.id,
+            name="read")
+        update_role = keycloak.Role("update_role",
+            realm_id=realm.id,
+            name="update")
+        delete_role = keycloak.Role("delete_role",
+            realm_id=realm.id,
+            name="delete")
+        # client role
         client = keycloak.openid.Client("client",
-            access_type="BEARER-ONLY",
+            realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
-            realm_id=realm.id)
-        client_role = keycloak.Role("clientRole",
-            client_id=keycloak_client["client"]["id"],
-            description="My Client Role",
-            realm_id=realm.id)
-        admin_role = keycloak.Role("adminRole",
+            access_type="BEARER-ONLY")
+        client_role = keycloak.Role("client_role",
+            realm_id=realm.id,
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
+            description="My Client Role")
+        admin_role = keycloak.Role("admin_role",
+            realm_id=realm.id,
+            name="admin",
             composite_roles=[
                 "{keycloak_role.create_role.id}",
                 "{keycloak_role.read_role.id}",
                 "{keycloak_role.update_role.id}",
                 "{keycloak_role.delete_role.id}",
                 "{keycloak_role.client_role.id}",
-            ],
-            realm_id=realm.id)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -924,65 +924,14 @@
 
         Allows for creating and managing Keycloak clients that use the SAML protocol.
 
         Clients are entities that can use Keycloak for user authentication. Typically,
         clients are applications that redirect users to Keycloak for authentication
         in order to take advantage of Keycloak's user sessions for SSO.
 
-        ### Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_keycloak as keycloak
-
-        realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
-            client_id="test-saml-client",
-            include_authn_statement=True,
-            realm_id=realm.id,
-            sign_assertions=True,
-            sign_documents=False,
-            signing_certificate=(lambda path: open(path).read())("saml-cert.pem"),
-            signing_private_key=(lambda path: open(path).read())("saml-key.pem"))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ### Argument Reference
-
-        The following arguments are supported:
-
-        - `realm_id` - (Required) The realm this client is attached to.
-        - `client_id` - (Required) The unique ID of this client, referenced in the URI during authentication and in issued tokens.
-        - `name` - (Optional) The display name of this client in the GUI.
-        - `enabled` - (Optional) When false, this client will not be able to initiate a login or obtain access tokens. Defaults to `true`.
-        - `description` - (Optional) The description of this client in the GUI.
-        - `include_authn_statement` - (Optional) When `true`, an `AuthnStatement` will be included in the SAML response.
-        - `sign_documents` - (Optional) When `true`, the SAML document will be signed by Keycloak using the realm's private key.
-        - `sign_assertions` - (Optional) When `true`, the SAML assertions will be signed by Keycloak using the realm's private key, and embedded within the SAML XML Auth response.
-        - `client_signature_required` - (Optional) When `true`, Keycloak will expect that documents originating from a client will be signed using the certificate and/or key configured via `signing_certificate` and `signing_private_key`.
-        - `force_post_binding` - (Optional) When `true`, Keycloak will always respond to an authentication request via the SAML POST Binding.
-        - `front_channel_logout` - (Optional) When `true`, this client will require a browser redirect in order to perform a logout.
-        - `name_id_format` - (Optional) Sets the Name ID format for the subject.
-        - `root_url` - (Optional) When specified, this value is prepended to all relative URLs.
-        - `valid_redirect_uris` - (Optional) When specified, Keycloak will use this list to validate given Assertion Consumer URLs specified in the authentication request.
-        - `base_url` - (Optional) When specified, this URL will be used whenever Keycloak needs to link to this client.
-        - `master_saml_processing_url` - (Optional) When specified, this URL will be used for all SAML requests.
-        - `signing_certificate` - (Optional) If documents or assertions from the client are signed, this certificate will be used to verify the signature.
-        - `signing_private_key` - (Optional) If documents or assertions from the client are signed, this private key will be used to verify the signature.
-        - `idp_initiated_sso_url_name` - (Optional) URL fragment name to reference client when you want to do IDP Initiated SSO.
-        - `idp_initiated_sso_relay_state` - (Optional) Relay state you want to send with SAML request when you want to do IDP Initiated SSO.
-        - `assertion_consumer_post_url` - (Optional) SAML POST Binding URL for the client's assertion consumer service (login responses).
-        - `assertion_consumer_redirect_url` - (Optional) SAML Redirect Binding URL for the client's assertion consumer service (login responses).
-        - `logout_service_post_binding_url` - (Optional) SAML POST Binding URL for the client's single logout service.
-        - `logout_service_redirect_binding_url` - (Optional) SAML Redirect Binding URL for the client's single logout service.
-        - `full_scope_allowed` - (Optional) - Allow to include all roles mappings in the access token
-
         ### Import
 
         Clients can be imported using the format `{{realm_id}}/{{client_keycloak_id}}`, where `client_keycloak_id` is the unique ID that Keycloak
         assigns to the client upon creation. This value can be found in the URI when editing this client in the GUI, and is typically a GUID.
 
         Example:
 
@@ -1000,65 +949,14 @@
 
         Allows for creating and managing Keycloak clients that use the SAML protocol.
 
         Clients are entities that can use Keycloak for user authentication. Typically,
         clients are applications that redirect users to Keycloak for authentication
         in order to take advantage of Keycloak's user sessions for SSO.
 
-        ### Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_keycloak as keycloak
-
-        realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
-            client_id="test-saml-client",
-            include_authn_statement=True,
-            realm_id=realm.id,
-            sign_assertions=True,
-            sign_documents=False,
-            signing_certificate=(lambda path: open(path).read())("saml-cert.pem"),
-            signing_private_key=(lambda path: open(path).read())("saml-key.pem"))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ### Argument Reference
-
-        The following arguments are supported:
-
-        - `realm_id` - (Required) The realm this client is attached to.
-        - `client_id` - (Required) The unique ID of this client, referenced in the URI during authentication and in issued tokens.
-        - `name` - (Optional) The display name of this client in the GUI.
-        - `enabled` - (Optional) When false, this client will not be able to initiate a login or obtain access tokens. Defaults to `true`.
-        - `description` - (Optional) The description of this client in the GUI.
-        - `include_authn_statement` - (Optional) When `true`, an `AuthnStatement` will be included in the SAML response.
-        - `sign_documents` - (Optional) When `true`, the SAML document will be signed by Keycloak using the realm's private key.
-        - `sign_assertions` - (Optional) When `true`, the SAML assertions will be signed by Keycloak using the realm's private key, and embedded within the SAML XML Auth response.
-        - `client_signature_required` - (Optional) When `true`, Keycloak will expect that documents originating from a client will be signed using the certificate and/or key configured via `signing_certificate` and `signing_private_key`.
-        - `force_post_binding` - (Optional) When `true`, Keycloak will always respond to an authentication request via the SAML POST Binding.
-        - `front_channel_logout` - (Optional) When `true`, this client will require a browser redirect in order to perform a logout.
-        - `name_id_format` - (Optional) Sets the Name ID format for the subject.
-        - `root_url` - (Optional) When specified, this value is prepended to all relative URLs.
-        - `valid_redirect_uris` - (Optional) When specified, Keycloak will use this list to validate given Assertion Consumer URLs specified in the authentication request.
-        - `base_url` - (Optional) When specified, this URL will be used whenever Keycloak needs to link to this client.
-        - `master_saml_processing_url` - (Optional) When specified, this URL will be used for all SAML requests.
-        - `signing_certificate` - (Optional) If documents or assertions from the client are signed, this certificate will be used to verify the signature.
-        - `signing_private_key` - (Optional) If documents or assertions from the client are signed, this private key will be used to verify the signature.
-        - `idp_initiated_sso_url_name` - (Optional) URL fragment name to reference client when you want to do IDP Initiated SSO.
-        - `idp_initiated_sso_relay_state` - (Optional) Relay state you want to send with SAML request when you want to do IDP Initiated SSO.
-        - `assertion_consumer_post_url` - (Optional) SAML POST Binding URL for the client's assertion consumer service (login responses).
-        - `assertion_consumer_redirect_url` - (Optional) SAML Redirect Binding URL for the client's assertion consumer service (login responses).
-        - `logout_service_post_binding_url` - (Optional) SAML POST Binding URL for the client's single logout service.
-        - `logout_service_redirect_binding_url` - (Optional) SAML Redirect Binding URL for the client's single logout service.
-        - `full_scope_allowed` - (Optional) - Allow to include all roles mappings in the access token
-
         ### Import
 
         Clients can be imported using the format `{{realm_id}}/{{client_keycloak_id}}`, where `client_keycloak_id` is the unique ID that Keycloak
         assigns to the client upon creation. This value can be found in the URI when editing this client in the GUI, and is typically a GUID.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,16 +208,17 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client_scope = keycloak.saml.ClientScope("samlClientScope",
+        saml_client_scope = keycloak.saml.ClientScope("saml_client_scope",
             realm_id=realm.id,
+            name="groups",
             description="This scope will map a user's group memberships to SAML assertion",
             gui_order=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -258,16 +259,17 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client_scope = keycloak.saml.ClientScope("samlClientScope",
+        saml_client_scope = keycloak.saml.ClientScope("saml_client_scope",
             realm_id=realm.id,
+            name="groups",
             description="This scope will map a user's group memberships to SAML assertion",
             gui_order=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,14 +398,15 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.saml.get_client(realm_id="my-realm",
         client_id="realm-management")
+    # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
     <!--End PulumiCodeChooser -->
 
 
@@ -472,14 +473,15 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.saml.get_client(realm_id="my-realm",
         client_id="realm-management")
+    # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1288,26 +1288,26 @@
         ### Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        realm_identity_provider = keycloak.saml.IdentityProvider("realmIdentityProvider",
+        realm_identity_provider = keycloak.saml.IdentityProvider("realm_identity_provider",
+            realm="my-realm",
             alias="my-idp",
+            single_sign_on_service_url="https://domain.com/adfs/ls/",
+            single_logout_service_url="https://domain.com/adfs/ls/?wa=wsignout1.0",
             backchannel_supported=True,
-            force_authn=True,
-            post_binding_authn_request=True,
-            post_binding_logout=True,
             post_binding_response=True,
-            realm="my-realm",
-            single_logout_service_url="https://domain.com/adfs/ls/?wa=wsignout1.0",
-            single_sign_on_service_url="https://domain.com/adfs/ls/",
+            post_binding_logout=True,
+            post_binding_authn_request=True,
             store_token=False,
-            trust_email=True)
+            trust_email=True,
+            force_authn=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -1407,26 +1407,26 @@
         ### Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
-        realm_identity_provider = keycloak.saml.IdentityProvider("realmIdentityProvider",
+        realm_identity_provider = keycloak.saml.IdentityProvider("realm_identity_provider",
+            realm="my-realm",
             alias="my-idp",
+            single_sign_on_service_url="https://domain.com/adfs/ls/",
+            single_logout_service_url="https://domain.com/adfs/ls/?wa=wsignout1.0",
             backchannel_supported=True,
-            force_authn=True,
-            post_binding_authn_request=True,
-            post_binding_logout=True,
             post_binding_response=True,
-            realm="my-realm",
-            single_logout_service_url="https://domain.com/adfs/ls/?wa=wsignout1.0",
-            single_sign_on_service_url="https://domain.com/adfs/ls/",
+            post_binding_logout=True,
+            post_binding_authn_request=True,
             store_token=False,
-            trust_email=True)
+            trust_email=True,
+            force_authn=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,20 +340,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client = keycloak.saml.Client("samlClient",
+        saml_client = keycloak.saml.Client("saml_client",
             realm_id=realm.id,
-            client_id="saml-client")
-        saml_script_mapper = keycloak.saml.ScriptProtocolMapper("samlScriptMapper",
+            client_id="saml-client",
+            name="saml-client")
+        saml_script_mapper = keycloak.saml.ScriptProtocolMapper("saml_script_mapper",
             realm_id=realm.id,
             client_id=saml_client.id,
+            name="script-mapper",
             script="exports = 'foo';",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -408,20 +410,22 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        saml_client = keycloak.saml.Client("samlClient",
+        saml_client = keycloak.saml.Client("saml_client",
             realm_id=realm.id,
-            client_id="saml-client")
-        saml_script_mapper = keycloak.saml.ScriptProtocolMapper("samlScriptMapper",
+            client_id="saml-client",
+            name="saml-client")
+        saml_script_mapper = keycloak.saml.ScriptProtocolMapper("saml_script_mapper",
             realm_id=realm.id,
             client_id=saml_client.id,
+            name="script-mapper",
             script="exports = 'foo';",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,25 +244,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=test["id"],
             client_id="test-saml-client",
-            realm_id=keycloak_realm["test"]["id"])
-        saml_user_attribute_mapper = keycloak.saml.UserAttributeProtocolMapper("samlUserAttributeMapper",
+            name="test-saml-client")
+        saml_user_attribute_mapper = keycloak.saml.UserAttributeProtocolMapper("saml_user_attribute_mapper",
+            realm_id=test["id"],
             client_id=saml_client.id,
-            realm_id=keycloak_realm["test"]["id"],
+            name="displayname-user-attribute-mapper",
+            user_attribute="displayName",
             saml_attribute_name="displayName",
-            saml_attribute_name_format="Unspecified",
-            user_attribute="displayName")
+            saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -307,25 +309,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=test["id"],
             client_id="test-saml-client",
-            realm_id=keycloak_realm["test"]["id"])
-        saml_user_attribute_mapper = keycloak.saml.UserAttributeProtocolMapper("samlUserAttributeMapper",
+            name="test-saml-client")
+        saml_user_attribute_mapper = keycloak.saml.UserAttributeProtocolMapper("saml_user_attribute_mapper",
+            realm_id=test["id"],
             client_id=saml_client.id,
-            realm_id=keycloak_realm["test"]["id"],
+            name="displayname-user-attribute-mapper",
+            user_attribute="displayName",
             saml_attribute_name="displayName",
-            saml_attribute_name_format="Unspecified",
-            user_attribute="displayName")
+            saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,25 +244,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=test["id"],
             client_id="test-saml-client",
-            realm_id=keycloak_realm["test"]["id"])
-        saml_user_property_mapper = keycloak.saml.UserPropertyProtocolMapper("samlUserPropertyMapper",
+            name="test-saml-client")
+        saml_user_property_mapper = keycloak.saml.UserPropertyProtocolMapper("saml_user_property_mapper",
+            realm_id=test["id"],
             client_id=saml_client.id,
-            realm_id=keycloak_realm["test"]["id"],
+            name="email-user-property-mapper",
+            user_property="email",
             saml_attribute_name="email",
-            saml_attribute_name_format="Unspecified",
-            user_property="email")
+            saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -307,25 +309,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
-        saml_client = keycloak.saml.Client("samlClient",
+            realm="my-realm",
+            enabled=True)
+        saml_client = keycloak.saml.Client("saml_client",
+            realm_id=test["id"],
             client_id="test-saml-client",
-            realm_id=keycloak_realm["test"]["id"])
-        saml_user_property_mapper = keycloak.saml.UserPropertyProtocolMapper("samlUserPropertyMapper",
+            name="test-saml-client")
+        saml_user_property_mapper = keycloak.saml.UserPropertyProtocolMapper("saml_user_property_mapper",
+            realm_id=test["id"],
             client_id=saml_client.id,
-            realm_id=keycloak_realm["test"]["id"],
+            name="email-user-property-mapper",
+            user_property="email",
             saml_attribute_name="email",
-            saml_attribute_name_format="Unspecified",
-            user_property="email")
+            saml_attribute_name_format="Unspecified")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,34 +321,34 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         user = keycloak.User("user",
-            email="bob@domain.com",
+            realm_id=realm.id,
+            username="bob",
             enabled=True,
+            email="bob@domain.com",
             first_name="Bob",
-            last_name="Bobson",
+            last_name="Bobson")
+        user_with_initial_password = keycloak.User("user_with_initial_password",
             realm_id=realm.id,
-            username="bob")
-        user_with_initial_password = keycloak.User("userWithInitialPassword",
-            email="alice@domain.com",
+            username="alice",
             enabled=True,
+            email="alice@domain.com",
             first_name="Alice",
+            last_name="Aliceberg",
             initial_password=keycloak.UserInitialPasswordArgs(
-                temporary=True,
                 value="some password",
-            ),
-            last_name="Aliceberg",
-            realm_id=realm.id,
-            username="alice")
+                temporary=True,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
@@ -392,34 +392,34 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
-            enabled=True,
-            realm="my-realm")
+            realm="my-realm",
+            enabled=True)
         user = keycloak.User("user",
-            email="bob@domain.com",
+            realm_id=realm.id,
+            username="bob",
             enabled=True,
+            email="bob@domain.com",
             first_name="Bob",
-            last_name="Bobson",
+            last_name="Bobson")
+        user_with_initial_password = keycloak.User("user_with_initial_password",
             realm_id=realm.id,
-            username="bob")
-        user_with_initial_password = keycloak.User("userWithInitialPassword",
-            email="alice@domain.com",
+            username="alice",
             enabled=True,
+            email="alice@domain.com",
             first_name="Alice",
+            last_name="Aliceberg",
             initial_password=keycloak.UserInitialPasswordArgs(
-                temporary=True,
                 value="some password",
-            ),
-            last_name="Aliceberg",
-            realm_id=realm.id,
-            username="alice")
+                temporary=True,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -175,58 +175,27 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        group = keycloak.Group("group", realm_id=realm.id)
-        user = keycloak.User("user",
-            realm_id=realm.id,
-            username="my-user")
-        user_groups = keycloak.UserGroups("userGroups",
+        group = keycloak.Group("group",
             realm_id=realm.id,
-            user_id=user.id,
-            group_ids=[group.id])
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ### Non Exhaustive Groups)
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_keycloak as keycloak
-
-        realm = keycloak.Realm("realm",
-            realm="my-realm",
-            enabled=True)
-        group_foo = keycloak.Group("groupFoo", realm_id=realm.id)
-        group_bar = keycloak.Group("groupBar", realm_id=realm.id)
+            name="foo")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="my-user")
-        user_groups_association1_user_groups = keycloak.UserGroups("userGroupsAssociation1UserGroups",
+        user_groups = keycloak.UserGroups("user_groups",
             realm_id=realm.id,
             user_id=user.id,
-            exhaustive=False,
-            group_ids=[group_foo.id])
-        user_groups_association1_index_user_groups_user_groups = keycloak.UserGroups("userGroupsAssociation1Index/userGroupsUserGroups",
-            realm_id=realm.id,
-            user_id=user.id,
-            exhaustive=False,
-            group_ids=[group_bar.id])
+            group_ids=[group.id])
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        This resource does not support import. Instead of importing, feel free to create this resource
-
-        as if it did not already exist on the server.
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] exhaustive: Indicates if the list of the user's groups is exhaustive. In this case, groups that are manually added to the user will be removed. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] group_ids: A list of group IDs that the user is member of.
         :param pulumi.Input[str] realm_id: The realm this group exists in.
         :param pulumi.Input[str] user_id: The ID of the user this resource should manage groups for.
         """
@@ -249,58 +218,27 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        group = keycloak.Group("group", realm_id=realm.id)
-        user = keycloak.User("user",
-            realm_id=realm.id,
-            username="my-user")
-        user_groups = keycloak.UserGroups("userGroups",
+        group = keycloak.Group("group",
             realm_id=realm.id,
-            user_id=user.id,
-            group_ids=[group.id])
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ### Non Exhaustive Groups)
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_keycloak as keycloak
-
-        realm = keycloak.Realm("realm",
-            realm="my-realm",
-            enabled=True)
-        group_foo = keycloak.Group("groupFoo", realm_id=realm.id)
-        group_bar = keycloak.Group("groupBar", realm_id=realm.id)
+            name="foo")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="my-user")
-        user_groups_association1_user_groups = keycloak.UserGroups("userGroupsAssociation1UserGroups",
+        user_groups = keycloak.UserGroups("user_groups",
             realm_id=realm.id,
             user_id=user.id,
-            exhaustive=False,
-            group_ids=[group_foo.id])
-        user_groups_association1_index_user_groups_user_groups = keycloak.UserGroups("userGroupsAssociation1Index/userGroupsUserGroups",
-            realm_id=realm.id,
-            user_id=user.id,
-            exhaustive=False,
-            group_ids=[group_bar.id])
+            group_ids=[group.id])
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        This resource does not support import. Instead of importing, feel free to create this resource
-
-        as if it did not already exist on the server.
-
         :param str resource_name: The name of the resource.
         :param UserGroupsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(UserGroupsArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,34 +180,37 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
-            client_id=keycloak_client["client"]["id"],
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
             description="My Client Role")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="bob",
             enabled=True,
             email="bob@domain.com",
             first_name="Bob",
             last_name="Bobson")
-        user_roles = keycloak.UserRoles("userRoles",
+        user_roles = keycloak.UserRoles("user_roles",
             realm_id=realm.id,
             user_id=user.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
@@ -258,34 +261,37 @@
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
-        realm_role = keycloak.Role("realmRole",
+        realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
+            name="my-realm-role",
             description="My Realm Role")
         client = keycloak.openid.Client("client",
             realm_id=realm.id,
             client_id="client",
+            name="client",
             enabled=True,
             access_type="BEARER-ONLY")
-        client_role = keycloak.Role("clientRole",
+        client_role = keycloak.Role("client_role",
             realm_id=realm.id,
-            client_id=keycloak_client["client"]["id"],
+            client_id=client_keycloak_client["id"],
+            name="my-client-role",
             description="My Client Role")
         user = keycloak.User("user",
             realm_id=realm.id,
             username="bob",
             enabled=True,
             email="bob@domain.com",
             first_name="Bob",
             last_name="Bobson")
-        user_roles = keycloak.UserRoles("userRoles",
+        user_roles = keycloak.UserRoles("user_roles",
             realm_id=realm.id,
             user_id=user.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,16 +219,17 @@
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        username_importer = keycloak.UserTemplateImporterIdentityProviderMapper("usernameImporter",
+        username_importer = keycloak.UserTemplateImporterIdentityProviderMapper("username_importer",
             realm=realm.id,
+            name="username-template-importer",
             identity_provider_alias=oidc.alias,
             template="${ALIAS}.${CLAIM.email}",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
         <!--End PulumiCodeChooser -->
@@ -284,16 +285,17 @@
             realm=realm.id,
             alias="oidc",
             authorization_url="https://example.com/auth",
             token_url="https://example.com/token",
             client_id="example_id",
             client_secret="example_token",
             default_scopes="openid random profile")
-        username_importer = keycloak.UserTemplateImporterIdentityProviderMapper("usernameImporter",
+        username_importer = keycloak.UserTemplateImporterIdentityProviderMapper("username_importer",
             realm=realm.id,
+            name="username-template-importer",
             identity_provider_alias=oidc.alias,
             template="${ALIAS}.${CLAIM.email}",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1713332823
+Version: 5.4.0a1713461881
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1713332823/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713332823/pyproject.toml` & `pulumi_keycloak-5.4.0a1713461881/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_keycloak"
   description = "A Pulumi package for creating and managing keycloak cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "keycloak"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.4.0a1713332823"
+  version = "5.4.0a1713461881"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-keycloak"
 
 [build-system]
```

